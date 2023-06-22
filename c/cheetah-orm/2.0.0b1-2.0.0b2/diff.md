# Comparing `tmp/cheetah_orm-2.0.0b1-py3-none-any.whl.zip` & `tmp/cheetah_orm-2.0.0b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13741 bytes, number of entries: 13
+Zip file size: 13733 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      210 b- defN 23-Jun-22 17:56 cheetah_orm/__init__.py
 -rw-rw-rw-  2.0 fat      849 b- defN 23-Jun-08 21:21 cheetah_orm/constants.py
 -rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-08 20:36 cheetah_orm/error.py
 -rw-rw-rw-  2.0 fat     7511 b- defN 23-Jun-15 21:19 cheetah_orm/fields.py
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-Jun-08 21:21 cheetah_orm/indexes.py
 -rw-rw-rw-  2.0 fat    27471 b- defN 23-Jun-22 17:06 cheetah_orm/mappers.py
 -rw-rw-rw-  2.0 fat    14124 b- defN 23-Jun-22 17:25 cheetah_orm/migrators.py
 -rw-rw-rw-  2.0 fat     1898 b- defN 23-Jun-20 03:51 cheetah_orm/model.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-22 17:56 cheetah_orm-2.0.0b1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6765 b- defN 23-Jun-22 17:56 cheetah_orm-2.0.0b1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 17:56 cheetah_orm-2.0.0b1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-22 17:56 cheetah_orm-2.0.0b1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1047 b- defN 23-Jun-22 17:56 cheetah_orm-2.0.0b1.dist-info/RECORD
-13 files, 64074 bytes uncompressed, 12001 bytes compressed:  81.3%
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-22 18:09 cheetah_orm-2.0.0b2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6754 b- defN 23-Jun-22 18:09 cheetah_orm-2.0.0b2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 18:09 cheetah_orm-2.0.0b2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-22 18:09 cheetah_orm-2.0.0b2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1047 b- defN 23-Jun-22 18:09 cheetah_orm-2.0.0b2.dist-info/RECORD
+13 files, 64063 bytes uncompressed, 11993 bytes compressed:  81.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: cheetah_orm/migrators.py
 Comment: 
 
 Filename: cheetah_orm/model.py
 Comment: 
 
-Filename: cheetah_orm-2.0.0b1.dist-info/LICENSE
+Filename: cheetah_orm-2.0.0b2.dist-info/LICENSE
 Comment: 
 
-Filename: cheetah_orm-2.0.0b1.dist-info/METADATA
+Filename: cheetah_orm-2.0.0b2.dist-info/METADATA
 Comment: 
 
-Filename: cheetah_orm-2.0.0b1.dist-info/WHEEL
+Filename: cheetah_orm-2.0.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: cheetah_orm-2.0.0b1.dist-info/top_level.txt
+Filename: cheetah_orm-2.0.0b2.dist-info/top_level.txt
 Comment: 
 
-Filename: cheetah_orm-2.0.0b1.dist-info/RECORD
+Filename: cheetah_orm-2.0.0b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cheetah_orm-2.0.0b1.dist-info/LICENSE` & `cheetah_orm-2.0.0b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cheetah_orm-2.0.0b1.dist-info/METADATA` & `cheetah_orm-2.0.0b2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheetah-orm
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: A lightweight and high-performance object-relational mapper for Python.
 Author-email: Cybermals <cybermals@googlegroups.com>
 License: MIT
 Keywords: object-relational mapper
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,15 +32,15 @@
 to use PostgreSQL, you will need to install the "psycopg" package too. SQLite support requires no
 additonal packages.
 
 
 # Building
 1. clone this repo
 2. install the "wheel" package by executing `pip install wheel`
-3. from the repo folder, execute `./setup.py bdist_wheel`
+3. from the repo folder, execute `pip wheel .`
 4. there will be a wheel file inside the "dist" folder
 
 
 # Features
 * support for sqlite3, MariaDB/MySQL, and PostgreSQL
 * high-level database-neutral API written in pure Python
 * automatically generates the needed SQL statements for whichever database system you prefer to
```

## Comparing `cheetah_orm-2.0.0b1.dist-info/RECORD` & `cheetah_orm-2.0.0b2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 cheetah_orm/constants.py,sha256=fojdJdDRVwQolDdDm6j1aJFGdjkxSK3mmgwLGT9Ra9U,849
 cheetah_orm/error.py,sha256=Pe7nQ8lq07n5hpoqJru5bCOl6I-6CZ8PiXIovZFcOKQ,483
 cheetah_orm/fields.py,sha256=o6aWmqLNmi8S-zA8QzKBBbzxtc3j_yzsietWy1roL9A,7511
 cheetah_orm/indexes.py,sha256=eKoloBGZo2uj-CTNIwYgJNWnNIIHSx4LlzCB-RkmVdQ,2520
 cheetah_orm/mappers.py,sha256=idxfH0SXhXpPkNcjq293r12C-SuYJk10ckH2rPqNeYM,27471
 cheetah_orm/migrators.py,sha256=WfLuftq7OsHMp3GhlY0LuNN2A0GT8BnCoD_m90dd9QM,14124
 cheetah_orm/model.py,sha256=5lTnPXhpbkTfeOUJLl95NqIUpEpTnzOJr9o5S6t0faE,1898
-cheetah_orm-2.0.0b1.dist-info/LICENSE,sha256=8jBr0dsKeC3z7oRXG4rt7swwMNm1sQVL_67_T71Fq0k,1092
-cheetah_orm-2.0.0b1.dist-info/METADATA,sha256=YHPGVjwIzMB0wqJy54gX8vMZJHkfyc3c0kxcOFxtlws,6765
-cheetah_orm-2.0.0b1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cheetah_orm-2.0.0b1.dist-info/top_level.txt,sha256=V3lo5iuVk8dwLfgSrIXFlsSogMqqSyfODL5rHI8fxpM,12
-cheetah_orm-2.0.0b1.dist-info/RECORD,,
+cheetah_orm-2.0.0b2.dist-info/LICENSE,sha256=8jBr0dsKeC3z7oRXG4rt7swwMNm1sQVL_67_T71Fq0k,1092
+cheetah_orm-2.0.0b2.dist-info/METADATA,sha256=AgPEC-4Kpt86RueVLxvKXsCCsuoRwTeYCDiyEyESIHI,6754
+cheetah_orm-2.0.0b2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cheetah_orm-2.0.0b2.dist-info/top_level.txt,sha256=V3lo5iuVk8dwLfgSrIXFlsSogMqqSyfODL5rHI8fxpM,12
+cheetah_orm-2.0.0b2.dist-info/RECORD,,
```

