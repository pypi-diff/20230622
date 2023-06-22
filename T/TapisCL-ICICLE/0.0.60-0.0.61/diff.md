# Comparing `tmp/TapisCL-ICICLE-0.0.60.tar.gz` & `tmp/TapisCL-ICICLE-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.60.tar", last modified: Fri Jun 16 03:35:09 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.61.tar", last modified: Thu Jun 22 20:53:24 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.60.tar` & `TapisCL-ICICLE-0.0.61.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.499647 TapisCL-ICICLE-0.0.60/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.60/LICENSE
--rw-rw-rw-   0        0        0    44549 2023-06-16 03:35:09.498647 TapisCL-ICICLE-0.0.60/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-05-06 23:32:02.000000 TapisCL-ICICLE-0.0.60/README.md
--rw-rw-rw-   0        0        0     1225 2023-06-16 03:35:00.000000 TapisCL-ICICLE-0.0.60/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 03:35:09.499647 TapisCL-ICICLE-0.0.60/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.475143 TapisCL-ICICLE-0.0.60/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.476143 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.477143 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0     9614 2023-06-16 03:29:32.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0     8443 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.483645 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3270 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/appCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.485647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0    14578 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0     6867 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     3159 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4900 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    11391 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7537 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.486647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1453 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     2210 2023-06-16 03:18:11.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0    10602 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/systemCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.489647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0     9976 2023-06-16 03:30:19.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0     7659 2023-06-16 02:40:58.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      462 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/serviceCheck.py
--rw-rw-rw-   0        0        0      171 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.490647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4384 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.493647 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     1436 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-16 03:35:09.497647 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44549 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1560 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      117 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-16 03:35:09.000000 TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      316 2023-06-06 01:10:45.000000 TapisCL-ICICLE-0.0.60/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.788768 TapisCL-ICICLE-0.0.61/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/LICENSE
+-rw-rw-rw-   0        0        0    44549 2023-06-22 20:53:24.787768 TapisCL-ICICLE-0.0.61/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/README.md
+-rw-rw-rw-   0        0        0     1174 2023-06-22 20:52:32.000000 TapisCL-ICICLE-0.0.61/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 20:53:24.788768 TapisCL-ICICLE-0.0.61/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.561062 TapisCL-ICICLE-0.0.61/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.571054 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.585952 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0     8950 2023-06-22 19:06:32.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.646796 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/appCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.655488 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     5534 2023-06-22 18:45:31.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.668846 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/systemCommands.py
+-rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.689150 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0     7904 2023-06-22 19:13:30.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/serviceCheck.py
+-rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.750255 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.772256 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.785767 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44549 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/__init__.py
+-rw-rw-rw-   0        0        0      316 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/__main__.py
```

### Comparing `TapisCL-ICICLE-0.0.60/LICENSE` & `TapisCL-ICICLE-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/PKG-INFO` & `TapisCL-ICICLE-0.0.61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.60
+Version: 0.0.61
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.60/README.md` & `TapisCL-ICICLE-0.0.61/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/pyproject.toml` & `TapisCL-ICICLE-0.0.61/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.60"
+version = "0.0.61"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
@@ -19,26 +19,23 @@
 keywords = ["Tapis", "CLI", "Agave", "HPC", "Tapis Pods", "TACC"]
 dependencies = [
     "pydantic",
     "pyfiglet",
     "tapipy",
     "pyperclip",
     "py2neo",
-    "psycopg",
+    "psycopg2-binary",
     "blessed",
     "prompt_toolkit",
     "TapisFederatedAuthClientAPI",
     "requests"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
 Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE"
 
-[project.entry-points."TapisCLICICLE.__main__"]
-TapisCLICICLE = "src:__main__"
-
-[tool.poetry.scripts]
-TapisCLICICLE = "src.__main__"
+[project.entry-points."console_scripts"]
+TapisCLICICLE = "src.__main__:main"
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         self.connection = connection
     
     def close(self):
         self.connection.close()
 
 
 class CLI(handlers.Handlers):
+    debug=False
     """
     Receive user input, either direct from bash environment or from the custom interface, then parse these commands and send them to the server to be executed. 
     """
     def __init__(self, IP: str, PORT: int):
         super().__init__()
 
         self.term = Terminal()
@@ -46,45 +47,38 @@
 
         setup_message = schemas.ResponseData(request_content={'setup_success':True})
         try:
             self.username, self.url = self.connect()
             self.connection.send(setup_message)
         except (KeyboardInterrupt, Exception) as e:
             error_str = traceback.format_exc()
-            print(error_str)
+            if self.debug:
+                print(error_str)
             print(e)
             setup_message.error = str(e)
             setup_message.request_content['setup_success'] = False
             self.connection.send(setup_message)
             os._exit(0)
 
         self.pwd = ""
         self.current_system = ""
 
     def parser_error(self, args):
         print(f"Ignoring unrecognized arguments: {args}")
     
     def configure_parser(self, arguments):
-        parser = argparse.ArgumentParser(description="Command Line Argument Parser", exit_on_error=False, usage=argparse.SUPPRESS, add_help=False)
-        parser.add_argument('command')
+        parser = argparse.ArgumentParser(description="Command Line Argument Parser", exit_on_error=False, usage=argparse.SUPPRESS, add_help=False, conflict_handler='resolve')
+        parser.add_argument('command_selection')
         parser.add_argument('positionals', nargs='*', default='default1')
         parser.error = self.parser_error
 
         for arg_name, arg in arguments.items():
-            print(arg_name)
-            print(arg)
-            if not arg['positional'] and arg['action'] == 'store':
-                parser.add_argument(arg['truncated_arg'], arg['full_arg'],
-                                    default=arg['default_value'], choices=arg['choices'],
-                                    action=arg['action'])#, type=handlers.ParserTypeLenEnforcer(name=arg_name, 
-                                                                                          #size=arg['size_limit'], 
-                                                                                          #data_type=arg['data_type'],
-                                                                                          #choices=arg['choices']))
-            elif not arg['positional']:
-                parser.add_argument(arg['truncated_arg'], arg['full_arg'], action=arg['action'])
+            print(arg['truncated_arg'])
+            parser.add_argument(f"-{arg['truncated_arg']}", arg['full_arg'],
+                                action=arg['action'])
         return parser
 
     def initialize_server(self): 
         """
         detect client operating system. The local server intitialization is different between unix and windows based systems
         """
         if 'win' in sys.platform:
@@ -101,15 +95,15 @@
         timeout_time = time.time() + 30 # server setup timeout. If expires, there is a problem!
         while True:
             if time.time() > timeout_time: # connection timeout condition
                 sys.stdout.write("\r[-] Connection timeout")
                 os._exit(0)
             try:
                 self.connection.connect((self.ip, self.port)) 
-                self.connection = ClientSideConnection(self.connection)
+                self.connection = ClientSideConnection(self.connection, debug=self.debug)
                 if startup_flag:
                     startup.kill()
                 break
             except Exception as e:
                 if not startup_flag:
                     startup = killableThread.KillableThread(target=self.initialize_server) # run the server setup on a separate thread
                     startup.start() 
@@ -139,22 +133,20 @@
         #self.connection.connect((self.ip, self.port)) # enable me for debugging. Requires manual server start
         connection_info: schemas.StartupData = self.connection.receive() # receive info from the server whether it is a first time connection
         if connection_info.initial: # if the server is receiving its first connection for the session\
             username, url = self.auth()
         else:
             username, url = connection_info.username, connection_info.url
         arguments: schemas.ResponseData = self.connection.receive()
-        for name, val in arguments.request_content.items():
-            print(f"{name} :: {val}\n\n\n")
         self.parser = self.configure_parser(arguments.request_content)
 
         return username, url # return the username and url
 
     def interface(self, kwargs):
-        if not kwargs['command']:
+        if not kwargs['command_selection']:
             return
         command_request = schemas.CommandData(request_content=kwargs)
         self.connection.send(command_request)
         while True:
             command_response = self.connection.receive()
             if isinstance(command_response, schemas.ResponseData):
                 self.url, self.username = command_response.url, command_response.active_username
@@ -198,17 +190,19 @@
             except (TypeError, argparse.ArgumentError, argparse.ArgumentTypeError) as e:
                 print(e)
                 error_str = traceback.format_exc()
                 print(error_str)
                 print("Invalid command")
             except Exception as e:
                 error_str = traceback.format_exc()
-                print(error_str)
-                error_message = schemas.CommandData(error=str(e))
+                if self.debug:
+                    print(error_str)
+                error_message = schemas.ResponseData(error=str(e))
                 self.connection.send(error_message)
+        
 
     def main(self):
         if len(sys.argv) > 1: # checks if any command line arguments were provided. Does not open CLI
             self.terminal_cli()
         self.cli_window()
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,18 +156,22 @@
                                     name = str(input(f"enter the {attrs['data_type']['name']} for the instance of {attrs['name']}"))
                                     sub_answer, repeat = self.form_handler(attrs['data_type'], term)
                                     answer[name] = sub_answer
                         case 'str_input':
                             answer = prompt(f"{attrs['name']}: ", validator=self.validator)
                         case 'confirmation':
                             answer = self.confirmation_handler()
+                        case 'silent':
+                            continue
                         case _:
                             raise AttributeError(f"There is not argument type {arg_type}")
                     response[field] = answer
                     break
+                except KeyboardInterrupt:
+                    raise RuntimeError('Form cancelled, command execution stopped')
                 except Exception as e:
                     with open(saved_command, 'w') as f:
                         f.write(json.dumps(response))
                         print(f"Argument input failure, command data written to file {saved_command}")
                         raise e
         return response, repeat
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/appCommands.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/appCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,150 +74,178 @@
             raise TypeError(f"The decorator parameter of the command {name} is invalid. Must be set to None or to a decorator type. Currently is {type(attrs['decorator'])}")
         
     def __check_command_opt(self, name, attrs):
         if 'command_opt' in list(attrs.keys()) and type((attrs['command_opt'])) != list:
             raise TypeError(f"The command opt attribute of the command {name} must be a list!")
 
 
+class HelpMenu:
+    def __init__(self, required_arguments: dict[str, Argument], optional_arguments: dict[str, Argument]):
+        self.required_arguments = required_arguments
+        self.optional_arguments = optional_arguments
+        self.arguments = {**required_arguments, **optional_arguments}
+        self.help = self.create_help_menu()
+
+    def create_help_menu(self):
+        help_dict = {'required':dict(), 'optional':dict()}
+        for arg_name, argument in self.required_arguments.items():
+            help_dict['required'][arg_name] = argument.help_message()
+        for arg_name, argument in self.optional_arguments.items():
+            help_dict['optional'][arg_name] = argument.help_message()
+        return help_dict
+    
+    def dict(self):
+        return self.arguments
+
+
 class BaseCommand(ABC, HelpStringRetriever, metaclass=CommandMetaClass):
     decorator = None
     return_formatter = None
     command_opt: list = None
     supports_config_file: bool = False
     required_arguments: list[Argument] | dict = list()
     optional_arguments: list[Argument] | dict = list()
     def __init__(self):
         self.t = None
         self.username = None
         self.password = None
         self.server = None
-        self.arg_names = [argument.argument for argument in self.required_arguments] + [argument.argument for argument in self.optional_arguments]
         self.arguments = dict()
         if isinstance(self.required_arguments, list):
             self.required_arguments = {argument.argument:argument for argument in self.required_arguments}
+            self.required_arguments['connection'] = Argument('connection', arg_type='silent')
             self.arguments.update(**self.required_arguments)
         if isinstance(self.optional_arguments, list):  
             self.optional_arguments = {argument.argument:argument for argument in self.optional_arguments}
             self.arguments.update(**self.optional_arguments)
         self.positional_arguments = [arg_name for arg_name, arg in self.required_arguments.items() if arg.positional]
+        self.form_arguments = [arg_name for arg_name, arg in self.arguments.items() if arg.arg_type not in  ('standard', 'silent')]
         self.help: dict[dict[str, list[dict[str, str]]]] = dict()
 
+        self.command_execution_sequence = [self.verify_argument_rules_followed]
+        if self.supports_config_file:
+            self.command_execution_sequence.append(self.handle_config_file)
+        if self.form_arguments:
+            self.command_execution_sequence.append(self.handle_form_input)
+        if self.positional_arguments:
+            self.command_execution_sequence.append(self.check_for_positionals)
+        if self.command_opt:
+            self.command_execution_sequence.append(self.handle_arg_opts)
+        self.command_execution_sequence.append(self.filter_kwargs)
+
+    async def verify_argument_rules_followed(self, kwargs):
+        for name, value in kwargs.items():
+            if name in self.optional_arguments and value and name not in self.form_arguments:
+                kwargs[name] = self.optional_arguments[name].verify_standard_value(value)
+            elif name in self.required_arguments:
+                kwargs[name] = self.required_arguments[name].verify_standard_value(value)
+        return kwargs
+
+    async def filter_kwargs(self, kwargs):
+        filtered_kwargs = dict()
+        for arg, value in kwargs.items():
+            if arg in self.arguments and value != None:
+                if (self.arguments[arg].arg_type in typing.get_args(ALLOWED_ARG_TYPES) and kwargs[arg]) or self.arguments[arg].arg_type == 'standard':
+                    filtered_kwargs[arg] = value
+        return filtered_kwargs
+
+    async def handle_config_file(self, kwargs):
+        if kwargs['file']:
+            with open(kwargs['file'], 'r') as f:
+                kwargs = json.loads(f.read)
+        return kwargs
+    
+    async def handle_form_input(self, kwargs):
+        for arg_name in self.form_arguments:
+            if kwargs[arg_name] or arg_name in self.required_arguments:
+                request = schemas.FormRequest(request_content={arg_name:self.arguments[arg_name] for arg_name in self.form_arguments if kwargs[arg_name] or arg_name in self.required_arguments})
+                await kwargs['connection'].send(request)
+                response: schemas.FormResponse = await kwargs['connection'].receive()
+                kwargs.update(**response.request_content)
+        print(kwargs)
+        return kwargs
+    
+    async def handle_arg_opts(self, kwargs):
+        for opt in self.command_opt:
+            kwargs = opt(kwargs)
+        return kwargs
+    
+    async def check_for_positionals(self, kwargs):
+        for arg_name, value in zip(self.positional_arguments, kwargs['positionals']):
+            kwargs[arg_name] = value
+        return kwargs
+
     def set_t_and_creds(self, t, username, password, server):
         self.t = t
         self.username = username
         self.password = password
         self.server = server
         for key, arg in self.optional_arguments.items():
             if issubclass(arg.choices.__class__, DynamicChoiceList):
                 arg.choices = arg.choices(self.t)
 
-    def update_args_with_truncated(self, aggregate_args_dict):
+    def update_args_with_truncated(self, truncated_args_dict):
         try:
-            for key, arg in self.required_arguments.items():
-                self.required_arguments[key] = aggregate_args_dict[key]
-            for key, arg in self.optional_arguments.items():
-                self.optional_arguments[key] = aggregate_args_dict[key]
-            self.help['required'] = self.__argument_list_help_compiler(self.required_arguments)
-            self.help['optional'] = self.__argument_list_help_compiler(self.optional_arguments)
+            for key in self.required_arguments:
+                self.required_arguments[key].truncated_arg = f"-{truncated_args_dict[key]}"
+            for key in self.optional_arguments:
+                self.optional_arguments[key].truncated_arg = f"-{truncated_args_dict[key]}"
+            self.help['required'] = self.__argument_help_compiler(self.required_arguments)
+            self.help['optional'] = self.__argument_help_compiler(self.optional_arguments)
         except Exception as e:
             print(self.__class__.__name__)
             raise e
         
-    def __argument_list_help_compiler(self, arg_dict: dict):
-        argument_help_dict = dict()
+    def __argument_help_compiler(self, arg_dict: dict[str, Argument]):
+        verbose_dict = dict()
+        standard_str = str()
         for name, argument in arg_dict.items():
-            if argument.positional:
-                arg_help = {name:f"<{argument.argument}>",
-                "description":argument.description}
-            elif argument.action != 'store':
-                arg_help = {name:f"{argument.truncated_arg}/{argument.full_arg}",
-                "description":argument.description}
-            else:
-                arg_help = {name:f"{argument.truncated_arg}/{argument.full_arg} <{argument.argument}>",
-                "description":argument.description}
-            argument_help_dict[name] = arg_help
-        return argument_help_dict
-    
-    def __non_verbose_help_string_creator(self, help_dict):
-        help_string = ""
-        for arg_name, arg_help in help_dict.items():
-            help_string += f"{arg_help[arg_name]}\n"
-        return help_string
+            if not (name in self.required_arguments and name in self.form_arguments) and argument.arg_type != 'silent':
+                verbose_dict[name] = argument.help_message()
+                standard_str += argument.str()
+        return {'verbose':verbose_dict, 'standard':standard_str}
 
     def __get_help(self, verbose):
         help_dict = {"Command":self.__class__.__name__,
                     "Description":self.help_string_retriever()}
         if not verbose:
             help_dict.update(**{
-                "Syntax":f"{self.__class__.__name__} {self.__non_verbose_help_string_creator(self.help['required'])}",
-                "Optional Arguments":self.__non_verbose_help_string_creator(self.help['optional'])
-            })
+                "Syntax":f"{self.__class__.__name__} {self.help['required']['standard']}\n(Optional Arguments) {self.help['optional']['standard']}"})
         else:
             help_dict.update(**{
                 "Syntax":f"{self.__class__.__name__}",
-                "Required Arguments":self.help['required'],
-                "Optional Arguments":self.help['optional']
-            })
+                "Required Arguments":self.help['required']['verbose'],
+                "Optional Arguments":self.help['optional']['verbose']})
         return help_dict
