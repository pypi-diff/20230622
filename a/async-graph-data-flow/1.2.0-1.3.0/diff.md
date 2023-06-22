# Comparing `tmp/async-graph-data-flow-1.2.0.tar.gz` & `tmp/async_graph_data_flow-1.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-graph-data-flow-1.2.0.tar", last modified: Wed Apr 26 14:57:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

