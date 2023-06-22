# Comparing `tmp/lxdx-0.4.2.tar.gz` & `tmp/lxdx-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxdx-0.4.2.tar", max compression
+gzip compressed data, was "lxdx-0.4.3.tar", max compression
```

## Comparing `lxdx-0.4.2.tar` & `lxdx-0.4.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1509 2023-01-28 21:18:09.875849 lxdx-0.4.2/LICENSE
--rw-r--r--   0        0        0     4066 2023-01-28 21:18:09.875849 lxdx-0.4.2/README.rst
--rw-r--r--   0        0        0       44 2023-01-28 21:18:09.875849 lxdx-0.4.2/lxdx/__init__.py
--rw-r--r--   0        0        0    20981 2023-01-28 21:18:09.875849 lxdx-0.4.2/lxdx/dixt.py
--rw-r--r--   0        0        0     1603 2023-01-28 21:18:09.875849 lxdx-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4848 1970-01-01 00:00:00.000000 lxdx-0.4.2/setup.py
--rw-r--r--   0        0        0     5374 1970-01-01 00:00:00.000000 lxdx-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1509 2023-06-22 03:30:43.660877 lxdx-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4066 2023-06-22 03:30:43.660877 lxdx-0.4.3/README.rst
+-rw-r--r--   0        0        0       44 2023-06-22 03:30:43.664877 lxdx-0.4.3/lxdx/__init__.py
+-rw-r--r--   0        0        0    21135 2023-06-22 03:30:43.664877 lxdx-0.4.3/lxdx/dixt.py
+-rw-r--r--   0        0        0     1603 2023-06-22 03:30:43.664877 lxdx-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 lxdx-0.4.3/PKG-INFO
```

### Comparing `lxdx-0.4.2/LICENSE` & `lxdx-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lxdx-0.4.2/README.rst` & `lxdx-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `lxdx-0.4.2/lxdx/dixt.py` & `lxdx-0.4.3/lxdx/dixt.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 """
 
 import json
 import re
 
 from collections import defaultdict
 from collections.abc import KeysView, ItemsView, ValuesView, MutableMapping
+from copy import deepcopy
 from typing import Any, Dict, List, Mapping, Tuple, Union, Hashable
 
 __all__ = ['Dixt']
 
 
 class Dixt(MutableMapping):
     """``Dixt`` is an "extended" Python ``dict``, works just like ``dict``,
@@ -49,15 +50,17 @@
     # supported meta flags
     __metas__ = {'hidden': bool}
 
     # flags and their corresponding 'off' values.
     __meta_resets__ = {'hidden': False}
 
     def __new__(cls, data=None, /, **kwargs):
-        spec = dict(data or {}) | kwargs
+        # use deepcopy 'cause sometimes data can be an iterator,
+        # so it won't be 'used up' before __init__()
+        spec = dict(deepcopy(data) or {}) | kwargs
         dx = super().__new__(cls)
 
         # holds all normalised keys including non-str keys
         dx.__dict__['__keymap__'] = {_normalise_key(key): key
                                      for key in spec.keys()}
         return dx
```

