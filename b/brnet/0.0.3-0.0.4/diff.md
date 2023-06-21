# Comparing `tmp/brnet-0.0.3.tar.gz` & `tmp/brnet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brnet-0.0.3.tar", last modified: Wed Jun 21 21:10:41 2023, max compression
+gzip compressed data, was "brnet-0.0.4.tar", last modified: Wed Jun 21 22:46:05 2023, max compression
```

## Comparing `brnet-0.0.3.tar` & `brnet-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.527262 brnet-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 21:10:22.000000 brnet-0.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 21:10:22.000000 brnet-0.0.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-21 21:10:22.000000 brnet-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 21:10:22.000000 brnet-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 21:10:22.000000 brnet-0.0.3/01-phys-to-bridge
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 21:10:22.000000 brnet-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 21:10:22.000000 brnet-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-21 21:10:41.527262 brnet-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-21 21:10:22.000000 brnet-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-21 21:10:22.000000 brnet-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:10:22.000000 brnet-0.0.3/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-21 21:10:22.000000 brnet-0.0.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:22.000000 brnet-0.0.3/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-21 21:10:22.000000 brnet-0.0.3/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 21:10:41.527262 brnet-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/sh/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 21:10:22.000000 brnet-0.0.3/sh/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-21 21:10:22.000000 brnet-0.0.3/sh/brnet
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 21:10:22.000000 brnet-0.0.3/sh/pidp11.sh.diff
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-21 21:10:22.000000 brnet-0.0.3/sh/wait_for_if
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.519262 brnet-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/src/brnet/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 21:10:22.000000 brnet-0.0.3/src/brnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-06-21 21:10:22.000000 brnet-0.0.3/src/brnet/bridger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-06-21 21:10:22.000000 brnet-0.0.3/src/brnet/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 21:10:22.000000 brnet-0.0.3/src/brnet/external.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/src/brnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 21:10:41.000000 brnet-0.0.3/src/brnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:41.523262 brnet-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 21:10:22.000000 brnet-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 21:10:22.000000 brnet-0.0.3/tests/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 21:10:22.000000 brnet-0.0.3/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-21 21:10:22.000000 brnet-0.0.3/wrapper.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-21 22:45:51.000000 brnet-0.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-21 22:45:51.000000 brnet-0.0.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-21 22:45:51.000000 brnet-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 22:45:51.000000 brnet-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 22:45:51.000000 brnet-0.0.4/01-phys-to-bridge
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 22:45:51.000000 brnet-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-21 22:45:51.000000 brnet-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-21 22:46:05.930070 brnet-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-21 22:45:51.000000 brnet-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-21 22:45:51.000000 brnet-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:45:51.000000 brnet-0.0.4/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-21 22:45:51.000000 brnet-0.0.4/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:45:51.000000 brnet-0.0.4/requirements/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-21 22:45:51.000000 brnet-0.0.4/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:46:05.930070 brnet-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/sh/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-21 22:45:51.000000 brnet-0.0.4/sh/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-21 22:45:51.000000 brnet-0.0.4/sh/brnet
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-21 22:45:51.000000 brnet-0.0.4/sh/pidp11.sh.diff
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-21 22:45:51.000000 brnet-0.0.4/sh/wait_for_if
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.926070 brnet-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/src/brnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 22:45:51.000000 brnet-0.0.4/src/brnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-06-21 22:45:51.000000 brnet-0.0.4/src/brnet/bridger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-06-21 22:45:51.000000 brnet-0.0.4/src/brnet/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 22:45:51.000000 brnet-0.0.4/src/brnet/external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/src/brnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 22:46:05.000000 brnet-0.0.4/src/brnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:05.930070 brnet-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:45:51.000000 brnet-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-21 22:45:51.000000 brnet-0.0.4/tests/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-21 22:45:51.000000 brnet-0.0.4/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-21 22:45:51.000000 brnet-0.0.4/wrapper.sh
```

### Comparing `brnet-0.0.3/.github/workflows/ci.yaml` & `brnet-0.0.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/.gitignore` & `brnet-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/LICENSE` & `brnet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/Makefile` & `brnet-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/PKG-INFO` & `brnet-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `brnet-0.0.3/README.md` & `brnet-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/pyproject.toml` & `brnet-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/requirements/dev.txt` & `brnet-0.0.4/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/sh/README.md` & `brnet-0.0.4/sh/README.md`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/sh/brnet` & `brnet-0.0.4/sh/brnet`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/src/brnet/bridger.py` & `brnet-0.0.4/src/brnet/bridger.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,16 @@
         self._create_bridge()
         self._create_taps()
         self._bridge_phys_if()
 
     def _create_bridge(self) -> None:
         cmd = ["ip", "link", "add", self._bridge, "type", "bridge"]
         run_check(args=cmd, logger=self._logger)
+        cmd = ["ip", "link", "set", "dev", self._bridge, "up"]
+        run_check(args=cmd, logger=self._logger)
 
     def _create_taps(self) -> None:
         for i in range(self._first_tap, (self._first_tap + self._num_taps)):
             tapdev = f"tap{i}"
             cmd = ["ip", "tuntap", "add", "mode", "tap", tapdev]
             run_check(args=cmd, logger=self._logger)
             cmd = ["ip", "link", "set", "dev", tapdev, "master", self._bridge]
@@ -153,15 +155,14 @@
             run_check(args=cmd, logger=self._logger)
 
     def _bridge_phys_if(self) -> None:
         cmd = ["ip", "addr", "del", "dev", self._interface, self._ip]
         run_check(args=cmd, logger=self._logger)
         cmd = ["ip", "addr", "replace", "dev", self._bridge, self._ip]
         run_check(args=cmd, logger=self._logger)
-        cmd = ["ip", "link", "set", "dev", self._bridge, "up"]
         if self._gateway:
             cmd = [
                 "ip",
                 "route",
                 "add",
                 "default",
                 "metric",
```

### Comparing `brnet-0.0.3/src/brnet/cli.py` & `brnet-0.0.4/src/brnet/cli.py`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/src/brnet/external.py` & `brnet-0.0.4/src/brnet/external.py`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/src/brnet.egg-info/PKG-INFO` & `brnet-0.0.4/src/brnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `brnet-0.0.3/src/brnet.egg-info/SOURCES.txt` & `brnet-0.0.4/src/brnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/tox.ini` & `brnet-0.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `brnet-0.0.3/wrapper.sh` & `brnet-0.0.4/wrapper.sh`

 * *Files 22% similar despite different names*

```diff
@@ -11,17 +11,32 @@
 if [ ! -d "${venv}" ]; then
     python3 -m venv ${venv}
 fi
 if [ ! -d "${venv}" ]; then
     echo "No virtualenv at ${venv}; giving up" 1>&2
     exit 1
 fi
-source ${venv}/bin/activate
+source ${venv}/bin/activate || exit 2
 if [ "$(which brnet)" != "${venv}/bin/brnet" ]; then
     python3 -m pip install brnet
 fi
 if [ "$(which brnet)" != "${venv}/bin/brnet" ]; then
+    cwd=$(pwd)
+    mkdir -p "${venv}/src"
+    cd "${venv}/src"
+    if [ -d brnet ]; then
+        cd brnet
+        git checkout main
+        git pull
+    else
+        git clone https://github.com/athornton/brnet
+        cd brnet
+    fi
+    python3 -m pip install -e .
+    cd "${cwd}"
+fi
+if [ "$(which brnet)" != "${venv}/bin/brnet" ]; then
     echo "No brnet in virtualenv; giving up" 1>&2
-    exit 2
+    exit 3
 fi
 
 brnet $*
```

