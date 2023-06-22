# Comparing `tmp/pinecone_datasets-0.5.0rc7.tar.gz` & `tmp/pinecone_datasets-0.5.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_datasets-0.5.0rc7.tar", max compression
+gzip compressed data, was "pinecone_datasets-0.5.0rc8.tar", max compression
```

## Comparing `pinecone_datasets-0.5.0rc7.tar` & `pinecone_datasets-0.5.0rc8.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     8945 2023-06-10 20:04:06.109588 pinecone_datasets-0.5.0rc7/README.md
--rw-r--r--   0        0        0      263 2023-06-15 08:51:37.997122 pinecone_datasets-0.5.0rc7/pinecone_datasets/__init__.py
--rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.5.0rc7/pinecone_datasets/catalog.py
--rw-r--r--   0        0        0     1185 2023-06-12 13:33:01.718779 pinecone_datasets-0.5.0rc7/pinecone_datasets/cfg.py
--rw-r--r--   0        0        0    20186 2023-06-15 08:42:45.599902 pinecone_datasets-0.5.0rc7/pinecone_datasets/dataset.py
--rw-r--r--   0        0        0     1765 2023-06-10 19:50:50.284354 pinecone_datasets-0.5.0rc7/pinecone_datasets/ds_utils.py
--rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc7/pinecone_datasets/fs.py
--rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc7/pinecone_datasets/public.py
--rw-r--r--   0        0        0      227 2023-06-10 19:50:50.277429 pinecone_datasets-0.5.0rc7/pinecone_datasets/testing.py
--rw-r--r--   0        0        0      832 2023-06-15 08:51:46.177765 pinecone_datasets-0.5.0rc7/pyproject.toml
--rw-r--r--   0        0        0    10090 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc7/setup.py
--rw-r--r--   0        0        0     9909 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc7/PKG-INFO
+-rw-r--r--   0        0        0     8945 2023-06-10 20:04:06.109588 pinecone_datasets-0.5.0rc8/README.md
+-rw-r--r--   0        0        0      263 2023-06-22 11:27:52.743731 pinecone_datasets-0.5.0rc8/pinecone_datasets/__init__.py
+-rw-r--r--   0        0        0     3088 2023-06-01 03:29:23.061670 pinecone_datasets-0.5.0rc8/pinecone_datasets/catalog.py
+-rw-r--r--   0        0        0     1185 2023-06-12 13:33:01.718779 pinecone_datasets-0.5.0rc8/pinecone_datasets/cfg.py
+-rw-r--r--   0        0        0    21160 2023-06-22 11:17:50.597209 pinecone_datasets-0.5.0rc8/pinecone_datasets/dataset.py
+-rw-r--r--   0        0        0     1765 2023-06-10 19:50:50.284354 pinecone_datasets-0.5.0rc8/pinecone_datasets/ds_utils.py
+-rw-r--r--   0        0        0      969 2023-06-09 17:14:09.503269 pinecone_datasets-0.5.0rc8/pinecone_datasets/fs.py
+-rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.0rc8/pinecone_datasets/public.py
+-rw-r--r--   0        0        0      227 2023-06-10 19:50:50.277429 pinecone_datasets-0.5.0rc8/pinecone_datasets/testing.py
+-rw-r--r--   0        0        0      915 2023-06-22 11:27:48.939559 pinecone_datasets-0.5.0rc8/pyproject.toml
+-rw-r--r--   0        0        0     9956 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.0rc8/PKG-INFO
```

### Comparing `pinecone_datasets-0.5.0rc7/README.md` & `pinecone_datasets-0.5.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc7/pinecone_datasets/catalog.py` & `pinecone_datasets-0.5.0rc8/pinecone_datasets/catalog.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc7/pinecone_datasets/cfg.py` & `pinecone_datasets-0.5.0rc8/pinecone_datasets/cfg.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc7/pinecone_datasets/dataset.py` & `pinecone_datasets-0.5.0rc8/pinecone_datasets/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,30 +4,40 @@
 import itertools
 import time
 import json
 import asyncio
 import warnings
 from urllib.parse import urlparse
 from dataclasses import dataclass
