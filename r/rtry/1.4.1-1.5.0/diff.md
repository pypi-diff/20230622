# Comparing `tmp/rtry-1.4.1.tar.gz` & `tmp/rtry-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtry-1.4.1.tar", last modified: Sun Jan 23 17:51:04 2022, max compression
+gzip compressed data, was "rtry-1.5.0.tar", last modified: Thu Jun 22 17:00:38 2023, max compression
```

## Comparing `rtry-1.4.1.tar` & `rtry-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-23 17:51:04.132676 rtry-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-01-23 17:50:55.000000 rtry-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7182 2022-01-23 17:51:04.132676 rtry-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6372 2022-01-23 17:50:55.000000 rtry-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-23 17:51:04.132676 rtry-1.4.1/rtry/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-01-23 17:50:55.000000 rtry-1.4.1/rtry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-01-23 17:50:55.000000 rtry-1.4.1/rtry/_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     5162 2022-01-23 17:50:55.000000 rtry-1.4.1/rtry/_retry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3494 2022-01-23 17:50:55.000000 rtry-1.4.1/rtry/_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4925 2022-01-23 17:50:55.000000 rtry-1.4.1/rtry/_timeout.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-01-23 17:50:55.000000 rtry-1.4.1/rtry/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-23 17:50:55.000000 rtry-1.4.1/rtry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-23 17:51:04.132676 rtry-1.4.1/rtry/types/
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-01-23 17:50:55.000000 rtry-1.4.1/rtry/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-23 17:51:04.132676 rtry-1.4.1/rtry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7182 2022-01-23 17:51:04.000000 rtry-1.4.1/rtry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-01-23 17:51:04.000000 rtry-1.4.1/rtry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-23 17:51:04.000000 rtry-1.4.1/rtry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-23 17:51:04.000000 rtry-1.4.1/rtry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-01-23 17:51:04.132676 rtry-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-01-23 17:50:55.000000 rtry-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:00:38.595158 rtry-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 17:00:28.000000 rtry-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-06-22 17:00:38.595158 rtry-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-06-22 17:00:28.000000 rtry-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:00:38.595158 rtry-1.5.0/rtry/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-22 17:00:28.000000 rtry-1.5.0/rtry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-22 17:00:28.000000 rtry-1.5.0/rtry/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-22 17:00:28.000000 rtry-1.5.0/rtry/_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-22 17:00:28.000000 rtry-1.5.0/rtry/_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-22 17:00:28.000000 rtry-1.5.0/rtry/_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 17:00:28.000000 rtry-1.5.0/rtry/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:00:28.000000 rtry-1.5.0/rtry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:00:38.595158 rtry-1.5.0/rtry/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-22 17:00:28.000000 rtry-1.5.0/rtry/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:00:38.595158 rtry-1.5.0/rtry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-06-22 17:00:38.000000 rtry-1.5.0/rtry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 17:00:38.000000 rtry-1.5.0/rtry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:00:38.000000 rtry-1.5.0/rtry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 17:00:38.000000 rtry-1.5.0/rtry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-22 17:00:38.595158 rtry-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-22 17:00:28.000000 rtry-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:00:38.595158 rtry-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13822 2023-06-22 17:00:28.000000 rtry-1.5.0/tests/test_async_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-06-22 17:00:28.000000 rtry-1.5.0/tests/test_async_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-06-22 17:00:28.000000 rtry-1.5.0/tests/test_async_timeout_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-06-22 17:00:28.000000 rtry-1.5.0/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-22 17:00:28.000000 rtry-1.5.0/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-06-22 17:00:28.000000 rtry-1.5.0/tests/test_timeout_context.py
```

### Comparing `rtry-1.4.1/LICENSE.txt` & `rtry-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rtry-1.4.1/PKG-INFO` & `rtry-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: rtry
-Version: 1.4.1
+Version: 1.5.0
 Summary: The easiest way to retry operations
