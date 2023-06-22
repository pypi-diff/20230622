# Comparing `tmp/wcd-0.0.0a8.tar.gz` & `tmp/wcd-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcd-0.0.0a8.tar", last modified: Tue Oct 26 01:30:59 2021, max compression
+gzip compressed data, was "wcd-0.1.0.tar", max compression
```

## Comparing `wcd-0.0.0a8.tar` & `wcd-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,15 @@
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2021-10-26 01:30:59.106508 wcd-0.0.0a8/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1067 2021-10-14 07:45:01.000000 wcd-0.0.0a8/LICENSE
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3912 2021-10-26 01:30:59.106508 wcd-0.0.0a8/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3390 2021-10-25 17:39:09.000000 wcd-0.0.0a8/README.md
--rw-r--r--   0 bruno     (1000) bruno     (1000)      105 2021-10-16 21:34:37.000000 wcd-0.0.0a8/pyproject.toml
--rw-r--r--   0 bruno     (1000) bruno     (1000)       38 2021-10-26 01:30:59.106508 wcd-0.0.0a8/setup.cfg
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1173 2021-10-26 00:17:39.000000 wcd-0.0.0a8/setup.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2021-10-26 01:30:59.103174 wcd-0.0.0a8/wcd/
--rw-r--r--   0 bruno     (1000) bruno     (1000)      142 2021-10-26 00:19:52.000000 wcd-0.0.0a8/wcd/__init__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)       32 2021-10-25 17:34:38.000000 wcd-0.0.0a8/wcd/__main__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)      277 2021-10-26 00:23:37.000000 wcd-0.0.0a8/wcd/__version__.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1742 2021-10-15 20:34:45.000000 wcd-0.0.0a8/wcd/cfg.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)      731 2021-10-18 04:53:09.000000 wcd-0.0.0a8/wcd/default-cfg.yml
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1155 2021-10-25 17:43:38.000000 wcd-0.0.0a8/wcd/event.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3076 2021-10-16 22:50:26.000000 wcd-0.0.0a8/wcd/funcs.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1374 2021-10-25 18:00:07.000000 wcd-0.0.0a8/wcd/trace.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     1527 2021-10-18 05:20:54.000000 wcd-0.0.0a8/wcd/wcc.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2727 2021-10-25 17:40:30.000000 wcd-0.0.0a8/wcd/wcd.py
--rw-r--r--   0 bruno     (1000) bruno     (1000)     2194 2021-10-16 22:50:43.000000 wcd-0.0.0a8/wcd/wp_cache.py
-drwxr-xr-x   0 bruno     (1000) bruno     (1000)        0 2021-10-26 01:30:59.106508 wcd-0.0.0a8/wcd.egg-info/
--rw-r--r--   0 bruno     (1000) bruno     (1000)     3912 2021-10-26 01:30:59.000000 wcd-0.0.0a8/wcd.egg-info/PKG-INFO
--rw-r--r--   0 bruno     (1000) bruno     (1000)      364 2021-10-26 01:30:59.000000 wcd-0.0.0a8/wcd.egg-info/SOURCES.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        1 2021-10-26 01:30:59.000000 wcd-0.0.0a8/wcd.egg-info/dependency_links.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       57 2021-10-26 01:30:59.000000 wcd-0.0.0a8/wcd.egg-info/entry_points.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)       32 2021-10-26 01:30:59.000000 wcd-0.0.0a8/wcd.egg-info/requires.txt
--rw-r--r--   0 bruno     (1000) bruno     (1000)        4 2021-10-26 01:30:59.000000 wcd-0.0.0a8/wcd.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1067 2021-10-14 07:45:01.806356 wcd-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3433 2021-10-26 02:06:02.251628 wcd-0.1.0/README.md
+-rw-r--r--   0        0        0      871 2023-06-22 20:43:37.681789 wcd-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      142 2021-10-26 00:19:52.294276 wcd-0.1.0/wcd/__init__.py
+-rw-r--r--   0        0        0       32 2021-10-25 17:34:38.397588 wcd-0.1.0/wcd/__main__.py
+-rw-r--r--   0        0        0      277 2021-10-26 00:23:37.559590 wcd-0.1.0/wcd/__version__.py
+-rw-r--r--   0        0        0     1742 2021-10-15 20:34:45.395456 wcd-0.1.0/wcd/cfg.py
+-rw-r--r--   0        0        0      731 2021-10-18 04:53:09.453245 wcd-0.1.0/wcd/default-cfg.yml
+-rw-r--r--   0        0        0     1155 2021-10-25 17:43:38.043604 wcd-0.1.0/wcd/event.py
+-rw-r--r--   0        0        0     3076 2021-10-16 22:50:26.338698 wcd-0.1.0/wcd/funcs.py
+-rw-r--r--   0        0        0     1374 2021-10-25 18:00:07.687711 wcd-0.1.0/wcd/trace.py
+-rw-r--r--   0        0        0     1527 2021-10-18 05:20:54.360141 wcd-0.1.0/wcd/wcc.py
+-rw-r--r--   0        0        0     2727 2021-10-25 17:40:30.138115 wcd-0.1.0/wcd/wcd.py
+-rw-r--r--   0        0        0     2194 2021-10-16 22:50:43.498945 wcd-0.1.0/wcd/wp_cache.py
+-rw-r--r--   0        0        0     4481 1970-01-01 00:00:00.000000 wcd-0.1.0/PKG-INFO
```

### Comparing `wcd-0.0.0a8/LICENSE` & `wcd-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wcd-0.0.0a8/PKG-INFO` & `wcd-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: wcd
-Version: 0.0.0a8
-Summary: A daemon which manages your desktop wallpapers. Sort of the 'mpd' of wallpapers.
-Home-page: http://github.com/brunofauth/wcd
-Author: Bruno Fauth
-Author-email: bvfauth@hotmail.com
+Version: 0.1.0
+Summary: 'Wallpaper changing daemon' is exactly what its name suggests. It tries to be the 'mpd' of wallpapers.
+Home-page: https://github.com/brunofauth/wcd
 License: MIT
