# Comparing `tmp/mikkoo-1.1.2.tar.gz` & `tmp/mikkoo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mikkoo-1.1.2.tar", last modified: Fri Dec 20 14:30:13 2019, max compression
+gzip compressed data, was "mikkoo-2.0.0.tar", last modified: Thu Jan 26 21:24:57 2023, max compression
```

## Comparing `mikkoo-1.1.2.tar` & `mikkoo-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-20 14:30:13.000000 mikkoo-1.1.2/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-20 14:30:13.000000 mikkoo-1.1.2/mikkoo.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17356 2019-12-20 14:30:13.000000 mikkoo-1.1.2/mikkoo.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-20 14:30:13.000000 mikkoo-1.1.2/mikkoo.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-20 14:30:13.000000 mikkoo-1.1.2/mikkoo.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-12-20 14:30:13.000000 mikkoo-1.1.2/mikkoo.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      356 2019-12-20 14:30:13.000000 mikkoo-1.1.2/mikkoo.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      118 2019-12-20 14:30:13.000000 mikkoo-1.1.2/mikkoo.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2019-12-20 14:30:13.000000 mikkoo-1.1.2/mikkoo.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    17356 2019-12-20 14:30:13.000000 mikkoo-1.1.2/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-20 14:30:13.000000 mikkoo-1.1.2/mikkoo/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3845 2019-12-20 14:29:45.000000 mikkoo-1.1.2/mikkoo/state.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1966 2019-12-20 14:29:45.000000 mikkoo-1.1.2/mikkoo/controller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5519 2019-12-20 14:29:45.000000 mikkoo-1.1.2/mikkoo/statsd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27643 2019-12-20 14:29:45.000000 mikkoo-1.1.2/mikkoo/worker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      146 2019-12-20 14:29:45.000000 mikkoo-1.1.2/mikkoo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1841 2019-12-20 14:29:45.000000 mikkoo-1.1.2/mikkoo/stats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16084 2019-12-20 14:29:45.000000 mikkoo-1.1.2/mikkoo/mcp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      215 2019-12-20 14:30:13.000000 mikkoo-1.1.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    13799 2019-12-20 14:29:45.000000 mikkoo-1.1.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1650 2019-12-20 14:29:45.000000 mikkoo-1.1.2/setup.py
+drwxr-xr-x   0 gavinr     (501) staff       (20)        0 2023-01-26 21:24:57.064085 mikkoo-2.0.0/
+-rw-r--r--   0 gavinr     (501) staff       (20)     1481 2023-01-24 16:31:38.000000 mikkoo-2.0.0/LICENSE
+-rw-r--r--   0 gavinr     (501) staff       (20)    14937 2023-01-26 21:24:57.064170 mikkoo-2.0.0/PKG-INFO
+-rw-r--r--   0 gavinr     (501) staff       (20)    13799 2023-01-24 16:31:38.000000 mikkoo-2.0.0/README.rst
+drwxr-xr-x   0 gavinr     (501) staff       (20)        0 2023-01-26 21:24:57.062790 mikkoo-2.0.0/mikkoo/
+-rw-r--r--   0 gavinr     (501) staff       (20)      132 2023-01-26 18:54:43.000000 mikkoo-2.0.0/mikkoo/__init__.py
+-rw-r--r--   0 gavinr     (501) staff       (20)     1996 2023-01-26 18:54:54.000000 mikkoo-2.0.0/mikkoo/controller.py
+-rw-r--r--   0 gavinr     (501) staff       (20)    15839 2023-01-26 18:56:33.000000 mikkoo-2.0.0/mikkoo/mcp.py
+-rw-r--r--   0 gavinr     (501) staff       (20)     3462 2023-01-25 19:30:54.000000 mikkoo-2.0.0/mikkoo/state.py
+-rw-r--r--   0 gavinr     (501) staff       (20)     3172 2023-01-26 18:36:15.000000 mikkoo-2.0.0/mikkoo/stats.py
+-rw-r--r--   0 gavinr     (501) staff       (20)    26515 2023-01-26 18:59:36.000000 mikkoo-2.0.0/mikkoo/worker.py
+drwxr-xr-x   0 gavinr     (501) staff       (20)        0 2023-01-26 21:24:57.063841 mikkoo-2.0.0/mikkoo.egg-info/
+-rw-r--r--   0 gavinr     (501) staff       (20)    14937 2023-01-26 21:24:57.000000 mikkoo-2.0.0/mikkoo.egg-info/PKG-INFO
+-rw-r--r--   0 gavinr     (501) staff       (20)      347 2023-01-26 21:24:57.000000 mikkoo-2.0.0/mikkoo.egg-info/SOURCES.txt
+-rw-r--r--   0 gavinr     (501) staff       (20)        1 2023-01-26 21:24:57.000000 mikkoo-2.0.0/mikkoo.egg-info/dependency_links.txt
+-rw-r--r--   0 gavinr     (501) staff       (20)       50 2023-01-26 21:24:57.000000 mikkoo-2.0.0/mikkoo.egg-info/entry_points.txt
+-rw-r--r--   0 gavinr     (501) staff       (20)      356 2023-01-26 21:24:57.000000 mikkoo-2.0.0/mikkoo.egg-info/requires.txt
+-rw-r--r--   0 gavinr     (501) staff       (20)        7 2023-01-26 21:24:57.000000 mikkoo-2.0.0/mikkoo.egg-info/top_level.txt
+-rw-r--r--   0 gavinr     (501) staff       (20)        1 2023-01-24 16:43:01.000000 mikkoo-2.0.0/mikkoo.egg-info/zip-safe
+-rw-r--r--   0 gavinr     (501) staff       (20)     2193 2023-01-26 21:24:57.064658 mikkoo-2.0.0/setup.cfg
+-rw-r--r--   0 gavinr     (501) staff       (20)       61 2023-01-24 16:41:42.000000 mikkoo-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mikkoo-1.1.2/mikkoo/state.py` & `mikkoo-2.0.0/mikkoo/state.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Base State Tracking Class
 
 """
 import logging
 import time
+import typing
 
 LOGGER = logging.getLogger(__name__)
 
 
-class State(object):
+class State:
     """Class that is to be extended by MCP and process for maintaining the
     internal state of the application.
 
     """
     # State constants
     STATE_INITIALIZING = 0x01
     STATE_CONNECTING = 0x02
@@ -20,144 +21,97 @@
     STATE_ACTIVE = 0x04
     STATE_SLEEPING = 0x05
     STATE_STOP_REQUESTED = 0x06
     STATE_SHUTTING_DOWN = 0x07
     STATE_STOPPED = 0x08
     STATE_RECONNECTING = 0x09
     STATE_BLOCKED = 0x10
+    STATE_CLOSED = 0x11
 
     # For reverse lookup
     STATES = {
         0x01: 'Initializing',
         0x02: 'Connecting',
         0x03: 'Idle',
         0x04: 'Active',
         0x05: 'Sleeping',
         0x06: 'Stop Requested',
         0x07: 'Shutting down',
         0x08: 'Stopped',
         0x09: 'Reconnecting',
-        0x10: 'Blocked'
+        0x10: 'Blocked',
+        0x11: 'Closed'
     }
 
     def __init__(self):
         """Initialize the state of the object"""
         self.state = self.STATE_INITIALIZING
         self.state_start = time.time()
 
-    def set_state(self, new_state):
+    def set_state(self, new_state: int) -> typing.NoReturn:
         """Assign the specified state to this consumer object.
 
