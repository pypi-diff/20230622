# Comparing `tmp/stringzilla-0.1.1-cp39-cp39-manylinux_2_28_x86_64.whl.zip` & `tmp/stringzilla-0.1.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,7 @@
-Zip file size: 228824 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 20:45 stringzilla-0.1.1.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-21 20:45 stringzilla./
--rwxr-xr-x  2.0 unx   382129 b- defN 23-Jun-21 20:45 stringzilla.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     3532 b- defN 23-Jun-21 20:45 stringzilla-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-21 20:45 stringzilla-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      519 b- defN 23-Jun-21 20:45 stringzilla-0.1.1.dist-info/RECORD
--rw-r--r--  2.0 unx      112 b- defN 23-Jun-21 20:45 stringzilla-0.1.1.dist-info/WHEEL
--rwxr-xr-x  2.0 unx   253289 b- defN 23-Jun-21 20:45 stringzilla./libgomp-22744126.so.1.0.0
-8 files, 639593 bytes uncompressed, 227664 bytes compressed:  64.4%
+Zip file size: 89863 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat   212480 b- defN 23-Jun-22 08:51 stringzilla.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     4019 b- defN 23-Jun-22 08:51 stringzilla-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-22 08:51 stringzilla-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-22 08:51 stringzilla-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      404 b- defN 23-Jun-22 08:51 stringzilla-0.1.2.dist-info/RECORD
+5 files, 217015 bytes uncompressed, 89113 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,25 +1,16 @@
-Filename: stringzilla-0.1.1.dist-info/
+Filename: stringzilla.cp39-win_amd64.pyd
 Comment: 
 
