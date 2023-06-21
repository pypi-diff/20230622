# Comparing `tmp/libretrofuzz-3.3.0.tar.gz` & `tmp/libretrofuzz-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.3.0.tar", max compression
+gzip compressed data, was "libretrofuzz-3.3.1.tar", max compression
```

## Comparing `libretrofuzz-3.3.0.tar` & `libretrofuzz-3.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-21 16:17:18.247891 libretrofuzz-3.3.0/LICENSE
--rw-r--r--   0        0        0     7554 2023-06-21 16:17:18.247891 libretrofuzz-3.3.0/README.rst
--rw-r--r--   0        0        0       22 2023-06-21 16:17:18.247891 libretrofuzz-3.3.0/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    56529 2023-06-21 16:17:18.251891 libretrofuzz-3.3.0/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-21 16:17:18.251891 libretrofuzz-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     8735 2023-06-21 16:17:27.613899 libretrofuzz-3.3.0/setup.py
--rw-r--r--   0        0        0     8743 2023-06-21 16:17:27.615116 libretrofuzz-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-21 20:40:39.374696 libretrofuzz-3.3.1/LICENSE
+-rw-r--r--   0        0        0     7554 2023-06-21 20:40:39.374696 libretrofuzz-3.3.1/README.rst
+-rw-r--r--   0        0        0       22 2023-06-21 20:40:39.374696 libretrofuzz-3.3.1/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    56497 2023-06-21 20:40:39.374696 libretrofuzz-3.3.1/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-21 20:40:39.374696 libretrofuzz-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8735 2023-06-21 20:40:49.232031 libretrofuzz-3.3.1/setup.py
+-rw-r--r--   0        0        0     8743 2023-06-21 20:40:49.232984 libretrofuzz-3.3.1/PKG-INFO
```

### Comparing `libretrofuzz-3.3.0/LICENSE` & `libretrofuzz-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.3.0/README.rst` & `libretrofuzz-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.3.0/libretrofuzz/__main__.py` & `libretrofuzz-3.3.1/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # have the same system.
 
 from pathlib import Path
 from typing import Optional, List
 from urllib.request import unquote, quote
 from tempfile import TemporaryDirectory
 from contextlib import asynccontextmanager, contextmanager
-from itertools import chain, tee
+from itertools import chain
 from struct import unpack
 import json
 import os
 import sys
 import io
 import zlib
 import fnmatch
@@ -301,34 +301,34 @@
 class TitleScorer(object):
     def __init__(self, normcache, normcache2, hack):
         self.normcache = normcache
         self.normcache2 = normcache2
         self.hack = hack
 
     def __call__(self, name, other, score_cutoff=None):
-        if name == other:
-            return MAX_SCORE
-        (_, name_ns, _, _, digits) = self.normcache[name]
-        (_, other_ns, _, other_ns_subs, other_digits) = self.normcache2[other]
-        if name_ns == other_ns:
+        (name, name_ns, _, _, digits) = self.normcache[name]
+        (other, other_ns, _, other_ns_subs, other_digits) = self.normcache2[other]
+        if name == other or name_ns == other_ns:
             return MAX_SCORE
 
         remaining = MAX_SCORE - DEF_SCORE
 
         cnbrs = fuzz.ratio(digits, other_digits)  # normalized to 0-100
         # 2 heuristics (this time), however they don't both have the same weight
         increment_common_number = remaining * 0.03
         increment_common_length = remaining * 0.97
 
         sum_ns = ""
         for sub_ns in other_ns_subs:
             # if you find a exact match on either a subtitle
             # or a sequence of subtitles from the start, give
             # a 'winning' score but distingish them by the rest
-            # by name ratio and digits ratio
+            # by name ratio and digits ratio; note that this
+            # doesn't include subtitles in 'name' matching a
+            # subtitle in 'other', that's full of false positives
             if name_ns == (sum_ns := sum_ns + sub_ns) or name_ns == sub_ns:
                 # reset increment and rest of score
                 rest_of_score = increment_common_number * 0.01 * cnbrs
                 rest_of_score += increment_common_length * 0.01 * fuzz.WRatio(name, other)
                 return DEF_SCORE + rest_of_score
 
         rest_of_score = increment_common_number * 0.01 * cnbrs  # 100 gives 1
@@ -1045,58 +1045,51 @@
     # (until you call again without --no-merge anyway
     # or if they have the same score)
     remote_names = set()
     remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
     if not remote_names:
         raise StopPlaylist()
 
-    # build the function that will be called to print data
-    short_names = os.getenv("SHORT")
-    short_names = True if short_names and short_names != "0" else False
-
-    def strfy_runtime(s, urldict=None):
-        return strfy(score, short_names, nub_verbose, s, urldict)
-
     # preprocess data to build a heuristic later. Do not move
     # into the later loop because thats when the heuristic is used
     def norm(n):
         return normalizer(nometa, hack, n)
 
     def norm_local(n):
         return norm(regex.sub(forbidden, "_", extractbefore(before, n)))
 
