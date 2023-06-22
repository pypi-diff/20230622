# Comparing `tmp/piwwwaterflow-0.2.1.tar.gz` & `tmp/piwwwaterflow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.2.1.tar", last modified: Wed Jun 21 17:03:32 2023, max compression
+gzip compressed data, was "piwwwaterflow-0.2.2.tar", last modified: Thu Jun 22 13:31:25 2023, max compression
```

## Comparing `piwwwaterflow-0.2.1.tar` & `piwwwaterflow-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.791098 piwwwaterflow-0.2.1/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.791098 piwwwaterflow-0.2.1/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.791098 piwwwaterflow-0.2.1/piwwwaterflow/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/css/iepngfix.htc
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.795098 piwwwaterflow-0.2.1/piwwwaterflow/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/blank.gif
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/piwaterflow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/play.png
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/shadow.gif
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/img/top.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.795098 piwwwaterflow-0.2.1/piwwwaterflow/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/static/js/code.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.791098 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 17:03:32.000000 piwwwaterflow-0.2.1/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:32.799098 piwwwaterflow-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:03:18.000000 piwwwaterflow-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.398343 piwwwaterflow-0.2.2/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.402343 piwwwaterflow-0.2.2/piwwwaterflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.402343 piwwwaterflow-0.2.2/piwwwaterflow/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/css/iepngfix.htc
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/piwwwaterflow/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/blank.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/piwaterflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/shadow.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/img/top.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/piwwwaterflow/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/static/js/code.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/piwwwaterflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.402343 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 13:31:25.000000 piwwwaterflow-0.2.2/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:25.406343 piwwwaterflow-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:12.000000 piwwwaterflow-0.2.2/tests/__init__.py
```

### Comparing `piwwwaterflow-0.2.1/PKG-INFO` & `piwwwaterflow-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/static/css/iepngfix.htc` & `piwwwaterflow-0.2.2/piwwwaterflow/static/css/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/static/css/view.css` & `piwwwaterflow-0.2.2/piwwwaterflow/static/css/view.css`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/static/img/icon-256.png` & `piwwwaterflow-0.2.2/piwwwaterflow/static/img/icon-256.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/static/img/icon-32.png` & `piwwwaterflow-0.2.2/piwwwaterflow/static/img/icon-32.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/static/img/piwaterflow.svg` & `piwwwaterflow-0.2.2/piwwwaterflow/static/img/piwaterflow.svg`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/static/img/play.png` & `piwwwaterflow-0.2.2/piwwwaterflow/static/img/play.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/static/js/code.js` & `piwwwaterflow-0.2.2/piwwwaterflow/static/js/code.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -219,94 +219,88 @@
 
 function forceProgram(control, program_forced) {
     if (forceTriggersEnabled && confirm("Are you sure you want to force program?.")) {
         let requestservice = new XMLHttpRequest();
         requestservice.open('POST', '/force');
         requestservice.responseType = 'text';
         requestservice.onload = function() {
-            if (requestservice.response == 'false') {
-
+            if (requestservice.response == 'true') {
+                control.style.color = '#22FF22'
+                _setEnableForceTriggers(false)
             }
         }
         var data = new FormData();
         data.append('type', 'program');
         data.append('value', program_forced);
 
         requestservice.send(data);
-
-        control.style.color = '#22FF22'
-        _setEnableForceTriggers(false)
     } else {
         control.checked = false
     }
 }
 
 function forceValve(control, valve_forced) {
     if (forceTriggersEnabled && confirm("Are you sure you want to force valve?.")) {
         let requestservice = new XMLHttpRequest();
         requestservice.open('POST', '/force');
         requestservice.responseType = 'text';
         requestservice.onload = function() {
-            if (requestservice.response == 'false') {
-
+            if (requestservice.response == 'true') {
+                control.style.color = '#22FF22'
+                _setEnableForceTriggers(false)
             }
         }
         var data = new FormData();
         data.append('type', 'valve');
         data.append('value', valve_forced);
 
         requestservice.send(data);
-        control.style.color = '#22FF22'
-        _setEnableForceTriggers(false)
     } else {
         control.checked = false
     }
 }
 
 function stopWaterflow(button) {
     let requestservice = new XMLHttpRequest();
     requestservice.open('POST', '/stop');
     requestservice.send();
     button.disabled = true;
 }
 
 function save(button) {
     let requestservice = new XMLHttpRequest();
-    requestservice.open('POST', '/force');
+    requestservice.open('POST', '/save');
     requestservice.responseType = 'text';
     requestservice.onload = function() {
-        if (requestservice.response == 'false') {
-
-        }
-    }
-    var data = new FormData();
-    data.append('save', [{
-        'name': getProgramName(0),
-        'time': document.getElementById("time1").value,
-        'valves': [{
-            'name': getValveName(0),
-            'time': parseInt(document.getElementById("valve11").value)
-        }, {
-            'name': getValveName(1),
-            'time': parseInt(document.getElementById("valve12").value)
-        }, ],
-        'enabled': document.getElementById("prog1enabled").checked
-    }, {
-        'name': getProgramName(1),
-        'time': document.getElementById("time2").value,
-        'valves': [{
-            'name': getValveName(0),
-            'time': parseInt(document.getElementById("valve21").value)
-        }, {
-            'name': getValveName(1),
-            'time': parseInt(document.getElementById("valve22").value)
-        }, ],
-        'enabled': document.getElementById("prog2enabled").checked
-    }], function ack(result) {
-        if (result) {
+        if (requestservice.response == 'true') {
             saveCurrentValues();
             refreshSaveButton();
             button.disabled = true;
         }
-    });
-    requestservice.send();
+    }
+    var data = new FormData();
+    data.append('save', JSON.stringify(
+        [{
+            'name': getProgramName(0),
+            'time': document.getElementById("time1").value,
+            'valves': [{
+                'name': getValveName(0),
+                'time': parseInt(document.getElementById("valve11").value)
+            }, {
+                'name': getValveName(1),
+                'time': parseInt(document.getElementById("valve12").value)
+            }, ],
+            'enabled': document.getElementById("prog1enabled").checked
+        }, {
+            'name': getProgramName(1),
+            'time': document.getElementById("time2").value,
+            'valves': [{
+                'name': getValveName(0),
+                'time': parseInt(document.getElementById("valve21").value)
+            }, {
+                'name': getValveName(1),
+                'time': parseInt(document.getElementById("valve22").value)
+            }, ],
+            'enabled': document.getElementById("prog2enabled").checked
+        }]));
+    requestservice.send(data);
 }
```

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/templates/form.html` & `piwwwaterflow-0.2.2/piwwwaterflow/templates/form.html`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/webservice.py` & `piwwwaterflow-0.2.2/piwwwaterflow/webservice.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Webservice to control and manage the piwaterflow loop """
 from datetime import datetime
-
-from flask import Flask, render_template, request
+import json
+from flask import Flask, render_template, request, make_response, Response
 from flask_compress import Compress
 from importlib_metadata import version, PackageNotFoundError
 
 from piwaterflow import Waterflow
 from log_mgr import Logger, LoggerMode
 from revproxy_auth import RevProxyAuth
 
@@ -86,62 +86,64 @@
             # Change to string so that javascript can manage with it
             for program in responsedict['config']['programs']:
                 program['start_time'] = program['start_time'].strftime('%H:%M')
         except Exception as ex:
             self.logger.error('Error calculating service request: %s', ex)
             raise RuntimeError(f'Exception on service request: {ex}') from ex
 
-        return responsedict
+        return make_response(json.dumps(responsedict), 200)
 
-    def on_force(self, data: dict):
+    def on_force(self):
         """ On force action request
         Args:
             data (dict): 'type': Must be 'valve' or 'program'
                          'value': Must be the index of the program or value to be forced
         """
         waterflow = Waterflow()
 
         if request.method == 'POST':
-            self.logger.info('Force requested...%s', data)
-            type_force = request.form.get['type']
-            value_force = request.form.get['value']
+            type_force = request.form.get('type')
+            value_force = request.form.get('value')
+            self.logger.info('Force requested: %s = %s', type_force, value_force)
+
             waterflow.force(type_force, value_force)
+            return make_response('Force scheduled: %s = %s', type_force, value_force, 200)
         else:
             forced_data = waterflow.get_forced_info()
-            return forced_data
-            # return json.dumps(forced_data)
+            return make_response(json.dumps(forced_data), 200)
 
     def on_stop(self):
         """ Event to stop current operation """
         waterflow = Waterflow()
 
         if request.method == 'POST':
             self.logger.info('Stop requested...')
             waterflow.stop()
+            return "true"
         else:
             stop_requested = waterflow.stop_requested()
-            return "true" if stop_requested else "false"
+            return make_response(json.dumps(stop_requested), 200)
 
     def on_save(self):
         """ Event to save the changes in the watering system schedulling
         Args:
             data (dict): Information about the required schedulling
         Returns:
             bool: If everything went ok
         """
         waterflow = Waterflow()
 
         self.logger.info("Saving programs...")
-        data = request.form.get['save']
+        data = json.loads(request.form.get('save'))
         parsed_config = waterflow.config.get_dict_copy()
         for program, update in zip(parsed_config['programs'], data):
             self._change_program(program, update)
 
         waterflow.update_config(programs=parsed_config['programs'])
-        return True
+        return "true"
 
     def _filter_public_config(self, config):
         del config['influxdbconn']
         return config
 
     def _change_program(self, program, new_program):
         inputbox_text = new_program['time']
```

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow/wsgi.py` & `piwwwaterflow-0.2.2/piwwwaterflow/wsgi.py`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.2.2/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.2.1/piwwwaterflow.egg-info/SOURCES.txt` & `piwwwaterflow-0.2.2/piwwwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.2.1/setup.py` & `piwwwaterflow-0.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwwwaterflow",
-    version="0.2.1",
+    version="0.2.2",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwwwaterflow",
     packages=setuptools.find_packages(),
```

