# Comparing `tmp/abejacli-2.1.0rc1-py3-none-any.whl.zip` & `tmp/abejacli-2.2.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 80414 bytes, number of entries: 50
+Zip file size: 80412 bytes, number of entries: 50
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abejacli/__init__.py
 -rw-r--r--  2.0 unx     3756 b- defN 80-Jan-01 00:00 abejacli/bucket/__init__.py
 -rw-r--r--  2.0 unx     4355 b- defN 80-Jan-01 00:00 abejacli/bucket/download_job.py
 -rw-r--r--  2.0 unx     6484 b- defN 80-Jan-01 00:00 abejacli/bucket/process_file_job.py
 -rw-r--r--  2.0 unx     3200 b- defN 80-Jan-01 00:00 abejacli/bucket/upload_job.py
 -rw-r--r--  2.0 unx     5354 b- defN 80-Jan-01 00:00 abejacli/click_custom.py
 -rw-r--r--  2.0 unx     5278 b- defN 80-Jan-01 00:00 abejacli/common/__init__.py
@@ -40,13 +40,13 @@
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 abejacli/template/requirements-local.txt-tpl
 -rw-r--r--  2.0 unx     1432 b- defN 80-Jan-01 00:00 abejacli/template/train.py-tpl
 -rw-r--r--  2.0 unx     6891 b- defN 80-Jan-01 00:00 abejacli/training/__init__.py
 -rw-r--r--  2.0 unx      905 b- defN 80-Jan-01 00:00 abejacli/training/client.py
 -rw-r--r--  2.0 unx    59110 b- defN 80-Jan-01 00:00 abejacli/training/commands.py
 -rw-r--r--  2.0 unx    17869 b- defN 80-Jan-01 00:00 abejacli/training/jobs.py
 -rw-r--r--  2.0 unx       83 b- defN 80-Jan-01 00:00 abejacli/version.py
-?rw-r--r--  2.0 unx       43 b- defN 16-Jan-01 00:00 abejacli-2.1.0rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx    11344 b- defN 80-Jan-01 00:00 abejacli-2.1.0rc1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 abejacli-2.1.0rc1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1206 b- defN 16-Jan-01 00:00 abejacli-2.1.0rc1.dist-info/METADATA
-?rw-r--r--  2.0 unx     4239 b- defN 16-Jan-01 00:00 abejacli-2.1.0rc1.dist-info/RECORD
-50 files, 315682 bytes uncompressed, 73656 bytes compressed:  76.7%
+-rw-r--r--  2.0 unx    11344 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1107 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     4239 b- defN 16-Jan-01 00:00 abejacli-2.2.0rc1.dist-info/RECORD
+50 files, 315588 bytes uncompressed, 73654 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -129,23 +129,23 @@
 
 Filename: abejacli/training/jobs.py
 Comment: 
 
 Filename: abejacli/version.py
 Comment: 
 
-Filename: abejacli-2.1.0rc1.dist-info/entry_points.txt
+Filename: abejacli-2.2.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: abejacli-2.1.0rc1.dist-info/LICENSE
+Filename: abejacli-2.2.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: abejacli-2.1.0rc1.dist-info/WHEEL
+Filename: abejacli-2.2.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: abejacli-2.1.0rc1.dist-info/METADATA
+Filename: abejacli-2.2.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: abejacli-2.1.0rc1.dist-info/RECORD
+Filename: abejacli-2.2.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abejacli/docker/container_run.py

```diff
@@ -115,15 +115,15 @@
         """setup cli
 
         docker client will default to connecting to the following respectively.
         unix://var/run/docker.sock : linux / osx
         tcp://127.0.0.1:2376       : windows
 
         judge operation system using by os.name
-        cf. https://docs.python.org/3.6/library/os.html#os.name
+        cf. https://docs.python.org/3.9/library/os.html#os.name
         """
         if os.name == 'nt':
             base_url = 'tcp://127.0.0.1:2376'
         else:
             base_url = 'unix://var/run/docker.sock'
         self._docker_cli = docker.APIClient(base_url=base_url)
```

## abejacli/model/docker_handler.py

```diff
@@ -58,15 +58,15 @@
         setup cli
 
         docker client will default to connecting to the following respectively.
         unix://var/run/docker.sock : linux / osx
         tcp://127.0.0.1:2376       : windows
 
         judge operation system using by os.name
-        cf. https://docs.python.org/3.6/library/os.html#os.name
+        cf. https://docs.python.org/3.9/library/os.html#os.name
 
         """
         if os.name == 'nt':
             base_url = 'tcp://127.0.0.1:2376'
         else:
             base_url = 'unix://var/run/docker.sock'
         self._docker_cli = docker.APIClient(base_url=base_url)
```

## Comparing `abejacli-2.1.0rc1.dist-info/LICENSE` & `abejacli-2.2.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `abejacli-2.1.0rc1.dist-info/METADATA` & `abejacli-2.2.0rc1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: abejacli
-Version: 2.1.0rc1
+Version: 2.2.0rc1
 Summary: ABEJA Platform Command line tool
 License: Apache-2.0
 Author: ABEJA Inc.
 Author-email: platform-support@abejainc.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: cerberus (>=1.3.0,<1.4.0)
 Requires-Dist: click (>=7.0.0,<7.1.0)
 Requires-Dist: click-config-file (>=0.5.0,<0.6.0)
 Requires-Dist: docker (>=2.5.1,<2.6.0)
 Requires-Dist: pygments (>=2.0)
 Requires-Dist: python-dateutil (>=2.6.0,<2.7.0)
