# Comparing `tmp/enfobench-0.1.0.tar.gz` & `tmp/enfobench-0.1.1.tar.gz`

## Comparing `enfobench-0.1.0.tar` & `enfobench-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 enfobench-0.1.0/Makefile
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 enfobench-0.1.0/README.md
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 enfobench-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/__version__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/py.typed
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/utils.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/__init__.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/_cross_validate.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/_evaluate.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/client.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/metrics.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/protocols.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enfobench-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enfobench-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 enfobench-0.1.0/tests/test_metrics.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 enfobench-0.1.0/.gitignore
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 enfobench-0.1.0/LICENCE
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 enfobench-0.1.0/README.md
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 enfobench-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 enfobench-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 enfobench-0.1.1/Makefile
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 enfobench-0.1.1/README.md
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 enfobench-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/__version__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/py.typed
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/utils.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/evaluation/__init__.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/evaluation/_cross_validate.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/evaluation/_evaluate.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/evaluation/client.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/evaluation/metrics.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/evaluation/protocols.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 enfobench-0.1.1/src/enfobench/evaluation/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enfobench-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enfobench-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 enfobench-0.1.1/tests/test_metrics.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 enfobench-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 enfobench-0.1.1/LICENCE
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 enfobench-0.1.1/README.md
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 enfobench-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 enfobench-0.1.1/PKG-INFO
```

### Comparing `enfobench-0.1.0/Makefile` & `enfobench-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `enfobench-0.1.0/pyproject.toml` & `enfobench-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `enfobench-0.1.0/src/enfobench/evaluation/_cross_validate.py` & `enfobench-0.1.1/src/enfobench/evaluation/_cross_validate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Union, List, Optional
+from typing import List, Optional, Union
 
 import pandas as pd
 from tqdm import tqdm
 
-from enfobench.utils import steps_in_horizon
-
 from enfobench.evaluation.client import ForecastClient
 from enfobench.evaluation.protocols import Model
+from enfobench.utils import steps_in_horizon
 
 
 def generate_cutoff_dates(
     start: pd.Timestamp,
     end: pd.Timestamp,
     horizon: pd.Timedelta,
     step: pd.Timedelta,
@@ -39,42 +38,47 @@
         raise ValueError("No dates for cross-validation")
     return cutoff_dates
 
 
 def cross_validate(
     model: Union[Model, ForecastClient],
     start: pd.Timestamp,
+    end: pd.Timestamp,
     horizon: pd.Timedelta,
     step: pd.Timedelta,
     y: pd.Series,
     level: Optional[List[int]] = None,
     freq: Optional[str] = None,
 ) -> pd.DataFrame:
     """Cross-validate a model.
 
     Parameters
     ----------
     model:
         Model to cross-validate.
     start:
         Start date of the time series.
+    end:
+        End date of the time series.
     horizon:
         Forecast horizon.
     step:
         Step size between cutoff dates.
     y:
         Time series target values.
     level:
         Prediction intervals to compute.
         (Optional, if not provided, simple point forecasts will be computed.)
     freq:
         Frequency of the time series.
         (Optional, if not provided, it will be inferred from the time series index.)
     """
-    cutoff_dates = generate_cutoff_dates(start, y.index[-1], horizon, step)
+    if end > y.index[-1]:
+        raise ValueError("End date is beyond the target values.")
+    cutoff_dates = generate_cutoff_dates(start, end, horizon, step)
     horizon_length = steps_in_horizon(horizon, freq or y.index.inferred_freq)
 
     # Cross-validation
     forecasts = []
     for cutoff in tqdm(cutoff_dates):
         # make sure that there is no data leakage
         history = y.loc[y.index <= cutoff]
```

### Comparing `enfobench-0.1.0/src/enfobench/evaluation/_evaluate.py` & `enfobench-0.1.1/src/enfobench/evaluation/_evaluate.py`

 * *Files identical despite different names*

### Comparing `enfobench-0.1.0/src/enfobench/evaluation/client.py` & `enfobench-0.1.1/src/enfobench/evaluation/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import io
-from typing import Dict, Union, Optional, List
+from typing import Dict, List, Optional, Union
 
 import pandas as pd
 import requests
 
 from enfobench.evaluation.protocols import EnvironmentInfo, ModelInfo
 
 
@@ -42,15 +42,15 @@
     ) -> pd.DataFrame:
         params: Dict[str, Union[int, List[int]]] = {
             "horizon": horizon,
         }
         if level is not None:
             params["level"] = level
 
-        y_df = y.rename_axis('ds').reset_index()
+        y_df = y.rename_axis("ds").reset_index()
         files = {
             "y": to_buffer(y_df),
             # "X": to_buffer(X),
         }
 
         response = self.session.post(
             url=f"{self.base_url}/predict",
```

### Comparing `enfobench-0.1.0/src/enfobench/evaluation/metrics.py` & `enfobench-0.1.1/src/enfobench/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `enfobench-0.1.0/src/enfobench/evaluation/protocols.py` & `enfobench-0.1.1/src/enfobench/evaluation/protocols.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Any, Protocol, Optional, List, Dict
+from typing import Any, Dict, List, Optional, Protocol
 
 import pandas as pd
 from pydantic import BaseModel
 
 
 class ForecasterType(str, Enum):
     point = "point"
```

### Comparing `enfobench-0.1.0/src/enfobench/evaluation/server.py` & `enfobench-0.1.1/src/enfobench/evaluation/server.py`

 * *Files identical despite different names*

### Comparing `enfobench-0.1.0/tests/test_metrics.py` & `enfobench-0.1.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `enfobench-0.1.0/.gitignore` & `enfobench-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `enfobench-0.1.0/LICENCE` & `enfobench-0.1.1/LICENCE`

 * *Files identical despite different names*

