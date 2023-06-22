# Comparing `tmp/pilot_platform_object_storage-1.1.1.tar.gz` & `tmp/pilot_platform_object_storage-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot_platform_object_storage-1.1.1.tar", max compression
+gzip compressed data, was "pilot_platform_object_storage-1.2.0.tar", max compression
```

## Comparing `pilot_platform_object_storage-1.1.1.tar` & `pilot_platform_object_storage-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3336 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/README.md
--rw-r--r--   0        0        0      120 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/__init__.py
--rw-r--r--   0        0        0      324 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/__init__.py
--rw-r--r--   0        0        0     4506 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/azure_blob_client.py
--rw-r--r--   0        0        0     5162 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/azure_container_client.py
--rw-r--r--   0        0        0     2143 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/base_container_client.py
--rw-r--r--   0        0        0     2051 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/clients/base_file_client.py
--rw-r--r--   0        0        0     1902 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/factories.py
--rw-r--r--   0        0        0      239 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/managers/__init__.py
--rw-r--r--   0        0        0     3762 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/managers/azure_blob_manager.py
--rw-r--r--   0        0        0      727 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/managers/base_manager.py
--rw-r--r--   0        0        0      196 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/providers/__init__.py
--rw-r--r--   0        0        0     4902 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/providers/azure.py
--rw-r--r--   0        0        0      444 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/object_storage/providers/enum.py
--rw-r--r--   0        0        0     1009 2023-05-31 15:19:27.085006 pilot_platform_object_storage-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.1.1/setup.py
--rw-r--r--   0        0        0     3914 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3493 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/README.md
+-rw-r--r--   0        0        0      120 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/__init__.py
+-rw-r--r--   0        0        0      324 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/clients/__init__.py
+-rw-r--r--   0        0        0     6442 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/clients/azure_blob_client.py
+-rw-r--r--   0        0        0     7083 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/clients/azure_container_client.py
+-rw-r--r--   0        0        0     2143 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/clients/base_container_client.py
+-rw-r--r--   0        0        0     2051 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/clients/base_file_client.py
+-rw-r--r--   0        0        0     1902 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/factories.py
+-rw-r--r--   0        0        0      239 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/managers/__init__.py
+-rw-r--r--   0        0        0     3763 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/managers/azure_blob_manager.py
+-rw-r--r--   0        0        0      727 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/managers/base_manager.py
+-rw-r--r--   0        0        0      266 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/providers/__init__.py
+-rw-r--r--   0        0        0     6322 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/providers/azure.py
+-rw-r--r--   0        0        0      444 2023-06-22 14:30:36.162749 pilot_platform_object_storage-1.2.0/object_storage/providers/enum.py
+-rw-r--r--   0        0        0     1181 2023-06-22 14:30:36.166749 pilot_platform_object_storage-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.2.0/setup.py
+-rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.2.0/PKG-INFO
```

### Comparing `pilot_platform_object_storage-1.1.1/README.md` & `pilot_platform_object_storage-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 [![Run Tests](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml)
 [![Python](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/pilot-platform-object-storage.svg)](https://pypi.org/project/pilot-platform-object-storage/)
 
 Provides a simple and flexible Python library for efficient and reliable object storage solutions. Enables direct interaction with multiple object storage APIs, starting with Azure Blob API and with plans to add more in the future
 
-
 ## Getting Started
 
 ### Manager
 ```python
 import asyncio
 from object_storage.factories import get_manager
 
@@ -53,15 +52,14 @@
 
 container_sas_url = 'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature'
 azr_container_client = get_container_client('azure', container_sas_url)
 asyncio.run(azr_container_client.upload_file('small.txt', './small.txt'))
 
 ```
 
-
 ## Installation & Quick Start
 The latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.
 
 Pip install from PyPi:
 ```
 pip install pilot-platform-object-storage
 ```
@@ -72,14 +70,18 @@
 ```
 
 Pip install from a local `.whl` file:
 ```
 pip install pilot_platform_object_storage-<VERSION>-py3-none-any.whl
 ```
 
+## Documentation
+
+API Reference and User Guide available at [pilotdataplatform.github.io/object-storage](https://pilotdataplatform.github.io/object-storage/)
+
 ## Contribution
 
 You can contribute the project in following ways:
 
 * Report a bug.
 * Suggest a feature.
 * Open a pull request for fixing issues or adding functionality. Please consider using [pre-commit](https://pre-commit.com) in this case.
```

### Comparing `pilot_platform_object_storage-1.1.1/object_storage/clients/azure_container_client.py` & `pilot_platform_object_storage-1.2.0/object_storage/clients/azure_container_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import Optional
 
 from azure.storage.blob import BlobProperties
 from azure.storage.blob.aio import ContainerClient
+from azure.storage.blob.aio import StorageStreamDownloader
 
 from object_storage.clients.base_container_client import BaseContainerClient
 from object_storage.providers.azure import AzureClient
 
-logger = logging.getLogger('pilot.obect_storage')
+logger = logging.getLogger('pilot.object-storage')
 
 
 class AzureContainerClient(BaseContainerClient, AzureClient):
     """A client for interacting with Azure Blob Storage.
 
     Inherits from:
         - BaseObjectStorageClient: to provide a generic interface for object storage clients
@@ -38,98 +39,134 @@
         self,
         key: str,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> Dict[str, Any]:
         """Uploads a file to a blob in the specified container."""
-
-        async with ContainerClient.from_container_url(
-            container_url=self.container_sas_url, max_block_size=chunk_size
-        ) as container_client:
-            blob_client = container_client.get_blob_client(key)
-            return await self._upload(blob_client, file_path, key, progress_callback)
+        try:
+            async with ContainerClient.from_container_url(
+                container_url=self.container_sas_url, max_block_size=chunk_size
+            ) as container_client:
+                blob_client = container_client.get_blob_client(key)
+                return await self._upload(blob_client, file_path, key, progress_callback)
+        except Exception as exc:
+            raise self._handle_exception(exc)
 
     async def resume_upload(
         self,
         key: str,
         file_path: str,
         chunk_size: int = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Uploads a file to an Azure Blob Storage container, resuming an interrupted upload if there is an uncommitted
         block list."""
-
-        async with ContainerClient.from_container_url(
-            container_url=self.container_sas_url, max_block_size=chunk_size
-        ) as container_client:
-            blob_client = container_client.get_blob_client(key)
-            await self._resume_upload(blob_client, key, file_path, chunk_size, progress_callback)
+        try:
+            async with ContainerClient.from_container_url(
+                container_url=self.container_sas_url, max_block_size=chunk_size
+            ) as container_client:
+                blob_client = container_client.get_blob_client(key)
+                await self._resume_upload(blob_client, key, file_path, chunk_size, progress_callback)
+        except Exception as exc:
+            raise self._handle_exception(exc)
 
     async def download_file_to_bytes(
         self,
         key: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> bytes:
         """Download a file from the specified container."""
-
-        async with ContainerClient.from_container_url(
-            container_url=self.container_sas_url, max_chunk_get_size=chunk_size
-        ) as container_client:
-            blob_client = container_client.get_blob_client(key)
-            return await self._download_bytes(blob_client, key, progress_callback=progress_callback)
+        try:
+            async with ContainerClient.from_container_url(
+                container_url=self.container_sas_url, max_chunk_get_size=chunk_size
+            ) as container_client:
+                blob_client = container_client.get_blob_client(key)
+                return await self._download_bytes(blob_client, key, progress_callback=progress_callback)
+        except Exception as exc:
+            raise self._handle_exception(exc)
 
     async def download_file(
         self,
         key: str,
         file_path: str,
         chunk_size: Optional[int] = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Download a file from the specified container."""
 
         await self._create_parent_dir(file_path)
-
-        async with ContainerClient.from_container_url(
-            container_url=self.container_sas_url, max_chunk_get_size=chunk_size
-        ) as container_client:
-            blob_client = container_client.get_blob_client(key)
-            await self._download(blob_client, key, file_path, chunk_size, progress_callback)
+        try:
+            async with ContainerClient.from_container_url(
+                container_url=self.container_sas_url, max_chunk_get_size=chunk_size
+            ) as container_client:
+                blob_client = container_client.get_blob_client(key)
+                await self._download(blob_client, key, file_path, chunk_size, progress_callback)
+        except Exception as exc:
+            raise self._handle_exception(exc)
 
     async def copy_file_from_url(
         self,
         key: str,
         source_url: str,
     ) -> str:
         """Copies a file from a URL to a blob in the specified container."""
-
-        async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
-            blob_client = container_client.get_blob_client(key)
-            return await self._copy_from_url(blob_client, source_url)
+        try:
+            async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+                blob_client = container_client.get_blob_client(key)
+                return await self._copy_from_url(blob_client, source_url)
+        except Exception as exc:
+            raise self._handle_exception(exc)
 
     async def delete_file(self, key: str) -> None:
         """Deleted a file with all its snapshots."""
-
-        async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
-            blob_client = container_client.get_blob_client(key)
-            return await self._delete(blob_client)
+        try:
+            async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+                blob_client = container_client.get_blob_client(key)
+                return await self._delete(blob_client)
+        except Exception as exc:
+            raise self._handle_exception(exc)
 
     async def get_file_url(
         self,
         key: str,
     ) -> str:
         """Returns the URL that can be used to access the specified file."""
-
-        async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
-            blob_client = container_client.get_blob_client(key)
-            return blob_client.url
+        try:
+            async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+                blob_client = container_client.get_blob_client(key)
+                return blob_client.url
+        except Exception as exc:
+            raise self._handle_exception(exc)
 
     async def get_file_properties(
         self,
         key: str,
     ) -> BlobProperties:
         """Retrieves the properties of a blob in the specified container."""
-
-        async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
-            blob_client = container_client.get_blob_client(blob=key)
-            return await blob_client.get_blob_properties()
+        try:
+            async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+                blob_client = container_client.get_blob_client(blob=key)
+                return await blob_client.get_blob_properties()
+        except Exception as exc:
+            raise self._handle_exception(exc)
+
+    async def commit_file(self, key: str) -> None:
+        """Commits the uncommitted blocks of a blob, making them a part of the blob's content."""
+
+        try:
+            async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+                blob_client = container_client.get_blob_client(blob=key)
+                await self._commit_blob(blob_client)
+        except Exception as exc:
+            raise self._handle_exception(exc)
+
+    async def get_file_chunks(self, key: str) -> StorageStreamDownloader[str]:
+        """Returns a stream downloader for downloading the contents of a blob in chunks."""
+
+        try:
+            async with ContainerClient.from_container_url(container_url=self.container_sas_url) as container_client:
+                blob_client = container_client.get_blob_client(blob=key)
+                return await self._get_blob_chunks(blob_client)
+        except Exception as exc:
+            raise self._handle_exception(exc)
```

### Comparing `pilot_platform_object_storage-1.1.1/object_storage/clients/base_container_client.py` & `pilot_platform_object_storage-1.2.0/object_storage/clients/base_container_client.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.1/object_storage/clients/base_file_client.py` & `pilot_platform_object_storage-1.2.0/object_storage/clients/base_file_client.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.1/object_storage/factories.py` & `pilot_platform_object_storage-1.2.0/object_storage/factories.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.1/object_storage/managers/azure_blob_manager.py` & `pilot_platform_object_storage-1.2.0/object_storage/managers/azure_blob_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from azure.storage.blob import BlobSasPermissions
 from azure.storage.blob import generate_blob_sas
 from azure.storage.blob import generate_container_sas
 from azure.storage.blob.aio import BlobServiceClient
 
 from object_storage.managers.base_manager import BaseObjectStorageManager
 
-logger = logging.getLogger('pilot.obect_storage')
+logger = logging.getLogger('pilot.object-storage')
 
 
 class AzureBlobStorageManager(BaseObjectStorageManager):
     """A client for interacting with Azure Blob Storage.
 
     Inherits from:
         - BaseObjectStorageManager: to provide a generic interface for object storage clients
```

### Comparing `pilot_platform_object_storage-1.1.1/object_storage/managers/base_manager.py` & `pilot_platform_object_storage-1.2.0/object_storage/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.1.1/object_storage/providers/azure.py` & `pilot_platform_object_storage-1.2.0/object_storage/providers/azure.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,56 @@
 # Copyright (C) 2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
+import logging
 from pathlib import Path
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from uuid import uuid4
 
 import aiofiles
 import aiofiles.os
 from aiofiles.os import makedirs
+from azure.core.exceptions import ClientAuthenticationError
+from azure.core.exceptions import HttpResponseError
+from azure.core.exceptions import ResourceNotFoundError
 from azure.storage.blob import BlobBlock
 from azure.storage.blob.aio import BlobClient
+from azure.storage.blob.aio import StorageStreamDownloader
+
+logger = logging.getLogger('pilot.object-storage')
 
 
 class AzureClient:
     """Base base class for object storage clients."""
 
+    def _handle_exception(self, exc: Exception) -> Exception:
+        """Handles exceptions raised during Azure Blob Storage operations."""
+        if isinstance(exc, ClientAuthenticationError):
+            logger.exception(
+                'Failed to authenticate with Azure. Check the correctness of tenant_id, client_id, or client_secret.'
+            )
+        elif isinstance(exc, ResourceNotFoundError):
+            logger.info('The requested resource was not found.')
+        elif isinstance(exc, HttpResponseError):
+            logger.exception(f'Error in HTTP response: {exc.status_code} - {exc.reason}')
+        else:
+            logger.exception('Unexpected error occurred')
+        return exc
+
+    async def _create_parent_dir(self, file_path: str) -> None:
+        """The funtion will create the parent folder by the file path."""
+
+        dirname = str(Path(file_path).parent)
+        await makedirs(dirname, exist_ok=True)
+
     async def _upload(
         self,
         client: BlobClient,
         file_path: str,
         key: str,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> Dict[str, Any]:
@@ -45,15 +72,15 @@
         self,
         client: BlobClient,
         key: str,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> bytes:
         """Download a file from the specified container."""
 
-        stream = await client.download_blob(max_concurrency=4)
+        stream = await self._get_blob_chunks(client)
         chunk_list = []
         current = 0
         async for chunk in stream.chunks():
             current += len(chunk)
             if progress_callback:
                 await progress_callback(key, current, stream.size)
             chunk_list.append(chunk)
@@ -103,38 +130,48 @@
         """Uploads a file to an Azure Blob Storage container, resuming an interrupted upload if there is an uncommitted
         block list."""
 
         uploaded_blocks = []
         offset = 0
         current = 0
 
-        async with client as blob_client:
-            _, block_list = await blob_client.get_block_list('uncommitted')
-            for block in block_list:
-                offset += block.size
-                uploaded_blocks.append(block.id)
-
-            current = offset
-            file_length = (await aiofiles.os.stat(file_path)).st_size
-            file_renaming_length = file_length - offset
-
-            if file_renaming_length:
-                async with aiofiles.open(file_path, mode='rb') as f:
-                    await f.seek(offset)
-                    while True:
-                        chunk = await f.read(chunk_size)
-                        if not chunk:
-                            break
-                        block_id = str(uuid4())
-                        await blob_client.stage_block(block_id=block_id, data=chunk)
-                        current += chunk_size
-                        if progress_callback:
-                            await progress_callback(key, current, file_length)
-                        uploaded_blocks.append(BlobBlock(block_id=block_id))
+        _, block_list = await client.get_block_list('uncommitted')
+        for block in block_list:
+            offset += block.size
+            uploaded_blocks.append(block.id)
+
+        current = offset
+        file_length = (await aiofiles.os.stat(file_path)).st_size
+        file_renaming_length = file_length - offset
+
+        if file_renaming_length:
+            async with aiofiles.open(file_path, mode='rb') as f:
+                await f.seek(offset)
+                while True:
+                    chunk = await f.read(chunk_size)
+                    if not chunk:
+                        break
+                    block_id = str(uuid4())
+                    await client.stage_block(block_id=block_id, data=chunk)
+                    current += chunk_size
+                    if progress_callback:
+                        await progress_callback(key, current, file_length)
+                    uploaded_blocks.append(BlobBlock(block_id=block_id))
 
-            await blob_client.commit_block_list(uploaded_blocks)
+        await client.commit_block_list(uploaded_blocks)
 
-    async def _create_parent_dir(self, file_path: str) -> None:
-        """The funtion will create the parent folder by the file path."""
+    async def _commit_blob(
+        self,
+        client: BlobClient,
+    ) -> None:
+        """Commits the uncommitted blocks of a blob, making them a part of the blob's content."""
 
-        dirname = str(Path(file_path).parent)
-        await makedirs(dirname, exist_ok=True)
+        _, block_list = await client.get_block_list('uncommitted')
+        await client.commit_block_list(block_list)
+
+    async def _get_blob_chunks(
+        self,
+        client: BlobClient,
+    ) -> StorageStreamDownloader[str]:
+        """Returns a stream downloader for downloading the contents of a blob in chunks."""
+
+        return await client.download_blob(max_concurrency=4)
```

### Comparing `pilot_platform_object_storage-1.1.1/pyproject.toml` & `pilot_platform_object_storage-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 [tool.poetry]
 name = "pilot-platform-object-storage"
-version = "1.1.1"
+version = "1.2.0"
 description = "Python library for interacting with multiple object storage APIs."
 authors = ["Indoc Research"]
 readme = "README.md"
 packages = [{include = "object_storage"}]
+license = "Proprietary"
+documentation = "https://pilotdataplatform.github.io/object-storage/"
+
 
 [tool.poetry.dependencies]
 python = "^3.9"
 azure-storage-blob = "^12.16.0"
 aiohttp = "^3.8.4"
 aiofiles = "^23.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-random-order = "^1.1.0"
 testcontainers = "^3.7.1"
 pytest-asyncio = "^0.21.0"
+mkdocs = "^1.4.3"
+pymdown-extensions = "^10.0.1"
+mkdocs-material = "^9.1.15"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `pilot_platform_object_storage-1.1.1/setup.py` & `pilot_platform_object_storage-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 install_requires = \
 ['aiofiles>=23.1.0,<24.0.0',
  'aiohttp>=3.8.4,<4.0.0',
  'azure-storage-blob>=12.16.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'pilot-platform-object-storage',
-    'version': '1.1.1',
+    'version': '1.2.0',
     'description': 'Python library for interacting with multiple object storage APIs.',
-    'long_description': '# Pilot Platform Storage Manager\n\n[![Run Tests](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml)\n[![Python](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://www.python.org/)\n[![PyPI](https://img.shields.io/pypi/v/pilot-platform-object-storage.svg)](https://pypi.org/project/pilot-platform-object-storage/)\n\nProvides a simple and flexible Python library for efficient and reliable object storage solutions. Enables direct interaction with multiple object storage APIs, starting with Azure Blob API and with plans to add more in the future\n\n\n## Getting Started\n\n### Manager\n```python\nimport asyncio\nfrom object_storage.factories import get_manager\n\nconnection_string = \'DefaultEndpointsProtocol=https;AccountName=pilot;AccountKey=any;EndpointSuffix=core.windows.net\'\nazr_manager = get_manager(\'azure\', connection_string)\n\naccount_sas = asyncio.run(azr_manager.get_container_sas(\'test\'))\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\n\n\nblob_sas = asyncio.run(azr_manager.get_blob_sas(\'test\', \'small.txt\'))\n\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=blob_signature\'\n\n\nblobs_list = asyncio.run(azr_manager.list_objects(\'test\'))\nprint(blobs_list)\n> [<class \'azure.storage.blob._models.BlobProperties\'>, ...]\n\n\nblobs_list = asyncio.run(azr_manager.create_container(\'test\'))\n```\n\n### File Client\n```python\nimport asyncio\nfrom object_storage.factories import get_file_client\n\nblob_sas_url = \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_file_client = get_file_client(\'azure\', blob_sas_url)\nasyncio.run(azr_file_client.upload_file(\'./small.txt\'))\n```\n\n### Container Client\n```python\nimport asyncio\nfrom object_storage.factories import get_container_client\n\ncontainer_sas_url = \'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_container_client = get_container_client(\'azure\', container_sas_url)\nasyncio.run(azr_container_client.upload_file(\'small.txt\', \'./small.txt\'))\n\n```\n\n\n## Installation & Quick Start\nThe latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.\n\nPip install from PyPi:\n```\npip install pilot-platform-object-storage\n```\n\nIn `pyproject.toml`:\n```\npilot-platform-object-storage = "^<VERSION>"\n```\n\nPip install from a local `.whl` file:\n```\npip install pilot_platform_object_storage-<VERSION>-py3-none-any.whl\n```\n\n## Contribution\n\nYou can contribute the project in following ways:\n\n* Report a bug.\n* Suggest a feature.\n* Open a pull request for fixing issues or adding functionality. Please consider using [pre-commit](https://pre-commit.com) in this case.\n* For general guidelines on how to contribute to the project, please take a look at the [contribution guide](CONTRIBUTING.md).\n',
+    'long_description': '# Pilot Platform Storage Manager\n\n[![Run Tests](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml)\n[![Python](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://www.python.org/)\n[![PyPI](https://img.shields.io/pypi/v/pilot-platform-object-storage.svg)](https://pypi.org/project/pilot-platform-object-storage/)\n\nProvides a simple and flexible Python library for efficient and reliable object storage solutions. Enables direct interaction with multiple object storage APIs, starting with Azure Blob API and with plans to add more in the future\n\n## Getting Started\n\n### Manager\n```python\nimport asyncio\nfrom object_storage.factories import get_manager\n\nconnection_string = \'DefaultEndpointsProtocol=https;AccountName=pilot;AccountKey=any;EndpointSuffix=core.windows.net\'\nazr_manager = get_manager(\'azure\', connection_string)\n\naccount_sas = asyncio.run(azr_manager.get_container_sas(\'test\'))\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\n\n\nblob_sas = asyncio.run(azr_manager.get_blob_sas(\'test\', \'small.txt\'))\n\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=blob_signature\'\n\n\nblobs_list = asyncio.run(azr_manager.list_objects(\'test\'))\nprint(blobs_list)\n> [<class \'azure.storage.blob._models.BlobProperties\'>, ...]\n\n\nblobs_list = asyncio.run(azr_manager.create_container(\'test\'))\n```\n\n### File Client\n```python\nimport asyncio\nfrom object_storage.factories import get_file_client\n\nblob_sas_url = \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_file_client = get_file_client(\'azure\', blob_sas_url)\nasyncio.run(azr_file_client.upload_file(\'./small.txt\'))\n```\n\n### Container Client\n```python\nimport asyncio\nfrom object_storage.factories import get_container_client\n\ncontainer_sas_url = \'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_container_client = get_container_client(\'azure\', container_sas_url)\nasyncio.run(azr_container_client.upload_file(\'small.txt\', \'./small.txt\'))\n\n```\n\n## Installation & Quick Start\nThe latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.\n\nPip install from PyPi:\n```\npip install pilot-platform-object-storage\n```\n\nIn `pyproject.toml`:\n```\npilot-platform-object-storage = "^<VERSION>"\n```\n\nPip install from a local `.whl` file:\n```\npip install pilot_platform_object_storage-<VERSION>-py3-none-any.whl\n```\n\n## Documentation\n\nAPI Reference and User Guide available at [pilotdataplatform.github.io/object-storage](https://pilotdataplatform.github.io/object-storage/)\n\n## Contribution\n\nYou can contribute the project in following ways:\n\n* Report a bug.\n* Suggest a feature.\n* Open a pull request for fixing issues or adding functionality. Please consider using [pre-commit](https://pre-commit.com) in this case.\n* For general guidelines on how to contribute to the project, please take a look at the [contribution guide](CONTRIBUTING.md).\n',
     'author': 'Indoc Research',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pilot_platform_object_storage-1.1.1/PKG-INFO` & `pilot_platform_object_storage-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: pilot-platform-object-storage
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python library for interacting with multiple object storage APIs.
+License: Proprietary
 Author: Indoc Research
 Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: azure-storage-blob (>=12.16.0,<13.0.0)
+Project-URL: Documentation, https://pilotdataplatform.github.io/object-storage/
 Description-Content-Type: text/markdown
 
 # Pilot Platform Storage Manager
 
 [![Run Tests](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml)
 [![Python](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/pilot-platform-object-storage.svg)](https://pypi.org/project/pilot-platform-object-storage/)
 
 Provides a simple and flexible Python library for efficient and reliable object storage solutions. Enables direct interaction with multiple object storage APIs, starting with Azure Blob API and with plans to add more in the future
 
-
 ## Getting Started
 
 ### Manager
 ```python
 import asyncio
 from object_storage.factories import get_manager
 
@@ -68,15 +70,14 @@
 
 container_sas_url = 'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature'
 azr_container_client = get_container_client('azure', container_sas_url)
 asyncio.run(azr_container_client.upload_file('small.txt', './small.txt'))
 
 ```
 
-
 ## Installation & Quick Start
 The latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.
 
 Pip install from PyPi:
 ```
 pip install pilot-platform-object-storage
 ```
@@ -87,14 +88,18 @@
 ```
 
 Pip install from a local `.whl` file:
 ```
 pip install pilot_platform_object_storage-<VERSION>-py3-none-any.whl
 ```
 
+## Documentation
+
+API Reference and User Guide available at [pilotdataplatform.github.io/object-storage](https://pilotdataplatform.github.io/object-storage/)
+
 ## Contribution
 
 You can contribute the project in following ways:
 
 * Report a bug.
 * Suggest a feature.
 * Open a pull request for fixing issues or adding functionality. Please consider using [pre-commit](https://pre-commit.com) in this case.
```