```

## Comparing `abejacli-2.1.0rc1.dist-info/RECORD` & `abejacli-2.2.0rc1.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 abejacli/datalake/process_file_job.py,sha256=r7LN6SgqRMorsuXcAUYfJ17a7Dt17N3c2V8xHRz52WA,6482
 abejacli/datalake/upload_job.py,sha256=xi8AcB_oeQiFbpzmWxfHA16ZOCIDga4Tq9cBsgx-Cxg,4618
 abejacli/dataset/__init__.py,sha256=pAsg3XaP7io6A6o9_KzXVmjrduu6keKt0GMtd5fsdtw,4339
 abejacli/dataset/commands.py,sha256=gWtysraygVHBy19pxk0OQWAJpF12PX5BtpOMdLaxJP8,9753
 abejacli/docker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abejacli/docker/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abejacli/docker/commands/run.py,sha256=plvtD0m5sHL2IzmpGMNc4SOH_ed1SL9lJ9qEav1Nhrk,8452
-abejacli/docker/container_run.py,sha256=FYkbU3v6szuY58_967C71LVrA8_09sR7QfqFCKt76B8,9155
+abejacli/docker/container_run.py,sha256=9xZ3Y4hwszpLST1MUnf5tseZ2h2Eoc9vrdB9Q2rR-e0,9155
 abejacli/docker/utils.py,sha256=nCTlrvmWreW9jf5gg5ZCotFxq8k2-EWY2jtijkdrd60,746
 abejacli/exceptions.py,sha256=BOSeNT7GgQMQ0-IVdbzCKtflAqWfQUT58LydccKCMIY,282
 abejacli/fs_utils.py,sha256=V6uWQ1knu0OOxGdG2XHGwOEeUTwFpMd1T9a_eF85GkA,6964
 abejacli/logger.py,sha256=skvYF-qmkGVBbs6rzDvqibz91xoxKLh54NQGWUb8PbE,1228
 abejacli/model/__init__.py,sha256=yn_QtqimDjul0PCLa2Ps4guoDzoZcZzo4twuPuuaE-o,217
-abejacli/model/docker_handler.py,sha256=wt3BoguBJc42dqqm6bsE_z9Spfb1kPKF5HhHfC1Sw5o,6405
+abejacli/model/docker_handler.py,sha256=Oh5QrGHzQMwFeqea4-XuEIBf9goSPtDKU72DWa4uGqE,6405
 abejacli/model/local_server_manager.py,sha256=TRGOVSLNYbZooTNppBoKHJcoJQBqcakJNjQCFTXonnY,1731
 abejacli/model/runtime_utils.py,sha256=GsCmE-Avb4oOrreSRh_YNc-KQ4M-G5Vi370gAERgkQk,831
 abejacli/registry/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abejacli/registry/commands.py,sha256=1Ea-XdLUY2Smmjj2-1zRv7vVrR8xtomgtJnHEYapINw,5703
 abejacli/run.py,sha256=0T3CS2jjTxmm9uiFlCIktMCF2SY5A0-PMjRPMyqW874,76654
 abejacli/session.py,sha256=M6JxGW30YvZzREv3VDPSiqGV0ND8h6COE4P3TH3IlkU,4623
 abejacli/startapp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -39,12 +39,12 @@
 abejacli/template/requirements-local.txt-tpl,sha256=i_YQz8eFRWEs7hEWL-ww8UyVhLAzQcasrROGjVWp0nk,25
 abejacli/template/train.py-tpl,sha256=fTqep3aHzojqX664KExwotET8WihoqLMlSZhpybQZTc,1432
 abejacli/training/__init__.py,sha256=G8P-bJOy0Hjb-C_EA7NfP-M884PWlIAKLXwf53B9E54,6891
 abejacli/training/client.py,sha256=CLjI_UojbGLiTJg-mPFIcAv4-2npGCM3Se1TniB6hp8,905
 abejacli/training/commands.py,sha256=3WpVkEEnHT5GAkhSFnCa3lrsSN7xhFgJbSg7YAfFf9A,59110
 abejacli/training/jobs.py,sha256=PN1oW40dZNoJbdcxmyeF_8tlbNFog8RpKOQZvnGHegA,17869
 abejacli/version.py,sha256=g4QC6oBBD54l5EAZFkxCrEY9h47YON2VDCA9PItYOQM,83
-abejacli-2.1.0rc1.dist-info/entry_points.txt,sha256=0sfIdUU9v0_JsInKJ7Qf5pVUSL9wbAlOOXp7qCHDDjg,43
-abejacli-2.1.0rc1.dist-info/LICENSE,sha256=LasG9nAf8e8HZVQSsSkIKAm0s_kjYPGuk968yRClNSw,11344
-abejacli-2.1.0rc1.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-abejacli-2.1.0rc1.dist-info/METADATA,sha256=KQjt_S-JcQ00Bt9NEvIeOPTNn7v5JW_IN8d8aXB8cBA,1206
-abejacli-2.1.0rc1.dist-info/RECORD,,
+abejacli-2.2.0rc1.dist-info/LICENSE,sha256=LasG9nAf8e8HZVQSsSkIKAm0s_kjYPGuk968yRClNSw,11344
+abejacli-2.2.0rc1.dist-info/METADATA,sha256=Pt0MU1tNhUBuOu2nRcTmSz2Re-OPXBxo9MKb80vIsH8,1107
+abejacli-2.2.0rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+abejacli-2.2.0rc1.dist-info/entry_points.txt,sha256=0sfIdUU9v0_JsInKJ7Qf5pVUSL9wbAlOOXp7qCHDDjg,43
+abejacli-2.2.0rc1.dist-info/RECORD,,
```

