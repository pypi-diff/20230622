# Comparing `tmp/pyscemu-0.2.5.tar.gz` & `tmp/pyscemu-0.2.6.tar.gz`

## Comparing `pyscemu-0.2.5.tar` & `pyscemu-0.2.6.tar`

### file list

```diff
@@ -1,76 +1,17 @@
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 pyscemu-0.2.5/local_dependencies/libscemu/Cargo.toml
--rw-r--r--   0     1000     1000       20 2023-02-08 08:58:52.000000 pyscemu-0.2.5/local_dependencies/libscemu/.gitignore
--rw-r--r--   0     1000     1000     3756 2023-05-10 08:34:06.000000 pyscemu-0.2.5/local_dependencies/libscemu/README.md
--rw-r--r--   0     1000     1000     2111 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/config.rs
--rw-r--r--   0     1000     1000   207596 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/banzai.rs
--rw-r--r--   0     1000     1000     1415 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/breakpoint.rs
--rw-r--r--   0     1000     1000     2136 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/colors.rs
--rw-r--r--   0     1000     1000     6119 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/console.rs
--rw-r--r--   0     1000     1000    21322 2023-06-15 13:48:58.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/constants.rs
--rw-r--r--   0     1000     1000     4531 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/context32.rs
--rw-r--r--   0     1000     1000     7059 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/context64.rs
--rw-r--r--   0     1000     1000      325 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/eflags.rs
--rw-r--r--   0     1000     1000     6381 2023-06-21 15:56:00.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/elf32.rs
--rw-r--r--   0     1000     1000        0 2023-05-22 16:19:13.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/elf64.rs
--rw-r--r--   0     1000     1000     5774 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/endpoint.rs
--rw-r--r--   0     1000     1000      438 2023-05-10 08:02:00.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/err.rs
--rw-r--r--   0     1000     1000      529 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/exception.rs
--rw-r--r--   0     1000     1000    41937 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/flags.rs
--rw-r--r--   0     1000     1000     3934 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/fpu.rs
--rw-r--r--   0     1000     1000     3304 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/hook.rs
--rw-r--r--   0     1000     1000    28890 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/inline.rs
--rw-r--r--   0     1000     1000     2294 2023-06-15 13:48:58.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/macros.rs
--rw-r--r--   0     1000     1000     5696 2023-02-08 08:58:52.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/maps/mem.rs.bkp
--rw-r--r--   0     1000     1000     8070 2023-06-15 13:48:58.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/maps/mem64.rs
--rw-r--r--   0     1000     1000    29894 2023-06-15 13:48:58.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/maps.rs
--rw-r--r--   0     1000     1000    27696 2023-06-15 13:48:58.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/pe32.rs
--rw-r--r--   0     1000     1000    15371 2023-06-15 13:48:58.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/pe64.rs
--rw-r--r--   0     1000     1000    12205 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/peb32.rs
--rw-r--r--   0     1000     1000    10597 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/peb64.rs
--rw-r--r--   0     1000     1000    59842 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/regs64.rs
--rw-r--r--   0     1000     1000    40512 2023-05-09 16:52:48.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/script.rs
--rw-r--r--   0     1000     1000    45055 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/structures.rs
--rw-r--r--   0     1000     1000    77207 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/syscall32.rs
--rw-r--r--   0     1000     1000    31568 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/syscall64.rs
--rw-r--r--   0     1000     1000     3811 2023-05-09 08:49:01.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/advapi32.rs
--rw-r--r--   0     1000     1000     3418 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/crypt32.rs
--rw-r--r--   0     1000     1000     1566 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/dnsapi.rs
--rw-r--r--   0     1000     1000     2562 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/helper.rs
--rw-r--r--   0     1000     1000   100743 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/kernel32.rs
--rw-r--r--   0     1000     1000      608 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/mscoree.rs
--rw-r--r--   0     1000     1000     4907 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/msvcrt.rs
--rw-r--r--   0     1000     1000    31754 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/ntdll.rs
--rw-r--r--   0     1000     1000     1998 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/oleaut32.rs
--rw-r--r--   0     1000     1000      400 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/shlwapi.rs
--rw-r--r--   0     1000     1000     1449 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/user32.rs
--rw-r--r--   0     1000     1000    23249 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/wininet.rs
--rw-r--r--   0     1000     1000    15159 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32/ws2_32.rs
--rw-r--r--   0     1000     1000     1546 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi32.rs
--rw-r--r--   0     1000     1000     1465 2023-05-09 07:18:21.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi64/advapi32.rs
--rw-r--r--   0     1000     1000      461 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi64/dnsapi.rs
--rw-r--r--   0     1000     1000    60676 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi64/kernel32.rs
--rw-r--r--   0     1000     1000    21740 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi64/ntdll.rs
--rw-r--r--   0     1000     1000     1063 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi64/user32.rs
--rw-r--r--   0     1000     1000      460 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi64/winhttp.rs
--rw-r--r--   0     1000     1000    16787 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi64/wininet.rs
--rw-r--r--   0     1000     1000    11038 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi64/ws2_32.rs
--rw-r--r--   0     1000     1000     1289 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu/winapi64.rs
--rw-r--r--   0     1000     1000   401454 2023-06-21 15:52:13.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/emu.rs
--rw-r--r--   0     1000     1000     1414 2023-05-09 07:13:40.000000 pyscemu-0.2.5/local_dependencies/libscemu/src/lib.rs
--rw-r--r--   0        0        0      312 1970-01-01 00:00:00.000000 pyscemu-0.2.5/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.5/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.5/.gitignore
--rw-r--r--   0     1000     1000    11699 2023-05-10 08:42:26.000000 pyscemu-0.2.5/DOCUMENTATION.md
--rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.5/README.md
--rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.5/examples/danabot_rsa.ipynb
--rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.5/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.5/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.5/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.5/examples/scripts/test.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.5/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.5/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.5/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.5/pyproject.toml
--rw-r--r--   0     1000     1000    26649 2023-06-21 15:56:51.000000 pyscemu-0.2.5/src/lib.rs
--rw-r--r--   0     1000     1000    32606 2023-06-21 16:06:10.000000 pyscemu-0.2.5/Cargo.lock
--rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 pyscemu-0.2.6/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.2.6/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.2.6/.gitignore
+-rw-r--r--   0     1000     1000    11699 2023-05-10 08:42:26.000000 pyscemu-0.2.6/DOCUMENTATION.md
+-rw-r--r--   0     1000     1000    10083 2023-05-09 16:58:06.000000 pyscemu-0.2.6/README.md
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.2.6/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.2.6/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.2.6/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.2.6/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      766 2023-05-09 15:35:14.000000 pyscemu-0.2.6/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.2.6/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      427 2023-05-10 08:13:44.000000 pyscemu-0.2.6/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.2.6/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.2.6/pyproject.toml
+-rw-r--r--   0     1000     1000    26649 2023-06-21 15:56:51.000000 pyscemu-0.2.6/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-06-22 08:41:07.000000 pyscemu-0.2.6/Cargo.lock
+-rw-r--r--   0        0        0    10409 1970-01-01 00:00:00.000000 pyscemu-0.2.6/PKG-INFO
```

### Comparing `pyscemu-0.2.5/.github/workflows/CI.yml` & `pyscemu-0.2.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/.gitignore` & `pyscemu-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/DOCUMENTATION.md` & `pyscemu-0.2.6/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/README.md` & `pyscemu-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/examples/danabot_rsa.ipynb` & `pyscemu-0.2.6/examples/danabot_rsa.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/examples/raccoon_strings.ipynb` & `pyscemu-0.2.6/examples/raccoon_strings.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/examples/scripts/raccoon_strings.py` & `pyscemu-0.2.6/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/examples/scripts/test.py` & `pyscemu-0.2.6/examples/scripts/test.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/examples/scripts/xloader_dexor.py` & `pyscemu-0.2.6/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/examples/xloader_keygen.ipynb` & `pyscemu-0.2.6/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/src/lib.rs` & `pyscemu-0.2.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyscemu-0.2.5/Cargo.lock` & `pyscemu-0.2.6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -394,15 +394,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.12.5"
+version = "0.12.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7884c09bc473386eec552c11d73d4420363e7dac4023ecfd19b7e878efa31c18"
 dependencies = [
  "attohttpc",
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
@@ -682,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.2.5/PKG-INFO` & `pyscemu-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.2.5
+Version: 0.2.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
```

