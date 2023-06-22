# Comparing `tmp/bkv-0.0.1.tar.gz` & `tmp/bkv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkv-0.0.1.tar", last modified: Thu Jun 22 06:51:56 2023, max compression
+gzip compressed data, was "bkv-0.0.2.tar", last modified: Thu Jun 22 08:54:00 2023, max compression
```

## Comparing `bkv-0.0.1.tar` & `bkv-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 06:51:56.226652 bkv-0.0.1/
--rw-rw-rw-   0        0        0      608 2023-06-22 06:51:56.225650 bkv-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-06-22 04:47:10.000000 bkv-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 06:51:56.210631 bkv-0.0.1/bkv/
--rw-rw-rw-   0        0        0     1554 2023-06-22 06:28:10.000000 bkv-0.0.1/bkv/__init__.py
--rw-rw-rw-   0        0        0     6126 2023-06-22 06:27:09.000000 bkv-0.0.1/bkv/file_store.py
--rw-rw-rw-   0        0        0     4682 2023-06-22 04:29:19.000000 bkv-0.0.1/bkv/mem_store.py
--rw-rw-rw-   0        0        0     2235 2023-06-22 06:44:57.000000 bkv-0.0.1/bkv/shell.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:51:56.225650 bkv-0.0.1/bkv.egg-info/
--rw-rw-rw-   0        0        0      608 2023-06-22 06:51:55.000000 bkv-0.0.1/bkv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-22 06:51:55.000000 bkv-0.0.1/bkv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 06:51:55.000000 bkv-0.0.1/bkv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-22 06:51:55.000000 bkv-0.0.1/bkv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 06:51:56.226652 bkv-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-06-22 06:49:37.000000 bkv-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:54:00.043896 bkv-0.0.2/
+-rw-rw-rw-   0        0        0      675 2023-06-22 08:54:00.043896 bkv-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-22 07:06:35.000000 bkv-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 08:54:00.023671 bkv-0.0.2/bkv/
+-rw-rw-rw-   0        0        0     1884 2023-06-22 08:36:07.000000 bkv-0.0.2/bkv/__init__.py
+-rw-rw-rw-   0        0        0     7090 2023-06-22 08:47:47.000000 bkv-0.0.2/bkv/file_store.py
+-rw-rw-rw-   0        0        0     4409 2023-06-22 08:46:42.000000 bkv-0.0.2/bkv/mem_store.py
+-rw-rw-rw-   0        0        0     2766 2023-06-22 08:37:11.000000 bkv-0.0.2/bkv/shell.py
+-rw-rw-rw-   0        0        0      369 2023-06-22 08:16:21.000000 bkv-0.0.2/bkv/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:54:00.033069 bkv-0.0.2/bkv.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-06-22 08:53:59.000000 bkv-0.0.2/bkv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-06-22 08:53:59.000000 bkv-0.0.2/bkv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:53:59.000000 bkv-0.0.2/bkv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-22 08:53:59.000000 bkv-0.0.2/bkv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 08:54:00.044899 bkv-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      885 2023-06-22 08:53:53.000000 bkv-0.0.2/setup.py
```

### Comparing `bkv-0.0.1/bkv/__init__.py` & `bkv-0.0.2/bkv/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # -*- coding:utf-8 -*-
 '''
 Author: xupingmao
 email: 578749341@qq.com
 Date: 2023-06-22 12:23:46
 LastEditors: xupingmao
-LastEditTime: 2023-06-22 14:27:17
-FilePath: \bkv\bkv\__init__.py
+LastEditTime: 2023-06-22 16:36:07
+FilePath: /bkv/bkv/__init__.py
 Description: 键值对存储，基于Bitcask模型
 '''
 import threading
-from bkv.file_store import MetaFile, StoreFile
+from bkv.file_store import MetaFile, DataFile
+from bkv import utils
 
 class DB:
-    def __init__(self, db_dir = "./data"):
+    def __init__(self, db_dir = "./data", **kw):
         self.db_dir = db_dir
         self.meta = MetaFile(db_dir)
-        self.store = StoreFile(db_dir, self.meta.meta.store_file)
+        self.store = DataFile(db_dir, self.meta.meta.data_file, **kw)
         self.lock = threading.RLock()
     
     def compact(self):
         with self.lock:
-            new_file = self.meta.create_new_store_file()
-            new_store = StoreFile(self.db_dir, new_file)
-            for key, pos_str in self.store.mem_store._data:
+            new_file = self.meta.create_new_data_file()
+            new_store = DataFile(self.db_dir, new_file)
+            for key, pos_int in self.store.mem_store._data:
                 val = self.get(key)
                 if val != None:
                     new_store.put(key, val)
             # 先更新meta信息
