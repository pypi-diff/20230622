# Comparing `tmp/ciff-toolkit-0.1.0.tar.gz` & `tmp/ciff-toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciff-toolkit-0.1.0.tar", max compression
+gzip compressed data, was "ciff-toolkit-0.1.1.tar", max compression
```

## Comparing `ciff-toolkit-0.1.0.tar` & `ciff-toolkit-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-06-13 11:33:05.816128 ciff-toolkit-0.1.0/LICENSE
--rw-r--r--   0        0        0     3561 2023-06-13 12:35:59.394263 ciff-toolkit-0.1.0/README.md
--rw-r--r--   0        0        0        0 2022-12-23 15:05:50.925135 ciff-toolkit-0.1.0/ciff_toolkit/__init__.py
--rw-r--r--   0        0        0     3063 2023-01-11 11:11:04.153606 ciff-toolkit-0.1.0/ciff_toolkit/ciff_pb2.py
--rw-r--r--   0        0        0     2207 2023-05-23 07:47:35.899100 ciff-toolkit-0.1.0/ciff_toolkit/cli.py
--rw-r--r--   0        0        0     7497 2023-06-13 09:43:56.254880 ciff-toolkit-0.1.0/ciff_toolkit/merge.py
--rw-r--r--   0        0        0     2467 2023-01-11 10:55:00.541545 ciff-toolkit-0.1.0/ciff_toolkit/protos/ciff.proto
--rw-r--r--   0        0        0     4186 2023-06-13 10:49:07.762696 ciff-toolkit-0.1.0/ciff_toolkit/read.py
--rw-r--r--   0        0        0     2063 2023-06-13 10:46:21.783379 ciff-toolkit-0.1.0/ciff_toolkit/util.py
--rw-r--r--   0        0        0     1874 2023-06-13 08:48:14.053159 ciff-toolkit-0.1.0/ciff_toolkit/write.py
--rw-r--r--   0        0        0     1003 2023-06-13 12:53:05.057999 ciff-toolkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4742 2023-06-13 12:54:01.060396 ciff-toolkit-0.1.0/setup.py
--rw-r--r--   0        0        0     4287 2023-06-13 12:54:01.060728 ciff-toolkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-13 11:33:05.816128 ciff-toolkit-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3561 2023-06-13 12:35:59.394263 ciff-toolkit-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2022-12-23 15:05:50.925135 ciff-toolkit-0.1.1/ciff_toolkit/__init__.py
+-rw-r--r--   0        0        0     3063 2023-01-11 11:11:04.153606 ciff-toolkit-0.1.1/ciff_toolkit/ciff_pb2.py
+-rw-r--r--   0        0        0     2207 2023-05-23 07:47:35.899100 ciff-toolkit-0.1.1/ciff_toolkit/cli.py
+-rw-r--r--   0        0        0     7341 2023-06-22 12:26:48.128396 ciff-toolkit-0.1.1/ciff_toolkit/merge.py
+-rw-r--r--   0        0        0     2467 2023-01-11 10:55:00.541545 ciff-toolkit-0.1.1/ciff_toolkit/protos/ciff.proto
+-rw-r--r--   0        0        0     4192 2023-06-22 12:22:53.268983 ciff-toolkit-0.1.1/ciff_toolkit/read.py
+-rw-r--r--   0        0        0     2063 2023-06-13 10:46:21.783379 ciff-toolkit-0.1.1/ciff_toolkit/util.py
+-rw-r--r--   0        0        0     1887 2023-06-22 12:23:29.208893 ciff-toolkit-0.1.1/ciff_toolkit/write.py
+-rw-r--r--   0        0        0     1032 2023-06-22 12:23:46.620849 ciff-toolkit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4742 2023-06-22 12:26:51.700827 ciff-toolkit-0.1.1/setup.py
+-rw-r--r--   0        0        0     4287 2023-06-22 12:26:51.701770 ciff-toolkit-0.1.1/PKG-INFO
```

### Comparing `ciff-toolkit-0.1.0/LICENSE` & `ciff-toolkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ciff-toolkit-0.1.0/README.md` & `ciff-toolkit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ciff-toolkit-0.1.0/ciff_toolkit/ciff_pb2.py` & `ciff-toolkit-0.1.1/ciff_toolkit/ciff_pb2.py`

 * *Files identical despite different names*

### Comparing `ciff-toolkit-0.1.0/ciff_toolkit/cli.py` & `ciff-toolkit-0.1.1/ciff_toolkit/cli.py`

 * *Files identical despite different names*

### Comparing `ciff-toolkit-0.1.0/ciff_toolkit/merge.py` & `ciff-toolkit-0.1.1/ciff_toolkit/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,28 +68,25 @@
         result = Header()
 
         assert len(set(h.version for h in headers)) == 1
         assert len(set(h.total_postings_lists for h in headers)) == 1
         assert len(set(h.total_docs for h in headers)) == 1
         assert len(set(h.total_terms_in_collection for h in headers)) == 1
         assert len(set(h.average_doclength for h in headers)) == 1
