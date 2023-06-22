# Comparing `tmp/ipyaladin-0.2.3.tar.gz` & `tmp/ipyaladin-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyaladin-0.2.3.tar", last modified: Tue May 30 12:09:04 2023, max compression
+gzip compressed data, was "ipyaladin-0.2.4.tar", last modified: Thu Jun 22 16:12:29 2023, max compression
```

## Comparing `ipyaladin-0.2.3.tar` & `ipyaladin-0.2.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.559184 ipyaladin-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-30 12:09:04.559184 ipyaladin-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/ipyaladin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/ipyaladin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/ipyaladin/aladin_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/563.9c25681782097966161a.js
--rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/590.b90399830948d2f839e2.js
--rw-r--r--   0 runner    (1001) docker     (123)    22071 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/remoteEntry.baf7991223a7feb4e9c0.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 12:09:01.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 12:08:50.000000 ipyaladin-0.2.3/ipyaladin/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-05-30 12:08:51.000000 ipyaladin-0.2.3/ipyaladin/nbextension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:08:38.000000 ipyaladin-0.2.3/ipyaladin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/ipyaladin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/js/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/amd-public-path.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/js/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-05-30 12:08:52.000000 ipyaladin-0.2.3/js/dist/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/js/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/lib/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/lib/jupyter-aladin.js
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/lib/labplugin.js
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)    82533 2023-05-30 12:08:48.000000 ipyaladin-0.2.3/js/yarn.lock
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-30 12:09:04.559184 ipyaladin-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/ipyaladin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/ipyaladin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/ipyaladin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/ipyaladin/aladin_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/ipyaladin/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-22 16:12:28.000000 ipyaladin-0.2.4/ipyaladin/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/ipyaladin/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-22 16:12:28.000000 ipyaladin-0.2.4/ipyaladin/labextension/static/563.e86cfcd7efe0f971a73e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27532 2023-06-22 16:12:28.000000 ipyaladin-0.2.4/ipyaladin/labextension/static/590.c686e7199dfcb1a5e45b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22071 2023-06-22 16:12:28.000000 ipyaladin-0.2.4/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-22 16:12:28.000000 ipyaladin-0.2.4/ipyaladin/labextension/static/remoteEntry.501d5d2382e909d58004.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-22 16:12:26.000000 ipyaladin-0.2.4/ipyaladin/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-22 16:12:28.000000 ipyaladin-0.2.4/ipyaladin/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/ipyaladin/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-22 16:12:14.000000 ipyaladin-0.2.4/ipyaladin/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27424 2023-06-22 16:12:16.000000 ipyaladin-0.2.4/ipyaladin/nbextension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/ipyaladin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-22 16:12:29.000000 ipyaladin-0.2.4/ipyaladin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-22 16:12:29.000000 ipyaladin-0.2.4/ipyaladin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:12:29.000000 ipyaladin-0.2.4/ipyaladin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:12:02.000000 ipyaladin-0.2.4/ipyaladin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 16:12:29.000000 ipyaladin-0.2.4/ipyaladin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 16:12:29.000000 ipyaladin-0.2.4/ipyaladin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/ipyaladin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/js/amd-public-path.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/js/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    27424 2023-06-22 16:12:16.000000 ipyaladin-0.2.4/js/dist/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:12:29.359444 ipyaladin-0.2.4/js/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/js/lib/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/js/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/js/lib/jupyter-aladin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/js/lib/labplugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/js/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/js/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)    82533 2023-06-22 16:12:12.000000 ipyaladin-0.2.4/js/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-22 16:12:29.363444 ipyaladin-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-22 16:11:37.000000 ipyaladin-0.2.4/setup.py
```

### Comparing `ipyaladin-0.2.3/LICENSE.md` & `ipyaladin-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/PKG-INFO` & `ipyaladin-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyaladin
-Version: 0.2.3
+Version: 0.2.4
 Summary: ipyaladin
 Home-page: https://github.com/cds-astro/ipyaladin
 Author: Jerome Desroziers, Thomas Boch & Matthieu Baumann
 Author-email: matthieu.baumann@astro.unistra.fr
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/cds-astro/ipyaladin/issues
 Project-URL: Live Testing, https://mybinder.org/v2/gh/cds-astro/ipyaladin/master
@@ -70,15 +70,15 @@
 And you are ready to use ipyaladin inside your notebooks!
 Additionny, for a jupyterlab usage you will need to:
 
     jupyter labextension develop ipyaladin --overwrite
 
 There is also a conda package that can be installed with:
 
-    conda install -c bmatthieu3 ipyaladin==0.2.3
+    conda install -c bmatthieu3 ipyaladin==0.2.4
 
 ## New features corner
 
 ![new_features](assets/new_features.gif)
 
 ## Development installation
```

### Comparing `ipyaladin-0.2.3/README.md` & `ipyaladin-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 And you are ready to use ipyaladin inside your notebooks!
 Additionny, for a jupyterlab usage you will need to:
 
     jupyter labextension develop ipyaladin --overwrite
 
 There is also a conda package that can be installed with:
 
-    conda install -c bmatthieu3 ipyaladin==0.2.3
+    conda install -c bmatthieu3 ipyaladin==0.2.4
 
 ## New features corner
 
 ![new_features](assets/new_features.gif)
 
 ## Development installation
