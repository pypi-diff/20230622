# Comparing `tmp/snapstream-0.0.6.tar.gz` & `tmp/snapstream-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-0.0.6.tar", max compression
+gzip compressed data, was "snapstream-0.0.7.tar", max compression
```

## Comparing `snapstream-0.0.6.tar` & `snapstream-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-05-31 05:19:52.000025 snapstream-0.0.6/LICENSE
--rw-r--r--   0        0        0     2536 2023-05-31 05:19:52.000025 snapstream-0.0.6/README.md
--rw-r--r--   0        0        0     2034 2023-05-31 05:20:03.196342 snapstream-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2277 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/__init__.py
--rw-r--r--   0        0        0     7897 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/__main__.py
--rw-r--r--   0        0        0     9781 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/caching.py
--rw-r--r--   0        0        0     2562 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/codecs.py
--rw-r--r--   0        0        0    10677 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/core.py
--rw-r--r--   0        0        0     3255 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/utils.py
--rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-22 20:32:31.360191 snapstream-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2536 2023-06-22 20:32:31.360191 snapstream-0.0.7/README.md
+-rw-r--r--   0        0        0     2034 2023-06-22 20:32:44.784464 snapstream-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2277 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/__init__.py
+-rw-r--r--   0        0        0     7897 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/__main__.py
+-rw-r--r--   0        0        0     9781 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/caching.py
+-rw-r--r--   0        0        0     2812 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/codecs.py
+-rw-r--r--   0        0        0    10774 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/core.py
+-rw-r--r--   0        0        0     3255 2023-06-22 20:32:31.364192 snapstream-0.0.7/snapstream/utils.py
+-rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-0.0.7/PKG-INFO
```

### Comparing `snapstream-0.0.6/LICENSE` & `snapstream-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.6/README.md` & `snapstream-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.6/pyproject.toml` & `snapstream-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snapstream"
-version = "0.0.6"
+version = "0.0.7"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Menziess/snapstream"
 documentation = "https://snapstream.readthedocs.io"
 license = "MIT"
 keywords = ["kafka", "pubsub"]
```

### Comparing `snapstream-0.0.6/snapstream/__init__.py` & `snapstream-0.0.7/snapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.6/snapstream/__main__.py` & `snapstream-0.0.7/snapstream/__main__.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.6/snapstream/caching.py` & `snapstream-0.0.7/snapstream/caching.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.6/snapstream/codecs.py` & `snapstream-0.0.7/snapstream/codecs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Snapstream codecs."""
 
 import logging
 from abc import ABCMeta, abstractmethod
 from io import BytesIO
 from json import dumps, loads
-from typing import Any, cast
+from typing import Any, Union, cast
 
 from avro.io import BinaryDecoder, BinaryEncoder, DatumReader, DatumWriter
 from avro.schema import Schema, parse
 from toolz import curry
 
 logger = logging.getLogger(__name__)
 
@@ -76,18 +76,23 @@
         """Deserialize message."""
         return deserialize_json(s)
 
 
 class AvroCodec(ICodec):
     """Serialize/deserialize avro messages."""
 
-    def __init__(self, path: str):
+    def __init__(self, schema: Union[str, Schema]):
         """Load avro schema."""
-        with open(path) as a:
-            self.schema = parse(a.read())
+        if isinstance(schema, Schema):
+            self.schema = schema
+        elif isinstance(schema, str):
+            with open(schema) as a:
+                self.schema = parse(a.read())
+        else:
+            raise TypeError('Expected .avsc filepath str, or avro.schema.Schema instance.')
 
     def encode(self, obj: Any) -> bytes:
         """Serialize message."""
         val = serialize_avro(self.schema, obj)
         return cast(bytes, val)
 
     def decode(self, s: bytes) -> object:
```

### Comparing `snapstream-0.0.6/snapstream/core.py` & `snapstream-0.0.7/snapstream/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     @staticmethod
     def distribute_messages(it, queue, kwargs):
         """Publish messages from iterable."""
         iterable_key = str(id(it))
         try:
             for el in it:
                 pub.sendMessage(iterable_key, msg=el, kwargs=kwargs)
-        except Exception as e:
+        except BaseException as e:
             logger.debug(f'Exception in thread {current_thread().name}.')
             queue.put(e)
         finally:
             queue.put(None)
             logger.debug(f'Stopping thread {current_thread().name}.')
 
     def start(self, **kwargs):
@@ -140,27 +140,28 @@
         - Should serialize using topic codec.
         - Should skip sending message when dry is True.
         - Should show a warning when skipped.
         """
         raise NotImplementedError
 
 
-def _consumer_handler(c, conf, poll_timeout, codec):
+def _consumer_handler(c, conf, poll_timeout, codec, raise_error):
     manual_commit = pipe(
         conf.get('enable.auto.commit'),
         str,
         str.lower
     ) == 'false'
 
     while True:
         msg = c.poll(poll_timeout)
         if msg is None:
             continue
         if err := msg.error():
-            raise KafkaException(err)
+            if raise_error:
+                raise KafkaException(err)
         if codec:
             decoded_val = codec.decode(msg.value())
             msg.set_value(decoded_val)
 
         yield msg
 
         if manual_commit:
@@ -170,30 +171,31 @@
 @contextmanager
 def get_consumer(
     topic: str,
     conf: dict,
     offset=None,
     codec: Optional[ICodec] = None,
     poll_timeout: float = 1.0,
-    poller=_consumer_handler
+    poller=_consumer_handler,
+    raise_error=False
 ) -> Iterator[Iterable[Any]]:
     """Yield an iterable to consume from kafka."""
     c = Consumer(conf, logger=logger)
 
     def consume():
         def on_assign(c, ps):
             for p in ps:
-                if offset:
+                if offset is not None:
                     p.offset = offset
             c.assign(ps)
 
         logger.debug(f'Subscribing to topic: {topic}.')
         c.subscribe([topic], on_assign=on_assign)
         logger.debug(f'Consuming from topic: {topic}.')
-        yield from poller(c, conf, poll_timeout, codec)
+        yield from poller(c, conf, poll_timeout, codec, raise_error)
 
     try:
         yield consume()
     finally:
         c.close()
```

### Comparing `snapstream-0.0.6/snapstream/utils.py` & `snapstream-0.0.7/snapstream/utils.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.6/PKG-INFO` & `snapstream-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 0.0.6
+Version: 0.0.7
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 License: MIT
 Keywords: kafka,pubsub
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

