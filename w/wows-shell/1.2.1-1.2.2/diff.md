# Comparing `tmp/wows_shell-1.2.1.tar.gz` & `tmp/wows_shell-1.2.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wows_shell-1.2.1.tar", last modified: Mon Jun 19 19:00:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