-
+    
     @abstractmethod
     async def run(self, *args, **kwargs):
         pass
 
-    def run_command_opts(self, **kwargs):
-        if self.command_opt:
-            for opt in self.command_opt:
-                kwargs = opt(kwargs)
-        return kwargs
-    
-    def check_commands_for_special_requests(self, kwargs):
-        require_further_input = dict()
-        for name, arg in kwargs.items():
-            if arg and name in list(self.arguments.keys()) and self.arguments[name].arg_type in typing.get_args(ALLOWED_ARG_TYPES):
-                require_further_input[name] = arg.json()
-        return require_further_input
-    
-    def check_for_positionals(self, kwargs):
-        for arg_name, value in zip(self.positional_arguments, kwargs['positionals']):
-            kwargs[arg_name] = value
-        return kwargs
-
     async def __call__(self, **kwargs):
+        command = kwargs.pop('command_selection')
+
+        if self.decorator:
+            return_value = await self.decorator(input_command=self, **kwargs)
+        
         verbose = kwargs.pop('verbose')
         help = kwargs.pop('help')
-        command = kwargs.pop('command')
+
         if help:
             return self.__get_help(verbose=verbose)
-        
-        elif self.supports_config_file and 'file' in list(kwargs.keys()):
-            with open(kwargs['file'], 'r') as f:
-                kwargs = json.loads(f.read)
-
-        kwargs = self.check_for_positionals(kwargs)
-
-        require_further_input = self.check_commands_for_special_requests(kwargs)
-        if require_further_input:
-            request = schemas.FormRequest(request_content=require_further_input)
-            await kwargs['connection'].send(request)
-            response: schemas.FormResponse = await kwargs['connection'].receive()
-            kwargs.update(**response.request_content)
-
-        kwargs = self.run_command_opts(**kwargs)
-
-        if self.decorator:
-            return_value = await self.decorator(self, **kwargs)
+        for handler in self.command_execution_sequence:
+            kwargs = await handler(kwargs)
         else:
             return_value = await self.run(**kwargs)
         if self.return_formatter:
             return_value = self.return_formatter(return_value, verbose)
         return return_value
     
 
 class BaseQuery(BaseCommand):
