# Comparing `tmp/Kuyruk-9.4.0.tar.gz` & `tmp/Kuyruk-9.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Kuyruk-9.4.0.tar", last modified: Thu Mar 26 21:21:39 2020, max compression
+gzip compressed data, was "Kuyruk-9.4.1.tar", last modified: Thu Jun 22 21:03:42 2023, max compression
```

## Comparing `Kuyruk-9.4.0.tar` & `Kuyruk-9.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      898 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1076 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      335 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-03-26 21:21:24.000000 Kuyruk-9.4.0/VERSION
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/Kuyruk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/Kuyruk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-26 21:20:30.000000 Kuyruk-9.4.0/Kuyruk.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/Kuyruk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/Kuyruk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/Kuyruk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/Kuyruk.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/Kuyruk.egg-info/SOURCES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-26 21:21:39.000000 Kuyruk-9.4.0/kuyruk/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/importer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1575 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14967 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/worker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2622 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3300 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/signals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      444 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3923 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4480 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/kuyruk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1318 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1609 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/heartbeat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8111 2020-03-26 21:20:29.000000 Kuyruk-9.4.0/kuyruk/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:03:42.537269 Kuyruk-9.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:03:42.537269 Kuyruk-9.4.1/Kuyruk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-22 21:03:42.000000 Kuyruk-9.4.1/Kuyruk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-22 21:03:42.000000 Kuyruk-9.4.1/Kuyruk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:03:42.000000 Kuyruk-9.4.1/Kuyruk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-22 21:03:42.000000 Kuyruk-9.4.1/Kuyruk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 21:03:42.000000 Kuyruk-9.4.1/Kuyruk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 21:03:42.000000 Kuyruk-9.4.1/Kuyruk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:02:47.000000 Kuyruk-9.4.1/Kuyruk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-22 21:03:42.537269 Kuyruk-9.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 21:03:35.000000 Kuyruk-9.4.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:03:42.537269 Kuyruk-9.4.1/kuyruk/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/kuyruk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15126 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/kuyruk/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-22 21:03:42.537269 Kuyruk-9.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-22 21:02:38.000000 Kuyruk-9.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Kuyruk-9.4.0/README.rst` & `Kuyruk-9.4.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 .. image:: https://raw.githubusercontent.com/cenkalti/kuyruk/master/docs/_static/lemur.png
    :alt: Kuyruk Logo
 
 Kuyruk
 ======
 
-.. image:: https://travis-ci.org/cenkalti/kuyruk.svg?branch=master
-   :target: https://travis-ci.org/cenkalti/kuyruk?branch=master
+.. image:: https://github.com/cenkalti/kuyruk/actions/workflows/build.yml/badge.svg?branch=master
+   :target: https://github.com/cenkalti/kuyruk/actions
 
 .. image:: https://coveralls.io/repos/github/cenkalti/kuyruk/badge.svg?branch=master
    :target: https://coveralls.io/github/cenkalti/kuyruk?branch=master
 
 .. image:: https://img.shields.io/pypi/v/kuyruk.svg?branch=master
    :target: https://pypi.org/project/Kuyruk/
 
 
 Kuyruk is a simple and easy way of distributing tasks to run on servers.
 
 It uses `RabbitMQ <http://www.rabbitmq.com>`_ as message broker and
 depends on `amqp <http://amqp.readthedocs.org/>`_
 which is a pure-Python RabbitMQ client library.
-Compatible with Python 3.5+.
+Compatible with Python 3.8+.
 
 
 Where is the documentation?
 ---------------------------
 Here it is: http://kuyruk.readthedocs.org
```

### Comparing `Kuyruk-9.4.0/setup.py` & `Kuyruk-9.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,13 +36,12 @@
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
         'Topic :: Software Development :: Object Brokering',
         'Topic :: System :: Distributed Computing',
     ],
 )
