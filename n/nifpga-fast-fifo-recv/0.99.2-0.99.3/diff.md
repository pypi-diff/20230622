# Comparing `tmp/nifpga_fast_fifo_recv-0.99.2.tar.gz` & `tmp/nifpga_fast_fifo_recv-0.99.3.tar.gz`

## Comparing `nifpga_fast_fifo_recv-0.99.2.tar` & `nifpga_fast_fifo_recv-0.99.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.2/Cargo.toml
--rw-r--r--   0        0        0     1081 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.2/LICENSE
--rw-r--r--   0        0        0     6175 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.2/README.md
--rw-r--r--   0        0        0      561 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.2/pyproject.toml
--rw-r--r--   0        0        0        9 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.2/requirements.txt
--rw-r--r--   0        0        0     7728 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.2/src/lib.rs
--rw-r--r--   0        0        0    10405 2023-06-22 09:52:57.000000 nifpga_fast_fifo_recv-0.99.2/Cargo.lock
--rw-r--r--   0        0        0     6749 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.2/PKG-INFO
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.3/Cargo.toml
+-rw-r--r--   0        0        0     1081 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.3/LICENSE
+-rw-r--r--   0        0        0     5061 2023-06-22 09:57:52.000000 nifpga_fast_fifo_recv-0.99.3/README.md
+-rw-r--r--   0        0        0      561 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.3/pyproject.toml
+-rw-r--r--   0        0        0        9 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.3/requirements.txt
+-rw-r--r--   0        0        0     7728 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.3/src/lib.rs
+-rw-r--r--   0        0        0    10405 2023-06-22 09:57:53.000000 nifpga_fast_fifo_recv-0.99.3/Cargo.lock
+-rw-r--r--   0        0        0     5635 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.3/PKG-INFO
```

### Comparing `nifpga_fast_fifo_recv-0.99.2/Cargo.toml` & `nifpga_fast_fifo_recv-0.99.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "nifpga-fast-fifo-recv"
 readme = "README.md"
-version = "0.99.2"
+version = "0.99.3"
 edition = "2021"
 license = "MIT"
 authors = ["Mattia Donato"]
 description = "A Python module for fast reading of data from NI FPGA FIFOs with a separate thread."
 repository = "https://github.com/mattia-donato/nifpga-fast-fifo-recv"
 exclude = ["nifpga.*", "NiFpga.*", ".idea/*" ]
```

### Comparing `nifpga_fast_fifo_recv-0.99.2/LICENSE` & `nifpga_fast_fifo_recv-0.99.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.2/README.md` & `nifpga_fast_fifo_recv-0.99.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: nifpga-fast-fifo-recv
+Version: 0.99.3
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
+Summary: A Python module for fast reading of data from NI FPGA FIFOs with a separate thread.
+Author: Mattia Donato
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Documentation, https://github.com/mattia-donato/nifpga-fast-fifo-recv
+
 # nifpga-fast-fifo-recv
 A Python module for fast reading of data from NI FPGA FIFOs with a separate thread.
 
 This module provides in Python a class and the methods to start a separate thread which acquire continously 
 data and store them into a queue which can be read asynchronously. 
 This allows to receive data from NI FPGA in Python ideally without loosing data even for fast data-rate.
 
@@ -104,56 +118,15 @@
 
 In order to compile this project you need *maturin* 
 
 ```
 pip install maturin
 ```
 
