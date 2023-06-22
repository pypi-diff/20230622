# Comparing `tmp/docker_shaper-0.1.0.tar.gz` & `tmp/docker_shaper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.0.tar", max compression
+gzip compressed data, was "docker_shaper-0.1.1.tar", max compression
```

## Comparing `docker_shaper-0.1.0.tar` & `docker_shaper-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1850 2023-06-22 09:03:14.437565 docker_shaper-0.1.0/Readme.md
--rw-r--r--   0        0        0        0 2023-06-22 08:21:29.063512 docker_shaper-0.1.0/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0      905 2023-06-22 08:52:26.423436 docker_shaper-0.1.0/docker_shaper/cli.py
--rw-r--r--   0        0        0        0 2023-06-22 08:30:25.674562 docker_shaper-0.1.0/docker_shaper/common.py
--rw-r--r--   0        0        0      107 2023-06-22 08:41:33.292047 docker_shaper-0.1.0/docker_shaper/dynamic.py
--rw-r--r--   0        0        0     1081 2023-06-22 09:00:49.308987 docker_shaper-0.1.0/docker_shaper/server.py
--rw-r--r--   0        0        0      149 2023-06-22 09:02:28.913379 docker_shaper-0.1.0/docker_shaper/templates/result.html
--rw-r--r--   0        0        0     3209 2023-06-22 08:33:31.403730 docker_shaper-0.1.0/docker_shaper/utils.py
--rw-r--r--   0        0        0     2171 2023-06-22 09:08:22.686895 docker_shaper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 docker_shaper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2052 2023-06-22 09:48:36.723418 docker_shaper-0.1.1/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-22 08:21:29.063512 docker_shaper-0.1.1/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0      905 2023-06-22 08:52:26.423436 docker_shaper-0.1.1/docker_shaper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-22 08:30:25.674562 docker_shaper-0.1.1/docker_shaper/common.py
+-rw-r--r--   0        0        0      107 2023-06-22 08:41:33.292047 docker_shaper-0.1.1/docker_shaper/dynamic.py
+-rw-r--r--   0        0        0     1079 2023-06-22 09:48:00.959480 docker_shaper-0.1.1/docker_shaper/server.py
+-rw-r--r--   0        0        0      149 2023-06-22 09:02:28.913379 docker_shaper-0.1.1/docker_shaper/templates/result.html
+-rw-r--r--   0        0        0     3105 2023-06-22 09:47:12.279585 docker_shaper-0.1.1/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2171 2023-06-22 09:49:41.491335 docker_shaper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 docker_shaper-0.1.1/PKG-INFO
```

### Comparing `docker_shaper-0.1.0/Readme.md` & `docker_shaper-0.1.1/Readme.md`

 * *Files 13% similar despite different names*

```diff
@@ -27,27 +27,39 @@
 - [ ] dockermon
 - [ ] increase/decrease logging
 - [ ] Quart interface
 
 
 ### Setup
 
-For active development you need to have `poetry` and `pre-commit` installed
+### Prerequisites
+
+* Python 3.8.10
+* `poetry`
+* `pre-commit`
+
 
 ```sh
 python3 -m pip install --upgrade --user poetry pre-commit
 git clone ssh://review.lan.tribe29.com:29418/checkmk_ci
 cd checkmk_ci
 pre-commit install
 # if you need a specific version of Python inside your dev environment
-poetry env use ~/.pyenv/versions/3.10.4/bin/python3
+poetry env use ~/.pyenv/versions/3.8.10/bin/python3
 poetry install
 ```
 
 ### Workflow
+poetry config repositories.checkmk https://upload.pypi.org/legacy/
+poetry config pypi-token.checkmk pypi-
+
+pip3 install --user --upgrade docker-shaper
+~/.local/bin/docker-shaper server
+
+poetry run mypy docker_shaper
 
 * (once and only for publishing to PyPi) Get token on PyPi.org
 * (once and only for publishing to PyPi) `poetry config pypi-token.pypi pypi-<LONG-STRING>`
   (will write to `~/.config/pypoetry/auth.toml`)
 * modify and check commits via `pre-commit`
 * after work is done locally:
   - adapt version in `pyproject.toml`
