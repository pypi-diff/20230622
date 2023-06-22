# Comparing `tmp/pydraulics-0.1.3.tar.gz` & `tmp/pydraulics-0.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydraulics-0.1.3.tar", last modified: Thu Jun 22 11:07:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

