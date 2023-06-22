# Comparing `tmp/octoai_sdk-0.1.0.tar.gz` & `tmp/octoai_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoai_sdk-0.1.0.tar", max compression
+gzip compressed data, was "octoai_sdk-0.1.1.tar", max compression
```

## Comparing `octoai_sdk-0.1.0.tar` & `octoai_sdk-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      227 2023-06-13 16:22:01.228527 octoai_sdk-0.1.0/octoai/__init__.py
--rw-r--r--   0        0        0     7264 2023-06-13 18:33:42.757007 octoai_sdk-0.1.0/octoai/client.py
--rw-r--r--   0        0        0      995 2023-06-09 21:08:23.293946 octoai_sdk-0.1.0/octoai/errors.py
--rw-r--r--   0        0        0       56 2023-06-09 21:08:23.294496 octoai_sdk-0.1.0/octoai/scaffolds/flan-t5/requirements.txt
--rw-r--r--   0        0        0      833 2023-06-09 21:08:23.294697 octoai_sdk-0.1.0/octoai/scaffolds/flan-t5/service.py
--rw-r--r--   0        0        0     1290 2023-06-12 17:09:46.783772 octoai_sdk-0.1.0/octoai/scaffolds/flan-t5/test_request.py
--rw-r--r--   0        0        0        0 2023-06-09 21:08:23.296075 octoai_sdk-0.1.0/octoai/scaffolds/hello-world/requirements.txt
--rw-r--r--   0        0        0      395 2023-06-09 21:08:23.296287 octoai_sdk-0.1.0/octoai/scaffolds/hello-world/service.py
--rw-r--r--   0        0        0     1272 2023-06-12 17:09:46.788205 octoai_sdk-0.1.0/octoai/scaffolds/hello-world/test_request.py
--rw-r--r--   0        0        0       34 2023-06-13 16:21:58.470830 octoai_sdk-0.1.0/octoai/scaffolds/wav2vec/requirements.txt
--rw-r--r--   0        0        0     1100 2023-06-13 16:21:58.472295 octoai_sdk-0.1.0/octoai/scaffolds/wav2vec/service.py
--rw-r--r--   0        0        0     1458 2023-06-13 16:21:58.473214 octoai_sdk-0.1.0/octoai/scaffolds/wav2vec/test_request.py
--rw-r--r--   0        0        0       33 2023-06-09 21:08:23.297221 octoai_sdk-0.1.0/octoai/scaffolds/yolov8/requirements.txt
--rw-r--r--   0        0        0     1852 2023-06-09 21:08:23.297368 octoai_sdk-0.1.0/octoai/scaffolds/yolov8/service.py
--rw-r--r--   0        0        0     1809 2023-06-12 17:09:46.790769 octoai_sdk-0.1.0/octoai/scaffolds/yolov8/test_request.py
--rw-r--r--   0        0        0     6199 2023-06-12 17:09:46.796808 octoai_sdk-0.1.0/octoai/server.py
--rw-r--r--   0        0        0     2698 2023-06-12 17:09:46.799814 octoai_sdk-0.1.0/octoai/service.py
--rw-r--r--   0        0        0    10484 2023-06-12 17:09:46.801688 octoai_sdk-0.1.0/octoai/types.py
--rw-r--r--   0        0        0     4000 2023-06-13 18:33:42.759467 octoai_sdk-0.1.0/octoai/utils.py
--rw-r--r--   0        0        0     1071 2023-06-13 17:59:54.334737 octoai_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 octoai_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-06-13 16:22:01.228527 octoai_sdk-0.1.1/octoai/__init__.py
+-rw-r--r--   0        0        0     7264 2023-06-22 15:51:11.411771 octoai_sdk-0.1.1/octoai/client.py
+-rw-r--r--   0        0        0      995 2023-06-09 21:08:23.293946 octoai_sdk-0.1.1/octoai/errors.py
+-rw-r--r--   0        0        0       56 2023-06-09 21:08:23.294496 octoai_sdk-0.1.1/octoai/scaffolds/flan-t5/requirements.txt
+-rw-r--r--   0        0        0     1323 2023-06-21 00:01:12.459613 octoai_sdk-0.1.1/octoai/scaffolds/flan-t5/service.py
+-rw-r--r--   0        0        0     1290 2023-06-12 17:09:46.783772 octoai_sdk-0.1.1/octoai/scaffolds/flan-t5/test_request.py
+-rw-r--r--   0        0        0        0 2023-06-09 21:08:23.296075 octoai_sdk-0.1.1/octoai/scaffolds/hello-world/requirements.txt
+-rw-r--r--   0        0        0      395 2023-06-09 21:08:23.296287 octoai_sdk-0.1.1/octoai/scaffolds/hello-world/service.py
+-rw-r--r--   0        0        0     1272 2023-06-12 17:09:46.788205 octoai_sdk-0.1.1/octoai/scaffolds/hello-world/test_request.py
+-rw-r--r--   0        0        0       34 2023-06-13 16:21:58.470830 octoai_sdk-0.1.1/octoai/scaffolds/wav2vec/requirements.txt
+-rw-r--r--   0        0        0     1956 2023-06-21 00:01:12.461702 octoai_sdk-0.1.1/octoai/scaffolds/wav2vec/service.py
+-rw-r--r--   0        0        0     1458 2023-06-13 16:21:58.473214 octoai_sdk-0.1.1/octoai/scaffolds/wav2vec/test_request.py
+-rw-r--r--   0        0        0       33 2023-06-09 21:08:23.297221 octoai_sdk-0.1.1/octoai/scaffolds/yolov8/requirements.txt
+-rw-r--r--   0        0        0     3474 2023-06-21 00:01:12.463890 octoai_sdk-0.1.1/octoai/scaffolds/yolov8/service.py
+-rw-r--r--   0        0        0     1809 2023-06-12 17:09:46.790769 octoai_sdk-0.1.1/octoai/scaffolds/yolov8/test_request.py
+-rw-r--r--   0        0        0     6199 2023-06-12 17:09:46.796808 octoai_sdk-0.1.1/octoai/server.py
+-rw-r--r--   0        0        0     2698 2023-06-12 17:09:46.799814 octoai_sdk-0.1.1/octoai/service.py
+-rw-r--r--   0        0        0    13192 2023-06-21 00:01:12.467552 octoai_sdk-0.1.1/octoai/types.py
+-rw-r--r--   0        0        0     4000 2023-06-22 15:51:11.413837 octoai_sdk-0.1.1/octoai/utils.py
+-rw-r--r--   0        0        0     1050 2023-06-22 18:25:34.256859 octoai_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 octoai_sdk-0.1.1/PKG-INFO
```

### Comparing `octoai_sdk-0.1.0/octoai/client.py` & `octoai_sdk-0.1.1/octoai/client.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.0/octoai/errors.py` & `octoai_sdk-0.1.1/octoai/errors.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.0/octoai/scaffolds/flan-t5/test_request.py` & `octoai_sdk-0.1.1/octoai/scaffolds/flan-t5/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.0/octoai/scaffolds/hello-world/test_request.py` & `octoai_sdk-0.1.1/octoai/scaffolds/hello-world/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.0/octoai/scaffolds/wav2vec/test_request.py` & `octoai_sdk-0.1.1/octoai/scaffolds/wav2vec/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.0/octoai/scaffolds/yolov8/test_request.py` & `octoai_sdk-0.1.1/octoai/scaffolds/yolov8/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.0/octoai/server.py` & `octoai_sdk-0.1.1/octoai/server.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.0/octoai/service.py` & `octoai_sdk-0.1.1/octoai/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.0/octoai/types.py` & `octoai_sdk-0.1.1/octoai/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 images or audio) over HTTP. These type definitions can be useful
 both when creating endpoints (implementing ``octoai.service.Service``
 as directed by the ``octoai`` command-line interface) and when
 communicating with live endpoints using the client SDK.
 """
 
 import base64
+import importlib
 import os
+import sys
 from io import BytesIO
-from typing import Any, Dict, Tuple
+from types import ModuleType
+from typing import Any, Dict, Tuple, Union
 
 import httpx
-import soundfile
 from numpy.typing import ArrayLike
 from PIL import Image as PImage
 from pydantic import BaseModel, Field
 
 
 def file_b64encode(file_bytes: bytes) -> str:
     """Encode binary file as a base64 string.