-Filename: stringzilla./
+Filename: stringzilla-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: stringzilla.cpython-39-x86_64-linux-gnu.so
+Filename: stringzilla-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: stringzilla-0.1.1.dist-info/METADATA
+Filename: stringzilla-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: stringzilla-0.1.1.dist-info/top_level.txt
-Comment: 
-
-Filename: stringzilla-0.1.1.dist-info/RECORD
-Comment: 
-
-Filename: stringzilla-0.1.1.dist-info/WHEEL
-Comment: 
-
-Filename: stringzilla./libgomp-22744126.so.1.0.0
+Filename: stringzilla-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `stringzilla-0.1.1.dist-info/METADATA` & `stringzilla-0.1.2.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,143 +1,150 @@
-Metadata-Version: 2.1
-Name: stringzilla
-Version: 0.1.1
-Summary: Crunch 100+ GB Strings in Python with ease
-License: Apache-2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
-
-# Stringzilla
-
-## Crunch 100+ GB Strings in Python with ease, leveraging SIMD Assembly
-
-Stringzilla was born many years ago as a [tutorial for SIMD accelerated string-processing][tutorial].
-But one day, processing 100+ GB Chemistry and AI datasets, I decided to transform it into a library.
-It's designed to replace `open(...).readlines()`, `str().splitlines()` and many other common workloads with very long strings.
-
-<table>
-<tr>
-<td>
-
-<table>
-<thead>
-<tr>
-<th style="text-align:left">Benchmark</th>
-<th style="text-align:center">IoT</th>
-<th style="text-align:center">Arm Laptop</th>
-<th style="text-align:center">x86 Server</th>
-</tr>
-</thead>
-<tbody>
-<tr>
-<td style="text-align:left">Python: <code>str.find</code></td>
-<td style="text-align:center">4 MB/s</td>
-<td style="text-align:center">14 MB/s</td>
-<td style="text-align:center">11 MB/s</td>
-</tr>
-<tr>
-<td style="text-align:left">C++: <code>std::string::find</code></td>
-<td style="text-align:center">560 MB/s</td>
-<td style="text-align:center">1,2 GB/s</td>
-<td style="text-align:center">1,3 GB/s</td>
-</tr>
-<tr>
-<td style="text-align:left">Stringzilla</td>
-<td style="text-align:center">4,3 Gb/s</td>
-<td style="text-align:center">12 GB/s</td>
-<td style="text-align:center">12,1 GB/s</td>
-</tr>
-</tbody>
-</table>
-
-</td>
-<td>
-<img src="https://github.com/ashvardanian/Stringzilla/blob/main/stringzilla.jpeg?raw=true" height=150px>
-</td>
-<tr>
-</table>
-
-[tutorial]: https://youtu.be/6Sh9QWdzo58
-
-## Usage
-
-```sh
-pip install stringzilla
-```
-
-There are two classes you can use interchangibly:
-
-```python
-from stringzilla import Str, File, Slices
-
-text: str = 'some-string'
-text: Str = Str('some-string')
-text: File = File('some-file.txt')
-```
-
-Once constructed, following interfaces are supported:
-
-```python
-len(text) -> int
-'substring' in text -> bool
-text[42] -> str
-
-text.contains(
-    'subtring',
-    start=0, # optional
-    end=9223372036854775807, # optional
-) -> bool
-
-text.find(
-    'subtring',
-    start=0, # optional
-    end=9223372036854775807, # optional
-) -> int
-
-text.count(
-    'subtring',
-    start=0, # optional
-    end=9223372036854775807, # optional
-    **, # non-traditional arguments:
-    allowoverlap=False, # optional
-) -> int
-
-text.splitlines(
-    keeplinebreaks=False, # optional
-    **, # non-traditional arguments:
-    separator='\n', # optional
-) -> Slices # similar to list[str]
-
-text.split(
-    separator=' ', # optional
-    maxsplit=9223372036854775807, # optional
-    **, # non-traditional arguments:
-    keepseparator=False, # optional
-) -> Slices # similar to list[str]
-```
-
-## Development
-
-```sh
-rm -rf build && pip install -e . && pytest scripts/test.py -s -x
-```
-
-To benchmark on some custom file and pattern combination:
-
-```sh
-python scripts/bench.py --path "your file" --pattern "your pattern"
-```
-
-To validate packaging:
-
-```sh
-cibuildwheel --platform linux
-```
+Metadata-Version: 2.1
+Name: stringzilla
+Version: 0.1.2
+Summary: Crunch 100+ GB Strings in Python with ease
+License: Apache-2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: File Formats
+Classifier: Topic :: Internet :: Log Analysis
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: Text Processing :: General
+Classifier: Topic :: Text Processing :: Indexing
+Description-Content-Type: text/markdown
+
+# Stringzilla
+
+## Crunch 100+ GB Strings in Python with ease, leveraging SIMD Assembly
+
+Stringzilla was born many years ago as a [tutorial for SIMD accelerated string-processing][tutorial].
+But one day, processing 100+ GB Chemistry and AI datasets, I decided to transform it into a library.
+It's designed to replace `open(...).readlines()`, `str().splitlines()` and many other common workloads with very long strings.
+
+<table>
+<tr>
+<td>
+
+<table>
+<thead>
+<tr>
+<th style="text-align:left">Benchmark</th>
+<th style="text-align:center">IoT</th>
+<th style="text-align:center">Arm Laptop</th>
+<th style="text-align:center">x86 Server</th>
+</tr>
+</thead>
+<tbody>
+<tr>
+<td style="text-align:left">Python: <code>str.find</code></td>
+<td style="text-align:center">4 MB/s</td>
+<td style="text-align:center">14 MB/s</td>
+<td style="text-align:center">11 MB/s</td>
+</tr>
+<tr>
+<td style="text-align:left">C++: <code>std::string::find</code></td>
+<td style="text-align:center">560 MB/s</td>
+<td style="text-align:center">1,2 GB/s</td>
+<td style="text-align:center">1,3 GB/s</td>
+</tr>
+<tr>
+<td style="text-align:left">Stringzilla</td>
+<td style="text-align:center">4,3 Gb/s</td>
+<td style="text-align:center">12 GB/s</td>
+<td style="text-align:center">12,1 GB/s</td>
+</tr>
+</tbody>
+</table>
+
+</td>
+<td>
+<img src="https://github.com/ashvardanian/Stringzilla/blob/main/stringzilla.jpeg?raw=true" height=150px>
+</td>
+<tr>
+</table>
+
+[tutorial]: https://youtu.be/6Sh9QWdzo58
+
+## Usage
+
+```sh
+pip install stringzilla
+```
+
+There are two classes you can use interchangibly:
+
+```python
+from stringzilla import Str, File, Slices
+
+text: str = 'some-string'
+text: Str = Str('some-string')
+text: File = File('some-file.txt')
+```
+
+Once constructed, following interfaces are supported:
+
+```python
+len(text) -> int
+'substring' in text -> bool
+text[42] -> str
+
+text.contains(
+    'subtring',
+    start=0, # optional
+    end=9223372036854775807, # optional
+) -> bool
+
+text.find(
+    'subtring',
+    start=0, # optional
+    end=9223372036854775807, # optional
+) -> int
+
+text.count(
+    'subtring',
+    start=0, # optional
+    end=9223372036854775807, # optional
+    **, # non-traditional arguments:
+    allowoverlap=False, # optional
+) -> int
+
+text.splitlines(
+    keeplinebreaks=False, # optional
+    **, # non-traditional arguments:
+    separator='\n', # optional
+) -> Slices # similar to list[str]
+
+text.split(
+    separator=' ', # optional
+    maxsplit=9223372036854775807, # optional
+    **, # non-traditional arguments:
+    keepseparator=False, # optional
+) -> Slices # similar to list[str]
+```
+
+## Development
+
+```sh
+rm -rf build && pip install -e . && pytest scripts/test.py -s -x
+```
+
+To benchmark on some custom file and pattern combination:
+
+```sh
+python scripts/bench.py --path "your file" --pattern "your pattern"
+```
+
+To validate packaging:
+
+```sh
+cibuildwheel --platform linux
+```
```

