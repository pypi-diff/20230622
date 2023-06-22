# Comparing `tmp/gpged-0.0.1.tar.gz` & `tmp/gpged-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpged-0.0.1.tar", last modified: Wed Jun 21 18:32:36 2023, max compression
+gzip compressed data, was "gpged-0.0.2.tar", last modified: Thu Jun 22 14:20:27 2023, max compression
```

## Comparing `gpged-0.0.1.tar` & `gpged-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-21 18:32:36.049410 gpged-0.0.1/
--rw-r--r--   0 sky        (501) staff       (20)     1048 2023-06-20 14:50:03.000000 gpged-0.0.1/LICENSE
--rw-r--r--   0 sky        (501) staff       (20)     1599 2023-06-21 18:32:36.049247 gpged-0.0.1/PKG-INFO
--rw-r--r--   0 sky        (501) staff       (20)       25 2023-06-20 14:49:41.000000 gpged-0.0.1/README.md
-drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-21 18:32:36.047966 gpged-0.0.1/gpged/
--rw-r--r--   0 sky        (501) staff       (20)       71 2023-06-20 14:44:22.000000 gpged-0.0.1/gpged/__init__.py
--rw-r--r--   0 sky        (501) staff       (20)      582 2023-06-20 15:19:09.000000 gpged-0.0.1/gpged/__main__.py
--rw-r--r--   0 sky        (501) staff       (20)     5898 2023-06-20 15:51:47.000000 gpged-0.0.1/gpged/app.py
--rw-r--r--   0 sky        (501) staff       (20)      213 2023-06-20 15:16:49.000000 gpged-0.0.1/gpged/run_gpged.py
-drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-21 18:32:36.048980 gpged-0.0.1/gpged.egg-info/
--rw-r--r--   0 sky        (501) staff       (20)     1599 2023-06-21 18:32:36.000000 gpged-0.0.1/gpged.egg-info/PKG-INFO
--rw-r--r--   0 sky        (501) staff       (20)      281 2023-06-21 18:32:36.000000 gpged-0.0.1/gpged.egg-info/SOURCES.txt
--rw-r--r--   0 sky        (501) staff       (20)        1 2023-06-21 18:32:36.000000 gpged-0.0.1/gpged.egg-info/dependency_links.txt
--rw-r--r--   0 sky        (501) staff       (20)       42 2023-06-21 18:32:36.000000 gpged-0.0.1/gpged.egg-info/entry_points.txt
--rw-r--r--   0 sky        (501) staff       (20)        6 2023-06-21 18:32:36.000000 gpged-0.0.1/gpged.egg-info/top_level.txt
--rw-r--r--   0 sky        (501) staff       (20)        1 2023-06-21 18:32:36.000000 gpged-0.0.1/gpged.egg-info/zip-safe
--rw-r--r--   0 sky        (501) staff       (20)      533 2023-06-21 18:32:22.000000 gpged-0.0.1/pyproject.toml
--rw-r--r--   0 sky        (501) staff       (20)       38 2023-06-21 18:32:36.049464 gpged-0.0.1/setup.cfg
--rw-r--r--   0 sky        (501) staff       (20)     1054 2023-06-21 18:32:32.000000 gpged-0.0.1/setup.py
+drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-22 14:20:27.533016 gpged-0.0.2/
+-rw-r--r--   0 sky        (501) staff       (20)     1048 2023-06-20 14:50:03.000000 gpged-0.0.2/LICENSE
+-rw-r--r--   0 sky        (501) staff       (20)     2283 2023-06-22 14:20:27.532857 gpged-0.0.2/PKG-INFO
+-rw-r--r--   0 sky        (501) staff       (20)      772 2023-06-22 14:17:28.000000 gpged-0.0.2/README.md
+drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-22 14:20:27.531280 gpged-0.0.2/gpged/
+-rw-r--r--   0 sky        (501) staff       (20)       72 2023-06-22 13:29:38.000000 gpged-0.0.2/gpged/__init__.py
+-rw-r--r--   0 sky        (501) staff       (20)      579 2023-06-22 13:29:38.000000 gpged-0.0.2/gpged/__main__.py
+-rw-r--r--   0 sky        (501) staff       (20)     5830 2023-06-22 13:48:39.000000 gpged-0.0.2/gpged/app.py
+-rw-r--r--   0 sky        (501) staff       (20)      215 2023-06-22 13:29:38.000000 gpged-0.0.2/gpged/run_gpged.py
+drwxr-xr-x   0 sky        (501) staff       (20)        0 2023-06-22 14:20:27.532574 gpged-0.0.2/gpged.egg-info/
+-rw-r--r--   0 sky        (501) staff       (20)     2283 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/PKG-INFO
+-rw-r--r--   0 sky        (501) staff       (20)      248 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/SOURCES.txt
+-rw-r--r--   0 sky        (501) staff       (20)        1 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/dependency_links.txt
+-rw-r--r--   0 sky        (501) staff       (20)       42 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/entry_points.txt
+-rw-r--r--   0 sky        (501) staff       (20)        6 2023-06-22 14:20:27.000000 gpged-0.0.2/gpged.egg-info/top_level.txt
+-rw-r--r--   0 sky        (501) staff       (20)      616 2023-06-22 14:17:54.000000 gpged-0.0.2/pyproject.toml
+-rw-r--r--   0 sky        (501) staff       (20)       38 2023-06-22 14:20:27.533070 gpged-0.0.2/setup.cfg
```

### Comparing `gpged-0.0.1/LICENSE` & `gpged-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpged-0.0.1/PKG-INFO` & `gpged-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: gpged
-Version: 0.0.1
+Version: 0.0.2
 Summary: GUI for encrypting and decrypting text with GPG.