```

### Comparing `Kuyruk-9.4.0/LICENSE` & `Kuyruk-9.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Kuyruk-9.4.0/PKG-INFO` & `Kuyruk-9.4.1/Kuyruk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: Kuyruk
-Version: 9.4.0
+Version: 9.4.1
 Summary: Simple task queue
 Home-page: https://github.com/cenkalti/kuyruk
 Author: Cenk Altı
 Author-email: cenkalti@gmail.com
-License: UNKNOWN
-Description: .. image:: https://raw.githubusercontent.com/cenkalti/kuyruk/master/docs/_static/lemur.png
-           :alt: Kuyruk Logo
-        
-        Kuyruk
-        ======
-        
-        .. image:: https://travis-ci.org/cenkalti/kuyruk.svg?branch=master
-           :target: https://travis-ci.org/cenkalti/kuyruk?branch=master
-        
-        .. image:: https://coveralls.io/repos/github/cenkalti/kuyruk/badge.svg?branch=master
-           :target: https://coveralls.io/github/cenkalti/kuyruk?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/kuyruk.svg?branch=master
-           :target: https://pypi.org/project/Kuyruk/
-        
-        
-        Kuyruk is a simple and easy way of distributing tasks to run on servers.
-        
-        It uses `RabbitMQ <http://www.rabbitmq.com>`_ as message broker and
-        depends on `amqp <http://amqp.readthedocs.org/>`_
-        which is a pure-Python RabbitMQ client library.
-        Compatible with Python 3.5+.
-        
-        
-        Where is the documentation?
-        ---------------------------
-        Here it is: http://kuyruk.readthedocs.org
-        
 Keywords: rabbitmq distributed task queue
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Topic :: System :: Distributed Computing
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/cenkalti/kuyruk/master/docs/_static/lemur.png
+   :alt: Kuyruk Logo
+
+Kuyruk
+======
+
+.. image:: https://github.com/cenkalti/kuyruk/actions/workflows/build.yml/badge.svg?branch=master
+   :target: https://github.com/cenkalti/kuyruk/actions
+
+.. image:: https://coveralls.io/repos/github/cenkalti/kuyruk/badge.svg?branch=master
+   :target: https://coveralls.io/github/cenkalti/kuyruk?branch=master
+
+.. image:: https://img.shields.io/pypi/v/kuyruk.svg?branch=master
+   :target: https://pypi.org/project/Kuyruk/
+
+
+Kuyruk is a simple and easy way of distributing tasks to run on servers.
+
+It uses `RabbitMQ <http://www.rabbitmq.com>`_ as message broker and
+depends on `amqp <http://amqp.readthedocs.org/>`_
+which is a pure-Python RabbitMQ client library.
+Compatible with Python 3.8+.
+
+
+Where is the documentation?
+---------------------------
+Here it is: http://kuyruk.readthedocs.org
```

### Comparing `Kuyruk-9.4.0/Kuyruk.egg-info/PKG-INFO` & `Kuyruk-9.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: Kuyruk
-Version: 9.4.0
+Version: 9.4.1
 Summary: Simple task queue
 Home-page: https://github.com/cenkalti/kuyruk
 Author: Cenk Altı
 Author-email: cenkalti@gmail.com
