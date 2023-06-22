# Comparing `tmp/sagemaker-huggingface-inference-toolkit-2.1.1.tar.gz` & `tmp/sagemaker-huggingface-inference-toolkit-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-huggingface-inference-toolkit-2.1.1.tar", last modified: Mon Dec 12 22:00:03 2022, max compression
+gzip compressed data, was "sagemaker-huggingface-inference-toolkit-2.1.2.tar", last modified: Thu Jun 22 20:11:02 2023, max compression
```

## Comparing `sagemaker-huggingface-inference-toolkit-2.1.1.tar` & `sagemaker-huggingface-inference-toolkit-2.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-12 22:00:03.050127 sagemaker-huggingface-inference-toolkit-2.1.1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10141 2022-09-22 22:36:38.000000 sagemaker-huggingface-inference-toolkit-2.1.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       96 2022-09-22 22:36:38.000000 sagemaker-huggingface-inference-toolkit-2.1.1/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       67 2022-09-22 22:36:38.000000 sagemaker-huggingface-inference-toolkit-2.1.1/NOTICE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8730 2022-12-12 22:00:03.050127 sagemaker-huggingface-inference-toolkit-2.1.1/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7456 2022-10-14 20:16:25.000000 sagemaker-huggingface-inference-toolkit-2.1.1/README.md
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       57 2022-09-22 22:36:38.000000 sagemaker-huggingface-inference-toolkit-2.1.1/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      517 2022-12-12 22:00:03.050127 sagemaker-huggingface-inference-toolkit-2.1.1/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4400 2022-12-12 21:26:51.000000 sagemaker-huggingface-inference-toolkit-2.1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-12 22:00:03.046127 sagemaker-huggingface-inference-toolkit-2.1.1/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-12 22:00:03.050127 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      681 2022-09-22 22:36:38.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1267 2022-09-22 22:36:38.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/content_types.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5519 2022-09-22 22:36:38.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/decoder_encoder.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11272 2022-09-22 22:36:38.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/handler_service.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4934 2022-10-18 16:25:42.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/mms_model_server.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1135 2022-09-22 22:36:38.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/serving.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9876 2022-12-12 21:18:08.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/transformers_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-12 22:00:03.050127 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8730 2022-12-12 22:00:03.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      902 2022-12-12 22:00:03.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-12 22:00:03.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2022-12-12 22:00:03.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      607 2022-12-12 22:00:03.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2022-12-12 22:00:03.000000 sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:11:02.470026 sagemaker-huggingface-inference-toolkit-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)    10141 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       96 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-06-22 20:11:02.470026 sagemaker-huggingface-inference-toolkit-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7456 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      517 2023-06-22 20:11:02.470026 sagemaker-huggingface-inference-toolkit-2.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:11:02.470026 sagemaker-huggingface-inference-toolkit-2.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:11:02.470026 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/
+-rw-r--r--   0 root         (0) root         (0)      681 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/content_types.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/decoder_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    11272 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/handler_service.py
+-rw-r--r--   0 root         (0) root         (0)     4934 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/mms_model_server.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/serving.py
+-rw-r--r--   0 root         (0) root         (0)     9876 2023-06-22 19:56:07.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/transformers_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:11:02.470026 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8730 2023-06-22 20:11:02.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-22 20:11:02.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:11:02.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-22 20:11:02.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      607 2023-06-22 20:11:02.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-22 20:11:02.000000 sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/top_level.txt
```

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/LICENSE` & `sagemaker-huggingface-inference-toolkit-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/PKG-INFO` & `sagemaker-huggingface-inference-toolkit-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-huggingface-inference-toolkit
-Version: 2.1.1
+Version: 2.1.2
 Summary: Open source library for running inference workload with Hugging Face Deep Learning Containers on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-huggingface-inference-toolkit
 Author: HuggingFace and Amazon Web Services
 License: Apache License 2.0
 Keywords: NLP deep-learning transformer pytorch tensorflow BERT GPT GPT-2 AWS Amazon SageMaker Cloud
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/README.md` & `sagemaker-huggingface-inference-toolkit-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/setup.cfg` & `sagemaker-huggingface-inference-toolkit-2.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/setup.py` & `sagemaker-huggingface-inference-toolkit-2.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import os
 from datetime import date
 from setuptools import find_packages, setup
 
 # We don't declare our dependency on transformers here because we build with
 # different packages for different variants
 
-VERSION = "2.1.1"
+VERSION = "2.1.2"
 
 
 # Ubuntu packages
 # libsndfile1-dev: torchaudio requires the development version of the libsndfile package which can be installed via a system package manager. On Ubuntu it can be installed as follows: apt install libsndfile1-dev
 # ffmpeg: ffmpeg is required for audio processing. On Ubuntu it can be installed as follows: apt install ffmpeg
 # libavcodec-extra : libavcodec-extra  inculdes additional codecs for ffmpeg
```

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/__init__.py` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/content_types.py` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/content_types.py`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/decoder_encoder.py` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/decoder_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     """
 
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         elif isinstance(obj, np.floating):
             return float(obj)
-        elif isinstance(obj, np.ndarray):
+        elif hasattr(obj, "tolist"):
             return obj.tolist()
         elif isinstance(obj, datetime.datetime):
             return obj.__str__()
         elif isinstance(obj, Image.Image):
             with BytesIO() as out:
                 obj.save(out, format="PNG")
                 png_string = out.getvalue()
```

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/handler_service.py` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/handler_service.py`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/mms_model_server.py` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/mms_model_server.py`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/serving.py` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/serving.py`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit/transformers_utils.py` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit/transformers_utils.py`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/PKG-INFO` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-huggingface-inference-toolkit
-Version: 2.1.1
+Version: 2.1.2
 Summary: Open source library for running inference workload with Hugging Face Deep Learning Containers on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-huggingface-inference-toolkit
 Author: HuggingFace and Amazon Web Services
 License: Apache License 2.0
 Keywords: NLP deep-learning transformer pytorch tensorflow BERT GPT GPT-2 AWS Amazon SageMaker Cloud
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/SOURCES.txt` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sagemaker-huggingface-inference-toolkit-2.1.1/src/sagemaker_huggingface_inference_toolkit.egg-info/requires.txt` & `sagemaker-huggingface-inference-toolkit-2.1.2/src/sagemaker_huggingface_inference_toolkit.egg-info/requires.txt`

 * *Files identical despite different names*

