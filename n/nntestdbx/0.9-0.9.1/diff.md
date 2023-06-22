# Comparing `tmp/nntestdbx-0.9-py3-none-any.whl.zip` & `tmp/nntestdbx-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 1507 bytes, number of entries: 6
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 15:52 nntestdbx/__init__.py
--rw-r--r--  2.0 unx      262 b- defN 23-Jun-21 15:52 nntestdbx/sentence_model.py
--rw-r--r--  2.0 unx      135 b- defN 23-Jun-21 15:52 nntestdbx-0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 15:52 nntestdbx-0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-21 15:52 nntestdbx-0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      455 b- defN 23-Jun-21 15:52 nntestdbx-0.9.dist-info/RECORD
-6 files, 954 bytes uncompressed, 677 bytes compressed:  29.0%
+Zip file size: 1916 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 16:21 modelutils/__init__.py
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-21 16:21 modelutils/modelutils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 16:21 nntestdbx/__init__.py
+-rw-r--r--  2.0 unx      250 b- defN 23-Jun-21 16:21 nntestdbx/sentence_model.py
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-21 16:21 nntestdbx-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 16:21 nntestdbx-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-21 16:21 nntestdbx-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      619 b- defN 23-Jun-21 16:21 nntestdbx-0.9.1.dist-info/RECORD
+8 files, 1220 bytes uncompressed, 826 bytes compressed:  32.3%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
+Filename: modelutils/__init__.py
+Comment: 
+
+Filename: modelutils/modelutils.py
+Comment: 
+
 Filename: nntestdbx/__init__.py
 Comment: 
 
 Filename: nntestdbx/sentence_model.py
 Comment: 
 
-Filename: nntestdbx-0.9.dist-info/METADATA
+Filename: nntestdbx-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: nntestdbx-0.9.dist-info/WHEEL
+Filename: nntestdbx-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: nntestdbx-0.9.dist-info/top_level.txt
+Filename: nntestdbx-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nntestdbx-0.9.dist-info/RECORD
+Filename: nntestdbx-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nntestdbx/sentence_model.py

```diff
@@ -1,11 +1,10 @@
 from modelutils.modelutils import TextUtils
 
 
 class SentenceModel(TextUtils):
     def __init__(self) -> None:
         pass
 
-    @staticmethod
-    def sentence_to_words(s: str) -> list:
+    def sentence_to_words(self, s: str) -> list:
         s_capit = self.capitalize_string(s)
         return s_capit.split(" ")
```