-Home-page: https://github.com/skymoore/gpged
-Author: Sky Moore
 Author-email: Sky Moore <i@msky.me>
 License: Copyright 2022 Sky Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -15,8 +13,28 @@
 Keywords: gpg,gnupg,pgp,gui,encryption,decryption,cryptography
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GPG Encrypt Decrypt GUI
+# GPG Encrypt Decrypt GUI: gpged
+> `gpged` is a QT6 python application that makes use of GnuPG to present a simple interface for basic pgp operations.
+
+## Install with Pip from Pypi:  
+`pip install gpged`
+## Install with Pip from source:  
+```bash
+# clone the repo then
+cd gpged
+pip install .
+```
+## Install with pipenv from source:  
+`pipenv install --system --deploy`
+## Run gpged
+`gpged`
+### Nice UI  
+![layout](https://github.com/skymoore/gpged/blob/main/gpged/images/layout.png?raw=true)
+### Encrypt with multiple public keys  
+![multi-key select](https://github.com/skymoore/gpged/blob/main/gpged/images/multi_key_select.png?raw=true)
+### Decrypt messages  
+![decypted message](https://github.com/skymoore/gpged/blob/main/gpged/images/decrypted_message.png?raw=true)
```

### Comparing `gpged-0.0.1/gpged/__main__.py` & `gpged-0.0.2/gpged/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import argparse
 import os
 import sys
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('-d', action='store_true')
+    parser.add_argument("-d", action="store_true")
     args = parser.parse_args()
 
     if not args.d:
         script_dir = os.path.dirname(os.path.realpath(__file__))
-        script_path = os.path.join(script_dir, 'run_gpged.py')
+        script_path = os.path.join(script_dir, "run_gpged.py")
         subprocess.Popen([sys.executable, script_path])
         sys.exit(0)
 
     # If -d flag was supplied, run the application in the current process
     run_app()
-    
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `gpged-0.0.1/gpged.egg-info/PKG-INFO` & `gpged-0.0.2/gpged.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: gpged
-Version: 0.0.1
+Version: 0.0.2
 Summary: GUI for encrypting and decrypting text with GPG.
-Home-page: https://github.com/skymoore/gpged
-Author: Sky Moore
 Author-email: Sky Moore <i@msky.me>
 License: Copyright 2022 Sky Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -15,8 +13,28 @@
 Keywords: gpg,gnupg,pgp,gui,encryption,decryption,cryptography
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# GPG Encrypt Decrypt GUI
+# GPG Encrypt Decrypt GUI: gpged
+> `gpged` is a QT6 python application that makes use of GnuPG to present a simple interface for basic pgp operations.
+
+## Install with Pip from Pypi:  
+`pip install gpged`
+## Install with Pip from source:  
+```bash
+# clone the repo then
+cd gpged
+pip install .
+```
+## Install with pipenv from source:  
+`pipenv install --system --deploy`
+## Run gpged
+`gpged`
+### Nice UI  
+![layout](https://github.com/skymoore/gpged/blob/main/gpged/images/layout.png?raw=true)
+### Encrypt with multiple public keys  
+![multi-key select](https://github.com/skymoore/gpged/blob/main/gpged/images/multi_key_select.png?raw=true)
+### Decrypt messages  
+![decypted message](https://github.com/skymoore/gpged/blob/main/gpged/images/decrypted_message.png?raw=true)
```

### Comparing `gpged-0.0.1/pyproject.toml` & `gpged-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "gpged"
-version = "0.0.1"
+version = "0.0.2"
 description = "GUI for encrypting and decrypting text with GPG."
 readme = "README.md"
 authors = [{name = "Sky Moore", email = "i@msky.me"}]
 license = {file = "LICENSE"}
 keywords = ["gpg","gnupg", "pgp", "gui", "encryption", "decryption", "cryptography"]
 classifiers = [
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.10",
 ]
 
 [project.gui-scripts]
 gpged = "gpged.__main__:main"
+
+[options]
+py_modules = ["gpged"]
+packages = ["gpged"]
+include_package_data = true
```

