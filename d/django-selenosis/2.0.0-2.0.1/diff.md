# Comparing `tmp/django-selenosis-2.0.0.tar.gz` & `tmp/django_selenosis-2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-selenosis-2.0.0.tar", last modified: Thu Jul  8 17:48:00 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