-        :param int new_state: The new state of the object
         :raises: ValueError
 
         """
-        # Make sure it's a valid state
         if new_state not in self.STATES:
-            raise ValueError('Invalid state value: %r' % new_state)
-
-        # Set the state
+            raise ValueError(f'Invalid state value: {new_state}')
         LOGGER.debug('State changing from %s to %s', self.STATES[self.state],
                      self.STATES[new_state])
         self.state = new_state
         self.state_start = time.time()
 
     @property
-    def is_blocked(self):
-        """Returns a bool specifying if the process is blocked by RabbitMQ
-
-        :rtype: bool
-
-        """
+    def is_blocked(self) -> bool:
+        """Return True if the process is blocked by RabbitMQ"""
         return self.state == self.STATE_BLOCKED
 
     @property
-    def is_connecting(self):
-        """Returns a bool specifying if the process is currently connecting.
-
-        :rtype: bool
-
-        """
+    def is_connecting(self) -> bool:
+        """Returns True if the process is currently connecting."""
         return self.state == self.STATE_CONNECTING
 
     @property
-    def is_idle(self):
-        """Returns a bool specifying if the process is currently idle.
-
-        :rtype: bool
-
-        """
+    def is_idle(self) -> bool:
+        """Returns a bool specifying if the process is currently idle."""
         return self.state == self.STATE_IDLE
 
     @property
-    def is_reconnecting(self):
-        """Returns a bool specifying if the process is currently reconnecting.
-
-        :rtype: bool
-
-        """
+    def is_reconnecting(self) -> bool:
+        """Returns True if the process is currently reconnecting"""
         return self.state == self.STATE_RECONNECTING
 
     @property
-    def is_running(self):
-        """Returns a bool determining if the process is in a running state or
-        not
-
-        :rtype: bool
-
-        """
+    def is_running(self) -> bool:
+        """Indicates if the process is in a running state"""
         return self.state in [self.STATE_IDLE, self.STATE_ACTIVE,
                               self.STATE_SLEEPING]
 
     @property
-    def is_shutting_down(self):
-        """Designates if the process is shutting down.
-
-        :rtype: bool
-
-        """
+    def is_shutting_down(self) -> bool:
+        """Designates if the process is shutting down."""
         return self.state == self.STATE_SHUTTING_DOWN
 
     @property
-    def is_sleeping(self):
-        """Returns a bool determining if the process is sleeping
-
-        :rtype: bool
-
-        """
+    def is_sleeping(self) -> bool:
+        """Returns a bool determining if the process is sleeping"""
         return self.state == self.STATE_SLEEPING
 
     @property
-    def is_stopped(self):
-        """Returns a bool determining if the process is stopped or stopping
-
-        :rtype: bool
-
-        """
+    def is_stopped(self) -> bool:
+        """Returns a bool determining if the process is stopped or stopping"""
         return self.state == self.STATE_STOPPED
 
     @property
-    def is_waiting_to_shutdown(self):
-        """Designates if the process is waiting to start shutdown
-
-        :rtype: bool
-
-        """
+    def is_waiting_to_shutdown(self) -> bool:
+        """Designates if the process is waiting to start shutdown"""
         return self.state == self.STATE_STOP_REQUESTED
 
     @property
-    def state_description(self):
-        """Return the string description of our running state.
-
-        :rtype: str
-
-        """
+    def state_description(self) -> str:
+        """Return the string description of our running state."""
         return self.STATES[self.state]
 
     @property
-    def time_in_state(self):
-        """Return the time that has been spent in the current state.
-
-        :rtype: float
-
-        """
+    def time_in_state(self) -> float:
+        """Return the time that has been spent in the current state."""
         return time.time() - self.state_start
```

### Comparing `mikkoo-1.1.2/mikkoo/controller.py` & `mikkoo-2.0.0/mikkoo/controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 """
-Mikkoo
-======
 PgQ -> RabbitMQ Relay
 
 """
 import logging
 import signal
+import typing
 
 import helper
-from helper import parser
+from helper import controller, parser
 
 from mikkoo import mcp
 
 DESCRIPTION = 'Mikkoo is a PgQ to RabbitMQ Relay'
 LOGGER = logging.getLogger(__name__)
 
 
-class Controller(helper.Controller):
+class Controller(controller.Controller):
     """The Mikkoo controller application that invokes the MCP and handles all
-    of the OS level concerns.
+    OS level concerns.
 
     """
     def __init__(self, *args, **kwargs):
         super(Controller, self).__init__(*args, **kwargs)
         self._mcp = None
 
-    def _master_control_program(self):
-        """Return an instance of the MasterControlProgram.
-
-        :rtype: rejected.mcp.MasterControlProgram
-
-        """
+    def _master_control_program(self) -> mcp.MasterControlProgram:
+        """Return an instance of the MasterControlProgram"""
         return mcp.MasterControlProgram(self.config)
 
-    def stop(self):
+    def stop(self) -> typing.NoReturn:
         """Shutdown the MCP and child processes cleanly"""
         LOGGER.info('Shutting down controller')
         self.set_state(self.STATE_STOP_REQUESTED)
 
         # Clear out the timer
         signal.setitimer(signal.ITIMER_PROF, 0, 0)
 
@@ -54,23 +49,23 @@
             self._mcp.stop_processes()
             del self._mcp
 
         # Change our state
         self._stopped()
         LOGGER.info('Shutdown complete')
 
-    def run(self):
-        """Run the rejected Application"""
+    def run(self) -> typing.NoReturn:
+        """Run the Mikkoo Application"""
         self.setup()
         self._mcp = self._master_control_program()
         try:
             self._mcp.run()
         except KeyboardInterrupt:
             LOGGER.info('Caught CTRL-C, shutting down')
         if self.is_running:
             self.stop()
 
 
-def main():
+def main() -> typing.NoReturn:
     """Called when invoking the command line script."""
     parser.description(DESCRIPTION)
     helper.start(Controller)
```

### Comparing `mikkoo-1.1.2/mikkoo/worker.py` & `mikkoo-2.0.0/mikkoo/worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """
 Mikkoo Worker Process
 =====================
 Connects to Postgres and processes PgQ batches, publishing the events in
 the batch to RabbitMQ.
 
 """
-import contextlib
+import asyncio
 import copy
+import datetime
 import json
 import logging
 import multiprocessing
+import os
 import signal
 import socket
 import sys
 import time
+import typing
 import uuid
 
 import arrow
-from tornado import concurrent, ioloop
+import helper.config
 import pika
-from pika.adapters import tornado_connection
-import queries
-import simpleflake
+import pika.channel
+import psycopg
+from pika import connection, exceptions, frame, spec
+from pika.adapters import asyncio_connection
+from psycopg import rows, sql
+from uuid_extensions import uuid7
 
 try:
-    import raven
+    import sentry_sdk
 except ImportError:
-    raven = None
+    sentry_sdk = None
 
-from mikkoo import __version__
-from mikkoo import state
-from mikkoo import stats
+from mikkoo import __version__, state, stats
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Process(multiprocessing.Process, state.State):
 
     AMQP_APP_ID = 'mikkoo/%s' % __version__
@@ -67,414 +71,384 @@
                  target=None,
                  name=None,
                  args=(),
                  kwargs=None):
         if kwargs is None:
             kwargs = {}
         super(Process, self).__init__(group, target, name, args, kwargs)
-        self.channel = None
-        self.connection = None
         self.config = kwargs['config']
-
         self.confirm = kwargs['config']['worker'].get('confirm', False)
         self.consumer_name = kwargs['config']['worker'].get(
             'consumer_name', self.DEFAULT_CONSUMER_NAME)
-        self.current_batch = None
-        self.current_event = None
-        self.event_list = None
-        self.event_processed = None
-        self.ioloop = None
-        self.last_stats_time = None
+        self.current_batch: typing.Optional[int] = None
+        self.current_event: typing.Optional[dict] = None
+        self.event_list: typing.Optional[typing.List[dict]] = None
+        self.event_processed: typing.Optional[asyncio.Future] = None
+        self.ioloop: typing.Optional[asyncio.AbstractEventLoop] = None
+        self.last_stats_time: typing.Optional[float] = None
         self.maximum_failures = kwargs['config']['worker'].get(
             'max_failures', self.DEFAULT_MAX_FAILURES)
-        self.prepend_path = None
+        self.postgres: typing.Optional[psycopg.AsyncConnection] = None
+        self.rabbitmq: typing.Optional[
+            asyncio_connection.AsyncioConnection] = None
+        self.rabbitmq_channel: typing.Optional[pika.channel.Channel] = None
         self.retry_interval = kwargs['config']['worker'].get(
             'retry_interval', self.DEFAULT_RETRY_INTERVAL)
-        self.sentry_client = None
-        self.session = None
         self.state = self.STATE_INITIALIZING
         self.state_start = time.time()
-        self.stats = stats.Stats(self.name, kwargs['worker_name'],
-                                 kwargs['config'].get('statsd', {}),
-                                 self.on_statsd_failure)
+        self.stats = stats.Stats(
+            self.name,
+            kwargs['worker_name'],
+            kwargs['config'].get('statsd', {}))
+        self.stats_queue: multiprocessing.Queue = kwargs['stats_queue']
         self.wait_duration = kwargs['config']['worker'].get(
             'wait_duration', self.DEFAULT_WAIT_DURATION)
         self.worker_config = kwargs['config']['worker']
         self.worker_name = kwargs['worker_name']
 
-        if raven and 'sentry_dsn' in self.config:
-            self.sentry_client = raven.Client(
-                self.config['sentry_dsn'], **{
-                    'include_paths': ['arrow',
-                                      'mikkoo',
-                                      'pika',
-                                      'psycopg2',
-                                      'queries',
-                                      'simpleflake',
-                                      'tornado']})
-            self.set_sentry_context('worker', self.name)
+        if sentry_sdk and 'sentry_dsn' in self.config:
+            sentry_sdk.init(
+                self.config['sentry_dsn'],
+                release=__version__,
+                environment=os.getenv('ENVIRONMENT', 'unknown'),
+                in_app_include=['arrow',
+                                'mikkoo',
+                                'pika',
+                                'psycopg'])
+            sentry_sdk.set_context('mikkoo', {'worker': self.name})
 
         # Override ACTIVE with PROCESSING
         self.STATES[0x04] = 'Processing'
 
-    def connect_to_postgres(self):
+    async def connect_to_postgres(self) -> bool:
         """Connects to Postgres, shutting down the worker on failure"""
         LOGGER.debug('Connecting to Postgres')
         try:
-            self.session = queries.Session(
-                self.worker_config.get('postgres_url'), pool_max_size=1)
-        except queries.OperationalError as error:
+            self.postgres = await psycopg.AsyncConnection.connect(
+                self.worker_config.get('postgres_url'),
+                autocommit=True)
+        except psycopg.OperationalError as error:
             self.send_exception_to_sentry()
             LOGGER.error('Error connecting to Postgres: %s', error)
             return False
         return True
 
-    def callproc(self, name, *args):
+    def build_sql(self, proc_name: str, *args) -> str:
+        return sql.SQL('SELECT * FROM {proc_name}({values})'.format(
+            proc_name=proc_name,
+            values=','.join('%s' for _a in range(0, len(args))))).as_string(
+                self.postgres)
+
+    async def callproc(self, proc_name: str, *args) -> typing.Sequence[dict]:
         """Call the stored procedure in Postgres with the specified
         arguments.
 