-            self.meta.meta.store_file = new_file
+            self.meta.meta.data_file = new_file
             self.meta.save()
 
             # 更新成功后删除文件
             old_store = self.store
             old_store.delete_file()
             self.store = new_store
     
@@ -44,9 +45,21 @@
     
     def put(self, key, value):
         return self.store.put(key, value)
     
     def delete(self, key):
         return self.store.delete(key)
     
+    def count(self):
+        return self.store.count()
+    
+    def memory_info(self):
+        return utils.memory_info()
+    
+    def avg_key_len(self):
+        return self.store.avg_key_len()
+    
+    def keys(self, key, limit=100):
+        return self.store.keys(key, limit=limit)
+    
     def close(self):
         self.store.close()
```

### Comparing `bkv-0.0.1/bkv/file_store.py` & `bkv-0.0.2/bkv/file_store.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 """
 
 import json
 import os
 import datetime
 import time
 import threading
+import fnmatch
 from bkv.mem_store import MemoryKvStore
+from bkv import utils
 
 class StoreItem:
     def __init__(self):
         self.k = ""
         self.v = ""
         self.d = 0 # 删除标记
 
 class StoreMeta:
     def __init__(self):
         self.version = ""
         self.create_time = ""
-        self.store_file = ""
+        self.data_file = ""
 
 def format_datetime(value=None, format='%Y-%m-%d %H:%M:%S'):
     """格式化日期时间
     >>> format_datetime(0)
     '1970-01-01 08:00:00'
     """
     if value == None:
@@ -40,15 +42,15 @@
     else:
         st = time.localtime(value)
         return time.strftime(format, st)
 
 class MetaFile:
 
     meta_version = "1.0.0"
-    default_store_file = "data.txt"
+    default_data_file = "data-0.txt"
 
     def __init__(self, db_dir="./data"):
         meta_file = "./meta.txt"
         self.db_dir = db_dir
         self.meta_file = os.path.join(db_dir, meta_file)
         self.load_meta_file()
 
@@ -68,82 +70,91 @@
                 self.meta = self._load_meta(json_text)
             assert self.meta.version == self.meta_version, "broken meta"
 
     def create_meta(self):
         with open(self.meta_file, "w+") as fp:
             meta = StoreMeta()
             meta.version = self.meta_version
-            meta.store_file = self.default_store_file
+            meta.data_file = self.default_data_file
             meta.create_time = format_datetime()
             fp.write(json.dumps(meta.__dict__))
             fp.flush()
             return meta
             
     
     def _load_meta(self, json_str):
         json_dict = json.loads(json_str)
         item = StoreMeta()
         item.__dict__.update(json_dict)
-        if item.store_file == "":
-            item.store_file = "data-0.txt"
+        if item.data_file == "":
+            item.data_file = "data-0.txt"
         return item
     
     def save(self):
         with open(self.meta_file, "w+") as fp:
             fp.write(json.dumps(self.meta.__dict__))
     
-    def create_new_store_file(self):
+    def create_new_data_file(self):
         for i in range(100):
             fname = "data-%d.txt" % i
             fpath = os.path.join(self.db_dir, fname)
             if not os.path.exists(fpath):
                 return fname
         raise Exception("too many store files")
     
     def delete_old_data_files(self):
         for i in range(100):
             fname = "data-%d.txt" % i
             fpath = os.path.join(self.db_dir, fname)
-            if os.path.exists(fpath) and fname != self.meta.store_file:
+            if os.path.exists(fpath) and fname != self.meta.data_file:
                 print("found old data file:", fname)
 
-class StoreFile:
+class DataFile:
     """db存储，管理1个存储文件"""
 
-    def __init__(self, db_dir="./data", store_file="./data-1.txt"):
-        self.mem_store = MemoryKvStore()        
+    def __init__(self, db_dir="./data", data_file="./data-1.txt", **kw):
+        self.mem_store = MemoryKvStore(default_value=0)        
         self.last_pos = 0
         self.db_dir = db_dir
-        self.store_file = store_file
+        self.data_file = data_file
+        self.print_load_stats = kw.get("print_load_stats", False)
         self.load_data_file()
         self.lock = threading.RLock()
 
 
     def load_data_file(self):
         if not os.path.exists(self.db_dir):
             os.makedirs(self.db_dir)
     
-        fpath = os.path.join(self.db_dir, self.store_file)
+        fpath = os.path.join(self.db_dir, self.data_file)
         if not os.path.exists(fpath):
             with open(fpath, "w+") as fp:
                 pass
         
         with open(fpath, "r+") as fp:
+            count = 0
             while True:
                 pos = fp.tell()
                 line = fp.readline()
                 if line.strip() == "":
                     break
                 line_data = self._load_item(line)
                 key = line_data.k
                 if line_data.d == 1:
                     # 已删除
                     self.mem_store.delete(key)
                 else:
-                    self.mem_store.put(key, str(pos))
+                    self.mem_store.put(key, pos)
+                
+                count+=1
+                if self.print_load_stats and count % 10000 == 0:
+                    mem_info = utils.memory_info()
+                    keys = len(self.mem_store)
+                    rss = mem_info.rss/1024/1024
+                    print(f"keys:({keys}), memory:({rss:.2f}MB)")
         
         self.write_fp = open(fpath, "a+")
         self.last_pos = self.write_fp.tell()
     
     def _load_item(self, json_str):
         json_dict = json.loads(json_str)
         item = StoreItem()
@@ -161,38 +172,56 @@
         self.write_fp.write("\n")
         self.write_fp.flush()
         self.last_pos = self.write_fp.tell()
     
     def close(self):
         self.write_fp.close()
     
-    def get(self, key, **kw):
-        pos_str = self.mem_store.get(key, **kw)
-        if pos_str == None:
+    def get(self, key):
+        pos_int = self.mem_store.get(key)
+        if pos_int == None:
             return None
-        self.write_fp.seek(int(pos_str))
+        self.write_fp.seek(pos_int)
         line_str = self.write_fp.readline()
         return json.loads(line_str).get("v")
     
-    def put(self, key, val, **kw):
-        pos = self.write_fp.tell()
+    def put(self, key, val):
+        pos_int = self.write_fp.tell()
         exist = self.get(key)
         if exist == val:
             # 没变化
             return
         with self.lock:
-            self.mem_store.put(key, str(pos), **kw)
+            self.mem_store.put(key, pos_int)
             self.write(key, val)
 
     def delete(self, key):
         exist = self.get(key)
         if exist == None:
             # 已经删除
             return
         with self.lock:
             self.mem_store.delete(key)
             self.write(key=key, delete=1)
 
+    def count(self):
+        return len(self.mem_store)
+
+    def avg_key_len(self):
+        length = 0
+        for key, pos in self.mem_store._data:
+            length += len(key)
+        return length / len(self.mem_store)
+
+    def keys(self, key, limit=100):
+        result = []
+        for store_key, pos in self.mem_store._data:
+            if fnmatch.fnmatch(store_key, key):
+                result.append(store_key)
+                if len(result) >= limit:
+                    break
+        return result
+
     def delete_file(self):
         self.write_fp.close()
-        fpath = os.path.join(self.db_dir, self.store_file)
+        fpath = os.path.join(self.db_dir, self.data_file)
         os.remove(fpath)
```

### Comparing `bkv-0.0.1/bkv/mem_store.py` & `bkv-0.0.2/bkv/mem_store.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,19 @@
 # -*- coding:utf-8 -*-
+'''
+Author: xupingmao
+email: 578749341@qq.com
+Date: 2023-06-22 12:24:53
+LastEditors: xupingmao
+LastEditTime: 2023-06-22 16:44:51
+FilePath: /bkv/bkv/mem_store.py
+Description: 键值对存储，基于Bitcask模型, copied from leveldbpy
+'''
+
+# -*- coding:utf-8 -*-
 #!/usr/bin/env python
 #
 # Copyright (C) 2012 Space Monkey, Inc.
 #               2023 xupingmao 578749341@qq.com
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
@@ -19,74 +30,59 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
-"""
-@Author       : xupingmao
-@email        : 578749341@qq.com
-@Date         : 2023-02-01 23:15:02
-@LastEditors  : xupingmao
-@LastEditTime : 2023-02-05 13:45:55
-@FilePath     : /xnoted:/projects/learn-python/src/storage/my_kv.py
-@Description  : 键值对存储，基于Bitcask模型, copied from leveldbpy
-"""
 import bisect
 import threading
 
 
 class MemoryKvStore(object):
 
-    __slots__ = ["_data", "_lock", "_is_snapshot"]
-
-    def __init__(self, data=None, is_snapshot=False):
+    def __init__(self, data=None, default_value=""):
         if data is None:
             self._data = []
         else:
             self._data = data
         self._lock = threading.RLock()
-        self._is_snapshot = is_snapshot
+        self.default_value = default_value
 
     def close(self):
         with self._lock:
             self._data = []
 
     def put(self, key, val, **_kwargs):
-        if self._is_snapshot:
-            raise TypeError("cannot put on leveldb snapshot")
         assert isinstance(key, str)
-        assert isinstance(val, str)
         with self._lock:
-            idx = bisect.bisect_left(self._data, (key, ""))
+            idx = bisect.bisect_left(self._data, (key, val))
             if 0 <= idx < len(self._data) and self._data[idx][0] == key:
                 self._data[idx] = (key, val)
             else:
                 self._data.insert(idx, (key, val))
 
     def delete(self, key, **_kwargs):
-        if self._is_snapshot:
-            raise TypeError("cannot delete on leveldb snapshot")
         with self._lock:
-            idx = bisect.bisect_left(self._data, (key, ""))
+            idx = bisect.bisect_left(self._data, (key, self.default_value))
             if 0 <= idx < len(self._data) and self._data[idx][0] == key:
                 del self._data[idx]
 
     def get(self, key, **_kwargs):
         with self._lock:
-            idx = bisect.bisect_left(self._data, (key, ""))
+            idx = bisect.bisect_left(self._data, (key, self.default_value))
             if 0 <= idx < len(self._data) and self._data[idx][0] == key:
                 return self._data[idx][1]
             return None
+        
+    def __len__(self):
+        return len(self._data)
 
     # pylint: disable=W0212
     def write(self, batch, **_kwargs):
-        if self._is_snapshot:
-            raise TypeError("cannot write on leveldb snapshot")
         with self._lock:
             for key, val in batch._puts.iteritems():
                 self.put(key, val)
             for key in batch._deletes:
                 self.delete(key)
 
     def iterator(self, **_kwargs):
@@ -104,26 +100,27 @@
 class _IteratorMemImpl(object):
 
     __slots__ = ["_data", "_idx"]
 
     def __init__(self, memdb_data):
         self._data = memdb_data
         self._idx = -1
+        self.default_value = ""
 
     def valid(self):
         return 0 <= self._idx < len(self._data)
 
     def key(self):
         return self._data[self._idx][0]
 
     def val(self):
         return self._data[self._idx][1]
 
     def seek(self, key):
-        self._idx = bisect.bisect_left(self._data, (key, ""))
+        self._idx = bisect.bisect_left(self._data, (key, self.default_value))
 
     def seekFirst(self):
         self._idx = 0
 
     def seekLast(self):
         self._idx = len(self._data) - 1
```

### Comparing `bkv-0.0.1/bkv/shell.py` & `bkv-0.0.2/bkv/shell.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding:utf-8 -*-
 '''
 Author: xupingmao
 email: 578749341@qq.com
 Date: 2023-06-22 12:42:15
 LastEditors: xupingmao
-LastEditTime: 2023-06-22 14:44:57
-FilePath: \bkv\bkv\shell.py
+LastEditTime: 2023-06-22 16:36:28
+FilePath: /bkv/bkv/shell.py
 Description: 描述
 '''
 import bkv
+import traceback
 
 class Shell:
     
     def __init__(self) -> None:
         self.db = bkv.DB(db_dir="./test-data")
 
     def loop(self):
@@ -26,15 +27,18 @@
             if op == "quit" or op == "exit":
                 print("Bye")
                 break
             
             attr = "op_" + op
             if hasattr(self, attr):
                 meth = getattr(self, attr)
-                meth(parts)
+                try:
+                    meth(parts)
+                except:
+                    traceback.print_exc()
             else:
                 self.print_help()
 
         self.db.close()
         
     def op_put(self, parts: list[str]):
         if len(parts) != 3:
@@ -66,20 +70,34 @@
     def op_delete_old_files(self, parts):
         self.db.delete_old_files()
         print("OK")
     
     def op_compact(self, parts):
         self.db.compact()
         print("OK")
+    
+    def op_memory_info(self, parts):
+        print(self.db.memory_info())
+        print("OK")
+
+    def op_keys(self, parts):
+        if len(parts) != 2:
+            print("bad keys command")
+        else:
+            key = parts[1]
+            print(self.db.keys(key))
+            print("OK")
 
     def print_help(self):
         print("bad command, supported commands:")
         print("- get $key            get value by key")
         print("- put $key $value     set value by key")
         print("- set $key $value     set value by key")
         print("- delete $key         delete key")
+        print("- keys $key           search key")
         print("- compact             compact data files")
+        print("- memory_info         print memory info")
         print()
 
 if __name__ == "__main__":
     shell = Shell()
     shell.loop()
```

### Comparing `bkv-0.0.1/setup.py` & `bkv-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding:utf-8 -*-
 '''
 Author: xupingmao xupingmao@gmail.com
 Date: 2023-03-11 13:44:52
 LastEditors: xupingmao
-LastEditTime: 2023-06-22 14:49:14
-FilePath: \bkv\setup.py
+LastEditTime: 2023-06-22 16:53:53
+FilePath: /bkv/setup.py
 Description: A simple kv store
 '''
 import setuptools
 
 with open("README.md", "r+", encoding="utf-8") as fp:
     long_description = fp.read()
 
 setuptools.setup(
     name = "bkv",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "mark",
     author_email = "578749341@qq.com",
     description  = "A simple kv store",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/xupingmao/bkv",
     packages = setuptools.find_packages(),
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires = [
-    ]
+    install_requires = []
 )
```