-    a, b = tee(map(norm_local, names))
-    # store normalized local name as key
-    normcache = {t[0]: t for t in a}
-    # store the actual local name as key (cache)
-    normcache.update(zip(names, b))
-    # remote names normalization and cache
-    a, b = tee(map(norm, remote_names))
-    # store normalized remote name as key
-    normcache2 = {t[0]: t for t in a}
-    # remote name as key, normalized remote name as value
-    remote_names = {x: t[0] for x, t in zip(remote_names, b)}
+    # local names normalization cache
+    normcache = dict(zip(names, map(norm_local, names)))
+    # remote names normalization cache
+    normcache2 = dict(zip(remote_names, map(norm, remote_names)))
+
+    # short names bool, got from enviromental variable
+    short_names = os.getenv("SHORT")
+    short_names = True if short_names and short_names != "0" else False
+
+    # build the function that will be called to print data
+    def strfy_runtime(s, urldict=None):
+        return strfy(normcache2, score, short_names, nub_verbose, s, urldict)
+
     scorer = TitleScorer(normcache, normcache2, hack)
     for name, destination in zip(names, dbs):
         await asyncio.sleep(0)  # update key status
         checkEscape()  # check key status
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
-        # cached normalized name
-        nameaux = normcache[name][0]
         # normalization can make it so that the winner has the same score as the runner up(s)
         # so try in several versions (to prevent this use '--verbose 1')
         # improves results because spaces or case errors happen in the server
-        result = process.extract(nameaux, remote_names, scorer=scorer, limit=verbose or 2)
+        result = process.extract(name, remote_names, scorer=scorer, limit=verbose or 2)
         assert result
-        _, max_score, _ = result[0]
-        winners = [x for x in result if x[1] == max_score and x[1] >= score]
+        _, best_score, _ = result[0]
+        winners = [x for x in result if x[1] == best_score and x[1] >= score]
         show = result if verbose else winners
-        name_format = style((nameaux if short_names else name) + ": ", bold=True)
+        name_format = style((normcache[name][0] if short_names else name) + ": ", bold=True)
         # still remove the forbidden characters
         # the name will be used in the filename
         name = regex.sub(forbidden, "_", name)
         # Delete old images in the case of --filter.
         # this always happens, for consistency
         if filters and not dryrun:
             for dirname in Thumbs._fields:
@@ -1113,15 +1106,19 @@
                 missing_thumbs = 0
                 served__thumbs = False
                 for dirname in Thumbs._fields:
                     real = Path(real_thumb_dir, dirname, name + ".png")
                     if not real.exists():
                         missing_thumbs += 1
                         if not served__thumbs:
-                            served__thumbs = any(map(lambda x: x[2] in getattr(thumbs, dirname), winners))
+
+                            def checkremote(winner):
+                                return winner[0] in getattr(thumbs, dirname)
+
+                            served__thumbs = any(map(checkremote, winners))
                 allow = missing_thumbs == 3
                 # despite the above, print only for when it would download
                 # if it was allowed, otherwise it is confusing
                 if not allow and served__thumbs:
                     name_format = name_format + ", ".join((strfy_runtime(x) for x in show))
                     nomerge_format = f'{style("Nomerge",     fg=(128,128,128), bold=True)}: {name_format}'
                     echo(nomerge_format)
@@ -1143,15 +1140,15 @@
                 )
                 try:
                     for dirname in Thumbs._fields:
                         real = Path(real_thumb_dir, dirname, name + ".png")
                         temp = Path(down_thumb_dir, dirname, name + ".png")
                         downloaded_dict[dirname] = (real, temp)
                         for winner in winners:
-                            _, t_score, t_name = winner
+                            t_name, t_score, _ = winner
                             # something to download
                             url = getattr(thumbs, dirname).get(t_name, None)
                             if not url:
                                 continue
 
                             # with filters/reset you always download, and
                             # without only if it doesn't exist already.
@@ -1205,25 +1202,26 @@
     count = int(wait / 0.1)
     with handleContinueDownload():
         for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, leave=False):
             checkDownload()
             await asyncio.sleep(0.1)
 
 
-def strfy(required_score, short_names, nub_verbose, r, urlsdict=None):
-    thumb_norm, thumb_score, thumb_name = r
+def strfy(norm_cache, required_score, short_names, nub_verbose, r, urlsdict=None):
+    thumb_name, thumb_score, _ = r
+    thumb_norm = norm_cache[thumb_name][0]
     score_color = RED if thumb_score < required_score else GREEN
     thumb_magnt = f"{thumb_score:.4f}" if short_names else f"{thumb_score:.1f}"
     score_text = style(thumb_magnt, fg=score_color, bold=True)
     if nub_verbose:
         return f"{score_text} {thumb_norm}"
     elif urlsdict:
-        url1 = urlsdict.get((Thumbs._fields[0], r), None)
-        url2 = urlsdict.get((Thumbs._fields[1], r), None)
-        url3 = urlsdict.get((Thumbs._fields[2], r), None)
+        url1 = urlsdict.get(("Named_Boxarts", r), None)
+        url2 = urlsdict.get(("Named_Titles", r), None)
+        url3 = urlsdict.get(("Named_Snaps", r), None)
     else:
         url1 = None
         url2 = None
         url3 = None
     thumb_text = thumb_norm if short_names else thumb_name
     linked1 = link(url1, "🎴") if url1 else ""
     linked2 = link(url2, "🎬") if url2 else ""
```

### Comparing `libretrofuzz-3.3.0/pyproject.toml` & `libretrofuzz-3.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.3.0"
+version = "3.3.1"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.3.0/setup.py` & `libretrofuzz-3.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.3.0',
+    'version': '3.3.1',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.\n\nIf you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 15 --delay-after 15`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use ``--min 100``.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nA common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload because the glob used matches all names that start with 'Ishar' or 'ishar'.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.\n                        | [default: 90; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no delay or image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-3.3.0/PKG-INFO` & `libretrofuzz-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.3.0
+Version: 3.3.1
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

