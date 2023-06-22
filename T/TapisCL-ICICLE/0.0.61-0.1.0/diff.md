# Comparing `tmp/TapisCL-ICICLE-0.0.61.tar.gz` & `tmp/TapisCL-ICICLE-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.61.tar", last modified: Thu Jun 22 20:53:24 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.1.0.tar", last modified: Thu Jun 22 21:06:21 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.61.tar` & `TapisCL-ICICLE-0.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.788768 TapisCL-ICICLE-0.0.61/
--rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/LICENSE
--rw-rw-rw-   0        0        0    44549 2023-06-22 20:53:24.787768 TapisCL-ICICLE-0.0.61/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/README.md
--rw-rw-rw-   0        0        0     1174 2023-06-22 20:52:32.000000 TapisCL-ICICLE-0.0.61/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 20:53:24.788768 TapisCL-ICICLE-0.0.61/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.561062 TapisCL-ICICLE-0.0.61/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.571054 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.585952 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0     8950 2023-06-22 19:06:32.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.646796 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/appCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.655488 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     5534 2023-06-22 18:45:31.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.668846 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/systemCommands.py
--rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.689150 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0     7904 2023-06-22 19:13:30.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/serviceCheck.py
--rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.750255 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.772256 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-22 20:53:24.785767 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44549 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1663 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-06-22 20:53:24.000000 TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/__init__.py
--rw-rw-rw-   0        0        0      316 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.0.61/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.478770 TapisCL-ICICLE-0.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    44548 2023-06-22 21:06:21.477776 TapisCL-ICICLE-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2643 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1164 2023-06-22 21:05:29.000000 TapisCL-ICICLE-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 21:06:21.478770 TapisCL-ICICLE-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.248863 TapisCL-ICICLE-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.260384 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.280377 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0     8950 2023-06-22 19:06:32.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0     8649 2023-06-22 19:04:26.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.347416 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3270 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/appCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.362214 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     5534 2023-06-22 18:45:31.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0    16273 2023-06-22 18:22:47.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0     8371 2023-06-22 20:35:42.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     3159 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    10128 2023-06-22 18:12:37.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7545 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.403976 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1344 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     2442 2023-06-22 19:23:16.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0    16482 2023-06-22 17:47:34.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/systemCommands.py
+-rw-rw-rw-   0        0        0     7059 2023-06-22 20:48:12.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.424112 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10215 2023-06-22 19:16:49.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0     7904 2023-06-22 19:13:30.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      462 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/server/serviceCheck.py
+-rw-rw-rw-   0        0        0      171 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.441370 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4384 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.465620 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     1436 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-22 21:06:21.476770 TapisCL-ICICLE-0.1.0/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44548 2023-06-22 21:06:21.000000 TapisCL-ICICLE-0.1.0/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2023-06-22 21:06:21.000000 TapisCL-ICICLE-0.1.0/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 21:06:21.000000 TapisCL-ICICLE-0.1.0/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-22 21:06:21.000000 TapisCL-ICICLE-0.1.0/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2023-06-22 21:06:21.000000 TapisCL-ICICLE-0.1.0/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-22 21:06:21.000000 TapisCL-ICICLE-0.1.0/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/__init__.py
+-rw-rw-rw-   0        0        0      316 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.1.0/src/__main__.py
```

### Comparing `TapisCL-ICICLE-0.0.61/LICENSE` & `TapisCL-ICICLE-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/PKG-INFO` & `TapisCL-ICICLE-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.61
+Version: 0.1.0
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.61/README.md` & `TapisCL-ICICLE-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/pyproject.toml` & `TapisCL-ICICLE-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.61"
+version = "0.1.0"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
@@ -34,8 +34,8 @@
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
 Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE"
 
 [project.entry-points."console_scripts"]
-TapisCLICICLE = "src.__main__:main"
+TapisCLICICLE = "src:main"
```

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/client/cli.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/client/handlers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/appCommands.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/appCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/commandMap.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/podCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/systemCommands.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/systemCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/server/auth.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/server/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.1.0/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.1.0/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.61
+Version: 0.1.0
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.61/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.1.0/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

