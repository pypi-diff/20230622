# Comparing `tmp/rmmbr-0.0.8.tar.gz` & `tmp/rmmbr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmmbr-0.0.8.tar", last modified: Fri May 26 10:28:25 2023, max compression
+gzip compressed data, was "rmmbr-0.0.9.tar", last modified: Thu Jun 22 08:59:31 2023, max compression
```

## Comparing `rmmbr-0.0.8.tar` & `rmmbr-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:28:25.170658 rmmbr-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-26 10:28:25.170658 rmmbr-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:28:25.170658 rmmbr-0.0.8/rmmbr/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:28:25.170658 rmmbr-0.0.8/rmmbr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:28:25.170658 rmmbr-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-26 10:28:15.000000 rmmbr-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:59:31.061777 rmmbr-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-22 08:59:31.061777 rmmbr-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:59:31.057777 rmmbr-0.0.9/rmmbr/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 08:59:23.000000 rmmbr-0.0.9/rmmbr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-22 08:59:23.000000 rmmbr-0.0.9/rmmbr/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-06-22 08:59:23.000000 rmmbr-0.0.9/rmmbr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-22 08:59:23.000000 rmmbr-0.0.9/rmmbr/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-22 08:59:23.000000 rmmbr-0.0.9/rmmbr/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:59:31.061777 rmmbr-0.0.9/rmmbr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-22 08:59:31.000000 rmmbr-0.0.9/rmmbr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-22 08:59:31.000000 rmmbr-0.0.9/rmmbr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:59:31.000000 rmmbr-0.0.9/rmmbr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 08:59:31.000000 rmmbr-0.0.9/rmmbr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 08:59:31.000000 rmmbr-0.0.9/rmmbr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 08:59:31.000000 rmmbr-0.0.9/rmmbr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 08:59:31.061777 rmmbr-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-22 08:59:23.000000 rmmbr-0.0.9/setup.py
```

### Comparing `rmmbr-0.0.8/rmmbr/crypto.py` & `rmmbr-0.0.9/rmmbr/crypto.py`

 * *Files identical despite different names*

### Comparing `rmmbr-0.0.8/rmmbr/main.py` & `rmmbr-0.0.9/rmmbr/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 def _deserialize(s):
     return dict(json.loads(s))
 
 
 _cache_background_writes = set()
 
+
 def _abstract_cache_params(key, f, read, write):
     async def func(*args, **kwargs):
         key_result = key(*args, **kwargs)
         value = await read(key_result)
         if value is not None:
             return value
         y = await f(*args, **kwargs)
@@ -68,30 +69,18 @@
         _cache_background_writes.add(bg_write)
         bg_write.add_done_callback(_cache_background_writes.discard)
 
         return y
 
     return func
 
+
 def wait_all_writes():
     return asyncio.gather(*_cache_background_writes, return_exceptions=True)
 
-def mem_cache(f):
-    cache = {}
-
-    async def func(*args, **kwargs):
-        key_result = _key_arguments(*args, **kwargs)
-        if key_result in cache:
-            return cache[key_result]
-        y = await f(*args, **kwargs)
-        cache[key_result] = y
-        return y
-
-    return func
-
 
 def _make_local_read_write(name: str):
     def default_f():
         return _serialize({})
 
     file_path = _path_to_cache(name)
     cache = None
@@ -110,16 +99,16 @@
         cache = await get_cache()
         cache[key] = value
         await _write_string_to_file(file_path, _serialize(cache))
 
     return read, write
 
 
-def local_cache(id: str):
-    read, write = _make_local_read_write(id)
+def _local_cache(cache_id: str):
+    read, write = _make_local_read_write(cache_id)
     return lambda f: _abstract_cache_params(_key_arguments, f, read, write)
 
 
 class RmmbrAuthError(Exception):
     pass
 
 
@@ -182,21 +171,23 @@
     return encrypt(encryptor, serialize_output(output))
 
 
 def _decrypt_and_deserialize_output(encryptor: Encryptor, data: str) -> Serializable:
     return deserialize_output(decrypt(encryptor, data))
 
 
-def cloud_cache(
-    url: str,
-    token: str,
+def cache(
     cache_id: str,
     ttl: Optional[int],
     encryption_key: Optional[str],
+    url: Optional[str],
+    token: Optional[str],
 ):
+    if not token or not url:
+        return _local_cache(cache_id)
     if encryption_key is not None:
         encryptor = encryptor_from_key(encryption_key.encode())
         key_arguments_func = partial(_private_key_arguments, encryption_key.encode())
         serialize_output_func = partial(_serialize_and_encrypt_output, encryptor)
         deserialize_output_func = partial(_decrypt_and_deserialize_output, encryptor)
 
     else:
```

### Comparing `rmmbr-0.0.8/rmmbr/main_test.py` & `rmmbr-0.0.9/rmmbr/main_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import pathlib
 
 import dotenv
 import redis.asyncio as redis
 
-from rmmbr import cloud_cache, local_cache, mem_cache, wait_all_writes
+from rmmbr import cache, wait_all_writes
 
 
 def _cache_test_helper(instance_implies_new_cache: bool, expires_after_2_seconds: bool):
     async def inner(cacher):
         n_called = 0
 
         async def f(x):
@@ -42,23 +42,18 @@
             _rmdir(item)
         else:
             item.unlink()
     directory.rmdir()
 
 
 async def test_local_cache():
-    cacher = local_cache("some-id")
-    await _cache_test_helper(False, False)(cacher)
+    await _cache_test_helper(False, False)(cache("some-id", None, None, None, None))
     _rmdir("./.rmmbr")
 
 
-async def test_memory_cache():
-    await _cache_test_helper(True, False)(mem_cache)
-
-
 def _env_param(s: str) -> str:
     value = dotenv.dotenv_values(".env")[s]
     assert value
     return value
 
 
 async def _clean_redis():
@@ -74,29 +69,35 @@
 _port = _env_param("PORT")
 _mock_backend_url = f"http://localhost:{_port}"
 
 
 async def test_cloud_cache():
     await _clean_redis()
     await _cache_test_helper(False, False)(
-        cloud_cache(_mock_backend_url, "some-token", "my_function_name", None, None)
+        cache(
+            "my_function_name",
+            None,
+            None,
+            _mock_backend_url,
+            "some-token",
+        )
     )
 
 
 async def test_cloud_cache_expiration():
     await _clean_redis()
     await _cache_test_helper(False, True)(
-        cloud_cache(_mock_backend_url, "some-token", "my_function_name", 1, None)
+        cache("my_function_name", 1, None, _mock_backend_url, "some-token")
     )
 
 
 async def test_cloud_cache_encryption():
     await _clean_redis()
     await _cache_test_helper(False, False)(
-        cloud_cache(
-            _mock_backend_url,
-            "some-token",
+        cache(
             "my_function_name",
             None,
             "Cqq33cbHu9AEUaP_wS3LCDQN7wy40XKWzALoPHbU5S8=",
+            _mock_backend_url,
+            "some-token",
         )
     )
```

### Comparing `rmmbr-0.0.8/setup.py` & `rmmbr-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 _repo_dir = os.environ.get("GITHUB_WORKSPACE")
 assert _repo_dir
 setup(
     name="rmmbr",
-    version="0.0.8",
+    version="0.0.9",
     description="Simple persistent caching.",
     long_description=(pathlib.Path(_repo_dir) / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/uriva/rmmbr",
     packages=find_packages(),
     install_requires=[
         "redis>=3.5.3",
```

