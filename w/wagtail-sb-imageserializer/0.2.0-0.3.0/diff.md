# Comparing `tmp/wagtail_sb_imageserializer-0.2.0.tar.gz` & `tmp/wagtail_sb_imageserializer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_sb_imageserializer-0.2.0.tar", max compression
+gzip compressed data, was "wagtail_sb_imageserializer-0.3.0.tar", max compression
```

## Comparing `wagtail_sb_imageserializer-0.2.0.tar` & `wagtail_sb_imageserializer-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      166 2023-06-01 04:52:35.471837 wagtail_sb_imageserializer-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-05-14 23:31:08.874809 wagtail_sb_imageserializer-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1794 2023-06-01 04:52:29.051818 wagtail_sb_imageserializer-0.2.0/README.md
--rw-r--r--   0        0        0     2034 2023-06-01 04:52:35.471837 wagtail_sb_imageserializer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       88 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/admin.py
--rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/api/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/api/fields.py
--rw-r--r--   0        0        0      182 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/apps.py
--rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/models.py
--rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/tests.py
--rw-r--r--   0        0        0       20 2023-06-01 04:52:35.471837 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/version.py
--rw-r--r--   0        0        0        0 2023-05-14 23:31:08.878809 wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/views.py
--rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 wagtail_sb_imageserializer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      272 2023-06-22 16:35:22.192421 wagtail_sb_imageserializer-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-06-22 12:48:47.544906 wagtail_sb_imageserializer-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     3707 2023-06-22 12:48:47.544906 wagtail_sb_imageserializer-0.3.0/README.md
+-rw-r--r--   0        0        0     2499 2023-06-22 16:35:22.192421 wagtail_sb_imageserializer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/admin.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/api/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/api/fields.py
+-rw-r--r--   0        0        0      182 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/apps.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/models.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/tests.py
+-rw-r--r--   0        0        0       20 2023-06-22 16:35:22.192421 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/version.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/views.py
+-rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 wagtail_sb_imageserializer-0.3.0/PKG-INFO
```

### Comparing `wagtail_sb_imageserializer-0.2.0/LICENSE.txt` & `wagtail_sb_imageserializer-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_sb_imageserializer-0.2.0/src/wagtail_sb_imageserializer/api/fields.py` & `wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/api/fields.py`

 * *Files identical despite different names*

