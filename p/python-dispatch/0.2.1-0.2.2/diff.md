# Comparing `tmp/python-dispatch-0.2.1.tar.gz` & `tmp/python-dispatch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dispatch-0.2.1.tar", last modified: Mon Dec 19 20:20:44 2022, max compression
+gzip compressed data, was "python-dispatch-0.2.2.tar", last modified: Thu Jun 22 16:52:10 2023, max compression
```

## Comparing `python-dispatch-0.2.1.tar` & `python-dispatch-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:20:44.664831 python-dispatch-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-19 20:19:53.000000 python-dispatch-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-19 20:19:53.000000 python-dispatch-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2022-12-19 20:20:44.664831 python-dispatch-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2022-12-19 20:19:53.000000 python-dispatch-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:20:44.664831 python-dispatch-0.2.1/pydispatch/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-19 20:19:53.000000 python-dispatch-0.2.1/pydispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2022-12-19 20:19:53.000000 python-dispatch-0.2.1/pydispatch/aioutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2022-12-19 20:19:53.000000 python-dispatch-0.2.1/pydispatch/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2022-12-19 20:19:53.000000 python-dispatch-0.2.1/pydispatch/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2022-12-19 20:19:53.000000 python-dispatch-0.2.1/pydispatch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:20:44.664831 python-dispatch-0.2.1/python_dispatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2022-12-19 20:20:44.000000 python-dispatch-0.2.1/python_dispatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2022-12-19 20:20:44.000000 python-dispatch-0.2.1/python_dispatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 20:20:44.000000 python-dispatch-0.2.1/python_dispatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-19 20:20:44.000000 python-dispatch-0.2.1/python_dispatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2022-12-19 20:20:44.668831 python-dispatch-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-19 20:19:53.000000 python-dispatch-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:52:10.989647 python-dispatch-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-22 16:52:10.989647 python-dispatch-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:52:10.989647 python-dispatch-0.2.2/pydispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/pydispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/pydispatch/aioutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/pydispatch/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/pydispatch/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/pydispatch/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/pydispatch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:52:10.989647 python-dispatch-0.2.2/python_dispatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-22 16:52:10.000000 python-dispatch-0.2.2/python_dispatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-22 16:52:10.000000 python-dispatch-0.2.2/python_dispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:52:10.000000 python-dispatch-0.2.2/python_dispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 16:52:10.000000 python-dispatch-0.2.2/python_dispatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-22 16:52:10.989647 python-dispatch-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:52:10.989647 python-dispatch-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14721 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/tests/test_aio_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/tests/test_aio_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/tests/test_global_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/tests/test_subclass_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-22 16:52:04.000000 python-dispatch-0.2.2/tests/test_version_attribute.py
```

### Comparing `python-dispatch-0.2.1/LICENSE.txt` & `python-dispatch-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-dispatch-0.2.1/PKG-INFO` & `python-dispatch-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dispatch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Lightweight Event Handling
 Home-page: https://github.com/nocarryr/python-dispatch
 Author: Matthew Reid
 Author-email: matt@nomadic-recording.com
 License: MIT
 Project-URL: Documentation, https://python-dispatch.readthedocs.io
 Project-URL: Source, https://github.com/nocarryr/python-dispatch
```

### Comparing `python-dispatch-0.2.1/README.md` & `python-dispatch-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python-dispatch-0.2.1/pydispatch/aioutils.py` & `python-dispatch-0.2.2/pydispatch/aioutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import threading
 from _weakref import ref
 from _weakrefset import _IterationGuard
 
 from pydispatch.utils import (
     WeakMethodContainer,
+    isfunction,
     get_method_vars,
     _remove_dead_weakref,
 )
 
 
 class AioSimpleLock(object):
     """:class:`asyncio.Lock` alternative backed by a :class:`threading.Lock`
@@ -196,17 +197,21 @@
         """Add a coroutine function
 
         Args:
             loop: The :class:`event loop <asyncio.BaseEventLoop>` instance
                 on which to schedule callbacks
             callback: The :term:`coroutine function` to add
         """
-        f, obj = get_method_vars(callback)
-        wrkey = (f, id(obj))
-        self[wrkey] = obj
+        if isfunction(callback):
+            wrkey = ('function', id(callback))
+            self[wrkey] = callback
+        else:
+            f, obj = get_method_vars(callback)
+            wrkey = (f, id(obj))
+            self[wrkey] = obj
         self.event_loop_map[wrkey] = loop
     def iter_instances(self):
         """Iterate over the stored objects
 
         .. seealso:: :meth:`pydispatch.utils.WeakMethodContainer.iter_instances`
         """
         with _IterationGuard(self):
@@ -217,16 +222,19 @@
         Yields:
             Stored :term:`coroutine function` objects
 
         .. seealso:: :meth:`pydispatch.utils.WeakMethodContainer.iter_instances`
         """
         for wrkey, obj in self.iter_instances():
             f, obj_id = wrkey
+            if f == 'function':
+                m = self[wrkey]
+            else:
+                m = getattr(obj, f.__name__)
             loop = self.event_loop_map[wrkey]