```

### Comparing `ipyaladin-0.2.3/ipyaladin/__init__.py` & `ipyaladin-0.2.4/ipyaladin/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/ipyaladin/aladin_widget.py` & `ipyaladin-0.2.4/ipyaladin/aladin_widget.py`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/ipyaladin/labextension/package.json` & `ipyaladin-0.2.4/ipyaladin/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988839285714286%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.501d5d2382e909d58004.js'}}"}*

```diff
@@ -12,15 +12,15 @@
     },
     "files": [
         "dist/*.js"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.baf7991223a7feb4e9c0.js"
+            "load": "static/remoteEntry.501d5d2382e909d58004.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../ipyaladin/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
```

### Comparing `ipyaladin-0.2.3/ipyaladin/labextension/static/563.9c25681782097966161a.js` & `ipyaladin-0.2.4/ipyaladin/labextension/static/563.e86cfcd7efe0f971a73e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -32,16 +32,16 @@
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "AladinModel",
                         _view_name: "AladinView",
                         _model_module: "ipyaladin",
                         _view_module: "ipyaladin",
-                        _model_module_version: "0.2.3",
-                        _view_module_version: "0.2.3"
+                        _model_module_version: "0.2.4",
+                        _view_module_version: "0.2.4"
                     }
                 }
             }
             let h = 0;
             class d extends i.DOMWidgetView {
                 render() {
                     l.then((() => {
@@ -105,15 +105,15 @@
                         });
                         this.al.addCatalog(t), t.addSourcesAsArray(this.model.get("table_keys"), this.model.get("table_columns"))
                     }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (() => {
                         let t = A.graphicOverlay(this.model.get("overlay_options"));
                         this.al.addOverlay(t), t.addFootprints(A.footprintsFromSTCS(this.model.get("stc_string")))
                     }), this), this.listenTo(this.model, "change:listener_flag", (() => {
                         let t = this.model.get("listener_type");
-                        this.al.on(t, (function(e) {
+                        this.al.on(t, (e => {
                             if ("select" !== t) e && this.send({
                                 event: "callback",
                                 type: t,
                                 data: {
                                     data: e.data,
                                     dec: e.dec,
                                     ra: e.ra,
```

### Comparing `ipyaladin-0.2.3/ipyaladin/labextension/static/590.b90399830948d2f839e2.js` & `ipyaladin-0.2.4/ipyaladin/labextension/static/590.c686e7199dfcb1a5e45b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1410,16 +1410,16 @@
                         defaults() {
                             return {
                                 ...super.defaults(),
                                 _model_name: "AladinModel",
                                 _view_name: "AladinView",
                                 _model_module: "ipyaladin",
                                 _view_module: "ipyaladin",
-                                _model_module_version: "0.2.3",
-                                _view_module_version: "0.2.3"
+                                _model_module_version: "0.2.4",
+                                _view_module_version: "0.2.4"
                             }
                         }
                     }
                     let i = 0;
                     class u extends t.DOMWidgetView {
                         render() {
                             n.then((() => {
@@ -1483,15 +1483,15 @@
                                 });
                                 this.al.addCatalog(t), t.addSourcesAsArray(this.model.get("table_keys"), this.model.get("table_columns"))
                             }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (() => {
                                 let t = A.graphicOverlay(this.model.get("overlay_options"));
                                 this.al.addOverlay(t), t.addFootprints(A.footprintsFromSTCS(this.model.get("stc_string")))
                             }), this), this.listenTo(this.model, "change:listener_flag", (() => {
                                 let t = this.model.get("listener_type");
-                                this.al.on(t, (function(e) {
+                                this.al.on(t, (e => {
                                     if ("select" !== t) e && this.send({
                                         event: "callback",
                                         type: t,
                                         data: {
                                             data: e.data,
                                             dec: e.dec,
                                             ra: e.ra,
```

### Comparing `ipyaladin-0.2.3/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js` & `ipyaladin-0.2.4/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/ipyaladin/labextension/static/remoteEntry.baf7991223a7feb4e9c0.js` & `ipyaladin-0.2.4/ipyaladin/labextension/static/remoteEntry.501d5d2382e909d58004.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, l, u, d, s, f, c, p, h, v, b, g, m, y = {
+    var e, r, t, n, o, a, i, l, u, d, f, s, p, c, h, v, b, g, m, y = {
             460: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(672), t.e(590)]).then((() => () => t(590))),
                         "./extension": () => Promise.all([t.e(672), t.e(563)]).then((() => () => t(563)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         w = {};
 
     function S(e) {
         var r = w[e];
@@ -38,76 +38,76 @@
     }
     S.m = y, S.c = w, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        563: "9c25681782097966161a",
-        590: "b90399830948d2f839e2",
-        672: "d1c8706d8114ce8e432a",
+        563: "e86cfcd7efe0f971a73e",
+        590: "c686e7199dfcb1a5e45b",
+        672: "8fb04855ed1efc9fb044",
         794: "644314dbf6493c3f7619"
     } [e] + ".js?v=" + {
-        563: "9c25681782097966161a",
-        590: "b90399830948d2f839e2",
-        672: "d1c8706d8114ce8e432a",
+        563: "e86cfcd7efe0f971a73e",
+        590: "c686e7199dfcb1a5e45b",
+        672: "8fb04855ed1efc9fb044",
         794: "644314dbf6493c3f7619"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyaladin:", S.l = (t, n, a, o) => {
+    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyaladin:", S.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
-            if (void 0 !== a)
+            if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var s = u[d];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        i = s;
+                    var f = u[d];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var s = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, S.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         S.S = {};
         var e = {},
             r = {};
         S.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 S.o(S.S, t) || (S.S[t] = {});
-                var o = S.S[t],
+                var a = S.S[t],
                     i = "ipyaladin",
                     l = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            l = a[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
+                        var o = a[e] = a[e] || {},
+                            l = o[r];
+                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
                 return "default" === t && (l("ipyaladin", "0.2.3", (() => Promise.all([S.e(672), S.e(590)]).then((() => () => S(590))))), l("underscore", "1.13.6", (() => S.e(794).then((() => () => S(794)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
@@ -129,98 +129,98 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
             var i = r[n],
                 l = (typeof i)[0];
-            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var i = [];
-        for (o = 1; o < e.length; o++) {
-            var l = e[o];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
+        for (a = 1; a < e.length; a++) {
+            var l = e[a];
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
         }
         return u();
 
         function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+                o = n < 0;
+            o && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var d, s, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !u || ("u" == f ? l > n && !a : "" == f != a);
-                if ("u" == s) {
-                    if (!u || "u" != f) return !1
+                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == s ? l > n && !o : "" == s != o);
+                if ("u" == f) {
+                    if (!u || "u" != s) return !1
                 } else if (u)
-                    if (f == s)
+                    if (s == f)
                         if (l <= n) {
                             if (d != e[l]) return !1
                         } else {
-                            if (a ? d > e[l] : d < e[l]) return !1;
+                            if (o ? d > e[l] : d < e[l]) return !1;
                             d != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (a || l <= n) return !1;
+                else if ("s" != s && "n" != s) {
+                    if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < f != a) return !1;
+                    if (l <= n || f < s != o) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
-        var a = l(e, t);
-        return o(n, a) || f(u(e, t, a, n)), c(e[t][a])
-    }, s = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, f = e => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
+        var o = l(e, t);
+        return a(n, o) || s(u(e, t, o, n)), p(e[t][o])
+    }, f = (e, r, t) => {
+        var o = e[r];
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, a) {
-        var o = S.I(r);
-        return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, a)) : e(r, S.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), v = p(((e, r, t, n, a) => {
-        var o = r && S.o(r, t) && s(r, t, n);
-        return o ? c(o) : a()
+    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
+        var a = S.I(r);
+        return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
+        var a = r && S.o(r, t) && f(r, t, n);
+        return a ? p(a) : o()
     })), b = {}, g = {
         672: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
@@ -238,50 +238,50 @@
                 },
                 n = r => {
                     delete b[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
             try {
-                var a = g[e]();
-                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                var o = g[e]();
+                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             879: 0
         };
         S.f.j = (r, t) => {
             var n = S.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (672 != r) {
-                var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                t.push(n[2] = a);
-                var o = S.p + S.u(r),
+                var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                t.push(n[2] = o);
+                var a = S.p + S.u(r),
                     i = new Error;
-                S.l(o, (t => {
+                S.l(a, (t => {
                     if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var a = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                        var o = t && ("load" === t.type ? "missing" : t.type),
+                            a = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, a, [o, i, l] = t,
+                var n, o, [a, i, l] = t,
                     u = 0;
-                if (o.some((r => 0 !== e[r]))) {
+                if (a.some((r => 0 !== e[r]))) {
                     for (n in i) S.o(i, n) && (S.m[n] = i[n]);
                     l && l(S)
                 }
-                for (r && r(t); u < o.length; u++) a = o[u], S.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); u < a.length; u++) o = a[u], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkipyaladin = self.webpackChunkipyaladin || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var E = S(460);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyaladin = E
 })();
```

### Comparing `ipyaladin-0.2.3/ipyaladin/labextension/static/third-party-licenses.json` & `ipyaladin-0.2.4/ipyaladin/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/ipyaladin/nbextension/extension.js` & `ipyaladin-0.2.4/ipyaladin/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/ipyaladin/nbextension/index.js` & `ipyaladin-0.2.4/ipyaladin/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1406,16 +1406,16 @@
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: "AladinModel",
                     _view_name: "AladinView",
                     _model_module: "ipyaladin",
                     _view_module: "ipyaladin",
-                    _model_module_version: "0.2.3",
-                    _view_module_version: "0.2.3"
+                    _model_module_version: "0.2.4",
+                    _view_module_version: "0.2.4"
                 }
             }
         }
         let a = 0;
         class u extends t.DOMWidgetView {
             render() {
                 n.then((() => {
@@ -1479,15 +1479,15 @@
                     });
                     this.al.addCatalog(t), t.addSourcesAsArray(this.model.get("table_keys"), this.model.get("table_columns"))
                 }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (() => {
                     let t = A.graphicOverlay(this.model.get("overlay_options"));
                     this.al.addOverlay(t), t.addFootprints(A.footprintsFromSTCS(this.model.get("stc_string")))
                 }), this), this.listenTo(this.model, "change:listener_flag", (() => {
                     let t = this.model.get("listener_type");
-                    this.al.on(t, (function(e) {
+                    this.al.on(t, (e => {
                         if ("select" !== t) e && this.send({
                             event: "callback",
                             type: t,
                             data: {
                                 data: e.data,
                                 dec: e.dec,
                                 ra: e.ra,
```

### Comparing `ipyaladin-0.2.3/ipyaladin.egg-info/PKG-INFO` & `ipyaladin-0.2.4/ipyaladin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyaladin
-Version: 0.2.3
+Version: 0.2.4
 Summary: ipyaladin
 Home-page: https://github.com/cds-astro/ipyaladin
 Author: Jerome Desroziers, Thomas Boch & Matthieu Baumann
 Author-email: matthieu.baumann@astro.unistra.fr
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/cds-astro/ipyaladin/issues
 Project-URL: Live Testing, https://mybinder.org/v2/gh/cds-astro/ipyaladin/master
@@ -70,15 +70,15 @@
 And you are ready to use ipyaladin inside your notebooks!
 Additionny, for a jupyterlab usage you will need to:
 
     jupyter labextension develop ipyaladin --overwrite
 
 There is also a conda package that can be installed with:
 
-    conda install -c bmatthieu3 ipyaladin==0.2.3
+    conda install -c bmatthieu3 ipyaladin==0.2.4
 
 ## New features corner
 
 ![new_features](assets/new_features.gif)
 
 ## Development installation
```

### Comparing `ipyaladin-0.2.3/ipyaladin.egg-info/SOURCES.txt` & `ipyaladin-0.2.4/ipyaladin.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 ipyaladin.egg-info/PKG-INFO
 ipyaladin.egg-info/SOURCES.txt
 ipyaladin.egg-info/dependency_links.txt
 ipyaladin.egg-info/not-zip-safe
 ipyaladin.egg-info/requires.txt
 ipyaladin.egg-info/top_level.txt
 ipyaladin/labextension/package.json
-ipyaladin/labextension/static/563.9c25681782097966161a.js
-ipyaladin/labextension/static/590.b90399830948d2f839e2.js
+ipyaladin/labextension/static/563.e86cfcd7efe0f971a73e.js
+ipyaladin/labextension/static/590.c686e7199dfcb1a5e45b.js
 ipyaladin/labextension/static/794.644314dbf6493c3f7619.js
-ipyaladin/labextension/static/remoteEntry.baf7991223a7feb4e9c0.js
+ipyaladin/labextension/static/remoteEntry.501d5d2382e909d58004.js
 ipyaladin/labextension/static/style.js
 ipyaladin/labextension/static/third-party-licenses.json
 ipyaladin/nbextension/extension.js
 ipyaladin/nbextension/index.js
 js/README.md
 js/amd-public-path.js
 js/package.json
```

### Comparing `ipyaladin-0.2.3/js/amd-public-path.js` & `ipyaladin-0.2.4/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/js/dist/index.js` & `ipyaladin-0.2.4/js/dist/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1406,16 +1406,16 @@
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: "AladinModel",
                     _view_name: "AladinView",
                     _model_module: "ipyaladin",
                     _view_module: "ipyaladin",
-                    _model_module_version: "0.2.3",
-                    _view_module_version: "0.2.3"
+                    _model_module_version: "0.2.4",
+                    _view_module_version: "0.2.4"
                 }
             }
         }
         let a = 0;
         class u extends t.DOMWidgetView {
             render() {
                 n.then((() => {
@@ -1479,15 +1479,15 @@
                     });
                     this.al.addCatalog(t), t.addSourcesAsArray(this.model.get("table_keys"), this.model.get("table_columns"))
                 }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (() => {
                     let t = A.graphicOverlay(this.model.get("overlay_options"));
                     this.al.addOverlay(t), t.addFootprints(A.footprintsFromSTCS(this.model.get("stc_string")))
                 }), this), this.listenTo(this.model, "change:listener_flag", (() => {
                     let t = this.model.get("listener_type");
-                    this.al.on(t, (function(e) {
+                    this.al.on(t, (e => {
                         if ("select" !== t) e && this.send({
                             event: "callback",
                             type: t,
                             data: {
                                 data: e.data,
                                 dec: e.dec,
                                 ra: e.ra,
```

### Comparing `ipyaladin-0.2.3/js/lib/jupyter-aladin.js` & `ipyaladin-0.2.4/js/lib/jupyter-aladin.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -67,16 +67,16 @@
             ...super.defaults(),
             _model_name: 'AladinModel',
             _view_name: 'AladinView',
 
             _model_module: 'ipyaladin',
             _view_module: 'ipyaladin',
 
-            _model_module_version: '0.2.3',
-            _view_module_version: '0.2.3',
+            _model_module_version: '0.2.4',
+            _view_module_version: '0.2.4',
         };
     }
 }
 
 
 let idxView = 0;
 export class AladinView extends DOMWidgetView {
@@ -233,15 +233,15 @@
             let overlay = A.graphicOverlay(this.model.get('overlay_options'));
             this.al.addOverlay(overlay);
             overlay.addFootprints(A.footprintsFromSTCS(this.model.get('stc_string')));
         }, this);
 
         this.listenTo(this.model, 'change:listener_flag', () => {
             let type = this.model.get('listener_type');
-            this.al.on(type, function(object) {
+            this.al.on(type, (object) => {
                 if (type === 'select') {
                     let sources = object;
                     // first, deselect previously selected sources
                     for (let catalog of this.al.view.catalogs) {
                         catalog.deselectAll();
                     }
                     let sourcesData = [];
```

### Comparing `ipyaladin-0.2.3/js/package.json` & `ipyaladin-0.2.4/js/package.json`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/js/webpack.config.js` & `ipyaladin-0.2.4/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/js/yarn.lock` & `ipyaladin-0.2.4/js/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   integrity sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==
 
 "@jridgewell/set-array@^1.0.1":
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/@jridgewell/set-array/-/set-array-1.1.2.tgz#7c6cf998d6d20b914c0a55a91ae928ff25965e72"
   integrity sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==
 
-"@jridgewell/source-map@^0.3.2":
+"@jridgewell/source-map@^0.3.3":
   version "0.3.3"
   resolved "https://registry.yarnpkg.com/@jridgewell/source-map/-/source-map-0.3.3.tgz#8108265659d4c33e72ffe14e33d6cc5eb59f2fda"
   integrity sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==
   dependencies:
     "@jridgewell/gen-mapping" "^0.3.0"
     "@jridgewell/trace-mapping" "^0.3.9"
 
@@ -64,17 +64,17 @@
     "@types/backbone" "1.4.14"
     "@types/lodash" "^4.14.134"
     backbone "1.4.0"
     jquery "^3.1.1"
     lodash "^4.17.4"
 
 "@jupyterlab/builder@^3.0.0 || ^4.0.0":
-  version "4.0.1"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-4.0.1.tgz#4acf37d46fa68c06849acd5970c0f94a3a835a75"
-  integrity sha512-j1UWwRfZWeDR5Z72OGI406srr2HzxYi3chwnKCSxBA4mVgoJ4+ntRL/67q9K6cRvrUOsaVLTFHG1SKJ8S7w0ZA==
+  version "4.0.2"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-4.0.2.tgz#77c0d40d87d452915f73b85c8e393b3436ac770e"
+  integrity sha512-b4NPnnMNkfs07jeqxD2kctsZqYGncXWTmo0VsiMeiO4P19QaRMJrigjI56SC3V6100FpQby24yDZK625CR41lg==
   dependencies:
     "@lumino/algorithm" "^2.0.0"
     "@lumino/application" "^2.1.1"
     "@lumino/commands" "^2.1.1"
     "@lumino/coreutils" "^2.1.1"
     "@lumino/disposable" "^2.1.1"
     "@lumino/domutils" "^2.0.0"
@@ -100,80 +100,80 @@
     supports-color "^7.2.0"
     terser-webpack-plugin "^5.3.7"
     webpack "^5.76.1"
     webpack-cli "^5.0.1"
     webpack-merge "^5.8.0"
     worker-loader "^3.0.2"
 
-"@jupyterlab/coreutils@^5.6.3":
-  version "5.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.3.tgz#3b0b5d481b14596158b560336833c89be509e84e"
-  integrity sha512-jRVTpwGzP9wBNYuaZTip89FS1qbeSYrEO2qdNVdW2rs0mQHcIlu3Fkv5muMFmKYGi0XHhG3UhZiWQ7qiPw2svQ==
+"@jupyterlab/coreutils@^5.6.4":
+  version "5.6.4"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/coreutils/-/coreutils-5.6.4.tgz#b0fa5ce1d8b1832bd17fab4ec1bc1e7cb5606304"
+  integrity sha512-KKZcX+b4YPhoOkDKpxPXhc/QUmPNImgcsVsxceCNrznXNxLwwQcreSCMfKQ+i9Z1QayvYUETphAO5dUmfUQkjg==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     minimist "~1.2.0"
     moment "^2.24.0"
     path-browserify "^1.0.0"
     url-parse "~1.5.1"
 
-"@jupyterlab/nbformat@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.3.tgz#8520338e3679cbe8ce2ea8eb5a9b816f8b774ad3"
-  integrity sha512-0qJLa4dtOmu9EmHFeM7gaZi4qheovIPc9ZrgGGRuG0obajs4YYlvh4MQvCSgpVhme4AuBfGlcfzhlx+Gbzr5Xw==
+"@jupyterlab/nbformat@^3.6.4":
+  version "3.6.4"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.4.tgz#da2ad8dfd433009245a679c023a69f5eae9a4978"
+  integrity sha512-FIXm3PjtVJOyd+og8mMBcKMgSSq5iGf11rDH9rjFzd1Uo6TwCBiKmkipyAaa8wVcB07A5ocpU0wCE/do2m24kg==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/observables@^4.6.3":
-  version "4.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.3.tgz#49a9ca49fbda7428abbd1bfb8a4006ecd406c18d"
-  integrity sha512-CvQoL+9WHXOy/CXp/PQLi4c5iZVJ4psz11+GrycDDinX1AdVQ8a43OLTC0gxWl3Tk2C8ZvAi1sgn4FS68E1ACQ==
+"@jupyterlab/observables@^4.6.4":
+  version "4.6.4"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.4.tgz#a6568e3aae0d14f5c3bb8e4229a31fddaf38458d"
+  integrity sha512-HqIYzHj+HYWnZTFMWr6b0GG92UfrFk7k8ihLlVm0W289Pz+0YlOBPgXhEJsTPPIm+YiICXD8WzvySXUWo92ryA==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/messaging" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
 
 "@jupyterlab/services@^6.0.0":
-  version "6.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.3.tgz#303938e5dc5aebce7a86324a64ed89c25c61c9e7"
-  integrity sha512-BxEOMRl9X18T5wY7iV6ZJhARnibFghpD3OruqeSbnGdbRv6XJi8prsRbCQQ6Mf9agvf81B20KmDvYKikPHC0xQ==
-  dependencies:
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/settingregistry" "^3.6.3"
-    "@jupyterlab/statedb" "^3.6.3"
+  version "6.6.4"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/services/-/services-6.6.4.tgz#f47092556e209d399d8e588a9dc760ba9e5bf505"
+  integrity sha512-qtPnCfPWyKvQmr5w/YLO3+Tif1fYkJvCAufLljiWpAORFF06LvURbP9Lb+GOsXS9VHZQTcXLBv8sdlQSbj5qNg==
+  dependencies:
+    "@jupyterlab/coreutils" "^5.6.4"
+    "@jupyterlab/nbformat" "^3.6.4"
+    "@jupyterlab/observables" "^4.6.4"
+    "@jupyterlab/settingregistry" "^3.6.4"
+    "@jupyterlab/statedb" "^3.6.4"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/polling" "^1.9.0"
     "@lumino/signaling" "^1.10.0"
     node-fetch "^2.6.0"
     ws "^7.4.6"
 
-"@jupyterlab/settingregistry@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.3.tgz#642f8b6449d626821ef13a7e778ae716fa8331c9"
-  integrity sha512-pnzIge0ZC8V63R97HiNroJ0eaPM0DN6x65SStyLuv/K8Qez4XqpOdc0Wfell5ri5mxMvm1qKekuFeTikqSXQKQ==
+"@jupyterlab/settingregistry@^3.6.4":
+  version "3.6.4"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/settingregistry/-/settingregistry-3.6.4.tgz#bf2f7ade628b0a108df9f8796faa98c9f4bd9f2c"
+  integrity sha512-DD3qrd2X6fvkC67MlNkPlHZBh14mecu5+fkE8KBbAQwPZsn9E/JdOVbNVc3sd5Jl/hzobGdtcMhQUTfK46g6ow==
   dependencies:
-    "@jupyterlab/statedb" "^3.6.3"
+    "@jupyterlab/statedb" "^3.6.4"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/signaling" "^1.10.0"
     ajv "^6.12.3"
     json5 "^2.1.1"
 
-"@jupyterlab/statedb@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.3.tgz#6ba2166af9232c9a185cf0077cf1272f24cc9a69"
-  integrity sha512-A36L+0NN8f0WOES2GdtZjp9uFuC7IBjhKiO/RlKRX5AFjNxoJ9oO3PZtoxJQYPnGBljMqVdRa+m9aYEfvKhYyQ==
+"@jupyterlab/statedb@^3.6.4":
+  version "3.6.4"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/statedb/-/statedb-3.6.4.tgz#754add8947347c1c466797790fd030f8b9ad7487"
+  integrity sha512-sfbAMU7wTf8pzdyW1TLOUzdki1wu7amtDD9JgrD6RrUXTve9QaiKjC+FenFEBPMzogWDogZGAtBEoTLMY+k3pg==
   dependencies:
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/disposable" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
 
@@ -409,17 +409,17 @@
   resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.4.tgz#37fc1223f0786c39627068a12e94d6e6fc61de16"
   integrity sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==
   dependencies:
     "@types/eslint" "*"
     "@types/estree" "*"
 
 "@types/eslint@*":
-  version "8.40.0"
-  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.40.0.tgz#ae73dc9ec5237f2794c4f79efd6a4c73b13daf23"
-  integrity sha512-nbq2mvc/tBrK9zQQuItvjJl++GTN5j06DaPtp3hZCpngmG6Q3xoyEmd0TwZI0gAy/G1X0zhGBbr2imsGFdFV0g==
+  version "8.40.2"
+  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.40.2.tgz#2833bc112d809677864a4b0e7d1de4f04d7dac2d"
+  integrity sha512-PRVjQ4Eh9z9pmmtaq8nTjZjQwKFk7YIHIud3lRoKRBgUQjgjRmoGxxGEPXQkF+lH7QkHJRNr5F4aBgYCW0lqpQ==
   dependencies:
     "@types/estree" "*"
     "@types/json-schema" "*"
 
 "@types/estree@*", "@types/estree@^1.0.0":
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.1.tgz#aa22750962f3bf0e79d753d3cc067f010c95f194"
@@ -439,17 +439,17 @@
 
 "@types/lodash@^4.14.134":
   version "4.14.195"
   resolved "https://registry.yarnpkg.com/@types/lodash/-/lodash-4.14.195.tgz#bafc975b252eb6cea78882ce8a7b6bf22a6de632"
   integrity sha512-Hwx9EUgdwf2GLarOjQp5ZH8ZmblzcbTBC2wtQWNKARBSxM9ezRIAUpeDTgoQRAFB0+8CNWXVA9+MaSOzOF3nPg==
 
 "@types/node@*":
-  version "20.2.5"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.2.5.tgz#26d295f3570323b2837d322180dfbf1ba156fefb"
-  integrity sha512-JJulVEQXmiY9Px5axXHeYGLSjhkZEnD+MDPDGbCbIAbMslkKwmygtZFy1X6s/075Yo94sf8GuSlFfPzysQrWZQ==
+  version "20.3.1"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.3.1.tgz#e8a83f1aa8b649377bb1fb5d7bac5cb90e784dfe"
+  integrity sha512-EhcH/wvidPy1WeML3TtYFGR83UzjxeWRen9V402T8aUGYsCHOmfoisV3ZSg03gAFIbLq8TnWOJ0f4cALtnSEUg==
 
 "@types/sizzle@*":
   version "2.3.3"
   resolved "https://registry.yarnpkg.com/@types/sizzle/-/sizzle-2.3.3.tgz#ff5e2f1902969d305225a047c8a0fd5c915cebef"
   integrity sha512-JYM8x9EGF163bEyhdJBpR2QX1R5naCJHC8ucJylJ3w9/CVBaskdQ8WqBf8MmQrd1kRvp/a4TS8HJ+bxzR7ZJYQ==
 
 "@types/source-list-map@*":
@@ -588,28 +588,28 @@
   version "1.11.6"
   resolved "https://registry.yarnpkg.com/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz#a7bf8dd7e362aeb1668ff43f35cb849f188eff20"
   integrity sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==
   dependencies:
     "@webassemblyjs/ast" "1.11.6"
     "@xtuc/long" "4.2.2"
 
-"@webpack-cli/configtest@^2.1.0":
-  version "2.1.0"
-  resolved "https://registry.yarnpkg.com/@webpack-cli/configtest/-/configtest-2.1.0.tgz#b59b33377b1b896a9a7357cfc643b39c1524b1e6"
-  integrity sha512-K/vuv72vpfSEZoo5KIU0a2FsEoYdW0DUMtMpB5X3LlUwshetMZRZRxB7sCsVji/lFaSxtQQ3aM9O4eMolXkU9w==
+"@webpack-cli/configtest@^2.1.1":
+  version "2.1.1"
+  resolved "https://registry.yarnpkg.com/@webpack-cli/configtest/-/configtest-2.1.1.tgz#3b2f852e91dac6e3b85fb2a314fb8bef46d94646"
+  integrity sha512-wy0mglZpDSiSS0XHrVR+BAdId2+yxPSoJW8fsna3ZpYSlufjvxnP4YbKTCBZnNIcGN4r6ZPXV55X4mYExOfLmw==
 
-"@webpack-cli/info@^2.0.1":
-  version "2.0.1"
-  resolved "https://registry.yarnpkg.com/@webpack-cli/info/-/info-2.0.1.tgz#eed745799c910d20081e06e5177c2b2569f166c0"
-  integrity sha512-fE1UEWTwsAxRhrJNikE7v4EotYflkEhBL7EbajfkPlf6E37/2QshOy/D48Mw8G5XMFlQtS6YV42vtbG9zBpIQA==
+"@webpack-cli/info@^2.0.2":
+  version "2.0.2"
+  resolved "https://registry.yarnpkg.com/@webpack-cli/info/-/info-2.0.2.tgz#cc3fbf22efeb88ff62310cf885c5b09f44ae0fdd"
+  integrity sha512-zLHQdI/Qs1UyT5UBdWNqsARasIA+AaF8t+4u2aS2nEpBQh2mWIVb8qAklq0eUENnC5mOItrIB4LiS9xMtph18A==
 
-"@webpack-cli/serve@^2.0.4":
-  version "2.0.4"
-  resolved "https://registry.yarnpkg.com/@webpack-cli/serve/-/serve-2.0.4.tgz#3982ee6f8b42845437fc4d391e93ac5d9da52f0f"
-  integrity sha512-0xRgjgDLdz6G7+vvDLlaRpFatJaJ69uTalZLRSMX5B3VUrDmXcrVA3+6fXXQgmYz7bY9AAgs348XQdmtLsK41A==
+"@webpack-cli/serve@^2.0.5":
+  version "2.0.5"
+  resolved "https://registry.yarnpkg.com/@webpack-cli/serve/-/serve-2.0.5.tgz#325db42395cd49fe6c14057f9a900e427df8810e"
+  integrity sha512-lqaoKnRYBdo1UgDX8uF24AfGMifWK19TxPmM5FHc2vAGxrJ/qtyUyFBWoY1tISZdelsQ5fBcOusifo5o5wSJxQ==
 
 "@xtuc/ieee754@^1.2.0":
   version "1.2.0"
   resolved "https://registry.yarnpkg.com/@xtuc/ieee754/-/ieee754-1.2.0.tgz#eef014a3145ae477a1cbc00cd1e552336dceb790"
   integrity sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==
 
 "@xtuc/long@4.2.2":
@@ -623,18 +623,18 @@
   integrity sha512-j2afSsaIENvHZN2B8GOpF566vZ5WVk5opAiMTvWgaQT8DkbOqsTfvNAvHoRGU2zzP8cPoqys+xHTRDWW8L+/BA==
 
 acorn-import-assertions@^1.9.0:
   version "1.9.0"
   resolved "https://registry.yarnpkg.com/acorn-import-assertions/-/acorn-import-assertions-1.9.0.tgz#507276249d684797c84e0734ef84860334cfb1ac"
   integrity sha512-cmMwop9x+8KFhxvKrKfPYmN6/pKTYYHBqLa0DfvVZcKMJWNyWLnaqND7dx/qn66R7ewM1UX5XMaDVP5wlVTaVA==
 
-acorn@^8.5.0, acorn@^8.7.1:
-  version "8.8.2"
-  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.8.2.tgz#1b2f25db02af965399b9776b0c2c391276d37c4a"
-  integrity sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==
+acorn@^8.7.1, acorn@^8.8.2:
+  version "8.9.0"
+  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.9.0.tgz#78a16e3b2bcc198c10822786fa6679e245db5b59"
+  integrity sha512-jaVNAFBHNLXspO543WnNNPZFRtavh3skAkITqD0/2aeMkKZTN+254PyhwxFYrk3vQ1xfY+2wbesJMs/JC8/PwQ==
 
 ajv-formats@^2.1.1:
   version "2.1.1"
   resolved "https://registry.yarnpkg.com/ajv-formats/-/ajv-formats-2.1.1.tgz#6e669400659eb74973bbf2e33327180a0996b520"
   integrity sha512-Wx0Kx52hxE7C18hkMEggYlEifqWZtYaRgouJor+WMdPnQyEK13vgEWyVNup7SoeeoLMsr4kf5h6dOW11I15MUA==
   dependencies:
     ajv "^8.0.0"
@@ -700,32 +700,32 @@
   resolved "https://registry.yarnpkg.com/brace-expansion/-/brace-expansion-1.1.11.tgz#3c7fcbf529d87226f3d2f52b966ff5271eb441dd"
   integrity sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==
   dependencies:
     balanced-match "^1.0.0"
     concat-map "0.0.1"
 
 browserslist@^4.14.5:
-  version "4.21.7"
-  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.7.tgz#e2b420947e5fb0a58e8f4668ae6e23488127e551"
-  integrity sha512-BauCXrQ7I2ftSqd2mvKHGo85XR0u7Ru3C/Hxsy/0TkfCtjrmAbPdzLGasmoiBxplpDXlPvdjX9u7srIMfgasNA==
+  version "4.21.9"
+  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.9.tgz#e11bdd3c313d7e2a9e87e8b4b0c7872b13897635"
+  integrity sha512-M0MFoZzbUrRU4KNfCrDLnvyE7gub+peetoTid3TBIqtunaDJyXlwhakT+/VkvSXcfIzFfK/nkCs4nmyTmxdNSg==
   dependencies:
-    caniuse-lite "^1.0.30001489"
-    electron-to-chromium "^1.4.411"
+    caniuse-lite "^1.0.30001503"
+    electron-to-chromium "^1.4.431"
     node-releases "^2.0.12"
     update-browserslist-db "^1.0.11"
 
 buffer-from@^1.0.0:
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.2.tgz#2b146a6fd72e80b4f55d255f35ed59a3a9a41bd5"
   integrity sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==
 
-caniuse-lite@^1.0.30001489:
-  version "1.0.30001491"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001491.tgz#eab0e0f392de6f7411751d148de9b5bd6b203e46"
-  integrity sha512-17EYIi4TLnPiTzVKMveIxU5ETlxbSO3B6iPvMbprqnKh4qJsQGk5Nh1Lp4jIMAE0XfrujsJuWZAM3oJdMHaKBA==
+caniuse-lite@^1.0.30001503:
+  version "1.0.30001506"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001506.tgz#35bd814b310a487970c585430e9e80ee23faf14b"
+  integrity sha512-6XNEcpygZMCKaufIcgpQNZNf00GEqc7VQON+9Rd0K1bMYo8xhMZRAo5zpbnbMNizi4YNgIDAFrdykWsvY3H4Hw==
 
 chalk@^2.3.0:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
@@ -826,41 +826,41 @@
   integrity sha512-aO50/qPC7X2ChjRFniRiscxBLT/K01bALqfcDaf8Ih5OqQ1N4iT/Abx9Ofu3/ms446vHTm46FACIuJUmgUQcDQ==
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
-electron-to-chromium@^1.4.411:
-  version "1.4.413"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.413.tgz#0067c3122946ae234cbefb9401ecefde851cdcf2"
-  integrity sha512-Gd+/OAhRca06dkVxIQo/W7dr6Nmk9cx6lQdZ19GvFp51k5B/lUAokm6SJfNkdV8kFLsC3Z4sLTyEHWCnB1Efbw==
+electron-to-chromium@^1.4.431:
+  version "1.4.437"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.437.tgz#d0e73a431a9ade4467f73d48a59d752d91909316"
+  integrity sha512-ZFekRuBOHUXp21wrR5lshT6pZa/KmjkhKBAtmZz4NN5sCWlHOk3kdhiwFINrDBsRLX6FjyBAb1TRN+KBeNlyzQ==
 
 emojis-list@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/emojis-list/-/emojis-list-3.0.0.tgz#5570662046ad29e2e916e71aae260abdff4f6a78"
   integrity sha512-/kyM18EfinwXZbno9FyUGeFh87KC8HRQBQGildHZbEuRyWFOmv1U10o9BBp8XVZDVNNuQKyIGIu5ZYAAXJ0V2Q==
 
-enhanced-resolve@^5.14.1:
-  version "5.14.1"
-  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.14.1.tgz#de684b6803724477a4af5d74ccae5de52c25f6b3"
-  integrity sha512-Vklwq2vDKtl0y/vtwjSesgJ5MYS7Etuk5txS8VdKL4AOS1aUlD96zqIfsOSLQsdv3xgMRbtkWM8eG9XDfKUPow==
+enhanced-resolve@^5.15.0:
+  version "5.15.0"
+  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.15.0.tgz#1af946c7d93603eb88e9896cee4904dc012e9c35"
+  integrity sha512-LXYT42KJ7lpIKECr2mAXIaMldcNCh/7E0KBKOu4KSfkHmP+mZmSs+8V5gBAqisWBy0OO4W5Oyys0GO1Y8KtdKg==
   dependencies:
     graceful-fs "^4.2.4"
     tapable "^2.2.0"
 
 envinfo@^7.7.3:
-  version "7.8.1"
-  resolved "https://registry.yarnpkg.com/envinfo/-/envinfo-7.8.1.tgz#06377e3e5f4d379fea7ac592d5ad8927e0c4d475"
-  integrity sha512-/o+BXHmB7ocbHEAs6F2EnG0ogybVVUdkRunTT2glZU9XAaGmhqskrvKwqXuDfNjEO0LZKWdejEEpnq8aM0tOaw==
+  version "7.9.0"
+  resolved "https://registry.yarnpkg.com/envinfo/-/envinfo-7.9.0.tgz#47594a13081be0d9be6e513534e8c58dbb26c7a1"
+  integrity sha512-RODB4txU+xImYDemN5DqaKC0CHk05XSVkOX4pq0hK26Qx+1LChkuOyUDlGEjYb3ACr0n9qBhFjg37hQuJvpkRQ==
 
 es-module-lexer@^1.2.1:
-  version "1.2.1"
-  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-1.2.1.tgz#ba303831f63e6a394983fde2f97ad77b22324527"
-  integrity sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==
+  version "1.3.0"
+  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-1.3.0.tgz#6be9c9e0b4543a60cd166ff6f8b4e9dae0b0c16f"
+  integrity sha512-vZK7T0N2CBmBOixhmjdqx2gWVbFZ4DXZ/NyRMZVlJXPa7CyFS+/a4QQsDGDQy9ZfEzxFuNEsMLeQJnKP2p5/JA==
 
 escalade@^3.1.1:
   version "3.1.1"
   resolved "https://registry.yarnpkg.com/escalade/-/escalade-3.1.1.tgz#d8cfdc7000965c5a0174b4a82eaa5c0552742e40"
   integrity sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==
 
 escape-string-regexp@^1.0.5:
@@ -1410,42 +1410,42 @@
   resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-2.7.1.tgz#1ca4f32d1b24c590c203b8e7a50bf0ea4cd394d7"
   integrity sha512-SHiNtMOUGWBQJwzISiVYKu82GiV4QYGePp3odlY1tuKO7gPtphAT5R/py0fA6xtbgLL/RvtJZnU9b8s0F1q0Xg==
   dependencies:
     "@types/json-schema" "^7.0.5"
     ajv "^6.12.4"
     ajv-keywords "^3.5.2"
 
-schema-utils@^3.0.0, schema-utils@^3.1.1, schema-utils@^3.1.2:
-  version "3.1.2"
-  resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-3.1.2.tgz#36c10abca6f7577aeae136c804b0c741edeadc99"
-  integrity sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==
+schema-utils@^3.0.0, schema-utils@^3.1.1, schema-utils@^3.2.0:
+  version "3.3.0"
+  resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-3.3.0.tgz#f50a88877c3c01652a15b622ae9e9795df7a60fe"
+  integrity sha512-pN/yOAvcC+5rQ5nERGuwrjLlYvLTbCibnZ1I7B1LaiAz9BRBlE9GMgE/eqV30P7aJQUf7Ddimy/RsbYO/GrVGg==
   dependencies:
     "@types/json-schema" "^7.0.8"
     ajv "^6.12.5"
     ajv-keywords "^3.5.2"
 
 schema-utils@^4.0.0:
-  version "4.0.1"
-  resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-4.0.1.tgz#eb2d042df8b01f4b5c276a2dfd41ba0faab72e8d"
-  integrity sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==
+  version "4.2.0"
+  resolved "https://registry.yarnpkg.com/schema-utils/-/schema-utils-4.2.0.tgz#70d7c93e153a273a805801882ebd3bff20d89c8b"
+  integrity sha512-L0jRsrPpjdckP3oPug3/VxNKt2trR8TcabrM6FOAAlvC/9Phcmm+cuAgTlxBqdBR1WJx7Naj9WHw+aOmheSVbw==
   dependencies:
     "@types/json-schema" "^7.0.9"
     ajv "^8.9.0"
     ajv-formats "^2.1.1"
     ajv-keywords "^5.1.0"
 
 semver@^5.4.1:
   version "5.7.1"
   resolved "https://registry.yarnpkg.com/semver/-/semver-5.7.1.tgz#a954f931aeba508d307bbf069eff0c01c96116f7"
   integrity sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==
 
 semver@^7.3.8:
-  version "7.5.1"
-  resolved "https://registry.yarnpkg.com/semver/-/semver-7.5.1.tgz#c90c4d631cf74720e46b21c1d37ea07edfab91ec"
-  integrity sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==
+  version "7.5.2"
+  resolved "https://registry.yarnpkg.com/semver/-/semver-7.5.2.tgz#5b851e66d1be07c1cdaf37dfc856f543325a2beb"
+  integrity sha512-SoftuTROv/cRjCze/scjGyiDtcUyxw1rgYQSZY7XTmtR5hX+dm76iDbTH8TkLPHCQmlbQVSSbNZCPM2hb0knnQ==
   dependencies:
     lru-cache "^6.0.0"
 
 serialize-javascript@^6.0.1:
   version "6.0.1"
   resolved "https://registry.yarnpkg.com/serialize-javascript/-/serialize-javascript-6.0.1.tgz#b206efb27c3da0b0ab6b52f48d170b7996458e5c"
   integrity sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==
@@ -1549,20 +1549,20 @@
     "@jridgewell/trace-mapping" "^0.3.17"
     jest-worker "^27.4.5"
     schema-utils "^3.1.1"
     serialize-javascript "^6.0.1"
     terser "^5.16.8"
 
 terser@^5.16.8:
-  version "5.17.6"
-  resolved "https://registry.yarnpkg.com/terser/-/terser-5.17.6.tgz#d810e75e1bb3350c799cd90ebefe19c9412c12de"
-  integrity sha512-V8QHcs8YuyLkLHsJO5ucyff1ykrLVsR4dNnS//L5Y3NiSXpbK1J+WMVUs67eI0KTxs9JtHhgEQpXQVHlHI92DQ==
+  version "5.18.1"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-5.18.1.tgz#6d8642508ae9fb7b48768e48f16d675c89a78460"
+  integrity sha512-j1n0Ao919h/Ai5r43VAnfV/7azUYW43GPxK7qSATzrsERfW7+y2QW9Cp9ufnRF5CQUWbnLSo7UJokSWCqg4tsQ==
   dependencies:
-    "@jridgewell/source-map" "^0.3.2"
-    acorn "^8.5.0"
+    "@jridgewell/source-map" "^0.3.3"
+    acorn "^8.8.2"
     commander "^2.20.0"
     source-map-support "~0.5.20"
 
 tr46@^2.1.0:
   version "2.1.0"
   resolved "https://registry.yarnpkg.com/tr46/-/tr46-2.1.0.tgz#fa87aa81ca5d5941da8cbf1f9b749dc969a4e240"
   integrity sha512-15Ih7phfcdP5YxqiB+iDtLoaTz4Nd35+IiAv0kQ5FNKHzXgdWqPoTIqEDDJmXceQt4JZk6lVPT8lnDlPpGDppw==
@@ -1627,22 +1627,22 @@
 
 webidl-conversions@^6.1.0:
   version "6.1.0"
   resolved "https://registry.yarnpkg.com/webidl-conversions/-/webidl-conversions-6.1.0.tgz#9111b4d7ea80acd40f5270d666621afa78b69514"
   integrity sha512-qBIvFLGiBpLjfwmYAaHPXsn+ho5xZnGvyGvsarywGNc8VyQJUMHJ8OBKGGrPER0okBeMDaan4mNBlgBROxuI8w==
 
 webpack-cli@^5.0.1:
-  version "5.1.1"
-  resolved "https://registry.yarnpkg.com/webpack-cli/-/webpack-cli-5.1.1.tgz#c211ac6d911e77c512978f7132f0d735d4a97ace"
-  integrity sha512-OLJwVMoXnXYH2ncNGU8gxVpUtm3ybvdioiTvHgUyBuyMLKiVvWy+QObzBsMtp5pH7qQoEuWgeEUQ/sU3ZJFzAw==
+  version "5.1.4"
+  resolved "https://registry.yarnpkg.com/webpack-cli/-/webpack-cli-5.1.4.tgz#c8e046ba7eaae4911d7e71e2b25b776fcc35759b"
+  integrity sha512-pIDJHIEI9LR0yxHXQ+Qh95k2EvXpWzZ5l+d+jIo+RdSm9MiHfzazIxwwni/p7+x4eJZuvG1AJwgC4TNQ7NRgsg==
   dependencies:
     "@discoveryjs/json-ext" "^0.5.0"
-    "@webpack-cli/configtest" "^2.1.0"
-    "@webpack-cli/info" "^2.0.1"
-    "@webpack-cli/serve" "^2.0.4"
+    "@webpack-cli/configtest" "^2.1.1"
+    "@webpack-cli/info" "^2.0.2"
+    "@webpack-cli/serve" "^2.0.5"
     colorette "^2.0.14"
     commander "^10.0.1"
     cross-spawn "^7.0.3"
     envinfo "^7.7.3"
     fastest-levenshtein "^1.0.12"
     import-local "^3.0.2"
     interpret "^3.1.1"
@@ -1667,38 +1667,38 @@
 
 webpack-sources@^3.2.3:
   version "3.2.3"
   resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-3.2.3.tgz#2d4daab8451fd4b240cc27055ff6a0c2ccea0cde"
   integrity sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==
 
 webpack@^5, webpack@^5.76.1:
-  version "5.84.1"
-  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.84.1.tgz#d4493acdeca46b26ffc99d86d784cabfeb925a15"
-  integrity sha512-ZP4qaZ7vVn/K8WN/p990SGATmrL1qg4heP/MrVneczYtpDGJWlrgZv55vxaV2ul885Kz+25MP2kSXkPe3LZfmg==
+  version "5.88.0"
+  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.88.0.tgz#a07aa2f8e7a64a8f1cec0c6c2e180e3cb34440c8"
+  integrity sha512-O3jDhG5e44qIBSi/P6KpcCcH7HD+nYIHVBhdWFxcLOcIGN8zGo5nqF3BjyNCxIh4p1vFdNnreZv2h2KkoAw3lw==
   dependencies:
     "@types/eslint-scope" "^3.7.3"
     "@types/estree" "^1.0.0"
     "@webassemblyjs/ast" "^1.11.5"
     "@webassemblyjs/wasm-edit" "^1.11.5"
     "@webassemblyjs/wasm-parser" "^1.11.5"
     acorn "^8.7.1"
     acorn-import-assertions "^1.9.0"
     browserslist "^4.14.5"
     chrome-trace-event "^1.0.2"
-    enhanced-resolve "^5.14.1"
+    enhanced-resolve "^5.15.0"
     es-module-lexer "^1.2.1"
     eslint-scope "5.1.1"
     events "^3.2.0"
     glob-to-regexp "^0.4.1"
     graceful-fs "^4.2.9"
     json-parse-even-better-errors "^2.3.1"
     loader-runner "^4.2.0"
     mime-types "^2.1.27"
     neo-async "^2.6.2"
-    schema-utils "^3.1.2"
+    schema-utils "^3.2.0"
     tapable "^2.1.1"
     terser-webpack-plugin "^5.3.7"
     watchpack "^2.4.0"
     webpack-sources "^3.2.3"
 
 whatwg-mimetype@^2.3.0:
   version "2.3.0"
```

### Comparing `ipyaladin-0.2.3/setup.cfg` & `ipyaladin-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.3/setup.py` & `ipyaladin-0.2.4/setup.py`

 * *Files identical despite different names*

