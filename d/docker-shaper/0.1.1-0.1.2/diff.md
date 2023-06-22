# Comparing `tmp/docker_shaper-0.1.1.tar.gz` & `tmp/docker_shaper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.1.tar", max compression
+gzip compressed data, was "docker_shaper-0.1.2.tar", max compression
```

## Comparing `docker_shaper-0.1.1.tar` & `docker_shaper-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     2052 2023-06-22 09:48:36.723418 docker_shaper-0.1.1/Readme.md
--rw-r--r--   0        0        0        0 2023-06-22 08:21:29.063512 docker_shaper-0.1.1/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0      905 2023-06-22 08:52:26.423436 docker_shaper-0.1.1/docker_shaper/cli.py
--rw-r--r--   0        0        0        0 2023-06-22 08:30:25.674562 docker_shaper-0.1.1/docker_shaper/common.py
--rw-r--r--   0        0        0      107 2023-06-22 08:41:33.292047 docker_shaper-0.1.1/docker_shaper/dynamic.py
--rw-r--r--   0        0        0     1079 2023-06-22 09:48:00.959480 docker_shaper-0.1.1/docker_shaper/server.py
--rw-r--r--   0        0        0      149 2023-06-22 09:02:28.913379 docker_shaper-0.1.1/docker_shaper/templates/result.html
--rw-r--r--   0        0        0     3105 2023-06-22 09:47:12.279585 docker_shaper-0.1.1/docker_shaper/utils.py
--rw-r--r--   0        0        0     2171 2023-06-22 09:49:41.491335 docker_shaper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 docker_shaper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2140 2023-06-22 11:46:34.742492 docker_shaper-0.1.2/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-22 08:21:29.063512 docker_shaper-0.1.2/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1459 2023-06-22 14:10:38.638778 docker_shaper-0.1.2/docker_shaper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-22 08:30:25.674562 docker_shaper-0.1.2/docker_shaper/common.py
+-rw-r--r--   0        0        0     2502 2023-06-22 15:03:04.151806 docker_shaper-0.1.2/docker_shaper/docker_stuff.py
+-rw-r--r--   0        0        0     3977 2023-06-22 13:56:29.288322 docker_shaper-0.1.2/docker_shaper/dynamic.py
+-rw-r--r--   0        0        0     8379 2023-06-22 15:03:04.195806 docker_shaper-0.1.2/docker_shaper/server.py
+-rw-r--r--   0        0        0      149 2023-06-22 09:02:28.913379 docker_shaper-0.1.2/docker_shaper/templates/result.html
+-rw-r--r--   0        0        0     4907 2023-06-22 15:03:03.603804 docker_shaper-0.1.2/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2171 2023-06-22 15:05:30.024252 docker_shaper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 docker_shaper-0.1.2/PKG-INFO
```

### Comparing `docker_shaper-0.1.1/Readme.md` & `docker_shaper-0.1.2/Readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # Docker Shaper
 
 This repository includes scripts/tools for Checkmk developers.
 
 ## Installation
 
 ```sh
-[<PYTHON> -m] pip[3] install [--upgrade] docker-shaper
+[<PYTHON> -m] pip[3] install [--user] [--upgrade] docker-shaper
 ```
 
 ## Usage
 
-
-**`--log-level`**
-
-Provide a Python `logging` level name, e.g. `DEBUG` (case-insensitive)
+```
+docker-shaper serve`
+```
+Navigate to e.g. http://build-fra-003:5432/
 
 
 ## Development & Contribution
 
 ### Todo
 
-- [ ] pip package
+- [x] pip package
+- [x] quart interface
+- [ ] increase/decrease logging
+- [ ] bring in dgcd
+- [ ] untag certain tags
 - [ ] outsource config
-- [ ] list_volumes
-- [ ] container cleanup
+- [ ] bring in list_volumes
 - [ ] dockermon
-- [ ] increase/decrease logging
+- [ ] container cleanup
 - [ ] Quart interface
 
 
 ### Setup
 
 ### Prerequisites
 
@@ -68,15 +71,15 @@
 poetry build && \
 twine check dist/* &&
 python3 -m pip uninstall -y checkmk_dev_tools && \
 python3 -m pip install --user dist/checkmk_dev_tools-$(grep -E "^version.?=" pyproject.toml | cut -d '"' -f 2)-py3-none-any.whl
 ```
   - check installed package
   - go through review process
-  - publish the new package `poetry publish --build`
+  - publish the new package `poetry publish --build --repository checkmk`
   - commit new version && push
 
 
 ## Knowledge
 
 * https://blog.miguelgrinberg.com/post/beautiful-interactive-tables-for-your-flask-templates
 * https://stackoverflow.com/questions/49957034/live-updating-dynamic-variable-on-html-with-flask
```

### Comparing `docker_shaper-0.1.1/pyproject.toml` & `docker_shaper-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.1"
+version = "0.1.2"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
   {include = "docker_shaper/**/*.html"},
```

### Comparing `docker_shaper-0.1.1/PKG-INFO` & `docker_shaper-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 0.1.1
+Version: 0.1.2
 Summary: Keeps Docker resources in shape based on rules and usage
 Home-page: https://github.com/Checkmk/checkmk-dev-tools
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -19,35 +19,38 @@
 # Docker Shaper
 
 This repository includes scripts/tools for Checkmk developers.
 
 ## Installation
 
 ```sh
-[<PYTHON> -m] pip[3] install [--upgrade] docker-shaper
+[<PYTHON> -m] pip[3] install [--user] [--upgrade] docker-shaper
 ```
 
 ## Usage
 
-
-**`--log-level`**
-
-Provide a Python `logging` level name, e.g. `DEBUG` (case-insensitive)
+```
+docker-shaper serve`
+```
+Navigate to e.g. http://build-fra-003:5432/
 
 
 ## Development & Contribution
 
 ### Todo
 
-- [ ] pip package
+- [x] pip package
+- [x] quart interface
+- [ ] increase/decrease logging
+- [ ] bring in dgcd
+- [ ] untag certain tags
 - [ ] outsource config
-- [ ] list_volumes
-- [ ] container cleanup
+- [ ] bring in list_volumes
 - [ ] dockermon
-- [ ] increase/decrease logging
+- [ ] container cleanup
 - [ ] Quart interface
 
 
 ### Setup
 
 ### Prerequisites
 
@@ -86,15 +89,15 @@
 poetry build && \
 twine check dist/* &&
 python3 -m pip uninstall -y checkmk_dev_tools && \
 python3 -m pip install --user dist/checkmk_dev_tools-$(grep -E "^version.?=" pyproject.toml | cut -d '"' -f 2)-py3-none-any.whl
 ```
   - check installed package
   - go through review process
-  - publish the new package `poetry publish --build`
+  - publish the new package `poetry publish --build --repository checkmk`
   - commit new version && push
 
 
 ## Knowledge
 
 * https://blog.miguelgrinberg.com/post/beautiful-interactive-tables-for-your-flask-templates
 * https://stackoverflow.com/questions/49957034/live-updating-dynamic-variable-on-html-with-flask
```