-            m = getattr(obj, f.__name__)
             yield loop, m
     def _on_weakref_fin(self, key):
         if key in self.event_loop_map:
             del self.event_loop_map[key]
     def submit_coroutine(self, coro, loop):
         """Schedule and await a coroutine on the specified loop
```

### Comparing `python-dispatch-0.2.1/pydispatch/dispatch.py` & `python-dispatch-0.2.2/pydispatch/dispatch.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,59 @@
     EmissionHoldLock,
     iscoroutinefunction,
 )
 from pydispatch.properties import Property
 import asyncio
 from pydispatch.aioutils import AioWeakMethodContainer, AioEventWaiters
 
+__all__ = (
+    'DoesNotExistError', 'ExistsError', 'EventExistsError',
+    'PropertyExistsError', 'Event', 'Dispatcher',
+)
+
+
+class DoesNotExistError(KeyError):
+    """Raised when binding to an :class:`Event` or :class:`~.properties.Property`
+    that does not exist
+
+    .. versionadded:: 0.2.2
+    """
+    def __init__(self, name):
+        self.name = name
+
+    def __str__(self):
+        return f'Event "{self.name}" not registered'
+
+
+class ExistsError(RuntimeError):
+    """Raised when registering an event name that already exists
+    as either a normal :class:`Event` or :class:`~.properies.Property`
+
+    .. versionadded:: 0.2.2
+    """
+    def __init__(self, name):
+        self.name = name
+
+    def __str__(self):
+        return f'"{self.name}" already exists'
+
+class EventExistsError(ExistsError):
+    """Raised when registering an event name that already exists
+    as an :class:`Event`
+
+    .. versionadded:: 0.2.2
+    """
+
+
+class PropertyExistsError(ExistsError):
+    """Raised when registering an event name that already exists
+    as a :class:`~.properties.Property`
+
+    .. versionadded:: 0.2.2
+    """
 
 
 class Event(object):
     """Holds references to event names and subscribed listeners
 
     This is used internally by :class:`Dispatcher`.
     """
@@ -104,18 +149,28 @@
             self.__property_events[name] = Event(name)
             prop._add_instance(self)
     def register_event(self, *names):
         """Registers new events after instance creation
 
         Args:
             *names (str): Name or names of the events to register
+
+        Raises:
+            EventExistsError: If an event with the given name already exists
+            PropertyExistsError: If a property with the given name already exists
+
+        .. versionchanged:: 0.2.2
+            :class:`ExistsError` exceptions are raised when attempting to
+            register an event or property that already exists
         """
         for name in names:
             if name in self.__events:
-                continue
+                raise EventExistsError(name)
+            elif name in self.__property_events:
+                raise PropertyExistsError(name)
             self.__events[name] = Event(name)
     def bind(self, **kwargs):
         """Subscribes to events or to :class:`~pydispatch.properties.Property` updates
 
         Keyword arguments are used with the Event or Property names as keys
         and the callbacks as values::
 
@@ -136,14 +191,16 @@
             Callbacks may be :term:`coroutine functions <coroutine function>`
             (defined using :keyword:`async def` or decorated with
             :func:`@asyncio.coroutine <asyncio.coroutine>`), but an event loop
             must be explicitly provided with the keyword
             argument ``"__aio_loop__"`` (an instance of
             :class:`asyncio.BaseEventLoop`)
 
+            >>> import asyncio
+
             >>> class Foo(Dispatcher):
             ...     _events_ = ['test_event']
 
             >>> class Bar(object):
             ...     def __init__(self):
             ...         self.got_foo_event = asyncio.Event()
             ...     async def wait_for_foo(self):
@@ -160,25 +217,36 @@
 
             >>> foo.emit('test_event')
             >>> loop.run_until_complete(fut)
             got foo!
 
             This can also be done using :meth:`bind_async`.
 
+            Raises:
+                DoesNotExistError: If attempting to bind to an event or
+                    property that has not been registered
+
+            .. versionchanged:: 0.2.2
+                :class:`DoesNotExistError` is now raised when binding to
+                non-existent events or properties
+
             .. versionadded:: 0.1.0
 
         """
         aio_loop = kwargs.pop('__aio_loop__', None)
         props = self.__property_events
         events = self.__events
         for name, cb in kwargs.items():
             if name in props:
                 e = props[name]
             else:
-                e = events[name]
+                try:
+                    e = events[name]
+                except KeyError:
+                    raise DoesNotExistError(name)
             e.add_listener(cb, __aio_loop__=aio_loop)
     def unbind(self, *args):
         """Unsubscribes from events or :class:`~pydispatch.properties.Property` updates
 
         Multiple arguments can be given. Each of which can be either the method
         that was used for the original call to :meth:`bind` or an instance
         object.
@@ -220,34 +288,55 @@
             If a listener returns :obj:`False`, the event will stop dispatching to
             other listeners. Any other return value is ignored.
 
         Args:
             name (str): The name of the :class:`Event` to dispatch
             *args (Optional): Positional arguments to be sent to listeners
             **kwargs (Optional): Keyword arguments to be sent to listeners