-and you need also the **NiFpga.dll** and the **NiFpga.lib** in the project folder.
-
-### Missing libraries ###
- How to solve `note: LINK : fatal error LNK1181: cannot open input file NiFpga.lib` ?
-
-The nifpga-rs compilation needs `NiFpga.lib`. Unfortunatly, NI distribute with LabView only the `NiFpga.dll` and not the `.lib`.
-You will find it on `C:\Windows\SysWOW64` or `C:\Windows\System32`.
-The `nifpga.lib` can be generated starting from the `nifpga.dll` the following steps.
-
-Create a folder and copy there `nifpga.dll` file. Then from the Visual Studio developer Powershell open `cmd.exe`
-
-```
-cmd
-cd C:\THEFOLDER
-```
-
-then go in the folder where you have copied `nifpga.dll`
-
-```
-echo LIBRARY NIFPGA > nifpga.def
-echo EXPORTS >> nifpga.def
-for /f "skip=19 tokens=4" %A in ('dumpbin /exports nifpga.dll') do echo %A >> nifpga.def
-```
-
-once the process is done
-
-```
-lib /def:nifpga.def /out:nifpga.lib /machine:x64
-```
-
-Now you can copy the `nifpga.lib` to the rust project folder and be able to compile it.
-
-### Compile the module ###
-
-```
-maturin develop
-```
-Now you can import from python
-```
-import nifpga_fast_fifo_recv 
-```
-
+and you need also the **NiFpga.dll** installed in your system.
 
 # License #
 Copyright (c) 2023 Mattia Donato
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
@@ -171,7 +144,8 @@
 OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
+
```

### Comparing `nifpga_fast_fifo_recv-0.99.2/pyproject.toml` & `nifpga_fast_fifo_recv-0.99.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.2/src/lib.rs` & `nifpga_fast_fifo_recv-0.99.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.2/Cargo.lock` & `nifpga_fast_fifo_recv-0.99.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
  "libc",
  "nifpga-sys",
  "nifpga-type-macro",
 ]
 
 [[package]]
 name = "nifpga-fast-fifo-recv"
-version = "0.99.2"
+version = "0.99.3"
 dependencies = [
  "cc",
  "crossbeam",
  "nifpga",
  "nifpga-sys",
  "nifpga-type-macro",
  "pyo3",
```

### Comparing `nifpga_fast_fifo_recv-0.99.2/PKG-INFO` & `nifpga_fast_fifo_recv-0.99.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: nifpga-fast-fifo-recv
-Version: 0.99.2
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-License-File: LICENSE
-Summary: A Python module for fast reading of data from NI FPGA FIFOs with a separate thread.
-Author: Mattia Donato
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, https://github.com/mattia-donato/nifpga-fast-fifo-recv
-
 # nifpga-fast-fifo-recv
 A Python module for fast reading of data from NI FPGA FIFOs with a separate thread.
 
 This module provides in Python a class and the methods to start a separate thread which acquire continously 
 data and store them into a queue which can be read asynchronously. 
 This allows to receive data from NI FPGA in Python ideally without loosing data even for fast data-rate.
 
@@ -118,56 +104,15 @@
 
 In order to compile this project you need *maturin* 
 
 ```
 pip install maturin
 ```
 
-and you need also the **NiFpga.dll** and the **NiFpga.lib** in the project folder.
-
-### Missing libraries ###
- How to solve `note: LINK : fatal error LNK1181: cannot open input file NiFpga.lib` ?
-
-The nifpga-rs compilation needs `NiFpga.lib`. Unfortunatly, NI distribute with LabView only the `NiFpga.dll` and not the `.lib`.
-You will find it on `C:\Windows\SysWOW64` or `C:\Windows\System32`.
-The `nifpga.lib` can be generated starting from the `nifpga.dll` the following steps.
-
-Create a folder and copy there `nifpga.dll` file. Then from the Visual Studio developer Powershell open `cmd.exe`
-
-```
-cmd
-cd C:\THEFOLDER
-```
-
-then go in the folder where you have copied `nifpga.dll`
-
-```
-echo LIBRARY NIFPGA > nifpga.def
-echo EXPORTS >> nifpga.def
-for /f "skip=19 tokens=4" %A in ('dumpbin /exports nifpga.dll') do echo %A >> nifpga.def
-```
-
-once the process is done
-
-```
-lib /def:nifpga.def /out:nifpga.lib /machine:x64
-```
-
-Now you can copy the `nifpga.lib` to the rust project folder and be able to compile it.
-
-### Compile the module ###
-
-```
-maturin develop
-```
-Now you can import from python
-```
-import nifpga_fast_fifo_recv 
-```
-
+and you need also the **NiFpga.dll** installed in your system.
 
 # License #
 Copyright (c) 2023 Mattia Donato
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
@@ -185,8 +130,7 @@
 OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
-
```

