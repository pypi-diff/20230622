# Comparing `tmp/libprick-1.1.1.tar.gz` & `tmp/libprick-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libprick-1.1.1.tar", last modified: Thu Jun 22 16:19:37 2023, max compression
+gzip compressed data, was "libprick-1.2.0.tar", last modified: Thu Jun 22 17:53:38 2023, max compression
```

## Comparing `libprick-1.1.1.tar` & `libprick-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 16:19:37.696699 libprick-1.1.1/
--rw-rw-rw-   0        0        0      661 2023-06-22 16:19:37.696699 libprick-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      266 2021-01-01 05:41:16.000000 libprick-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 16:19:37.670631 libprick-1.1.1/libprick/
--rw-rw-rw-   0        0        0     7661 2021-04-04 21:30:03.000000 libprick-1.1.1/libprick/FFMpeg.py
--rw-rw-rw-   0        0        0     2039 2021-04-04 22:06:42.000000 libprick-1.1.1/libprick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:19:37.694817 libprick-1.1.1/libprick.egg-info/
--rw-rw-rw-   0        0        0      661 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 16:19:37.000000 libprick-1.1.1/libprick.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 16:19:37.699739 libprick-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-06-22 16:19:27.000000 libprick-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:53:38.360078 libprick-1.2.0/
+-rw-rw-rw-   0        0        0      661 2023-06-22 17:53:38.360078 libprick-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2021-01-01 05:41:16.000000 libprick-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 17:53:38.338041 libprick-1.2.0/libprick/
+-rw-rw-rw-   0        0        0     8734 2023-06-22 17:50:14.000000 libprick-1.2.0/libprick/FFMpeg.py
+-rw-rw-rw-   0        0        0     2039 2021-04-04 22:06:42.000000 libprick-1.2.0/libprick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:53:38.358073 libprick-1.2.0/libprick.egg-info/
+-rw-rw-rw-   0        0        0      661 2023-06-22 17:53:38.000000 libprick-1.2.0/libprick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-22 17:53:38.000000 libprick-1.2.0/libprick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 17:53:38.000000 libprick-1.2.0/libprick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 17:53:38.000000 libprick-1.2.0/libprick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 17:53:38.000000 libprick-1.2.0/libprick.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-22 17:53:38.361055 libprick-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-06-22 17:52:53.000000 libprick-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:53:38.359076 libprick-1.2.0/tests/
+-rw-rw-rw-   0        0        0      391 2023-06-22 17:51:50.000000 libprick-1.2.0/tests/test_FFMpeg.py
```

### Comparing `libprick-1.1.1/PKG-INFO` & `libprick-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: libprick
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python interface to the Last.FM API/website with caching support
 Home-page: https://github.com/spiritualized/libprick
