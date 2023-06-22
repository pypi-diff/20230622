# Comparing `tmp/configu-0.1.4.tar.gz` & `tmp/configu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configu-0.1.4.tar", max compression
+gzip compressed data, was "configu-0.2.0.tar", max compression
```

## Comparing `configu-0.1.4.tar` & `configu-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      759 2023-04-24 16:42:15.764914 configu-0.1.4/README.md
--rw-r--r--   0        0        0      555 2023-04-24 16:42:15.764914 configu-0.1.4/configu/__init__.py
--rw-r--r--   0        0        0      123 2023-04-24 16:42:15.764914 configu-0.1.4/configu/commands/__init__.py
--rw-r--r--   0        0        0    13948 2023-04-24 16:42:15.764914 configu-0.1.4/configu/commands/eval_command.py
--rw-r--r--   0        0        0     2695 2023-04-24 16:42:15.764914 configu-0.1.4/configu/commands/upsert_command.py
--rw-r--r--   0        0        0      423 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/__init__.py
--rw-r--r--   0        0        0      354 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/command.py
--rw-r--r--   0        0        0     6442 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/config_schema.py
--rw-r--r--   0        0        0     1383 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/config_set.py
--rw-r--r--   0        0        0      457 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/config_store.py
--rw-r--r--   0        0        0    11311 2023-04-24 16:42:45.559380 configu-0.1.4/configu/core/generated.py
--rw-r--r--   0        0        0      187 2023-04-24 16:42:15.764914 configu-0.1.4/configu/stores/__init__.py
--rw-r--r--   0        0        0     2507 2023-04-24 16:42:15.764914 configu-0.1.4/configu/stores/configu_store.py
--rw-r--r--   0        0        0     1320 2023-04-24 16:42:15.764914 configu-0.1.4/configu/stores/in_memory_store.py
--rw-r--r--   0        0        0     2482 2023-04-24 16:42:15.764914 configu-0.1.4/configu/stores/json_file_store.py
--rw-r--r--   0        0        0     1234 2023-04-24 16:42:15.764914 configu-0.1.4/configu/utils.py
--rw-r--r--   0        0        0     1815 2023-04-24 16:43:09.861249 configu-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 configu-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1753 2023-06-22 12:18:20.254169 configu-0.2.0/README.md
+-rw-r--r--   0        0        0      644 2023-06-22 12:18:20.254169 configu-0.2.0/configu/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-22 12:18:20.254169 configu-0.2.0/configu/commands/__init__.py
+-rw-r--r--   0        0        0    11244 2023-06-22 12:18:20.254169 configu-0.2.0/configu/commands/eval_command.py
+-rw-r--r--   0        0        0     1033 2023-06-22 12:18:20.254169 configu-0.2.0/configu/commands/export_command.py
+-rw-r--r--   0        0        0     2496 2023-06-22 12:18:20.254169 configu-0.2.0/configu/commands/upsert_command.py
+-rw-r--r--   0        0        0      423 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/__init__.py
+-rw-r--r--   0        0        0      354 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/command.py
+-rw-r--r--   0        0        0     6446 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/config_schema.py
+-rw-r--r--   0        0        0     1383 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/config_set.py
+-rw-r--r--   0        0        0      457 2023-06-22 12:18:20.254169 configu-0.2.0/configu/core/config_store.py
+-rw-r--r--   0        0        0    11311 2023-06-22 12:18:54.814052 configu-0.2.0/configu/core/generated.py
+-rw-r--r--   0        0        0      223 2023-06-22 12:18:20.254169 configu-0.2.0/configu/stores/__init__.py
+-rw-r--r--   0        0        0     2481 2023-06-22 12:18:20.254169 configu-0.2.0/configu/stores/configu_store.py
+-rw-r--r--   0        0        0     1326 2023-06-22 12:18:20.254169 configu-0.2.0/configu/stores/in_memory_store.py
+-rw-r--r--   0        0        0     2488 2023-06-22 12:18:20.254169 configu-0.2.0/configu/stores/json_file_store.py
+-rw-r--r--   0        0        0     1239 2023-06-22 12:18:20.254169 configu-0.2.0/configu/utils.py
+-rw-r--r--   0        0        0     1815 2023-06-22 12:19:33.917935 configu-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2908 1970-01-01 00:00:00.000000 configu-0.2.0/PKG-INFO
```

### Comparing `configu-0.1.4/configu/commands/upsert_command.py` & `configu-0.2.0/configu/commands/upsert_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,44 @@
-from typing import Dict, Union
-
-from pydantic import BaseModel, Field
+from typing import Dict, TypedDict
 
 from ..core import (
-    ConfigSet,
-    ConfigStore,
-    ConfigSchema,
     CfguType,
-    Config,
     Command,
+    Config,
+    ConfigSchema,
+    ConfigSet,
+    ConfigStore,
 )
