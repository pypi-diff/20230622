# Comparing `tmp/redis_rate_limiters-0.2.0.tar.gz` & `tmp/redis_rate_limiters-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_rate_limiters-0.2.0.tar", max compression
+gzip compressed data, was "redis_rate_limiters-0.3.0.tar", max compression
```

## Comparing `redis_rate_limiters-0.2.0.tar` & `redis_rate_limiters-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1652 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/LICENSE
--rw-r--r--   0        0        0     5218 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/README.md
--rw-r--r--   0        0        0      294 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/__init__.py
--rw-r--r--   0        0        0     1593 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/base.py
--rw-r--r--   0        0        0      143 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/py.typed
--rw-r--r--   0        0        0     1544 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/semaphore.lua
--rw-r--r--   0        0        0     4434 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/semaphore.py
--rw-r--r--   0        0        0     2349 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/token_bucket.lua
--rw-r--r--   0        0        0     3328 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/limiters/token_bucket.py
--rw-r--r--   0        0        0     3155 2023-06-13 22:13:00.200851 redis_rate_limiters-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6474 1970-01-01 00:00:00.000000 redis_rate_limiters-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1652 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5218 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/README.md
+-rw-r--r--   0        0        0      294 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/__init__.py
+-rw-r--r--   0        0        0     1593 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/base.py
+-rw-r--r--   0        0        0      143 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/py.typed
+-rw-r--r--   0        0        0     1544 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/semaphore.lua
+-rw-r--r--   0        0        0     4465 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/semaphore.py
+-rw-r--r--   0        0        0     2349 2023-06-22 13:12:30.716618 redis_rate_limiters-0.3.0/limiters/token_bucket.lua
+-rw-r--r--   0        0        0     3328 2023-06-22 13:12:30.716618 redis_rate_limiters-0.3.0/limiters/token_bucket.py
+-rw-r--r--   0        0        0     3155 2023-06-22 13:12:30.716618 redis_rate_limiters-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6474 1970-01-01 00:00:00.000000 redis_rate_limiters-0.3.0/PKG-INFO
```

### Comparing `redis_rate_limiters-0.2.0/LICENSE` & `redis_rate_limiters-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.2.0/README.md` & `redis_rate_limiters-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.2.0/limiters/base.py` & `redis_rate_limiters-0.3.0/limiters/base.py`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.2.0/limiters/semaphore.lua` & `redis_rate_limiters-0.3.0/limiters/semaphore.lua`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.2.0/limiters/semaphore.py` & `redis_rate_limiters-0.3.0/limiters/semaphore.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 logger = logging.getLogger(__name__)
 
 
 class SemaphoreBase(BaseModel):
     name: str
     capacity: int = Field(gt=0)
     max_sleep: float = Field(ge=0, default=0.0)
-    expiry: int | None = None
+    expiry: int = 30
 
     @property
     def key(self) -> str:
         """Key to use for the Semaphore list."""
         return f'{{limiter}}:semaphore:{self.name}'
 
     @property
@@ -48,40 +48,40 @@
 
         if semaphore_created:
             logger.info('Created new semaphore `%s` with capacity %s', self.name, self.capacity)
         else:
             logger.debug('Skipped creating semaphore, since one exists')
 
         start = datetime.now()
+
         self.connection.blpop(self.key, self.max_sleep)
+        pipeline = self.connection.pipeline()
+        pipeline.expire(self.key, self.expiry)
+        pipeline.expire(self.exists, self.expiry)
+        pipeline.execute()
 
         # Raise an exception if we exceeded `max_sleep`
         if 0.0 < self.max_sleep < (datetime.now() - start).total_seconds():
             raise MaxSleepExceededError('Max sleep exceeded waiting for Semaphore')
 
         logger.debug('Acquired semaphore %s', self.name)
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
-        if self.expiry:
-            pipeline = self.connection.pipeline()
-            # Return capacity to the semaphore
-            pipeline.lpush(self.key, 1)
-            # Set expiry to prevent deadlocks
-            pipeline.expire(self.key, self.expiry)
-            pipeline.expire(self.exists, self.expiry)
-            pipeline.execute()
-        else:
-            self.connection.lpush(self.key, 1)
+        pipeline = self.connection.pipeline()
+        pipeline.lpush(self.key, 1)
+        pipeline.expire(self.key, self.expiry)
+        pipeline.expire(self.exists, self.expiry)
+        pipeline.execute()
 
