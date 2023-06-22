# Comparing `tmp/nifpga_fast_fifo_recv-0.99.0.tar.gz` & `tmp/nifpga_fast_fifo_recv-0.99.1.tar.gz`

## Comparing `nifpga_fast_fifo_recv-0.99.0.tar` & `nifpga_fast_fifo_recv-0.99.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.0/Cargo.toml
--rw-r--r--   0        0        0     1081 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.0/LICENSE
--rw-r--r--   0        0        0     6175 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.0/README.md
--rw-r--r--   0        0        0      561 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.0/pyproject.toml
--rw-r--r--   0        0        0        9 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.0/requirements.txt
--rw-r--r--   0        0        0     7728 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.0/src/lib.rs
--rw-r--r--   0        0        0    10405 2023-06-21 09:32:50.000000 nifpga_fast_fifo_recv-0.99.0/Cargo.lock
--rw-r--r--   0        0        0     6749 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.0/PKG-INFO
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.1/Cargo.toml
+-rw-r--r--   0        0        0     1081 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.1/LICENSE
+-rw-r--r--   0        0        0     6175 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.1/README.md
+-rw-r--r--   0        0        0      561 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.1/pyproject.toml
+-rw-r--r--   0        0        0        9 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.1/requirements.txt
+-rw-r--r--   0        0        0     7728 2023-06-21 09:29:18.000000 nifpga_fast_fifo_recv-0.99.1/src/lib.rs
+-rw-r--r--   0        0        0    10405 2023-06-22 09:36:16.000000 nifpga_fast_fifo_recv-0.99.1/Cargo.lock
+-rw-r--r--   0        0        0     6749 1970-01-01 00:00:00.000000 nifpga_fast_fifo_recv-0.99.1/PKG-INFO
```

### Comparing `nifpga_fast_fifo_recv-0.99.0/Cargo.toml` & `nifpga_fast_fifo_recv-0.99.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "nifpga-fast-fifo-recv"
 readme = "README.md"
-version = "0.99.0"
+version = "0.99.1"
 edition = "2021"
 license = "MIT"
 authors = ["Mattia Donato"]
 description = "A Python module for fast reading of data from NI FPGA FIFOs with a separate thread."
 repository = "https://github.com/mattia-donato/nifpga-fast-fifo-recv"
 exclude = ["nifpga.*", "NiFpga.*", ".idea/*" ]
```

### Comparing `nifpga_fast_fifo_recv-0.99.0/LICENSE` & `nifpga_fast_fifo_recv-0.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.0/README.md` & `nifpga_fast_fifo_recv-0.99.1/README.md`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.0/pyproject.toml` & `nifpga_fast_fifo_recv-0.99.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.0/src/lib.rs` & `nifpga_fast_fifo_recv-0.99.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nifpga_fast_fifo_recv-0.99.0/Cargo.lock` & `nifpga_fast_fifo_recv-0.99.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -142,47 +142,47 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "nifpga"
-version = "0.1.4"
-source = "git+https://github.com/mattia-donato/nifpga-win-rs#69a287546b93de3fb9df182886a1631b4cc7adb4"
+version = "0.1.5"
+source = "git+https://github.com/mattia-donato/nifpga-win-rs#bf61ce6523a4f5fa29580788675b7016a4d9f99f"
 dependencies = [
  "fehler",
  "libc",
  "nifpga-sys",
  "nifpga-type-macro",
 ]
 
 [[package]]
 name = "nifpga-fast-fifo-recv"
-version = "0.99.0"
+version = "0.99.1"
 dependencies = [
  "cc",
  "crossbeam",
  "nifpga",
  "nifpga-sys",
  "nifpga-type-macro",
  "pyo3",
 ]
 
 [[package]]
 name = "nifpga-sys"
-version = "0.1.4"
-source = "git+https://github.com/mattia-donato/nifpga-win-rs#69a287546b93de3fb9df182886a1631b4cc7adb4"
+version = "0.1.5"
+source = "git+https://github.com/mattia-donato/nifpga-win-rs#bf61ce6523a4f5fa29580788675b7016a4d9f99f"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "nifpga-type-macro"
-version = "0.1.4"
-source = "git+https://github.com/mattia-donato/nifpga-win-rs#69a287546b93de3fb9df182886a1631b4cc7adb4"
+version = "0.1.5"
+source = "git+https://github.com/mattia-donato/nifpga-win-rs#bf61ce6523a4f5fa29580788675b7016a4d9f99f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `nifpga_fast_fifo_recv-0.99.0/PKG-INFO` & `nifpga_fast_fifo_recv-0.99.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifpga-fast-fifo-recv
-Version: 0.99.0
+Version: 0.99.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: A Python module for fast reading of data from NI FPGA FIFOs with a separate thread.
 Author: Mattia Donato
 License: MIT
```

