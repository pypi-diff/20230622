# Comparing `tmp/android-tv-remote-0.1.5.tar.gz` & `tmp/android_tv_remote-0.1.6-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "android-tv-remote-0.1.5.tar", last modified: Tue Jan  4 19:51:37 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