-from functools import cached_property
-from typing import Any, Generator, Iterator, List, Union, Dict, Optional, Tuple
+from importlib.metadata import version
 
 import gcsfs
 import s3fs
-from pydantic import ValidationError
 import pandas as pd
-import pyarrow.parquet as pq
 from tqdm.auto import tqdm
-
-from pinecone import Client, Index, PineconeOpError
+import pyarrow.parquet as pq
+from pydantic import ValidationError
+from typing import Any, Generator, Iterator, List, Union, Dict, Optional, Tuple
 
 from pinecone_datasets import cfg
 from pinecone_datasets.catalog import DatasetMetadata
 from pinecone_datasets.fs import get_cloud_fs, LocalFileSystem
 
+if version("pinecone-client").startswith("3"):
+    from pinecone import Client as pc, Index
+elif version("pinecone-client").startswith("2"):
+    import pinecone as pc
+    from pinecone import GRPCIndex as Index
+else:
+    warnings.warn(
+        message="Pinecone client version not supported or non-existent,"
+        + "please use pip ineall pinecone-client to install v2 or "
+        + "pip install pinecone-datasets[clientv3] to install v3"
+    )
+
 
 @dataclass
 class UpsertResponse:
     upserted_count: int
 
 
 def iter_pandas_dataframe_slices(
@@ -103,21 +113,21 @@
         Keyword Args:
             kwargs (Dict): additional arguments to pass to the fsspec constructor
 
         Returns:
             Dataset: a Dataset object
         """
         clazz = Dataset(dataset_path=os.getcwd(), **kwargs)
-        clazz.documents = cls._read_pandas_dataframe(
+        clazz._documents = cls._read_pandas_dataframe(
             documents, documents_column_mapping, cfg.Schema.Names.documents
         )
-        clazz.queries = cls._read_pandas_dataframe(
+        clazz._queries = cls._read_pandas_dataframe(
             queries, queries_column_mapping, cfg.Schema.Names.queries
         )
-        clazz.metadata = metadata
+        clazz._metadata = metadata
         return clazz
 
     @staticmethod
     def _read_pandas_dataframe(
         df: pd.DataFrame,
         column_mapping: Dict[str, str],
         schema: List[Tuple[str, bool, Any]],
@@ -175,14 +185,17 @@
 
         """
         self._config = cfg
         endpoint = urlparse(dataset_path)._replace(path="").geturl()
         self._fs = get_cloud_fs(endpoint, **kwargs)
         self._dataset_path = dataset_path
         self._pinecone_client = None
+        self._documents = None
+        self._queries = None
+        self._metadata = None
 
         if not self._fs.exists(self._dataset_path):
             raise FileNotFoundError(
                 "Dataset does not exist. Please check the path or dataset_id"
             )
 
     def _is_datatype_exists(self, data_type: str) -> bool:
@@ -248,17 +261,19 @@
             return getattr(self, key)
         else:
             raise KeyError("Dataset does not have key: {}".format(key))
 
     def __len__(self) -> int:
         return self.documents.shape[0]
 
-    @cached_property
+    @property
     def documents(self) -> pd.DataFrame:
-        return self._safe_read_from_path("documents")
+        if self._documents is None:
+            self._documents = self._safe_read_from_path("documents")
+        return self._documents
 
     def iter_documents(self, batch_size: int = 1) -> Iterator[List[Dict[str, Any]]]:
         """
         Iterates over the documents in the dataset.
 
         Args:
             batch_size (int, optional): The batch size to use for the iterator. Defaults to 1.
@@ -276,17 +291,19 @@
                     axis=1, how="all"
                 ),
                 batch_size,
             )
         else:
             raise ValueError("batch_size must be greater than 0")
 
-    @cached_property
+    @property
     def queries(self) -> pd.DataFrame:
-        return self._safe_read_from_path("queries")
+        if self._queries is None:
+            self._queries = self._safe_read_from_path("queries")
+        return self._queries
 
     def iter_queries(self) -> Iterator[Dict[str, Any]]:
         """
         Iterates over the queries in the dataset.
 
         Returns:
             Iterator[Dict[str, Any]]: An iterator over the queries in the dataset.
@@ -296,17 +313,19 @@
                 results = index.query(**query)
                 # do something with the results
         """
         return iter_pandas_dataframe_single(
             self.queries[self._config.Schema.queries_select_columns]
         )
 
-    @cached_property
+    @property
     def metadata(self) -> DatasetMetadata:
-        return self._load_metadata()
+        if not self._metadata:
+            self._metadata = self._load_metadata()
+        return self._metadata
 
     def head(self, n: int = 5) -> pd.DataFrame:
         return self.documents.head(n)
 
     def to_path(self, dataset_path: str, **kwargs):
         """
         Saves the dataset to a local or cloud storage path.
@@ -357,33 +376,35 @@
             if catalog_base_path
             else os.environ.get("DATASETS_CATALOG_BASEPATH", cfg.Storage.endpoint)
         )
         dataset_path = os.path.join(catalog_base_path, f"{dataset_id}")
         self.to_path(dataset_path, **kwargs)
 
     async def _async_upsert(self, index_name: str, batch_size: int, concurrency: int):
