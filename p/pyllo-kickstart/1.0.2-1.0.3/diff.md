# Comparing `tmp/pyllo-kickstart-1.0.2.tar.gz` & `tmp/pyllo-kickstart-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllo-kickstart-1.0.2.tar", last modified: Thu Jun 22 06:43:22 2023, max compression
+gzip compressed data, was "pyllo-kickstart-1.0.3.tar", last modified: Thu Jun 22 06:50:44 2023, max compression
```

## Comparing `pyllo-kickstart-1.0.2.tar` & `pyllo-kickstart-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.478178 pyllo-kickstart-1.0.2/
--rw-r--r--   0 jane       (501) staff       (20)     9495 2022-06-05 08:31:40.000000 pyllo-kickstart-1.0.2/LICENSE.txt
--rw-r--r--   0 jane       (501) staff       (20)     5648 2023-06-22 06:43:22.478019 pyllo-kickstart-1.0.2/PKG-INFO
--rw-r--r--   0 jane       (501) staff       (20)     4879 2023-06-22 05:32:07.000000 pyllo-kickstart-1.0.2/README.md
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.474452 pyllo-kickstart-1.0.2/pyllo_kickstart/
--rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 12:02:08.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/__init__.py
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.475403 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/
--rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 13:07:30.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/__init__.py
--rw-r--r--   0 jane       (501) staff       (20)      222 2023-06-12 07:58:03.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/cookiecutter.json
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.475723 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/
--rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 06:09:44.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0 jane       (501) staff       (20)     3056 2023-06-07 05:51:11.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/setup.py
--rw-r--r--   0 jane       (501) staff       (20)      331 2023-06-07 05:58:32.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/startup.py
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.476380 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/
--rw-r--r--   0 jane       (501) staff       (20)       99 2022-04-17 07:23:59.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0 jane       (501) staff       (20)      297 2022-10-24 05:29:52.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/api.py
--rw-r--r--   0 jane       (501) staff       (20)     2018 2023-06-07 06:30:19.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/confpage.py
--rw-r--r--   0 jane       (501) staff       (20)     3128 2023-06-13 04:32:46.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/plugin.py
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.476638 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/widgets/
--rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 06:09:44.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/widgets/__init__.py
--rw-r--r--   0 jane       (501) staff       (20)     2015 2023-06-07 08:15:43.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/widgets/mainwidget.py
--rw-r--r--   0 jane       (501) staff       (20)     3722 2023-06-22 03:57:05.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/main.py
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.476852 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/
--rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 13:07:31.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/__init__.py
--rw-r--r--   0 jane       (501) staff       (20)      222 2023-06-12 07:57:16.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/cookiecutter.json
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.477201 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/
--rw-r--r--   0 jane       (501) staff       (20)       81 2023-06-07 05:50:57.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0 jane       (501) staff       (20)     3056 2023-06-07 05:51:11.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/setup.py
--rw-r--r--   0 jane       (501) staff       (20)      331 2023-06-07 05:58:32.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/startup.py
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.477823 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/
--rw-r--r--   0 jane       (501) staff       (20)       99 2022-04-17 07:23:59.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0 jane       (501) staff       (20)      297 2022-10-24 05:29:52.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/api.py
--rw-r--r--   0 jane       (501) staff       (20)     2018 2023-06-07 05:19:43.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/confpage.py
--rw-r--r--   0 jane       (501) staff       (20)     1330 2023-06-07 05:17:29.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/container.py
--rw-r--r--   0 jane       (501) staff       (20)     3093 2023-06-13 04:33:10.000000 pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/plugin.py
-drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:43:22.475195 pyllo-kickstart-1.0.2/pyllo_kickstart.egg-info/
--rw-r--r--   0 jane       (501) staff       (20)     5648 2023-06-22 06:43:22.000000 pyllo-kickstart-1.0.2/pyllo_kickstart.egg-info/PKG-INFO
--rw-r--r--   0 jane       (501) staff       (20)     1990 2023-06-22 06:43:22.000000 pyllo-kickstart-1.0.2/pyllo_kickstart.egg-info/SOURCES.txt
--rw-r--r--   0 jane       (501) staff       (20)        1 2023-06-22 06:43:22.000000 pyllo-kickstart-1.0.2/pyllo_kickstart.egg-info/dependency_links.txt
--rw-r--r--   0 jane       (501) staff       (20)       62 2023-06-22 06:43:22.000000 pyllo-kickstart-1.0.2/pyllo_kickstart.egg-info/entry_points.txt
--rw-r--r--   0 jane       (501) staff       (20)       56 2023-06-22 06:43:22.000000 pyllo-kickstart-1.0.2/pyllo_kickstart.egg-info/requires.txt
--rw-r--r--   0 jane       (501) staff       (20)       16 2023-06-22 06:43:22.000000 pyllo-kickstart-1.0.2/pyllo_kickstart.egg-info/top_level.txt
--rw-r--r--   0 jane       (501) staff       (20)       38 2023-06-22 06:43:22.478226 pyllo-kickstart-1.0.2/setup.cfg
--rw-r--r--   0 jane       (501) staff       (20)     3273 2023-06-22 06:42:23.000000 pyllo-kickstart-1.0.2/setup.py
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.102392 pyllo-kickstart-1.0.3/
+-rw-r--r--   0 jane       (501) staff       (20)     9495 2022-06-05 08:31:40.000000 pyllo-kickstart-1.0.3/LICENSE.txt
+-rw-r--r--   0 jane       (501) staff       (20)     5648 2023-06-22 06:50:44.102215 pyllo-kickstart-1.0.3/PKG-INFO
+-rw-r--r--   0 jane       (501) staff       (20)     4879 2023-06-22 05:32:07.000000 pyllo-kickstart-1.0.3/README.md
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.098490 pyllo-kickstart-1.0.3/pyllo_kickstart/
+-rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 12:02:08.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/__init__.py
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.099751 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/
+-rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 13:07:30.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/__init__.py
+-rw-r--r--   0 jane       (501) staff       (20)      222 2023-06-12 07:58:03.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/cookiecutter.json
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.100158 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/
+-rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 06:09:44.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0 jane       (501) staff       (20)     3056 2023-06-07 05:51:11.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/setup.py
+-rw-r--r--   0 jane       (501) staff       (20)      331 2023-06-07 05:58:32.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/startup.py
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.100658 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/
+-rw-r--r--   0 jane       (501) staff       (20)       99 2022-04-17 07:23:59.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0 jane       (501) staff       (20)      297 2022-10-24 05:29:52.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/api.py
+-rw-r--r--   0 jane       (501) staff       (20)     2018 2023-06-07 06:30:19.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/confpage.py
+-rw-r--r--   0 jane       (501) staff       (20)     3128 2023-06-13 04:32:46.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/plugin.py
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.100879 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/widgets/
+-rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 06:09:44.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/widgets/__init__.py
+-rw-r--r--   0 jane       (501) staff       (20)     2015 2023-06-07 08:15:43.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/widgets/mainwidget.py
+-rw-r--r--   0 jane       (501) staff       (20)     3722 2023-06-22 03:57:05.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/main.py
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.101090 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/
+-rw-r--r--   0 jane       (501) staff       (20)        0 2023-06-07 13:07:31.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/__init__.py
+-rw-r--r--   0 jane       (501) staff       (20)      222 2023-06-12 07:57:16.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/cookiecutter.json
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.101440 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/
+-rw-r--r--   0 jane       (501) staff       (20)       81 2023-06-07 05:50:57.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0 jane       (501) staff       (20)     3056 2023-06-07 05:51:11.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/setup.py
+-rw-r--r--   0 jane       (501) staff       (20)      331 2023-06-07 05:58:32.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/startup.py
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.102016 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/
+-rw-r--r--   0 jane       (501) staff       (20)       99 2022-04-17 07:23:59.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0 jane       (501) staff       (20)      297 2022-10-24 05:29:52.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/api.py
+-rw-r--r--   0 jane       (501) staff       (20)     2018 2023-06-07 05:19:43.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/confpage.py
+-rw-r--r--   0 jane       (501) staff       (20)     1330 2023-06-07 05:17:29.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/container.py
+-rw-r--r--   0 jane       (501) staff       (20)     3093 2023-06-13 04:33:10.000000 pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/plugin.py
+drwxr-xr-x   0 jane       (501) staff       (20)        0 2023-06-22 06:50:44.099463 pyllo-kickstart-1.0.3/pyllo_kickstart.egg-info/
+-rw-r--r--   0 jane       (501) staff       (20)     5648 2023-06-22 06:50:43.000000 pyllo-kickstart-1.0.3/pyllo_kickstart.egg-info/PKG-INFO
+-rw-r--r--   0 jane       (501) staff       (20)     1990 2023-06-22 06:50:44.000000 pyllo-kickstart-1.0.3/pyllo_kickstart.egg-info/SOURCES.txt
+-rw-r--r--   0 jane       (501) staff       (20)        1 2023-06-22 06:50:43.000000 pyllo-kickstart-1.0.3/pyllo_kickstart.egg-info/dependency_links.txt
+-rw-r--r--   0 jane       (501) staff       (20)       62 2023-06-22 06:50:43.000000 pyllo-kickstart-1.0.3/pyllo_kickstart.egg-info/entry_points.txt
+-rw-r--r--   0 jane       (501) staff       (20)       76 2023-06-22 06:50:43.000000 pyllo-kickstart-1.0.3/pyllo_kickstart.egg-info/requires.txt
+-rw-r--r--   0 jane       (501) staff       (20)       16 2023-06-22 06:50:44.000000 pyllo-kickstart-1.0.3/pyllo_kickstart.egg-info/top_level.txt
+-rw-r--r--   0 jane       (501) staff       (20)       38 2023-06-22 06:50:44.102442 pyllo-kickstart-1.0.3/setup.cfg
+-rw-r--r--   0 jane       (501) staff       (20)     3300 2023-06-22 06:49:19.000000 pyllo-kickstart-1.0.3/setup.py
```

### Comparing `pyllo-kickstart-1.0.2/LICENSE.txt` & `pyllo-kickstart-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/PKG-INFO` & `pyllo-kickstart-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllo-kickstart
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pyllo plugin generator
 Home-page: 
 Author: Shanghai Connet Information Technology Company Ltd.
 Author-email: tech_support@shconnet.com.cn
 License: UNKNOWN
 Keywords: pyllo plugin template generator
 Platform: UNKNOWN
