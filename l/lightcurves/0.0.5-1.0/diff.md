# Comparing `tmp/lightcurves-0.0.5.tar.gz` & `tmp/lightcurves-1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcurves-0.0.5.tar", last modified: Tue Jun  7 23:24:41 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

