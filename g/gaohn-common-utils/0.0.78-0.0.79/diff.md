# Comparing `tmp/gaohn-common-utils-0.0.78.tar.gz` & `tmp/gaohn-common-utils-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.78.tar", last modified: Thu Jun 22 09:03:11 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.79.tar", last modified: Thu Jun 22 09:08:49 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.78.tar` & `gaohn-common-utils-0.0.79.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.873240 gaohn-common-utils-0.0.78/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.873240 gaohn-common-utils-0.0.78/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.873240 gaohn-common-utils-0.0.78/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.873240 gaohn-common-utils-0.0.78/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.873240 gaohn-common-utils-0.0.78/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/core/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/common_utils/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/core/decorators/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/core/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.873240 gaohn-common-utils-0.0.78/common_utils/experiment_tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/common_utils/experiment_tracking/promoter/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/experiment_tracking/promoter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/experiment_tracking/promoter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.873240 gaohn-common-utils-0.0.78/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-22 09:03:11.000000 gaohn-common-utils-0.0.78/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 09:03:11.000000 gaohn-common-utils-0.0.78/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:03:11.000000 gaohn-common-utils-0.0.78/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-22 09:03:11.000000 gaohn-common-utils-0.0.78/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 09:03:11.000000 gaohn-common-utils-0.0.78/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-22 09:02:36.000000 gaohn-common-utils-0.0.78/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:03:11.877240 gaohn-common-utils-0.0.78/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.648123 gaohn-common-utils-0.0.79/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.648123 gaohn-common-utils-0.0.79/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.648123 gaohn-common-utils-0.0.79/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.648123 gaohn-common-utils-0.0.79/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.648123 gaohn-common-utils-0.0.79/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/core/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/common_utils/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/core/decorators/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/core/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.648123 gaohn-common-utils-0.0.79/common_utils/experiment_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/common_utils/experiment_tracking/promoter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/experiment_tracking/promoter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/experiment_tracking/promoter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.648123 gaohn-common-utils-0.0.79/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-22 09:08:49.000000 gaohn-common-utils-0.0.79/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 09:08:49.000000 gaohn-common-utils-0.0.79/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:08:49.000000 gaohn-common-utils-0.0.79/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-22 09:08:49.000000 gaohn-common-utils-0.0.79/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 09:08:49.000000 gaohn-common-utils-0.0.79/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-22 09:08:32.000000 gaohn-common-utils-0.0.79/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:08:49.652123 gaohn-common-utils-0.0.79/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.78/LICENSE` & `gaohn-common-utils-0.0.79/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/PKG-INFO` & `gaohn-common-utils-0.0.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.78
+Version: 0.0.79
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.78/README.md` & `gaohn-common-utils-0.0.79/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.79/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.79/common_utils/cloud/gcp/database/bigquery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-import logging
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 import pandas as pd
 from google.cloud import bigquery
 from google.cloud.exceptions import NotFound
-from rich.logging import RichHandler
 
 from common_utils.cloud.base import GCPConnector
+from common_utils.core.logger import Logger
 
 # Setup logging
-logging.basicConfig(
-    level="INFO",
-    format="%(asctime)s [%(levelname)s]: %(message)s",
-    datefmt="%Y-%m-%d %H:%M:%S",
-    handlers=[RichHandler()],
-)
+# logging.basicConfig(
+#     level="INFO",
+#     format="%(asctime)s [%(levelname)s]: %(message)s",
+#     datefmt="%Y-%m-%d %H:%M:%S",
+#     handlers=[RichHandler()],
+# )
 
-logger = logging.getLogger("rich")
+# logger = logging.getLogger("rich")
+
+
+# Setup logging
+logger = Logger(
+    module_name=__name__, propagate=False, log_root_dir=None, log_file=None
+).logger
 
 
 @dataclass
 class BigQuery(GCPConnector):
     # usually you call project_id.dataset_id.table_name
     dataset: str  # The ID of the dataset to use.
     table_name: str  # The name of the table to use.
```

### Comparing `gaohn-common-utils-0.0.78/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.79/common_utils/cloud/gcp/storage/gcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-import logging
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Dict, List, Literal
 
 from google.cloud import storage
 from google.cloud.exceptions import NotFound
-from rich.logging import RichHandler
 
 from common_utils.cloud.base import GCPConnector
+from common_utils.core.logger import Logger
 
 # Setup logging
-logging.basicConfig(
-    level="INFO",
-    format="%(asctime)s [%(levelname)s]: %(message)s",
-    datefmt="%Y-%m-%d %H:%M:%S",
-    handlers=[RichHandler()],
-)
+# logging.basicConfig(
+#     level="INFO",
+#     format="%(asctime)s [%(levelname)s]: %(message)s",
+#     datefmt="%Y-%m-%d %H:%M:%S",
+#     handlers=[RichHandler()],
+# )
 
-logger = logging.getLogger("rich")
+# logger = logging.getLogger("rich")
+
+
+# Setup logging
+logger = Logger(
+    module_name=__name__, propagate=False, log_root_dir=None, log_file=None
+).logger
 
 
 @dataclass
 class GCS(GCPConnector):
     bucket_name: str
     storage_client: storage.Client = field(init=False, repr=False)
     bucket: storage.Bucket = field(init=False, repr=False)
```

### Comparing `gaohn-common-utils-0.0.78/common_utils/core/base.py` & `gaohn-common-utils-0.0.79/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/core/common.py` & `gaohn-common-utils-0.0.79/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/core/decorators/decorators.py` & `gaohn-common-utils-0.0.79/common_utils/core/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/core/decorators/timer.py` & `gaohn-common-utils-0.0.79/common_utils/core/decorators/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Decorator Functions."""
 import functools
 import time
 from statistics import mean, median, stdev
-from typing import Any, Callable, TypeVar, Dict
+from typing import Any, Callable, Dict, TypeVar
 
 import numpy as np
 from prettytable import PrettyTable
 from rich.pretty import pprint
+
 from common_utils.core.logger import Logger
 
 # Setup logging
 LOGGER = Logger(
     module_name=__name__, propagate=False, log_root_dir=None, log_file=None
 ).logger
```

### Comparing `gaohn-common-utils-0.0.78/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.79/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/core/logger.py` & `gaohn-common-utils-0.0.79/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.79/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/experiment_tracking/promoter/base.py` & `gaohn-common-utils-0.0.79/common_utils/experiment_tracking/promoter/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/experiment_tracking/promoter/core.py` & `gaohn-common-utils-0.0.79/common_utils/experiment_tracking/promoter/core.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from typing import List, Literal, Optional
 
 from mlflow.tracking import MlflowClient
 
 from common_utils.core.logger import Logger
 from common_utils.experiment_tracking.promoter.base import (
-    PromotionManager,
     ModelVersion,
+    PromotionManager,
 )
 
 
 class MLFlowPromotionManager(PromotionManager):
     """A class that manages the promotion of machine learning models to production.
 
     This class adheres to several principles of good software design:
```

### Comparing `gaohn-common-utils-0.0.78/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.79/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.79/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.79/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.78
+Version: 0.0.79
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.78/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.79/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.78/pyproject.toml` & `gaohn-common-utils-0.0.79/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.78"
+version = "0.0.79"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

