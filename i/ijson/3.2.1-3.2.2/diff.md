# Comparing `tmp/ijson-3.2.1.tar.gz` & `tmp/ijson-3.2.2-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ijson-3.2.1.tar", last modified: Mon Jun 12 13:23:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

