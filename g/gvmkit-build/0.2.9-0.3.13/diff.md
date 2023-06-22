# Comparing `tmp/gvmkit_build-0.2.9.tar.gz` & `tmp/gvmkit_build-0.3.13-py3-none-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvmkit_build-0.2.9.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

