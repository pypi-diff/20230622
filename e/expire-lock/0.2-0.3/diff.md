# Comparing `tmp/expire_lock-0.2.tar.gz` & `tmp/expire_lock-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expire_lock-0.2.tar", last modified: Thu Jun 22 12:36:57 2023, max compression
+gzip compressed data, was "expire_lock-0.3.tar", last modified: Thu Jun 22 12:39:13 2023, max compression
```

## Comparing `expire_lock-0.2.tar` & `expire_lock-0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 12:36:57.720784 expire_lock-0.2/
--rw-rw-rw-   0        0        0     2821 2023-06-22 12:36:57.719786 expire_lock-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1653 2023-06-22 12:35:58.000000 expire_lock-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 12:36:57.702782 expire_lock-0.2/expire_lock/
--rw-rw-rw-   0        0        0     4762 2023-06-22 12:10:34.000000 expire_lock-0.2/expire_lock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 12:36:57.715785 expire_lock-0.2/expire_lock.egg-info/
--rw-rw-rw-   0        0        0     2821 2023-06-22 12:36:57.000000 expire_lock-0.2/expire_lock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-22 12:36:57.000000 expire_lock-0.2/expire_lock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 12:36:57.000000 expire_lock-0.2/expire_lock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-22 12:36:57.000000 expire_lock-0.2/expire_lock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 12:36:57.721783 expire_lock-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1696 2023-06-22 12:36:43.000000 expire_lock-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:39:13.881530 expire_lock-0.3/
+-rw-rw-rw-   0        0        0     2821 2023-06-22 12:39:13.879529 expire_lock-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1653 2023-06-22 12:35:58.000000 expire_lock-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 12:39:13.803454 expire_lock-0.3/expire_lock/
+-rw-rw-rw-   0        0        0     4762 2023-06-22 12:10:34.000000 expire_lock-0.3/expire_lock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:39:13.875528 expire_lock-0.3/expire_lock.egg-info/
+-rw-rw-rw-   0        0        0     2821 2023-06-22 12:39:13.000000 expire_lock-0.3/expire_lock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-22 12:39:13.000000 expire_lock-0.3/expire_lock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 12:39:13.000000 expire_lock-0.3/expire_lock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 12:39:13.000000 expire_lock-0.3/expire_lock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-22 12:39:13.000000 expire_lock-0.3/expire_lock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 12:39:13.882531 expire_lock-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1713 2023-06-22 12:39:10.000000 expire_lock-0.3/setup.py
```

### Comparing `expire_lock-0.2/PKG-INFO` & `expire_lock-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expire_lock
-Version: 0.2
+Version: 0.3
 Summary: 可以过期的python线程锁，基于python字典实现的锁可以过期,实现方式类似于redis锁过期的实现机制。使用字典代替 redis服务。
 Home-page: https://github.com/ydf0509/expire_lock
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `expire_lock-0.2/README.md` & `expire_lock-0.3/README.md`

 * *Files identical despite different names*

### Comparing `expire_lock-0.2/expire_lock/__init__.py` & `expire_lock-0.3/expire_lock/__init__.py`

 * *Files identical despite different names*

### Comparing `expire_lock-0.2/expire_lock.egg-info/PKG-INFO` & `expire_lock-0.3/expire_lock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expire-lock
-Version: 0.2
+Version: 0.3
 Summary: 可以过期的python线程锁，基于python字典实现的锁可以过期,实现方式类似于redis锁过期的实现机制。使用字典代替 redis服务。
 Home-page: https://github.com/ydf0509/expire_lock
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

### Comparing `expire_lock-0.2/setup.py` & `expire_lock-0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding=utf-8
 from setuptools import setup, find_packages
 
 setup(
     name='expire_lock',  #
-    version='0.2',
+    version='0.3',
     description=(
         '可以过期的python线程锁，基于python字典实现的锁可以过期,实现方式类似于redis锁过期的实现机制。使用字典代替 redis服务。'
     ),
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     keywords=['lock','lock timeout','lock expire','expire'],
     long_description_content_type="text/markdown",
     long_description=open('README.md', 'r', encoding='utf8').read(),
@@ -32,20 +32,20 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries'
     ],
     install_requires=[
-
+        'nb_log',
     ],
     extras_require={},
 )
 
 """
 
-python setup.py sdist & python -m  twine upload dist/expire_lock-0.2.tar.gz
+python setup.py sdist & python -m  twine upload dist/expire_lock-0.3.tar.gz
 
 
 
 
 """
```