-        index = self._pinecone_client.get_index(index_name=index_name)
+        index = (
+            self._pinecone_client.get_index(index_name=index_name)
+            if version("pinecone-client").startswith("3")
+            else Index(index_name=index_name)
+        )
 
         sem = asyncio.Semaphore(concurrency)
 
         pinecone_failed_batches: Dict[Int, Any] = {}
 
         async def send_batch(batch, i):
             async with sem:
                 try:
                     return await index.upsert(vectors=batch, async_req=True)
-                except PineconeOpError as pe:
+                except Exception as pe:
                     if i in pinecone_failed_batches:
-                        raise PineconeOpError("Uploading batch failed twice")
+                        raise pe
                     else:
                         pinecone_failed_batches[i] = batch
                         print(f"failed batches: {pinecone_failed_batches.keys()}")
                         return UpsertResponse(upserted_count=0)
-                except Exception as e:
-                    raise e
 
         tasks = [
             send_batch(chunk, i)
             for i, chunk in enumerate(self.iter_documents(batch_size=batch_size))
         ]
         failed_tasks_pinecone = []
 
@@ -420,34 +441,41 @@
 
         if not (api_key and environment):
             raise ValueError(
                 "Please set PINECONE_API_KEY and PINECONE_ENVIRONMENT environment variables, \
                 or pass them as arguments to the function"
             )
         # create client
-        self._pinecone_client = Client(api_key=api_key, region=environment)
+
+        if version("pinecone-client").startswith("3"):
+            self._pinecone_client = pc(api_key=api_key, region=environment)
+        elif version("pinecone-client").startswith("2"):
+            pc.init(api_key=api_key, environment=environment)
+            self._pinecone_client = pc
 
         pinecone_index_list = self._pinecone_client.list_indexes()
 
         if index_name in pinecone_index_list:
             raise ValueError(
                 f"index {index_name} already exists, Pinecone Datasets can only be upserted to a new indexe"
             )
         else:
             # create index
             print("creating index")
