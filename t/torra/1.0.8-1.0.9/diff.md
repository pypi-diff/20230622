# Comparing `tmp/torra-1.0.8.tar.gz` & `tmp/torra-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torra-1.0.8.tar", last modified: Tue Apr 13 09:08:11 2021, max compression
+gzip compressed data, was "dist/torra-1.0.9.tar", last modified: Tue Apr 13 10:46:18 2021, max compression
```

## Comparing `torra-1.0.8.tar` & `torra-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-04-13 09:08:11.000000 torra-1.0.8/
--rw-r--r--   0 pi        (1000) pi        (1000)      937 2021-04-13 09:08:11.000000 torra-1.0.8/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      576 2021-04-09 13:22:26.000000 torra-1.0.8/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2021-04-13 09:08:11.000000 torra-1.0.8/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)     1021 2021-04-13 09:07:23.000000 torra-1.0.8/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-04-13 09:08:11.000000 torra-1.0.8/torra/
--rw-r--r--   0 pi        (1000) pi        (1000)     1914 2021-03-24 12:28:21.000000 torra-1.0.8/torra/bencod.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1555 2021-03-28 09:54:09.000000 torra-1.0.8/torra/confs.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1418 2021-03-24 12:28:21.000000 torra-1.0.8/torra/conmenu.py
--rw-r--r--   0 pi        (1000) pi        (1000)      582 2021-03-24 12:28:21.000000 torra-1.0.8/torra/cons.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7999 2021-03-24 12:36:08.000000 torra-1.0.8/torra/gtk.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3136 2021-04-09 13:22:04.000000 torra-1.0.8/torra/layout.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1223 2021-03-28 09:55:29.000000 torra-1.0.8/torra/listtor.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2017 2021-03-24 20:27:34.000000 torra-1.0.8/torra/log.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1103 2021-04-10 11:20:52.000000 torra-1.0.8/torra/main.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1276 2021-03-24 12:28:21.000000 torra-1.0.8/torra/meninfo.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2539 2021-03-24 12:28:21.000000 torra-1.0.8/torra/next.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1920 2021-03-24 14:06:21.000000 torra-1.0.8/torra/overall.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1857 2021-03-24 15:20:21.000000 torra-1.0.8/torra/ratio.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1681 2021-03-24 14:04:52.000000 torra-1.0.8/torra/sets.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2386 2021-03-24 12:28:21.000000 torra-1.0.8/torra/stats.py
--rw-r--r--   0 pi        (1000) pi        (1000)      143 2021-03-24 12:28:21.000000 torra-1.0.8/torra/torben.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2232 2021-03-25 09:38:34.000000 torra-1.0.8/torra/torrent.py
--rw-r--r--   0 pi        (1000) pi        (1000)      886 2021-03-24 12:28:21.000000 torra-1.0.8/torra/treesel.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-04-13 09:08:11.000000 torra-1.0.8/torra.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      937 2021-04-13 09:08:10.000000 torra-1.0.8/torra.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      499 2021-04-13 09:08:10.000000 torra-1.0.8/torra.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-04-13 09:08:10.000000 torra-1.0.8/torra.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       43 2021-04-13 09:08:10.000000 torra-1.0.8/torra.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-04-13 09:08:10.000000 torra-1.0.8/torra.egg-info/not-zip-safe
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2021-04-13 09:08:10.000000 torra-1.0.8/torra.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2021-04-13 09:08:10.000000 torra-1.0.8/torra.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-04-13 10:46:18.000000 torra-1.0.9/
+-rw-r--r--   0 pi        (1000) pi        (1000)      995 2021-04-13 10:46:18.000000 torra-1.0.9/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      576 2021-04-09 13:22:26.000000 torra-1.0.9/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2021-04-13 10:46:18.000000 torra-1.0.9/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      871 2021-04-13 10:44:43.000000 torra-1.0.9/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-04-13 10:46:18.000000 torra-1.0.9/torra/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1914 2021-03-24 12:28:21.000000 torra-1.0.9/torra/bencod.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1555 2021-03-28 09:54:09.000000 torra-1.0.9/torra/confs.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1418 2021-03-24 12:28:21.000000 torra-1.0.9/torra/conmenu.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      582 2021-03-24 12:28:21.000000 torra-1.0.9/torra/cons.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7999 2021-03-24 12:36:08.000000 torra-1.0.9/torra/gtk.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3136 2021-04-09 13:22:04.000000 torra-1.0.9/torra/layout.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1223 2021-03-28 09:55:29.000000 torra-1.0.9/torra/listtor.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2017 2021-03-24 20:27:34.000000 torra-1.0.9/torra/log.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1103 2021-04-10 11:20:52.000000 torra-1.0.9/torra/main.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1276 2021-03-24 12:28:21.000000 torra-1.0.9/torra/meninfo.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2539 2021-03-24 12:28:21.000000 torra-1.0.9/torra/next.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1920 2021-03-24 14:06:21.000000 torra-1.0.9/torra/overall.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1857 2021-03-24 15:20:21.000000 torra-1.0.9/torra/ratio.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1681 2021-03-24 14:04:52.000000 torra-1.0.9/torra/sets.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2386 2021-03-24 12:28:21.000000 torra-1.0.9/torra/stats.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      143 2021-03-24 12:28:21.000000 torra-1.0.9/torra/torben.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2232 2021-03-25 09:38:34.000000 torra-1.0.9/torra/torrent.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      886 2021-03-24 12:28:21.000000 torra-1.0.9/torra/treesel.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-04-13 10:46:18.000000 torra-1.0.9/torra.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      995 2021-04-13 10:46:17.000000 torra-1.0.9/torra.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      499 2021-04-13 10:46:17.000000 torra-1.0.9/torra.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-04-13 10:46:17.000000 torra-1.0.9/torra.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       43 2021-04-13 10:46:17.000000 torra-1.0.9/torra.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-04-13 10:46:17.000000 torra-1.0.9/torra.egg-info/not-zip-safe
+-rw-r--r--   0 pi        (1000) pi        (1000)      101 2021-04-13 10:46:17.000000 torra-1.0.9/torra.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2021-04-13 10:46:17.000000 torra-1.0.9/torra.egg-info/top_level.txt
```

### Comparing `torra-1.0.8/PKG-INFO` & `torra-1.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torra
-Version: 1.0.8
+Version: 1.0.9
 Summary: Torrent client
 Home-page: https://github.com/colin-i/tora
 Author: bot
 Author-email: costin.botescu@gmail.com
 License: MIT
 Description: # Torrent client
         Using libtorrent (arvidn) with python bindings.\