### Comparing `lxdx-0.4.2/pyproject.toml` & `lxdx-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lxdx"
-version = "0.4.2"
+version = "0.4.3"
 authors = ["Hardy Stones <hardistones@hotmail.com>"]
 description = "Just an extended Python dict with attribute-accessibility, extra methods, and metadata"
 homepage = "https://github.com/hardistones/lxdx"
 documentation = "https://hardistones.github.io/lxdx"
 license = "3-Clause BSD License"
 readme = "README.rst"
 classifiers = [
```

### Comparing `lxdx-0.4.2/setup.py` & `lxdx-0.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,139 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: lxdx
+Version: 0.4.3
+Summary: Just an extended Python dict with attribute-accessibility, extra methods, and metadata
+Home-page: https://github.com/hardistones/lxdx
+License: 3-Clause BSD License
+Keywords: dict,extended,normalize,metadata
+Author: Hardy Stones
+Author-email: hardistones@hotmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Project-URL: Bug Tracker, https://github.com/hardistones/lxdx/issues
+Project-URL: Documentation, https://hardistones.github.io/lxdx
+Description-Content-Type: text/x-rst
 
-packages = \
-['lxdx']
+lxdx
+====
 
-package_data = \
-{'': ['*']}
+``lxdx`` is an "extended" Python ``dict`` with attribute-like accessibility.
+Other than the usual ``dict`` operations, functions and methods,
+some useful functions are incorporated as well.
 
-setup_kwargs = {
-    'name': 'lxdx',
-    'version': '0.4.2',
-    'description': 'Just an extended Python dict with attribute-accessibility, extra methods, and metadata',
-    'long_description': 'lxdx\n====\n\n``lxdx`` is an "extended" Python ``dict`` with attribute-like accessibility.\nOther than the usual ``dict`` operations, functions and methods,\nsome useful functions are incorporated as well.\n\nOnly supports Python 3.9+, due to the usage of the `union operator`_ for ``dict``.\n\nWhy this project?\n-----------------\n* Hobbies and curiosities. Just for the fun of programming.\n* ``dataclass`` is not cut for modelling hierarchical data.\n* Brackets when accessing multi-layer data is too many. `Dot notation`_ may be a cleaner way.\n* Introduce utility functions like ``get_from(path)``, inspired from `JsonPath`_, for programmability.\n* Ability to add metadata to the items.\n\nInstallation\n------------\n``lxdx`` is available in `PyPI <https://pypi.org/project/lxdx>`_, and installable via ``pip``:\n\n.. code-block::\n\n    pip install lxdx\n\n\nExamples\n--------\n.. code-block:: python\n\n    from lxdx import Dixt\n\n    assert Dixt() == {}\n    assert Dixt({1: 1, \'alpha\': \'α\'}) == {1: 1, \'alpha\': \'α\'}\n    assert Dixt(alpha=\'α\', beta=\'β\') == {\'alpha\': \'α\', \'beta\': \'β\'}\n    assert Dixt(alpha=\'α\', beta=\'β\').is_supermap_of({\'beta\': \'β\'})\n\n    # data can be deeply nested\n    data = {\'Accept-Encoding\': \'gzip\', \'metadata\': {\'Content-Type\': \'application/json\'}}\n    dx = Dixt(**data)\n\n    # update dx using the union operator\n    dx |= {\'other\': \'dict or Dixt obj\'}\n\n    # \'Normalise\' the keys to use it as attributes additionally.\n    assert dx[\'Accept-Encoding\'] == dx.accept_encoding\n    del dx.accept_encoding\n    print(dx.metadata.CONTENT_TYPE)\n\n    # Instead of\n    dx[\'a-list\'][1][\'obj-attr\'] = \'value\'\n\n    # Is way cleaner\n    dx.a_list[1].obj_attr = \'value\'\n\n    # Programmatically get values\n    assert dx.a_list[1].obj_attr == dx.get_from(\'$.a_list[1].obj_attr\')\n\n    json_str = \'{"a": "JSON string"}\'\n    assert Dixt.from_json(json_str).json() == json_str\n\nDocumentation\n-------------\nFull documentation is at https://hardistones.github.io/lxdx.\n\nFuture\n------\n``lxdx`` is supposed to be a library of "extended" ``list`` and ``dict``. For now there\'s no use case for the ``list`` extension.\n\n**To be supported**\n\n- User-defined meta specification.\n\nLicense\n-------\nThis project and all its files are licensed under the 3-Clause BSD License.\n\n    Copyright (c) 2021, @github.com/hardistones\n    All rights reserved.\n\n    Redistribution and use in source and binary forms, with or without modification,\n    are permitted provided that the following conditions are met:\n\n    1. Redistributions of source code must retain the above copyright notice, this\n       list of conditions and the following disclaimer.\n\n    2. Redistributions in binary form must reproduce the above copyright notice,\n       this list of conditions and the following disclaimer in the documentation\n       and/or other materials provided with the distribution.\n\n    3. Neither the name of the copyright holder nor the names of its contributors\n       may be used to endorse or promote products derived from this software without\n       specific prior written permission.\n\n    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND\n    ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED\n    WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\n    DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR\n    ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES\n    (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;\n    LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON\n    ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT\n    (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS\n    SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n\n\n.. References\n.. _union operator: https://www.python.org/dev/peps/pep-0584\n.. _dot notation: https://en.wikipedia.org/wiki/Property_(programming)#Dot_notation\n.. _JsonPath: https://github.com/json-path/JsonPath\n',
-    'author': 'Hardy Stones',
-    'author_email': 'hardistones@hotmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/hardistones/lxdx',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.9,<4.0',
-}
+Only supports Python 3.9+, due to the usage of the `union operator`_ for ``dict``.
 
+Why this project?
+-----------------
+* Hobbies and curiosities. Just for the fun of programming.
+* ``dataclass`` is not cut for modelling hierarchical data.
+* Brackets when accessing multi-layer data is too many. `Dot notation`_ may be a cleaner way.
+* Introduce utility functions like ``get_from(path)``, inspired from `JsonPath`_, for programmability.
+* Ability to add metadata to the items.
+
+Installation
+------------
+``lxdx`` is available in `PyPI <https://pypi.org/project/lxdx>`_, and installable via ``pip``:
+
+.. code-block::
+
+    pip install lxdx
+
+
+Examples
+--------
+.. code-block:: python
+
+    from lxdx import Dixt
+
+    assert Dixt() == {}
+    assert Dixt({1: 1, 'alpha': 'α'}) == {1: 1, 'alpha': 'α'}
+    assert Dixt(alpha='α', beta='β') == {'alpha': 'α', 'beta': 'β'}
+    assert Dixt(alpha='α', beta='β').is_supermap_of({'beta': 'β'})
+
+    # data can be deeply nested
+    data = {'Accept-Encoding': 'gzip', 'metadata': {'Content-Type': 'application/json'}}
+    dx = Dixt(**data)
+
+    # update dx using the union operator
+    dx |= {'other': 'dict or Dixt obj'}
+
+    # 'Normalise' the keys to use it as attributes additionally.
+    assert dx['Accept-Encoding'] == dx.accept_encoding
+    del dx.accept_encoding
+    print(dx.metadata.CONTENT_TYPE)
+
+    # Instead of
+    dx['a-list'][1]['obj-attr'] = 'value'
+
+    # Is way cleaner
+    dx.a_list[1].obj_attr = 'value'
+
+    # Programmatically get values
+    assert dx.a_list[1].obj_attr == dx.get_from('$.a_list[1].obj_attr')
+
+    json_str = '{"a": "JSON string"}'
+    assert Dixt.from_json(json_str).json() == json_str
+
+Documentation
+-------------
+Full documentation is at https://hardistones.github.io/lxdx.
+
+Future
+------
+``lxdx`` is supposed to be a library of "extended" ``list`` and ``dict``. For now there's no use case for the ``list`` extension.
+
+**To be supported**
+
+- User-defined meta specification.
+
+License
+-------
+This project and all its files are licensed under the 3-Clause BSD License.
+
+    Copyright (c) 2021, @github.com/hardistones
+    All rights reserved.
+
+    Redistribution and use in source and binary forms, with or without modification,
+    are permitted provided that the following conditions are met:
+
+    1. Redistributions of source code must retain the above copyright notice, this
+       list of conditions and the following disclaimer.
+
+    2. Redistributions in binary form must reproduce the above copyright notice,
+       this list of conditions and the following disclaimer in the documentation
+       and/or other materials provided with the distribution.
+
+    3. Neither the name of the copyright holder nor the names of its contributors
+       may be used to endorse or promote products derived from this software without
+       specific prior written permission.
+
+    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+    ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+    WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+    DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+    ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+    (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+    LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+    ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+    (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+    SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
+.. References
+.. _union operator: https://www.python.org/dev/peps/pep-0584
+.. _dot notation: https://en.wikipedia.org/wiki/Property_(programming)#Dot_notation
+.. _JsonPath: https://github.com/json-path/JsonPath
 
-setup(**setup_kwargs)
```