-License: UNKNOWN
-Description: .. image:: https://raw.githubusercontent.com/cenkalti/kuyruk/master/docs/_static/lemur.png
-           :alt: Kuyruk Logo
-        
-        Kuyruk
-        ======
-        
-        .. image:: https://travis-ci.org/cenkalti/kuyruk.svg?branch=master
-           :target: https://travis-ci.org/cenkalti/kuyruk?branch=master
-        
-        .. image:: https://coveralls.io/repos/github/cenkalti/kuyruk/badge.svg?branch=master
-           :target: https://coveralls.io/github/cenkalti/kuyruk?branch=master
-        
-        .. image:: https://img.shields.io/pypi/v/kuyruk.svg?branch=master
-           :target: https://pypi.org/project/Kuyruk/
-        
-        
-        Kuyruk is a simple and easy way of distributing tasks to run on servers.
-        
-        It uses `RabbitMQ <http://www.rabbitmq.com>`_ as message broker and
-        depends on `amqp <http://amqp.readthedocs.org/>`_
-        which is a pure-Python RabbitMQ client library.
-        Compatible with Python 3.5+.
-        
-        
-        Where is the documentation?
-        ---------------------------
-        Here it is: http://kuyruk.readthedocs.org
-        
 Keywords: rabbitmq distributed task queue
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Topic :: System :: Distributed Computing
+License-File: LICENSE
+
+.. image:: https://raw.githubusercontent.com/cenkalti/kuyruk/master/docs/_static/lemur.png
+   :alt: Kuyruk Logo
+
+Kuyruk
+======
+
+.. image:: https://github.com/cenkalti/kuyruk/actions/workflows/build.yml/badge.svg?branch=master
+   :target: https://github.com/cenkalti/kuyruk/actions
+
+.. image:: https://coveralls.io/repos/github/cenkalti/kuyruk/badge.svg?branch=master
+   :target: https://coveralls.io/github/cenkalti/kuyruk?branch=master
+
+.. image:: https://img.shields.io/pypi/v/kuyruk.svg?branch=master
+   :target: https://pypi.org/project/Kuyruk/
+
+
+Kuyruk is a simple and easy way of distributing tasks to run on servers.
+
+It uses `RabbitMQ <http://www.rabbitmq.com>`_ as message broker and
+depends on `amqp <http://amqp.readthedocs.org/>`_
+which is a pure-Python RabbitMQ client library.
+Compatible with Python 3.8+.
+
+
+Where is the documentation?
+---------------------------
+Here it is: http://kuyruk.readthedocs.org
```

### Comparing `Kuyruk-9.4.0/kuyruk/importer.py` & `Kuyruk-9.4.1/kuyruk/importer.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 
 def import_object_str(s: str) -> Any:
     module, obj = s.rsplit('.', 1)
     return import_object(module, obj)
 
 
 def main_module_name() -> str:
-    """Returns main module and module name pair."""
+    """Returns main module name."""
     if not hasattr(main_module, '__file__'):
         # running from interactive shell
-        return None
+        return 'None'
 
+    assert isinstance(main_module.__file__, str)
     main_filename = os.path.basename(main_module.__file__)
     module_name, ext = os.path.splitext(main_filename)
     return module_name
```

### Comparing `Kuyruk-9.4.0/kuyruk/exceptions.py` & `Kuyruk-9.4.1/kuyruk/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Tuple, Type
+from typing import Tuple, Type, Union
 from types import TracebackType
 
-ExcInfoType = Tuple[Type[BaseException], BaseException, TracebackType]
+ExcInfoType = Union[Tuple[Type[BaseException], BaseException, TracebackType], Tuple[None, None, None]]
 
 
 class KuyrukError(Exception):
     """Base class for Kuyruk exceptions."""
     pass
```

### Comparing `Kuyruk-9.4.0/kuyruk/worker.py` & `Kuyruk-9.4.1/kuyruk/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 import logging.config
 import threading
 import traceback
 import argparse
 import multiprocessing
 from time import monotonic
-from typing import Dict, Any, List, Tuple  # noqa
+from typing import Dict, Any, List, Tuple, Optional, Type, cast  # noqa
 
 import amqp
 
 from kuyruk import importer, signals
 from kuyruk.kuyruk import Kuyruk
 from kuyruk.task import Task
 from kuyruk.heartbeat import Heartbeat
@@ -45,19 +45,20 @@
                 return queue
 
         self._hostname = socket.gethostname()
         self.queues = [add_host(q) for q in args.queues]
         self._tasks = {}  # type: Dict[Tuple[str, str], Task]
         self.shutdown_pending = threading.Event()
         self.consuming = False