-from ..core.command import CommandReturn
 from ..utils import error_message
 
+UpsertCommandParameters = TypedDict(
+    "UpsertCommandParameters",
+    {
+        "store": ConfigStore,
+        "set": ConfigSet,
+        "schema": ConfigSchema,
+        "configs": Dict[str, str],
+    },
+)
 
-class UpsertCommandParameters(BaseModel):
-    """"""
-
-    store: ConfigStore
-    set: ConfigSet
-    schema_: ConfigSchema = Field(alias="schema")
-    configs: Dict[str, str]
 
+class UpsertCommand(Command):
+    """"""
 
-class UpsertCommand(Command[None]):
     parameters: UpsertCommandParameters
 
-    def __init__(
-        self, parameters: Union[UpsertCommandParameters, dict]
-    ) -> None:
-        if isinstance(parameters, dict):
-            parameters = UpsertCommandParameters.parse_obj(parameters)
+    def __init__(self, parameters: UpsertCommandParameters) -> None:
         super().__init__(parameters)
 
-    def run(self) -> CommandReturn:
+    def run(self):
         scope_location = ["UpsertCommand", "run"]
-        store = self.parameters.store
-        set_ = self.parameters.set
-        schema = self.parameters.schema_
-        configs = self.parameters.configs
+        store = self.parameters["store"]
+        set_ = self.parameters["set"]
+        schema = self.parameters["schema"]
+        configs = self.parameters["configs"]
         store.init()
         schema_content = ConfigSchema.parse(schema)
         upset_configs = []
         for key, value in configs.items():
             cfgu = schema_content.get(key)
             if cfgu is None:
                 raise ValueError(
@@ -78,8 +74,7 @@
                         f"invalid config value '{value}' for key '{key}'",
                         scope_location,
                         f"value '{value}' must be of type '{cfgu.type.value}'",
                     )
                 )
             upset_configs.append(Config(set=set_.path, key=key, value=value))
         store.set(upset_configs)