-        assert len(set(h.description for h in headers)) == 1
 
         result.version = headers[0].version
         result.total_postings_lists = headers[0].total_postings_lists
         result.total_docs = headers[0].total_docs
         result.total_terms_in_collection = headers[0].total_terms_in_collection
         result.average_doclength = headers[0].average_doclength
-        result.description = headers[0].description
 
         result.num_docs = sum(h.num_docs for h in headers)
 
-        # TODO: reset this description
-        # descriptions = '\n'.join(f' {i + 1}. {h.description}' for i, h in enumerate(headers))
-        # result.description = f'This is a combination of {len(headers)} CIFF files:\n\n{descriptions}'
+        descriptions = '\n'.join(f' {i + 1}. {h.description}' for i, h in enumerate(headers))
+        result.description = f'This is a combination of {len(headers)} CIFF files:\n\n{descriptions}'
 
         return result
 
     def merge_documents(self) -> Iterable[DocRecord]:
         docs_per_ciff = self.get_documents_per_ciff()
 
         pq: PriorityQueue[tuple[str, tuple[int, DocRecord]]] = PriorityQueue()
```

### Comparing `ciff-toolkit-0.1.0/ciff_toolkit/protos/ciff.proto` & `ciff-toolkit-0.1.1/ciff_toolkit/protos/ciff.proto`

 * *Files identical despite different names*

### Comparing `ciff-toolkit-0.1.0/ciff_toolkit/read.py` & `ciff-toolkit-0.1.1/ciff_toolkit/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class BufferedReader:
     filename: Optional[Path] = None
     chunk_reader: Optional[Iterator[bytes]] = None
     fp: Optional[IO[bytes]] = None
 
     def __init__(self, source: Union[str, Path, Iterable[bytes]]) -> None:
         if isinstance(source, (str, Path)):
-            self.filename = source
+            self.filename = Path(source)
         else:
             self.chunk_reader = iter(source)
 
         self.buffer = bytearray()
 
     def read_varint(self) -> int:
         self._fill_buffer(16)
```

### Comparing `ciff-toolkit-0.1.0/ciff_toolkit/util.py` & `ciff-toolkit-0.1.1/ciff_toolkit/util.py`

 * *Files identical despite different names*

### Comparing `ciff-toolkit-0.1.0/ciff_toolkit/write.py` & `ciff-toolkit-0.1.1/ciff_toolkit/write.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 class MessageWriter:
     filename: Optional[Path] = None
     output: Optional[IO[bytes]] = None
 
     def __init__(self, output: Union[str, Path, IO[bytes]]) -> None:
-        if isinstance(output, Path):
-            self.filename = output
+        if isinstance(output, (str, Path)):
+            self.filename = Path(output)
         else:
             self.output = output
 
         self.varint_encoder = _VarintEncoder()
 
     def write_message(self, message: Message):
         self.write_serialized(message.SerializeToString())
