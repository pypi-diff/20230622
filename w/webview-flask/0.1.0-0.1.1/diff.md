# Comparing `tmp/webview_flask-0.1.0.tar.gz` & `tmp/webview_flask-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webview_flask-0.1.0.tar", max compression
+gzip compressed data, was "webview_flask-0.1.1.tar", max compression
```

## Comparing `webview_flask-0.1.0.tar` & `webview_flask-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      549 2023-06-22 11:57:24.242587 webview_flask-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      345 2023-06-22 11:57:24.238587 webview_flask-0.1.0/readme.md
--rw-r--r--   0        0        0       22 2023-06-22 11:57:24.242587 webview_flask-0.1.0/src/webview_flask/__init__.py
--rwxr-xr-x   0        0        0      546 2023-06-22 11:57:24.242587 webview_flask-0.1.0/src/webview_flask/main.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 webview_flask-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      535 2023-06-22 13:05:38.403871 webview_flask-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      599 2023-06-22 13:05:02.525727 webview_flask-0.1.1/readme.md
+-rw-r--r--   0        0        0       22 2023-06-22 13:05:32.780153 webview_flask-0.1.1/src/webview_flask/__init__.py
+-rwxr-xr-x   0        0        0      702 2023-06-22 12:52:22.647590 webview_flask-0.1.1/src/webview_flask/main.py
+-rw-r--r--   0        0        0     1189 1970-01-01 00:00:00.000000 webview_flask-0.1.1/PKG-INFO
```

### Comparing `webview_flask-0.1.0/pyproject.toml` & `webview_flask-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "webview_flask"
-version = "0.1.0"
+version = "0.1.1"
 description = "flask app with webview"
 authors = ["Sander van Dragt <sander@vandragt.com>"]
 readme = "readme.md"
 
 [tool.poetry.dependencies]
-python = ">=3.11,<3.12" #pyinstaller
+python=">=3.8.0,<3.12"
 Flask = "^2.3.2"
 pywebview = "^4.1"
 pygobject = "^3.44.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 vext = "^0.7.6"
```

### Comparing `webview_flask-0.1.0/src/webview_flask/main.py` & `webview_flask-0.1.1/src/webview_flask/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 #!/usr/bin/env python3
 import os
 import webview
 import sys
 from flask import Flask
 
-if getattr(sys, 'frozen', False):
-    template_folder = os.path.join(sys._MEIPASS, 'templates')
-    static_folder = os.path.join(sys._MEIPASS, 'static')
+if getattr(sys, "frozen", False):
+    template_folder = os.path.join(sys._MEIPASS, "templates")
+    static_folder = os.path.join(sys._MEIPASS, "static")
     app = Flask(__name__, template_folder=template_folder, static_folder=static_folder)
 else:
     app = Flask(__name__)
 
+
 @app.route("/")
 def hello_world():
     return "<p>Hello, World!</p>"
 
 
 def main():
-    webview.create_window('Hello world', app)
+    if not (sys.version_info >= (3, 8) and sys.version_info < (3, 12)):
+        print("Python version is not between 3.8 and 3.11.")
+        sys.exit(1)
+
+    webview.create_window("Hello world", app)
     webview.start()
 
+
 if __name__ == "__main__":
     main()
```