-        :param str name: The stored procedure name
-        :param list args: The list of arguments to pass in to the stored proc
-        :rtype: :class:`~queries.Result`
-
         """
-        self.set_sentry_context('callproc', name)
-        LOGGER.debug('Executing %s with %r', name, args)
-        with self.statsd_track_duration('db.{0}.query_time'.format(name)):
-            try:
-                return self.session.callproc(name, args or [])
-            except queries.InternalError as error:
-                self.send_exception_to_sentry()
-                self.log_db_error(name, error)
-                raise PgQError(str(error))
-            except queries.Error as error:
-                self.send_exception_to_sentry()
-                self.log_db_error(name, error)
-
-    def log_db_error(self, name, error):
-        """Log database errors and increment the statsd counter
-
-        :param str name: The stored procedure name
-        :param error: The exception
-        :type error: :class:`~queries.Error`
+        sentry_sdk.set_context('mikkoo', {'function': proc_name})
+        with self.stats.track_duration(f'db.{proc_name}.query_time'):
+            async with self.postgres.cursor(
+                    row_factory=rows.dict_row) as cursor:
+                try:
+                    await cursor.execute(
+                        self.build_sql(proc_name, *args), args or [])
+                    return await cursor.fetchall()
+                except psycopg.InternalError as error:
+                    self.send_exception_to_sentry()
+                    self.log_db_error(proc_name, error)
+                    raise PgQError(str(error))
+                except psycopg.Error as error:
+                    self.send_exception_to_sentry()
+                    self.log_db_error(proc_name, error)
 
-        """
+    def log_db_error(self, name: str, error: Exception) -> typing.NoReturn:
+        """Log database errors and increment the stats counter"""
         LOGGER.error('Error executing %s.callproc: (%s) %s', name,
                      error.__class__.__name__, error)
-        self.statsd_incr('db.{0}.error.{1}'.format(name, str(error)))
+        self.stats.incr('db.{0}.error.{1}'.format(name, str(error)))
 
     def connect_to_rabbitmq(self):
         """Connect to RabbitMQ returning the connection handle."""
         self.set_state(self.STATE_CONNECTING)
-        params = pika.URLParameters(self.worker_config.get('rabbitmq_url'))
-        LOGGER.debug('Connecting to %s:%i:%s as %s',
-                     params.host, params.port, params.virtual_host,
-                     params.credentials.username)
-        return tornado_connection.TornadoConnection(
-            params, self.on_connect_open, self.on_connect_failed,
-            self.on_closed, False, self.ioloop)
-
-    def on_connect_failed(self, *args, **kwargs):
-        """Connection to RabbitMQ failed, so shut things down.
-
-        :param list args: Positional arguments
-        :param dict kwargs: Keyword arguments
-
-        """
-        LOGGER.critical('Could not connect to RabbitMQ: %r', (args, kwargs))
-        self.statsd_incr('amqp.connection_failed')
-        self.on_ready_to_stop()
-
-    def on_connect_open(self, conn):
+        return asyncio_connection.AsyncioConnection(
+            pika.URLParameters(self.worker_config.get('rabbitmq_url')),
+            on_open_callback=self.on_rabbitmq_open,
+            on_open_error_callback=self.on_rabbitmq_open_error,
+            on_close_callback=self.on_rabbitmq_closed)
+
+    def on_rabbitmq_open(self,
+                         conn: asyncio_connection.AsyncioConnection) \
+            -> typing.NoReturn:
         """This method is called by pika once the connection to RabbitMQ has
         been established. It passes the handle to the connection object in
         case we need it, but in this case, we'll just mark it unused.
 
-        :type conn: pika.adapters.tornado_connection.TornadoConnection
-
         """
         LOGGER.info('Connection to RabbitMQ established')
-        self.statsd_incr('amqp.connection_opened')
-        self.connection = conn
-        conn.add_on_connection_blocked_callback(self.on_connection_blocked)
-        conn.add_on_connection_unblocked_callback(self.on_connection_unblocked)
-        self.open_channel()
+        self.stats.incr('amqp.connection_opened')
+        self.rabbitmq = conn
+
+        try:
+            self.rabbitmq.channel(
+                on_open_callback=self.on_rabbitmq_channel_open)
+        except exceptions.ConnectionClosed as err:
+            LOGGER.warning('Channel open on closed connection')
+            self.on_rabbitmq_closed(self.rabbitmq, err)
+            return
 
-    def on_connection_blocked(self, _frame):
+        self.rabbitmq.add_on_connection_blocked_callback(
+            self.on_rabbitmq_blocked)
+        self.rabbitmq.add_on_connection_unblocked_callback(
+            self.on_rabbitmq_unblocked)
+
+    def on_rabbitmq_open_error(self,
+                               _c: connection.Connection,
+                               exc: typing.Union[str, Exception]) -> None:
+        """Connection to RabbitMQ failed, so shut things down."""
+        LOGGER.critical('Could not connect to RabbitMQ: %r', exc)
+        self.stats.incr('amqp.connection_failed')
+        self.on_ready_to_stop()
+
+    def on_rabbitmq_blocked(self,
+                            _c: connection.Connection,
+                            _f: frame.Method) -> typing.NoReturn:
         """Invoked when the RabbitMQ connection has notified us that it is
         blocking publishing.
 
-        :type _frame: :class:`pika.spec.Connection.Blocked`
-
         """
         LOGGER.warning('RabbitMQ is blocking the connection')
-        self.statsd_incr('amqp.connection_blocked')
+        self.stats.incr('amqp.connection_blocked')
         self.set_state(self.STATE_BLOCKED)
 
-    def on_connection_unblocked(self, _frame):
-        """Invoked when the RabbitMQ connection has notified us that it
+    def on_rabbitmq_unblocked(self,
+                              _c: connection.Connection,
+                              _f: frame.Method) -> typing.NoReturn:
+        """Invoked when the RabbitMQ connection has notified us that
         publishing is no longer unblocked.
 
-        :type _frame: :class:`pika.spec.Connection.Unblocked`
-
         """
         LOGGER.info('RabbitMQ is no longer blocking the connection')