-            self._pinecone_client.create_index(
-                name=index_name, dimension=self.metadata.dense_model.dimension, **kwargs
-            )
-            print("index created")
-
-        current_status = self._pinecone_client.describe_index(name=index_name).status
-        if current_status == "Ready":
-            return True
-        return False
+            try:
+                self._pinecone_client.create_index(
+                    name=index_name,
+                    dimension=self.metadata.dense_model.dimension,
+                    **kwargs,
+                )
+                print("index created")
+                return True
+            except Exception as e:
+                print(f"error creating index: {e}")
+                return False
 
     def to_pinecone_index(
         self,
         index_name: str,
         batch_size: int = 100,
         concurrency: int = 10,
         api_key: Optional[str] = None,
@@ -496,15 +524,14 @@
         cor = self._async_upsert(
             index_name=index_name,
             batch_size=batch_size,
             concurrency=concurrency,
         )
         return asyncio.run(cor)
 
-
     async def to_pinecone_index_async(
         self,
         index_name: str,
         batch_size: int = 100,
         concurrency: int = 10,
         api_key: Optional[str] = None,
         environment: Optional[str] = None,
```

### Comparing `pinecone_datasets-0.5.0rc7/pinecone_datasets/ds_utils.py` & `pinecone_datasets-0.5.0rc8/pinecone_datasets/ds_utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc7/pinecone_datasets/fs.py` & `pinecone_datasets-0.5.0rc8/pinecone_datasets/fs.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc7/pinecone_datasets/public.py` & `pinecone_datasets-0.5.0rc8/pinecone_datasets/public.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.0rc7/pyproject.toml` & `pinecone_datasets-0.5.0rc8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinecone-datasets"
-version = "0.5.0-rc.7"
+version = "0.5.0-rc.8"
 description = "Pinecone Datasets lets you easily load datasets into your Pinecone index."
 authors = ["Pinecone"]
 maintainers = [
     "Roy Miara <miararoy@gmail.com>",
 ]
 readme = "README.md"
 
@@ -15,17 +15,19 @@
 pyarrow = "^12.0.0"
 fsspec = "^2023.1.0"
 gcsfs = "^2023.1.0"
 s3fs = "^2023.1.0"
 pydantic = "^1.10.5"
 protobuf = ">=3.19.3,<3.20.0"
 pandas = "^2.0.0"
-pinecone-client = "3.0.0rc2"
 tqdm = "^4.65.0"
+pinecone-client = { version = "3.0.0rc2", optional = true }
 
+[tool.poetry.extras]
+clientv3 = ["pinecone-client"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.21.1"
 black = "^23.1.0"
```

### Comparing `pinecone_datasets-0.5.0rc7/setup.py` & `pinecone_datasets-0.5.0rc8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,230 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pinecone-datasets
+Version: 0.5.0rc8
+Summary: Pinecone Datasets lets you easily load datasets into your Pinecone index.
+Author: Pinecone
+Maintainer: Roy Miara
+Maintainer-email: miararoy@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: clientv3
+Requires-Dist: fsspec (>=2023.1.0,<2024.0.0)
+Requires-Dist: gcsfs (>=2023.1.0,<2024.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pinecone-client (==3.0.0rc2) ; extra == "clientv3"
+Requires-Dist: polars (>=0.16.4,<0.17.0)
+Requires-Dist: protobuf (>=3.19.3,<3.20.0)
+Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: s3fs (>=2023.1.0,<2024.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['pinecone_datasets']
+# Pinecone Datasets
 
-package_data = \
-{'': ['*']}
+## install
 
-install_requires = \
-['fsspec>=2023.1.0,<2024.0.0',
- 'gcsfs>=2023.1.0,<2024.0.0',
- 'pandas>=2.0.0,<3.0.0',
- 'pinecone-client==3.0.0rc2',
- 'polars>=0.16.4,<0.17.0',
- 'protobuf>=3.19.3,<3.20.0',
- 'pyarrow>=12.0.0,<13.0.0',
- 'pydantic>=1.10.5,<2.0.0',
- 's3fs>=2023.1.0,<2024.0.0',
- 'tqdm>=4.65.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'pinecone-datasets',
-    'version': '0.5.0rc7',
-    'description': 'Pinecone Datasets lets you easily load datasets into your Pinecone index.',
-    'long_description': '# Pinecone Datasets\n\n## install\n\n```bash\npip install pinecone-datasets\n```\n\n##  Usage - Loading\n\nYou can use Pinecone Datasets to load our public datasets or with your own datasets. Datasets library can be used in 2 main ways: ad-hoc loading of datasets from a path or as a catalog loader for datasets. \n\n### Loading Pinecone Public Datasets (catalog)\n\nPinecone hosts a public datasets catalog, you can load a dataset by name using `list_datasets` and `load_dataset` functions. This will use the default catalog endpoint (currently GCS) to list and load datasets.\n\n```python\nfrom pinecone_datasets import list_datasets, load_dataset\n\nlist_datasets()\n# ["quora_all-MiniLM-L6-bm25", ... ]\n\ndataset = load_dataset("quora_all-MiniLM-L6-bm25")\n\ndataset.head()\n\n# Prints\n# ┌─────┬───────────────────────────┬─────────────────────────────────────┬───────────────────┬──────┐\n# │ id  ┆ values                    ┆ sparse_values                       ┆ metadata          ┆ blob │\n# │     ┆                           ┆                                     ┆                   ┆      │\n# │ str ┆ list[f32]                 ┆ struct[2]                           ┆ struct[3]         ┆      │\n# ╞═════╪═══════════════════════════╪═════════════════════════════════════╪═══════════════════╪══════╡\n# │ 0   ┆ [0.118014, -0.069717, ... ┆ {[470065541, 52922727, ... 22364... ┆ {2017,12,"other"} ┆ .... │\n# │     ┆ 0.0060...                 ┆                                     ┆                   ┆      │\n# └─────┴───────────────────────────┴─────────────────────────────────────┴───────────────────┴──────┘\n```\n\n### Expected dataset structure\n\npinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)\n\n we expect data to be uploaded to the following directory structure:\n\n    ├── my-subdir                     # path to where all datasets\n    │   ├── my-dataset                # name of dataset\n    │   │   ├── metadata.json         # dataset metadata (optional, only for listed)\n    │   │   ├── documents             # datasets documents\n    │   │   │   ├── file1.parquet      \n    │   │   │   └── file2.parquet      \n    │   │   ├── queries               # dataset queries\n    │   │   │   ├── file1.parquet  \n    │   │   │   └── file2.parquet   \n    └── ...\n\nThe data schema is expected to be as follows:\n\n- `documents` directory contains parquet files with the following schema:\n    - Mandatory: `id: str, values: list[float]`\n    - Optional: `sparse_values: Dict: indices: List[int], values: List[float]`, `metadata: Dict`, `blob: dict`\n        - note: blob is a dict that can contain any data, it is not returned when iterating over the dataset and is inteded to be used for storing additional data that is not part of the dataset schema. however, it is sometime useful to store additional data in the dataset, for example, a document text. In future version this may become a first class citizen in the dataset schema.\n- `queries` directory contains parquet files with the following schema:\n    - Mandatory: `vector: list[float], top_k: int`\n    - Optional: `sparse_vector: Dict: indices: List[int], values: List[float]`, `filter: Dict`\n        - note: filter is a dict that contain pinecone filters, for more information see [here](https://docs.pinecone.io/docs/metadata-filtering)\n\nin addition, a metadata file is expected to be in the dataset directory, for example: `s3://my-bucket/my-dataset/metadata.json`\n\n```python\nfrom pinecone_datasets.catalog import DatasetMetadata\n\nmeta = DatasetMetadata(\n    name="test_dataset",\n    created_at="2023-02-17 14:17:01.481785",\n    documents=2,\n    queries=2,\n    source="manual",\n    bucket="LOCAL",\n    task="unittests",\n    dense_model={"name": "bert", "dimension": 3},\n    sparse_model={"name": "bm25"},\n)\n```\n\nfull metadata schema can be found in `pinecone_datasets.catalog.DatasetMetadata.schema`\n\n### Loading your own dataset from catalog\n\nTo set you own catalog endpoint, set the environment variable `DATASETS_CATALOG_BASEPATH` to your bucket. Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).\n\n```bash\nexport DATASETS_CATALOG_BASEPATH="s3://my-bucket/my-subdir"\n```\n\n```python\nfrom pinecone_datasets import list_datasets, load_dataset\n\nlist_datasets()\n\n# ["my-dataset", ... ]\n\ndataset = load_dataset("my-dataset")\n```\n\n### Loading your own dataset from path\n\nYou can load your own dataset from a local path or a remote path (GCS or S3). Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).\n\n```python\nfrom pinecone_datasets import Dataset\n\ndataset = Dataset("s3://my-bucket/my-subdir/my-dataset")\n```\n\n### Loading from a pandas dataframe\n\nPinecone Datasets enables you to load a dataset from a pandas dataframe. This is useful for loading a dataset from a local file and saving it to a remote storage.\nThe minimal required data is a documents dataset, and the minimal required columns are `id` and `values`. The `id` column is a unique identifier for the document, and the `values` column is a list of floats representing the document vector.\n\n```python\nimport pandas as pd\n\ndf = pd.read_parquet("my-dataset.parquet")\n\ndataset = Dataset.from_pandas(df)\n```\n\nPlease check the documentation for more information on the expected dataframe schema. There\'s also a column mapping variable that can be used to map the dataframe columns to the expected schema.\n\n\n## Usage - Accessing data\n\nPinecone Datasets is build on top of pandas. This means that you can use all the pandas API to access the data. In addition, we provide some helper functions to access the data in a more convenient way. \n\n### Accessing documents and queries dataframes\n\naccessing the documents and queries dataframes is done using the `documents` and `queries` properties. These properties are lazy and will only load the data when accessed. \n\n```python\ndocument_df: pd.DataFrame = dataset.documents\n\nquery_df: pd.DataFrame = dataset.queries\n```\n\n\n## Usage - Iterating\n\nOne of the main use cases for Pinecone Datasets is iterating over a dataset. This is useful for upserting a dataset to an index, or for benchmarking. It is also useful for iterating over large datasets - as of today, datasets are not yet lazy, however we are working on it.\n\n\n```python\n\n# List Iterator, where every list of size N Dicts with ("id", "values", "sparse_values", "metadata")\ndataset.iter_documents(batch_size=n) \n\n# Dict Iterator, where every dict has ("vector", "sparse_vector", "filter", "top_k")\ndataset.iter_queries()\n\n```\n\n### The \'blob\' column\n\nPinecone dataset ship with a blob column which is inteneded to be used for storing additional data that is not part of the dataset schema. however, it is sometime useful to store additional data in the dataset, for example, a document text. We added a utility function to move data from the blob column to the metadata column. This is useful for example when upserting a dataset to an index and want to use the metadata to store text data.\n\n```python\nfrom pinecone_datasets import import_documents_keys_from_blob_to_metadata\n\nnew_dataset = import_documents_keys_from_blob_to_metadata(dataset, keys=["text"])\n```\n\n\n### upserting to Index\n\nWhen upserting a Dataset to an Index, only the document data will be upserted to the index. The queries data will be ignored. \n\n```python\nds = load_dataset("dataset_name")\n\n# If index exists\nds.to_index("index_name")\n\n# If index does not exist use create_index=True, this will create the index with the default pinecone settings and dimension from the dataset metadata.\nds.to_index("index_name", create_index=True)\n\n```\n\nthe `to_index` function also accepts additional parameters\n\n* `batch_size` and `concurrency` - for controlling the upserting process\n* `kwargs` - for passing additional parameters to the index creation process\n\n\n## For developers\n\nThis project is using poetry for dependency managemet. supported python version are 3.8+. To start developing, on project root directory run:\n\n```bash\npoetry install --with dev\n```\n\nTo run test locally run \n\n```bash\npoetry run pytest --cov pinecone_datasets\n```',
-    'author': 'Pinecone',
-    'author_email': 'None',
-    'maintainer': 'Roy Miara',
-    'maintainer_email': 'miararoy@gmail.com',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+```bash
+pip install pinecone-datasets
+```
 
+##  Usage - Loading
 
-setup(**setup_kwargs)
+You can use Pinecone Datasets to load our public datasets or with your own datasets. Datasets library can be used in 2 main ways: ad-hoc loading of datasets from a path or as a catalog loader for datasets. 
+
+### Loading Pinecone Public Datasets (catalog)
+
+Pinecone hosts a public datasets catalog, you can load a dataset by name using `list_datasets` and `load_dataset` functions. This will use the default catalog endpoint (currently GCS) to list and load datasets.
+
+```python
+from pinecone_datasets import list_datasets, load_dataset
+
+list_datasets()
+# ["quora_all-MiniLM-L6-bm25", ... ]
+
+dataset = load_dataset("quora_all-MiniLM-L6-bm25")
+
+dataset.head()
+
+# Prints
+# ┌─────┬───────────────────────────┬─────────────────────────────────────┬───────────────────┬──────┐
+# │ id  ┆ values                    ┆ sparse_values                       ┆ metadata          ┆ blob │
+# │     ┆                           ┆                                     ┆                   ┆      │
+# │ str ┆ list[f32]                 ┆ struct[2]                           ┆ struct[3]         ┆      │
+# ╞═════╪═══════════════════════════╪═════════════════════════════════════╪═══════════════════╪══════╡
+# │ 0   ┆ [0.118014, -0.069717, ... ┆ {[470065541, 52922727, ... 22364... ┆ {2017,12,"other"} ┆ .... │
+# │     ┆ 0.0060...                 ┆                                     ┆                   ┆      │
+# └─────┴───────────────────────────┴─────────────────────────────────────┴───────────────────┴──────┘
+```
+
+### Expected dataset structure
+
+pinecone datasets can load dataset from every storage where it has access (using the default access: s3, gcs or local permissions)
+
+ we expect data to be uploaded to the following directory structure:
+
+    ├── my-subdir                     # path to where all datasets
+    │   ├── my-dataset                # name of dataset
+    │   │   ├── metadata.json         # dataset metadata (optional, only for listed)
+    │   │   ├── documents             # datasets documents
+    │   │   │   ├── file1.parquet      
+    │   │   │   └── file2.parquet      
+    │   │   ├── queries               # dataset queries
+    │   │   │   ├── file1.parquet  
+    │   │   │   └── file2.parquet   
+    └── ...
+
+The data schema is expected to be as follows:
+
+- `documents` directory contains parquet files with the following schema:
+    - Mandatory: `id: str, values: list[float]`
+    - Optional: `sparse_values: Dict: indices: List[int], values: List[float]`, `metadata: Dict`, `blob: dict`
+        - note: blob is a dict that can contain any data, it is not returned when iterating over the dataset and is inteded to be used for storing additional data that is not part of the dataset schema. however, it is sometime useful to store additional data in the dataset, for example, a document text. In future version this may become a first class citizen in the dataset schema.
+- `queries` directory contains parquet files with the following schema:
+    - Mandatory: `vector: list[float], top_k: int`
+    - Optional: `sparse_vector: Dict: indices: List[int], values: List[float]`, `filter: Dict`
+        - note: filter is a dict that contain pinecone filters, for more information see [here](https://docs.pinecone.io/docs/metadata-filtering)
+
+in addition, a metadata file is expected to be in the dataset directory, for example: `s3://my-bucket/my-dataset/metadata.json`
+
+```python
+from pinecone_datasets.catalog import DatasetMetadata
+
+meta = DatasetMetadata(
+    name="test_dataset",
+    created_at="2023-02-17 14:17:01.481785",
+    documents=2,
+    queries=2,
+    source="manual",
+    bucket="LOCAL",
+    task="unittests",
+    dense_model={"name": "bert", "dimension": 3},
+    sparse_model={"name": "bm25"},
+)
+```
+
+full metadata schema can be found in `pinecone_datasets.catalog.DatasetMetadata.schema`
+
+### Loading your own dataset from catalog
+
+To set you own catalog endpoint, set the environment variable `DATASETS_CATALOG_BASEPATH` to your bucket. Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).
+
+```bash
+export DATASETS_CATALOG_BASEPATH="s3://my-bucket/my-subdir"
+```
+
+```python
+from pinecone_datasets import list_datasets, load_dataset
+
+list_datasets()
+
+# ["my-dataset", ... ]
+
+dataset = load_dataset("my-dataset")
+```
+
+### Loading your own dataset from path
+
+You can load your own dataset from a local path or a remote path (GCS or S3). Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).
+
+```python
+from pinecone_datasets import Dataset
+
+dataset = Dataset("s3://my-bucket/my-subdir/my-dataset")
+```
+
+### Loading from a pandas dataframe
+
+Pinecone Datasets enables you to load a dataset from a pandas dataframe. This is useful for loading a dataset from a local file and saving it to a remote storage.
+The minimal required data is a documents dataset, and the minimal required columns are `id` and `values`. The `id` column is a unique identifier for the document, and the `values` column is a list of floats representing the document vector.
+
+```python
+import pandas as pd
+
+df = pd.read_parquet("my-dataset.parquet")
+
+dataset = Dataset.from_pandas(df)
+```
+
+Please check the documentation for more information on the expected dataframe schema. There's also a column mapping variable that can be used to map the dataframe columns to the expected schema.
+
+
+## Usage - Accessing data
+
+Pinecone Datasets is build on top of pandas. This means that you can use all the pandas API to access the data. In addition, we provide some helper functions to access the data in a more convenient way. 
+
+### Accessing documents and queries dataframes
+
+accessing the documents and queries dataframes is done using the `documents` and `queries` properties. These properties are lazy and will only load the data when accessed. 
+
+```python
+document_df: pd.DataFrame = dataset.documents
+
+query_df: pd.DataFrame = dataset.queries
+```
+
+
+## Usage - Iterating
+
+One of the main use cases for Pinecone Datasets is iterating over a dataset. This is useful for upserting a dataset to an index, or for benchmarking. It is also useful for iterating over large datasets - as of today, datasets are not yet lazy, however we are working on it.
+
+
+```python
+
+# List Iterator, where every list of size N Dicts with ("id", "values", "sparse_values", "metadata")
+dataset.iter_documents(batch_size=n) 
+
+# Dict Iterator, where every dict has ("vector", "sparse_vector", "filter", "top_k")
+dataset.iter_queries()
+
+```
+
+### The 'blob' column
+
+Pinecone dataset ship with a blob column which is inteneded to be used for storing additional data that is not part of the dataset schema. however, it is sometime useful to store additional data in the dataset, for example, a document text. We added a utility function to move data from the blob column to the metadata column. This is useful for example when upserting a dataset to an index and want to use the metadata to store text data.
+
+```python
+from pinecone_datasets import import_documents_keys_from_blob_to_metadata
+
+new_dataset = import_documents_keys_from_blob_to_metadata(dataset, keys=["text"])
+```
+
+
+### upserting to Index
+
+When upserting a Dataset to an Index, only the document data will be upserted to the index. The queries data will be ignored. 
+
+```python
+ds = load_dataset("dataset_name")
+
+# If index exists
+ds.to_index("index_name")
+
+# If index does not exist use create_index=True, this will create the index with the default pinecone settings and dimension from the dataset metadata.
+ds.to_index("index_name", create_index=True)
+
+```
+
+the `to_index` function also accepts additional parameters
+
+* `batch_size` and `concurrency` - for controlling the upserting process
+* `kwargs` - for passing additional parameters to the index creation process
+
+
+## For developers
+
+This project is using poetry for dependency managemet. supported python version are 3.8+. To start developing, on project root directory run:
+
+```bash
+poetry install --with dev
+```
+
+To run test locally run 
+
+```bash
+poetry run pytest --cov pinecone_datasets
+```
```