@@ -39,36 +41,98 @@
     :type file_b64: str
     :return: contents of a binary file
     :rtype: bytes
     """
     return base64.b64decode(bytes(file_b64, "ascii"))
 
 
+def _import_soundfile() -> ModuleType:
+    """Attempt to import the soundfile module."""
+    if "soundfile" in sys.modules:
+        return sys.modules["soundfile"]
+
+    try:
+        return importlib.import_module("soundfile")
+    except OSError:
+        raise Exception(
+            "Can't import the 'soundfile' module. "
+            "For Linux, try: sudo apt install libsndfile1. "
+            "For Mac, try: brew install libsndfile."
+        )
+
+
 class Text(BaseModel):
-    """Text type for models that accept or return text."""
+    """Text type for models that accept or return text.
+
+    The `Text` type is a simple wrapper for `str` that provides
+    a consistent API specification for endpoints. This type
+    supports typical string-like operations. The text is transferred
+    over HTTP without any additional encoding.
+
+    To create an instance of this type, call the constructor
+    with your string value: `Text("mytext")`
+    """
 
     text: str
 
+    def __init__(self, text: str):
+        super().__init__(text=text)
+
+    def __add__(self, other: Union["Text", str]) -> "Text":
+        """Concatenate."""
+        try:
+            return Text(self.text + other.text)  # type: ignore
+        except AttributeError:
+            return Text(self.text + other)  # type: ignore
+
+    def __contains__(self, item: Union["Text", str]) -> bool:
+        """Check inclusion."""
+        try:
+            return item.text in self.text  # type: ignore
+        except AttributeError:
+            return item in self.text  # type: ignore
+
+    def __getitem__(self, index):
+        """Get item."""
+        return Text(self.text.__getitem__(index))
+
+    def __mul__(self, other: int) -> "Text":
+        """Repeat."""
+        return Text(self.text * other)
+
+    def __str__(self) -> str:
+        """Convert to string."""
+        return self.text
+
 
 class Image(BaseModel):
     """Image helpers for models that accept or return images.
 
