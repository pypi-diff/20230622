# Comparing `tmp/scPANTHEON-0.3.1.tar.gz` & `tmp/scPANTHEON-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.3.1.tar", last modified: Thu Jun 22 15:04:34 2023, max compression
+gzip compressed data, was "scPANTHEON-0.3.2.tar", last modified: Thu Jun 22 15:09:25 2023, max compression
```

## Comparing `scPANTHEON-0.3.1.tar` & `scPANTHEON-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 15:04:34.625556 scPANTHEON-0.3.1/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-06-22 15:04:34.624454 scPANTHEON-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 15:04:34.611640 scPANTHEON-0.3.1/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      261 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 15:04:34.000000 scPANTHEON-0.3.1/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 15:04:34.623400 scPANTHEON-0.3.1/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.3.1/scpantheon/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-06-08 07:21:40.000000 scPANTHEON-0.3.1/scpantheon/bokeh_qt.py
--rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.3.1/scpantheon/data_qt.py
--rw-rw-rw-   0        0        0     1122 2023-05-18 11:21:14.000000 scPANTHEON-0.3.1/scpantheon/main.py
--rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.3.1/scpantheon/qt.py
--rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.3.1/scpantheon/run.py
--rw-rw-rw-   0        0        0     3270 2023-05-12 02:45:41.000000 scPANTHEON-0.3.1/scpantheon/save_qt.py
--rw-rw-rw-   0        0        0    60638 2023-06-22 14:44:00.000000 scPANTHEON-0.3.1/scpantheon/source.py
--rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.3.1/scpantheon/transform.py
--rw-rw-rw-   0        0        0       42 2023-06-22 15:04:34.625556 scPANTHEON-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-06-22 15:04:19.000000 scPANTHEON-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 15:09:25.516600 scPANTHEON-0.3.2/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-06-22 15:09:25.516600 scPANTHEON-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 15:09:25.503556 scPANTHEON-0.3.2/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-22 15:09:25.000000 scPANTHEON-0.3.2/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 15:09:25.515600 scPANTHEON-0.3.2/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.3.2/scpantheon/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-06-08 07:21:40.000000 scPANTHEON-0.3.2/scpantheon/bokeh_qt.py
+-rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.3.2/scpantheon/data_qt.py
+-rw-rw-rw-   0        0        0     1154 2023-06-22 15:08:18.000000 scPANTHEON-0.3.2/scpantheon/main.py
+-rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.3.2/scpantheon/qt.py
+-rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.3.2/scpantheon/run.py
+-rw-rw-rw-   0        0        0     3270 2023-05-12 02:45:41.000000 scPANTHEON-0.3.2/scpantheon/save_qt.py
+-rw-rw-rw-   0        0        0    60638 2023-06-22 14:44:00.000000 scPANTHEON-0.3.2/scpantheon/source.py
+-rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.3.2/scpantheon/transform.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 15:09:25.516600 scPANTHEON-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-06-22 15:08:50.000000 scPANTHEON-0.3.2/setup.py
```

### Comparing `scPANTHEON-0.3.1/scpantheon/bokeh_qt.py` & `scPANTHEON-0.3.2/scpantheon/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.1/scpantheon/data_qt.py` & `scPANTHEON-0.3.2/scpantheon/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.1/scpantheon/main.py` & `scPANTHEON-0.3.2/scpantheon/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 import warnings
 
 from bokeh.server.server import Server
 import multiprocessing
 import warnings
 
-import bokeh_qt, data_qt
+from scpantheon import bokeh_qt, data_qt
 
 class InstallWarning(Warning):
     def __init__(self, message):
         self.message = message
     def __str__(self):
         return repr(self.message)
 
 try: 
-    import source # import from online
+    from scpantheon import source # import from online
 except:
     warnings.warn('YOU HAVE TO INSTALL PyQt5',InstallWarning)
 
 def run():
     global server
     print('Opening Bokeh application on http://localhost:5006/')
     server = Server({'/': source.main},
```

### Comparing `scPANTHEON-0.3.1/scpantheon/qt.py` & `scPANTHEON-0.3.2/scpantheon/qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.1/scpantheon/save_qt.py` & `scPANTHEON-0.3.2/scpantheon/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.1/scpantheon/source.py` & `scPANTHEON-0.3.2/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.1/scpantheon/transform.py` & `scPANTHEON-0.3.2/scpantheon/transform.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.1/setup.py` & `scPANTHEON-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.3.1',#版本
+    version='0.3.2',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh==2.4.3','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
                         'appdirs==1.4.4'], # 依赖包,如果没有,可以不要
```