-        logger.debug('Released semaphore')
+        logger.debug('Released semaphore %s', self.name)
 
 
 class AsyncSemaphore(SemaphoreBase, AsyncLuaScriptBase):
     script_name: ClassVar[str] = 'semaphore.lua'
 
     async def __aenter__(self) -> None:
         """
@@ -94,33 +94,33 @@
             args=[self.capacity],
         ):
             logger.info('Created new semaphore `%s` with capacity %s', self.name, self.capacity)
         else:
             logger.debug('Skipped creating semaphore, since one exists')
 
         start = datetime.now()
+
         await self.connection.blpop(self.key, self.max_sleep)  # type: ignore[union-attr]
+        pipeline: Pipeline[str] | ClusterPipeline[str] = self.connection.pipeline()
+        pipeline.expire(self.key, self.expiry)  # type: ignore[union-attr]
+        pipeline.expire(self.exists, self.expiry)  # type: ignore[union-attr]
+        await pipeline.execute()
 
         # Raise an exception if we waited too long
         if 0.0 < self.max_sleep < (datetime.now() - start).total_seconds():
             raise MaxSleepExceededError(f'Max sleep ({self.max_sleep}s) exceeded waiting for Semaphore')
 
         logger.debug('Acquired semaphore %s', self.name)
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
-        if self.expiry:
-            pipeline: Pipeline[str] | ClusterPipeline[str] = self.connection.pipeline()
-            # Return capacity to the semaphore
-            pipeline.lpush(self.key, 1)  # type: ignore[union-attr]
-            # Set expiry to prevent deadlocks
-            pipeline.expire(self.key, self.expiry)  # type: ignore[union-attr]
-            pipeline.expire(self.exists, self.expiry)  # type: ignore[union-attr]
-            await pipeline.execute()
-        else:
-            await self.connection.lpush(self.key, 1)  # type: ignore[union-attr]
+        pipeline: Pipeline[str] | ClusterPipeline[str] = self.connection.pipeline()
+        pipeline.lpush(self.key, 1)  # type: ignore[union-attr]
+        pipeline.expire(self.key, self.expiry)  # type: ignore[union-attr]
+        pipeline.expire(self.exists, self.expiry)  # type: ignore[union-attr]
+        await pipeline.execute()
 
-        logger.debug('Released semaphore')
+        logger.debug('Released semaphore %s', self.name)
```

### Comparing `redis_rate_limiters-0.2.0/limiters/token_bucket.lua` & `redis_rate_limiters-0.3.0/limiters/token_bucket.lua`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.2.0/limiters/token_bucket.py` & `redis_rate_limiters-0.3.0/limiters/token_bucket.py`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.2.0/pyproject.toml` & `redis_rate_limiters-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-rate-limiters"
-version = "0.2.0"
+version = "0.3.0"
 description = "Distributed rate limiters"
 license = "BSD-4-Clause"
 authors = ["Sondre Lillebø Gundersen <sondrelg@live.no>"]
 readme = "README.md"
 homepage = "https://github.com/otovo/redis-rate-limiters"
 repository = "https://github.com/otovo/redis-rate-limiters"
 keywords = [
```

### Comparing `redis_rate_limiters-0.2.0/PKG-INFO` & `redis_rate_limiters-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-rate-limiters
-Version: 0.2.0
+Version: 0.3.0
 Summary: Distributed rate limiters
 Home-page: https://github.com/otovo/redis-rate-limiters
 License: BSD-4-Clause
 Keywords: async,sync,rate,limiting,limiters
 Author: Sondre Lillebø Gundersen
 Author-email: sondrelg@live.no
 Requires-Python: >=3.11,<4.0
```