-Project-URL: Bug Tracker, https://github.com/brunofauth/wcd/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Keywords: wallpaper
+Author: Bruno Fauth
+Author-email: 149593@upf.br
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: coloredlogs (>=15.0,<16.0)
+Requires-Dist: humanfriendly (>=10.0,<11.0)
+Project-URL: Bug Tracker, https://github.com/brunofauth/wcd/issues
+Project-URL: Repository, https://github.com/brunofauth/wcd
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Wallpaper Changing Daemon (wcd)
 Wallpaper Changing Daemon reminds me of mpd, but it manages wallpapers instead of music.
 
 ## Overview
 * It comes with wcc too, which is a CLI client app, used to interact with the Daemon.
 * It works on python 3.9 (and, probably, on 3.7 and 3.8 too, not sure about lower versions though).
@@ -58,12 +68,11 @@
 * Run: `wcc --help`, it stands for Wallpaper Changing Client and comes bundled with `wcd`
 
 ## sxhkd keybindings for wcc (append to your sxhkdrc)
     shift + XF86Audio{Play,Next,Prev}
         wcc {toggle_cycle,next,prev}
 
 ## TODO
-* aur package
+* update pkgbuild to aur, along with the systemd service
 * use less memory (tracemalloc says it's fine, but htop disagrees)
 
 
-
```

### Comparing `wcd-0.0.0a8/README.md` & `wcd-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,10 +42,10 @@
 * Run: `wcc --help`, it stands for Wallpaper Changing Client and comes bundled with `wcd`
 
 ## sxhkd keybindings for wcc (append to your sxhkdrc)
     shift + XF86Audio{Play,Next,Prev}
         wcc {toggle_cycle,next,prev}
 
 ## TODO
-* aur package
+* update pkgbuild to aur, along with the systemd service
 * use less memory (tracemalloc says it's fine, but htop disagrees)
```

### Comparing `wcd-0.0.0a8/wcd/cfg.py` & `wcd-0.1.0/wcd/cfg.py`

 * *Files identical despite different names*

### Comparing `wcd-0.0.0a8/wcd/default-cfg.yml` & `wcd-0.1.0/wcd/default-cfg.yml`

 * *Files identical despite different names*

### Comparing `wcd-0.0.0a8/wcd/event.py` & `wcd-0.1.0/wcd/event.py`

 * *Files identical despite different names*

### Comparing `wcd-0.0.0a8/wcd/funcs.py` & `wcd-0.1.0/wcd/funcs.py`

 * *Files identical despite different names*

### Comparing `wcd-0.0.0a8/wcd/trace.py` & `wcd-0.1.0/wcd/trace.py`

 * *Files identical despite different names*

### Comparing `wcd-0.0.0a8/wcd/wcc.py` & `wcd-0.1.0/wcd/wcc.py`

 * *Files identical despite different names*

### Comparing `wcd-0.0.0a8/wcd/wcd.py` & `wcd-0.1.0/wcd/wcd.py`

 * *Files identical despite different names*

### Comparing `wcd-0.0.0a8/wcd/wp_cache.py` & `wcd-0.1.0/wcd/wp_cache.py`

 * *Files identical despite different names*