-        return
```

### Comparing `configu-0.1.4/configu/core/config_schema.py` & `configu-0.2.0/configu/core/config_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     _cs_regex = r"^(?:([^:/?#\s]+):/{2})?(?:([^@/?#\s]+)@)?([^/?#\s]+)?(?:/([^?#\s]*))?(?:[?]([^#\s]+))?\S*$"  # noqa: E501
     NAME: str = "cfgu"
     EXT: str = ".cfgu"
     VALIDATORS: Dict[str, Callable[[str], bool]] = {
         "Boolean": pyvalidator.is_boolean,
         "Number": pyvalidator.is_number,
         "String": lambda value: isinstance(value, str),
-        "RegEx": lambda *args: re.fullmatch(args[0], args[1]) is None,
+        "RegEx": lambda *args: re.fullmatch(args[1], args[0]) is not None,
         "UUID": pyvalidator.is_uuid,
         "SemVer": pyvalidator.is_semantic_version,
         "Email": pyvalidator.is_email,
         "MobilePhone": pyvalidator.is_mobile_number,
         "LatLong": pyvalidator.is_lat_long,
         "Color": lambda value: (
             pyvalidator.is_hexadecimal(value)
```

### Comparing `configu-0.1.4/configu/core/config_set.py` & `configu-0.2.0/configu/core/config_set.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.4/configu/core/generated.py` & `configu-0.2.0/configu/core/generated.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.4/configu/stores/configu_store.py` & `configu-0.2.0/configu/stores/configu_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,26 +33,25 @@
         self.token = token
 
     def __call__(self, r):
         r.headers["token"] = self.token
         return r
 
 
-class ConfiguStore(ConfigStore):
+class ConfiguConfigStore(ConfigStore):
     _headers: Dict
     _auth: AuthBase
     _url: str
 
     def __init__(
         self, store_config: Union[ConfiguStoreConfiguration, dict]
     ) -> None:
         super().__init__(type="configu")
         if isinstance(store_config, dict):
             store_config = ConfiguStoreConfiguration.parse_obj(store_config)
-            print(store_config)
         self._headers = {
             "Org": store_config.credentials.org,
             "Source": store_config.source,
         }
         token = store_config.credentials.token
         self._auth = (
             BearerAuth(token)
```

### Comparing `configu-0.1.4/configu/stores/in_memory_store.py` & `configu-0.2.0/configu/stores/in_memory_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Union
 
 from ..core import Config, ConfigStoreQuery, ConfigStore
 from ..core.generated import config_store_query_from_dict, config_from_dict
 
 
-class InMemoryStore(ConfigStore):
+class InMemoryConfigStore(ConfigStore):
     _data: List[Config]
 
     def __init__(self) -> None:
         super().__init__(type="in-memory")
         self._data = []
 
     def get(self, queries: List[ConfigStoreQuery]) -> List[Config]:
```

### Comparing `configu-0.1.4/configu/stores/json_file_store.py` & `configu-0.2.0/configu/stores/json_file_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     config_store_query_from_dict,
     config_store_contents_to_dict,
     ConfigStoreContentsElement,
     config_store_contents_element_from_dict,
 )
 
 
-class JsonFileStore(ConfigStore):
+class JsonFileConfigStore(ConfigStore):
     _path: str
 
     def __init__(self, path: str) -> None:
         super().__init__(type="in-memory")
         self._path = path
 
     def read(self):
```

### Comparing `configu-0.1.4/configu/utils.py` & `configu-0.2.0/configu/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Optional, List, Dict
+from typing import Any, Dict, List, Optional
 
 import chevron
 
 
 def error_message(
     message: str,
     location: Optional[List[str]] = None,
@@ -38,9 +38,9 @@
                 )
             )
         if tag_type == "variable":
             template_vars.append(tag_key)
     return template_vars
 
 
-def render_template(template: str, context: Dict[str, str]) -> str:
+def render_template(template: str, context: Dict[str, Any]) -> str:
     return chevron.render(template, context)
```

### Comparing `configu-0.1.4/pyproject.toml` & `configu-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configu"
-version = "0.1.4"
+version = "0.2.0"
 description = "Configu Python SDK"
 authors = ["Configu <info@configu.com>"]
 maintainers = [
   "Ron Roditi <ron@configu.com>",
   "Or Levi <orlevi128@gmail.com>"
 ]
 license = "Apache-2.0"
```

### Comparing `configu-0.1.4/PKG-INFO` & `configu-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configu
-Version: 0.1.4
+Version: 0.2.0
 Summary: Configu Python SDK
 Home-page: https://configu.com/
 License: Apache-2.0
 Keywords: cfgu,configu,configu-sdk,configu-python-sdk
 Author: Configu
 Author-email: info@configu.com
 Maintainer: Ron Roditi
@@ -26,37 +26,74 @@
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://configu.com/docs/
 Project-URL: Repository, https://github.com/configu/configu
 Description-Content-Type: text/markdown
 
 # @configu/py
 
-> configu python sdk
+Configu SDK for Python
 
 ## Install
 
+To install the this package, simply type install [configu](https://pypi.org/project/configu/) using pip:
+
 ```bash
 pip install configu
 ```
 
 ## Usage
-See example in the examples folder
 
-## CONTRIBUTING
+```py
+import os
+
+import configu
+
+config_store = configu.InMemoryConfigStore()
+test_set = configu.ConfigSet("test")
+schema = configu.ConfigSchema("get-started.cfgu.json")
+
+configu.UpsertCommand({
+    "store": config_store,
+    "set": test_set,
+    "schema": schema,
+    "configs": {
+        'GREETING': 'hey',
+        'SUBJECT': 'configu python sdk'
+    },
+}).run()
+
+data = configu.EvalCommand({
+    "store": config_store,
+    "set": test_set,
+    "schema": schema,
+}).run()
+
+configuration_data = configu.ExportCommand({"data": data}).run()
+
+print(os.environ["MESSAGE"])
+# hey, configu python sdk!
+print(configuration_data)
+# {'GREETING': 'hey', 'SUBJECT': 'configu python sdk', 'MESSAGE': 'hey, configu python sdk!'}
+```
+
+## Reference
+
+See [oss.configu.com/py](https://oss.configu.com/py/configu.html)
+
+## Contributing
 
 ### Requirements
 
-1. Follow the instructions on the main [CONTRIBUTING.md](https://github.com/configu/configu/blob/main/CONTRIBUTING.md)
-   to set up node and npm. This is necessary for lint-staged workflow.
+1. Follow the [Development](https://github.com/configu/configu/blob/main/CONTRIBUTING.md#development) section from the `CONTRIBUTING.md`.
 2. Install [pyenv](https://github.com/pyenv/pyenv) | [Homebrew](https://formulae.brew.sh/formula/pyenv)
 3. Install [poetry](https://python-poetry.org/) | [Homebrew](https://formulae.brew.sh/formula/poetry)
 
 ### Setup
 
-#### Run these commands in order
+Run these commands in order:
 
 ```bash
 cd py
 ```
 
 ```bash
 pyenv install
@@ -70,7 +107,11 @@
 poetry env use $(pyenv which python)
 ```
 
 ```bash
 poetry install
 ```
 
+### Contribute
+
+Follow the [Sending a Pull Request](https://github.com/configu/configu/blob/main/CONTRIBUTING.md#sending-a-pull-request) section from the `CONTRIBUTING.md`.
+
```