-    decorator = None
     def get_pod_credentials(self, id):
         uname, pword = self.t.pods.get_pod_credentials(pod_id=id).user_username, self.t.pods.get_pod_credentials(pod_id=id).user_password
         return uname, pword
     
     @abstractmethod
     async def run(self, *args, **kwargs):
         pass
@@ -283,18 +311,18 @@
             self.aggregate_command_map.update({name:command})
             if command.required_arguments or command.optional_arguments:
                 self.__contribute_to_arguments(command)
 
     def __contribute_to_arguments(self, command):
         arg_dict = {**command.required_arguments, **command.optional_arguments}
         for name, arg in arg_dict.items():
-            if name not in list(self.arguments.keys()):
+            if name not in self.arguments:
                 self.arguments[name] = arg
-            elif self.arguments[name].json() != arg.json():
-                raise ValueError(f"Found two instances of the argument {arg.argument} that had different attributes.\n\n{command.__class__.__name__}: {arg.json()}\n\nvs\n\n{self.arguments[name].json()}")
+            elif self.arguments[name].check_for_copy_data() != arg.check_for_copy_data():
+                raise ValueError(f"Found two instances of the argument {arg.argument} that had different attributes.\n\n{command.__class__.__name__}: {arg.check_for_copy_data()}\n\nvs\n\n{self.arguments[name].check_for_copy_data()}")
 
     def __help_gen(self):
         verbose_help = dict()
         for command in self.command_map.values():
             verbose_help.update({command.__class__.__name__:command.help})
         return verbose_help
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/podCommands.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,180 +1,224 @@
+import pyperclip
+from tapipy.tapis import errors as TapisErrors
+
+
 if __name__ != "__main__":
