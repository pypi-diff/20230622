# Comparing `tmp/mandown-1.4.0.tar.gz` & `tmp/mandown-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mandown-1.4.0.tar", max compression
+gzip compressed data, was "mandown-1.5.0.tar", max compression
```

## Comparing `mandown-1.4.0.tar` & `mandown-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    34520 2023-04-28 17:41:44.184635 mandown-1.4.0/LICENSE
--rw-r--r--   0        0        0     3845 2023-06-21 03:20:51.716586 mandown-1.4.0/README.md
--rw-r--r--   0        0        0      523 2023-04-28 17:41:44.918635 mandown-1.4.0/mandown/__init__.py
--rw-r--r--   0        0        0    11958 2023-06-21 02:16:52.907651 mandown-1.4.0/mandown/api.py
--rw-r--r--   0        0        0     1700 2023-04-28 17:41:44.917635 mandown-1.4.0/mandown/base.py
--rw-r--r--   0        0        0    16688 2023-06-20 22:27:01.443946 mandown-1.4.0/mandown/cli.py
--rw-r--r--   0        0        0     2564 2023-04-28 17:41:44.917635 mandown-1.4.0/mandown/comic.py
--rw-r--r--   0        0        0      682 2023-06-20 22:05:26.357720 mandown-1.4.0/mandown/convert_utils.py
--rw-r--r--   0        0        0     5549 2023-04-28 17:41:44.918635 mandown-1.4.0/mandown/io.py
--rw-r--r--   0        0        0     5102 2023-04-28 17:41:44.926635 mandown-1.4.0/mandown/processor/__init__.py
--rw-r--r--   0        0        0     4109 2023-04-28 17:41:44.926635 mandown-1.4.0/mandown/processor/ops.py
--rw-r--r--   0        0        0     1603 2023-04-28 17:41:44.926635 mandown-1.4.0/mandown/processor/profiles.py
--rw-r--r--   0        0        0     1449 2023-06-21 02:53:38.485548 mandown-1.4.0/mandown/sources/__init__.py
--rw-r--r--   0        0        0     2017 2023-04-28 17:41:44.919635 mandown-1.4.0/mandown/sources/base_source.py
--rw-r--r--   0        0        0     4938 2023-04-28 17:41:44.919635 mandown-1.4.0/mandown/sources/source_mangadex.py
--rw-r--r--   0        0        0     2569 2023-06-21 02:59:09.077067 mandown-1.4.0/mandown/sources/source_mangakakalot.py
--rw-r--r--   0        0        0     2697 2023-04-28 17:41:44.920635 mandown-1.4.0/mandown/sources/source_manganato.py
--rw-r--r--   0        0        0     3744 2023-04-28 17:41:44.920635 mandown-1.4.0/mandown/sources/source_mangasee.py
--rw-r--r--   0        0        0     3051 2023-06-21 02:58:11.800715 mandown-1.4.0/mandown/sources/source_manhuaes.py
--rw-r--r--   0        0        0     3599 2023-06-21 02:59:45.366868 mandown-1.4.0/mandown/sources/source_readcomiconline.py
--rw-r--r--   0        0        0     4116 2023-04-28 17:41:44.920635 mandown-1.4.0/mandown/sources/source_webtoons.py
--rw-r--r--   0        0        0     4597 2023-04-28 17:41:44.928635 mandown-1.4.0/mandown/ui/form.ui
--rw-r--r--   0        0        0     7214 2023-04-28 17:41:44.928635 mandown-1.4.0/mandown/ui/mainwin.py
--rw-r--r--   0        0        0       38 2023-04-28 17:41:44.928635 mandown-1.4.0/mandown/ui/mandown-qt.pyproject
--rw-r--r--   0        0        0     7049 2023-04-28 17:41:44.928635 mandown-1.4.0/mandown/ui/ui.py
--rw-r--r--   0        0        0     1398 2023-06-21 03:26:10.118172 mandown-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5073 1970-01-01 00:00:00.000000 mandown-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:44.184635 mandown-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3876 2023-06-22 00:53:19.395438 mandown-1.5.0/README.md
+-rw-r--r--   0        0        0      523 2023-04-28 17:41:44.918635 mandown-1.5.0/mandown/__init__.py
+-rw-r--r--   0        0        0    11958 2023-06-21 02:16:52.907651 mandown-1.5.0/mandown/api.py
+-rw-r--r--   0        0        0     1700 2023-04-28 17:41:44.917635 mandown-1.5.0/mandown/base.py
+-rw-r--r--   0        0        0    17292 2023-06-22 01:19:59.487322 mandown-1.5.0/mandown/cli.py
+-rw-r--r--   0        0        0     2564 2023-04-28 17:41:44.917635 mandown-1.5.0/mandown/comic.py
+-rw-r--r--   0        0        0      700 2023-06-22 00:52:39.390941 mandown-1.5.0/mandown/convert_utils.py
+-rw-r--r--   0        0        0     5549 2023-04-28 17:41:44.918635 mandown-1.5.0/mandown/io.py
+-rw-r--r--   0        0        0     5102 2023-04-28 17:41:44.926635 mandown-1.5.0/mandown/processor/__init__.py
+-rw-r--r--   0        0        0     4109 2023-04-28 17:41:44.926635 mandown-1.5.0/mandown/processor/ops.py
+-rw-r--r--   0        0        0     1603 2023-04-28 17:41:44.926635 mandown-1.5.0/mandown/processor/profiles.py
+-rw-r--r--   0        0        0     1449 2023-06-21 02:53:38.485548 mandown-1.5.0/mandown/sources/__init__.py
+-rw-r--r--   0        0        0     2017 2023-04-28 17:41:44.919635 mandown-1.5.0/mandown/sources/base_source.py
+-rw-r--r--   0        0        0     4938 2023-04-28 17:41:44.919635 mandown-1.5.0/mandown/sources/source_mangadex.py
+-rw-r--r--   0        0        0     2569 2023-06-21 02:59:09.077067 mandown-1.5.0/mandown/sources/source_mangakakalot.py
+-rw-r--r--   0        0        0     2697 2023-04-28 17:41:44.920635 mandown-1.5.0/mandown/sources/source_manganato.py
+-rw-r--r--   0        0        0     3744 2023-04-28 17:41:44.920635 mandown-1.5.0/mandown/sources/source_mangasee.py
+-rw-r--r--   0        0        0     3051 2023-06-21 02:58:11.800715 mandown-1.5.0/mandown/sources/source_manhuaes.py
+-rw-r--r--   0        0        0     3599 2023-06-21 02:59:45.366868 mandown-1.5.0/mandown/sources/source_readcomiconline.py
+-rw-r--r--   0        0        0     4116 2023-04-28 17:41:44.920635 mandown-1.5.0/mandown/sources/source_webtoons.py
+-rw-r--r--   0        0        0     4597 2023-04-28 17:41:44.928635 mandown-1.5.0/mandown/ui/form.ui
+-rw-r--r--   0        0        0     7214 2023-04-28 17:41:44.928635 mandown-1.5.0/mandown/ui/mainwin.py
+-rw-r--r--   0        0        0       38 2023-04-28 17:41:44.928635 mandown-1.5.0/mandown/ui/mandown-qt.pyproject
+-rw-r--r--   0        0        0     7049 2023-04-28 17:41:44.928635 mandown-1.5.0/mandown/ui/ui.py
+-rw-r--r--   0        0        0     1403 2023-06-22 01:45:37.914981 mandown-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 mandown-1.5.0/PKG-INFO
```

### Comparing `mandown-1.4.0/LICENSE` & `mandown-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/README.md` & `mandown-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Download from PyPI](https://img.shields.io/pypi/v/mandown)](https://pypi.org/project/mandown)
 [![Download from the AUR](https://img.shields.io/aur/version/mandown-git)](https://aur.archlinux.org/packages/mandown-git)
 [![Latest release](https://img.shields.io/github/v/release/potatoeggy/mandown?display_name=tag)](https://github.com/potatoeggy/mandown/releases/latest)
 [![License](https://img.shields.io/github/license/potatoeggy/mandown)](/LICENSE)
 
-Mandown is a comic downloader and a CBZ, EPUB, and/or PDF converter. It also supports image post-processing to make them more readable on certain devices similarly to [Kindle Comic Converter](https://github.com/ciromattia/kcc).
+Mandown is a comic downloader and a CBZ, EPUB, MOBI, and/or PDF converter. It also supports image post-processing to make them more readable on certain devices similarly to [Kindle Comic Converter](https://github.com/ciromattia/kcc).
 
 ## Features
 
 - Download comics from [supported sites](#supported-sites)
   - Supports downloading a range of chapters
   - Supports multithreaded downloading
 - Process downloaded images
   - Rotate or split double-page spreads
   - Trim borders
   - Resize images
-- Convert downloaded comics to CBZ, EPUB, or PDF
-  - Convert any other CBZ, EPUB, or PDF comic to CBZ, EPUB, or PDF
+- Convert downloaded comics to CBZ, EPUB, MOBI, or PDF
+  - Convert any other CBZ, EPUB, MOBI, or PDF comic to CBZ, EPUB, MOBI, or PDF
 - [A library to easily do all of this from other Python scripts](#basic-library-usage)
 
 ## Usage
 
 Run `mandown --help` or see the [docs](/docs/) for more information and examples.
 
 ```
 mandown get <URL>
 ```
 
-To convert the download contents to CBZ/EPUB/PDF, append the `--convert` option. To apply image processing to the downloaded images, append the `--process` option.
+To convert the downloaded contents to CBZ/EPUB/MOBI/PDF, append the `--convert` option. To apply image processing to the downloaded images, append the `--process` option.
 
 ```
 mandown get <URL> --convert epub --process rotate_double_pages
 ```
 
 To download only a certain range of chapters, append the `--start` and/or `--end` options.
```

### Comparing `mandown-1.4.0/mandown/__init__.py` & `mandown-1.5.0/mandown/__init__.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/api.py` & `mandown-1.5.0/mandown/api.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/base.py` & `mandown-1.5.0/mandown/base.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/cli.py` & `mandown-1.5.0/mandown/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,44 +159,60 @@
 ) -> None:
     iterator = api.convert_progress(
         comic_path, target_format, dest_folder, remove_after, split_by_chapters
     )
 
     is_single_conversion = comic_path.is_dir()
 
-    len_first_conv = cast(int, next(iterator))
+    try:
+        len_first_conv = cast(int, next(iterator))
+    except RuntimeError as err:
+        # handle kindlegen errors
+        typer.secho(str(err), fg=typer.colors.RED)
+        raise typer.Abort() from None
+
     len_second_conv = -1
 
     first_convert_message = (
         f"Packing {target_format.value}(s)"
         if is_single_conversion
         else "Pre-converting comic"
     )
 
-    with typer.progressbar(
-        iterator,
-        length=len_first_conv,
-        label=first_convert_message,
-    ) as progress:
-        for res in progress:
-            if isinstance(res, int):
-                len_second_conv = res
-                break
-            if split_by_chapters:
-                progress.label = res
-
-    if not is_single_conversion:
-        # it *should* be guaranteed len_second_conv exists
+    try:
         with typer.progressbar(
             iterator,
-            length=len_second_conv,
-            label=f"Packing {target_format.value}",
+            length=len_first_conv,
+            label=first_convert_message,
         ) as progress:
-            for _ in progress:
-                ...
+            for res in progress:
+                if isinstance(res, int):
+                    len_second_conv = res
+                    break
+                if split_by_chapters:
+                    progress.label = res
+    except RuntimeError as err:
+        # handle kindlegen errors
+        typer.secho(str(err), fg=typer.colors.RED)
+        raise typer.Abort() from None
+
+    if not is_single_conversion:
+        # it *should* be guaranteed len_second_conv exists
+        try:
+            with typer.progressbar(
+                iterator,
+                length=len_second_conv,
+                label=f"Packing {target_format.value}",
+            ) as progress:
+                for _ in progress:
+                    ...
+        except RuntimeError as err:
+            # handle kindlegen errors
+            typer.secho(str(err), fg=typer.colors.RED)
+            raise typer.Abort() from None
 
     if not split_by_chapters:
         dest_file = dest_folder / f"{comic_path.stem}.{target_format.value}"
         typer.secho(f"Successfully converted to {dest_file}", fg=typer.colors.GREEN)
     else:
         typer.secho(f"Successfully converted to {dest_folder}", fg=typer.colors.GREEN)
 
@@ -367,15 +383,15 @@
         "-r",
         help="IF CONVERTING: Remove the downloaded folder after converting",
     ),
     split_by_chapters: bool = typer.Option(
         False,
         "--split-by-chapters",
         "-b",
-        help="Instead of returning one large comic file, create one comic"
+        help="IF CONVERTING: Instead of returning one large comic file, create one comic"
         "file for each chapter (applies only to Mandown-created comic folders)",
     ),
 ) -> None:
     """
     Download from a URL chapters start_chapter to end_chapter.
     Defaults to the first chapter and last chapter, respectively
     in the working directory.
```

### Comparing `mandown-1.4.0/mandown/comic.py` & `mandown-1.5.0/mandown/comic.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/convert_utils.py` & `mandown-1.5.0/mandown/convert_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     The formats that mandown can convert to. This is used for the `--format` option.
     """
 
     # for typing purposes
     CBZ = "cbz"
     EPUB = "epub"
     PDF = "pdf"
+    MOBI = "mobi"
     NONE = "none"
 
 
 def convert_one(
     comic: comicon.Comic, comic_path: Path, to: ConvertFormats, dest_folder: Path
 ) -> Iterator[str | int]:
     # save comicon.json
```

### Comparing `mandown-1.4.0/mandown/io.py` & `mandown-1.5.0/mandown/io.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/processor/__init__.py` & `mandown-1.5.0/mandown/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/processor/ops.py` & `mandown-1.5.0/mandown/processor/ops.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/processor/profiles.py` & `mandown-1.5.0/mandown/processor/profiles.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/sources/__init__.py` & `mandown-1.5.0/mandown/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/sources/base_source.py` & `mandown-1.5.0/mandown/sources/base_source.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/sources/source_mangadex.py` & `mandown-1.5.0/mandown/sources/source_mangadex.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/sources/source_mangakakalot.py` & `mandown-1.5.0/mandown/sources/source_mangakakalot.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/sources/source_manganato.py` & `mandown-1.5.0/mandown/sources/source_manganato.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/sources/source_mangasee.py` & `mandown-1.5.0/mandown/sources/source_mangasee.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/sources/source_manhuaes.py` & `mandown-1.5.0/mandown/sources/source_manhuaes.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/sources/source_readcomiconline.py` & `mandown-1.5.0/mandown/sources/source_readcomiconline.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/sources/source_webtoons.py` & `mandown-1.5.0/mandown/sources/source_webtoons.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/ui/form.ui` & `mandown-1.5.0/mandown/ui/form.ui`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/ui/mainwin.py` & `mandown-1.5.0/mandown/ui/mainwin.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/mandown/ui/ui.py` & `mandown-1.5.0/mandown/ui/ui.py`

 * *Files identical despite different names*

### Comparing `mandown-1.4.0/pyproject.toml` & `mandown-1.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mandown"
-version = "1.4.0"
-description = "Comic/manga/webtoon downloader and CBZ/EPUB/PDF converter"
+version = "1.5.0"
+description = "Comic/manga/webtoon downloader and CBZ/EPUB/MOBI/PDF converter"
 authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/potatoeggy/mandown"
 documentation = "https://github.com/potatoeggy/mandown"
 keywords = ["manga", "comic", "downloader", "download", "webtoons", "webtoon"]
 
@@ -21,15 +21,15 @@
 requests = "^2.31.0"
 lxml = "^4.9.2"
 Pillow = "^9.5.0"
 python-slugify = "^8.0.1"
 PySide6 = {version = "^6.4.0", optional = true}
 natsort = "^8.1.0"
 filetype = "^1.2.0"
-comicon = "^0.2.4"
+comicon = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.31.0.1"
 types-lxml = "^2023.3.28"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.2"
```

### Comparing `mandown-1.4.0/PKG-INFO` & `mandown-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mandown
-Version: 1.4.0
-Summary: Comic/manga/webtoon downloader and CBZ/EPUB/PDF converter
+Version: 1.5.0
+Summary: Comic/manga/webtoon downloader and CBZ/EPUB/MOBI/PDF converter
 Home-page: https://github.com/potatoeggy/mandown
 License: AGPL-3.0-only
 Keywords: manga,comic,downloader,download,webtoons,webtoon
 Author: Daniel Chen
 Author-email: danielchen04@hotmail.ca
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
 Requires-Dist: Pillow (>=9.5.0,<10.0.0)
 Requires-Dist: PySide6 (>=6.4.0,<7.0.0) ; extra == "gui"
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: comicon (>=0.2.4,<0.3.0)
+Requires-Dist: comicon (>=1.0.0,<2.0.0)
 Requires-Dist: feedparser (>=6.0.10,<7.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: natsort (>=8.1.0,<9.0.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
@@ -34,38 +34,38 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Download from PyPI](https://img.shields.io/pypi/v/mandown)](https://pypi.org/project/mandown)
 [![Download from the AUR](https://img.shields.io/aur/version/mandown-git)](https://aur.archlinux.org/packages/mandown-git)
 [![Latest release](https://img.shields.io/github/v/release/potatoeggy/mandown?display_name=tag)](https://github.com/potatoeggy/mandown/releases/latest)
 [![License](https://img.shields.io/github/license/potatoeggy/mandown)](/LICENSE)
 
-Mandown is a comic downloader and a CBZ, EPUB, and/or PDF converter. It also supports image post-processing to make them more readable on certain devices similarly to [Kindle Comic Converter](https://github.com/ciromattia/kcc).
+Mandown is a comic downloader and a CBZ, EPUB, MOBI, and/or PDF converter. It also supports image post-processing to make them more readable on certain devices similarly to [Kindle Comic Converter](https://github.com/ciromattia/kcc).
 
 ## Features
 
 - Download comics from [supported sites](#supported-sites)
   - Supports downloading a range of chapters
   - Supports multithreaded downloading
 - Process downloaded images
   - Rotate or split double-page spreads
   - Trim borders
   - Resize images
-- Convert downloaded comics to CBZ, EPUB, or PDF
-  - Convert any other CBZ, EPUB, or PDF comic to CBZ, EPUB, or PDF
+- Convert downloaded comics to CBZ, EPUB, MOBI, or PDF
+  - Convert any other CBZ, EPUB, MOBI, or PDF comic to CBZ, EPUB, MOBI, or PDF
 - [A library to easily do all of this from other Python scripts](#basic-library-usage)
 
 ## Usage
 
 Run `mandown --help` or see the [docs](/docs/) for more information and examples.
 
 ```
 mandown get <URL>
 ```
 
-To convert the download contents to CBZ/EPUB/PDF, append the `--convert` option. To apply image processing to the downloaded images, append the `--process` option.
+To convert the downloaded contents to CBZ/EPUB/MOBI/PDF, append the `--convert` option. To apply image processing to the downloaded images, append the `--process` option.
 
 ```
 mandown get <URL> --convert epub --process rotate_double_pages
 ```
 
 To download only a certain range of chapters, append the `--start` and/or `--end` options.
```

