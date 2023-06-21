# Comparing `tmp/pymongoarrow-0.7.0.tar.gz` & `tmp/pymongoarrow-1.0.0-cp38-cp38-macosx_10_14_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mongo-arrow/mongo-arrow/bindings/python/dist/.tmp-6d6kosvg/pymongoarrow-0.7.0.tar", last modified: Mon Jan 30 20:00:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

