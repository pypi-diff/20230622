# Comparing `tmp/structlog_sentry-2.0.2.tar.gz` & `tmp/structlog_sentry-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structlog_sentry-2.0.2.tar", max compression
+gzip compressed data, was "structlog_sentry-2.0.3.tar", max compression
```

## Comparing `structlog_sentry-2.0.2.tar` & `structlog_sentry-2.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       20 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/.coveragerc
--rw-r--r--   0        0        0      618 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1065 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/LICENSE
--rw-r--r--   0        0        0     5876 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/README.md
--rw-r--r--   0        0        0     1225 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     7884 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/structlog_sentry/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/structlog_sentry/py.typed
--rw-r--r--   0        0        0      581 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/tox.ini
--rw-r--r--   0        0        0     7178 1970-01-01 00:00:00.000000 structlog_sentry-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-06-22 10:35:29.978259 structlog_sentry-2.0.3/.coveragerc
+-rw-r--r--   0        0        0      716 2023-06-22 10:35:29.978259 structlog_sentry-2.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1065 2023-06-22 10:35:29.978259 structlog_sentry-2.0.3/LICENSE
+-rw-r--r--   0        0        0     5941 2023-06-22 10:35:29.978259 structlog_sentry-2.0.3/README.md
+-rw-r--r--   0        0        0     1209 2023-06-22 10:35:29.978259 structlog_sentry-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7465 2023-06-22 10:35:29.978259 structlog_sentry-2.0.3/structlog_sentry/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 10:35:29.978259 structlog_sentry-2.0.3/structlog_sentry/py.typed
+-rw-r--r--   0        0        0      581 2023-06-22 10:35:29.978259 structlog_sentry-2.0.3/tox.ini
+-rw-r--r--   0        0        0     6969 1970-01-01 00:00:00.000000 structlog_sentry-2.0.3/PKG-INFO
```

### Comparing `structlog_sentry-2.0.2/.pre-commit-config.yaml` & `structlog_sentry-2.0.3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,7 +20,12 @@
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
+
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.4.0
+    hooks:
+      - id: mypy
```

### Comparing `structlog_sentry-2.0.2/LICENSE` & `structlog_sentry-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `structlog_sentry-2.0.2/README.md` & `structlog_sentry-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 from structlog_sentry import SentryProcessor
 
 
 sentry_sdk.init()  # pass dsn in argument or via SENTRY_DSN env variable
 
 structlog.configure(
     processors=[
-        structlog.stdlib.add_logger_name,  # optional, but before SentryProcessor()
+        structlog.stdlib.add_logger_name,  # optional, must be placed before SentryProcessor()
         structlog.stdlib.add_log_level,  # required before SentryProcessor()
         SentryProcessor(event_level=logging.ERROR),
     ],
-    logger_factory=...,
-    wrapper_class=...,
+    logger_factory=structlog.stdlib.LoggerFactory(),
+    wrapper_class=structlog.stdlib.BoundLogger,
 )
 
 
 log = structlog.get_logger()
 ```
 
 Do not forget to add the `structlog.stdlib.add_log_level` and optionally the
```

### Comparing `structlog_sentry-2.0.2/pyproject.toml` & `structlog_sentry-2.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "structlog-sentry"
-version = "2.0.2"
+version = "2.0.3"
 description = "Sentry integration for structlog"
 authors = ["Kiwi.com platform <platform@kiwi.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/kiwicom/structlog-sentry"
 homepage = "https://github.com/kiwicom/structlog-sentry"
 
@@ -21,19 +21,18 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["*.md", "*.toml", "*.txt", "*.yml", "*.yaml", ".coveragerc", "tox.ini", "structlog_sentry/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-packaging = "*"
 sentry-sdk = "*"
 structlog = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.8.2"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `structlog_sentry-2.0.2/structlog_sentry/__init__.py` & `structlog_sentry-2.0.3/structlog_sentry/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from __future__ import annotations
 
 import logging
 import sys
 from fnmatch import fnmatch
 from typing import Any, Iterable, Optional
 
-from packaging import version
-
-from sentry_sdk import VERSION, Hub
+from sentry_sdk import Hub
 from sentry_sdk.integrations.logging import _IGNORED_LOGGERS
 from sentry_sdk.utils import capture_internal_exceptions, event_from_exception
 from structlog.types import EventDict, ExcInfo, WrappedLogger
 
-_IS_OLD_VERSION = version.parse(VERSION) < version.parse("1.17.0")
-
 
 def _figure_out_exc_info(v: Any) -> ExcInfo:
     """
     Depending on the Python version will try to do the smartest thing possible
     to transform *v* into an ``exc_info`` tuple.
     """
     if isinstance(v, BaseException):
@@ -67,15 +63,15 @@
         self.level = level
         self.active = active
         self.tag_keys = tag_keys
         self.verbose = verbose
 
         self._hub = hub
         self._as_context = as_context
-        self._original_event_dict: dict = None
+        self._original_event_dict: dict = {}
 
         self._ignored_loggers: set[str] = set()
         if ignore_loggers is not None:
             self._ignored_loggers.update(set(ignore_loggers))
 
     @staticmethod
     def _get_logger_name(logger: WrappedLogger, event_dict: dict) -> Optional[str]:
@@ -107,24 +103,17 @@
 
         :param event_dict: structlog event_dict
         """
         exc_info = _figure_out_exc_info(event_dict.get("exc_info", None))
         has_exc_info = exc_info and exc_info != (None, None, None)
 
         if has_exc_info:
-            options = self._get_hub().client.options
-            include_local_variables = options.get(
-                "include_local_variables", options.get("with_locals")
-            )
-            key = "with_locals" if _IS_OLD_VERSION else "include_local_variables"
             event, hint = event_from_exception(
                 exc_info,
-                client_options={
-                    key: include_local_variables,
-                },
+                client_options=self._get_hub().client.options,
             )
         else:
             event, hint = {}, {}
 
         event["message"] = event_dict.get("event")
         event["level"] = event_dict.get("level")
         if "logger" in event_dict:
```

### Comparing `structlog_sentry-2.0.2/tox.ini` & `structlog_sentry-2.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `structlog_sentry-2.0.2/PKG-INFO` & `structlog_sentry-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structlog-sentry
-Version: 2.0.2
+Version: 2.0.3
 Summary: Sentry integration for structlog
 Home-page: https://github.com/kiwicom/structlog-sentry
 License: MIT
 Author: Kiwi.com platform
 Author-email: platform@kiwi.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,21 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: packaging
 Requires-Dist: sentry-sdk
 Requires-Dist: structlog
 Project-URL: Repository, https://github.com/kiwicom/structlog-sentry
 Description-Content-Type: text/markdown
 
 # structlog-sentry
 
@@ -57,20 +51,20 @@
 from structlog_sentry import SentryProcessor
 
 
 sentry_sdk.init()  # pass dsn in argument or via SENTRY_DSN env variable
 
 structlog.configure(
     processors=[
-        structlog.stdlib.add_logger_name,  # optional, but before SentryProcessor()
+        structlog.stdlib.add_logger_name,  # optional, must be placed before SentryProcessor()
         structlog.stdlib.add_log_level,  # required before SentryProcessor()
         SentryProcessor(event_level=logging.ERROR),
     ],
-    logger_factory=...,
-    wrapper_class=...,
+    logger_factory=structlog.stdlib.LoggerFactory(),
+    wrapper_class=structlog.stdlib.BoundLogger,
 )
 
 
 log = structlog.get_logger()
 ```
 
 Do not forget to add the `structlog.stdlib.add_log_level` and optionally the
```

