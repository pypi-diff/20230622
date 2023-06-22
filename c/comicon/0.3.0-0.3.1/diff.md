# Comparing `tmp/comicon-0.3.0.tar.gz` & `tmp/comicon-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicon-0.3.0.tar", max compression
+gzip compressed data, was "comicon-0.3.1.tar", max compression
```

## Comparing `comicon-0.3.0.tar` & `comicon-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    34520 2023-04-28 17:41:58.054636 comicon-0.3.0/LICENSE
--rw-r--r--   0        0        0     1493 2023-04-28 17:41:58.055636 comicon-0.3.0/README.md
--rw-r--r--   0        0        0      348 2023-04-28 17:41:58.056636 comicon-0.3.0/comicon/__init__.py
--rw-r--r--   0        0        0      585 2023-06-20 21:51:44.295564 comicon-0.3.0/comicon/api.py
--rw-r--r--   0        0        0     1034 2023-04-28 17:41:58.057636 comicon-0.3.0/comicon/base.py
--rw-r--r--   0        0        0     3391 2023-06-20 21:41:12.912362 comicon-0.3.0/comicon/cirtools.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/__init__.py
--rw-r--r--   0        0        0      410 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/cbz.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/cir.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/epub.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.0/comicon/common/pdf.py
--rw-r--r--   0        0        0      673 2023-06-20 21:37:55.976776 comicon-0.3.0/comicon/errors.py
--rw-r--r--   0        0        0     1890 2023-04-28 17:41:58.058636 comicon-0.3.0/comicon/inputs/__init__.py
--rw-r--r--   0        0        0     4605 2023-04-28 17:41:58.058636 comicon-0.3.0/comicon/inputs/cbz.py
--rw-r--r--   0        0        0      631 2023-04-28 17:41:58.057636 comicon-0.3.0/comicon/inputs/cir.py
--rw-r--r--   0        0        0     5888 2023-04-28 17:41:58.058636 comicon-0.3.0/comicon/inputs/epub.py
--rw-r--r--   0        0        0     2810 2023-04-28 17:41:58.057636 comicon-0.3.0/comicon/inputs/pdf.py
--rw-r--r--   0        0        0     1873 2023-04-28 17:41:58.061636 comicon-0.3.0/comicon/outputs/__init__.py
--rw-r--r--   0        0        0     1845 2023-04-28 17:41:58.061636 comicon-0.3.0/comicon/outputs/cbz.py
--rw-r--r--   0        0        0      657 2023-04-28 17:41:58.061636 comicon-0.3.0/comicon/outputs/cir.py
--rw-r--r--   0        0        0     3117 2023-06-20 21:43:52.484820 comicon-0.3.0/comicon/outputs/epub.py
--rw-r--r--   0        0        0     1891 2023-04-28 17:41:58.062636 comicon-0.3.0/comicon/outputs/pdf.py
--rw-r--r--   0        0        0      964 2023-06-21 03:28:41.534008 comicon-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 comicon-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:58.054636 comicon-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1605 2023-06-22 00:48:57.443731 comicon-0.3.1/README.md
+-rw-r--r--   0        0        0      348 2023-04-28 17:41:58.056636 comicon-0.3.1/comicon/__init__.py
+-rw-r--r--   0        0        0      585 2023-06-20 21:51:44.295564 comicon-0.3.1/comicon/api.py
+-rw-r--r--   0        0        0     1764 2023-06-21 22:38:57.631788 comicon-0.3.1/comicon/base.py
+-rw-r--r--   0        0        0     3391 2023-06-20 21:41:12.912362 comicon-0.3.1/comicon/cirtools.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/cbz.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/cir.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/epub.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/pdf.py
+-rw-r--r--   0        0        0      673 2023-06-20 21:37:55.976776 comicon-0.3.1/comicon/errors.py
+-rw-r--r--   0        0        0     1890 2023-04-28 17:41:58.058636 comicon-0.3.1/comicon/inputs/__init__.py
+-rw-r--r--   0        0        0     4807 2023-06-21 22:40:25.769680 comicon-0.3.1/comicon/inputs/cbz.py
+-rw-r--r--   0        0        0      631 2023-04-28 17:41:58.057636 comicon-0.3.1/comicon/inputs/cir.py
+-rw-r--r--   0        0        0     6845 2023-06-21 22:57:31.844781 comicon-0.3.1/comicon/inputs/epub.py
+-rw-r--r--   0        0        0     3034 2023-06-21 22:56:41.986407 comicon-0.3.1/comicon/inputs/pdf.py
+-rw-r--r--   0        0        0     1905 2023-06-22 00:47:58.838468 comicon-0.3.1/comicon/outputs/__init__.py
+-rw-r--r--   0        0        0     1845 2023-04-28 17:41:58.061636 comicon-0.3.1/comicon/outputs/cbz.py
+-rw-r--r--   0        0        0      657 2023-04-28 17:41:58.061636 comicon-0.3.1/comicon/outputs/cir.py
+-rw-r--r--   0        0        0     3117 2023-06-20 21:43:52.484820 comicon-0.3.1/comicon/outputs/epub.py
+-rw-r--r--   0        0        0     1759 2023-06-22 00:47:44.641646 comicon-0.3.1/comicon/outputs/mobi.py
+-rw-r--r--   0        0        0     1891 2023-04-28 17:41:58.062636 comicon-0.3.1/comicon/outputs/pdf.py
+-rw-r--r--   0        0        0      977 2023-06-22 00:50:27.589598 comicon-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 comicon-0.3.1/PKG-INFO
```

### Comparing `comicon-0.3.0/LICENSE` & `comicon-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/README.md` & `comicon-0.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Comicon
 
