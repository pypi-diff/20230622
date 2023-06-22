# Comparing `tmp/docleaf-0.7.0-cp39-none-win_amd64.whl.zip` & `tmp/docleaf-0.8.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1076059 bytes, number of entries: 10
--rw-r--r--  4.6 unx     6823 b- defN 23-Jun-22 13:26 docleaf-0.7.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jun-22 13:26 docleaf-0.7.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3573 b- defN 23-Jun-22 13:26 docleaf-0.7.0.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx     5450 b- defN 23-Jun-22 13:26 docleaf/copied.py
--rw-r--r--  4.6 unx     3709 b- defN 23-Jun-22 13:26 docleaf/domains.py
--rw-r--r--  4.6 unx    17707 b- defN 23-Jun-22 13:26 docleaf/doxygen.py
--rw-r--r--  4.6 unx       99 b- defN 23-Jun-22 13:26 docleaf/errors.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-22 13:26 docleaf/__init__.py
--rwxr-xr-x  4.6 unx  3032576 b- defN 23-Jun-22 13:26 docleaf/backend.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      775 b- defN 23-Jun-22 13:26 docleaf-0.7.0.dist-info/RECORD
-10 files, 3070808 bytes uncompressed, 1074753 bytes compressed:  65.0%
+Zip file size: 1076466 bytes, number of entries: 10
+-rw-r--r--  4.6 unx     6823 b- defN 23-Jun-22 14:41 docleaf-0.8.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Jun-22 14:41 docleaf-0.8.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3573 b- defN 23-Jun-22 14:41 docleaf-0.8.0.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx     5450 b- defN 23-Jun-22 14:41 docleaf/copied.py
+-rw-r--r--  4.6 unx     3709 b- defN 23-Jun-22 14:41 docleaf/domains.py
+-rw-r--r--  4.6 unx    17707 b- defN 23-Jun-22 14:41 docleaf/doxygen.py
+-rw-r--r--  4.6 unx       99 b- defN 23-Jun-22 14:41 docleaf/errors.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-22 14:41 docleaf/__init__.py
+-rwxr-xr-x  4.6 unx  3032576 b- defN 23-Jun-22 14:41 docleaf/backend.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      775 b- defN 23-Jun-22 14:41 docleaf-0.8.0.dist-info/RECORD
+10 files, 3070808 bytes uncompressed, 1075160 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: docleaf-0.7.0.dist-info/METADATA
+Filename: docleaf-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: docleaf-0.7.0.dist-info/WHEEL
+Filename: docleaf-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: docleaf-0.7.0.dist-info/license_files/LICENSE.md
+Filename: docleaf-0.8.0.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: docleaf/copied.py
 Comment: 
 
 Filename: docleaf/domains.py
 Comment: 
@@ -21,11 +21,11 @@
 
 Filename: docleaf/__init__.py
 Comment: 
 
 Filename: docleaf/backend.cp39-win_amd64.pyd
 Comment: 
 
-Filename: docleaf-0.7.0.dist-info/RECORD
+Filename: docleaf-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `docleaf-0.7.0.dist-info/METADATA` & `docleaf-0.8.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: docleaf
-Version: 0.7.0
+Version: 0.8.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Requires-Dist: docutils>=0.12
 Requires-Dist: Sphinx>=4.0,<6,!=5.0.0
 License-File: LICENSE.md
 Summary: Integrate your doxygen-generated technical documentation into Sphinx
 Keywords: sphinx,doxygen
 Author-email: Michael Jones <michael.jones@docleaf.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: repository, https://github.com/docleaf-labs/docleaf
 Project-URL: homepage, https://docleaf.io
 Project-URL: changelog, https://github.com/docleaf-labs/docleaf/blob/main/CHANGELOG.md
-Project-URL: repository, https://github.com/docleaf-labs/docleaf
 
 <h1 align="center">
   Docleaf
 </h1>
 
 <p align="center">
    Your technical docs, beautifully integrated
```

## Comparing `docleaf-0.7.0.dist-info/license_files/LICENSE.md` & `docleaf-0.8.0.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

## Comparing `docleaf-0.7.0.dist-info/RECORD` & `docleaf-0.8.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-docleaf-0.7.0.dist-info/METADATA,sha256=qbq9wq51DvCrIHQgCotvbhcQTBadHQhU6YtZgAw0mjo,6823
-docleaf-0.7.0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
-docleaf-0.7.0.dist-info/license_files/LICENSE.md,sha256=ffIj5xgqX0xL1nd3_5YbHFc3paR7y61W6f1780Gp3lE,3573
+docleaf-0.8.0.dist-info/METADATA,sha256=dMLzC8NllZW9kIOjl5zWqxDx-JRp3s0SYEit2BipYQA,6823
+docleaf-0.8.0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
+docleaf-0.8.0.dist-info/license_files/LICENSE.md,sha256=ffIj5xgqX0xL1nd3_5YbHFc3paR7y61W6f1780Gp3lE,3573
 docleaf/copied.py,sha256=ikpVxMGeWhq1ZdUIiCEgIEfGsWgVzPX7uwGS7DdqaxU,5450
 docleaf/domains.py,sha256=5My3c04BEfWSBngVYiZqgxvkh_F09GfEmzgKiJkOa0o,3709
 docleaf/doxygen.py,sha256=q0UY8hJIr9Kau1igQF1j6b2t7QIXOkHXEt7DgP4VafM,17707
 docleaf/errors.py,sha256=sUYIqy64k8zKQ-cZjVzF6auax0klQ9FibFmKOCD9v2Y,99
 docleaf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-docleaf/backend.cp39-win_amd64.pyd,sha256=9N32DNcSGC7oCtXAe3yZe_QNTRKyWolvBjFETeWijUs,3032576
-docleaf-0.7.0.dist-info/RECORD,,
+docleaf/backend.cp39-win_amd64.pyd,sha256=iQe24t_rfZH6z_6Y1E_bqdhLRuLa7ZkJfoDaYqVRwr0,3032576
+docleaf-0.8.0.dist-info/RECORD,,
```