-        self.statsd_incr('amqp.connection_unblocked')
-        # If we were blocked while processing, resume
+        self.stats.incr('amqp.connection_unblocked')
         if self.event_list:
             LOGGER.debug('Resuming the processing of %i events',
                          len(self.event_list))
             self.set_state(self.STATE_PROCESSING)
-            self.ioloop.add_callback(self.process_event)
+            self.async_call_soon(self.process_event)
         else:
             self.set_state(self.STATE_IDLE)
-            self.ioloop.add_callback(self.process_batch)
+            self.async_call_soon(self.process_batch)
 
-    def on_closed(self, _unused, code, text):
+    def on_rabbitmq_closed(self,
+                           _conn: asyncio_connection.AsyncioConnection,
+                           error: Exception) -> typing.NoReturn:
         """This method is invoked by pika when the connection to RabbitMQ is
         closed unexpectedly. Shutdown if not already doing so.
 
-        :param pika.connection.Connection _unused: The closed connection
-        :param int code: The AMQP reply code
-        :param str text: The AMQP reply text
-
         """
-        LOGGER.critical('Connection from RabbitMQ closed in state %s (%s, %s)',
-                        self.state_description, code, text)
-        self.channel = None
-        self.statsd_incr('amqp.connection_closed')
+        LOGGER.critical('Connection from RabbitMQ closed in state %s (%)',
+                        self.state_description, error)
+        self.set_state(self.STATE_CLOSED)
+        self.rabbitmq_channel = None
+        self.stats.incr('amqp.connection_closed')
         if self.is_shutting_down or self.is_waiting_to_shutdown:
             self.on_ready_to_stop()
         else:
             LOGGER.info('Reconnecting to RabbitMQ')
-            self.ioloop.add_callback(self.connect_to_rabbitmq)
+            self.ioloop.call_soon(self.connect_to_rabbitmq)
 
-    def open_channel(self):
+    def open_rabbitmq_channel(self):
         """Open a channel on the existing open connection to RabbitMQ"""
         LOGGER.debug('Opening a new channel')
-        self.connection.channel(self.on_channel_open)
+        self.rabbitmq.channel(on_open_callback=self.on_rabbitmq_channel_open)
 
-    def on_channel_open(self, channel):
+    def on_rabbitmq_channel_open(self, channel: pika.channel.Channel) \
+            -> typing.NoReturn:
         """This method is invoked by pika when the channel has been opened. It
-        will change the state to IDLE, add the callbacks and setup the channel
+        will change the state to IDLE, add the callbacks and set up the channel
         to start consuming.
 
-        :param pika.channel.Channel channel: The channel object
-
         """
         LOGGER.debug('Channel %i opened', channel.channel_number)
-        self.statsd_incr('amqp.channel_opened')
-        self.channel = channel
-        self.channel.add_on_close_callback(self.on_channel_closed)
+        self.stats.incr('amqp.channel_opened')
+        self.rabbitmq_channel = channel
+        self.rabbitmq_channel.add_on_close_callback(
+            self.on_rabbitmq_channel_closed)
         if self.confirm:
             LOGGER.info('Enabling publisher confirmations')
-            self.channel.add_on_return_callback(self.on_publish_return)
-            self.channel.confirm_delivery(self.on_publish_confirm)
+            self.rabbitmq_channel.add_on_return_callback(
+                self.on_rabbitmq_publish_return)
+            self.rabbitmq_channel.confirm_delivery(
+                self.on_rabbitmq_publish_confirm)
 
         # Schedule the processing of the first batch if it's not reopening
         if not self.is_reconnecting:
             self.set_state(self.STATE_IDLE)
-            self.ioloop.add_callback(self.process_batch)
+            self.async_call_soon(self.process_batch)
 
-    def on_channel_closed(self, channel, reply_code, reply_text):
+    def on_rabbitmq_channel_closed(self,
+                                   channel: pika.channel.Channel,
+                                   error: Exception) -> typing.NoReturn:
         """Invoked by pika when RabbitMQ unexpectedly closes the channel.
         Channels are usually closed if you attempt to do something that
         violates the protocol, such as re-declare an exchange or queue with
         different parameters. In this case, we'll close the connection
-        to shutdown the object.
-
-        :param pika.channel.Channel channel: The AMQP Channel
-        :param int reply_code: The AMQP reply code
-        :param str reply_text: The AMQP reply text
+        to shut down the object.
 
         """
-        LOGGER.warning('Channel %i closed: (%s) %s',
-                       channel.channel_number, reply_code, reply_text)
-        self.statsd_incr('amqp.channel_closed')
-        if concurrent.is_future(self.event_processed):
+        LOGGER.warning('Channel %i closed: %s',
+                       channel.channel_number, error)
+        self.stats.incr('amqp.channel_closed')
+        self.rabbitmq_channel = None
+        if self.event_processed:
             self.set_state(self.STATE_RECONNECTING)
+            self.open_rabbitmq_channel()
+        else:
+            self.on_ready_to_stop()
 
-            def on_open(new_channel):
-                self.on_channel_open(new_channel)
-                self.set_state(self.STATE_PROCESSING)
-                exc = EventError(self.current_event, reply_text)
-                self.event_processed.set_exception(exc)
+    def on_rabbitmq_publish_confirm(self,
+                                    _f: pika.frame.Method) -> typing.NoReturn:
+        """Invoked by pika when a delivery confirmation is received."""
+        if self.event_processed and self.current_event:
+            LOGGER.debug('Event %s confirmed', self.current_event['ev_id'])
+            self.stats.incr('amqp.publisher_confirm')
+            self.event_processed.set_result(True)
 
-            return self.connection.channel(on_open)
+    def on_rabbitmq_publish_return(self,
+                                   _c: pika.channel.Channel,
+                                   method: spec.Basic.Return,
+                                   _p: spec.BasicProperties,
+                                   _b: bytes) -> typing.NoReturn:
+        """Invoked by pika when a delivery failure is received. Setting the
+        current confirmation future exception to a
+        :class:`mikkoo.worker.EventError`.
 
-        del self.channel
-        self.on_ready_to_stop()
+        """
+        LOGGER.debug('Event %s was returned as (%s) %s from RabbitMQ',
+                     self.current_event['ev_id'], method.reply_code,
+                     method.reply_text)
+        self.stats.incr('amqp.message_returned')
+        self.event_processed.set_exception(
+            EventError(self.current_event, method.reply_text))
 
-    def process_batch(self):
+    async def process_batch(self):
         """Query PgQ for a batch and process it, scheduling the next execution
         of itself with the IOLoop.
 
         """
         if not self.is_idle:
             LOGGER.warning('Process batch invoked while %s',
                            self.state_description)
             return
 
         self.set_state(self.STATE_PROCESSING)
         try:
-            batch = self.callproc('pgq.next_batch', self.worker_name,
-                                  self.consumer_name).as_dict()
+            batch = await self.callproc(
+                'pgq.next_batch', self.worker_name, self.consumer_name)
         except PgQError:
             batch = {}
 
-        if batch.get('next_batch') is None:
-            self.statsd_incr('empty_queue')
+        if batch and batch[0].get('next_batch') is None:
+            self.stats.incr('empty_queue')
             LOGGER.debug('Sleeping for %.2f seconds', self.wait_duration)
             self.set_state(self.STATE_IDLE)
-            self.statsd_add_timing('sleep', self.wait_duration)
-            self.ioloop.add_timeout(self.ioloop.time() + self.wait_duration,
-                                    self.process_batch)
+            self.stats.add_timing('sleep', self.wait_duration)
+            self.ioloop.call_later(
+                self.wait_duration,
+                lambda: asyncio.ensure_future(self.process_batch()))
             return
 
-        self.current_batch = batch['next_batch']
+        self.current_batch = batch[0]['next_batch']
+        LOGGER.debug('Grabbing events for %s', self.current_batch)
 
-        # Grab all of the events in the batch and convert the result to a list
         try:
-            result = self.callproc('pgq.get_batch_events', self.current_batch)
+            self.event_list = await self.callproc(
+                'pgq.get_batch_events', self.current_batch)
         except PgQError as error:
             LOGGER.error('Error getting batch: %s', error)
             self.set_state(self.STATE_IDLE)
-            return self.ioloop.add_callback(self.process_batch)
-
-        LOGGER.debug('Processing %i events', result.count())
-        self.event_list = [dict(row) for row in result]
-
-        # Start the processing of the event list
-        self.ioloop.add_callback(self.process_event)
+            return self.async_call_soon(self.process_batch)
+        LOGGER.debug('Received %i rows to process', len(self.event_list))
+        self.async_call_soon(self.process_event)
 
     @property