-Download-URL: https://github.com/libprick/lastfmcache/archive/v1.1.1.tar.gz
+Download-URL: https://github.com/libprick/lastfmcache/archive/v1.2.0.tar.gz
 Keywords: pricker,python,hash,sha256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `libprick-1.1.1/libprick/FFMpeg.py` & `libprick-1.2.0/libprick/FFMpeg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import logging
 import os
 import platform
 import sys
 import sysconfig
 from ctypes import Structure, POINTER, CFUNCTYPE, c_int, c_void_p, c_char, c_uint, c_int64, c_uint8, c_char_p, \
     c_ulong, CDLL, byref
 from typing import Optional
@@ -135,31 +136,33 @@
 
     def __init__(self):
         lib_path = FFMpeg.__get_lib_path()
 
         os_family = platform.system()
 
         if os_family == 'Windows':
-            FFMpeg.avcodec = CDLL("{0}avcodec-58".format(lib_path))
-            FFMpeg.avformat = CDLL("{0}avformat-58".format(lib_path))
-            FFMpeg.avutil = CDLL("{0}avutil-56".format(lib_path))
+            FFMpeg.avcodec = CDLL(FFMpeg.__find_matching_lib(lib_path, "avcodec"))
+            FFMpeg.avformat = CDLL(FFMpeg.__find_matching_lib(lib_path, "avformat"))
+            FFMpeg.avutil = CDLL(FFMpeg.__find_matching_lib(lib_path, "avutil"))
+            # FFMpeg.avcodec = CDLL("{0}avcodec-58".format(lib_path))
+            # FFMpeg.avformat = CDLL("{0}avformat-58".format(lib_path))
+            # FFMpeg.avutil = CDLL("{0}avutil-56".format(lib_path))
         elif os_family == 'Linux':
             cython = sysconfig.get_config_var('SOABI')
             FFMpeg.avcodec = CDLL("{0}codec/codec.{1}.so".format(lib_path, cython))
             FFMpeg.avformat = CDLL("{0}format.{1}.so".format(lib_path, cython))
             FFMpeg.avutil = CDLL("{0}utils.{1}.so".format(lib_path, cython))
         else:
             print("Platform '{0}' not supported".format(os_family), file=sys.stderr)
             exit(1)
 
-        FFMpeg.avcodec.av_free_packet.argtypes = [POINTER(AVPacket)]
+        FFMpeg.avcodec.av_packet_unref.argtypes = [POINTER(AVPacket)]
         FFMpeg.avformat.avformat_open_input.argtypes = [POINTER(POINTER(AVFormatContext)), c_char_p, c_char_p, c_char_p]
         FFMpeg.avformat.avformat_close_input.argtypes = [POINTER(POINTER(AVFormatContext))]
 
-        FFMpeg.avformat.av_register_all()
         FFMpeg.avutil.av_log_set_level(FFMpeg.AV_LOG_QUIET)
 
         self.pFormatCtx = None
 
     def open(self, path):
         self.pFormatCtx = POINTER(AVFormatContext)()
         res = FFMpeg.avformat.avformat_open_input(self.pFormatCtx, path.encode('utf-8'), None, None)
@@ -184,15 +187,15 @@
         res = FFMpeg.avformat.av_read_frame(self.pFormatCtx, byref(avp))
 
         if res < 0:
             return None
 
         stream_index = avp.stream_index
         data = bytes(avp.data[:avp.size])
-        FFMpeg.avcodec.av_free_packet(avp)
+        FFMpeg.avcodec.av_packet_unref(avp)
 
         return Frame(stream_index, data)
 
     def close(self) -> None:
         if self.pFormatCtx:
             FFMpeg.avformat.avformat_close_input(self.pFormatCtx)
         self.pFormatCtx = None
@@ -205,15 +208,15 @@
     @staticmethod
     def __get_lib_path() -> str:
 
         os_family = platform.system()
         path = ''
 
         if os_family == 'Windows':
-            path = "{0}\\Lib\\site-packages\\av\\".format(sys.exec_prefix)
+            path = "{0}\\Lib\\site-packages\\av.libs\\".format(sys.exec_prefix)
             if getattr(sys, 'frozen', False):
                 path = '{0}\\'.format(sys.exec_prefix)
 
         elif os_family == 'Linux':
             path = "{0}/lib/python{1}/site-packages/av/".format(sys.exec_prefix,
                                                                 '.'.join(platform.python_version_tuple()[0:2]))
             if getattr(sys, 'frozen', False):
@@ -223,7 +226,31 @@
             print("Platform '{0}' not supported".format(os_family), file=sys.stderr)
             exit(1)
 
         if not os.path.exists(path):
             raise FFMpegError("Could not load FFMpeg libs. Is the 'av' package installed?\nlib path: {0}".format(path))
 
         return path
+
+    @staticmethod
+    def __find_matching_lib(directory: str, prefix: str) -> str:
+
+        candidates = []
+        os_family = platform.system()
+
+        for x in os.listdir(directory):
+            if x.startswith(f"{prefix}-"):
+
+                if (os_family == "Windows" and x.lower().endswith(".dll")) \
+                        or (os_family == "Linux" and ".so" in x.lower()):
+                    candidates.append(x)
+
+        candidates = sorted(candidates)
+
+        if len(candidates) == 0:
+            raise OSError(f"Could not find a binary for {prefix}")
+
+        if len(candidates) > 1:
+            logging.warning(f"{len(candidates)} candidates for {prefix}, using {candidates[-1]}")
+            return os.path.join(directory, candidates[-1])
+
+        return os.path.join(directory, candidates[0])
```

### Comparing `libprick-1.1.1/libprick/__init__.py` & `libprick-1.2.0/libprick/__init__.py`

 * *Files identical despite different names*

### Comparing `libprick-1.1.1/libprick.egg-info/PKG-INFO` & `libprick-1.2.0/libprick.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: libprick
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python interface to the Last.FM API/website with caching support
 Home-page: https://github.com/spiritualized/libprick
-Download-URL: https://github.com/libprick/lastfmcache/archive/v1.1.1.tar.gz
+Download-URL: https://github.com/libprick/lastfmcache/archive/v1.2.0.tar.gz
 Keywords: pricker,python,hash,sha256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

