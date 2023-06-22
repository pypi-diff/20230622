# Comparing `tmp/renku_lock-2.5.0rc3-py3-none-any.whl.zip` & `tmp/renku_lock-2.6.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 3338 bytes, number of entries: 4
+Zip file size: 3324 bytes, number of entries: 4
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 renku_lock/__init__.py
--rw-r--r--  2.0 unx    11433 b- defN 80-Jan-01 00:00 renku_lock-2.5.0rc3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 renku_lock-2.5.0rc3.dist-info/WHEEL
-?rw-r--r--  2.0 unx      302 b- defN 16-Jan-01 00:00 renku_lock-2.5.0rc3.dist-info/RECORD
-4 files, 11848 bytes uncompressed, 2750 bytes compressed:  76.8%
+-rw-r--r--  2.0 unx    11311 b- defN 80-Jan-01 00:00 renku_lock-2.6.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 renku_lock-2.6.0rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      302 b- defN 16-Jan-01 00:00 renku_lock-2.6.0rc1.dist-info/RECORD
+4 files, 11726 bytes uncompressed, 2736 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
 Filename: renku_lock/__init__.py
 Comment: 
 
-Filename: renku_lock-2.5.0rc3.dist-info/METADATA
+Filename: renku_lock-2.6.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: renku_lock-2.5.0rc3.dist-info/WHEEL
+Filename: renku_lock-2.6.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: renku_lock-2.5.0rc3.dist-info/RECORD
+Filename: renku_lock-2.6.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## renku_lock/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "2.5.0rc3"
+__version__ = "2.6.0rc1"
```

## Comparing `renku_lock-2.5.0rc3.dist-info/METADATA` & `renku_lock-2.6.0rc1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renku-lock
-Version: 2.5.0rc3
+Version: 2.6.0rc1
 Summary: Python SDK and CLI for the Renku platform. lock package
 Home-page: https://github.com/swissdatasciencecenter/renku-python
 License: Apache-2.0
 Keywords: Renku,CLI
 Author: Swiss Data Science Center
 Author-email: contact@datascience.ch
 Requires-Python: >=3.8.1,<3.12
@@ -19,18 +19,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: BTrees (==5.0) ; python_version >= "3.7"
-Requires-Dist: CacheControl (==0.12.11) ; python_version >= "3.6"
+Requires-Dist: CacheControl (==0.12.13) ; python_version >= "3.6"
 Requires-Dist: Click (==8.1.3) ; python_version >= "3.7"
 Requires-Dist: Jinja2 (==3.1.2) ; python_version >= "3.7"
-Requires-Dist: MarkupSafe (==2.1.2) ; python_version >= "3.7"
+Requires-Dist: MarkupSafe (==2.1.3) ; python_version >= "3.7"
 Requires-Dist: PyPubSub (==4.0.3) ; python_version >= "3.3" and python_version < "4"
 Requires-Dist: PyYAML (==6.0) ; extra == "yaml" and python_version >= "3.6"
 Requires-Dist: Werkzeug (==2.2.3) ; python_version >= "3.7"
 Requires-Dist: ZConfig (==4.0) ; python_version >= "3.7"
 Requires-Dist: addict (==2.4.0)
 Requires-Dist: ansicon (==1.89.0) ; platform_system == "Windows"
 Requires-Dist: apispec (==6.3.0) ; python_version >= "3.7"
@@ -53,15 +53,15 @@
 Requires-Dist: click (==8.1.3) ; python_version >= "3.7"
 Requires-Dist: click-option-group (==0.5.5) ; python_version >= "3.6" and python_version < "4"
 Requires-Dist: click-plugins (==1.1.1)
 Requires-Dist: colorama (==0.4.6) ; python_version >= "2.7" and python_version < "3.0.dev0" and platform_system == "Windows" or python_version >= "3.7.dev0" and platform_system == "Windows"
 Requires-Dist: coloredlogs (==15.0.1) ; python_version >= "2.7" and python_version < "3.0.dev0" or python_version >= "3.5.dev0"
 Requires-Dist: coverage (==6.4.4) ; python_version >= "3.7"
 Requires-Dist: crontab (==1.0.1)
-Requires-Dist: cryptography (==40.0.2) ; python_version >= "3.6"
+Requires-Dist: cryptography (==41.0.1) ; python_version >= "3.7"
 Requires-Dist: cwl-upgrader (==1.2.8) ; python_version >= "3.6" and python_version < "4"
 Requires-Dist: cwl-utils (==0.27) ; python_version >= "3.6"
 Requires-Dist: cwltool (==3.1.20230425144158) ; python_version >= "3.6" and python_version < "4"
 Requires-Dist: deal (==4.24.1) ; python_version >= "3.7"
 Requires-Dist: deepdiff (==6.3.0) ; python_version >= "3.7"
 Requires-Dist: deepmerge (==1.0.1)
 Requires-Dist: dill (==0.3.6) ; python_version >= "3.7"
@@ -84,18 +84,17 @@
 Requires-Dist: importlib-resources (==5.12.0) ; python_version >= "3.7"
 Requires-Dist: inject (==4.3.1)
 Requires-Dist: isodate (==0.6.1)
 Requires-Dist: itsdangerous (==2.1.2) ; python_version >= "3.7"
 Requires-Dist: jinja2 (==3.1.2) ; python_version >= "3.7"
 Requires-Dist: jinxed (==1.2.0) ; platform_system == "Windows"
 Requires-Dist: lazy-object-proxy (==1.9.0) ; python_version >= "3.7"