-    from . import systemCommands, serverCommands, appCommands, podCommands, fileCommands, dataFormatters, baseCommand
-    from .query import postgres, neo4j
-    from utilities import exceptions
-    from commands.arguments.argument import Argument
-
-
-def CHECK_EXPLICIT_SYSTEM(kwargs):
-    if not kwargs['id']:
-        kwargs['id'] = kwargs['connection'].system
-    return kwargs
-
-class Systems(baseCommand.BaseCommandMap):
-    """
-    @help: run operations on Tapis systems
-    """
-    command_opt = [CHECK_EXPLICIT_SYSTEM]
-    data_formatter = dataFormatters.DataFormatters.system_formatter
-    command_map = {
-        'get_systems':systemCommands.get_systems(), # since initialization of commands is separate from __init__, you dont need to specify these as classes anymore
-        'get_system_info':systemCommands.get_system_info(),
-        'get_scheduler_profiles':systemCommands.get_scheduler_profiles(),
-        'create_child_system':systemCommands.create_child_system(),
-        'create_system':systemCommands.create_system(),
-        'system':systemCommands.system(),
-        'exit_system':systemCommands.exit_system(),
-        'delete_system':systemCommands.delete_system(),
-    }
-
-
-class Server(baseCommand.BaseCommandMap):
-    """
-    @help: run config operations on the 
-    """
-    data_formatter = dataFormatters.DataFormatters.server_formatter
-    command_map = {
-        'whoami':serverCommands.whoami(),
-        'whereami':serverCommands.whereami(),
-        'exit':serverCommands.exit(),
-        'shutdown':serverCommands.shutdown(),
-        "get_args":serverCommands.get_args(),
-        'switch_service':serverCommands.switch_service()
-    }
-
-
-class Pods(baseCommand.BaseCommandMap):
-    """
-    @help: run operations on tapis pods
-    """
-    data_formatter = dataFormatters.DataFormatters.pod_formatter
-    command_map = {
-        'get_pods':podCommands.get_pods(),
-        'get_pod':podCommands.get_pod(),
-        'create_pod':podCommands.create_pod(),
-        'start_pod':podCommands.start_pod(),
-        'restart_pod':podCommands.restart_pod(),
-        'delete_pod':podCommands.delete_pod(),
-        'set_pod_perms':podCommands.set_pod_perms(),
-        'stop_pod':podCommands.stop_pod(),
-        'delete_pod_perms':podCommands.delete_pod_perms(),
-        'get_perms':podCommands.get_perms(),
-        'copy_pod_password':podCommands.copy_pod_password(),
-        'get_pod_logs':podCommands.get_pod_logs(),
-    }
-
-
-class Files(baseCommand.BaseCommandMap):
-    """
-    @help: run operations on tapis files
-    """
-    command_opt = [CHECK_EXPLICIT_SYSTEM]
-    command_map = {
-        'ls':fileCommands.ls(),
-        'cd':fileCommands.cd(),
-        'showme':fileCommands.showme(),
-        'cat':fileCommands.cat(),
-        'mkdir':fileCommands.mkdir(),
-        'mv':fileCommands.mv(),
-        'cp':fileCommands.cp(),
-        'rm':fileCommands.rm(),
-        'get_recent_transfers':fileCommands.get_recent_transfers(),
-        'create_postit':fileCommands.create_postit(),
-        'list_postits':fileCommands.list_postits(),
-        'get_postit':fileCommands.get_postit(),
-        'delete_postit':fileCommands.delete_postit(),
-        'redeem_postit':fileCommands.redeem_postit(),
-        'upload':fileCommands.upload(),
-        'download':fileCommands.download(),
-    }
-
-
-class Apps(baseCommand.BaseCommandMap):
-    """
-    @help: Run operations on tapis apps
-    """
-    data_formatter = dataFormatters.DataFormatters.app_formatter
-    command_map = {
-        'create_app':appCommands.create_app(),
-        'get_apps':appCommands.get_apps(),
-        'delete_app':appCommands.delete_app(),
-        'get_app':appCommands.get_app(),
-        'run_job':appCommands.run_job(),
-        'get_job_status':appCommands.get_job_status(),
-        'download_job_output':appCommands.download_job_output(),
-    }
-
-
-class Query(baseCommand.BaseCommandMap):
-    """
-    @help: run integrated query CLIs
-    """
-    command_map = {
-        'postgres': postgres.postgres(),
-        'neo4j': neo4j.neo4j()
-    }
-
-
-class ArgsGenerator:
-    def process_all_args(self, arg_dict: dict) -> dict:
-        truncation_list = list()
-        for argument_name in arg_dict.keys():
-            truncated_argument = self.__generate_truncated_argument(argument_name, truncation_list)
-            truncation_list.append(truncated_argument)
-            arg_dict[argument_name].truncated_arg, arg_dict[argument_name].full_arg = f"-{truncated_argument}", f"--{argument_name}"
-        return arg_dict
-            
-    def __generate_truncated_argument(self, argument, truncated_arguments_list, attempt=1):
-        if argument[attempt-1] in ('_', '-'):
-            attempt += 1
-        truncated_argument = argument[:attempt]
-        if truncated_argument in truncated_arguments_list:
-            return self.__generate_truncated_argument(argument, truncated_arguments_list, attempt=attempt+1)
-        return truncated_argument
+    from . import baseCommand, decorators
+    from .arguments import argument
+    Argument = argument.Argument
+
+
+class get_pods(baseCommand.BaseCommand):
+    """
+    @help: return a list of pods the current tapis instance has access to
+    """
+    async def run(self, *args, **kwargs) -> str: 
+        pods_list = self.t.pods.get_pods()
+        return pods_list
+
+
+class get_pod(baseCommand.BaseCommand):
+    """
+    @help: return a specific pod based on pod_id
+    """
+    required_arguments=[
+        Argument('pod_id')
+    ]
+    async def run(self, *args, **kwargs) -> str: 
+        pod_data = self.t.pods.get_pod(pod_id=kwargs["pod_id"])
+        return pod_data
+
+
+class create_pod(baseCommand.BaseCommand):
+    """
+    @help: create a new pod on the selected Tapis service
+    """
+    supports_config_file=True
+    required_arguments=[
+        Argument('pod_id'),
+        Argument('pod_template')
+    ]
+    optional_arguments=[
+        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
+        Argument('command', arg_type='input_list'),
+        Argument('environment_variables', arg_type='input_dict'),
+        Argument('data_request', arg_type='input_list'),
+        Argument('roles_required', arg_type='input_list'),
+        Argument('time_to_stop_default', data_type='int'),
+        Argument('time_to_stop_instance', data_type='int'),
+        Argument('volume_mounts', arg_type='input_dict', data_type=argument.Form(
+            'property_name', arguments_list = [
+                Argument('type'),
+                Argument("mount_path"),
+                Argument('sub_path')
+            ]
+        )),
+        Argument('networking', arg_type='input_dict', data_type=argument.Form(
+            'property_name', arguments_list = [
+                Argument('protocol'),
+                Argument('port'),
+                Argument('url')
+            ]
+        )),
+        Argument('resources', arg_type='input_dict', data_type=argument.Form(
+            'property_name', arguments_list = [
+                Argument('cpu_request'),
+                Argument('cpu_limit'),
+                Argument('mem_request'),
+                Argument('mem_limit'),
+            ]
+        ))
+    ]
+    async def run(self, *args, **kwargs) -> str:
+        template_name = kwargs['pod_template']
+        template_formats = (f"template/{template_name}", f"{self.username}/{template_name}", template_name)
+        for template_format in template_formats:
+            try:
+                kwargs['pod_template'] = template_format
+                pod_information = self.t.pods.create_pod(**kwargs)
+                break
+            except TapisErrors.BadRequestError as e:
+                if template_format != template_formats[-1]:
+                    continue
+                raise ValueError(f"Failed to execute pod creation due to {str(e)}")
+        return pod_information
+    
+
+class update_pod(create_pod):
+    """
+    @help: update a pod. Must be restarted to stage changes
+    """
+    required_arguments=[
+        Argument('pod_id'),
+    ]
+    async def run(self, *args, **kwargs):
+        pod_information = self.t.pods.update_pod(**kwargs)
+        return pod_information
+
+
+class start_pod(baseCommand.BaseCommand):
+    """
+    @help: start the pod specified with pod_id
+    """
+    required_arguments=[
+        Argument('pod_id'),
+    ]
+    async def run(self, *args, **kwargs):
+        return_information = self.t.pods.start_pod(pod_id=kwargs['pod_id'])
+        return return_information
+
+
+class restart_pod(baseCommand.BaseCommand):
+    """
+    @help: initiate a pod restart
+    """
+    decorator=decorators.NeedsConfirmation()
+    required_arguments=[
+        Argument('pod_id'),
+    ]
+    async def run(self, *args, **kwargs) -> str:
+        return_information = self.t.pods.restart_pod(pod_id=kwargs['pod_id'])
+        return return_information
+
+
+class stop_pod(baseCommand.BaseCommand):
+    """
+    @help: stop a pod's operations
+    """
+    decorator=decorators.NeedsConfirmation()
+    required_arguments=[
+        Argument('pod_id'),
+    ]
+    async def run(self, *args, **kwargs):
+        return_information = self.t.pods.stop_pod(pod_id=kwargs['pod_id'])
+        return return_information
+
+
+class delete_pod(baseCommand.BaseCommand):
+    """
+    @help: delete select pod
+    """
+    decorator=decorators.NeedsConfirmation()
+    required_arguments=[
+        Argument('pod_id'),
+    ]
+    async def run(self, *args, **kwargs) -> str: 
+        return_information = self.t.pods.delete_pod(pod_id=kwargs['pod_id'])
+        return return_information
+    
+
+class set_pod_perms(baseCommand.BaseCommand):
+    """
+    @help: set the permissions for the pod selected
+    """
+    required_arguments=[
+        Argument('pod_id'),
+        Argument('username'),
+        Argument('level')
+    ]
+    async def run(self, *args, **kwargs) -> str: # set pod permissions, given a pod pod_id, user, and permission level
+        return_information = self.t.pods.set_pod_permission(pod_id=kwargs['pod_id'], user=kwargs['username'], level=kwargs['level'])
+        return return_information
+
+
+class delete_pod_perms(baseCommand.BaseCommand):
+    """
+    @help: delete the selected pod from the pods service you are connected to
+    """
+    decorator=decorators.NeedsConfirmation()
+    required_arguments=[
+        Argument('pod_id'),
+        Argument('username')
+    ]
+    async def run(self, *args, **kwargs) -> str: # take away someones perms if they are being malicious, or something
+        return_information = self.t.pods.delete_pod_perms(pod_id=kwargs['pod_id'], user=kwargs['username'])
+        return return_information
+
+
+class get_perms(baseCommand.BaseCommand):
+    """
+    @help: get the permissions list for the selected pod
+    """
+    required_arguments=[
+        Argument('pod_id'),
+    ]
+    async def run(self, *args, **kwargs) -> str: # return a list of permissions on a given pod
+        return_information = self.t.pods.get_pod_permissions(pod_id=kwargs['pod_id'])
+        return return_information
+
+
+class copy_pod_password(baseCommand.BaseCommand):
+    """
+    @help: copy the pod password to the clipboard
+    """
+    decorator=decorators.Auth()
+    required_arguments=[
+        Argument('pod_id'),
+    ]
+    async def run(self, *args, **kwargs) -> str: # copies the pod password to clipboard so that the user can access the pod via the neo4j desktop app. Maybe a security risk? not as bad as printing passwords out!
+        password = self.t.pods.get_pod_credentials(pod_id=kwargs['pod_id']).user_password
+        pyperclip.copy(password)
+        password = None
+        return 'copied to clipboard'
+
+
+class get_pod_logs(baseCommand.BaseCommand):
+    """
+    @help: retrieve the logs of an active pod and either print them to the console, or write them to the specified file
+    """
+    required_arguments=[
+        Argument('pod_id')
+    ]
+    optional_arguments=[
+        Argument('destination_file')
+    ]
+    async def run(self, *args, **kwargs):
+        logs = self.t.pods.get_pod_logs(pod_id=kwargs['pod_id'])
+        file = kwargs['destination_file']
+        if file:
+            with open(file, 'w') as f:
+                f.write(logs)
+            return f"Log saved at {file}"
+        return logs
     
 
-class AggregateCommandMap(baseCommand.CommandContainer, ArgsGenerator):
-    groups = {
-        'Systems': Systems(),
-        'Server': Server(),
-        'Pods': Pods(),
-        'Files': Files(),
-        #'Apps': Apps(),
-        'Query': Query(),
-    }
-    def __init__(self):
-        self.process_all_args(self.arguments)
-        for command in self.aggregate_command_map.values():
-            command.update_args_with_truncated(self.arguments)
-        self.help = self.__general_help()
-
-    def __general_help(self):
-        general_help = list()
-        for group in self.groups.values():
-            general_help.append(group.brief_help)
-        return general_help
-
-    def update_credentials(self, t, username, password):
-        for command_name, command in self.aggregate_command_map.items():
-            command.set_t_and_creds(t, username, password, self)
-
-    async def run_command(self, connection, command_data: dict):
-        """
-        process and run command based on received kwargs
-        """
-        command_name = command_data['command']
-
-        if command_name in list(self.aggregate_command_map.keys()):
-            command = self.aggregate_command_map[command_name]
-            if command.supports_config_file and 'file' in list(command_data.keys()) and command_data['file']:
-                command_data = {'file':command_data['file']}
-
-            command_data['connection'] = connection
-            command_data['server'] = self
-            return await command(**command_data)
-        elif command_name in list(self.groups.keys()):
-            return self.groups[command_name]()
-        elif command_name == "help":
-            return self.help
-        else:
-            raise exceptions.CommandNotFoundError(command_name)
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,58 +19,58 @@
 
 
 class BaseRequirementDecorator(abc.ABC):
     username: typing.Optional[str] = None
     password: typing.Optional[str] = None
 
     @abc.abstractmethod
