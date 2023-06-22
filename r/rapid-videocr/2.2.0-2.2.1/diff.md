# Comparing `tmp/rapid_videocr-2.2.0-py3-none-any.whl.zip` & `tmp/rapid_videocr-2.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14935 bytes, number of entries: 11
--rw-r--r--  2.0 unx      174 b- defN 23-Jun-22 04:09 rapid_videocr/__init__.py
--rw-r--r--  2.0 unx     4811 b- defN 23-Jun-22 04:09 rapid_videocr/main.py
--rw-r--r--  2.0 unx    12743 b- defN 23-Jun-22 04:09 rapid_videocr/rapid_videocr.py
--rw-r--r--  2.0 unx     2756 b- defN 23-Jun-22 04:09 rapid_videocr/utils.py
--rw-r--r--  2.0 unx     1297 b- defN 23-Jun-22 04:09 rapid_videocr/video_sub_finder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4648 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      934 b- defN 23-Jun-22 04:09 rapid_videocr-2.2.0.dist-info/RECORD
-11 files, 38885 bytes uncompressed, 13345 bytes compressed:  65.7%
+Zip file size: 14922 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-22 11:18 rapid_videocr/__init__.py
+-rw-r--r--  2.0 unx     4798 b- defN 23-Jun-22 11:18 rapid_videocr/main.py
+-rw-r--r--  2.0 unx    12743 b- defN 23-Jun-22 11:18 rapid_videocr/rapid_videocr.py
+-rw-r--r--  2.0 unx     2756 b- defN 23-Jun-22 11:18 rapid_videocr/utils.py
+-rw-r--r--  2.0 unx     1264 b- defN 23-Jun-22 11:18 rapid_videocr/video_sub_finder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4648 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      934 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/RECORD
+11 files, 38839 bytes uncompressed, 13332 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: rapid_videocr/utils.py
 Comment: 
 
 Filename: rapid_videocr/video_sub_finder.py
 Comment: 
 
-Filename: rapid_videocr-2.2.0.dist-info/LICENSE
+Filename: rapid_videocr-2.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: rapid_videocr-2.2.0.dist-info/METADATA
+Filename: rapid_videocr-2.2.1.dist-info/METADATA
 Comment: 
 
-Filename: rapid_videocr-2.2.0.dist-info/WHEEL
+Filename: rapid_videocr-2.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_videocr-2.2.0.dist-info/entry_points.txt
+Filename: rapid_videocr-2.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.0.dist-info/top_level.txt
+Filename: rapid_videocr-2.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.0.dist-info/RECORD
+Filename: rapid_videocr-2.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_videocr/main.py

```diff
@@ -35,15 +35,15 @@
         video_num = len(video_list)
         for i, one_video in enumerate(video_list):
             self.logger.info(
                 f'[{i+1}/{video_num}] Starting to extract {one_video} key frame'
             )
             with tempfile.TemporaryDirectory() as tmp_dir:
                 try:
-                    self.vsf(one_video, tmp_dir)
+                    self.vsf(str(one_video), tmp_dir)
                 except Exception as e:
                     self.logger.error(f'Extract {one_video} error, {e}, skip')
                     continue
 
                 self.logger.info(f'[{i+1}/{video_num}] Starting to run {one_video} ocr')
 
                 rgb_dir = Path(tmp_dir) / 'RGBImages'
@@ -119,19 +119,18 @@
         choices=[0, 1],
         help='Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.',
     )
     args = parser.parse_args()
 
     is_concat_rec = 'concat' in args.mode
 
-    if args.vsf_exe_path is not None:
-        if args.video_dir is None:
-            raise ValueError(
-                '--vsf_exe_path or --video_dir must not be None at the same time.'
-            )
+    if not (args.vsf_exe_path is None and args.video_dir is None):
+        raise ValueError(
+            '--vsf_exe_path or --video_dir must not be None at the same time.'
+        )
 
     if args.vsf_exe_path and args.video_dir:
         extractor = RapidVideoSubFinderOCR(
             vsf_exe_path=args.vsf_exe_path,
             is_concat_rec=is_concat_rec,
             concat_batch=args.concat_batch,
             out_format=args.out_format,
```

## rapid_videocr/video_sub_finder.py

```diff
@@ -36,12 +36,12 @@
                     "--top_video_image_percent_end",
                     str(self.te),
                 ],
                 check=False,
             )
             return output_dir
         except Exception as e:
-            raise VSFError('vsf meets error') from e
+            raise e
 
 
 class VSFError(Exception):
     pass
```

## Comparing `rapid_videocr-2.2.0.dist-info/LICENSE` & `rapid_videocr-2.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapid_videocr-2.2.0.dist-info/METADATA` & `rapid_videocr-2.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-videocr
-Version: 2.2.0
+Version: 2.2.1
 Summary: Tool for extracting hard subtitles from videos.
 Home-page: https://github.com/SWHL/RapidVideOCR.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr,videocr,subtitle
 Platform: Any
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.0 Summary: Tool for
+Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.1 Summary: Tool for
 extracting hard subtitles from videos. Home-page: https://github.com/SWHL/
 RapidVideOCR.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: rapidocr,videocr,subtitle Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