```

### Comparing `ciff-toolkit-0.1.0/pyproject.toml` & `ciff-toolkit-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "ciff-toolkit"
-version = "0.1.0"
+version = "0.1.1"
 description = "Toolkit for working with Common Index File Format (CIFF) files."
 authors = ["Gijs Hendriksen <g.hendriksen@cs.ru.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://opencode.it4i.eu/openwebsearcheu-public/ciff-toolkit/"
 repository = "https://opencode.it4i.eu/openwebsearcheu-public/ciff-toolkit/"
 keywords = ["ciff"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
+include = [
+    "LICENSE",
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 protobuf = "^4.21.12"
 tqdm = "^4.64.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `ciff-toolkit-0.1.0/setup.py` & `ciff-toolkit-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'console_scripts': ['ciff_dump = ciff_toolkit.cli:dump',
                      'ciff_merge = ciff_toolkit.cli:merge',
                      'ciff_swap = ciff_toolkit.cli:swap',
                      'ciff_zero_index = ciff_toolkit.cli:zero_index']}
 
 setup_kwargs = {
     'name': 'ciff-toolkit',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Toolkit for working with Common Index File Format (CIFF) files.',
     'long_description': "# CIFF Toolkit\n\nThis repository contains a Python toolkit for working with [Common Index File Format (CIFF)](https://github.com/osirrc/ciff/) files.\n\nSpecifically, it provides a `CiffReader` and `CiffWriter` for easily reading and writing CIFF files. It also provides a handful of CLI tools, such as merging a CIFF file or dumping its contents.\n\n## Installation\n\nTo use the CIFF toolkit, install it from PyPI:\n\n```bash\n$ pip install ciff-toolkit\n```\n\n## Usage\n\n### Reading\n\nTo read a CIFF file, you can use the `CiffReader` class. It returns the posting lists and documents as lazy generators, so operations that need to process large CIFF files do not need to load the entire index into memory.\n\nThe `CiffReader` can be used as a context manager, automatically opening files if a path is supplied as a `str` or `pathlib.Path`. \n\n```python\nfrom ciff_toolkit.read import CiffReader\n\nwith CiffReader('./path/to/index.ciff') as reader:\n    header = reader.read_header()\n\n    for pl in reader.read_postings_lists():\n        print(pl)\n\n    for doc in reader.read_documents():\n        print(doc)\n```\n\nAlternatively, the `CiffReader` also accepts iterables of bytes instead of file paths. This could be useful if, for instance, the index is in a remote location:\n\n```python\nimport requests\nfrom ciff_toolkit.read import CiffReader\n\nurl = 'https://example.com/remote-index.ciff'\nwith CiffReader(requests.get(url, stream=True).iter_content(1024)) as reader:\n    header = reader.read_header()\n    ...\n```\n\n### Writing\n\nThe `CiffWriter` offers a similar context manager API:\n\n```python\nfrom ciff_toolkit.ciff_pb2 import Header, PostingsList, DocRecord\nfrom ciff_toolkit.write import CiffWriter\n\nheader: Header = ...\npostings_lists: list[PostingsList] = ...\ndoc_records: list[DocRecord] = ...\n\nwith CiffWriter('./path/to/index.ciff') as writer:\n    writer.write_header(header)\n    writer.write_postings_lists(postings_lists)\n    writer.write_documents(doc_records)\n```\n\n### Command Line Interface\n\nA couple of CLI commands are supported:\n\n- `ciff_dump INPUT`\n\n  Dumps the contents of a CIFF file, in order to inspect its contents.\n- `ciff_merge INPUT... OUTPUT`\n\n  Merges two or more CIFF files into a single CIFF file. Ensures documents and terms are ordered correctly, and will read and write in a streaming manner (i.e. not read all data into memory at once).\n\n  Note: `ciff_merge` requires that the `DocRecord` messages occur before the `PostingsList` messages in the CIFF file, as it needs to remap the internal document identifiers before merging the posting lists. See `ciff_swap` below for more information on how to achieve that. \n- `ciff_swap --input-order [hpd|hdp] INPUT OUTPUT`\n\n  Swaps the `PostingsList` and `DocRecord` messages in a CIFF file (e.g. in order to prepare for merging). The `--input-order` argument specifies the current format of the CIFF file: `hpd` for header - posting lists - documents, and `hdp` for header - documents - posting lists.\n- `ciff_zero_index INPUT OUTPUT`\n\n  Takes a CIFF file with 1-indexed documents, and turns it into 0-indexed documents.\n\n## Development\n\nThis project uses [Poetry](https://python-poetry.org/) to manage dependencies, configure the project and publish it to PyPI.\n\nTo get started, use Poetry to install all dependencies:\n\n```bash\n$ poetry install\n```\n\nThen, either activate the virtual environment to execute all Python code in the virtual environment, or prepend every command with poetry run.\n\n```bash\n$ poetry shell\n(venv) $ ciff_dump index.ciff\n```\n\nor:\n\n```bash\n$ poetry run ciff_dump index.ciff\n```\n",
     'author': 'Gijs Hendriksen',
     'author_email': 'g.hendriksen@cs.ru.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://opencode.it4i.eu/openwebsearcheu-public/ciff-toolkit/',
```

### Comparing `ciff-toolkit-0.1.0/PKG-INFO` & `ciff-toolkit-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciff-toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolkit for working with Common Index File Format (CIFF) files.
 Home-page: https://opencode.it4i.eu/openwebsearcheu-public/ciff-toolkit/
 License: MIT
 Keywords: ciff
 Author: Gijs Hendriksen
 Author-email: g.hendriksen@cs.ru.nl
 Requires-Python: >=3.10,<4.0
```

