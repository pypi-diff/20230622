# Comparing `tmp/plone.namedfile-6.1.0.tar.gz` & `tmp/plone.namedfile-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.namedfile-6.1.0.tar", last modified: Mon May 22 21:09:52 2023, max compression
+gzip compressed data, was "plone.namedfile-6.1.1.tar", last modified: Thu Jun 22 19:12:26 2023, max compression
```

## Comparing `plone.namedfile-6.1.0.tar` & `plone.namedfile-6.1.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:09:52.961444 plone.namedfile-6.1.0/
--rw-r--r--   0 maurits    (501) staff       (20)    20512 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      123 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    36704 2023-05-22 21:09:52.961567 plone.namedfile-6.1.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      777 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:09:52.942435 plone.namedfile-6.1.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1217 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1481 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      457 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/docs/ZPL.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:09:52.942666 plone.namedfile-6.1.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:09:52.952903 plone.namedfile-6.1.0/plone/namedfile/
--rw-r--r--   0 maurits    (501) staff       (20)      214 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5087 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)     7145 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     1233 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      959 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/copy.py
--rw-r--r--   0 maurits    (501) staff       (20)     2388 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/editor.py
--rw-r--r--   0 maurits    (501) staff       (20)      522 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/editor.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3754 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/field.py
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/field.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    12410 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/file.py
--rw-r--r--   0 maurits    (501) staff       (20)      519 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/handler.py
--rw-r--r--   0 maurits    (501) staff       (20)     6201 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/handler.rst
--rw-r--r--   0 maurits    (501) staff       (20)      609 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/handler.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3040 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/marshaler.py
--rw-r--r--   0 maurits    (501) staff       (20)     8283 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/marshaler.rst
--rw-r--r--   0 maurits    (501) staff       (20)      313 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/marshaler.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6218 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/picture.py
--rw-r--r--   0 maurits    (501) staff       (20)    28292 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/scaling.py
--rw-r--r--   0 maurits    (501) staff       (20)     1853 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/scaling.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3164 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/storages.py
--rw-r--r--   0 maurits    (501) staff       (20)     6976 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/test.pt
--rw-r--r--   0 maurits    (501) staff       (20)      881 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)      636 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:09:52.959708 plone.namedfile-6.1.0/plone/namedfile/tests/
--rw-r--r--   0 maurits    (501) staff       (20)   160651 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/900.jpg
--rw-r--r--   0 maurits    (501) staff       (20)      234 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1279 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/dummy.py
--rw-r--r--   0 maurits    (501) staff       (20)     8351 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/file.pdf
--rw-r--r--   0 maurits    (501) staff       (20)      303 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/image.gif
--rw-r--r--   0 maurits    (501) staff       (20)     3641 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/image.jpg
--rw-r--r--   0 maurits    (501) staff       (20)      290 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/image.png
--rw-r--r--   0 maurits    (501) staff       (20)     3823 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/image.svg
--rw-r--r--   0 maurits    (501) staff       (20)   300316 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/image.tif
--rw-r--r--   0 maurits    (501) staff       (20)    13824 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/notimage.doc
--rw-r--r--   0 maurits    (501) staff       (20)     5205 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/test_adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)     4054 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/test_blobfile.py
--rw-r--r--   0 maurits    (501) staff       (20)     5736 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/test_display_file.py
--rw-r--r--   0 maurits    (501) staff       (20)      617 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     4381 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/test_image.py
--rw-r--r--   0 maurits    (501) staff       (20)    38372 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/test_scaling.py
--rw-r--r--   0 maurits    (501) staff       (20)     8577 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/test_scaling_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     2039 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/test_storable.py
--rw-r--r--   0 maurits    (501) staff       (20)     1427 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/test_svg.py
--rw-r--r--   0 maurits    (501) staff       (20)      168 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/tests/tool.gif
--rw-r--r--   0 maurits    (501) staff       (20)    14414 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/usage.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:09:52.961012 plone.namedfile-6.1.0/plone/namedfile/utils/
--rw-r--r--   0 maurits    (501) staff       (20)    11763 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/utils/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1092 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/utils/jpeg_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      866 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/utils/png_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1159 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/utils/svg_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      417 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/utils.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1537 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone/namedfile/z3c-blobfile.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:09:52.944920 plone.namedfile-6.1.0/plone.namedfile.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    36704 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone.namedfile.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2027 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone.namedfile.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone.namedfile.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone.namedfile.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone.namedfile.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      283 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone.namedfile.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/plone.namedfile.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      658 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      244 2023-05-22 21:09:52.962096 plone.namedfile-6.1.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2073 2023-05-22 21:09:52.000000 plone.namedfile-6.1.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:12:26.675692 plone.namedfile-6.1.1/
+-rw-r--r--   0 maurits    (501) staff       (20)    20766 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    36958 2023-06-22 19:12:26.675821 plone.namedfile-6.1.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      777 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:12:26.658629 plone.namedfile-6.1.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1217 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1481 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      457 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/docs/ZPL.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:12:26.658877 plone.namedfile-6.1.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:12:26.668583 plone.namedfile-6.1.1/plone/namedfile/
+-rw-r--r--   0 maurits    (501) staff       (20)      214 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5087 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7145 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1233 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      959 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/copy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2388 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/editor.py
+-rw-r--r--   0 maurits    (501) staff       (20)      522 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/editor.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3754 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/field.py
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/field.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    12410 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/file.py
+-rw-r--r--   0 maurits    (501) staff       (20)      519 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6201 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/handler.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      609 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/handler.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3040 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2902 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/marshaler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8283 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/marshaler.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      313 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/marshaler.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6218 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/picture.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28484 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/scaling.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1853 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/scaling.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3164 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/storages.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6976 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/test.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      881 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/testing.py
+-rw-r--r--   0 maurits    (501) staff       (20)      636 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:12:26.674314 plone.namedfile-6.1.1/plone/namedfile/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)   160651 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/900.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1279 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/dummy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8351 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)      303 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/image.gif
+-rw-r--r--   0 maurits    (501) staff       (20)     3641 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)      290 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/image.png
+-rw-r--r--   0 maurits    (501) staff       (20)     3823 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/image.svg
+-rw-r--r--   0 maurits    (501) staff       (20)   300316 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/image.tif
+-rw-r--r--   0 maurits    (501) staff       (20)    13824 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/notimage.doc
+-rw-r--r--   0 maurits    (501) staff       (20)     5205 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/test_adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4054 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/test_blobfile.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5736 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/test_display_file.py
+-rw-r--r--   0 maurits    (501) staff       (20)      617 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4381 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/test_image.py
+-rw-r--r--   0 maurits    (501) staff       (20)    39328 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/test_scaling.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8812 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/test_scaling_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2039 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/test_storable.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1427 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/test_svg.py
+-rw-r--r--   0 maurits    (501) staff       (20)      168 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/tests/tool.gif
+-rw-r--r--   0 maurits    (501) staff       (20)    14414 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/usage.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:12:26.675409 plone.namedfile-6.1.1/plone/namedfile/utils/
+-rw-r--r--   0 maurits    (501) staff       (20)    11763 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/utils/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1092 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/utils/jpeg_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      866 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/utils/png_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1159 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/utils/svg_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      417 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/utils.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1537 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/plone/namedfile/z3c-blobfile.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:12:26.660952 plone.namedfile-6.1.1/plone.namedfile.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    36958 2023-06-22 19:12:26.000000 plone.namedfile-6.1.1/plone.namedfile.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2027 2023-06-22 19:12:26.000000 plone.namedfile-6.1.1/plone.namedfile.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:12:26.000000 plone.namedfile-6.1.1/plone.namedfile.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:12:26.000000 plone.namedfile-6.1.1/plone.namedfile.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:12:26.000000 plone.namedfile-6.1.1/plone.namedfile.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      283 2023-06-22 19:12:26.000000 plone.namedfile-6.1.1/plone.namedfile.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:12:26.000000 plone.namedfile-6.1.1/plone.namedfile.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      658 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2023-06-22 19:12:26.676278 plone.namedfile-6.1.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2073 2023-06-22 19:12:25.000000 plone.namedfile-6.1.1/setup.py
```

### Comparing `plone.namedfile-6.1.0/CHANGES.rst` & `plone.namedfile-6.1.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.1.1 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Return a 400 Bad Request response if the `@@images` view is published without a subpath. @davisagli (#144)
+
+
+Tests
+
+
+- Fix tests to work with various ``beautifulsoup4`` versions.
+  [maurits] (#867)
+
+
 6.1.0 (2023-05-22)
 ------------------
 
 New features:
 
 
 - Move ``Zope2FileUploadStorable`` code from plone.app.z3cform to here to break a cyclic dependency.
```

### Comparing `plone.namedfile-6.1.0/PKG-INFO` & `plone.namedfile-6.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.namedfile
-Version: 6.1.0
+Version: 6.1.1
 Summary: File types and fields for images, files and blob files with filenames
 Home-page: https://pypi.org/project/plone.namedfile
 Author: Laurence Rowe, Martin Aspeli
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: plone named file image blob
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,14 +57,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.1.1 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Return a 400 Bad Request response if the `@@images` view is published without a subpath. @davisagli (#144)
+
+
+Tests
+
+
+- Fix tests to work with various ``beautifulsoup4`` versions.
+  [maurits] (#867)
+
+
 6.1.0 (2023-05-22)
 ------------------
 
 New features:
 
 
 - Move ``Zope2FileUploadStorable`` code from plone.app.z3cform to here to break a cyclic dependency.
```

### Comparing `plone.namedfile-6.1.0/README.rst` & `plone.namedfile-6.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/docs/INSTALL.txt` & `plone.namedfile-6.1.1/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/docs/LICENSE.txt` & `plone.namedfile-6.1.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/adapters.py` & `plone.namedfile-6.1.1/plone/namedfile/adapters.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/browser.py` & `plone.namedfile-6.1.1/plone/namedfile/browser.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/configure.zcml` & `plone.namedfile-6.1.1/plone/namedfile/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/copy.py` & `plone.namedfile-6.1.1/plone/namedfile/copy.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/editor.py` & `plone.namedfile-6.1.1/plone/namedfile/editor.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/editor.zcml` & `plone.namedfile-6.1.1/plone/namedfile/editor.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/field.py` & `plone.namedfile-6.1.1/plone/namedfile/field.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/file.py` & `plone.namedfile-6.1.1/plone/namedfile/file.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/handler.py` & `plone.namedfile-6.1.1/plone/namedfile/handler.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/handler.rst` & `plone.namedfile-6.1.1/plone/namedfile/handler.rst`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/handler.zcml` & `plone.namedfile-6.1.1/plone/namedfile/handler.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/interfaces.py` & `plone.namedfile-6.1.1/plone/namedfile/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/marshaler.py` & `plone.namedfile-6.1.1/plone/namedfile/marshaler.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/marshaler.rst` & `plone.namedfile-6.1.1/plone/namedfile/marshaler.rst`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/picture.py` & `plone.namedfile-6.1.1/plone/namedfile/picture.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/scaling.py` & `plone.namedfile-6.1.1/plone/namedfile/scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 from plone.scale.interfaces import IScaledImageQuality
 from plone.scale.scale import scaleImage
 from plone.scale.storage import IImageScaleStorage
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.utils import safe_encode
 from Products.Five import BrowserView
 from xml.sax.saxutils import quoteattr
+from zExceptions import BadRequest
 from zExceptions import Unauthorized
 from ZODB.blob import BlobFile
 from ZODB.POSException import ConflictError
 from zope.cachedescriptors.property import Lazy as lazy_property
 from zope.component import getMultiAdapter
 from zope.component import queryUtility
 from zope.deprecation import deprecate
 from zope.interface import alsoProvides
 from zope.interface import implementer
-from zope.publisher.interfaces import IPublishTraverse
+from zope.publisher.interfaces.browser import IBrowserPublisher
 from zope.publisher.interfaces import NotFound
 from zope.traversing.interfaces import ITraversable
 from zope.traversing.interfaces import TraversalError
 
 import functools
 import logging
 import warnings
@@ -386,15 +387,15 @@
             filename=orig_value.filename,
         )
         value.fieldname = self.fieldname
 
         return value, format_, dimensions
 
 
-@implementer(ITraversable, IPublishTraverse)
+@implementer(ITraversable, IBrowserPublisher)
 class ImageScaling(BrowserView):
     """view used for generating (and storing) image scales"""
 
     # Ignore some stacks to help with accessing via webdav, otherwise you get a
     # 404 NotFound error.
     _ignored_stacks = ("manage_DAVget", "manage_FTPget")
     _scale_view_class = ImageScale
@@ -430,14 +431,18 @@
                 self.request,
                 data=value,
                 fieldname=name,
             )
             return scale_view
         raise NotFound(self, name, self.request)
 
+    def browserDefault(self, request):
+        # There's nothing in the path after /@@images
+        raise BadRequest("Missing image scale path")
+
     def traverse(self, name, furtherPath):
         """used for path traversal, i.e. in zope page templates"""
         # validate access
         value = self.guarded_orig_image(name)
         if not furtherPath:
             image = self._scale_view_class(
                 self.context,
```

### Comparing `plone.namedfile-6.1.0/plone/namedfile/scaling.zcml` & `plone.namedfile-6.1.1/plone/namedfile/scaling.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/storages.py` & `plone.namedfile-6.1.1/plone/namedfile/storages.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/test.pt` & `plone.namedfile-6.1.1/plone/namedfile/test.pt`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/testing.py` & `plone.namedfile-6.1.1/plone/namedfile/testing.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/testing.zcml` & `plone.namedfile-6.1.1/plone/namedfile/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/900.jpg` & `plone.namedfile-6.1.1/plone/namedfile/tests/900.jpg`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/dummy.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/file.pdf` & `plone.namedfile-6.1.1/plone/namedfile/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/image.jpg` & `plone.namedfile-6.1.1/plone/namedfile/tests/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/image.svg` & `plone.namedfile-6.1.1/plone/namedfile/tests/image.svg`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/image.tif` & `plone.namedfile-6.1.1/plone/namedfile/tests/image.tif`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/notimage.doc` & `plone.namedfile-6.1.1/plone/namedfile/tests/notimage.doc`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/test_adapters.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/test_blobfile.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/test_blobfile.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/test_display_file.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/test_display_file.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/test_doctests.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/test_image.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/test_scaling.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/test_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -543,17 +543,25 @@
         tag = self.scaling.picture("image", picture_variant="medium")
         expected = """<picture>
  <source srcset="http://nohost/item/@@images/image-600-....png 600w,
 http://nohost/item/@@images/image-400-....png 400w,
 http://nohost/item/@@images/image-800-....png 800w,
 http://nohost/item/@@images/image-1000-....png 1000w,
 http://nohost/item/@@images/image-1200-....png 1200w"/>
- <img height="200" loading="lazy" src="http://nohost/item/@@images/image-600-....png" title="foo" width="200"/>
+ <img...src="http://nohost/item/@@images/image-600-....png".../>
 </picture>"""
-        self.assertTrue(_ellipsis_match(expected, tag))
+        self.assertTrue(_ellipsis_match(expected, tag.strip()))
+
+        # The exact placement of the img tag attributes can differ, especially
+        # with different beautifulsoup versions.
+        # So check here that all attributes are present.
+        self.assertIn('height="200"', tag)
+        self.assertIn('loading="lazy"', tag)
+        self.assertIn('title="foo"', tag)
+        self.assertIn('width="200"', tag)
 
     @patch.object(
         plone.namedfile.scaling,
         "get_picture_variants",
         new=patch_Img2PictureTag_picture_variants,
         spec=True,
     )
@@ -576,17 +584,26 @@
         base = self.item.absolute_url()
         expected = f"""<picture>
  <source srcset="{base}/@@images/image-600-....png 600w,
 {base}/@@images/image-400-....png 400w,
 {base}/@@images/image-800-....png 800w,
 {base}/@@images/image-1000-....png 1000w,
 {base}/@@images/image-1200-....png 1200w"/>
- <img alt="Alternative text" height="200" loading="lazy" src="{base}/@@images/image-600-....png" title="Custom title" width="200"/>
+ <img...src="{base}/@@images/image-600-....png".../>
 </picture>"""
-        self.assertTrue(_ellipsis_match(expected, tag))
+        self.assertTrue(_ellipsis_match(expected, tag.strip()))
+
+        # The exact placement of the img tag attributes can differ, especially
+        # with different beautifulsoup versions.
+        # So check here that all attributes are present.
+        self.assertIn('alt="Alternative text"', tag)
+        self.assertIn('height="200"', tag)
+        self.assertIn('loading="lazy"', tag)
+        self.assertIn('title="Custom title"', tag)
+        self.assertIn('width="200"', tag)
 
     @patch.object(
         plone.namedfile.scaling,
         "get_picture_variants",
         new=patch_Img2PictureTag_empty_picture_variants,
         spec=True,
     )
@@ -597,16 +614,23 @@
         spec=True,
     )
     @patch.object(plone.namedfile.picture, "uuidToObject", spec=True)
     def testGetPictureTagWithoutAnyVariants(self, mock_uuid_to_object):
         ImageScaling._sizes = patch_Img2PictureTag_allowed_scales()
         mock_uuid_to_object.return_value = self.item
         tag = self.scaling.picture("image", picture_variant="medium")
-        expected = """<img src="http://nohost/item/@@images/image-0-....png" title="foo" height="200" width="200" />"""
-        self.assertTrue(_ellipsis_match(expected, tag))
+        expected = """<img...src="http://nohost/item/@@images/image-0-....png".../>"""
+        self.assertTrue(_ellipsis_match(expected, tag.strip()))
+
+        # The exact placement of the img tag attributes can differ, especially
+        # with different beautifulsoup versions.
+        # So check here that all attributes are present.
+        self.assertIn('height="200"', tag)
+        self.assertIn('title="foo"', tag)
+        self.assertIn('width="200"', tag)
 
     def testGetUnknownScale(self):
         foo = self.scaling.scale("image", scale="foo?")
         self.assertEqual(foo, None)
 
     def testScaleInvalidation(self):
         dt = self.item.modified()
```

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/test_scaling_functional.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/test_scaling_functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from plone.namedfile.field import NamedImage as NamedImageField
 from plone.namedfile.file import NamedImage
 from plone.namedfile.interfaces import IImageScaleTraversable
 from plone.namedfile.scaling import ImageScaling
 from plone.namedfile.testing import PLONE_NAMEDFILE_FUNCTIONAL_TESTING
 from plone.namedfile.tests import getFile
 from plone.testing.zope import Browser
+from zExceptions import BadRequest
 from zope.annotation import IAttributeAnnotatable
 from zope.interface import implementer
 
 import PIL
 import transaction
 import unittest
 
@@ -211,12 +212,17 @@
         # and last a scaled version
         self.browser.open(
             self.layer["app"].absolute_url() + "/svg/@@images/image/thumb"
         )
         self.assertEqual("image/svg+xml", self.browser.headers["content-type"])
         self.assertEqual(self.browser.contents, data)
 
+    def testImagesViewWithNoSubpath(self):
+        transaction.commit()
+        with self.assertRaises(BadRequest):
+            self.browser.open(self.layer["app"].absolute_url() + "/item/@@images")
+
 
 def test_suite():
     from unittest import defaultTestLoader
 
     return defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/test_storable.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/test_storable.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/tests/test_svg.py` & `plone.namedfile-6.1.1/plone/namedfile/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/usage.rst` & `plone.namedfile-6.1.1/plone/namedfile/usage.rst`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/utils/__init__.py` & `plone.namedfile-6.1.1/plone/namedfile/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/utils/jpeg_utils.py` & `plone.namedfile-6.1.1/plone/namedfile/utils/jpeg_utils.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/utils/png_utils.py` & `plone.namedfile-6.1.1/plone/namedfile/utils/png_utils.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/utils/svg_utils.py` & `plone.namedfile-6.1.1/plone/namedfile/utils/svg_utils.py`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone/namedfile/z3c-blobfile.zcml` & `plone.namedfile-6.1.1/plone/namedfile/z3c-blobfile.zcml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/plone.namedfile.egg-info/PKG-INFO` & `plone.namedfile-6.1.1/plone.namedfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.namedfile
-Version: 6.1.0
+Version: 6.1.1
 Summary: File types and fields for images, files and blob files with filenames
 Home-page: https://pypi.org/project/plone.namedfile
 Author: Laurence Rowe, Martin Aspeli
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: plone named file image blob
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,14 +57,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.1.1 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Return a 400 Bad Request response if the `@@images` view is published without a subpath. @davisagli (#144)
+
+
+Tests
+
+
+- Fix tests to work with various ``beautifulsoup4`` versions.
+  [maurits] (#867)
+
+
 6.1.0 (2023-05-22)
 ------------------
 
 New features:
 
 
 - Move ``Zope2FileUploadStorable`` code from plone.app.z3cform to here to break a cyclic dependency.
```

### Comparing `plone.namedfile-6.1.0/plone.namedfile.egg-info/SOURCES.txt` & `plone.namedfile-6.1.1/plone.namedfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/pyproject.toml` & `plone.namedfile-6.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.namedfile-6.1.0/setup.py` & `plone.namedfile-6.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "6.1.0"
+version = "6.1.1"
 
 description = "File types and fields for images, files and blob files with " "filenames"
 long_description = "\n\n".join(
     [
         open("README.rst").read(),
         open("CHANGES.rst").read(),
         open(os.path.join("plone", "namedfile", "usage.rst")).read(),
```