-    async def __call__(self, command: typing.Type[object], connection: socket.socket, *args, **kwargs):
+    async def __call__(self, input_ommand: typing.Type[object], connection: socket.socket, *args, **kwargs):
         pass
 
 
 class Auth(BaseRequirementDecorator):
     """
     used for secure authentication from the client. Requires that the function has a username and password parameter for credentials. sends request for credentials from 
     the client, and checks those credentials against the stored credentials in the server.
     """
-    async def __call__(self, command, *args, **kwargs):
+    async def __call__(self, input_command, *args, **kwargs):
         connection = kwargs['connection']
         requires_username = True
         if connection:
             auth_request = schemas.FormRequest(request_content=argument.Form('auth', [
                         argument.Argument('username'),
                         argument.Argument('password', arg_type='secure')
                     ]).json(),
                     message={"message":"Password is required to continue. If you logged in using TACC password login, use that. Otherwise use the session password\nYour username was returned during initial login"})
             await connection.send(auth_request)
             auth_data = await connection.receive()
             if auth_data.request_content['password'] != self.password:
                 raise ValueError("The provided password does not match the stored password")
             if auth_data.request_content['username'] != self.username:
                 raise ValueError("The provided username does not match the stored username")
-            return await command.run(**kwargs)
-        return await command.run(**kwargs)
+            return await input_command.run(**kwargs)
+        return await input_command.run(**kwargs)
 
 
 class NeedsConfirmation(BaseRequirementDecorator):
     """
     add to functions that you want user confirmation to exit. If you accidentally enter a command to delete a pod, this will not let you until you confirm
     """
-    async def __call__(self, command, *args, **kwargs):
+    async def __call__(self, input_command, *args, **kwargs):
         connection = kwargs['connection']
         if connection:
             connection = connection
-            confirmation_request = schemas.FormRequest(message={"message":f"YOU REQUESTED TO {command.__class__.__name__.upper()}. THIS MIGHT CAUSE DATA LOSS! Please confirm (y/n)"},
+            confirmation_request = schemas.FormRequest(message={"message":f"YOU REQUESTED TO {input_command.__class__.__name__.upper()}. THIS MIGHT CAUSE DATA LOSS! Please confirm (y/n)"},
                                                        request_content={"confirmation":argument.Argument('confirm', arg_type='confirmation')})
             await connection.send(confirmation_request)
             confirmation_reply: schemas.FormResponse = await connection.receive()
             confirmed = confirmation_reply.request_content['confirmation']
             if not confirmed:
-                raise exceptions.NoConfirmationError(command)
-        return await command.run(**kwargs)
+                raise exceptions.NoConfirmationError(input_command)
+        return await input_command.run(**kwargs)
 
 
 DECORATOR_LIST = [
     NeedsConfirmation,
     Auth
 ]
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,64 @@
 if __name__ != "__main__":
     from . import baseCommand
     from .arguments import argument
     from . import decorators
+    from . import commandOpts
     Argument = argument.Argument
 
 
-class CHECK_PWD:
-    """
-    support the invocation of relative paths for tapis systems
-    """
-    def __init__(self, dir_simplify_args: tuple):
-        self.dir_simplify_args = dir_simplify_args
-
-    def __go_back_checker(self, index: int, path_list: list):
-        back_count = 0
-        for element in path_list[index:]:
-            if element != "..":
-                break
-            back_count += 1
-        return back_count
-
-    def __simplify_path(self, path: list):
-        index = 0
-        length = len(path)
-        try:
-            while index < length:
-                if path[index] == ".":
-                    path.pop(index)
-                    continue
-                elif path[index] == "..":
-                    back_count = self.__go_back_checker(index, path)
-                    desired_len = len(path) - (2 * back_count)
-                    while len(path) != desired_len:
-                        path.pop(index-back_count)
-                    continue
-                index += 1
-        except IndexError:
-            pass
-        finally:
-            path = "/".join(path)
-            if not path:
-                path = "/"
-        return path
-    
-    def __relative_to_absolute(self, absolute_path: str, relative_path: str):
-        if not relative_path:
-            return absolute_path
-        elif absolute_path[-1] == "/":
-            return f"{absolute_path}{relative_path}"
-        return f"{absolute_path}/{relative_path}"
-
-    def __call__(self, kwargs):
-        for file_argument_name in self.dir_simplify_args:
-            if not kwargs[file_argument_name] or kwargs['connection'].pwd not in kwargs[file_argument_name]:
-                file = self.__relative_to_absolute(kwargs['connection'].pwd, kwargs[file_argument_name])
-                kwargs[file_argument_name] = self.__simplify_path(file.split("/"))
-        return kwargs
-    
-
 class ls(baseCommand.BaseCommand):
     """
     @help: list the files on a system 
     """
-    command_opt = [CHECK_PWD(('file_path',))]
+    command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', size_limit=(1, 80)),
-        Argument('file_path', positional=True)
+        Argument('file_path', positional=True),
     ]
     async def run(self, *args, **kwargs) -> str: # lists files available on a tapis account
         file_list = self.t.files.listFiles(systemId=kwargs['systemId'], path=kwargs['file_path'])
         file_list_truncated = [f"{file.type} - {file.nativePermissions} ---- {file.name}" for file in file_list]
         return file_list_truncated
     
 
 class cd(baseCommand.BaseCommand):
     """
     @help: change the directory
     """
-    command_opt = [CHECK_PWD(('file_path',))]
+    command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', size_limit=(1, 80)),
-        Argument('file_path', positional=True)
+        Argument('file_path', positional=True),
     ]
     async def run(self, *args, **kwargs):
         self.t.files.listFiles(systemId=kwargs['systemId'], path=kwargs['file_path'])
         kwargs['connection'].pwd = kwargs['file_path']
         return kwargs['connection'].pwd
 
 
 class showme(baseCommand.BaseCommand):
     """
     @help: display file metadata
     """
-    command_opt = [CHECK_PWD(('file_path',))]
+    command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', size_limit=(1, 80)),
-        Argument('file_path', positional=True)
+        Argument('file_path', positional=True),
     ]
     async def run(self, *args, **kwargs):
         return_data = str(self.t.files.getStatInfo(systemId=kwargs['systemId'], path=kwargs['file_path']))
         return return_data
     
 
 class cat(baseCommand.BaseCommand):
     """
     @help: display small files directly to the terminal
     """
-    command_opt = [CHECK_PWD(('file_path',))]
+    command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', size_limit=(1, 80)),
         Argument('file_path', positional=True)
     ]
     async def run(self, *args, **kwargs):
         size = self.t.files.getStatInfo(systemId=kwargs['systemId'], path=kwargs['file_path']).size
         if size <= 4000:
@@ -121,44 +69,44 @@
         return file_info
     
 
 class mkdir(baseCommand.BaseCommand):
     """
     @help: create a new directory at the selected path
     """
-    command_opt = [CHECK_PWD(('file_path',))]
+    command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', size_limit=(1, 80)),
         Argument('file_path', positional=True)
     ]
     async def run(self, *args, **kwargs):
         self.t.files.mkdir(systemId=kwargs['systemId'], path=kwargs['file_path'])
         return f"Successfully created file at {kwargs['file_path']}"
     
 
 class mv(baseCommand.BaseCommand):
     """
     @help: move a file from a source directory to a destination directory within a system's file structure
     """
-    command_opt = [CHECK_PWD(('source_file', 'destination_file'))]
+    command_opt = [commandOpts.CHECK_PWD(('source_file', 'destination_file')), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', size_limit=(1, 80)),
         Argument('source_file'),
         Argument('desination_file')
     ]
     async def run(self, destination_file: str, *args, **kwargs):
         self.t.files.moveCopy(systemId=kwargs['systemId'], path=kwargs['source_file'], operation="MOVE", newPath=destination_file)
         return f"File moved successfully to {destination_file}"
     
 
 class cp(baseCommand.BaseCommand):
     """
     @help: copy a file from a source directory to another directory
     """
