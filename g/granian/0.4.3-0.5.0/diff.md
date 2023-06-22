# Comparing `tmp/granian-0.4.3.tar.gz` & `tmp/granian-0.5.0-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