-        self.current_task = None  # type: Task
-        self.current_args = None  # type: Tuple
-        self.current_kwargs = None  # type: Dict[str, Any]
+        self.current_task = None  # type: Optional[Task]
+        self.current_args = None  # type: Optional[Tuple]
+        self.current_kwargs = None  # type: Optional[Dict[str, Any]]
+        self._heartbeat_error: Optional[Exception]
 
-        self._started_at = None  # type: float
+        self._started_at = None  # type: Optional[float]
         self._pid = os.getpid()
 
         self._logging_level = app.config.WORKER_LOGGING_LEVEL
         if args.logging_level is not None:
             self._logging_level = args.logging_level
 
         self._max_run_time = app.config.WORKER_MAX_RUN_TIME
@@ -128,15 +129,15 @@
 
         logger.debug("End run worker")
 
     def _consume_messages(self) -> None:
         with self.kuyruk.channel() as ch:
             # Set prefetch count to 1. If we don't set this, RabbitMQ keeps
             # sending messages while we are already working on a message.
-            ch.basic_qos(0, 1, True)
+            ch.basic_qos(0, 1, False)
 
             self._declare_queues(ch)
             self._consume_queues(ch)
             logger.info('Consumer started')
             self._main_loop(ch)
 
     def _main_loop(self, ch: amqp.Channel) -> None:
@@ -240,15 +241,15 @@
             message.channel.basic_reject(message.delivery_tag, requeue=True)
         except Discard:
             logger.warning('Task is discarded')
             message.channel.basic_reject(message.delivery_tag, requeue=False)
             if reply_to:
                 exc_info = sys.exc_info()
                 self._send_reply(reply_to, message.channel, None, exc_info)
