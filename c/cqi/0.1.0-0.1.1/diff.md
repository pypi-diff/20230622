# Comparing `tmp/cqi-0.1.0.tar.gz` & `tmp/cqi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqi-0.1.0.tar", last modified: Wed Dec 15 10:33:44 2021, max compression
+gzip compressed data, was "cqi-0.1.1.tar", last modified: Thu Jun 22 10:31:04 2023, max compression
```

## Comparing `cqi-0.1.0.tar` & `cqi-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-12-15 10:33:44.533474 cqi-0.1.0/
--rw-rw-rw-   0        0        0     1072 2021-12-15 09:26:50.000000 cqi-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1534 2021-12-15 10:33:44.533474 cqi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      961 2021-12-15 09:36:45.000000 cqi-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2021-12-15 10:33:44.484323 cqi-0.1.0/cqi/
--rw-rw-rw-   0        0        0      157 2021-05-06 13:14:46.000000 cqi-0.1.0/cqi/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-15 10:33:44.508441 cqi-0.1.0/cqi/api/
--rw-rw-rw-   0        0        0       45 2021-05-06 13:14:46.000000 cqi-0.1.0/cqi/api/__init__.py
--rw-rw-rw-   0        0        0    22416 2021-11-15 11:54:00.000000 cqi-0.1.0/cqi/api/client.py
--rw-rw-rw-   0        0        0    12641 2021-12-15 09:49:41.000000 cqi-0.1.0/cqi/api/specification.py
--rw-rw-rw-   0        0        0     1583 2021-11-15 11:55:09.000000 cqi-0.1.0/cqi/client.py
--rw-rw-rw-   0        0        0     5926 2021-10-19 13:16:59.000000 cqi-0.1.0/cqi/errors.py
-drwxrwxrwx   0        0        0        0 2021-12-15 10:33:44.533474 cqi-0.1.0/cqi/models/
--rw-rw-rw-   0        0        0        0 2021-05-06 13:14:46.000000 cqi-0.1.0/cqi/models/__init__.py
--rw-rw-rw-   0        0        0     4424 2021-11-15 11:50:54.000000 cqi-0.1.0/cqi/models/attributes.py
--rw-rw-rw-   0        0        0     2180 2021-11-15 11:35:12.000000 cqi-0.1.0/cqi/models/corpora.py
--rw-rw-rw-   0        0        0     2088 2021-11-15 11:50:06.000000 cqi-0.1.0/cqi/models/ressource.py
--rw-rw-rw-   0        0        0     2527 2021-11-15 11:35:23.000000 cqi-0.1.0/cqi/models/subcorpora.py
--rw-rw-rw-   0        0        0       91 2021-12-15 09:27:22.000000 cqi-0.1.0/cqi/version.py
-drwxrwxrwx   0        0        0        0 2021-12-15 10:33:44.500446 cqi-0.1.0/cqi.egg-info/
--rw-rw-rw-   0        0        0     1534 2021-12-15 10:33:44.000000 cqi-0.1.0/cqi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2021-12-15 10:33:44.000000 cqi-0.1.0/cqi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-15 10:33:44.000000 cqi-0.1.0/cqi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2021-12-15 10:33:44.000000 cqi-0.1.0/cqi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-12-15 10:33:44.533474 cqi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      781 2021-12-15 10:33:07.000000 cqi-0.1.0/setup.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.787203 cqi-0.1.1/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2023-06-22 07:21:07.000000 cqi-0.1.1/LICENSE
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1537 2023-06-22 10:31:04.787203 cqi-0.1.1/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1051 2023-06-22 10:12:13.000000 cqi-0.1.1/README.md
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.777203 cqi-0.1.1/cqi/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      166 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/__init__.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.787203 cqi-0.1.1/cqi/api/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       45 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/api/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    21032 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/api/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    12641 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/api/specification.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1934 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     5821 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/errors.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.787203 cqi-0.1.1/cqi/models/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     5485 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/attributes.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2520 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/corpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2422 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/resource.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3216 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/models/subcorpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1084 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/status.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      145 2023-06-22 09:48:22.000000 cqi-0.1.1/cqi/version.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 10:31:04.787203 cqi-0.1.1/cqi.egg-info/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1537 2023-06-22 10:31:04.000000 cqi-0.1.1/cqi.egg-info/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      388 2023-06-22 10:31:04.000000 cqi-0.1.1/cqi.egg-info/SOURCES.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-06-22 10:31:04.000000 cqi-0.1.1/cqi.egg-info/dependency_links.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        4 2023-06-22 10:31:04.000000 cqi-0.1.1/cqi.egg-info/top_level.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-06-22 10:31:04.787203 cqi-0.1.1/setup.cfg
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      781 2023-06-22 07:21:07.000000 cqi-0.1.1/setup.py
```

### Comparing `cqi-0.1.0/LICENSE` & `cqi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cqi-0.1.0/PKG-INFO` & `cqi-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-Metadata-Version: 2.1
-Name: cqi
-Version: 0.1.0
-Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
-Home-page: https://github.com/Pevtrick/cqi-py
-Author: Patrick Jentsch
-Author-email: patrickjentsch@gmx.net
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CQi SDK for Python
-
-A Python library for the [IMS Open Corpus Workbench](http://cwb.sourceforge.net/) (CWB) [corpus query interface](http://cwb.sourceforge.net/cqi.php) (CQi) API.
-
-## Installation
-
-The latest stable version [is available on PyPI](https://pypi.python.org/pypi/cqi/). Either add `cqi` to your `requirements.txt` file or install with pip:
-
-```
-pip install cqi
-```
-
-## Version compatibility
-
-| Package version | Protocol version |
-|-----------------|------------------|
-| 0.1.0           | 0.1              |
-
-## Usage
-
-```python
-import cqi
-
-
-client = cqi.CQiClient('127.0.0.1')
-client.connect(username='anonymous', password='') # 258 ~ CQI_STATUS_CONNECT_OK
-client.ping() # 260 ~ CQI_STATUS_PING_OK
-corpus = client.corpora.get('CORPUS') # <Corpus: CORPUS>
-corpus.query('"and" []* "the";', 'Results') # 257 ~ CQI_STATUS_OK
-results = corpus.subcorpora.get('Results') # <Subcorpus: CORPUS:Results>
-client.disconnect() # 259 ~ CQI_STATUS_BYE_OK
-```
-
-
+Metadata-Version: 2.1
+Name: cqi
+Version: 0.1.1
+Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
+Home-page: https://github.com/Pevtrick/cqi-py
+Author: Patrick Jentsch
+Author-email: patrickjentsch@gmx.net
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CQi SDK for Python
+
+A Python library for the [IMS Open Corpus Workbench](http://cwb.sourceforge.net/) (CWB) [Corpus Query Interface](https://cwb.sourceforge.io/documentation.php#cqi) (CQi) API.
+
+## Installation
+
+The latest stable version [is available on PyPI](https://pypi.python.org/pypi/cqi/). Either add `cqi` to your `requirements.txt` file or install with pip:
+
+```
+pip install cqi
+```
+
+## Version compatibility
+
+| Package version | Protocol version |
+|-----------------|------------------|
+| 0.1.0           | 0.1              |
+| 0.1.1           | 0.1              |
+
+## Usage
+
+```python
+import cqi
+
+
+client = cqi.CQiClient('127.0.0.1')
+client.connect(username='anonymous', password='') # <class 'cqi.status.StatusConnectOk'>
+client.ping() # <class 'cqi.status.StatusPingOk'>
+corpus = client.corpora.get('CORPUS') # <Corpus: CORPUS>
+corpus.query('"and" []* "the";', 'Results') # <class 'cqi.status.StatusOk'>
+results = corpus.subcorpora.get('Results') # <Subcorpus: CORPUS:Results>
+client.disconnect() # <class 'cqi.status.StatusByeOk'>
+```
```

### Comparing `cqi-0.1.0/README.md` & `cqi-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # CQi SDK for Python
 
-A Python library for the [IMS Open Corpus Workbench](http://cwb.sourceforge.net/) (CWB) [corpus query interface](http://cwb.sourceforge.net/cqi.php) (CQi) API.
+A Python library for the [IMS Open Corpus Workbench](http://cwb.sourceforge.net/) (CWB) [Corpus Query Interface](https://cwb.sourceforge.io/documentation.php#cqi) (CQi) API.
 
 ## Installation
 
 The latest stable version [is available on PyPI](https://pypi.python.org/pypi/cqi/). Either add `cqi` to your `requirements.txt` file or install with pip:
 
 ```
 pip install cqi
 ```
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
 | 0.1.0           | 0.1              |
+| 0.1.1           | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
 
 
 client = cqi.CQiClient('127.0.0.1')
-client.connect(username='anonymous', password='') # 258 ~ CQI_STATUS_CONNECT_OK
-client.ping() # 260 ~ CQI_STATUS_PING_OK
+client.connect(username='anonymous', password='') # <class 'cqi.status.StatusConnectOk'>
+client.ping() # <class 'cqi.status.StatusPingOk'>
 corpus = client.corpora.get('CORPUS') # <Corpus: CORPUS>
-corpus.query('"and" []* "the";', 'Results') # 257 ~ CQI_STATUS_OK
+corpus.query('"and" []* "the";', 'Results') # <class 'cqi.status.StatusOk'>
 results = corpus.subcorpora.get('Results') # <Subcorpus: CORPUS:Results>
-client.disconnect() # 259 ~ CQI_STATUS_BYE_OK
+client.disconnect() # <class 'cqi.status.StatusByeOk'>
 ```
```

### Comparing `cqi-0.1.0/cqi/api/client.py` & `cqi-0.1.1/cqi/api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from . import specification
-from ..errors import (cl_error_lookup, error_lookup, cqp_error_lookup,
-                      CQiException)
+from typing import List, Tuple
 import math
 import socket
 import struct
 import time
+from . import specification
+from .. import errors
+from .. import status
 
 
 class APIClient:
-    """
+    '''
     A low-level client for the IMS Open Corpus Workbench (CWB) corpus query
     interface (CQi) API.
 
     Example:
     >>> import cqi
     >>> client = cqi.APIClient('127.0.0.1')
     >>> client.ctrl_connect('user', 'password')
@@ -26,577 +27,566 @@
     host (str): URL to the CQP server. For example,
         ``cqpserver.localhost`` or ``127.0.0.1``.
     port (int): Port the CQP server listens on. Default: ``4877``
     socket (socket.socket): Socket for communicating with a CQP server.
     timeout (int): Time to wait for bytes from the server. If the timeout is
         exceeded, an exception is raised. Default: ``math.inf``
     version (str): The version of the CQi protocol to use. Default: ``0.1``
-    """
-
-    def __init__(self, host, port=4877, timeout=math.inf, version='0.1'):
-        self.host = host
-        self.port = port
-        self.socket = socket.socket()
-        self.timeout = timeout
-        self.version = version
+    '''
 
-    def ctrl_connect(self, username, password):
+    def __init__(
+        self,
+        host: str,
+        port: int = 4877,
+        timeout: float = math.inf,
+        version: str = '0.1'
+    ):
+        self.host: str = host
+        self.port: int = port
+        self.socket: socket.socket = socket.socket()
+        self.timeout: float = timeout
+        self.version: str = version
+
+    def ctrl_connect(
+        self,
+        username: str,
+        password: str
+    ) -> status.StatusConnectOk:
         self.socket.connect((self.host, self.port))
-        # INPUT: (STRING username, STRING password)
-        # OUTPUT: CQI_STATUS_CONNECT_OK, CQI_ERROR_CONNECT_REFUSED
         self.__send_WORD(specification.CTRL_CONNECT)
         self.__send_STRING(username)
         self.__send_STRING(password)
         return self.__recv_response()
 
-    def ctrl_bye(self):
-        # INPUT: ()
-        # OUTPUT: CQI_STATUS_BYE_OK
+    def ctrl_bye(self) -> status.StatusByeOk:
         self.__send_WORD(specification.CTRL_BYE)
         response = self.__recv_response()
         self.socket.close()
         return response
 
     def ctrl_user_abort(self):
-        # INPUT: ()
-        # OUTPUT:
         self.__send_WORD(specification.CTRL_USER_ABORT)
 
-    def ctrl_ping(self):
-        # INPUT: ()
-        # OUTPUT: CQI_STATUS_PING_OK
+    def ctrl_ping(self) -> status.StatusPingOk:
         self.__send_WORD(specification.CTRL_PING)
         return self.__recv_response()
 
-    def ctrl_last_general_error(self):
-        # INPUT: ()
-        # OUTPUT: CQI_DATA_STRING
-        # full-text error message for the last general error reported by the
-        # CQi server
+    def ctrl_last_general_error(self) -> str:
+        ''' 
+            Full-text error message for the last general error reported by the
+            CQi server
+        '''
         self.__send_WORD(specification.CTRL_LAST_GENERAL_ERROR)
         return self.__recv_response()
 
-    def ask_feature_cqi_1_0(self):
-        # INPUT: ()
-        # OUTPUT: CQI_DATA_BOOL
+    def ask_feature_cqi_1_0(self) -> bool:
         self.__send_WORD(specification.ASK_FEATURE_CQI_1_0)
         return self.__recv_response()
 
-    def ask_feature_cl_2_3(self):
-        # INPUT: ()
-        # OUTPUT: CQI_DATA_BOOL
+    def ask_feature_cl_2_3(self) -> bool:
         self.__send_WORD(specification.ASK_FEATURE_CL_2_3)
         return self.__recv_response()
 
-    def ask_feature_cqp_2_3(self):
-        # INPUT: ()
-        # OUTPUT: CQI_DATA_BOOL
+    def ask_feature_cqp_2_3(self) -> bool:
         self.__send_WORD(specification.ASK_FEATURE_CL_2_3)
         return self.__recv_response()
 
-    def corpus_list_coprora(self):
-        # INPUT: ()
-        # OUTPUT: CQI_DATA_STRING_LIST
+    def corpus_list_coprora(self) -> List[str]:
         self.__send_WORD(specification.CORPUS_LIST_CORPORA)
         return self.__recv_response()
 
-    def corpus_charset(self, corpus):
-        # INPUT: (STRING corpus)
-        # OUTPUT: CQI_DATA_STRING
+    def corpus_charset(self, corpus: str) -> str:
         self.__send_WORD(specification.CORPUS_CHARSET)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
-    def corpus_properties(self, corpus):
-        # INPUT: (STRING corpus)
-        # OUTPUT: CQI_DATA_STRING_LIST
+    def corpus_properties(self, corpus: str) -> List[str]:
         self.__send_WORD(specification.CORPUS_PROPERTIES)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
-    def corpus_positional_attributes(self, corpus):
-        # INPUT: (STRING corpus)
-        # OUTPUT: CQI_DATA_STRING_LIST
+    def corpus_positional_attributes(self, corpus: str) -> List[str]:
         self.__send_WORD(specification.CORPUS_POSITIONAL_ATTRIBUTES)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
-    def corpus_structural_attributes(self, corpus):
-        # INPUT: (STRING corpus)
-        # OUTPUT: CQI_DATA_STRING_LIST
+    def corpus_structural_attributes(self, corpus: str) -> List[str]:
         self.__send_WORD(specification.CORPUS_STRUCTURAL_ATTRIBUTES)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
-    def corpus_structural_attribute_has_values(self, attribute):
-        # INPUT: (STRING attribute)
-        # OUTPUT: CQI_DATA_BOOL
+    def corpus_structural_attribute_has_values(self, attribute: str) -> bool:
         self.__send_WORD(specification.CORPUS_STRUCTURAL_ATTRIBUTE_HAS_VALUES)
         self.__send_STRING(attribute)
         return self.__recv_response()
 
-    def corpus_alignment_attributes(self, corpus):
-        # INPUT: (STRING corpus)
-        # OUTPUT: CQI_DATA_STRING_LIST
+    def corpus_alignment_attributes(self, corpus: str) -> List[str]:
         self.__send_WORD(specification.CORPUS_ALIGNMENT_ATTRIBUTES)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
-    def corpus_full_name(self, corpus):
-        # INPUT: (STRING corpus)
-        # OUTPUT: CQI_DATA_STRING
-        # the full name of <corpus> as specified in its registry entry
+    def corpus_full_name(self, corpus: str) -> str:
+        ''' the full name of <corpus> as specified in its registry entry '''
         self.__send_WORD(specification.CORPUS_FULL_NAME)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
-    def corpus_info(self, corpus):
-        # INPUT: (STRING corpus)
-        # OUTPUT: CQI_DATA_STRING_LIST
-        # returns the contents of the .info file of <corpus> as a list of lines
+    def corpus_info(self, corpus: str) -> List[str]:
+        ''' 
+            returns the contents of the .info file of <corpus> as a list of
+            lines
+        '''
         self.__send_WORD(specification.CORPUS_INFO)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
-    def corpus_drop_corpus(self, corpus):
-        # INPUT: (STRING corpus)
-        # OUTPUT: CQI_STATUS_OK
-        # try to unload a corpus and all its attributes from memory
+    def corpus_drop_corpus(self, corpus: str) -> status.StatusOk:
+        ''' try to unload a corpus and all its attributes from memory '''
         self.__send_WORD(specification.CORPUS_DROP_CORPUS)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
-    def cl_attribute_size(self, attribute):
-        # INPUT: (STRING attribute)
-        # OUTPUT: CQI_DATA_INT
-        # returns the size of <attribute>:
-        #     number of tokens        (positional)
-        #     number of regions       (structural)
-        #     number of alignments    (alignment)
+    def cl_attribute_size(self, attribute: str) -> int:
+        ''' 
+            returns the size of <attribute>:
+            - number of tokens        (positional)
+            - number of regions       (structural)
+            - number of alignments    (alignment)
+        '''
         self.__send_WORD(specification.CL_ATTRIBUTE_SIZE)
         self.__send_STRING(attribute)
         return self.__recv_response()
 
-    def cl_lexicon_size(self, attribute):
-        # INPUT: (STRING attribute)
-        # OUTPUT: CQI_DATA_INT
-        # returns the number of entries in the lexicon of a positional
-        # attribute;
-        # valid lexicon IDs range from 0 .. (lexicon_size - 1)
+    def cl_lexicon_size(self, attribute: str) -> int:
+        '''
+            returns the number of entries in the lexicon of a positional
+            attribute;
+
+            valid lexicon IDs range from 0 .. (lexicon_size - 1)
+        '''
         self.__send_WORD(specification.CL_LEXICON_SIZE)
         self.__send_STRING(attribute)
         return self.__recv_response()
 
-    def cl_drop_attribute(self, attribute):
-        # INPUT: (STRING attribute)
-        # OUTPUT: CQI_STATUS_OK
-        # unload attribute from memory
+    def cl_drop_attribute(self, attribute: str) -> status.StatusOk:
+        ''' unload attribute from memory '''
         self.__send_WORD(specification.CL_DROP_ATTRIBUTE)
         self.__send_STRING(attribute)
         return self.__recv_response()
 
-    """
-    " NOTE: simple (scalar) mappings are applied to lists (the returned list
-    "       has exactly the same length as the list passed as an argument)
-    """
-
-    def cl_str2id(self, attribute, strings):
-        # INPUT: (STRING attribute, STRING_LIST strings)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns -1 for every string in <strings> that is not found in the
-        # lexicon
+    '''
+    ' NOTE: simple (scalar) mappings are applied to lists (the returned list
+    '       has exactly the same length as the list passed as an argument)
+    '''
+
+    def cl_str2id(self, attribute: str, strings: List[str]) -> List[int]:
+        '''
+            returns -1 for every string in <strings> that is not found in the
+            lexicon
+        '''
         self.__send_WORD(specification.CL_STR2ID)
         self.__send_STRING(attribute)
         self.__send_STRING_LIST(strings)
         return self.__recv_response()
 
-    def cl_id2str(self, attribute, id):
-        # INPUT: (STRING attribute, INT_LIST id)
-        # OUTPUT: CQI_DATA_STRING_LIST
-        # returns "" for every ID in <id> that is out of range
+    def cl_id2str(self, attribute: str, id: List[int]) -> List[str]:
+        ''' returns "" for every ID in <id> that is out of range '''
         self.__send_WORD(specification.CL_ID2STR)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(id)
         return self.__recv_response()
 
-    def cl_id2freq(self, attribute, id):
-        # INPUT: (STRING attribute, INT_LIST id)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns 0 for every ID in <id> that is out of range
+    def cl_id2freq(self, attribute: str, id: List[int]) -> List[int]:
+        ''' returns 0 for every ID in <id> that is out of range '''
         self.__send_WORD(specification.CL_ID2FREQ)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(id)
         return self.__recv_response()
 
-    def cl_cpos2id(self, attribute, cpos):
-        # INPUT: (STRING attribute, INT_LIST cpos)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns -1 for every corpus position in <cpos> that is out of range
-        self.__send_WORD(specification.CL_ID2FREQ)
+    def cl_cpos2id(self, attribute: str, cpos: List[int]) -> List[int]:
+        ''' 
+            returns -1 for every corpus position in <cpos> that is out of
+            range
+        '''
+        self.__send_WORD(specification.CL_CPOS2ID)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
-    def cl_cpos2str(self, attribute, cpos):
-        # INPUT: (STRING attribute, INT_LIST cpos)
-        # OUTPUT: CQI_DATA_STRING_LIST
-        # returns "" for every corpus position in <cpos> that is out of range
+    def cl_cpos2str(self, attribute: str, cpos: List[int]) -> List[str]:
+        '''
+            returns "" for every corpus position in <cpos> that is out of
+            range
+        '''
         self.__send_WORD(specification.CL_CPOS2STR)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
-    def cl_cpos2struc(self, attribute, cpos):
-        # INPUT: (STRING attribute, INT_LIST cpos)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns -1 for every corpus position not inside a structure region
+    def cl_cpos2struc(self, attribute: str, cpos: List[int]) -> List[int]:
+        '''
+            returns -1 for every corpus position not inside a structure region
+        '''
         self.__send_WORD(specification.CL_CPOS2STRUC)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
-    """
-    " NOTE: temporary addition for the Euralex2000 tutorial, but should
-    "       probably be included in CQi specs
-    """
-
-    def cl_cpos2lbound(self, attribute, cpos):
-        # INPUT: (STRING attribute, INT_LIST cpos)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns left boundary of s-attribute region enclosing cpos, -1 if not
-        # in region
+    '''
+    ' NOTE: temporary addition for the Euralex2000 tutorial, but should
+    '       probably be included in CQi specs
+    '''
+
+    def cl_cpos2lbound(self, attribute: str, cpos: List[int]) -> List[int]:
+        '''
+            returns left boundary of s-attribute region enclosing cpos, -1 if
+            not in region
+        '''
         self.__send_WORD(specification.CL_CPOS2LBOUND)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
-    def cl_cpos2rbound(self, attribute, cpos):
-        # INPUT: (STRING attribute, INT_LIST cpos)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns right boundary of s-attribute region enclosing cpos, -1 if
-        # not in region
+    def cl_cpos2rbound(self, attribute: str, cpos: List[int]) -> List[int]:
+        '''
+            returns right boundary of s-attribute region enclosing cpos, -1 if
+            not in region
+        '''
         self.__send_WORD(specification.CL_CPOS2RBOUND)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
-    def cl_cpos2alg(self, attribute, cpos):
-        # INPUT: (STRING attribute, INT_LIST cpos)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns -1 for every corpus position not inside an alignment
+    def cl_cpos2alg(self, attribute: str, cpos: List[int]) -> List[int]:
+        ''' returns -1 for every corpus position not inside an alignment '''
         self.__send_WORD(specification.CL_CPOS2ALG)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(cpos)
         return self.__recv_response()
 
-    def cl_struc2str(self, attribute, strucs):
-        # INPUT: (STRING attribute, INT_LIST strucs)
-        # OUTPUT: CQI_DATA_STRING_LIST
-        # returns annotated string values of structure regions in <strucs>; ""
-        # if out of range
-        # check CQI_CORPUS_STRUCTURAL_ATTRIBUTE_HAS_VALUES(<attribute>) first
+    def cl_struc2str(self, attribute: str, strucs: List[int]) -> List[str]:
+        '''
+            returns annotated string values of structure regions in <strucs>;
+            "" if out of range
+
+            check corpus_structural_attribute_has_values(<attribute>) first
+        '''
         self.__send_WORD(specification.CL_STRUC2STR)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(strucs)
         return self.__recv_response()
 
-    """
-    " NOTE: the following mappings take a single argument and return multiple
-    "       values, including lists of arbitrary size
-    """
-
-    def cl_id2cpos(self, attribute, id):
-        # INPUT: (STRING attribute, INT id)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns all corpus positions where the given token occurs
+    '''
+    ' NOTE: the following mappings take a single argument and return multiple
+    '       values, including lists of arbitrary size
+    '''
+
+    def cl_id2cpos(self, attribute: str, id: int) -> List[int]:
+        ''' returns all corpus positions where the given token occurs '''
         self.__send_WORD(specification.CL_ID2CPOS)
         self.__send_STRING(attribute)
         self.__send_INT(id)
         return self.__recv_response()
 
-    def cl_idlist2cpos(self, attribute, id_list):
-        # INPUT: (STRING attribute, INT_LIST id_list)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns all corpus positions where one of the tokens in <id_list>
-        # occurs; the returned list is sorted as a whole, not per token id
+    def cl_idlist2cpos(self, attribute: str, id_list: List[int]) -> List[int]:
+        '''
+            returns all corpus positions where one of the tokens in <id_list>
+            occurs; the returned list is sorted as a whole, not per token id
+        '''
         self.__send_WORD(specification.CL_IDLIST2CPOS)
         self.__send_STRING(attribute)
         self.__send_INT_LIST(id_list)
         return self.__recv_response()
 
-    def cl_regex2id(self, attribute, regex):
-        # INPUT: (STRING attribute, STRING regex)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns lexicon IDs of all tokens that match <regex>; the returned
-        # list may be empty (size 0);
+    def cl_regex2id(self, attribute: str, regex: str) -> List[int]:
+        '''
+            returns lexicon IDs of all tokens that match <regex>; the returned
+            list may be empty (size 0);
+        '''
         self.__send_WORD(specification.CL_REGEX2ID)
         self.__send_STRING(attribute)
         self.__send_STRING(regex)
         return self.__recv_response()
 
-    def cl_struc2cpos(self, attribute, struc):
-        # INPUT: (STRING attribute, INT struc)
-        # OUTPUT: CQI_DATA_INT_INT
-        # returns start and end corpus positions of structure region <struc>
+    def cl_struc2cpos(self, attribute: str, struc: int) -> Tuple[int, int]:
+        '''
+            returns start and end corpus positions of structure region <struc>
+        '''
         self.__send_WORD(specification.CL_STRUC2CPOS)
         self.__send_STRING(attribute)
         self.__send_INT(struc)
         return self.__recv_response()
 
-    def cl_alg2cpos(self, attribute, alg):
-        # INPUT: (STRING attribute, INT alg)
-        # OUTPUT: CQI_DATA_INT_INT_INT_INT
-        # returns (src_start, src_end, target_start, target_end)
+    def cl_alg2cpos(self, attribute: str, alg: int) -> Tuple[int, int, int, int]:
+        ''' returns (src_start, src_end, target_start, target_end) '''
         self.__send_WORD(specification.CL_ALG2CPOS)
         self.__send_STRING(attribute)
         self.__send_INT(alg)
         return self.__recv_response()
 
-    def cqp_query(self, mother_corpus, subcorpus_name, query):
-        # INPUT: (STRING mother_corpus, STRING subcorpus_name, STRING query)
-        # OUTPUT: CQI_STATUS_OK
-        # <query> must include the ';' character terminating the query.
+    def cqp_query(self,
+        mother_corpus: str,
+        subcorpus_name: str,
+        query: str
+    ) -> status.StatusOk:
+        ''' <query> must include the ';' character terminating the query. '''
         self.__send_WORD(specification.CQP_QUERY)
         self.__send_STRING(mother_corpus)
         self.__send_STRING(subcorpus_name)
         self.__send_STRING(query)
         return self.__recv_response()
 
-    def cqp_list_subcorpora(self, corpus):
-        # INPUT: (STRING corpus)
-        # OUTPUT: CQI_DATA_STRING_LIST
+    def cqp_list_subcorpora(self, corpus: str) -> List[str]:
         self.__send_WORD(specification.CQP_LIST_SUBCORPORA)
         self.__send_STRING(corpus)
         return self.__recv_response()
 
-    def cqp_subcorpus_size(self, subcorpus):
-        # INPUT: (STRING subcorpus)
-        # OUTPUT: CQI_DATA_INT
+    def cqp_subcorpus_size(self, subcorpus: str) -> int:
         self.__send_WORD(specification.CQP_SUBCORPUS_SIZE)
         self.__send_STRING(subcorpus)
         return self.__recv_response()
 
-    def cqp_subcorpus_has_field(self, subcorpus, field):
-        # INPUT: (STRING subcorpus, BYTE field)
-        # OUTPUT: CQI_DATA_BOOL
+    def cqp_subcorpus_has_field(self, subcorpus: str, field: int) -> bool:
         self.__send_WORD(specification.CQP_SUBCORPUS_HAS_FIELD)
         self.__send_STRING(subcorpus)
         self.__send_BYTE(field)
         return self.__recv_response()
 
-    def cqp_dump_subcorpus(self, subcorpus, field, first, last):
-        # INPUT: (STRING subcorpus, BYTE field, INT first, INT last)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # Dump the values of <field> for match ranges <first> .. <last>
-        # in <subcorpus>. <field> is one of the CQI_CONST_FIELD_* constants.
+    def cqp_dump_subcorpus(
+        self,
+        subcorpus: str,
+        field: int,
+        first: int,
+        last: int
+    ) -> List[int]:
+        '''
+            Dump the values of <field> for match ranges <first> .. <last>
+            in <subcorpus>. <field> is one of the CQI_CONST_FIELD_* constants.
+        '''
         self.__send_WORD(specification.CQP_DUMP_SUBCORPUS)
         self.__send_STRING(subcorpus)
         self.__send_BYTE(field)
         self.__send_INT(first)
         self.__send_INT(last)
         return self.__recv_response()
 
-    def cqp_drop_subcorpus(self, subcorpus):
-        # INPUT: (STRING subcorpus)
-        # OUTPUT: CQI_STATUS_OK
-        # delete a subcorpus from memory
+    def cqp_drop_subcorpus(self, subcorpus: str) -> status.StatusOk:
+        ''' delete a subcorpus from memory '''
         self.__send_WORD(specification.CQP_DROP_SUBCORPUS)
         self.__send_STRING(subcorpus)
         return self.__recv_response()
 
-    """
-    " NOTE: The following two functions are temporarily included for the
-    "       Euralex 2000 tutorial demo
-    """
-
-    def cqp_fdist_1(self, subcorpus, cutoff, field, attribute):
-        """ NOTE: frequency distribution of single tokens """
-        # INPUT: (STRING subcorpus, INT cutoff, BYTE field, STRING attribute)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns <n> (id, frequency) pairs flattened into a list of size 2*<n>
-        # field is one of CQI_CONST_FIELD_MATCH, CQI_CONST_FIELD_TARGET,
-        #                 CQI_CONST_FIELD_KEYWORD
-        # NB: pairs are sorted by frequency desc.
+    '''
+    ' NOTE: The following two functions are temporarily included for the
+    '       Euralex 2000 tutorial demo
+    '''
+
+    def cqp_fdist_1(
+        self,
+        subcorpus: str,
+        cutoff: int,
+        field: int,
+        attribute: str
+    ) -> List[int]:
+        ''' frequency distribution of single tokens
+
+            returns <n> (id, frequency) pairs flattened into a list of size
+            2*<n>
+            field is one of
+            - CQI_CONST_FIELD_MATCH
+            - CQI_CONST_FIELD_TARGET
+            - CQI_CONST_FIELD_KEYWORD
+
+            NB: pairs are sorted by frequency desc.
+        '''
         self.__send_WORD(specification.CQP_FDIST_1)
         self.__send_STRING(subcorpus)
         self.__send_INT(cutoff)
         self.__send_BYTE(field)
         self.__send_STRING(attribute)
         return self.__recv_response()
 
-    def cqp_fdist_2(self, subcorpus, cutoff, field1, attribute1, field2,
-                    attribute2):
-        """ NOTE: frequency distribution of pairs of tokens """
-        # INPUT: (STRING subcorpus, INT cutoff, BYTE field1, STRING attribute1,
-        #         BYTE field2, STRING attribute2)
-        # OUTPUT: CQI_DATA_INT_LIST
-        # returns <n> (id1, id2, frequency) pairs flattened into a list of size
-        # 3*<n>
-        # NB: triples are sorted by frequency desc.
+    def cqp_fdist_2(
+        self,
+        subcorpus: str,
+        cutoff: int,
+        field1: int,
+        attribute1: str,
+        field2: int,
+        attribute2: str
+    ) -> List[int]:
+        ''' frequency distribution of pairs of tokens
+
+            returns <n> (id1, id2, frequency) pairs flattened into a list of
+            size 3*<n>
+
+            NB: triples are sorted by frequency desc.
+        '''
         self.__send_WORD(specification.CQP_FDIST_2)
         self.__send_STRING(subcorpus)
         self.__send_INT(cutoff)
         self.__send_BYTE(field1)
         self.__send_STRING(attribute1)
         self.__send_BYTE(field2)
         self.__send_STRING(attribute2)
         return self.__recv_response()
 
     def __recv_response(self):
         byte_data = self.__recv_WORD()
         response_type = byte_data >> 8
         if response_type == specification.CL_ERROR:
-            raise cl_error_lookup[byte_data]()
+            raise errors.cl_error_lookup[byte_data]()
         elif response_type == specification.CQP_ERROR:
-            raise cqp_error_lookup[byte_data]()
+            raise errors.cqp_error_lookup[byte_data]()
         elif response_type == specification.DATA:
             return self.__recv_DATA(byte_data)
         elif response_type == specification.ERROR:
-            raise error_lookup[byte_data]()
+            raise errors.error_lookup[byte_data]()
         elif response_type == specification.STATUS:
-            return byte_data
+            return status.status_lookup[byte_data]()
         else:
-            raise CQiException(f'Unknown response type: {response_type}')
+            raise errors.CQiException(f'Unknown response type: {response_type}')
 
     def __recv_DATA(self, data_type):
         if data_type == specification.DATA_BYTE:
-            data = self.__recv_DATA_BYTE()
+            return self.__recv_DATA_BYTE()
         elif data_type == specification.DATA_BOOL:
-            data = self.__recv_DATA_BOOL()
+            return self.__recv_DATA_BOOL()
         elif data_type == specification.DATA_INT:
-            data = self.__recv_DATA_INT()
+            return self.__recv_DATA_INT()
         elif data_type == specification.DATA_STRING:
-            data = self.__recv_DATA_STRING()
+            return self.__recv_DATA_STRING()
         elif data_type == specification.DATA_BYTE_LIST:
-            data = self.__recv_DATA_BYTE_LIST()
+            return self.__recv_DATA_BYTE_LIST()
         elif data_type == specification.DATA_BOOL_LIST:
-            data = self.__recv_DATA_BOOL_LIST()
+            return self.__recv_DATA_BOOL_LIST()
         elif data_type == specification.DATA_INT_LIST:
-            data = self.__recv_DATA_INT_LIST()
+            return self.__recv_DATA_INT_LIST()
         elif data_type == specification.DATA_STRING_LIST:
-            data = self.__recv_DATA_STRING_LIST()
+            return self.__recv_DATA_STRING_LIST()
         elif data_type == specification.DATA_INT_INT:
-            data = self.__recv_DATA_INT_INT()
+            return self.__recv_DATA_INT_INT()
         elif data_type == specification.DATA_INT_INT_INT_INT:
-            data = self.__recv_DATA_INT_INT_INT_INT()
+            return self.__recv_DATA_INT_INT_INT_INT()
         elif data_type == specification.DATA_INT_TABLE:
-            data = self.__recv_DATA_INT_TABLE()
+            return self.__recv_DATA_INT_TABLE()
         else:
-            raise CQiException(f'Unknown data type: {data_type}')
-        return data
+            raise errors.CQiException(f'Unknown data type: {data_type}')
 
-    def __recv_wrapper(self, bufsize):
+    def __recv_wrapper(self, bufsize: int) -> bytes:
         start_time = time.time()
         while time.time() - start_time < self.timeout:
             # Check if the server already sent over the desired number of bytes
             if len(self.socket.recv(bufsize, socket.MSG_PEEK)) == bufsize:
                 return self.socket.recv(bufsize)
             time.sleep(0.05)
         else:
-            raise CQiException('Timeout: Not enough bytes')
+            raise errors.CQiException('Timeout: Not enough bytes')
 
-    def __recv_DATA_BYTE(self):
+    def __recv_DATA_BYTE(self) -> int:
         byte_data = self.__recv_wrapper(1)
         return struct.unpack('!B', byte_data)[0]
 
-    def __recv_DATA_BOOL(self):
+    def __recv_DATA_BOOL(self) -> bool:
         byte_data = self.__recv_wrapper(1)
         return struct.unpack('!?', byte_data)[0]
 
-    def __recv_DATA_INT(self):
+    def __recv_DATA_INT(self) -> int:
         byte_data = self.__recv_wrapper(4)
         return struct.unpack('!i', byte_data)[0]
 
-    def __recv_DATA_STRING(self):
+    def __recv_DATA_STRING(self) -> str:
         n = self.__recv_WORD()
         byte_data = self.__recv_wrapper(n)
         return struct.unpack(f'!{n}s', byte_data)[0].decode()
 
-    def __recv_DATA_BYTE_LIST(self):
+    def __recv_DATA_BYTE_LIST(self) -> List[int]:
         data = []
         n = self.__recv_DATA_INT()
         while n > 0:
             data.append(self.__recv_DATA_BYTE())
             n -= 1
         return data
 
-    def __recv_DATA_BOOL_LIST(self):
+    def __recv_DATA_BOOL_LIST(self) -> List[bool]:
         data = []
         n = self.__recv_DATA_INT()
         while n > 0:
             data.append(self.__recv_DATA_BOOL())
             n -= 1
         return data
 
-    def __recv_DATA_INT_LIST(self):
+    def __recv_DATA_INT_LIST(self) -> List[int]:
         data = []
         n = self.__recv_DATA_INT()
         while n > 0:
             data.append(self.__recv_DATA_INT())
             n -= 1
         return data
 
-    def __recv_DATA_STRING_LIST(self):
+    def __recv_DATA_STRING_LIST(self) -> List[str]:
         data = []
         n = self.__recv_DATA_INT()
         while n > 0:
             data.append(self.__recv_DATA_STRING())
             n -= 1
         return data
 
-    def __recv_DATA_INT_INT(self):
+    def __recv_DATA_INT_INT(self) -> Tuple[int, int]:
         return (self.__recv_DATA_INT(), self.__recv_DATA_INT())
 
-    def __recv_DATA_INT_INT_INT_INT(self):
-        return (self.__recv_DATA_INT(),
-                self.__recv_DATA_INT(),
-                self.__recv_DATA_INT(),
-                self.__recv_DATA_INT())
+    def __recv_DATA_INT_INT_INT_INT(self) -> Tuple[int, int, int, int]:
+        return (
+            self.__recv_DATA_INT(),
+            self.__recv_DATA_INT(),
+            self.__recv_DATA_INT(),
+            self.__recv_DATA_INT()
+        )
 
-    def __recv_DATA_INT_TABLE(self):
+    def __recv_DATA_INT_TABLE(self) -> List[List[int]]:
         rows = self.__recv_DATA_INT()
         columns = self.__recv_DATA_INT()
         data = []
         for i in range(0, rows):
             row = []
             for j in range(0, columns):
                 row.append(self.__recv_DATA_INT())
             data.append(row)
         return data
 
-    def __recv_WORD(self):
+    def __recv_WORD(self) -> int:
         byte_data = self.__recv_wrapper(2)
         return struct.unpack('!H', byte_data)[0]
 
-    def __send_BYTE(self, byte_data):
+    def __send_BYTE(self, byte_data: int):
         data = struct.pack('!B', byte_data)
         self.socket.sendall(data)
 
-    def __send_BOOL(self, bool_data):
+    def __send_BOOL(self, bool_data: bool):
         data = struct.pack('!?', bool_data)
         self.socket.sendall(data)
 
-    def __send_INT(self, int_data):
+    def __send_INT(self, int_data: int):
         data = struct.pack('!i', int_data)
         self.socket.sendall(data)
 
-    def __send_STRING(self, string_data):
+    def __send_STRING(self, string_data: str):
         encoded_string_data = string_data.encode('utf-8')
         n = len(encoded_string_data)
         data = struct.pack(f'!H{n}s', n, encoded_string_data)
         self.socket.sendall(data)
 
-    def __send_INT_LIST(self, int_list_data):
+    def __send_INT_LIST(self, int_list_data: List[int]):
         n = len(int_list_data)
         self.__send_INT(n)
         for int_data in int_list_data:
             self.__send_INT(int_data)
 
-    def __send_STRING_LIST(self, string_list_data):
+    def __send_STRING_LIST(self, string_list_data: List[str]):
         n = len(string_list_data)
         self.__send_INT(n)
         for string_data in string_list_data:
             self.__send_STRING(string_data)
 
-    def __send_WORD(self, word_data):
+    def __send_WORD(self, word_data: int):
         data = struct.pack('!H', word_data)
         self.socket.sendall(data)
```

### Comparing `cqi-0.1.0/cqi/api/specification.py` & `cqi-0.1.1/cqi/api/specification.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.0/cqi/client.py` & `cqi-0.1.1/cqi/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,74 @@
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from .status import StatusByeOk, StatusConnectOk, StatusPingOk
+import math
 from .api import APIClient
 from .models.corpora import CorpusCollection
-import math
+
 
 
 class CQiClient:
-    """
+    '''
     A client for communicating with a CQi server.
 
     Example:
     >>> import cqi
     >>> client = cqi.CQiClient('127.0.0.1')
     >>> client.connect()
     258  # CQI_STATUS_CONNECT_OK
     >>> client.ping()
     260  # CQI_STATUS_PING_OK
     >>> client.disconnect()
     259  # CQI_STATUS_BYE_OK
 
     Attributes:
     api (APIClient): An API client pointing to the specified CQP server.
-    """
+    '''
 
-    def __init__(self, host, port=4877, timeout=math.inf, version='0.1'):
-        """
+    def __init__(
+        self,
+        host: str,
+        port: int = 4877,
+        timeout: float = math.inf,
+        version: str = '0.1'
+    ):
+        '''
         CQiClient constructor
 
         Args:
         host (str): URL to the CQP server. For example,
             ``cqpserver.localhost`` or ``127.0.0.1``.
         port (int): Port the CQP server listens on. Default: ``4877``
         timeout (int): Time to wait for bytes from the server. If the timeout
             is exceeded, an exception is raised. Default: ``math.inf``
         version (str): The version of the CQi protocol to use. Default: ``0.1``
-        """
-        self.api = APIClient(host, port=port, timeout=timeout, version=version)
+        '''
+        self.api: APIClient = APIClient(
+            host,
+            port=port,
+            timeout=timeout,
+            version=version
+        )
 
     @property
-    def corpora(self):
+    def corpora(self) -> CorpusCollection:
         return CorpusCollection(client=self)
 
-    def bye(self):
+    def bye(self) -> 'StatusByeOk':
         return self.api.ctrl_bye()
 
-    def connect(self, username='anonymous', password=''):
-        status = self.api.ctrl_connect(username, password)
-        return status
+    def connect(
+        self,
+        username: str = 'anonymous',
+        password: str = ''
+    ) -> 'StatusConnectOk':
+        return self.api.ctrl_connect(username, password)
 
-    def ping(self):
+    def ping(self) -> 'StatusPingOk':
         return self.api.ctrl_ping()
 
     def user_abort(self):
-        return self.api.ctrl_user_abort()
+        self.api.ctrl_user_abort()
 
     # Method aliases
     disconnect = bye
```

### Comparing `cqi-0.1.0/cqi/errors.py` & `cqi-0.1.1/cqi/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .api import specification
 
 
 class CQiException(Exception):
-    """
+    '''
     A base class from which all other exceptions inherit.
     If you want to catch all errors that the CQi package might raise,
     catch this base exception.
-    """
+    '''
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = None
         self.name = None
         self.description = None
 
@@ -56,66 +56,65 @@
 
 
 class CLErrorNoSuchAttribute(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_NO_SUCH_ATTRIBUTE
         self.name = specification.lookup[self.code]
-        self.description = "CQi server couldn't open attribute"
+        self.description = 'CQi server couldn\'t open attribute'
 
 
 class CLErrorWrongAttributeType(CLError):
-    # CDA_EATTTYPE
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_WRONG_ATTRIBUTE_TYPE
         self.name = specification.lookup[self.code]
 
 
 class CLErrorOutOfRange(CLError):
-    # CDA_EIDORNG, CDA_EIDXORNG, CDA_EPOSORNG
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_OUT_OF_RANGE
         self.name = specification.lookup[self.code]
 
 
 class CLErrorRegex(CLError):
-    # CDA_EPATTERN (not used), CDA_EBADREGEX
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_REGEX
         self.name = specification.lookup[self.code]
 
 
 class CLErrorCorpusAccess(CLError):
-    # CDA_ENODATA
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_CORPUS_ACCESS
         self.name = specification.lookup[self.code]
+        self.description = ''
 
 
 class CLErrorOutOfMemory(CLError):
-    # CDA_ENOMEM
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_OUT_OF_MEMORY
         self.name = specification.lookup[self.code]
-        self.description = ('CQi server has run out of memory; try discarding '
-                            'some other corpora and/or subcorpora')
+        self.description = (
+            'CQi server has run out of memory; try discarding some other '
+            'corpora and/or subcorpora'
+        )
 
 
 class CLErrorInternal(CLError):
-    # CDA_EOTHER, CDA_ENYI
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CL_ERROR_INTERNAL
         self.name = specification.lookup[self.code]
-        self.description = "Classical 'please contact technical support' error"
+        self.description = (
+            'The classical \'please contact technical support\' error'
+        )
 
 
 class CQPError(CQiException):
     # CQP error messages yet to be defined
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.code = specification.CQP_ERROR
```

### Comparing `cqi-0.1.0/cqi/models/corpora.py` & `cqi-0.1.1/cqi/models/corpora.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,81 @@
-from .attributes import (AlignmentAttributeCollection,
-                         PositionalAttributeCollection,
-                         StructuralAttributeCollection)
-from .ressource import Collection, Model
+from typing import Dict, List, TYPE_CHECKING
+if TYPE_CHECKING:
+    from ..status import StatusOk
+from .attributes import (
+    AlignmentAttributeCollection,
+    PositionalAttributeCollection,
+    StructuralAttributeCollection
+)
+from .resource import Collection, Model
 from .subcorpora import SubcorpusCollection
 
 
 class Corpus(Model):
-    id_attribute = 'api_name'
+    id_attribute: str = 'api_name'
 
     @property
-    def api_name(self):
+    def api_name(self) -> str:
         return self.attrs.get('api_name')
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self.attrs.get('name')
 
     @property
-    def size(self):
+    def size(self) -> int:
         return self.attrs.get('size')
 
     @property
-    def charset(self):
+    def charset(self) -> str:
         return self.attrs.get('charset')
 
     @property
-    def properties(self):
+    def properties(self) -> List[str]:
         return self.attrs.get('properties')
 
     @property
-    def alignment_attributes(self):
+    def alignment_attributes(self) -> AlignmentAttributeCollection:
         return AlignmentAttributeCollection(client=self.client, corpus=self)
 
     @property
-    def positional_attributes(self):
+    def positional_attributes(self) -> PositionalAttributeCollection:
         return PositionalAttributeCollection(client=self.client, corpus=self)
 
     @property
-    def structural_attributes(self):
+    def structural_attributes(self) -> StructuralAttributeCollection:
         return StructuralAttributeCollection(client=self.client, corpus=self)
 
     @property
-    def subcorpora(self):
+    def subcorpora(self) -> SubcorpusCollection:
         return SubcorpusCollection(client=self.client, corpus=self)
 
-    def drop(self):
+    def drop(self) -> 'StatusOk':
         return self.client.api.corpus_drop_corpus(self.api_name)
 
-    def query(self, subcorpus_name, query):
+    def query(self, subcorpus_name: str, query: str) -> 'StatusOk':
         return self.client.api.cqp_query(self.api_name, subcorpus_name, query)
 
 
 class CorpusCollection(Collection):
-    model = Corpus
+    model: Corpus = Corpus
 
-    def _get(self, corpus_name):
-        api_name = corpus_name
+    def _get(self, corpus_name: str) -> Dict:
+        api_name: str = corpus_name
         return {
             'api_name': corpus_name,
             'charset': self.client.api.corpus_charset(api_name),
             # 'full_name' = client.api.corpus_full_name(api_name),
             # 'info': client.api.corpus_info(api_name),
             'name': corpus_name,
             'properties': self.client.api.corpus_properties(api_name),
             'size': self.client.api.cl_attribute_size(f'{api_name}.word')
         }
 
-    def get(self, corpus_name):
+    def get(self, corpus_name: str) -> Corpus:
         return self.prepare_model(self._get(corpus_name))
 
-    def list(self):
-        return [self.prepare_model(self._get(x)) for x
-                in self.client.api.corpus_list_coprora()]
+    def list(self) -> List[Corpus]:
+        return [
+            self.prepare_model(self._get(x)) for x
+            in self.client.api.corpus_list_coprora()
+        ]
```

### Comparing `cqi-0.1.0/cqi/models/ressource.py` & `cqi-0.1.1/cqi/models/resource.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,88 @@
+from typing import Dict, List, TYPE_CHECKING
+if TYPE_CHECKING:
+    from ..client import CQiClient
+
+
 class Model:
-    """
+    '''
     A base class for representing a single object on the server.
-    """
-    id_attribute = 'Id'
+    '''
+    id_attribute: str = 'Id'
 
-    def __init__(self, attrs=None, client=None, collection=None):
+    def __init__(
+        self,
+        attrs: Dict = None,
+        client: 'CQiClient' = None,
+        collection: 'Collection' = None
+    ):
         #: A client pointing at the server that this object is on.
-        self.client = client
+        self.client: 'CQiClient' = client
 
         #: The collection that this model is part of.
-        self.collection = collection
+        self.collection: Collection = collection
 
         #: The raw representation of this object from the API
-        self.attrs = attrs or {}
+        self.attrs: Dict = attrs or {}
 
-    def __repr__(self):
-        return "<{}: {}>".format(self.__class__.__name__, self.id)
+    def __repr__(self) -> str:
+        return f'<{self.__class__.__name__}: {self.id}>'
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         return isinstance(other, self.__class__) and self.id == other.id
 
-    def __hash__(self):
-        return hash("{}:{}".format(self.__class__.__name__, self.id))
+    def __hash__(self) -> int:
+        return hash(f'{self.__class__.__name__}:{self.id}')
 
     @property
-    def id(self):
-        """
+    def id(self) -> str:
+        '''
         The ID of the object.
-        """
+        '''
         return self.attrs.get(self.id_attribute)
 
     def reload(self):
-        """
+        '''
         Load this object from the server again and update ``attrs`` with the
         new data.
-        """
-        new_model = self.collection.get(self.id)
-        self.attrs = new_model.attrs
+        '''
+        self.attrs = self.collection.get(self.id).attrs
 
 
 class Collection:
-    """
+    '''
     A base class for representing all objects of a particular type on the
     server.
-    """
+    '''
 
     #: The type of object this collection represents, set by subclasses
-    model = None
+    model: None = None
 
-    def __init__(self, client=None):
+    def __init__(self, client: 'CQiClient' = None):
         #: The client pointing at the server that this collection of objects
         #: is on.
-        self.client = client
+        self.client: 'CQiClient' = client
 
-    def list(self):
+    def list(self) -> List[Model]:
         raise NotImplementedError
 
-    def get(self, key):
+    def get(self, key) -> Model:
         raise NotImplementedError
 
-    def prepare_model(self, attrs):
-        """
+    def prepare_model(self, attrs) -> Model:
+        '''
         Create a model from a set of attributes.
-        """
+        '''
         if isinstance(attrs, Model):
             attrs.client = self.client
             attrs.collection = self
             return attrs
         elif isinstance(attrs, dict):
-            return self.model(attrs=attrs, client=self.client, collection=self)
+            return self.model(
+                attrs=attrs,
+                client=self.client,
+                collection=self
+            )
         else:
             raise Exception(
-                f'Can\'t create {self.model.__name__} from {attrs}')
+                f'Can\'t create {self.model.__name__} from {attrs}'
+            )
```

### Comparing `cqi-0.1.0/cqi.egg-info/PKG-INFO` & `cqi-0.1.1/cqi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-Metadata-Version: 2.1
-Name: cqi
-Version: 0.1.0
-Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
-Home-page: https://github.com/Pevtrick/cqi-py
-Author: Patrick Jentsch
-Author-email: patrickjentsch@gmx.net
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CQi SDK for Python
-
-A Python library for the [IMS Open Corpus Workbench](http://cwb.sourceforge.net/) (CWB) [corpus query interface](http://cwb.sourceforge.net/cqi.php) (CQi) API.
-
-## Installation
-
-The latest stable version [is available on PyPI](https://pypi.python.org/pypi/cqi/). Either add `cqi` to your `requirements.txt` file or install with pip:
-
-```
-pip install cqi
-```
-
-## Version compatibility
-
-| Package version | Protocol version |
-|-----------------|------------------|
-| 0.1.0           | 0.1              |
-
-## Usage
-
-```python
-import cqi
-
-
-client = cqi.CQiClient('127.0.0.1')
-client.connect(username='anonymous', password='') # 258 ~ CQI_STATUS_CONNECT_OK
-client.ping() # 260 ~ CQI_STATUS_PING_OK
-corpus = client.corpora.get('CORPUS') # <Corpus: CORPUS>
-corpus.query('"and" []* "the";', 'Results') # 257 ~ CQI_STATUS_OK
-results = corpus.subcorpora.get('Results') # <Subcorpus: CORPUS:Results>
-client.disconnect() # 259 ~ CQI_STATUS_BYE_OK
-```
-
-
+Metadata-Version: 2.1
+Name: cqi
+Version: 0.1.1
+Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
+Home-page: https://github.com/Pevtrick/cqi-py
+Author: Patrick Jentsch
+Author-email: patrickjentsch@gmx.net
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CQi SDK for Python
+
+A Python library for the [IMS Open Corpus Workbench](http://cwb.sourceforge.net/) (CWB) [Corpus Query Interface](https://cwb.sourceforge.io/documentation.php#cqi) (CQi) API.
+
+## Installation
+
+The latest stable version [is available on PyPI](https://pypi.python.org/pypi/cqi/). Either add `cqi` to your `requirements.txt` file or install with pip:
+
+```
+pip install cqi
+```
+
+## Version compatibility
+
+| Package version | Protocol version |
+|-----------------|------------------|
+| 0.1.0           | 0.1              |
+| 0.1.1           | 0.1              |
+
+## Usage
+
+```python
+import cqi
+
+
+client = cqi.CQiClient('127.0.0.1')
+client.connect(username='anonymous', password='') # <class 'cqi.status.StatusConnectOk'>
+client.ping() # <class 'cqi.status.StatusPingOk'>
+corpus = client.corpora.get('CORPUS') # <Corpus: CORPUS>
+corpus.query('"and" []* "the";', 'Results') # <class 'cqi.status.StatusOk'>
+results = corpus.subcorpora.get('Results') # <Subcorpus: CORPUS:Results>
+client.disconnect() # <class 'cqi.status.StatusByeOk'>
+```
```

### Comparing `cqi-0.1.0/setup.py` & `cqi-0.1.1/setup.py`

 * *Files identical despite different names*