+
+        Raises:
+            DoesNotExistError: If attempting to emit an event or
+                property that has not been registered
+
+        .. versionchanged:: 0.2.2
+            :class:`DoesNotExistError` is now raised if the event or property
+            does not exist
         """
         e = self.__property_events.get(name)
         if e is None:
-            e = self.__events[name]
+            try:
+                e = self.__events[name]
+            except KeyError:
+                raise DoesNotExistError(name)
         return e(*args, **kwargs)
     def get_dispatcher_event(self, name):
         """Retrieves an Event object by name
 
         Args:
             name (str): The name of the :class:`Event` or
                 :class:`~pydispatch.properties.Property` object to retrieve
 
         Returns:
             The :class:`Event` instance for the event or property definition
 
+        Raises:
+            DoesNotExistError: If no event or property with the given name exists
+
+        .. versionchanged:: 0.2.2
+            :class:`DoesNotExistError` is now raised if the event or property
+            does not exist
+
         .. versionadded:: 0.1.0
         """
         e = self.__property_events.get(name)
         if e is None:
-            e = self.__events[name]
+            try:
+                e = self.__events[name]
+            except KeyError:
+                raise DoesNotExistError(name)
         return e
     def emission_lock(self, name):
         """Holds emission of events and dispatches the last event on release
 
         The context manager returned will store the last event data called by
         :meth:`emit` and prevent callbacks until it exits. On exit, it will
         dispatch the last event captured (if any)
@@ -275,13 +364,30 @@
             If available, this will also be an async context manager to be used
             with the :keyword:`async with` statement (see `PEP 492`_).
 
         Note:
             The context manager is re-entrant, meaning that multiple calls to
             this method within nested context scopes are possible.
 
+        Raises:
+            DoesNotExistError: If no event or property with the given name exists
+
+        .. versionchanged:: 0.2.2
+            :class:`DoesNotExistError` is now raised if the event or property
+            does not exist
+
         .. _PEP 492: https://www.python.org/dev/peps/pep-0492/#asynchronous-context-managers-and-async-with
         """
-        e = self.__property_events.get(name)
-        if e is None:
-            e = self.__events[name]
+        e = self.get_dispatcher_event(name)
         return e.emission_lock
+
+
+class _GlobalDispatcher(Dispatcher):
+    def _has_event(self, name):
+        try:
+            self.get_dispatcher_event(name)
+        except KeyError:
+            return False
+        return True
+
+
+_GLOBAL_DISPATCHER = _GlobalDispatcher()
```

### Comparing `python-dispatch-0.2.1/pydispatch/properties.py` & `python-dispatch-0.2.2/pydispatch/properties.py`

 * *Files identical despite different names*

### Comparing `python-dispatch-0.2.1/pydispatch/utils.py` & `python-dispatch-0.2.2/pydispatch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import asyncio
 
 def get_method_vars(m):
     f = m.__func__
     obj = m.__self__
     return f, obj
 
+def isfunction(m):
+    return isinstance(m, types.FunctionType)
+
 def iscoroutinefunction(obj):
     return asyncio.iscoroutinefunction(obj)
 
 class WeakMethodContainer(weakref.WeakValueDictionary):
     """Container to store weak references to callbacks
 
     Instance methods are stored using the underlying :term:`function` object
@@ -24,27 +27,27 @@
     """
     def add_method(self, m, **kwargs):
         """Add an instance method or function
 
         Args:
             m: The instance method or function to store
         """
-        if isinstance(m, types.FunctionType):
+        if isfunction(m):
             self['function', id(m)] = m
         else:
             f, obj = get_method_vars(m)
             wrkey = (f, id(obj))
             self[wrkey] = obj
     def del_method(self, m):
         """Remove an instance method or function if it exists
 
         Args:
             m: The instance method or function to remove
         """
-        if isinstance(m, types.FunctionType) and not iscoroutinefunction(m):
+        if isfunction(m):
             wrkey = ('function', id(m))
         else:
             f, obj = get_method_vars(m)
             wrkey = (f, id(obj))
         if wrkey in self:
             del self[wrkey]
     def del_instance(self, obj):
```

### Comparing `python-dispatch-0.2.1/python_dispatch.egg-info/PKG-INFO` & `python-dispatch-0.2.2/python_dispatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dispatch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Lightweight Event Handling
 Home-page: https://github.com/nocarryr/python-dispatch
 Author: Matthew Reid
 Author-email: matt@nomadic-recording.com
 License: MIT
 Project-URL: Documentation, https://python-dispatch.readthedocs.io
 Project-URL: Source, https://github.com/nocarryr/python-dispatch
```

### Comparing `python-dispatch-0.2.1/setup.cfg` & `python-dispatch-0.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-dispatch
-version = 0.2.1
+version = 0.2.2
 author = Matthew Reid
 author_email = matt@nomadic-recording.com
 url = https://github.com/nocarryr/python-dispatch
 project_urls = 
 	Documentation = https://python-dispatch.readthedocs.io
 	Source = https://github.com/nocarryr/python-dispatch
 	Tracker = https://github.com/nocarryr/python-dispatch/issues
```