```

### Comparing `pyllo-kickstart-1.0.2/README.md` & `pyllo-kickstart-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/setup.py` & `pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/setup.py`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/confpage.py` & `pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/confpage.py`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/plugin.py` & `pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/plugin.py`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/widgets/mainwidget.py` & `pyllo-kickstart-1.0.3/pyllo_kickstart/dockableplugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/widgets/mainwidget.py`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart/main.py` & `pyllo-kickstart-1.0.3/pyllo_kickstart/main.py`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/setup.py` & `pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/setup.py`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/confpage.py` & `pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/confpage.py`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/container.py` & `pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/container.py`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/plugin.py` & `pyllo-kickstart-1.0.3/pyllo_kickstart/plugin/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/plugin.py`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart.egg-info/PKG-INFO` & `pyllo-kickstart-1.0.3/pyllo_kickstart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllo-kickstart
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pyllo plugin generator
 Home-page: 
 Author: Shanghai Connet Information Technology Company Ltd.
 Author-email: tech_support@shconnet.com.cn
 License: UNKNOWN
 Keywords: pyllo plugin template generator
 Platform: UNKNOWN
```

### Comparing `pyllo-kickstart-1.0.2/pyllo_kickstart.egg-info/SOURCES.txt` & `pyllo-kickstart-1.0.3/pyllo_kickstart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllo-kickstart-1.0.2/setup.py` & `pyllo-kickstart-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,26 +54,27 @@
 # Files added to the package
 # =============================================================================
 EXTLIST = ['.json', '.py']
 
 
 install_requires = [
     "pyllo>=1.0.0.dev0",
-    "rich==13.3.5"
+    "rich==13.3.5",
+    "cookiecutter==2.1.1"
 ]
 
 if sys.platform == "darwin":
     install_requires += [
         'applaunchservices==0.3.0'
     ]
 
 
 setup(
     name=NAME,
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     package_data={LIBNAME: get_package_data(LIBNAME, EXTLIST)},
     entry_points={
         'console_scripts': [
             'pyllo-kickstart=pyllo_kickstart.main:main',
         ]
     },
```

