# Comparing `tmp/embaas-0.0.3.tar.gz` & `tmp/embaas-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embaas-0.0.3.tar", last modified: Thu Jun 22 03:20:32 2023, max compression
+gzip compressed data, was "embaas-0.0.4.tar", last modified: Thu Jun 22 05:06:28 2023, max compression
```

## Comparing `embaas-0.0.3.tar` & `embaas-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 03:20:32.627812 embaas-0.0.3/
--rw-r--r--   0 juliuslipp   (501) staff       (20)     1063 2023-06-22 00:48:52.000000 embaas-0.0.3/LICENSE
--rw-r--r--   0 juliuslipp   (501) staff       (20)     2076 2023-06-22 03:20:32.627692 embaas-0.0.3/PKG-INFO
--rw-r--r--   0 juliuslipp   (501) staff       (20)      333 2023-06-22 02:00:01.000000 embaas-0.0.3/README.md
-drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 03:20:32.622530 embaas-0.0.3/embaas/
--rw-r--r--   0 juliuslipp   (501) staff       (20)     1319 2023-06-22 00:57:02.000000 embaas-0.0.3/embaas/__init__.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)    13400 2023-06-22 00:45:04.000000 embaas-0.0.3/embaas/client.py
-drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 03:20:32.624287 embaas-0.0.3/embaas/core/
--rw-r--r--   0 juliuslipp   (501) staff       (20)      304 2023-06-22 03:19:55.000000 embaas-0.0.3/embaas/core/__init__.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)     1047 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/core/datetime_utils.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)     3710 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/core/jsonable_encoder.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      385 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/core/remove_none_from_headers.py
-drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 03:20:32.624764 embaas-0.0.3/embaas/errors/
--rw-r--r--   0 juliuslipp   (501) staff       (20)      170 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/errors/__init__.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      426 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/errors/api_error.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      307 2023-06-22 03:20:06.000000 embaas-0.0.3/embaas/errors/unprocessable_entity_error.py
-drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 03:20:32.627511 embaas-0.0.3/embaas/types/
--rw-r--r--   0 juliuslipp   (501) staff       (20)     1740 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/__init__.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)     2773 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/chunk_splitter.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      856 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/document_chunk.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      913 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/document_extraction_response.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      986 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/document_extraction_response_with_embeddings.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      868 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/document_extraction_result.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      753 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/document_usage.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      856 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/document_with_embeddings_usage.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      819 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/embedding.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      861 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/embeddings_response.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      399 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/handle_byte_extraction_v_1_document_extract_text_bytes_post_response.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      394 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/handle_file_extraction_v_1_document_extract_text_post_response.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      843 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/http_validation_error.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      814 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/usage.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      869 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/validation_error.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      128 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/validation_error_loc_item.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      893 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/whisper_response.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      788 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/whisper_result.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      758 2023-06-13 21:00:46.000000 embaas-0.0.3/embaas/types/whisper_usage.py
--rw-r--r--   0 juliuslipp   (501) staff       (20)      930 2023-06-14 06:48:15.000000 embaas-0.0.3/embaas/utils.py
-drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 03:20:32.623423 embaas-0.0.3/embaas.egg-info/
--rw-r--r--   0 juliuslipp   (501) staff       (20)     2076 2023-06-22 03:20:32.000000 embaas-0.0.3/embaas.egg-info/PKG-INFO
--rw-r--r--   0 juliuslipp   (501) staff       (20)     1225 2023-06-22 03:20:32.000000 embaas-0.0.3/embaas.egg-info/SOURCES.txt
--rw-r--r--   0 juliuslipp   (501) staff       (20)        1 2023-06-22 03:20:32.000000 embaas-0.0.3/embaas.egg-info/dependency_links.txt
--rw-r--r--   0 juliuslipp   (501) staff       (20)       15 2023-06-22 03:20:32.000000 embaas-0.0.3/embaas.egg-info/requires.txt
--rw-r--r--   0 juliuslipp   (501) staff       (20)        7 2023-06-22 03:20:32.000000 embaas-0.0.3/embaas.egg-info/top_level.txt
--rw-r--r--   0 juliuslipp   (501) staff       (20)      689 2023-06-22 03:20:28.000000 embaas-0.0.3/pyproject.toml
--rw-r--r--   0 juliuslipp   (501) staff       (20)       38 2023-06-22 03:20:32.627848 embaas-0.0.3/setup.cfg
+drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 05:06:28.893648 embaas-0.0.4/
+-rw-r--r--   0 juliuslipp   (501) staff       (20)     1063 2023-06-22 00:48:52.000000 embaas-0.0.4/LICENSE
+-rw-r--r--   0 juliuslipp   (501) staff       (20)     2076 2023-06-22 05:06:28.893533 embaas-0.0.4/PKG-INFO
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      333 2023-06-22 02:00:01.000000 embaas-0.0.4/README.md
+drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 05:06:28.888013 embaas-0.0.4/embaas/
+-rw-r--r--   0 juliuslipp   (501) staff       (20)     1168 2023-06-22 05:05:47.000000 embaas-0.0.4/embaas/__init__.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)    13077 2023-06-22 05:05:01.000000 embaas-0.0.4/embaas/client.py
+drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 05:06:28.889791 embaas-0.0.4/embaas/core/
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      241 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/core/__init__.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      984 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/core/datetime_utils.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)     3647 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/core/jsonable_encoder.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      322 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/core/remove_none_from_headers.py
+drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 05:06:28.890321 embaas-0.0.4/embaas/errors/
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      151 2023-06-22 05:02:38.000000 embaas-0.0.4/embaas/errors/__init__.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      363 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/errors/api_error.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      244 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/errors/unprocessable_entity_error.py
+drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 05:06:28.893342 embaas-0.0.4/embaas/types/
+-rw-r--r--   0 juliuslipp   (501) staff       (20)     1519 2023-06-22 05:02:38.000000 embaas-0.0.4/embaas/types/__init__.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)     2710 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/chunk_splitter.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      312 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/document_byte_text_extraction_response.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      793 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/document_chunk.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      850 2023-06-22 05:02:38.000000 embaas-0.0.4/embaas/types/document_extraction_response.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      923 2023-06-22 05:02:38.000000 embaas-0.0.4/embaas/types/document_extraction_response_with_embeddings.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      805 2023-06-22 05:02:38.000000 embaas-0.0.4/embaas/types/document_extraction_result.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      312 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/document_file_text_extraction_response.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      690 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/document_usage.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      793 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/document_with_embeddings_usage.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      756 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/embedding.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      798 2023-06-22 05:02:38.000000 embaas-0.0.4/embaas/types/embeddings_response.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      780 2023-06-22 05:02:38.000000 embaas-0.0.4/embaas/types/http_validation_error.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      749 2023-06-22 05:02:17.000000 embaas-0.0.4/embaas/types/usage.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      806 2023-06-22 05:02:38.000000 embaas-0.0.4/embaas/types/validation_error.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)       65 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/validation_error_loc_item.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      830 2023-06-22 05:02:38.000000 embaas-0.0.4/embaas/types/whisper_response.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      725 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/whisper_result.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      695 2023-06-22 05:02:12.000000 embaas-0.0.4/embaas/types/whisper_usage.py
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      930 2023-06-14 06:48:15.000000 embaas-0.0.4/embaas/utils.py
+drwxr-xr-x   0 juliuslipp   (501) staff       (20)        0 2023-06-22 05:06:28.888709 embaas-0.0.4/embaas.egg-info/
+-rw-r--r--   0 juliuslipp   (501) staff       (20)     2076 2023-06-22 05:06:28.000000 embaas-0.0.4/embaas.egg-info/PKG-INFO
+-rw-r--r--   0 juliuslipp   (501) staff       (20)     1171 2023-06-22 05:06:28.000000 embaas-0.0.4/embaas.egg-info/SOURCES.txt
+-rw-r--r--   0 juliuslipp   (501) staff       (20)        1 2023-06-22 05:06:28.000000 embaas-0.0.4/embaas.egg-info/dependency_links.txt
+-rw-r--r--   0 juliuslipp   (501) staff       (20)       15 2023-06-22 05:06:28.000000 embaas-0.0.4/embaas.egg-info/requires.txt
+-rw-r--r--   0 juliuslipp   (501) staff       (20)        7 2023-06-22 05:06:28.000000 embaas-0.0.4/embaas.egg-info/top_level.txt
+-rw-r--r--   0 juliuslipp   (501) staff       (20)      689 2023-06-22 05:06:19.000000 embaas-0.0.4/pyproject.toml
+-rw-r--r--   0 juliuslipp   (501) staff       (20)       38 2023-06-22 05:06:28.893693 embaas-0.0.4/setup.cfg
```

### Comparing `embaas-0.0.3/LICENSE` & `embaas-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `embaas-0.0.3/PKG-INFO` & `embaas-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embaas
-Version: 0.0.3
+Version: 0.0.4
 Summary: embaas Python SDK
 Author-email: Julius Lipp <julius@embaas.io>, embaas <info@embaas.io>
 License: MIT License
         
         Copyright (c) 2023 Embaas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `embaas-0.0.3/embaas/client.py` & `embaas-0.0.4/embaas/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,19 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 from pydantic import BaseModel, root_validator
 