-Requires-Dist: lockfile (==0.12.2) ; extra == "filecache"
 Requires-Dist: lxml (==4.9.2) ; python_version >= "2.7" and python_version < "3.0.dev0" or python_version >= "3.5.dev0"
 Requires-Dist: markdown-it-py (==2.2.0) ; python_version >= "3.7"
-Requires-Dist: markupsafe (==2.1.2) ; extra == "flask" and python_version >= "3.7"
+Requires-Dist: markupsafe (==2.1.3) ; extra == "flask" and python_version >= "3.7"
 Requires-Dist: marshmallow (==3.19.0) ; python_version >= "3.7"
 Requires-Dist: marshmallow-oneofschema (==3.0.1) ; python_version >= "3.6"
 Requires-Dist: mdurl (==0.1.2) ; python_version >= "3.7"
 Requires-Dist: mistune (==2.0.5)
 Requires-Dist: msgpack (==1.0.5)
 Requires-Dist: mypy-extensions (==1.0.0) ; python_version >= "3.5"
 Requires-Dist: networkx (==3.1) ; python_version >= "3.8"
@@ -130,38 +129,38 @@
 Requires-Dist: python-gitlab (==3.8.1) ; python_full_version >= "3.7.0"
 Requires-Dist: pytz (==2023.3)
 Requires-Dist: pywin32 (==227) ; sys_platform == "win32"
 Requires-Dist: pyyaml (==6.0) ; python_version >= "3.6"
 Requires-Dist: pyzmq (==25.1.0) ; python_version >= "3.6"
 Requires-Dist: rdflib (==6.3.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: redis (==4.5.5) ; python_version >= "3.7"
-Requires-Dist: renku (==2.5.0rc3)
+Requires-Dist: renku (==2.6.0rc1)
 Requires-Dist: requests (==2.31.0) ; python_version >= "3.7"
 Requires-Dist: requests-toolbelt (==1.0.0) ; python_version >= "2.7" and python_version < "3.0.dev0" or python_version >= "3.4.dev0"
 Requires-Dist: rich (==13.3.5) ; python_full_version >= "3.7.0"
-Requires-Dist: rq (==1.14.1) ; python_version >= "3.6"
+Requires-Dist: rq (==1.15.0) ; python_version >= "3.6"
 Requires-Dist: rq-scheduler (==0.13.1)
 Requires-Dist: ruamel.yaml (==0.17.21) ; python_version >= "3.7"
 Requires-Dist: ruamel.yaml.clib (==0.2.7) ; platform_python_implementation == "CPython" and python_version < "3.11" and python_version >= "3.5"
 Requires-Dist: schema-salad (==8.4.20230601112322) ; python_version >= "3.6" and python_version < "3.12"
-Requires-Dist: sentry-sdk (==1.23.1)
+Requires-Dist: sentry-sdk (==1.25.0)
 Requires-Dist: setuptools (==67.8.0) ; python_version >= "3.7"
 Requires-Dist: shellescape (==3.8.1)
 Requires-Dist: shellingham (==1.5.0.post1) ; python_version >= "3.7"
 Requires-Dist: six (==1.16.0) ; python_version >= "2.7" and python_version < "3.0.dev0" or python_version >= "3.3.dev0"
 Requires-Dist: smmap (==5.0.0) ; python_version >= "3.6"
 Requires-Dist: tabulate (==0.9.0) ; python_version >= "3.7"
 Requires-Dist: termcolor (==1.1.0)
 Requires-Dist: toil (==5.10.0) ; python_version >= "3.7"
 Requires-Dist: tomli (==2.0.1) ; python_full_version <= "3.11.0a6" and extra == "toml" and python_version >= "3.7"
 Requires-Dist: tomlkit (==0.11.8) ; python_version >= "3.7"
 Requires-Dist: tornado (==6.3.2) ; python_version >= "3.8"
-Requires-Dist: tqdm (==4.62.3) ; python_version >= "2.7" and python_version < "3.0.dev0" or python_version >= "3.4.dev0"
+Requires-Dist: tqdm (==4.65.0) ; python_version >= "3.7"
 Requires-Dist: transaction (==3.1.0) ; python_version >= "2.7" and python_version < "3.0.dev0" or python_version >= "3.5.dev0"
-Requires-Dist: typing-extensions (==4.6.2) ; python_version >= "3.7"
+Requires-Dist: typing-extensions (==4.6.3) ; python_version >= "3.7"
 Requires-Dist: urllib3 (==1.26.16) ; python_version >= "2.7" and python_version < "3.0.dev0" or python_version >= "3.6.dev0"
 Requires-Dist: walrus (==0.9.2)
 Requires-Dist: wcwidth (==0.2.6)
 Requires-Dist: websocket-client (==1.5.2) ; python_version >= "3.7"
 Requires-Dist: werkzeug (==2.2.3) ; python_version >= "3.7"
 Requires-Dist: yagup (==0.1.1)
 Requires-Dist: yaspin (==2.1.0) ; python_full_version >= "3.6.2" and python_full_version < "4.0.0"
```