-    def is_processing(self):
-        """Returns a bool specifying if the consumer is currently processing
-
-        :rtype: bool
-
-        """
+    def is_processing(self) -> bool:
+        """Returns a bool specifying if the consumer is currently processing"""
         return self.state in [self.STATE_PROCESSING, self.STATE_STOP_REQUESTED]
 
-    def on_batch_complete(self):
+    async def on_batch_complete(self):
         LOGGER.debug('Batch %s complete', self.current_batch)
-        self.callproc('pgq.finish_batch', self.current_batch)
+        await self.callproc('pgq.finish_batch', self.current_batch)
         self.stats.incr(self.BATCHES)
         self.current_batch = None
         if self.is_waiting_to_shutdown:
             return self.on_ready_to_stop()
         self.set_state(self.STATE_IDLE)
-        self.ioloop.add_callback(self.process_batch)
+        self.async_call_soon(self.process_batch)
 
     def process_event(self):
         if not self.event_list:
             return self.on_batch_complete()
         elif not self.is_processing:
             LOGGER.debug('Processing of %i events paused due to %s state',
                          len(self.event_list), self.state_description)
             return
 
-        self.event_processed = concurrent.TracebackFuture()
+        self.event_processed = asyncio.Future()
         self.event_processed.add_done_callback(self.on_event_processed)
         self.current_event = event = self.event_list.pop(0)
 
-        self.statsd_incr('publish.{0}.{1}'.format(event['ev_extra1'],
-                                                  event['ev_type']))
+        self.stats.incr(f'publish.{event["ev_extra1"]}.{event["ev_type"]}')
         try:
-            self.channel.basic_publish(event['ev_extra1'],
-                                       event['ev_type'],
-                                       event['ev_data'],
-                                       self.build_properties_kwargs(event),
-                                       mandatory=True)
+            self.rabbitmq_channel.basic_publish(
+                event['ev_extra1'], event['ev_type'], event['ev_data'],
+                self.build_properties_kwargs(event), mandatory=True)
         except TypeError as error:
             self.send_exception_to_sentry()
-            message = 'Error building kwargs for the event: {0}'.format(error)
-            self.event_processed.set_exception(EventError(event, message))
+            self.event_processed.set_exception(
+                EventError(
+                    event, f'Error building kwargs for the event: {error}'))
         if not self.confirm:
             self.event_processed.set_result(True)
 
-    def build_properties_kwargs(self, event):
+    def build_properties_kwargs(self, event: dict) -> spec.BasicProperties:
         """Build the :class:`~pika.BasicProperties` object to use when
         publishing the AMQP message
 
-        :param dict event: The event to build kwargs for
-        :rtype: :class:`~pika.BasicProperties`
-
         """
         kwargs = {
             'app_id': self.AMQP_APP_ID,
             'content_type': event['ev_extra2'],
             'correlation_id': str(uuid.uuid4()),
             'timestamp': self.get_timestamp(event['ev_time'])
         }
         if event['ev_extra4']:
             kwargs['headers'] = json.loads(event['ev_extra4'].encode('utf-8'))
         if event['ev_extra3']:
             try:
                 properties = json.loads(event['ev_extra3'])
             except ValueError:
-                LOGGER.warning('Failed to decode properties from ev_extra3: %r',
+                LOGGER.warning('Failed to decode ev_extra3: %r',
                                event['ev_extra3'])
                 properties = {}
             for key in properties:
                 if key.encode('ascii') in self.VALID_PROPERTIES:
                     kwargs[key.encode('ascii')] = properties[key]
         if 'headers' not in kwargs:
             kwargs['headers'] = {}
 
         kwargs['headers'].setdefault('origin', socket.getfqdn())
-        kwargs['headers'].setdefault('sequence', simpleflake.simpleflake())
+        kwargs['headers'].setdefault('sequence', str(uuid7()))
         kwargs['headers'].setdefault('txid', event['ev_txid'])
         kwargs['headers'].setdefault(
             'timestamp', arrow.get(event['ev_time']).to('utc').isoformat())
         return pika.BasicProperties(**kwargs)
 
     @staticmethod
-    def get_timestamp(value):
-        """Return the timestamp in UTC
-
-        :param datetime.datetime value: The event time
-        :rtype: int
-
-        """
-        return arrow.get(value).to('utc').timestamp
-
-    def on_publish_confirm(self, _frame):
-        """Invoked by pika when a delivery confirmation is received.
-
-        :param _frame: The confirmation frame
-        :type _frame: :class:`pika.spec.Basic.Ack`
-
-        """
-        # Acks occur event on a basic_return.
-        if self.event_processed and self.current_event:
-            LOGGER.debug('Event %s confirmed', self.current_event['ev_id'])
-            self.statsd_incr('amqp.publisher_confirm')
-            self.event_processed.set_result(True)
-
-    def on_publish_return(self, _channel, method, _properties, _body):
-        """Invoked by pika when a delivery failure is received. Setting the
-        current confirmation future exception to a
-        :class:`mikkoo.worker.EventError`.
-
-        :param _channel: The channel the message was returned on
-        :type _channel: :class:`~pika.channel.Channel`
-        :param method: The ``Basic.Return`` method frame
-        :type method: :class:`~pika.spec.Basic.Return`
-        :param _properties: The message properties of the returned message
-        :type _properties: :class:`~pika.spec.Basic.Properties`
-        :param bytes _body: The message body that was returned
-
-        """
-        LOGGER.debug('Event %s was returned as (%s) %s from RabbitMQ',
-                     self.current_event['ev_id'], method.reply_code,
-                     method.reply_text)
-        self.statsd_incr('amqp.message_returned')
-        self.event_processed.set_exception(EventError(self.current_event,
-                                                      method.reply_text))
+    def get_timestamp(value: datetime.datetime) -> int:
+        """Return the timestamp in UTC"""
+        return int(arrow.get(value).to('utc').timestamp())
 
     def on_event_processed(self, future):
         """Invoked once the message is published or an exception is raised
         when processing the message.
 
         :param future: Future representing the disposition of the processing
         :type future: :class:`~tornado.concurrent.TracebackFuture`
@@ -485,234 +459,202 @@
             self.stats.incr(self.ERROR)
             LOGGER.error(str(exc))
             if exc.event.get('ev_retry', 0) >= self.maximum_failures:
                 LOGGER.warning('Discarding event %s: %r',
                                exc.event['ev_id'],
                                exc.event)
             else:
-                self.callproc('pgq.event_retry', self.current_batch,
-                              exc.event['ev_id'], self.retry_interval)
+                self.async_call_soon(
+                    self.on_event_error,  self.current_batch,
+                    exc.event['ev_id'])
         else:
             self.stats.incr(self.PROCESSED)
         self.current_event = None
-        self.ioloop.add_callback(self.process_event)
+        self.async_call_soon(self.process_event)
+
+    async def on_event_error(self, batch, ev_id):
+        LOGGER.debug('on_event_error %s %s', batch, ev_id)
+        await self.callproc(
+            'pgq.event_retry', batch, ev_id, self.retry_interval)
 
     def run(self):
         """Entry-point that is automatically invoked as part of the
         :class:`~multiprocess.Process` startup. The process will block here
         until it is shutdown.
 
         Processing of PgQ batches is started in
         :meth:`~mikkoo.worker.Process.on_channel_open`.
 
         """
-        self.setup()
+        self.set_state(self.STATE_INITIALIZING)
+        self.ioloop = asyncio.get_event_loop()
+        self.ioloop.run_until_complete(self.setup())
         if not self.is_stopped:
             LOGGER.info('%s worker started', self.name)
             try:
-                self.ioloop.start()
+                self.ioloop.run_forever()
             except KeyboardInterrupt:
                 LOGGER.warning('CTRL-C while waiting for clean shutdown')
-            except Exception:
-                self.send_exception_to_sentry()
+            finally:
+                self.ioloop.run_until_complete(
+                    self.ioloop.shutdown_asyncgens())
+                self.ioloop.close()
 
-    def setup(self):
-        """Ensure that all the things that are required are setup when the
+    async def setup(self) -> typing.NoReturn:
+        """Ensure that all the things that are required are set up when the
         Process is started.
 
         """
+        helper.config.LoggingConfig(self.config['logging']).configure()
 
-        if not self.connect_to_postgres():
+        if not await self.connect_to_postgres():
             LOGGER.info('Could not connect to Postgres, stopping')
             self.set_state(self.STATE_STOPPED)
             return
 
+        await self.stats.start()
+
         self.stats[self.ERROR] = 0
         self.stats[self.PROCESSED] = 0
         self.stats[self.PENDING] = 0
 
-        self.create_queue()
-        self.register_consumer()
+        await self.create_queue()
+        await self.register_consumer()
 
         self.setup_signal_handlers()
-        self.ioloop = ioloop.IOLoop.current()
-
-        self.ioloop.add_callback(self.connect_to_rabbitmq)
-
-    def create_queue(self):
-        """Create the PgQ for the worker.
+        self.connect_to_rabbitmq()
 
-        :rtype: :class:`~queries.Result`
-
-        """
+    async def create_queue(self) -> typing.NoReturn:
+        """Create the PgQ for the worker."""
         LOGGER.debug('Fetching PgQ information')
-        result = self.callproc('pgq.create_queue', self.worker_name)
+        result = await self.callproc('pgq.create_queue', self.worker_name)
         if not result:
             LOGGER.debug('Queue already exists')
 
-    def register_consumer(self):
+    async def register_consumer(self) -> typing.NoReturn:
         """Register the consumer. If registration fails, shutdown the worker.
 
         """
-        results = self.callproc('pgq.register_consumer',
-                                self.worker_name, self.consumer_name)
-        if results is None:
+        results = await self.callproc(
+            'pgq.register_consumer', self.worker_name, self.consumer_name)
+        if not results:
             LOGGER.critical('Registration of the consumer failed')
-            self.stop()
+            self.async_call_soon(self.stop)
 
-        elif not results.as_dict()['register_consumer']:
+        elif not results[0]['register_consumer']:
             LOGGER.debug('Consumer is already registered')
 
-    def unregister_consumer(self):
+    async def unregister_consumer(self) -> typing.NoReturn:
         """Unregister the consumer with PgQ"""
-        self.callproc('pgq.unregister_consumer',
-                      self.worker_name, self.consumer_name)
+        await self.callproc(
+            'pgq.unregister_consumer', self.worker_name, self.consumer_name)
 
-    def on_ready_to_stop(self):
+    def on_ready_to_stop(self) -> typing.NoReturn:
         """Invoked when the worker is shutting down and is no longer processing
         a PgQ batch.
 
         """
         # Set the state to shutting down if it wasn't set as that during loop
         self.set_state(self.STATE_SHUTTING_DOWN)
 
         # Reset any signal handlers
-        signal.signal(signal.SIGABRT, signal.SIG_IGN)
-        signal.signal(signal.SIGINT, signal.SIG_IGN)
-        signal.signal(signal.SIGPROF, signal.SIG_IGN)
-        signal.signal(signal.SIGTERM, signal.SIG_IGN)
+        self.ioloop.remove_signal_handler(signal.SIGABRT)
+        self.ioloop.remove_signal_handler(signal.SIGPROF)
 
         # Unregister the consumer from PgQ
         if self.worker_config.get('unregister', True):
             self.unregister_consumer()
 
         # If the connection is still around, close it
-        if self.connection and self.connection.is_open:
+        if self.rabbitmq and self.rabbitmq.is_open:
             LOGGER.debug('Closing connection to RabbitMQ')
-            self.connection.close()
+            self.rabbitmq.close()
 
         # Stop the IOLoop
         if self.ioloop:
             LOGGER.debug('Stopping IOLoop')
             self.ioloop.stop()
 
         # Note that shutdown is complete and set the state accordingly
         self.set_state(self.STATE_STOPPED)
         LOGGER.debug('Shutdown complete')
 
     def setup_signal_handlers(self):
-        """Setup the stats and stop signal handlers."""
+        """Set up the stats and stop signal handlers."""
         signal.signal(signal.SIGINT, signal.SIG_IGN)
         signal.signal(signal.SIGTERM, signal.SIG_IGN)
-        signal.signal(signal.SIGPROF, self.on_sigprof)
-        signal.signal(signal.SIGABRT, self.stop)
-        signal.siginterrupt(signal.SIGPROF, False)
-        signal.siginterrupt(signal.SIGABRT, False)
+
+        self.ioloop.add_signal_handler(signal.SIGABRT, self.on_sigabrt)
+        self.ioloop.add_signal_handler(signal.SIGPROF, self.on_sigprof)
         LOGGER.debug('Signal handlers setup')
 
-    def on_sigprof(self, _unused_signum, _unused_frame):
+    def async_call_soon(self, func: typing.Callable, *args) -> typing.NoReturn:
+        self.ioloop.call_soon(asyncio.ensure_future(func(*args)))
+
+    def on_sigabrt(self) -> typing.NoReturn:
+        """Invoked when the MCP sends a SIGABRT to shut down the worker"""
+        LOGGER.debug('on_sigabrt when %s', self.state_description)
+        self.async_call_soon(self.stop)
+
+    def on_sigprof(self) -> typing.NoReturn:
         """Called when SIGPROF is sent to the process, will dump the stats, in
         future versions, queue them for the master process to get data.
 
-        :param int _unused_signum: The signal number
-        :param frame _unused_frame: The python frame the signal was received at
-
         """
         LOGGER.debug('on_sigprof')
         signal.siginterrupt(signal.SIGPROF, False)
-        self.ioloop.add_callback_from_signal(self.submit_stats_report)
-
-    def on_statsd_failure(self):
-        self.set_state(self.STATE_STOP_REQUESTED)
+        self.async_call_soon(self.submit_stats_report)
 
-    def submit_stats_report(self):
+    async def submit_stats_report(self):
         """Invoked by the IOLoop"""
         LOGGER.debug('Submitting stats report')
-        result = self.callproc('pgq.get_consumer_info', self.worker_name,
-                               self.consumer_name)
-        LOGGER.debug('Post consumer info: %r', result)
+        result = await self.callproc(
+            'pgq.get_consumer_info', self.worker_name, self.consumer_name)
         self.stats.set_gauge(self.PENDING, result[0].get('pending_events', 0))
-        self._kwargs['stats_queue'].put(self.stats.report(), True)
+        self.stats_queue.put(self.stats.report(), True)
         self.last_stats_time = time.time()
 
-    def stop(self, signum=None, _unused=None):
+    async def stop(self) -> typing.NoReturn:
         """Stop the consumer from consuming by calling BasicCancel and setting
         our state.
-        :param int signum: The signal received
-        :param frame _unused: The stack frame from when the signal was called
         """
         LOGGER.debug('Stop called in state: %s', self.state_description)
         if self.is_stopped:
             LOGGER.warning('Stop requested but worker is already stopped')
             return
         elif self.is_shutting_down:
             LOGGER.warning('Stop requested, worker is already shutting down')
             return
         elif self.is_waiting_to_shutdown:
             LOGGER.warning('Stop requested but already waiting to shut down')
             return
 
-        # Wait until the consumer has finished processing to shutdown
+        # Wait until the consumer has finished processing to shut down
         if self.is_processing:
             LOGGER.info('Waiting for batch to finish processing')
             self.set_state(self.STATE_STOP_REQUESTED)
-            if signum == signal.SIGTERM:
-                signal.siginterrupt(signal.SIGTERM, False)
             return
 
-        # Stop and flush the statds data
-        if self.stats.statsd:
-            self.stats.statsd.stop()
+        # Stop and flush the stats data
+        await self.stats.stop()
 
         self.on_ready_to_stop()
 
-    def send_exception_to_sentry(self):
-        """Send an exception to Sentry if enabled.
-        :param tuple exc_info: exception information as returned from
-            :func:`sys.exc_info`
-        """
-        if self.sentry_client:
-            self.sentry_client.captureException(sys.exc_info())
-
-    def set_sentry_context(self, tag, value):
-        """Set a context tag in Sentry for the given key and value.
-        :param str tag: The context tag name
-        :param str value: The context value
-        """
-        if self.sentry_client:
-            LOGGER.debug('Setting sentry context for %s to %s', tag, value)
-            self.sentry_client.tags_context({tag: value})
+    @staticmethod
+    def send_exception_to_sentry() -> typing.NoReturn:
+        """Send an exception to Sentry if enabled."""
+        if sentry_sdk:
+            sentry_sdk.capture_exception(sys.exc_info())
 
-    def statsd_add_timing(self, key, duration):
-        """Add a timing to statsd
-        :param str key: The key to add the timing to
-        :param int|float duration: The timing value
-        """
-        if self.stats.statsd:
-            self.stats.statsd.add_timing(key, duration)
-
-    def statsd_incr(self, key, value=1):
-        """Increment the specified key in statsd if statsd is enabled.
-        :param str key: The key to increment
-        :param int value: The value to increment the key by
-        """
-        if self.stats.statsd:
-            self.stats.statsd.incr(key, value)
-
-    @contextlib.contextmanager
-    def statsd_track_duration(self, key):
-        """Time around a context and emit a statsd metric.
-        :param str key: The key for the timing to track
-        """
-        start_time = time.time()
-        try:
-            yield
-        finally:
-            finish_time = max(start_time, time.time())
-            self.statsd_add_timing(key, finish_time - start_time)
+    @staticmethod
+    def set_sentry_context(tag: str, value: str) -> typing.NoReturn:
+        """Set a context tag in Sentry for the given key and value."""
+        if sentry_sdk:
+            LOGGER.debug('Setting sentry context for %s to %s', tag, value)
+            sentry_sdk.set_tag(tag, value)
 
 
 class MikkooError(Exception):
     """Base class for all Mikkoo exceptions"""
     pass
```

### Comparing `mikkoo-1.1.2/mikkoo/mcp.py` & `mikkoo-2.0.0/mikkoo/mcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
 Master Control Program
 
 """
 import logging
 import multiprocessing
 import os
-import psutil
-try:
-    import Queue as queue
-except ImportError:
-    import queue
+import queue
 import signal
 import sys
 import time
+import types
+import typing
+
+import helper.config
+import psutil
 
-from mikkoo import state
-from mikkoo import worker
-from mikkoo import __version__
+from mikkoo import __version__, state, worker
 
 LOGGER = logging.getLogger(__name__)
 
 
-class Worker(object):
+class Worker:
     """Class used for keeping track of each worker type being managed by
     the MCP
 
     """
-    def __init__(self, config, stats_queue):
+    def __init__(self,
+                 config: helper.config.Config,
+                 stats_queue: multiprocessing.Queue):
         self.config = config
         self.process = None
         self.stats_queue = stats_queue
         self.unresponsive = 0
 
 
 class MasterControlProgram(state.State):
@@ -38,49 +39,39 @@
 
     MAX_UNRESPONSIVE = 3
     MAX_SHUTDOWN_WAIT = 10
     POLL_INTERVAL = 60.0
     POLL_RESULTS_INTERVAL = 3.0
     SHUTDOWN_WAIT = 1
 
-    def __init__(self, config):
-        """Initialize the Master Control Program
-
-        :param helper.config.Config config: Mikkoo Configuration
-
-        """
+    def __init__(self, config: helper.config.Config):
+        """Initialize the Master Control Program"""
         self.set_process_name()
         LOGGER.info('Mikkoo v%s initializing', __version__)
         super(MasterControlProgram, self).__init__()
         self.config = config
-
-        self.last_poll_results = dict()
-        self.poll_data = {'time': 0, 'processes': list()}
+        self.last_poll_results = {}
+        self.poll_data = {'time': 0, 'processes': []}
         self.poll_timer = None
         self.results_timer = None
-        self.stats = dict()
+        self.stats = {}
         self.stats_queue = multiprocessing.Queue()
         self.polled = False
-
-        self.workers = dict()
+        self.workers = {}
         for name in config.application.workers.keys():
-            self.workers[name] = Worker(config.application.workers[name],
-                                        self.stats_queue)
+            self.workers[name] = Worker(
+                config.application.workers[name], self.stats_queue)
 
-        self.poll_interval = config.application.get('poll_interval',
-                                                    self.POLL_INTERVAL)
+        self.poll_interval = config.application.get(
+            'poll_interval', self.POLL_INTERVAL)
 
     @property
-    def active_processes(self):
-        """Return a list of all active processes, pruning dead ones
-
-        :rtype: list
-
-        """
-        active_processes, dead_processes = list(), list()
+    def active_processes(self) -> typing.List[psutil.Process]:
+        """Return a list of all active processes, pruning dead ones"""
+        active_processes, dead_processes = [], []
         for name in self.workers.keys():
             if self.workers[name].process.pid == os.getpid():
                 continue
             try:
                 proc = psutil.Process(self.workers[name].process.pid)
             except psutil.NoSuchProcess:
                 dead_processes.append(name)
@@ -93,28 +84,23 @@
 
         if dead_processes:
             LOGGER.debug('Removing %i dead process(es)', len(dead_processes))
             for name in dead_processes:
                 self.remove_worker_process(name)
         return active_processes
 
-    def calculate_stats(self, data):
-        """Calculate the stats data for our process level data.
-
-        :param data: The collected stats data to report on
-        :type data: dict
-
-        """
+    def calculate_stats(self, data: dict) -> dict:
+        """Calculate the stats data for our process level data."""
         timestamp = data['timestamp']
         del data['timestamp']
         LOGGER.debug('Calculating stats for data timestamp: %i', timestamp)
 
         # Iterate through the last poll results
         stats = self.worker_stats_counter()
-        worker_stats = dict()
+        worker_stats = {}
         for name in data.keys():
             worker_stats[name] = self.worker_stats_counter()
             for key in stats:
                 value = data[name]['counts'].get(key, 0)
                 stats[key] += value
                 worker_stats[name][key] += value
 
@@ -123,85 +109,71 @@
         return {
             'last_poll': timestamp,
             'workers': worker_stats,
             'process_data': data,
             'counts': stats
         }
 
-    def check_processes(self):
+    def check_processes(self) -> typing.NoReturn:
         """Check to make sure the worker processes are working..."""
         LOGGER.debug('Checking worker processes')
         for name in self.workers.keys():
             if self.workers[name].unresponsive >= self.MAX_UNRESPONSIVE:
                 if self.workers[name].process:
                     LOGGER.info('Killing unresponsive %s worker', name)
                     os.kill(int(self.workers[name].process.pid),
                             signal.SIGKILL)
                 self.workers[name].process = None
         for name in self.workers.keys():
             if (not self.workers[name].process or
                     not self.workers[name].process.is_alive()):
                 self.start_process(name)
 
-    def collect_results(self, data_values):
-        """Receive the data from the workers polled and process it.
-
-        :param dict data_values: The poll data returned from the worker
-        :type data_values: dict
-
-        """
+    def collect_results(self, data_values: dict) -> typing.NoReturn:
+        """Receive the data from the workers polled and process it."""
         self.last_poll_results['timestamp'] = self.poll_data['timestamp']
 
         # Get the name and worker name and remove it from what is reported
         worker_name = data_values['worker_name']
         del data_values['worker_name']
         del data_values['name']
 
         # Add it to our last poll global data
         self.last_poll_results[worker_name] = data_values
 
         # Calculate the stats
         self.stats = self.calculate_stats(self.last_poll_results)
 
     @staticmethod
-    def worker_stats_counter():
-        """Return a new worker stats counter instance.
-
-        :rtype: dict
-
-        """
+    def worker_stats_counter() -> dict:
+        """Return a new worker stats counter instance."""
         return {
             worker.Process.BATCHES: 0,
             worker.Process.ERROR: 0,
             worker.Process.PROCESSED: 0,
             worker.Process.PENDING: 0
         }
 
     @staticmethod
-    def is_dead(process):
-        """Checks to see if the specified process is dead.
-
-        :param psutil.Process process: The process to check
-        :rtype: bool
-
-        """
+    def is_dead(process: psutil.Process) -> bool:
+        """Checks to see if the specified process is dead."""
         status = process.status()
         LOGGER.debug('Process status (%r): %r', process.pid, status)
         try:
             if status == psutil.STATUS_ZOMBIE:
                 process.terminate()
                 return True
             elif status == psutil.STATUS_DEAD:
                 return True
         except psutil.NoSuchProcess:
             LOGGER.debug('Process is dead and does not exist')
             return True
         return False
 
-    def kill_processes(self):
+    def kill_processes(self) -> typing.NoReturn:
         """Gets called on shutdown by the timer when too much time has gone by,
         calling the terminate method instead of nicely asking for the workers
         to stop.
 
         """
         LOGGER.critical('Max shutdown exceeded, forcibly exiting')
         processes = True
@@ -213,15 +185,15 @@
                                    process.name, process.pid)
                     os.kill(int(process.pid), signal.SIGKILL)
             time.sleep(0.5)
 
         LOGGER.info('Killed all children')
         return self.set_state(self.STATE_STOPPED)
 
-    def log_stats(self):
+    def log_stats(self) -> typing.NoReturn:
         """Output the stats to the LOGGER."""
         if not self.stats.get('counts'):
             LOGGER.info('Did not receive any stats data from children')
             return
 
         if self.poll_data['processes']:
             LOGGER.warning('%i process(es) did not respond with stats: %r',
@@ -235,95 +207,91 @@
             LOGGER.info('%s worker processed %i events with %i errors '
                         'in %i batches with %i pending events', name,
                         self.stats['workers'][name][worker.Process.PROCESSED],
                         self.stats['workers'][name][worker.Process.ERROR],
                         self.stats['workers'][name][worker.Process.BATCHES],
                         self.stats['workers'][name][worker.Process.PENDING])
 
-    def new_process(self, name):
-        """Create a new worker instances
-
-        :param str name: The name of the worker
-        :return tuple: (str, process.Process)
-
-        """
+    def new_process(self, name: str) -> worker.Process:
+        """Create a new worker instance / process"""
         LOGGER.debug('Creating a new %s process', name)
         kwargs = {
             'config': {
+                'logging': self.config.logging,
                 'statsd': self.config.application.get('statsd', {}),
                 'worker': self.workers[name].config
             },
             'daemon': False,
             'stats_queue': self.stats_queue,
             'worker_name': name,
         }
         return worker.Process(name=name, kwargs=kwargs)
 
-    def on_abort(self, _signum, _unused_frame):
+    def on_abort(self,
+                 _signum: int,
+                 _frame: types.FrameType) -> typing.NoReturn:
         LOGGER.debug('Abort signal received from child')
         time.sleep(1)
         if not self.active_processes:
             LOGGER.info('Stopping with no active processes and child error')
             self.set_state(self.STATE_STOPPED)
 
-    def on_timer(self, _signum, _unused_frame):
+    def on_timer(self,
+                 _signum: int,
+                 _frame: types.FrameType) -> typing.NoReturn:
         if self.is_shutting_down:
             LOGGER.debug('Polling timer fired while shutting down')
             return
         if not self.polled:
             self.poll()
             self.polled = True
             self.set_timer(5)  # Wait 5 seconds for results
         else:
             self.polled = False
             self.poll_results_check()
             self.set_timer(self.poll_interval)  # Wait poll interval duration
             self.log_stats()
 
-    def poll(self):
+    def poll(self) -> typing.NoReturn:
         """Start the poll process by invoking the get_stats method of the
         workers. If we hit this after another interval without fully
         processing, note it with a warning.
 
         """
         self.set_state(self.STATE_ACTIVE)
 
         # If we don't have any active workers, spawn new ones
         if not self.total_process_count:
             LOGGER.debug('Did not find any active workers in poll')
             return self.check_processes()
 
         # Start our data collection dict
-        self.poll_data = {'timestamp': time.time(), 'processes': list()}
+        self.poll_data = {'timestamp': time.time(), 'processes': []}
 
-        # Iterate through all of the workers
+        # Iterate through the worker processes
         for process in self.active_processes:
             LOGGER.debug('Checking runtime state of %s', process.name)
             if process == multiprocessing.current_process():
                 LOGGER.debug('Matched current process in active_processes')
                 continue
 
             # Send the profile signal
             os.kill(int(process.pid), signal.SIGPROF)
             self.poll_data['processes'].append(process.name)
 
         # Check if we need to start more processes
         self.check_processes()
 
     @property
-    def poll_duration_exceeded(self):
-        """Return true if the poll time has been exceeded.
-
-        :rtype: bool
-
-        """
+    def poll_duration_exceeded(self) -> bool:
+        """Return true if the poll time has been exceeded."""
         return (time.time() -
                 self.poll_data['timestamp']) >= self.poll_interval
 
-    def poll_results_check(self):
+    def poll_results_check(self) -> typing.NoReturn:
         """Check the polling results by checking to see if the stats queue is
         empty. If it is not, try and collect stats. If it is set a timer to
         call ourselves in _POLL_RESULTS_INTERVAL.
 
         """
         LOGGER.debug('Checking for poll results')
         while True:
@@ -337,28 +305,24 @@
                 pass
             self.collect_results(stats)
 
         if self.poll_data['processes']:
             LOGGER.warning('Did not receive results from %r',
                            self.poll_data['processes'])
 
-    def remove_worker_process(self, name):
-        """Remove all details for the specified worker and process name.
-
-        :param str name: The worker name
-
-        """
+    def remove_worker_process(self, name: str) -> typing.NoReturn:
+        """Remove all details for the specified worker and process name."""
         if self.workers[name].process.is_alive():
             try:
                 self.workers[name].process.terminate()
             except OSError:
                 pass
         self.workers[name].process = None
 
-    def run(self):
+    def run(self) -> typing.NoReturn:
         """When the worker is ready to start running, kick off all of our
         worker workers and then loop while we process messages.
 
         """
         self.set_state(self.STATE_ACTIVE)
         self.setup_workers()
 
@@ -374,65 +338,57 @@
         # Loop for the lifetime of the app, pausing for a signal to pop up
         while self.is_running:
             if not self.is_sleeping:
                 self.set_state(self.STATE_SLEEPING)
             signal.pause()
 
     @staticmethod
-    def set_process_name():
+    def set_process_name() -> typing.NoReturn:
         """Set the process name for the top level process so that it shows up
         in logs in a more trackable fashion.
 
         """
         proc = multiprocessing.current_process()
         for offset in range(0, len(sys.argv)):
             if sys.argv[offset] == '-c':
                 name = sys.argv[offset + 1].split('/')[-1]
                 proc.name = name.split('.')[0]
                 break
 
-    def set_timer(self, duration):
-        """Setup the next alarm to fire and then wait for it to fire.
-
-        :param int duration: How long to sleep
-
-        """
+    def set_timer(self, duration: int) -> typing.NoReturn:
+        """Set up the next alarm to fire and then wait for it to fire."""
         # Make sure that the application is not shutting down before sleeping
         if self.is_shutting_down:
             LOGGER.debug('Not sleeping, application is trying to shutdown')
             return
 
         # Set the signal timer
         signal.setitimer(signal.ITIMER_REAL, duration, 0)
 
-    def start_process(self, name):
-        """Start a new worker process for the given worker & connection name
-
-        :param str name: The worker name
-
-        """
+    def start_process(self, name: str) -> typing.NoReturn:
+        """Start a new worker process for the given worker & connection name"""
         process = self.new_process(name)
         LOGGER.info('Spawning %s process', name)
 
         # Append the process to the worker process list
         self.workers[name].process = process
 
         # Start the process
         process.start()
 
-    def setup_workers(self):
+    def setup_workers(self) -> typing.NoReturn:
         """Iterate through each worker in the configuration and kick off the
         minimal amount of processes, setting up the runtime data as well.
 
         """
         for name in self.config.application.workers.keys():
             self.start_process(name)
 
-    def stop_processes(self):
-        """Iterate through all of the worker processes shutting them down."""
+    def stop_processes(self) -> typing.NoReturn:
+        """Iterate through the worker processes shutting them down."""
         self.set_state(self.STATE_SHUTTING_DOWN)
         LOGGER.info('Stopping worker processes')
 
         signal.signal(signal.SIGABRT, signal.SIG_IGN)
         signal.signal(signal.SIGALRM, signal.SIG_IGN)
         signal.signal(signal.SIGCHLD, signal.SIG_IGN)
         signal.signal(signal.SIGPROF, signal.SIG_IGN)
@@ -463,14 +419,10 @@
                 break
             processes = self.total_process_count
 
         LOGGER.debug('All worker processes stopped')
         self.set_state(self.STATE_STOPPED)
 
     @property
-    def total_process_count(self):
-        """Returns the active worker process count
-
-        :rtype: int
-
-        """
+    def total_process_count(self) -> int:
+        """Returns the active worker process count"""
         return len(self.active_processes)
```

### Comparing `mikkoo-1.1.2/README.rst` & `mikkoo-2.0.0/README.rst`

 * *Files identical despite different names*