-from .core.jsonable_encoder import jsonable_encoder
-from .core.remove_none_from_headers import remove_none_from_headers
-from .errors.api_error import ApiError
-from .errors.unprocessable_entity_error import UnprocessableEntityError
-from .types.chunk_splitter import ChunkSplitter
-from .types.embeddings_response import EmbeddingsResponse
-from .types.handle_byte_extraction_v_1_document_extract_text_bytes_post_response import (
-    HandleByteExtractionV1DocumentExtractTextBytesPostResponse,
-)
-from .types.handle_file_extraction_v_1_document_extract_text_post_response import (
-    HandleFileExtractionV1DocumentExtractTextPostResponse,
-)
-from .types.whisper_response import WhisperResponse
+from .core import jsonable_encoder, remove_none_from_headers
+from .errors import ApiError, UnprocessableEntityError
 from .utils import get_from_dict_or_env
+from .types import DocumentExtractionResponseWithEmbeddings, DocumentExtractionResponse, EmbeddingsResponse, \
+    DocumentByteTextExtractionResponse, DocumentFileTextExtractionResponse, WhisperResponse, ChunkSplitter
 
 OMIT = typing.cast(typing.Any, ...)
 T = typing.TypeVar("T", bound=BaseModel)
 DEFAULT_ENVIRONMENT = "https://api.embaas.io"
 DEFAULT_MODEL = "e5-large-v2"
 
 