@@ -17,7 +17,9 @@
         | Dogecoin  | DP28QjzNcWCF4XqdUoDcZ7DeWKhjTmZqY9         |
         | Decred    | DsSdAMyVkKbX18fXK5pYJbNgXhfisc4onT9        |
         | Digibyte  | DPK6t296EMSHNMzuoMyP2zbxRjtisaaCRu         |
         | Ravencoin | RECqJbqzqNiGQeodcRSBqkAZjh2fbroUHL         |
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+Provides-Extra: libtorrent
+Provides-Extra: libtorrent-bin
```

### Comparing `torra-1.0.8/README.md` & `torra-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/bencod.py` & `torra-1.0.9/torra/bencod.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/confs.py` & `torra-1.0.9/torra/confs.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/conmenu.py` & `torra-1.0.9/torra/conmenu.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/cons.py` & `torra-1.0.9/torra/cons.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/gtk.py` & `torra-1.0.9/torra/gtk.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/layout.py` & `torra-1.0.9/torra/layout.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/listtor.py` & `torra-1.0.9/torra/listtor.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/log.py` & `torra-1.0.9/torra/log.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/main.py` & `torra-1.0.9/torra/main.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/meninfo.py` & `torra-1.0.9/torra/meninfo.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/next.py` & `torra-1.0.9/torra/next.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/overall.py` & `torra-1.0.9/torra/overall.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/ratio.py` & `torra-1.0.9/torra/ratio.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/sets.py` & `torra-1.0.9/torra/sets.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/stats.py` & `torra-1.0.9/torra/stats.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/torrent.py` & `torra-1.0.9/torra/torrent.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra/treesel.py` & `torra-1.0.9/torra/treesel.py`

 * *Files identical despite different names*

### Comparing `torra-1.0.8/torra.egg-info/PKG-INFO` & `torra-1.0.9/torra.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torra
-Version: 1.0.8
+Version: 1.0.9
 Summary: Torrent client
 Home-page: https://github.com/colin-i/tora
 Author: bot
 Author-email: costin.botescu@gmail.com
 License: MIT
 Description: # Torrent client
         Using libtorrent (arvidn) with python bindings.\
@@ -17,7 +17,9 @@
         | Dogecoin  | DP28QjzNcWCF4XqdUoDcZ7DeWKhjTmZqY9         |
         | Decred    | DsSdAMyVkKbX18fXK5pYJbNgXhfisc4onT9        |
         | Digibyte  | DPK6t296EMSHNMzuoMyP2zbxRjtisaaCRu         |
         | Ravencoin | RECqJbqzqNiGQeodcRSBqkAZjh2fbroUHL         |
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+Provides-Extra: libtorrent
+Provides-Extra: libtorrent-bin
```

