# Comparing `tmp/libprick-1.1.0.tar.gz` & `tmp/libprick-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libprick-1.1.0.tar", last modified: Mon Apr  5 21:33:25 2021, max compression
+gzip compressed data, was "libprick-1.1.1.tar", last modified: Thu Jun 22 16:19:37 2023, max compression
```

## Comparing `libprick-1.1.0.tar` & `libprick-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-04-05 21:33:25.165921 libprick-1.1.0/
--rw-rw-rw-   0        0        0      760 2021-04-05 21:33:25.165921 libprick-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-04-05 21:33:25.165921 libprick-1.1.0/libprick/
--rw-rw-rw-   0        0        0     7661 2021-04-04 21:30:03.577034 libprick-1.1.0/libprick/FFMpeg.py
--rw-rw-rw-   0        0        0     2039 2021-04-04 22:06:42.168407 libprick-1.1.0/libprick/__init__.py
--rw-rw-rw-   0        0        0       40 2021-01-01 05:41:16.679830 libprick-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      850 2021-04-05 21:32:48.072970 libprick-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:19:37.696699 libprick-1.1.1/
+-rw-rw-rw-   0        0        0      661 2023-06-22 16:19:37.696699 libprick-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2021-01-01 05:41:16.000000 libprick-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 16:19:37.670631 libprick-1.1.1/libprick/
+-rw-rw-rw-   0        0        0     7661 2021-04-04 21:30:03.000000 libprick-1.1.1/libprick/FFMpeg.py
+-rw-rw-rw-   0        0        0     2039 2021-04-04 22:06:42.000000 libprick-1.1.1/libprick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 16:19:37.694817 libprick-1.1.1/libprick.egg-info/
+-rw-rw-rw-   0        0        0      661 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-22 16:19:37.699739 libprick-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-06-22 16:19:27.000000 libprick-1.1.1/setup.py
```

### Comparing `libprick-1.1.0/libprick/FFMpeg.py` & `libprick-1.1.1/libprick/FFMpeg.py`

 * *Files identical despite different names*

### Comparing `libprick-1.1.0/libprick/__init__.py` & `libprick-1.1.1/libprick/__init__.py`

 * *Files identical despite different names*

### Comparing `libprick-1.1.0/setup.py` & `libprick-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
     name = 'libprick',
     packages = ['libprick'],
-    version = '1.1.0',
+    version = '1.1.1',
     description = 'Python interface to the Last.FM API/website with caching support',
     url = 'https://github.com/spiritualized/libprick',
-    download_url = 'https://github.com/libprick/lastfmcache/archive/v1.1.0.tar.gz',
+    download_url = 'https://github.com/libprick/lastfmcache/archive/v1.1.1.tar.gz',
     keywords = ['pricker', 'python', 'hash', 'sha256'],
     install_requires = [
-                    'av==8.0.2'
+                    'av==10.0.0'
                 ],
 
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'Programming Language :: Python :: 3',
```

