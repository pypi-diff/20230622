# Comparing `tmp/libretrofuzz-3.3.2.tar.gz` & `tmp/libretrofuzz-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.3.2.tar", max compression
+gzip compressed data, was "libretrofuzz-3.3.3.tar", max compression
```

## Comparing `libretrofuzz-3.3.2.tar` & `libretrofuzz-3.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-21 23:42:49.633411 libretrofuzz-3.3.2/LICENSE
--rw-r--r--   0        0        0     7554 2023-06-21 23:42:49.633411 libretrofuzz-3.3.2/README.rst
--rw-r--r--   0        0        0       22 2023-06-21 23:42:49.633411 libretrofuzz-3.3.2/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    56507 2023-06-21 23:42:49.633411 libretrofuzz-3.3.2/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-21 23:42:49.633411 libretrofuzz-3.3.2/pyproject.toml
--rw-r--r--   0        0        0     8735 2023-06-21 23:42:58.982224 libretrofuzz-3.3.2/setup.py
--rw-r--r--   0        0        0     8743 2023-06-21 23:42:58.983201 libretrofuzz-3.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-22 04:05:13.362689 libretrofuzz-3.3.3/LICENSE
+-rw-r--r--   0        0        0     7554 2023-06-22 04:05:13.362689 libretrofuzz-3.3.3/README.rst
+-rw-r--r--   0        0        0       22 2023-06-22 04:05:13.362689 libretrofuzz-3.3.3/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    56511 2023-06-22 04:05:13.366689 libretrofuzz-3.3.3/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-22 04:05:13.366689 libretrofuzz-3.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8735 2023-06-22 04:05:23.446710 libretrofuzz-3.3.3/setup.py
+-rw-r--r--   0        0        0     8743 2023-06-22 04:05:23.447914 libretrofuzz-3.3.3/PKG-INFO
```

### Comparing `libretrofuzz-3.3.2/LICENSE` & `libretrofuzz-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.3.2/README.rst` & `libretrofuzz-3.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.3.2/libretrofuzz/__main__.py` & `libretrofuzz-3.3.3/libretrofuzz/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1054,17 +1054,17 @@
     def norm(n):
         return normalizer(nometa, hack, n)
 
     def norm_local(n):
         return norm(regex.sub(forbidden, "_", extractbefore(before, n)))
 
     # local names normalization cache
-    normcache = dict(zip(names, map(norm_local, names)))
+    normcache = dict(map(lambda n: (n, norm_local(n)), names))
     # remote names normalization cache
-    normcache2 = dict(zip(remote_names, map(norm, remote_names)))
+    normcache2 = dict(map(lambda n: (n, norm(n)), remote_names))
 
     # short names bool, got from enviromental variable
     short_names = os.getenv("SHORT")
     short_names = True if short_names and short_names != "0" else False
 
     # build the function that will be called to print data
     def strfy_runtime(s, urldict=None):
@@ -1075,15 +1075,15 @@
         await asyncio.sleep(0)  # update key status
         checkEscape()  # check key status
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
         # normalization can make it so that the winner has the same score as the runner up(s)
         # so enabling 'verbose 2+' can improve results if the server is badly organized
-        # however, don not do it by default, since it's a bit confusing.
+        # however, do not do it by default, since it's a bit confusing.
         result = process.extract(name, remote_names, scorer=scorer, limit=verbose or 1)
         assert result
         _, best_score, _ = result[0]
         winners = [x for x in result if x[1] == best_score and x[1] >= score]
         show = result if verbose else winners
         name_format = style((normcache[name][0] if short_names else name) + ": ", bold=True)
         # still remove the forbidden characters
```

### Comparing `libretrofuzz-3.3.2/pyproject.toml` & `libretrofuzz-3.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.3.2"
+version = "3.3.3"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.3.2/setup.py` & `libretrofuzz-3.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.3.2',
+    'version': '3.3.3',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.\n\nIf you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 15 --delay-after 15`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use ``--min 100``.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nA common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload because the glob used matches all names that start with 'Ishar' or 'ishar'.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.\n                        | [default: 90; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no delay or image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-3.3.2/PKG-INFO` & `libretrofuzz-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.3.2
+Version: 3.3.3
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