@@ -103,15 +94,15 @@
             chunk_size: typing.Optional[int] = OMIT,
             chunk_overlap: typing.Optional[int] = OMIT,
             chunk_splitter: typing.Optional[ChunkSplitter] = OMIT,
             separators: typing.Optional[typing.List[str]] = OMIT,
             should_embed: typing.Optional[bool] = OMIT,
             model: typing.Optional[str] = OMIT,
             instruction: typing.Optional[str] = OMIT,
-    ) -> HandleFileExtractionV1DocumentExtractTextPostResponse:
+    ) -> DocumentFileTextExtractionResponse:
         pass
 
     @abc.abstractmethod
     def extract_text_from_bytes(
             self,
             *,
             bytes_or_base64: typing.Union[bytes, str],
@@ -119,15 +110,15 @@
             chunk_size: typing.Optional[int] = OMIT,
             chunk_overlap: typing.Optional[int] = OMIT,
             chunk_splitter: typing.Optional[ChunkSplitter] = OMIT,
             separators: typing.Optional[typing.List[str]] = OMIT,
             should_embed: typing.Optional[bool] = OMIT,
             model: typing.Optional[str] = OMIT,
             instruction: typing.Optional[str] = OMIT,
-    ) -> HandleByteExtractionV1DocumentExtractTextBytesPostResponse:
+    ) -> DocumentByteTextExtractionResponse:
         pass
 
     @abc.abstractmethod
     def whisper(self, *, file: typing.IO) -> WhisperResponse:
         pass
 
 
@@ -170,15 +161,15 @@
             chunk_size: typing.Optional[int] = OMIT,
             chunk_overlap: typing.Optional[int] = OMIT,
             chunk_splitter: typing.Optional[ChunkSplitter] = OMIT,
             separators: typing.Optional[typing.List[str]] = OMIT,
             should_embed: typing.Optional[bool] = OMIT,
             model: typing.Optional[str] = OMIT,
             instruction: typing.Optional[str] = OMIT,
