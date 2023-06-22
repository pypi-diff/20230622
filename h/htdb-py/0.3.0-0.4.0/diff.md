# Comparing `tmp/htdb-py-0.3.0.tar.gz` & `tmp/htdb-py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htdb-py-0.3.0.tar", last modified: Sun Jun 18 10:00:04 2023, max compression
+gzip compressed data, was "htdb-py-0.4.0.tar", last modified: Thu Jun 22 11:10:29 2023, max compression
```

## Comparing `htdb-py-0.3.0.tar` & `htdb-py-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 10:00:04.000000 htdb-py-0.3.0/
--rw-rw-rw-   0        0        0    11558 2023-06-17 09:16:02.000000 htdb-py-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       18 2023-06-17 09:35:40.000000 htdb-py-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      123 2023-06-18 10:00:06.000000 htdb-py-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb/
--rw-rw-rw-   0        0        0    13080 2023-06-18 09:39:28.000000 htdb-py-0.3.0/htdb/dict.c
--rw-rw-rw-   0        0        0     2705 2023-06-17 08:31:04.000000 htdb-py-0.3.0/htdb/dict.h
--rw-rw-rw-   0        0        0     8088 2023-06-18 09:55:42.000000 htdb-py-0.3.0/htdb/htdb.c
--rw-rw-rw-   0        0        0     1672 2023-06-17 08:31:04.000000 htdb-py-0.3.0/htdb/htdb.h
--rw-rw-rw-   0        0        0    14397 2023-06-14 11:09:50.000000 htdb-py-0.3.0/htdb/siphash.c
--rw-rw-rw-   0        0        0      254 2023-06-15 13:51:52.000000 htdb-py-0.3.0/htdb/siphash.h
-drwxrwxrwx   0        0        0        0 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/
--rw-rw-rw-   0        0        0      123 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 09:04:40.000000 htdb-py-0.3.0/htdb_py.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-06-17 09:30:36.000000 htdb-py-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 10:00:06.000000 htdb-py-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      548 2023-06-18 09:59:02.000000 htdb-py-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 10:00:04.000000 htdb-py-0.3.0/src/
--rw-rw-rw-   0        0        0     5278 2023-06-18 08:08:34.000000 htdb-py-0.3.0/src/bindings.cpp
+drwxrwxrwx   0        0        0        0 2023-06-22 11:10:30.000000 htdb-py-0.4.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-17 09:16:02.000000 htdb-py-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-06-17 09:35:40.000000 htdb-py-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      123 2023-06-22 11:10:30.000000 htdb-py-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb/
+-rw-rw-rw-   0        0        0    13075 2023-06-19 14:03:48.000000 htdb-py-0.4.0/htdb/dict.c
+-rw-rw-rw-   0        0        0     2705 2023-06-17 08:31:04.000000 htdb-py-0.4.0/htdb/dict.h
+-rw-rw-rw-   0        0        0     8066 2023-06-18 10:00:50.000000 htdb-py-0.4.0/htdb/htdb.c
+-rw-rw-rw-   0        0        0     1672 2023-06-17 08:31:04.000000 htdb-py-0.4.0/htdb/htdb.h
+-rw-rw-rw-   0        0        0    14397 2023-06-14 11:09:50.000000 htdb-py-0.4.0/htdb/siphash.c
+-rw-rw-rw-   0        0        0      254 2023-06-15 13:51:52.000000 htdb-py-0.4.0/htdb/siphash.h
+drwxrwxrwx   0        0        0        0 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/
+-rw-rw-rw-   0        0        0      123 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 09:04:40.000000 htdb-py-0.4.0/htdb_py.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-22 11:10:30.000000 htdb-py-0.4.0/htdb_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-06-17 09:30:36.000000 htdb-py-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 11:10:30.000000 htdb-py-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      548 2023-06-22 11:07:56.000000 htdb-py-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 11:10:30.000000 htdb-py-0.4.0/src/
+-rw-rw-rw-   0        0        0     6109 2023-06-21 13:56:08.000000 htdb-py-0.4.0/src/bindings.cpp
```

### Comparing `htdb-py-0.3.0/LICENSE` & `htdb-py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htdb-py-0.3.0/htdb/dict.c` & `htdb-py-0.4.0/htdb/dict.c`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #include <stdio.h>
 #include <stdint.h>
 #include <stdbool.h>
 #include <assert.h>
 #include <string.h>
 #include "dict.h"
 
-typedef int32_t ix_t;
+typedef int64_t ix_t;
 
 #define DKIX_EMPTY (-1)
 #define DKIX_DUMMY (-2)
 
 #define USABLE_FRACTION(n) (((n) << 1)/3)
 #define GROWTH_RATE(dict)  ((dict)->used*3)
 
@@ -308,15 +308,15 @@
     DictKeyEntry* ep0 = DK_ENTRIES(dk);
     size_t perturb = (size_t)hash;
     size_t size = DK_SIZE(dk);
     // size_t i = hash % size;
     size_t mask = DK_MASK(dk);
     size_t i = (size_t)hash & mask;
     for (; ; ) {
-        ix_t ix = _DictKeys_GetIndex(dk, i);
+        ix = _DictKeys_GetIndex(dk, i);
         if (ix >= 0) {
             DictKeyEntry* ep = &ep0[ix];
             if (dk->keyCmpFunc(ep->key, key) == 1) {
                 return ix;
             }
         } else if (ix == DKIX_DUMMY) {
             if (!skip_dummy) {
```