-    command_opt = [CHECK_PWD(('source_file', 'destination_file'))]
+    command_opt = [commandOpts.CHECK_PWD(('source_file', 'destination_file')), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', size_limit=(1, 80)),
         Argument('source_file'),
         Argument('destination_file')
     ]
     async def run(self, *args, **kwargs):
         self.t.files.moveCopy(systemId=kwargs['systemId'], path=kwargs['source_file'], operation="COPY", newPath=kwargs['destination_file'])
@@ -166,15 +114,15 @@
     
 
 class rm(baseCommand.BaseCommand):
     """
     @help: delete a selected file
     """
     decorator=decorators.NeedsConfirmation()
-    command_opt = [CHECK_PWD(('file_path',))]
+    command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', size_limit=(1, 80)),
         Argument('file_path', positional=True)
     ]
     async def run(self, *args, **kwargs):
         self.t.delete(systemId=kwargs['systemId'], path=kwargs['file_path'])
         return f"file {kwargs['file_path']} successfully deleted"
@@ -189,15 +137,15 @@
         return str(recent_transfers)
     
 
 class create_postit(baseCommand.BaseCommand):
     """
     @help: create a postit to easily share file with other users
     """
-    command_opt = [CHECK_PWD(('file_path',))]
+    command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', size_limit=(1, 80)),
         Argument('file_path', positional=True)
     ]
     optional_arguments = [
         Argument('allowed_uses', data_type='int'),
         Argument('expiration_time', data_type='int')
@@ -258,19 +206,20 @@
 class upload(baseCommand.BaseCommand):
     """
     @help: upload a file to the system 
     the source and destination files must both be in the file argument, respectively, separated by a comma
     @todo: make it so that this doesnt need to take both source and destination files, but have it so it retrieves the current file location on the tapis system
     and sets that file location to be the upload point. Do the same for downloads but in reverse
     """
-    command_opt = [CHECK_PWD(('destination_file',))]
+    command_opt = [commandOpts.CHECK_PWD(('destination_file',))]
     required_arguments = [
         Argument('source_file'),
         Argument('destination_file'),
-        Argument('systemId', size_limit=(1, 80))
+        Argument('systemId', size_limit=(1, 80)),
+        Argument('connection', arg_type='silent')
     ]
     async def run(self, *args, **kwargs) -> str: # upload a file from local to remote using tapis. Takes source and destination paths
         if not kwargs['destination_file']:
             kwargs['destination_file'] = kwargs['connection'].pwd
         self.t.upload(system_id=kwargs['systemId'],
                 source_file_path=kwargs['source_file'],
                 dest_file_path=kwargs['destination_file'])
@@ -278,22 +227,25 @@
 
 
 class download(baseCommand.BaseCommand):
     """
     @help: download a file from the system
     the source and destination files must both be in the file argument, respectively, separated by a comma
     """
-    command_opt = [CHECK_PWD(('source_file',))]
+    command_opt = [commandOpts.CHECK_PWD(('source_file',))]
     required_arguments = [
         Argument('source_file'),
         Argument('destination_file'),
-        Argument('systemId', size_limit=(1, 80))
+        Argument('systemId', size_limit=(1, 80)),
+        Argument('connection', arg_type='silent')
     ]
     async def run(self, *args, **kwargs) -> str: # download a remote file using tapis, operates basically the same as upload
         if not kwargs["source_file"]:
             kwargs["source_file"] = kwargs['connection'].pwd
         file_info = self.t.files.getContents(systemId=kwargs['systemId'],
                             path=kwargs["source_file"])
         file_info = file_info.decode('utf-8')
         with open(kwargs['destination_file'], 'w') as f:
             f.write(file_info)
-        return f'successfully downloaded {kwargs["source_file"]} to {kwargs["destination_file"]}'
+        return f'successfully downloaded {kwargs["source_file"]} to {kwargs["destination_file"]}'
+    
+
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,224 +1,223 @@
-import pyperclip
 from tapipy.tapis import errors as TapisErrors
 
 
 if __name__ != "__main__":
     from . import baseCommand, decorators
     from .arguments import argument
+    from . import commandOpts
     Argument = argument.Argument
 
 
-class get_pods(baseCommand.BaseCommand):
+class get_volumes(baseCommand.BaseCommand):
     """
-    @help: return a list of pods the current tapis instance has access to
+    @help: get a list of volumes registered to your account
     """
-    async def run(self, *args, **kwargs) -> str: 
-        pods_list = self.t.pods.get_pods()
-        return pods_list
-
+    async def run(self, *args, **kwargs):
+        return self.t.pods.get_volumes()
+    
 
-class get_pod(baseCommand.BaseCommand):
+class create_volume(baseCommand.BaseCommand):
     """
-    @help: return a specific pod based on pod_id
+    @help: create a new volume on which to store files to be used by Tapis pods. This allows several pods to share the same persistent files
     """
-    required_arguments=[
-        Argument('pod_id')
+    supports_config_file=True
+    required_arguments = [
+        Argument('volume_id')
     ]
-    async def run(self, *args, **kwargs) -> str: 
-        pod_data = self.t.pods.get_pod(pod_id=kwargs["pod_id"])
-        return pod_data
+    optional_arguments = [
+        Argument('description', arg_type='str_input'),
+        Argument('size_limit', data_type='int', default_value=1024)
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.pods.create_volume(**kwargs)
+    
 
+class get_volume(baseCommand.BaseCommand):
+    """
+    @help: get information on a specific volume
+    """
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id')
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.pods.get_volume(**kwargs)
+    
 
-class create_pod(baseCommand.BaseCommand):
+class volume(baseCommand.BaseCommand):
     """
-    @help: create a new pod on the selected Tapis service
+    @help: enter the volume to interact with its files more directly
     """
-    supports_config_file=True
-    required_arguments=[
-        Argument('pod_id'),
-        Argument('pod_template')
-    ]
-    optional_arguments=[
-        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
-        Argument('command', arg_type='input_list'),
-        Argument('environment_variables', arg_type='input_dict'),
-        Argument('data_request', arg_type='input_list'),
-        Argument('roles_required', arg_type='input_list'),
-        Argument('time_to_stop_default', data_type='int'),
-        Argument('time_to_stop_instance', data_type='int'),
-        Argument('volume_mounts', arg_type='input_dict', data_type=argument.Form(
-            'property_name', arguments_list = [
-                Argument('type'),
-                Argument("mount_path"),
-                Argument('sub_path')
-            ]
-        )),
-        Argument('networking', arg_type='input_dict', data_type=argument.Form(
-            'property_name', arguments_list = [
-                Argument('protocol'),
-                Argument('port'),
-                Argument('url')
-            ]
-        )),
-        Argument('resources', arg_type='input_dict', data_type=argument.Form(
-            'property_name', arguments_list = [
-                Argument('cpu_request'),
-                Argument('cpu_limit'),
-                Argument('mem_request'),
-                Argument('mem_limit'),
-            ]
-        ))
-    ]
-    async def run(self, *args, **kwargs) -> str:
-        template_name = kwargs['template']
-        template_formats = (f"template/{template_name}", f"{self.username}/{template_name}", template_name)
-        for template_format in template_formats:
-            try:
-                kwargs['template'] = template_format
-                pod_information = self.t.pods.create_pod(**kwargs)
-                break
-            except TapisErrors.BadRequestError as e:
-                if template_format != template_formats[-1]:
-                    continue
-                raise ValueError(f"Failed to execute pod creation due to {str(e)}")
-        return pod_information
-    
-
-class update_pod(create_pod):
-    """
-    @help: update a pod. Must be restarted to stage changes
-    """
-    required_arguments=[
-        Argument('pod_id'),
-    ]
-    async def run(self, *args, **kwargs):
-        pod_information = self.t.pods.update_pod(**kwargs)
-        return pod_information
-
-
-class start_pod(baseCommand.BaseCommand):
-    """
-    @help: start the pod specified with pod_id
-    """
-    required_arguments=[
-        Argument('pod_id'),
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id')
     ]
     async def run(self, *args, **kwargs):
-        return_information = self.t.pods.start_pod(pod_id=kwargs['pod_id'])
-        return return_information
+        volume_info = self.t.pods.get_volume(volume_id=kwargs['volume_id'])
+        kwargs['connection'].system = volume_info
+        kwargs['connection'].pwd = "/"
+        return f"successfully entered the volume {kwargs['connection'].system}"
+    
 
+class update_volume(create_volume):
+    """
+    @help: update a volume's information
+    """
+    supports_config_file=True
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    async def run(self, *args, **kwargs):
+        return self.t.pods.update_volume(**kwargs)
+    
 
-class restart_pod(baseCommand.BaseCommand):
+class delete_volume(baseCommand.BaseCommand):
     """
-    @help: initiate a pod restart
+    @help: delete a volume
     """
     decorator=decorators.NeedsConfirmation()
-    required_arguments=[
-        Argument('pod_id'),
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id')
     ]
-    async def run(self, *args, **kwargs) -> str:
-        return_information = self.t.pods.restart_pod(pod_id=kwargs['pod_id'])
-        return return_information
+    async def run(self, *args, **kwargs):
+        return self.t.pods.delete_volume_files(**kwargs)
 
 
-class stop_pod(baseCommand.BaseCommand):
+class dir(baseCommand.BaseCommand):
     """
-    @help: stop a pod's operations
+    @help: list all files in the selected volume
     """
-    decorator=decorators.NeedsConfirmation()
-    required_arguments=[
-        Argument('pod_id'),
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id')
     ]
     async def run(self, *args, **kwargs):
-        return_information = self.t.pods.stop_pod(pod_id=kwargs['pod_id'])
-        return return_information
-
+        return self.t.pods.list_volume_files(**kwargs)
+    
 
-class delete_pod(baseCommand.BaseCommand):
+class upload_volume(baseCommand.BaseCommand):
     """
-    @help: delete select pod
+    @help: upload a file from your local machine to the volume
     """
-    decorator=decorators.NeedsConfirmation()
-    required_arguments=[
-        Argument('pod_id'),
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id'), commandOpts.CHECK_PWD('path',)]
+    required_arguments = [
+        Argument('volume_id'),
+        Argument('path'),
+        Argument('file')
     ]
-    async def run(self, *args, **kwargs) -> str: 
-        return_information = self.t.pods.delete_pod(pod_id=kwargs['pod_id'])
-        return return_information
+    async def run(self, *args, **kwargs):
+        return self.t.pods.upload_to_volume(**kwargs)
     
 
-class set_pod_perms(baseCommand.BaseCommand):
+class set_volume_permission(baseCommand.BaseCommand):
     """
-    @help: set the permissions for the pod selected
+    @help: set the permission for a user on a volume
     """
-    required_arguments=[
-        Argument('pod_id'),
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id'),
         Argument('username'),
         Argument('level')
     ]
-    async def run(self, *args, **kwargs) -> str: # set pod permissions, given a pod pod_id, user, and permission level
-        return_information = self.t.pods.set_pod_permission(pod_id=kwargs['pod_id'], user=kwargs['username'], level=kwargs['level'])
-        return return_information
+    async def run(self, *args, **kwargs):
+        user = kwargs.pop('username')
+        kwargs['user'] = user
+        return self.t.pods.set_volume_permission(**kwargs)
 
 
-class delete_pod_perms(baseCommand.BaseCommand):
+class get_volume_permissions(baseCommand.BaseCommand):
     """
-    @help: delete the selected pod from the pods service you are connected to
+    @help: set the permission for a user on a volume
     """
-    decorator=decorators.NeedsConfirmation()
-    required_arguments=[
-        Argument('pod_id'),
-        Argument('username')
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id'),
     ]
-    async def run(self, *args, **kwargs) -> str: # take away someones perms if they are being malicious, or something
-        return_information = self.t.pods.delete_pod_perms(pod_id=kwargs['pod_id'], user=kwargs['username'])
-        return return_information
-
+    async def run(self, *args, **kwargs):
+        return self.t.pods.get_volume_permission(**kwargs)
+    
 
-class get_perms(baseCommand.BaseCommand):
+class delete_volume_permission(baseCommand.BaseCommand):
     """
-    @help: get the permissions list for the selected pod
+    @help: delete the persmission for a user on a volume
     """
-    required_arguments=[
-        Argument('pod_id'),
+    decorator=decorators.NeedsConfirmation()
+    required_arguments = [
+        Argument('volume_id'),
+        Argument('username'),
+        Argument('level')
     ]
-    async def run(self, *args, **kwargs) -> str: # return a list of permissions on a given pod
-        return_information = self.t.pods.get_pod_permissions(pod_id=kwargs['pod_id'])
-        return return_information
+    async def run(self, *args, **kwargs):
+        user = kwargs.pop('username')
+        kwargs['user'] = user
+        return self.t.pods.delete_volume_permission(**kwargs)
+    
 
+class get_snapshots(baseCommand.BaseCommand):
+    """
+    @help: get a list of snapshots on the tenant you have access to
+    """
+    async def run(self, *args, **kwargs):
+        return self.t.pods.get_snapshots()
+    
 
-class copy_pod_password(baseCommand.BaseCommand):
+class create_snapshot(baseCommand.BaseCommand):
     """
-    @help: copy the pod password to the clipboard
+    @help: create a backup of the volume selected or specific files in the volume
     """
-    decorator=decorators.Auth()
-    required_arguments=[
-        Argument('pod_id'),
+    supports_config_file=True
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('source_volume_id'), commandOpts.CHECK_PWD(('source_volume_path', 'destination_path'))]
+    required_arguments = [
+        Argument('snapshot_id'),
+        Argument('source_volume_id'),
+        Argument('source_volume_path')
+    ]
+    optional_arguments = [
+        Argument('destination_path', description="Required if your snapshot is of a single file"),
+        Argument('description', arg_type='str_input'),
+        Argument('size_limit', data_type='int', description='maximum size in megabytes of the snapshot'),
+        Argument('cron'),
+        Argument('retention_policy')
     ]
-    async def run(self, *args, **kwargs) -> str: # copies the pod password to clipboard so that the user can access the pod via the neo4j desktop app. Maybe a security risk? not as bad as printing passwords out!
-        password = self.t.pods.get_pod_credentials(pod_id=kwargs['pod_id']).user_password
-        pyperclip.copy(password)
-        password = None
-        return 'copied to clipboard'
+    async def run(self, *args, **kwargs):
+        return self.t.pods.create_snapshot(**kwargs)
+    
 
+class get_snapshot(baseCommand.BaseCommand):
+    required_arguments = [
+        Argument('snapshot_id')
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.pods.get_snapshot(**kwargs)
+    
 
-class get_pod_logs(baseCommand.BaseCommand):
-    """
-    @help: retrieve the logs of an active pod and either print them to the console, or write them to the specified file
-    """
-    required_arguments=[
-        Argument('pod_id')
+class update_snapshot(baseCommand.BaseCommand):
+    supports_config_file=True
+    required_arguments = [
+        Argument('snapshot_id')
     ]
-    optional_arguments=[
-        Argument('destination_file')
+    optional_arguments = [
+        Argument('description', arg_type='str_input'),
+        Argument('size_limit', data_type='int'),
+        Argument('cron'),
+        Argument('retention_policy')
     ]
     async def run(self, *args, **kwargs):
-        logs = self.t.pods.get_pod_logs(pod_id=kwargs['pod_id'])
-        file = kwargs['destination_file']
-        if file:
-            with open(file, 'w') as f:
-                f.write(logs)
-            return f"Log saved at {file}"
-        return logs
+        return self.t.pods.update_snapshot(**kwargs)
     
 
+class delete_snapshot(baseCommand.BaseCommand):
+    decorator=decorators.NeedsConfirmation()
+    required_arguments = [
+        Argument('snapshot_id')
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.pods.delete_snapshot(**kwargs)
+    
+
+class list_snapshot_files(baseCommand.BaseCommand):
+    required_arguments = [
+        Argument('snapshot_id')
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.pods.list_snapshot_files(**kwargs)
+
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,17 @@
         argument.Argument('id'),
         argument.Argument('expression', arg_type='expression')
     ]
     async def run(self, *args, **kwargs) -> str: # function to submit queries to a Neo4j knowledge graph
         uname, pword = self.get_pod_credentials(kwargs["id"])
         graph = Graph(f"bolt+ssc://{kwargs['id']}.pods.{self.t.base_url.split('https://')[1]}:443", auth=(uname, pword), secure=True, verify=True)
 
-        try:
-            return_value = graph.run(kwargs['expression'])
-            print(type(return_value))
-            if str(return_value) == '(No data)' and 'create' in kwargs['expression'].lower(): # if no data is returned (mostly if something is created) then just say 'success'
-                return f'[+][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] Success'
-            elif str(return_value) == '(No data)':
-                return f'[-][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] KG is empty'
+        return_value = graph.run(kwargs['expression'])
+        print(type(return_value))
+        if str(return_value) == '(No data)' and 'create' in kwargs['expression'].lower(): # if no data is returned (mostly if something is created) then just say 'success'
+            return f'[+][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] Success'
+        elif str(return_value) == '(No data)':
+            return f'[-][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] KG is empty'
 
-            print(return_value)
-            print(type(return_value))
-            return str(f'[+][{kwargs["id"]}] {return_value}')
-        except Exception as e:
-            return str(e)
+        print(return_value)
+        print(type(return_value))
+        return str(f'[+][{kwargs["id"]}] {return_value}')
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,29 +11,32 @@
 
 class switch_service(baseCommand.BaseCommand):
     """
     @help: switch the connected tapis service
     @todo: upgrade to federated auth
     """
     required_arguments=[
-        Argument('link', size_limit=80),
-        Argument('auth', choices=['password', 'device_code', 'federated'])
+        Argument('link', size_limit=(0, 80)),
+        Argument('auth', choices=['password', 'device_code', 'federated']),
+        Argument('connection', arg_type='silent')
     ]
     async def run(self, *args, **kwargs):  # link is the baseURL
         auth = kwargs['auth']
         link = kwargs['link']
         self.server.auth_type = auth
         if auth == "password":
             results = await self.server.password_grant(link, kwargs['connection'])
         elif auth == "device_code":
             results = await self.server.device_code_grant(link, kwargs['connection'])
         elif auth == "federated":
             results = await self.server.federated_grant(link, kwargs['connection'])
         else:
             results = None
+        self.server.configure_decorators(self.server.username, self.server.password)
+        self.server.update_credentials(self.server.t, self.server.username, self.server.password)
         return results
       
 
 class exit(baseCommand.BaseCommand):
     """
     @help: exit the CLI without shutting down the service
     """
@@ -60,16 +63,16 @@
     
 
 class get_args(baseCommand.BaseCommand):
     """
     @help: get the list of possible arguments 
     """
     async def run(self, *args, **kwargs):
-        return kwargs['server'].arguments
+        return self.server.arguments
     
 
 class whereami(baseCommand.BaseCommand):
     """
     @help: get the URI of current tapis tenant
     """
     async def run(self, *args, **kwargs):
-        return kwargs['server'].url
+        return self.server.url
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             username_password_response = await connection.receive()
             username = username_password_response.request_content['username']
             password = username_password_response.request_content['password']
             try:
                 self.t = Tapis(f"https://{link}",
                                username=username,
                                password=password)
+                print(self.t.base_url)
                 self.t.get_tokens()
                 break
             except exceptions.ClientSideError as e:
                 raise e
             except Exception as e:
                 if attempt > 3:
                     username_password_request.message = None
@@ -76,14 +77,16 @@
                                       message={"message":"Go to the URL if it doesnt open automatically and enter the user code to authenticate. Then click y when you enter the code", 
                                                "url":authentication_information.verification_uri, 
                                                "user_code": authentication_information.user_code},
                                       request_content={'entered_confirm':argument.Argument('entered_confirm', arg_type='confirmation')})
         await connection.send(payload)
         webbrowser.open(authentication_information.verification_uri)
         confirmation = await connection.receive()
+        if not confirmation.request_content['entered_confirm']:
+            raise RuntimeError(f"User indicated that device code auth failed") # get rid of this feature and switch to polling
         start_time = time.time()
         while True:
             try:
                 access_info = self.t.authenticator.create_token(grant_type="device_code", device_code=authentication_information.device_code, client_id=client_id)
                 break
             except:
                 time.sleep(1)
@@ -128,15 +131,15 @@
 
         return f"Successfully initialized tapis service on {self.url}"
 
     async def auth_startup(self, connection):
         session_auth_type_request = schemas.AuthRequest(request_content={"uri":argument.Argument('uri', arg_type='str_input'), "auth_type":argument.Argument('auth_type', choices=['password', 'device_code', 'federated'], arg_type='str_input')},
                                                         auth_request_type="requested",
                                                         message={"message":"Enter the URI of the Tapis tenant you wish to connect to, then select your auth type from the options below",
-                                                                 "options":['password', 'device_code', 'federated']})
+                                                                 "grant options":['password', 'device_code', 'federated']})
         while True:
             try:
                 await connection.send(session_auth_type_request)
                 session_auth_type_response: schemas.FormResponse = await connection.receive()
                 auth_type = session_auth_type_response.request_content['auth_type']
                 if auth_type not in ('password', 'device_code', 'federated'):
                     raise exceptions.InvalidCredentialsReceived()
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 
 class Server(commandMap.AggregateCommandMap, logger.ServerLogger, decorators.DecoratorSetup, auth.ServerSideAuth):
     """
     Receives commands from the client and executes Tapis operations
     """
     SESSION_TIME = 1200
+    debug=False
     def __init__(self, IP: str, PORT: int):
         super().__init__()
         self.initial = True
 
         self.t = None
         self.url = None
         self.access_token = None
@@ -65,21 +66,25 @@
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.sock.setblocking(False)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.bind((self.ip, self.port))
         self.sock.listen(1)
         self.end_time = time.time() + self.SESSION_TIME # start the countdown on the timeout
 
-        self.task_list = []
+        self.task_list: list[asyncio.Task] = []
 
         self.server = None
         self.num_connections = 0
 
         self.logger.info('initialization complete')
 
+    def cancel_tasks(self):
+        for task in self.task_list:
+            task.cancel()
+
     async def handshake(self, connection):
         self.logger.info("Handshake starting")
         if self.initial:  # if this is the first time in the session that the cli is connecting
             startup_data = schemas.StartupData(initial = self.initial)
             await connection.send(startup_data)
             await self.auth_startup(connection)
         else:
@@ -89,15 +94,15 @@
         self.logger.info("Final connection data sent")
 
     async def accept(self, reader, writer):
         """
         accept connection request and initialize communication with the client
         """  
         self.num_connections += 1
-        connection = ServerConnection(f"CON-{self.num_connections}", reader=reader, writer=writer, debug=True)
+        connection = ServerConnection(f"CON-{self.num_connections}", reader=reader, writer=writer, debug=self.debug)
         self.timeout_handler()
         ip, port= writer.transport.get_extra_info('socket').getsockname()
         if ip != socket.gethostbyname(socket.gethostname()):
             raise exceptions.UnauthorizedAccessError(ip)
         self.logger.info("Received connection request")
         try:
             await self.handshake(connection)
@@ -121,14 +126,15 @@
             self.logger.warning(f"The setup of the connection {connection.name} failed")
             return
 
         loop = asyncio.get_event_loop()
         task: asyncio.Task = loop.create_task(self.receive_and_execute(connection))
         callback = TaskCallback(self.logger, task)
         task.add_done_callback(callback)
+        self.task_list.append(task)
 
     def timeout_handler(self):  
         """
         checks if the timeout has been exceeded
         """
         if time.time() > self.end_time: 
             raise exceptions.TimeoutError
@@ -150,14 +156,15 @@
             except exceptions.ClientSideError as e:
                 self.logger.warning(e)
                 continue
             except (exceptions.TimeoutError, exceptions.Shutdown) as e:
                 error_response = schemas.ResponseData(error=str(e), exit_status=1, url=self.url, active_username=self.username)
                 await connection.send(error_response)
                 self.logger.warning(str(e))
+                self.cancel_tasks()
                 self.server.close()
                 loop = asyncio.get_event_loop()
                 loop.stop()
                 loop.close()
                 sys.exit(0)
             except exceptions.Exit as e:
                 self.logger.info("user exit initiated")
@@ -178,13 +185,14 @@
     async def main(self):
         self.server = await asyncio.start_server(self.accept, sock=self.sock)
         try:
             async with self.server:
                 await self.server.serve_forever()
         except KeyboardInterrupt:
             self.server.close()
+            self.cancel_tasks()
             sys.exit(0)
 
 
 if __name__ == '__main__':
     server = Server(socket.gethostbyname(socket.gethostname()), 30000)
     asyncio.run(server.main())
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.60
+Version: 0.0.61
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.60/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
+src/__init__.py
 src/__main__.py
 src/TapisCLICICLE/__init__.py
 src/TapisCLICICLE/serverRun.py
 src/TapisCLICICLE/client/__init__.py
 src/TapisCLICICLE/client/cli.py
 src/TapisCLICICLE/client/handlers.py
 src/TapisCLICICLE/commands/__init__.py
 src/TapisCLICICLE/commands/appCommands.py
 src/TapisCLICICLE/commands/baseCommand.py
 src/TapisCLICICLE/commands/commandMap.py
+src/TapisCLICICLE/commands/commandOpts.py
 src/TapisCLICICLE/commands/dataFormatters.py
 src/TapisCLICICLE/commands/decorators.py
 src/TapisCLICICLE/commands/fileCommands.py
 src/TapisCLICICLE/commands/podCommands.py
 src/TapisCLICICLE/commands/serverCommands.py
 src/TapisCLICICLE/commands/systemCommands.py
+src/TapisCLICICLE/commands/volumeCommands.py
 src/TapisCLICICLE/commands/arguments/__init__.py
 src/TapisCLICICLE/commands/arguments/argument.py
 src/TapisCLICICLE/commands/query/__init__.py
 src/TapisCLICICLE/commands/query/neo4j.py
 src/TapisCLICICLE/commands/query/postgres.py
 src/TapisCLICICLE/server/__init__.py
 src/TapisCLICICLE/server/auth.py
```

