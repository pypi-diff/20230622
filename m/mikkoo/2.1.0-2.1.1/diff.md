# Comparing `tmp/mikkoo-2.1.0.tar.gz` & `tmp/mikkoo-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikkoo-2.1.0.tar", last modified: Thu Jun 22 17:22:21 2023, max compression
+gzip compressed data, was "mikkoo-2.1.1.tar", last modified: Thu Jun 22 18:01:14 2023, max compression
```

## Comparing `mikkoo-2.1.0.tar` & `mikkoo-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:22:21.729352 mikkoo-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     1481 2023-06-22 17:22:20.000000 mikkoo-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    18880 2023-06-22 17:22:21.729352 mikkoo-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17742 2023-06-22 17:22:20.000000 mikkoo-2.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:22:21.729352 mikkoo-2.1.0/mikkoo/
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-22 17:22:20.000000 mikkoo-2.1.0/mikkoo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-22 17:22:20.000000 mikkoo-2.1.0/mikkoo/controller.py
--rw-r--r--   0 root         (0) root         (0)    15839 2023-06-22 17:22:20.000000 mikkoo-2.1.0/mikkoo/mcp.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-22 17:22:20.000000 mikkoo-2.1.0/mikkoo/state.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-06-22 17:22:20.000000 mikkoo-2.1.0/mikkoo/stats.py
--rw-r--r--   0 root         (0) root         (0)    29501 2023-06-22 17:22:20.000000 mikkoo-2.1.0/mikkoo/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:22:21.729352 mikkoo-2.1.0/mikkoo.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18880 2023-06-22 17:22:21.000000 mikkoo-2.1.0/mikkoo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-22 17:22:21.000000 mikkoo-2.1.0/mikkoo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:22:21.000000 mikkoo-2.1.0/mikkoo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 17:22:21.000000 mikkoo-2.1.0/mikkoo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      357 2023-06-22 17:22:21.000000 mikkoo-2.1.0/mikkoo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 17:22:21.000000 mikkoo-2.1.0/mikkoo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:22:21.000000 mikkoo-2.1.0/mikkoo.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     2194 2023-06-22 17:22:21.729352 mikkoo-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-22 17:22:20.000000 mikkoo-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:01:14.930294 mikkoo-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-06-22 18:01:13.000000 mikkoo-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    19008 2023-06-22 18:01:14.930294 mikkoo-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17870 2023-06-22 18:01:13.000000 mikkoo-2.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:01:14.930294 mikkoo-2.1.1/mikkoo/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/controller.py
+-rw-r--r--   0 root         (0) root         (0)    15839 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/mcp.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/state.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/stats.py
+-rw-r--r--   0 root         (0) root         (0)    29525 2023-06-22 18:01:13.000000 mikkoo-2.1.1/mikkoo/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:01:14.930294 mikkoo-2.1.1/mikkoo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19008 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      357 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:01:14.000000 mikkoo-2.1.1/mikkoo.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-06-22 18:01:14.934294 mikkoo-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-22 18:01:13.000000 mikkoo-2.1.1/setup.py
```

### Comparing `mikkoo-2.1.0/LICENSE` & `mikkoo-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.0/PKG-INFO` & `mikkoo-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikkoo
-Version: 2.1.0
+Version: 2.1.1
 Summary: Mikkoo is a PgQ to RabbitMQ Relay
 Home-page: https://github.com/gmr/mikkoo
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gmr/mikkoo/issues
 Project-URL: Documentation, https://mikkoo.readthedocs.io
@@ -336,15 +336,21 @@
 
       workers:
         test:
           confirm: False
           consumer_name: my_consumer
           max_failures: 5
           postgres_url: postgresql://localhost:5432/postgres
-          rabbitmq_url: amqp://localhost:5672/%2f
+          rabbitmq:
+            host: localhost
+            port: 5671
+            username: guest
+            password: guest
+            ssl_options:
+              protocol: 2
           retry_delay: 5
           unregister: False
           wait_duration: 5
 
     Daemon:
       user: mikkoo
       pidfile: /var/run/mikkoo
```

### Comparing `mikkoo-2.1.0/README.rst` & `mikkoo-2.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -305,15 +305,21 @@
 
       workers:
         test:
           confirm: False
           consumer_name: my_consumer
           max_failures: 5
           postgres_url: postgresql://localhost:5432/postgres
-          rabbitmq_url: amqp://localhost:5672/%2f
+          rabbitmq:
+            host: localhost
+            port: 5671
+            username: guest
+            password: guest
+            ssl_options:
+              protocol: 2
           retry_delay: 5
           unregister: False
           wait_duration: 5
 
     Daemon:
       user: mikkoo
       pidfile: /var/run/mikkoo
```

### Comparing `mikkoo-2.1.0/mikkoo/controller.py` & `mikkoo-2.1.1/mikkoo/controller.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.0/mikkoo/mcp.py` & `mikkoo-2.1.1/mikkoo/mcp.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.0/mikkoo/state.py` & `mikkoo-2.1.1/mikkoo/state.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.0/mikkoo/stats.py` & `mikkoo-2.1.1/mikkoo/stats.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.1.0/mikkoo/worker.py` & `mikkoo-2.1.1/mikkoo/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,16 +198,16 @@
 
         """
         return pika.ConnectionParameters(
             self.worker_config['rabbitmq'].get('host', 'localhost'),
             self.worker_config['rabbitmq'].get('port', 5672),
             self.worker_config['rabbitmq'].get('vhost', '/'),
             pika.PlainCredentials(
-                self.worker_config.get('username', 'guest'),
-                self.worker_config.get('password', 'guest')),
+                self.worker_config['rabbitmq'].get('username', 'guest'),
+                self.worker_config['rabbitmq'].get('password', 'guest')),
             ssl_options=self.connection_parameters_ssl_options,
             frame_max=self.worker_config['rabbitmq'].get(
                 'frame_max', spec.FRAME_MAX_SIZE),
             socket_timeout=self.worker_config['rabbitmq'].get(
                 'socket_timeout', 10),
             heartbeat=self.worker_config['rabbitmq'].get(
                 'heartbeat_interval', 300))
```

### Comparing `mikkoo-2.1.0/mikkoo.egg-info/PKG-INFO` & `mikkoo-2.1.1/mikkoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikkoo
-Version: 2.1.0
+Version: 2.1.1
 Summary: Mikkoo is a PgQ to RabbitMQ Relay
 Home-page: https://github.com/gmr/mikkoo
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gmr/mikkoo/issues
 Project-URL: Documentation, https://mikkoo.readthedocs.io
@@ -336,15 +336,21 @@
 
       workers:
         test:
           confirm: False
           consumer_name: my_consumer
           max_failures: 5
           postgres_url: postgresql://localhost:5432/postgres
-          rabbitmq_url: amqp://localhost:5672/%2f
+          rabbitmq:
+            host: localhost
+            port: 5671
+            username: guest
+            password: guest
+            ssl_options:
+              protocol: 2
           retry_delay: 5
           unregister: False
           wait_duration: 5
 
     Daemon:
       user: mikkoo
       pidfile: /var/run/mikkoo
```

### Comparing `mikkoo-2.1.0/setup.cfg` & `mikkoo-2.1.1/setup.cfg`

 * *Files identical despite different names*