-Home-page: https://github.com/nikitanovosibirsk/rtry
+Home-page: https://github.com/tsv1/rtry
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # rtry
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/rtry/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/rtry)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/rtry/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/rtry)
 [![PyPI](https://img.shields.io/pypi/v/rtry.svg?style=flat-square)](https://pypi.python.org/pypi/rtry/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rtry?style=flat-square)](https://pypi.python.org/pypi/rtry/)
 [![Python Version](https://img.shields.io/pypi/pyversions/rtry.svg?style=flat-square)](https://pypi.python.org/pypi/rtry/)
 
 ## Installation
 
 ```bash
@@ -313,9 +309,7 @@
     # <ClientResponse(https://httpbin.org/status/500) [500 INTERNAL SERVER ERROR]>
     # <ClientResponse(https://httpbin.org/status/500) [500 INTERNAL SERVER ERROR]>
     # Traceback
     #   AssertionError
 
 asyncio.run(main())
 ```
-
-
```

### Comparing `rtry-1.4.1/README.md` & `rtry-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # rtry
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/rtry/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/rtry)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/rtry/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/rtry)
 [![PyPI](https://img.shields.io/pypi/v/rtry.svg?style=flat-square)](https://pypi.python.org/pypi/rtry/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rtry?style=flat-square)](https://pypi.python.org/pypi/rtry/)
 [![Python Version](https://img.shields.io/pypi/pyversions/rtry.svg?style=flat-square)](https://pypi.python.org/pypi/rtry/)
 
 ## Installation
 
 ```bash
```

### Comparing `rtry-1.4.1/rtry/_retry.py` & `rtry-1.5.0/rtry/_retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,24 @@
             except CancelledError:
                 raise
             except self._swallow as e:
                 exception = e
             else:
                 if self._until is None:
                     return result
-                elif not(self._until(result)):
+                elif not self._until(result):
                     return result
                 exception = None
             retried += 1
             if hasattr(self._logger, "__call__"):
                 self._logger(retried, exception or result, self._fn)  # type: ignore
             if self._delay is not None:
                 delay = self._delay
                 if hasattr(self._delay, "__call__"):
-                    delay = self._delay(retried)  # type: ignore
+                    delay = self._delay(retried)
                 time.sleep(delay)  # type: ignore
             else:
                 time.sleep(0)
         if exception:
             raise exception
         return result
 
@@ -87,24 +87,24 @@
             except (CancelledError, asyncio.CancelledError):
                 raise
             except self._swallow as e:
                 exception = e
             else:
                 if self._until is None:
                     return result
-                elif not(self._until(result)):
+                elif not self._until(result):
                     return result
                 exception = None
             retried += 1
             if hasattr(self._logger, "__call__"):
                 self._logger(retried, exception or result, self._fn)  # type: ignore
             if self._delay is not None:
                 delay = self._delay
                 if hasattr(self._delay, "__call__"):
-                    delay = self._delay(retried)  # type: ignore
+                    delay = self._delay(retried)
                 await asyncio.sleep(delay)  # type: ignore
             else:
                 await asyncio.sleep(0)
         if exception:
             raise exception
         return result
```

### Comparing `rtry-1.4.1/rtry/_scheduler.py` & `rtry-1.5.0/rtry/_scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         orig_handler = signal.getsignal(signal.SIGALRM)
         if not isinstance(orig_handler, type(self)):
             self._orig_handler = orig_handler
 
         priority = -len(self._scheduler.queue)
         event = self._scheduler.enter(seconds, priority, handler)
 
-        signal.signal(signal.SIGALRM, self)
+        signal.signal(signal.SIGALRM, self)  # type: ignore
         signal.setitimer(self._itimer, self._next_event())
 
         return event
 
     def cancel(self, event: Union[Event, None]) -> None:
         try:
             self._scheduler.cancel(event)  # type: ignore
```

### Comparing `rtry-1.4.1/rtry/_timeout.py` & `rtry-1.5.0/rtry/_timeout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import sys
 from functools import wraps
 from types import TracebackType
 from typing import Any, Optional, Type, Union
 
 from ._errors import CancelledError
 from ._scheduler import AsyncEvent, AsyncScheduler, Event, Scheduler
 from ._types import AnyCallable, ExceptionType, TimeoutValue
@@ -85,18 +84,15 @@
                  exc_tb: Optional[TracebackType]) -> bool:
         self._scheduler.cancel(self._event)
         if isinstance(exc_val, self._exception):
             return self._silent
         return exc_val is None
 
     async def __aenter__(self) -> AsyncTimeoutProxy:
-        if sys.version_info >= (3, 7):  # pragma: no cover
-            task = asyncio.current_task()
-        else:  # pragma: no cover
-            task = asyncio.Task.current_task()
+        task = asyncio.current_task()
 
         def async_handler(task: "Optional[asyncio.Task[None]]" = task) -> None:
             self._async_scheduler.cancel(self._event)
             if task:  # pragma: no branch
                 self._raised = self._exception()
                 task.cancel()
```

### Comparing `rtry-1.4.1/rtry/_types.py` & `rtry-1.5.0/rtry/_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from signal import Handlers, Signals
+from signal import Handlers
 from types import FrameType
 from typing import Any, Callable, Tuple, Type, Union
 
 __all__ = ("AttemptValue", "TimeoutValue", "DelayValue", "DelayCallable",
            "AnyCallable", "ExceptionType", "LoggerCallable", "UntilCallable",
            "SwallowException", "SignalHandler",)
 
@@ -11,8 +11,8 @@
 DelayValue = Union[float, int]
 DelayCallable = Callable[[AttemptValue], DelayValue]
 AnyCallable = Callable[..., Any]
 ExceptionType = Type[BaseException]
 LoggerCallable = Callable[[AttemptValue, Any, AnyCallable], Any]
 UntilCallable = Callable[[Any], bool]
 SwallowException = Union[Tuple[ExceptionType, ...], ExceptionType]
-SignalHandler = Union[Callable[[Signals, FrameType], None], int, Handlers, None]
+SignalHandler = Union[Callable[[int, Union[FrameType, None]], Any], int, Handlers, None]
```

### Comparing `rtry-1.4.1/rtry/types/__init__.py` & `rtry-1.5.0/rtry/types/__init__.py`

 * *Files identical despite different names*

### Comparing `rtry-1.4.1/rtry.egg-info/PKG-INFO` & `rtry-1.5.0/rtry.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: rtry
-Version: 1.4.1
+Version: 1.5.0
 Summary: The easiest way to retry operations
-Home-page: https://github.com/nikitanovosibirsk/rtry
+Home-page: https://github.com/tsv1/rtry
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # rtry
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/rtry/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/rtry)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/rtry/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/rtry)
 [![PyPI](https://img.shields.io/pypi/v/rtry.svg?style=flat-square)](https://pypi.python.org/pypi/rtry/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rtry?style=flat-square)](https://pypi.python.org/pypi/rtry/)
 [![Python Version](https://img.shields.io/pypi/pyversions/rtry.svg?style=flat-square)](https://pypi.python.org/pypi/rtry/)
 
 ## Installation
 
 ```bash
@@ -313,9 +309,7 @@
     # <ClientResponse(https://httpbin.org/status/500) [500 INTERNAL SERVER ERROR]>
     # <ClientResponse(https://httpbin.org/status/500) [500 INTERNAL SERVER ERROR]>
     # Traceback
     #   AssertionError
 
 asyncio.run(main())
 ```
-
-
```

### Comparing `rtry-1.4.1/setup.cfg` & `rtry-1.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.4.1
+current_version = 1.5.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `rtry-1.4.1/setup.py` & `rtry-1.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,33 +9,30 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="rtry",
-    version="1.4.1",
+    version="1.5.0",
     description="The easiest way to retry operations",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
-    python_requires=">=3.6.0",
-    url="https://github.com/nikitanovosibirsk/rtry",
+    author_email="tsv1@fastmail.com",
+    python_requires=">=3.7",
+    url="https://github.com/tsv1/rtry",
     license="MIT",
-    packages=find_packages(exclude=("tests",)),
+    packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"rtry": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
 )
```

