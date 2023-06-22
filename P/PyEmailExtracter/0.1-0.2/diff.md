# Comparing `tmp/PyEmailExtracter-0.1.tar.gz` & `tmp/PyEmailExtracter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailExtracter-0.1.tar", last modified: Thu Jun 22 09:37:55 2023, max compression
+gzip compressed data, was "PyEmailExtracter-0.2.tar", last modified: Thu Jun 22 10:21:28 2023, max compression
```

## Comparing `PyEmailExtracter-0.1.tar` & `PyEmailExtracter-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 09:37:55.399383 PyEmailExtracter-0.1/
--rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 09:37:55.399383 PyEmailExtracter-0.1/PKG-INFO
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 09:37:55.399383 PyEmailExtracter-0.1/PyEmailExtracter/
--rw-rw-r--   0 karki     (1000) karki     (1000)        0 2023-06-22 09:24:52.000000 PyEmailExtracter-0.1/PyEmailExtracter/__init__.py
--rw-rw-r--   0 karki     (1000) karki     (1000)      750 2023-06-22 09:36:43.000000 PyEmailExtracter-0.1/PyEmailExtracter/driver.py
--rw-rw-r--   0 karki     (1000) karki     (1000)     1898 2023-06-22 09:32:55.000000 PyEmailExtracter-0.1/PyEmailExtracter/helper.py
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 09:37:55.399383 PyEmailExtracter-0.1/PyEmailExtracter.egg-info/
--rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 09:37:55.000000 PyEmailExtracter-0.1/PyEmailExtracter.egg-info/PKG-INFO
--rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-22 09:37:55.000000 PyEmailExtracter-0.1/PyEmailExtracter.egg-info/SOURCES.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-22 09:37:55.000000 PyEmailExtracter-0.1/PyEmailExtracter.egg-info/dependency_links.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       81 2023-06-22 09:37:55.000000 PyEmailExtracter-0.1/PyEmailExtracter.egg-info/requires.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-22 09:37:55.000000 PyEmailExtracter-0.1/PyEmailExtracter.egg-info/top_level.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)        0 2023-06-22 09:26:17.000000 PyEmailExtracter-0.1/README.md
--rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-22 09:37:55.399383 PyEmailExtracter-0.1/setup.cfg
--rw-rw-r--   0 karki     (1000) karki     (1000)      471 2023-06-22 09:32:02.000000 PyEmailExtracter-0.1/setup.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 10:21:28.463800 PyEmailExtracter-0.2/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 10:21:28.463800 PyEmailExtracter-0.2/PKG-INFO
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 10:21:28.463800 PyEmailExtracter-0.2/PyEmailExtracter/
+-rw-rw-r--   0 karki     (1000) karki     (1000)        0 2023-06-22 09:24:52.000000 PyEmailExtracter-0.2/PyEmailExtracter/__init__.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)      957 2023-06-22 10:21:01.000000 PyEmailExtracter-0.2/PyEmailExtracter/driver.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1898 2023-06-22 09:32:55.000000 PyEmailExtracter-0.2/PyEmailExtracter/helper.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 10:21:28.463800 PyEmailExtracter-0.2/PyEmailExtracter.egg-info/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 10:21:28.000000 PyEmailExtracter-0.2/PyEmailExtracter.egg-info/PKG-INFO
+-rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-22 10:21:28.000000 PyEmailExtracter-0.2/PyEmailExtracter.egg-info/SOURCES.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-22 10:21:28.000000 PyEmailExtracter-0.2/PyEmailExtracter.egg-info/dependency_links.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       81 2023-06-22 10:21:28.000000 PyEmailExtracter-0.2/PyEmailExtracter.egg-info/requires.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-22 10:21:28.000000 PyEmailExtracter-0.2/PyEmailExtracter.egg-info/top_level.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)        0 2023-06-22 09:26:17.000000 PyEmailExtracter-0.2/README.md
+-rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-22 10:21:28.463800 PyEmailExtracter-0.2/setup.cfg
+-rw-rw-r--   0 karki     (1000) karki     (1000)      471 2023-06-22 10:21:25.000000 PyEmailExtracter-0.2/setup.py
```

### Comparing `PyEmailExtracter-0.1/PyEmailExtracter/driver.py` & `PyEmailExtracter-0.2/PyEmailExtracter/driver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from helper import *
 
 
-# Example: "/home/user_name/some_directory/resumes"
-directory = str(input("Paste the absolute path of the directory and press enter.\n"))
-file_extensions = [".docx", ".pdf"]
-files = fetch_files(directory, file_extensions)
+def extract_emails(dir=""):
+    # Example: "/home/user_name/some_directory/resumes"
+    # directory = str(
+    #     input("Paste the absolute path of the directory and press enter.\n")
+    # )
+    directory = str(dir)
+    file_extensions = [".docx", ".pdf"]
+    files = fetch_files(directory, file_extensions)
 
-with open("total_files.txt", "a") as f:
-    f.write("Total files fetched: \n" + str(len(files)) + "\n")
+    # with open("total_files.txt", "a") as f:
+    #     f.write("Total files fetched: \n" + str(len(files)) + "\n")
+    arr = []
 
-
-for file in files:
-    current_ext = str(file).split(".")[1]
-    if current_ext == "pdf":
-        emails = extract_email_from_pdf(file)
-    elif current_ext == "docx":
-        emails = extract_email_from_docx(file)
-    else:
-        print("Currently we dont support ", str(current_ext))
-    for email in emails:
-        with open("email_list.txt", "a") as f:
-            f.write(str(email) + "\n")
+    for file in files:
+        current_ext = str(file).split(".")[1]
+        if current_ext == "pdf":
+            emails = extract_email_from_pdf(file)
+        elif current_ext == "docx":
+            emails = extract_email_from_docx(file)
+        else:
+            print("Currently we dont support ", str(current_ext))
+        for email in emails:
+            arr.append(email)
+            # with open("email_list.txt", "a") as f:
+            #     f.write(str(email) + "\n")\
+    return arr
```

### Comparing `PyEmailExtracter-0.1/PyEmailExtracter/helper.py` & `PyEmailExtracter-0.2/PyEmailExtracter/helper.py`

 * *Files identical despite different names*