-Comicon is a lightweight comic converter library between CBZ, PDF, and EPUB that preserves metadata. Once Comicon has converted a comic, it is **guaranteed** that the reverse conversion will restore the original comic with all of its original metadata.
+Comicon is a lightweight comic converter library between CBZ, PDF, EPUB, and MOBI that preserves metadata. Once Comicon has converted a comic, it is **guaranteed** that the reverse conversion will restore the original comic with all of its original metadata.
 
 ## Usage
 
 For a command line interface, please see [Mandown](https://github.com/potatoeggy/mandown).
 
 ```python
 import comicon
@@ -18,19 +18,20 @@
 
 ```
 pip install comicon
 ```
 
 ## Supported conversions
 
-| Format | Convert from? | Convert to? |
-| --- | --- | --- |
-| CBZ | :heavy_check_mark: | :heavy_check_mark: |
-| EPUB | :heavy_check_mark: | :heavy_check_mark: |
-| PDF | :heavy_check_mark: | :heavy_check_mark: |
+| Format | Convert from?      | Convert to?        |
+| ------ | ------------------ | ------------------ |
+| CBZ    | :heavy_check_mark: | :heavy_check_mark: |
+| EPUB   | :heavy_check_mark: | :heavy_check_mark: |
+| PDF    | :heavy_check_mark: | :heavy_check_mark: |
+| MOBI   | :x:                | :heavy_check_mark: |
 
 ### Format discrepancies
 
 - Only EPUB supports a table of contents. CBZ and PDF will encode the table of contents so that it is restored upon converting to EPUB.
 - PDF does not support importing genre data due to a lack of library support. This may be worked around in the future.
 
 ## Notes
```

### Comparing `comicon-0.3.0/comicon/api.py` & `comicon-0.3.1/comicon/api.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/comicon/cirtools.py` & `comicon-0.3.1/comicon/cirtools.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/comicon/errors.py` & `comicon-0.3.1/comicon/errors.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/comicon/inputs/__init__.py` & `comicon-0.3.1/comicon/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/comicon/inputs/cbz.py` & `comicon-0.3.1/comicon/inputs/cbz.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,18 @@
                         case "Genre":
                             data_dict["genres"] = str(el.text).split(", ")
             elif name.endswith(IR_DATA_FILE):
                 with z.open(name) as file:
                     data = file.read()
 
                 comic = Comic.from_json(data)
+                # TODO: guarantee that this is done last after we've looked
+                # at all other possible sources of metadata
+                comic.metadata.merge_with(Metadata(**data_dict))
+
                 found_comicon_metadata = True
                 break
             elif "cover" in name and Path(name).suffix in ACCEPTED_IMAGE_EXTENSIONS:
                 # assume that any *cover*.{img} is the cover image
                 # TODO: CAN AND WILL BREAK ON FOLDER NAMES
                 data_dict["cover_path_rel"] = name
             elif (path := Path(name)).suffix in ACCEPTED_IMAGE_EXTENSIONS:
```

### Comparing `comicon-0.3.0/comicon/inputs/cir.py` & `comicon-0.3.1/comicon/inputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/comicon/inputs/epub.py` & `comicon-0.3.1/comicon/inputs/epub.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,24 +8,70 @@
 from ..base import Chapter, Comic, Metadata
 
 XML_NAMESPACE = "http://purl.org/dc/elements/1.1/"
 
 
 def create_cir(path: Path, dest: Path) -> Iterator[str | int]:
     book = epub.read_epub(path)
+    comic = create_metadata_from_comicon(book)
+    book_metadata = create_metadata_from_book(book)
+    if comic:
+        comic.metadata.merge_with(book_metadata)
+        return create_cir_from_comicon(dest, book, comic)
+    return create_cir_from_other(dest, book, book_metadata)
+
+
+def create_metadata_from_comicon(book: epub.EpubBook) -> Comic | None:
+    """
+    Search the book for a Comicon data file and attempt to parse its metadata.
+    If no data file is found, return None.
+    """
     out: list[epub.EpubItem] = list(book.get_items())
-    comic = None
     for item in out:
         match item.file_name.split("/"):
             case ["static", cirtools.IR_DATA_FILE]:
-                comic = Comic.from_json(item.get_content())
-                return create_cir_from_comicon(dest, book, comic)
+                return Comic.from_json(item.get_content())
             case _:
                 ...
-    return create_cir_from_other(dest, book)
+    return None
+
+
+def create_metadata_from_book(book: epub.EpubBook) -> Metadata:
+    """
+    Search for metadata in the book itself, returning a comic
+    with the populated metadata but no chapters.
+    """
+    # look at TOC, take title and slug from each
+    # look at spine, be like noveldown
+    metadata = book.metadata[XML_NAMESPACE]
+    title: str = metadata["title"][0][0]
+    description: str = metadata["description"][0][0]
+    authors: list[str] = [author for author, _ in metadata["creator"]]
+    genres: list[str] = [genre for genre, _ in metadata["subject"]]
+
+    cover_item_rel: str | None = None
+    cover_item = get_cover_item(book)
+    if cover_item:
+        cover_item_rel = cover_item.file_name.split("/")[-1]
+
+    return Metadata(title, authors, description, genres, cover_item_rel)
+
+
+def get_cover_item(book: epub.EpubBook) -> epub.EpubItem | None:
+    """
+    Attempt to find the cover image item in the book.
+    """
+    try:
+        imgdir = book.get_metadata("OPF", "cover")[0][1]["content"]
+        cover_item: epub.EpubItem = book.get_item_with_id(imgdir)
+        return cover_item
+    except (KeyError, IndexError):
+        # no cover image
+        ...
+    return None
 
 
 def create_cir_from_comicon(
     dest: Path, book: epub.EpubBook, comic: Comic
 ) -> Iterator[str | int]:
     # we can make a *lot* of assumptions
     (dest / cirtools.IR_DATA_FILE).write_text(comic.to_json())
@@ -47,36 +93,22 @@
                 dest_path.write_bytes(item.get_content())
             case _:
                 # ignore all other files because comicon.json has everything
                 # we need
                 pass
 
 
-def create_cir_from_other(dest: Path, book: epub.EpubBook) -> Iterator[str | int]:
-    # look at TOC, take title and slug from each
-    # look at spine, be like noveldown
-    metadata = book.metadata[XML_NAMESPACE]
-    title: str = metadata["title"][0][0]
-    description: str = metadata["description"][0][0]
-    authors: list[str] = [author for author, _ in metadata["creator"]]
-    genres: list[str] = [genre for genre, _ in metadata["subject"]]
-    cover_item_rel: str | None = None
-
-    try:
-        imgdir = book.get_metadata("OPF", "cover")[0][1]["content"]
-        cover_item: epub.EpubItem = book.get_item_with_id(imgdir)
-
-        cover_path = dest / cover_item.file_name.split("/")[-1]
+def create_cir_from_other(
+    dest: Path, book: epub.EpubBook, metadata: Metadata
+) -> Iterator[str | int]:
+    if metadata.cover_path_rel:
+        cover_path = dest / metadata.cover_path_rel
+        # this must be true because cover_path_rel exists
+        cover_item = cast(epub.EpubItem, get_cover_item(book))
         cover_path.write_bytes(cover_item.get_content())
-        cover_item_rel = cover_item.file_name.split("/")[-1]
-    except (KeyError, IndexError):
-        # no cover image
-        ...
-
-    comic_metadata = Metadata(title, authors, description, genres, cover_item_rel)
 
     # assume that there can be no duplicate IDs in
     # a properly formed EPUB
     cache_dict: dict[str, epub.EpubItem] = {}
 
     for item in book.get_items():
         cache_dict[item.id] = item
@@ -103,15 +135,15 @@
             item += 1
             chapters[item - 1][1].append(page)
         elif item > 0:
             # ignore anything before the first chapter
             # this is a hack so we don't have to create a new chapter
             chapters[item - 1][1].append(page)
 
-    comic = Comic(comic_metadata, [chapter.base_chap for chapter, _ in chapters])
+    comic = Comic(metadata, [chapter.base_chap for chapter, _ in chapters])
     (dest / cirtools.IR_DATA_FILE).write_text(comic.to_json())
 
     for chapter, page_list in chapters:
         chapter_dir = dest / chapter.base_chap.slug
         chapter_dir.mkdir(exist_ok=True)
         # copy meta
         for i, page in enumerate(page_list, start=1):
```

### Comparing `comicon-0.3.0/comicon/inputs/pdf.py` & `comicon-0.3.1/comicon/inputs/pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,26 +23,30 @@
 
         author_str = reader.metadata.author
         authors = author_str.split(",") if author_str else []
 
         # PyPDF does not support getting keywords
         # genre_str = reader.documentInfo["/Keywords"]
         # genres = genre_str.split(",") if genre_str else []
-        genres = []
+        genres: list[str] = []
         description = reader.metadata.subject
 
         # det if this is a comicon comic
         # we can use the "extra_metadata": "pdf_pages" fields to
         # to check via duck typings
+        inferred_metadata = Metadata(title, authors, description, genres, "")
 
         if reader.metadata.producer == "comicon":
             comic = Comic.from_json(reader.metadata.creator)
+            comic.metadata.merge_with(inferred_metadata)
         else:
-            metadata = Metadata(title, authors, description, genres, "")
-            comic = Comic(metadata, [Chapter("Chapter 1", "chapter-1")])
+            comic = Comic(inferred_metadata, [Chapter("Chapter 1", "chapter-1")])
+    else:
+        empty_metadata = Metadata(title, [], "", [], "")
+        comic = Comic(empty_metadata, [Chapter("Chapter 1", "chapter-1")])
 
         # use first image as cover
     yield len(reader.pages)
 
     # below is for OTHER only
     cover_name = ""  # guaranteed to be set in loop unless there are no images
```

### Comparing `comicon-0.3.0/comicon/outputs/__init__.py` & `comicon-0.3.1/comicon/outputs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from pathlib import Path
 from typing import Callable, Iterator, Literal, get_args
 
 from .. import cirtools
-from . import cbz, cir, epub, pdf
+from . import cbz, cir, epub, mobi, pdf
 
-SupportedOutputs = Literal["cbz", "epub", "pdf", "cir"]
+SupportedOutputs = Literal["cbz", "epub", "pdf", "cir", "mobi"]
 OutputFn = Callable[[Path, Path], Iterator[str | int]]
 
-SupportedOutputList: tuple[SupportedOutputs] = get_args(SupportedOutputs)  # type: ignore # noqa: B950
+SupportedOutputList: tuple[SupportedOutputs] = get_args(SupportedOutputs)  # type: ignore
 
 OUTPUT_FN_MAP: dict[SupportedOutputs, OutputFn] = {
     "cbz": cbz.create_comic,
     "epub": epub.create_comic,
     "pdf": pdf.create_comic,
     "cir": cir.create_comic,
+    "mobi": mobi.create_comic,
 }
 
 
 def create_comic(
     ir_path: Path | str,
     dest: Path | str,
     ext: SupportedOutputs | None = None,
```

### Comparing `comicon-0.3.0/comicon/outputs/cbz.py` & `comicon-0.3.1/comicon/outputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/comicon/outputs/cir.py` & `comicon-0.3.1/comicon/outputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/comicon/outputs/epub.py` & `comicon-0.3.1/comicon/outputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/comicon/outputs/pdf.py` & `comicon-0.3.1/comicon/outputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.0/pyproject.toml` & `comicon-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "comicon"
-version = "0.3.0"
-description = "A simple comic conversion library between CBZ/EPUB/PDF"
+version = "0.3.1"
+description = "A simple comic conversion library between CBZ/EPUB/MOBI/PDF"
 authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 repository = "https://github.com/potatoeggy/comicon"
 documentation = "https://github.com/potatoeggy/comicon"
-keywords = ["converter", "comic", "cbz", "epub", "pdf"]
+keywords = ["converter", "comic", "cbz", "epub", "pdf", "mobi"]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 ebooklib = "^0.18"
 pillow = "^9.4.0"
 lxml = "^4.9.2"
 pypdf = {extras = ["image"], version = "^3.2.1"}
```

### Comparing `comicon-0.3.0/PKG-INFO` & `comicon-0.3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: comicon
-Version: 0.3.0
-Summary: A simple comic conversion library between CBZ/EPUB/PDF
+Version: 0.3.1
+Summary: A simple comic conversion library between CBZ/EPUB/MOBI/PDF
 Home-page: https://github.com/potatoeggy/comicon
 License: AGPL-3.0-only
-Keywords: converter,comic,cbz,epub,pdf
+Keywords: converter,comic,cbz,epub,pdf,mobi
 Author: Daniel Chen
 Author-email: danielchen04@hotmail.ca
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,15 +18,15 @@
 Requires-Dist: pypdf[image] (>=3.2.1,<4.0.0)
 Project-URL: Documentation, https://github.com/potatoeggy/comicon
 Project-URL: Repository, https://github.com/potatoeggy/comicon
 Description-Content-Type: text/markdown
 
 # Comicon
 
-Comicon is a lightweight comic converter library between CBZ, PDF, and EPUB that preserves metadata. Once Comicon has converted a comic, it is **guaranteed** that the reverse conversion will restore the original comic with all of its original metadata.
+Comicon is a lightweight comic converter library between CBZ, PDF, EPUB, and MOBI that preserves metadata. Once Comicon has converted a comic, it is **guaranteed** that the reverse conversion will restore the original comic with all of its original metadata.
 
 ## Usage
 
 For a command line interface, please see [Mandown](https://github.com/potatoeggy/mandown).
 
 ```python
 import comicon
@@ -40,19 +40,20 @@
 
 ```
 pip install comicon
 ```
 
 ## Supported conversions
 
-| Format | Convert from? | Convert to? |
-| --- | --- | --- |
-| CBZ | :heavy_check_mark: | :heavy_check_mark: |
-| EPUB | :heavy_check_mark: | :heavy_check_mark: |
-| PDF | :heavy_check_mark: | :heavy_check_mark: |
+| Format | Convert from?      | Convert to?        |
+| ------ | ------------------ | ------------------ |
+| CBZ    | :heavy_check_mark: | :heavy_check_mark: |
+| EPUB   | :heavy_check_mark: | :heavy_check_mark: |
+| PDF    | :heavy_check_mark: | :heavy_check_mark: |
+| MOBI   | :x:                | :heavy_check_mark: |
 
 ### Format discrepancies
 
 - Only EPUB supports a table of contents. CBZ and PDF will encode the table of contents so that it is restored upon converting to EPUB.
 - PDF does not support importing genre data due to a lack of library support. This may be worked around in the future.
 
 ## Notes
```