### Comparing `htdb-py-0.3.0/htdb/dict.h` & `htdb-py-0.4.0/htdb/dict.h`

 * *Files identical despite different names*

### Comparing `htdb-py-0.3.0/htdb/htdb.c` & `htdb-py-0.4.0/htdb/htdb.c`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         fwrite(&valobj->len, sizeof(xobjlen_t), 1, stream);
         fwrite(keyobj->data, keyobj->len, 1, stream);
         fwrite(valobj->data, valobj->len, 1, stream);
     }
 }
 
 void xdbLoad(xdb *db, FILE *stream) {
-    char start_mark;
     uint8_t key_type, value_type;
     xobjlen_t key_len, value_len;
     char *data_buffer = (char *)malloc(65535);  // the max size of xobjlen_t
 
     while (fgetc(stream) == RECORD_START_MARK) {
 
         fread(&key_type, sizeof(uint8_t), 1, stream);
```

### Comparing `htdb-py-0.3.0/htdb/htdb.h` & `htdb-py-0.4.0/htdb/htdb.h`

 * *Files identical despite different names*

### Comparing `htdb-py-0.3.0/htdb/siphash.c` & `htdb-py-0.4.0/htdb/siphash.c`

 * *Files identical despite different names*

### Comparing `htdb-py-0.3.0/setup.py` & `htdb-py-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import glob
 
 from setuptools import setup
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 
 ext_modules=[
     Pybind11Extension(
         name="htdb",
         sources=sorted(glob.glob("htdb/*.c")) + sorted(glob.glob("src/*.cpp")),
         include_dirs=["htdb/"],
```

### Comparing `htdb-py-0.3.0/src/bindings.cpp` & `htdb-py-0.4.0/src/bindings.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 #include <iostream>
 #include <stdio.h>
 
 namespace py = pybind11;
 using namespace pybind11::literals;
 
 
+auto _xobj2pyobj(xobj *obj) -> py::object {
+    py::object pyobj;
+    if (obj->type == XOBJ_TYPE_INT) {
+        pyobj = py::int_(*(uint64_t *)obj->data);
+    } else if (obj->type == XOBJ_TYPE_BYTES) {
+        pyobj = py::bytes((char *)obj->data, obj->len);
+    } else {
+        throw std::runtime_error("err: unknown value type");
+    }
+    return pyobj;
+}
+
+
 class Htdb {
 public:
     Htdb() {
         _db = xdbNew(0, 0);
     }
     ~Htdb() {
         xdbFree(_db);
@@ -130,14 +143,30 @@
         xdbLoad(_db, fp);
         fclose(fp);
     }
 
     auto load(std::filesystem::path filename) -> void {
         load(filename.string());
     }
+
+    auto getDataList() -> py::list {
+        py::list ret;
+
+        DictIter iter = {_db->table, 0};
+        xobj *keyobj, *valobj;
+
+        for (; dictIterNext(&iter, (void **)&keyobj, (void **)&valobj);) {
+            py::object key = _xobj2pyobj(keyobj);
+            py::object value = _xobj2pyobj(valobj);
+
+            ret.append(py::make_tuple(key, value));
+        }
+
+        return ret;
+    }
 private:
     xdb *_db;
 };
 
 PYBIND11_MODULE(htdb, m) {
     py::class_<Htdb>(m, "Htdb")
         .def(py::init<>())
@@ -147,9 +176,10 @@
         .def("remove", &Htdb::remove)
         .def("dump", static_cast<void (Htdb::*)(std::string)>(&Htdb::dump), "filename"_a = "")
         .def("dump", static_cast<void (Htdb::*)(std::filesystem::path)>(&Htdb::dump), "filename"_a)
         .def("load", static_cast<void (Htdb::*)(std::string)>(&Htdb::load), "filename"_a)
         .def("load", static_cast<void (Htdb::*)(std::filesystem::path)>(&Htdb::load), "filename"_a)
         .def("__len__", &Htdb::getSize)
         .def("__contains__", &Htdb::has)
+        .def("list", &Htdb::getDataList)
     ;
 }
```