+    The `Image` type is a wrapper for binary image files that provides a
+    consistent API specification for your endpoint. The image data is
+    transferred over HTTP encoded as base64. This type provides support for
+    encoding and decoding, reading image data as Pillow, creating image files
+    from Pillow, and reading image files from disk or remote URLs.
+
     To create an instance of this type, users can select the appropriate
     ``Image.from_...()`` method depending on the format of their input.
 
     :param BaseModel: base model
     :type BaseModel: :class:`BaseModel`
     :raises ValueError: ``from_file`` method failed to load image.
     :raises ValueError: ``from_url`` method was unable to reach the url.
     :return: base64 encoded image
     :rtype: str
     """
 
     image_b64: str = Field(description="base64-encoded image file")
 
+    def __init__(self, image_b64: str):
+        super().__init__(image_b64=image_b64)
+
     @classmethod
     def from_base64(cls, b64: str):
         """Create from base64 encoded string, such as that returned from an HTTP call.
 
         See also ``Image.from_endpoint_response()``.
 
         :param b64: contents of a binary image file as a base64 encoded string
@@ -176,27 +240,36 @@
         with open(file_name, "wb") as fd:
             fd.write(file_b64decode(self.image_b64))
 
 
 class Audio(BaseModel):
     """Audio helpers for models that accept or return audio.
 
+    The `Audio` type is a wrapper for binary audio files that provides a
+    consistent API specification for endpoints. The audio data is
+    transferred over HTTP encoded as base64. This type provides support for
+    encoding and decoding, reading audio data as numpy, creating audio files
+    from numpy, and reading audio files from disk or remote URLs.
+
     To create an instance of this type, users can select the appropriate
     ``Audio.from_...()`` method depending on the format of their input.
 
     :param BaseModel: base model
     :type BaseModel: :class:`BaseModel`
     :raises ValueError: ``from_file`` method failed to load file
     :raises ValueError: ``from_url`` method was unable to reach the url.
     :return: base64 encoded audio
     :rtype: str
     """
 
     audio_b64: str = Field(description="base64-encoded audio file")
 
+    def __init__(self, audio_b64: str):
+        super().__init__(audio_b64=audio_b64)
+
     @classmethod
     def from_base64(cls, b64: str):
         """Create from base64 encoded string, such as that returned from an HTTP call.
 
         See also ``Audio.from_endpoint_response()``.
 
         :param b64: contents of a binary audio file as a base64 encoded string
@@ -239,14 +312,15 @@
         :param sample_rate: samples per second taken to create signal
         :type sample_rate: int
         :param format: target format, defaults to "WAV"
         :type format: str, optional
         :return: Audio object
         :rtype: :class:`Audio`
         """
+        soundfile = _import_soundfile()
         buffer = BytesIO()
         soundfile.write(buffer, data=data, samplerate=sample_rate, format=format)
         return cls(audio_b64=file_b64encode(buffer.getvalue()))
 
     @classmethod
     def from_file(cls, audio_file: str):
         """Create from local file.
@@ -295,14 +369,15 @@
 
     def to_numpy(self) -> Tuple[ArrayLike, int]:
         """Convert to numpy array.
 
         :return: numpy array representation (frames x channels)
         :rtype: Tuple[ArrayLike, int]
         """
+        soundfile = _import_soundfile()
         fd = BytesIO(file_b64decode(self.audio_b64))
         data, sample_rate = soundfile.read(fd)
         return (data, sample_rate)
 
     def to_file(self, file_name: str):
         """Save to disk.
```

### Comparing `octoai_sdk-0.1.0/octoai/utils.py` & `octoai_sdk-0.1.1/octoai/utils.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.0/pyproject.toml` & `octoai_sdk-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octoai-sdk"
-version = "0.1.0"
+version = "0.1.1"
 description = "A runtime library for OctoAI."
 authors = ["OctoML"]
 packages = [
     { include = "octoai" }
 ]
 
 [tool.poetry.dependencies]
@@ -13,15 +13,14 @@
 fastapi = "^0.95.2"
 httpx = "^0.24.0"
 numpy = "^1.24.3"
 pillow = "^9.5.0"
 pydantic = "^1.10.8"
 pyyaml = "^6.0"
 soundfile = "^0.12.1"
-requests = "^2.31.0"
 types-pyyaml = "^6.0.12.10"
 uvicorn = "^0.22.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.0.0"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.7.0"
```

### Comparing `octoai_sdk-0.1.0/PKG-INFO` & `octoai_sdk-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoai-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A runtime library for OctoAI.
 Author: OctoML
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,11 +12,10 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fastapi (>=0.95.2,<0.96.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: soundfile (>=0.12.1,<0.13.0)
 Requires-Dist: types-pyyaml (>=6.0.12.10,<7.0.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
```