-        except HeartbeatError as e:
+        except HeartbeatError:
             exc_info = sys.exc_info()
             logger.error('Heartbeat error:\n%s', ''.join(traceback.format_exception(*exc_info)))
             signals.worker_failure.send(
                 self.kuyruk,
                 description=description,
                 task=task,
                 args=args,
@@ -316,15 +317,15 @@
             logger.info("%s finished in %i seconds." % (task.name, delta))
 
     def _send_reply(
             self,
             reply_to: str,
             channel: amqp.Channel,
             result: Any,
-            exc_info: ExcInfoType,
+            exc_info: Optional[ExcInfoType],
     ) -> None:
         logger.debug("Sending reply result=%r", result)
 
         reply = {'result': result}
         if exc_info:
             reply['exception'] = self._exc_info_dict(exc_info)
 
@@ -339,15 +340,15 @@
         msg = amqp.Message(body=body)
         channel.basic_publish(msg, exchange="", routing_key=reply_to)
 
     @staticmethod
     def _exc_info_dict(exc_info: ExcInfoType) -> Dict[str, str]:
         type_, val, tb = exc_info
         return {
-            'type': '%s.%s' % (type_.__module__, type_.__name__),
+            'type': '%s.%s' % (type_.__module__, cast(Type[BaseException], type_).__name__),
             'value': str(val),
             'traceback': ''.join(traceback.format_tb(tb)),
         }
 
     def _watch_load(self) -> None:
         """Pause consuming messages if lood goes above the allowed limit."""
         while not self.shutdown_pending.wait(1):
@@ -361,15 +362,15 @@
         return os.times().elapsed - self._started_at
 
     def _shutdown_timer(self) -> None:
         """Counts down from MAX_WORKER_RUN_TIME. When it reaches zero sutdown
         gracefully.
 
         """
-        remaining = self._max_run_time - self.uptime
+        remaining = cast(float, self._max_run_time) - self.uptime
         if not self.shutdown_pending.wait(remaining):
             logger.warning('Run time reached zero')
             self.shutdown()
 
     def shutdown(self) -> None:
         """Exits after the current task is finished."""
         logger.warning("Shutdown requested")
```

### Comparing `Kuyruk-9.4.0/kuyruk/__main__.py` & `Kuyruk-9.4.1/kuyruk/__main__.py`

 * *Files identical despite different names*

### Comparing `Kuyruk-9.4.0/kuyruk/signals.py` & `Kuyruk-9.4.1/kuyruk/signals.py`

 * *Files identical despite different names*

### Comparing `Kuyruk-9.4.0/kuyruk/config.py` & `Kuyruk-9.4.1/kuyruk/config.py`

 * *Files identical despite different names*

### Comparing `Kuyruk-9.4.0/kuyruk/kuyruk.py` & `Kuyruk-9.4.1/kuyruk/kuyruk.py`

 * *Files identical despite different names*

### Comparing `Kuyruk-9.4.0/kuyruk/result.py` & `Kuyruk-9.4.1/kuyruk/result.py`

 * *Files identical despite different names*

### Comparing `Kuyruk-9.4.0/kuyruk/heartbeat.py` & `Kuyruk-9.4.1/kuyruk/heartbeat.py`

 * *Files identical despite different names*

### Comparing `Kuyruk-9.4.0/kuyruk/task.py` & `Kuyruk-9.4.1/kuyruk/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import platform
 import signal
 import socket
 import logging
 from uuid import uuid1
 from datetime import datetime
 from contextlib import contextmanager
-from typing import Callable, Tuple, Dict, Any, NamedTuple, TYPE_CHECKING, Union, Iterator
+from typing import Callable, Tuple, Dict, Any, NamedTuple, TYPE_CHECKING, Union, Iterator, Optional
 
 import amqp
 from blinker import Signal
 
 from kuyruk import signals, importer
 from kuyruk.exceptions import Timeout
 from kuyruk.result import Result
@@ -23,15 +23,15 @@
 logger = logging.getLogger(__name__)
 
 
 SubTask = NamedTuple("SubTask", [
     ("task", 'Task'),
     ("args", Tuple),
     ("kwargs", Dict[str, Any]),
-    ("host", str),
+    ("host", Optional[str]),
 ])
 
 
 class Task:
     """Calling a :class:`~kuyruk.Task` object serializes the task to JSON
     and sends it to the queue.
 
@@ -59,22 +59,22 @@
         sending this task to queue instead of invoking the function
         without changing the client code.
 
         """
         logger.debug("Task.__call__ args=%r, kwargs=%r", args, kwargs)
         self.send_to_queue(args, kwargs)
 
-    def subtask(self, args: Tuple=(), kwargs: Dict[str, Any]={}, host: str=None) -> SubTask:
+    def subtask(self, args: Tuple=(), kwargs: Dict[str, Any]={}, host: Optional[str]=None) -> SubTask:
         return SubTask(self, args, kwargs, host)
 
     def send_to_queue(
             self,
             args: Tuple=(),
             kwargs: Dict[str, Any]={},
-            host: str=None,
+            host: Optional[str]=None,
             wait_result: Union[int, float]=None,
             message_ttl: Union[int, float]=None,
     ) -> Any:
         """
         Sends a message to the queue.
         A worker will run the task's function when it receives the message.
 
@@ -125,15 +125,15 @@
             ch.queue_declare(queue=queue, durable=True, auto_delete=False)
             ch.basic_publish(msg, exchange="", routing_key=queue)
             self._send_signal(signals.task_postsend, args=args, kwargs=kwargs, description=description)
 
             if wait_result:
                 return result.wait(wait_result)
 
-    def _queue_for_host(self, host: str) -> str:
+    def _queue_for_host(self, host: Optional[str]) -> str:
         if not host:
             return self.queue
         if host == 'localhost':
             host = socket.gethostname()
         return "%s.%s" % (self.queue, host)
 
     def _get_description(self, args: Tuple, kwargs: Dict[str, Any]) -> Dict[str, Any]:
```