-    ) -> HandleFileExtractionV1DocumentExtractTextPostResponse:
+    ) -> DocumentFileTextExtractionResponse:
         request_data: typing.Dict[str, typing.Any] = {
             "should_chunk": should_chunk,
             "chunk_size": chunk_size,
             "chunk_overlap": chunk_overlap,
             "chunk_splitter": chunk_splitter,
             "separators": separators,
             "should_embed": should_embed,
@@ -186,15 +177,15 @@
             "instruction": instruction,
         }
         files = {"file": file}
 
         return self.send_request(
             "POST",
             "v1/document/extract-text/",
-            HandleFileExtractionV1DocumentExtractTextPostResponse,
+            DocumentExtractionResponseWithEmbeddings if should_embed is True else DocumentExtractionResponse,
             request_data=request_data,
             files=files,
         )
 
     def extract_text_from_bytes(
             self,
             *,
@@ -203,15 +194,15 @@
             chunk_size: typing.Optional[int] = OMIT,
             chunk_overlap: typing.Optional[int] = OMIT,
             chunk_splitter: typing.Optional[ChunkSplitter] = OMIT,
             separators: typing.Optional[typing.List[str]] = OMIT,
             should_embed: typing.Optional[bool] = OMIT,
             model: typing.Optional[str] = OMIT,
             instruction: typing.Optional[str] = OMIT,
-    ) -> HandleByteExtractionV1DocumentExtractTextBytesPostResponse:
+    ) -> DocumentByteTextExtractionResponse:
         request_data: typing.Dict[str, typing.Any] = {
             "should_chunk": should_chunk,
             "chunk_size": chunk_size,
             "chunk_overlap": chunk_overlap,
             "chunk_splitter": chunk_splitter,
             "separators": separators,
             "should_embed": should_embed,
@@ -220,15 +211,15 @@
             "bytes": base64.b64encode(bytes_or_base64).decode() if isinstance(bytes_or_base64,
                                                                               bytes) else bytes_or_base64,
         }
 
         return self.send_request(
             "POST",
             "v1/document/extract-text/bytes/",
-            HandleByteExtractionV1DocumentExtractTextBytesPostResponse,
+            DocumentExtractionResponseWithEmbeddings if should_embed is True else DocumentExtractionResponse,
             request_data=request_data,
         )
 
     def whisper(self, *, file: typing.IO) -> WhisperResponse:
         files = {"file": file}
 
         return self.send_request(
@@ -278,15 +269,15 @@
             chunk_size: typing.Optional[int] = OMIT,
             chunk_overlap: typing.Optional[int] = OMIT,
             chunk_splitter: typing.Optional[ChunkSplitter] = OMIT,
             separators: typing.Optional[typing.List[str]] = OMIT,
             should_embed: typing.Optional[bool] = OMIT,
             model: typing.Optional[str] = OMIT,
             instruction: typing.Optional[str] = OMIT,
-    ) -> HandleFileExtractionV1DocumentExtractTextPostResponse:
+    ) -> DocumentFileTextExtractionResponse:
         request_data: typing.Dict[str, typing.Any] = {
             "should_chunk": should_chunk,
             "chunk_size": chunk_size,
             "chunk_overlap": chunk_overlap,
             "chunk_splitter": chunk_splitter,
             "separators": separators,
             "should_embed": should_embed,
@@ -294,15 +285,15 @@
             "instruction": instruction,
         }
         files = {"file": file}
 
         return await self.send_request(
             "POST",
             "v1/document/extract-text/",
-            HandleFileExtractionV1DocumentExtractTextPostResponse,
+            DocumentExtractionResponseWithEmbeddings if should_embed is True else DocumentExtractionResponse,
             request_data=request_data,
             files=files,
         )
 
     async def extract_text_from_bytes(
             self,
             *,
@@ -311,15 +302,15 @@
             chunk_size: typing.Optional[int] = OMIT,
             chunk_overlap: typing.Optional[int] = OMIT,
             chunk_splitter: typing.Optional[ChunkSplitter] = OMIT,
             separators: typing.Optional[typing.List[str]] = OMIT,
             should_embed: typing.Optional[bool] = OMIT,
             model: typing.Optional[str] = OMIT,
             instruction: typing.Optional[str] = OMIT,
-    ) -> HandleByteExtractionV1DocumentExtractTextBytesPostResponse:
+    ) -> DocumentByteTextExtractionResponse:
         request_data: typing.Dict[str, typing.Any] = {
             "should_chunk": should_chunk,
             "chunk_size": chunk_size,
             "chunk_overlap": chunk_overlap,
             "chunk_splitter": chunk_splitter,
             "separators": separators,
             "should_embed": should_embed,
@@ -328,15 +319,15 @@
             "bytes": base64.b64encode(bytes_or_base64).decode() if isinstance(bytes_or_base64,
                                                                               bytes) else bytes_or_base64,
         }
 
         return await self.send_request(
             "POST",
             "v1/document/extract-text/bytes/",
-            HandleByteExtractionV1DocumentExtractTextBytesPostResponse,
+            DocumentExtractionResponseWithEmbeddings if should_embed is True else DocumentExtractionResponse,
             request_data=request_data,
         )
 
     async def whisper(self, *, file: typing.IO) -> WhisperResponse:
         files = {"file": file}
 
         return await self.send_request(
```

### Comparing `embaas-0.0.3/embaas/core/datetime_utils.py` & `embaas-0.0.4/embaas/core/datetime_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 
 
 def serialize_datetime(v: dt.datetime) -> str:
     """
     Serialize a datetime including timezone info.
```

### Comparing `embaas-0.0.3/embaas/core/jsonable_encoder.py` & `embaas-0.0.4/embaas/core/jsonable_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 """
 jsonable_encoder converts a Python object to a JSON-friendly dict
 (e.g. datetimes to strings, Pydantic models to dicts).
 
 Taken from FastAPI, and made a bit simpler
 https://github.com/tiangolo/fastapi/blob/master/fastapi/encoders.py
```

### Comparing `embaas-0.0.3/embaas/types/chunk_splitter.py` & `embaas-0.0.4/embaas/types/chunk_splitter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
```

### Comparing `embaas-0.0.3/embaas/types/document_chunk.py` & `embaas-0.0.4/embaas/types/whisper_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentChunk(pydantic.BaseModel):
-    text: str
-    metadata: typing.Dict[str, typing.Any]
-    embedding: typing.Optional[typing.List[float]]
-    index: int
+class WhisperResult(pydantic.BaseModel):
+    transcription: str
+    start: float
+    end: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `embaas-0.0.3/embaas/types/document_extraction_response.py` & `embaas-0.0.4/embaas/types/document_extraction_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ..core.datetime_utils import serialize_datetime
 from .document_extraction_result import DocumentExtractionResult
 from .document_usage import DocumentUsage
+from ..core.datetime_utils import serialize_datetime
 
 
 class DocumentExtractionResponse(pydantic.BaseModel):
     usage: DocumentUsage
     data: DocumentExtractionResult
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `embaas-0.0.3/embaas/types/document_extraction_response_with_embeddings.py` & `embaas-0.0.4/embaas/types/document_extraction_response_with_embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ..core.datetime_utils import serialize_datetime
 from .document_extraction_result import DocumentExtractionResult
 from .document_with_embeddings_usage import DocumentWithEmbeddingsUsage
+from ..core.datetime_utils import serialize_datetime
 
 
 class DocumentExtractionResponseWithEmbeddings(pydantic.BaseModel):
     usage: DocumentWithEmbeddingsUsage
     data: DocumentExtractionResult
     model: str
```

### Comparing `embaas-0.0.3/embaas/types/document_extraction_result.py` & `embaas-0.0.4/embaas/types/whisper_usage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_chunk import DocumentChunk
 
 
-class DocumentExtractionResult(pydantic.BaseModel):
-    chunks: typing.List[DocumentChunk]
-    metadata: typing.Dict[str, typing.Any]
+class WhisperUsage(pydantic.BaseModel):
+    total_duration: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `embaas-0.0.3/embaas/types/document_usage.py` & `embaas-0.0.4/embaas/types/usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# This file was auto-generated by Fern from our API Definition.
-
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class DocumentUsage(pydantic.BaseModel):
-    total_mb: float
+class Usage(pydantic.BaseModel):
+    prompt_tokens: int
+    total_tokens: int
+    completion_tokens: typing.Optional[int]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `embaas-0.0.3/embaas/types/document_with_embeddings_usage.py` & `embaas-0.0.4/embaas/types/document_with_embeddings_usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
```

### Comparing `embaas-0.0.3/embaas/types/embedding.py` & `embaas-0.0.4/embaas/types/document_usage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class Embedding(pydantic.BaseModel):
-    embedding: typing.List[float]
-    index: int
-    was_truncated: typing.Optional[bool]
+class DocumentUsage(pydantic.BaseModel):
+    total_mb: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `embaas-0.0.3/embaas/types/embeddings_response.py` & `embaas-0.0.4/embaas/types/validation_error.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
+from .validation_error_loc_item import ValidationErrorLocItem
 from ..core.datetime_utils import serialize_datetime
-from .embedding import Embedding
-from .usage import Usage
 
 
-class EmbeddingsResponse(pydantic.BaseModel):
-    usage: Usage
-    model: str
-    data: typing.List[Embedding]
+class ValidationError(pydantic.BaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `embaas-0.0.3/embaas/types/http_validation_error.py` & `embaas-0.0.4/embaas/types/http_validation_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ..core.datetime_utils import serialize_datetime
 from .validation_error import ValidationError
+from ..core.datetime_utils import serialize_datetime
 
 
 class HttpValidationError(pydantic.BaseModel):
     detail: typing.Optional[typing.List[ValidationError]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `embaas-0.0.3/embaas/types/whisper_response.py` & `embaas-0.0.4/embaas/types/whisper_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ..core.datetime_utils import serialize_datetime
 from .whisper_result import WhisperResult
 from .whisper_usage import WhisperUsage
+from ..core.datetime_utils import serialize_datetime
 
 
 class WhisperResponse(pydantic.BaseModel):
     data: typing.List[WhisperResult]
     usage: WhisperUsage
     model: str
```

### Comparing `embaas-0.0.3/embaas/types/whisper_result.py` & `embaas-0.0.4/embaas/types/document_extraction_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
+from .document_chunk import DocumentChunk
 from ..core.datetime_utils import serialize_datetime
 
 
-class WhisperResult(pydantic.BaseModel):
-    transcription: str
-    start: float
-    end: float
+class DocumentExtractionResult(pydantic.BaseModel):
+    chunks: typing.List[DocumentChunk]
+    metadata: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `embaas-0.0.3/embaas/types/whisper_usage.py` & `embaas-0.0.4/embaas/types/embeddings_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-# This file was auto-generated by Fern from our API Definition.
+
 
 import datetime as dt
 import typing
 
 import pydantic
 
+from .embedding import Embedding
+from .usage import Usage
 from ..core.datetime_utils import serialize_datetime
 
 
-class WhisperUsage(pydantic.BaseModel):
-    total_duration: float
+class EmbeddingsResponse(pydantic.BaseModel):
+    usage: Usage
+    model: str
+    data: typing.List[Embedding]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `embaas-0.0.3/embaas/utils.py` & `embaas-0.0.4/embaas/utils.py`

 * *Files identical despite different names*

### Comparing `embaas-0.0.3/embaas.egg-info/PKG-INFO` & `embaas-0.0.4/embaas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embaas
-Version: 0.0.3
+Version: 0.0.4
 Summary: embaas Python SDK
 Author-email: Julius Lipp <julius@embaas.io>, embaas <info@embaas.io>
 License: MIT License
         
         Copyright (c) 2023 Embaas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `embaas-0.0.3/embaas.egg-info/SOURCES.txt` & `embaas-0.0.4/embaas.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 embaas/core/jsonable_encoder.py
 embaas/core/remove_none_from_headers.py
 embaas/errors/__init__.py
 embaas/errors/api_error.py
 embaas/errors/unprocessable_entity_error.py
 embaas/types/__init__.py
 embaas/types/chunk_splitter.py
+embaas/types/document_byte_text_extraction_response.py
 embaas/types/document_chunk.py
 embaas/types/document_extraction_response.py
 embaas/types/document_extraction_response_with_embeddings.py
 embaas/types/document_extraction_result.py
+embaas/types/document_file_text_extraction_response.py
 embaas/types/document_usage.py
 embaas/types/document_with_embeddings_usage.py
 embaas/types/embedding.py
 embaas/types/embeddings_response.py
-embaas/types/handle_byte_extraction_v_1_document_extract_text_bytes_post_response.py
-embaas/types/handle_file_extraction_v_1_document_extract_text_post_response.py
 embaas/types/http_validation_error.py
 embaas/types/usage.py
 embaas/types/validation_error.py
 embaas/types/validation_error_loc_item.py
 embaas/types/whisper_response.py
 embaas/types/whisper_result.py
 embaas/types/whisper_usage.py
```

### Comparing `embaas-0.0.3/pyproject.toml` & `embaas-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embaas"
-version = "0.0.3"
+version = "0.0.4"
 description = "embaas Python SDK"
 readme = "README.md"
 authors = [
     { name = "Julius Lipp", email = "julius@embaas.io" },
     { name = "embaas", email = "info@embaas.io" }
 ]
 license = { file = "LICENSE" }
```

