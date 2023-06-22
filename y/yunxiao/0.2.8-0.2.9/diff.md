# Comparing `tmp/yunxiao-0.2.8.tar.gz` & `tmp/yunxiao-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.2.8.tar", last modified: Thu Jun 15 05:57:02 2023, max compression
+gzip compressed data, was "yunxiao-0.2.9.tar", last modified: Thu Jun 22 17:41:19 2023, max compression
```

## Comparing `yunxiao-0.2.8.tar` & `yunxiao-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 05:57:02.733653 yunxiao-0.2.8/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.8/LICENSE
--rw-rw-rw-   0        0        0    12954 2023-06-15 05:57:02.732643 yunxiao-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.8/README.md
--rw-rw-rw-   0        0        0     1250 2023-06-15 05:56:45.000000 yunxiao-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 05:57:02.733653 yunxiao-0.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 05:57:02.720496 yunxiao-0.2.8/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.8/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:57:02.725569 yunxiao-0.2.8/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.8/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.8/yunxiao/app.py
--rw-rw-rw-   0        0        0    20799 2023-06-15 05:56:37.000000 yunxiao-0.2.8/yunxiao/v2.py
--rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.8/yunxiao/web.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.8/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:57:02.731632 yunxiao-0.2.8/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    12954 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 05:57:02.000000 yunxiao-0.2.8/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 17:41:19.360899 yunxiao-0.2.9/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     6351 2023-06-22 17:41:19.359861 yunxiao-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.2.9/README.md
+-rw-rw-rw-   0        0        0     1290 2023-06-22 17:41:06.000000 yunxiao-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 17:41:19.360899 yunxiao-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 17:41:19.351755 yunxiao-0.2.9/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.9/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:41:19.354291 yunxiao-0.2.9/yunxiao/
+-rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.2.9/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    32806 2023-06-22 17:34:42.000000 yunxiao-0.2.9/yunxiao/v2.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.9/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:41:19.358848 yunxiao-0.2.9/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     6351 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 17:41:19.000000 yunxiao-0.2.9/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.2.8/LICENSE` & `yunxiao-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.8/pyproject.toml` & `yunxiao-0.2.9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.2.8"
+version = "0.2.9"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,14 +22,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.2.9" = "删除其他，只使用V2"
 "0.2.6" = "V2 中更多使用分片读取。"
 "0.2.5" = "修复 V2 中的 API端点错误。新增 loop 装饰器便于分片提取大量数据。"
 "0.2.4" = "修复 v2 中一个API端点错误及鉴权更新错误"
 "0.2.2" = "新增 v2, 更清晰的函数命名，简洁快速的拉取全部数据。"
 "0.2.1" = "web 端请求 BUG 修复"
 "0.2.0" = "BUG修复"
 "0.1.9" = "更改鉴权方式，保存鉴权到系统环境变量。当因鉴权失效导致请求失败时，自动更新鉴权并重新发起请求。意图减少更新鉴权的次数。"
```

### Comparing `yunxiao-0.2.8/yunxiao/yunxiao.py` & `yunxiao-0.2.9/yunxiao/yunxiao.py`

 * *Files identical despite different names*