```

### Comparing `docker_shaper-0.1.0/docker_shaper/cli.py` & `docker_shaper-0.1.1/docker_shaper/cli.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.0/docker_shaper/server.py` & `docker_shaper-0.1.1/docker_shaper/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,9 +48,9 @@
 
 def serve():
     app.terminator = asyncio.Event()
     app.run(
         host="0.0.0.0",
         port=5432,
         # debug=True,
-        # loop=asyncio.get_event_loop()
+        loop=asyncio.get_event_loop()
     )
```

### Comparing `docker_shaper-0.1.0/docker_shaper/utils.py` & `docker_shaper-0.1.1/docker_shaper/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 def log() -> logging.Logger:
     """Logger for this module"""
     return logging.getLogger("docker-shaper.utils")
 
 
 def watchdog(
-    afunc: Callable[..., Coroutine[object, object, object]]
-) -> Callable[..., Coroutine[object, object, object]]:
+    afunc: Callable
+) -> Callable:
     """Watch for async functions to throw an unhandled exception"""
 
     @wraps(afunc)
     async def run(*args: object, **kwargs: object) -> object:
         """Run wrapped function and handle exceptions"""
         try:
             return await afunc(*args, **kwargs)
@@ -38,17 +38,17 @@
 
     return run
 
 
 @watchdog
 async def watch_changes(
     path: Path,
-    callback: Callable[[set[Path]], None],
+    callback: Callable,
     *,
-    queue: asyncio.Queue[str] = asyncio.Queue(),
+    queue: asyncio.Queue = asyncio.Queue(),
     mask: Mask = Mask.CLOSE_WRITE | Mask.MOVED_TO | Mask.CREATE,
     postpone: bool = False,
     timeout: float = 2,
 ) -> None:
     """Controllable, timed filesystem watcher"""
 
     # pylint: disable=too-many-locals
```

### Comparing `docker_shaper-0.1.0/pyproject.toml` & `docker_shaper-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.0"
+version = "0.1.1"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
   {include = "docker_shaper/**/*.html"},
```

### Comparing `docker_shaper-0.1.0/PKG-INFO` & `docker_shaper-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Keeps Docker resources in shape based on rules and usage
 Home-page: https://github.com/Checkmk/checkmk-dev-tools
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -45,27 +45,39 @@
 - [ ] dockermon
 - [ ] increase/decrease logging
 - [ ] Quart interface
 
 
 ### Setup
 
-For active development you need to have `poetry` and `pre-commit` installed
+### Prerequisites
+
+* Python 3.8.10
+* `poetry`
+* `pre-commit`
+
 
 ```sh
 python3 -m pip install --upgrade --user poetry pre-commit
 git clone ssh://review.lan.tribe29.com:29418/checkmk_ci
 cd checkmk_ci
 pre-commit install
 # if you need a specific version of Python inside your dev environment
-poetry env use ~/.pyenv/versions/3.10.4/bin/python3
+poetry env use ~/.pyenv/versions/3.8.10/bin/python3
 poetry install
 ```
 
 ### Workflow
+poetry config repositories.checkmk https://upload.pypi.org/legacy/
+poetry config pypi-token.checkmk pypi-
+
+pip3 install --user --upgrade docker-shaper
+~/.local/bin/docker-shaper server
+
+poetry run mypy docker_shaper
 
 * (once and only for publishing to PyPi) Get token on PyPi.org
 * (once and only for publishing to PyPi) `poetry config pypi-token.pypi pypi-<LONG-STRING>`
   (will write to `~/.config/pypoetry/auth.toml`)
 * modify and check commits via `pre-commit`
 * after work is done locally:
   - adapt version in `pyproject.toml`
```

