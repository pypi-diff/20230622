# Comparing `tmp/msaDocModels-0.0.80.tar.gz` & `tmp/msaDocModels-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msaDocModels-0.0.80.tar", last modified: Thu Jun 22 08:21:29 2023, max compression
+gzip compressed data, was "msaDocModels-0.0.9.tar", last modified: Fri Nov 25 11:39:48 2022, max compression
```

## Comparing `msaDocModels-0.0.80.tar` & `msaDocModels-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-06-22 08:21:29.287775 msaDocModels-0.0.80/
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     1099 2023-03-17 10:04:49.000000 msaDocModels-0.0.80/LICENCE
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     3679 2023-06-22 08:21:29.287775 msaDocModels-0.0.80/PKG-INFO
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     2198 2023-03-17 10:04:49.000000 msaDocModels-0.0.80/README.md
-drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-06-22 08:21:29.287775 msaDocModels-0.0.80/msaDocModels/
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      479 2023-06-22 08:19:02.000000 msaDocModels-0.0.80/msaDocModels/__init__.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      562 2023-03-17 10:04:49.000000 msaDocModels-0.0.80/msaDocModels/health.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     3763 2023-03-17 10:04:49.000000 msaDocModels-0.0.80/msaDocModels/msg.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      409 2023-05-29 13:58:15.000000 msaDocModels-0.0.80/msaDocModels/openapi.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     2413 2023-03-17 10:04:49.000000 msaDocModels-0.0.80/msaDocModels/scheduler.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)   144423 2023-06-22 06:49:20.000000 msaDocModels-0.0.80/msaDocModels/sdu.py
-drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-06-22 08:21:29.287775 msaDocModels-0.0.80/msaDocModels/utils/
--rw-rw-r--   0 eduard    (1000) eduard    (1000)        0 2023-03-17 10:04:49.000000 msaDocModels-0.0.80/msaDocModels/utils/__init__.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     1826 2023-03-17 10:04:49.000000 msaDocModels-0.0.80/msaDocModels/utils/htmlutils.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)    22179 2023-03-17 10:42:12.000000 msaDocModels-0.0.80/msaDocModels/wdc.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     2103 2023-03-17 10:04:49.000000 msaDocModels-0.0.80/msaDocModels/wfl.py
-drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-06-22 08:21:29.287775 msaDocModels-0.0.80/msaDocModels.egg-info/
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     3679 2023-06-22 08:21:29.000000 msaDocModels-0.0.80/msaDocModels.egg-info/PKG-INFO
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      442 2023-06-22 08:21:29.000000 msaDocModels-0.0.80/msaDocModels.egg-info/SOURCES.txt
--rw-rw-r--   0 eduard    (1000) eduard    (1000)        1 2023-06-22 08:21:29.000000 msaDocModels-0.0.80/msaDocModels.egg-info/dependency_links.txt
--rw-rw-r--   0 eduard    (1000) eduard    (1000)       13 2023-06-22 08:21:29.000000 msaDocModels-0.0.80/msaDocModels.egg-info/top_level.txt
--rw-rw-r--   0 eduard    (1000) eduard    (1000)        1 2023-06-22 08:21:29.000000 msaDocModels-0.0.80/msaDocModels.egg-info/zip-safe
--rw-rw-r--   0 eduard    (1000) eduard    (1000)       38 2023-06-22 08:21:29.287775 msaDocModels-0.0.80/setup.cfg
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     2164 2023-03-17 10:04:49.000000 msaDocModels-0.0.80/setup.py
+drwxrwxr-x   0 vitaliy   (1000) vitaliy   (1000)        0 2022-11-25 11:39:48.407721 msaDocModels-0.0.9/
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     1099 2022-11-09 11:53:39.000000 msaDocModels-0.0.9/LICENCE
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     3633 2022-11-25 11:39:48.407721 msaDocModels-0.0.9/PKG-INFO
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     2153 2022-11-09 11:53:39.000000 msaDocModels-0.0.9/README.md
+drwxrwxr-x   0 vitaliy   (1000) vitaliy   (1000)        0 2022-11-25 11:39:48.407721 msaDocModels-0.0.9/msaDocModels/
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)      484 2022-11-25 11:38:58.000000 msaDocModels-0.0.9/msaDocModels/__init__.py
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)      562 2022-11-18 16:38:17.000000 msaDocModels-0.0.9/msaDocModels/health.py
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     3731 2022-11-09 11:53:39.000000 msaDocModels-0.0.9/msaDocModels/msg.py
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)      387 2022-11-22 10:24:03.000000 msaDocModels-0.0.9/msaDocModels/openapi.py
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     2412 2022-11-18 16:38:17.000000 msaDocModels-0.0.9/msaDocModels/scheduler.py
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)    13177 2022-11-25 11:19:58.000000 msaDocModels-0.0.9/msaDocModels/sdu.py
+drwxrwxr-x   0 vitaliy   (1000) vitaliy   (1000)        0 2022-11-25 11:39:48.407721 msaDocModels-0.0.9/msaDocModels/utils/
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)        0 2022-11-21 13:25:40.000000 msaDocModels-0.0.9/msaDocModels/utils/__init__.py
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     1825 2022-11-10 09:04:48.000000 msaDocModels-0.0.9/msaDocModels/utils/htmlutils.py
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)    22525 2022-11-09 11:53:39.000000 msaDocModels-0.0.9/msaDocModels/wdc.py
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     2209 2022-11-09 11:53:39.000000 msaDocModels-0.0.9/msaDocModels/wfl.py
+drwxrwxr-x   0 vitaliy   (1000) vitaliy   (1000)        0 2022-11-25 11:39:48.407721 msaDocModels-0.0.9/msaDocModels.egg-info/
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     3633 2022-11-25 11:39:48.000000 msaDocModels-0.0.9/msaDocModels.egg-info/PKG-INFO
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)      442 2022-11-25 11:39:48.000000 msaDocModels-0.0.9/msaDocModels.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)        1 2022-11-25 11:39:48.000000 msaDocModels-0.0.9/msaDocModels.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)       13 2022-11-25 11:39:48.000000 msaDocModels-0.0.9/msaDocModels.egg-info/top_level.txt
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)        1 2022-11-18 15:00:50.000000 msaDocModels-0.0.9/msaDocModels.egg-info/zip-safe
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)       38 2022-11-25 11:39:48.407721 msaDocModels-0.0.9/setup.cfg
+-rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     2154 2022-11-09 11:53:39.000000 msaDocModels-0.0.9/setup.py
```

### Comparing `msaDocModels-0.0.80/LICENCE` & `msaDocModels-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `msaDocModels-0.0.80/PKG-INFO` & `msaDocModels-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msaDocModels
-Version: 0.0.80
+Version: 0.0.9
 Summary: msaDocModels - MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and AI results for processed documents
 Home-page: https://github.com/swelcker/msaDocModels
 Download-URL: http://pypi.python.org/pypi/msaDocModels
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
 Project-URL: Documentation, http://msaDocModels.u2d.ai/
@@ -55,15 +55,14 @@
 
 ------
 
 ## Features
 - **Schema/Models for Document Understanding Result Data**: sdu.
 - **Schema/Models for General Document Handling Data**: wdc.
 - **Schema/Models for Workflow Definition and Processing Data**: wfl.
-- **Schema/Models for Work With Text**: spk.
 - **API Message class**: msg, allows generic API JSON message creation with capabilities to re-create original datatypes and class instances.
 
 
 ## Main Dependencies
 
 - msaUtils >= 0.0.2
 - Pydantic
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: msaDocModels Version: 0.0.80 Summary: msaDocModels
-- MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and
-AI results for processed documents Home-page: https://github.com/swelcker/
+Metadata-Version: 2.1 Name: msaDocModels Version: 0.0.9 Summary: msaDocModels -
+MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and AI
+results for processed documents Home-page: https://github.com/swelcker/
 msaDocModels Download-URL: http://pypi.python.org/pypi/msaDocModels Author:
 Stefan Welcker Author-email: stefan@u2d.ai License: MIT Project-URL:
 Documentation, http://msaDocModels.u2d.ai/ Project-URL: Source, https://
 github.com/swelcker/msaDocModels Project-URL: Tracker, https://github.com/
 swelcker/msaDocModels/issues Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: FastAPI Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -24,22 +24,21 @@
                NLP, NLU and AI results for processed documents
                    Optimized for use with FastAPI/Pydantic.
                  [Package_version] [Supported_Python_versions]
 ------ **Documentation**: msaDocModels_Documentation_(https://
 msaDocModels.u2d.ai/) ------ ## Features - **Schema/Models for Document
 Understanding Result Data**: sdu. - **Schema/Models for General Document
 Handling Data**: wdc. - **Schema/Models for Workflow Definition and Processing
-Data**: wfl. - **Schema/Models for Work With Text**: spk. - **API Message
-class**: msg, allows generic API JSON message creation with capabilities to re-
-create original datatypes and class instances. ## Main Dependencies - msaUtils
->= 0.0.2 - Pydantic ## License Agreement - `msaDocModels` is based on `MIT`
-open source and free to use, it is free for commercial use, but please show/
-list the copyright information about msaDocModels somewhere. ## How to create
-the documentation We use mkdocs and mkdocsstring. The code reference and nav
-entry get's created virtually by the triggered python script /docs/
-gen_ref_pages.py while ``mkdocs`` ``serve`` or ``build`` is executed. ###
-Requirements Install for the PDF creation option: PDF Export is using mainly
-weasyprint, if you get some errors here pls. check there documentation.
-Installation is part of the msaDocModels, so this should be fine. We can now
-test and view our documentation using: mkdocs serve Build static Site: mkdocs
-build ## Build and Publish Build: python setup.py sdist Publish to pypi: twine
-upload dist/*
+Data**: wfl. - **API Message class**: msg, allows generic API JSON message
+creation with capabilities to re-create original datatypes and class instances.
+## Main Dependencies - msaUtils >= 0.0.2 - Pydantic ## License Agreement -
+`msaDocModels` is based on `MIT` open source and free to use, it is free for
+commercial use, but please show/list the copyright information about
+msaDocModels somewhere. ## How to create the documentation We use mkdocs and
+mkdocsstring. The code reference and nav entry get's created virtually by the
+triggered python script /docs/gen_ref_pages.py while ``mkdocs`` ``serve`` or
+``build`` is executed. ### Requirements Install for the PDF creation option:
+PDF Export is using mainly weasyprint, if you get some errors here pls. check
+there documentation. Installation is part of the msaDocModels, so this should
+be fine. We can now test and view our documentation using: mkdocs serve Build
+static Site: mkdocs build ## Build and Publish Build: python setup.py sdist
+Publish to pypi: twine upload dist/*
```

### Comparing `msaDocModels-0.0.80/README.md` & `msaDocModels-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 ------
 
 ## Features
 - **Schema/Models for Document Understanding Result Data**: sdu.
 - **Schema/Models for General Document Handling Data**: wdc.
 - **Schema/Models for Workflow Definition and Processing Data**: wfl.
-- **Schema/Models for Work With Text**: spk.
 - **API Message class**: msg, allows generic API JSON message creation with capabilities to re-create original datatypes and class instances.
 
 
 ## Main Dependencies
 
 - msaUtils >= 0.0.2
 - Pydantic
```

#### html2text {}

```diff
@@ -4,22 +4,21 @@
                NLP, NLU and AI results for processed documents
                    Optimized for use with FastAPI/Pydantic.
                  [Package_version] [Supported_Python_versions]
 ------ **Documentation**: msaDocModels_Documentation_(https://
 msaDocModels.u2d.ai/) ------ ## Features - **Schema/Models for Document
 Understanding Result Data**: sdu. - **Schema/Models for General Document
 Handling Data**: wdc. - **Schema/Models for Workflow Definition and Processing
-Data**: wfl. - **Schema/Models for Work With Text**: spk. - **API Message
-class**: msg, allows generic API JSON message creation with capabilities to re-
-create original datatypes and class instances. ## Main Dependencies - msaUtils
->= 0.0.2 - Pydantic ## License Agreement - `msaDocModels` is based on `MIT`
-open source and free to use, it is free for commercial use, but please show/
-list the copyright information about msaDocModels somewhere. ## How to create
-the documentation We use mkdocs and mkdocsstring. The code reference and nav
-entry get's created virtually by the triggered python script /docs/
-gen_ref_pages.py while ``mkdocs`` ``serve`` or ``build`` is executed. ###
-Requirements Install for the PDF creation option: PDF Export is using mainly
-weasyprint, if you get some errors here pls. check there documentation.
-Installation is part of the msaDocModels, so this should be fine. We can now
-test and view our documentation using: mkdocs serve Build static Site: mkdocs
-build ## Build and Publish Build: python setup.py sdist Publish to pypi: twine
-upload dist/*
+Data**: wfl. - **API Message class**: msg, allows generic API JSON message
+creation with capabilities to re-create original datatypes and class instances.
+## Main Dependencies - msaUtils >= 0.0.2 - Pydantic ## License Agreement -
+`msaDocModels` is based on `MIT` open source and free to use, it is free for
+commercial use, but please show/list the copyright information about
+msaDocModels somewhere. ## How to create the documentation We use mkdocs and
+mkdocsstring. The code reference and nav entry get's created virtually by the
+triggered python script /docs/gen_ref_pages.py while ``mkdocs`` ``serve`` or
+``build`` is executed. ### Requirements Install for the PDF creation option:
+PDF Export is using mainly weasyprint, if you get some errors here pls. check
+there documentation. Installation is part of the msaDocModels, so this should
+be fine. We can now test and view our documentation using: mkdocs serve Build
+static Site: mkdocs build ## Build and Publish Build: python setup.py sdist
+Publish to pypi: twine upload dist/*
```

### Comparing `msaDocModels-0.0.80/msaDocModels/health.py` & `msaDocModels-0.0.9/msaDocModels/health.py`

 * *Files identical despite different names*

### Comparing `msaDocModels-0.0.80/msaDocModels/msg.py` & `msaDocModels-0.0.9/msaDocModels/msg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 import dataclasses
 import datetime
 from dataclasses import dataclass
-from typing import Generic, Type, TypeVar
 
 from genson import SchemaBuilder
 from pydantic.types import UUID
+from typing import Generic, TypeVar, Type
 
-_T = TypeVar("_T")
+_T = TypeVar('_T')
 
 try:
     import orjson as json
 except:
     try:
         import ujson as json
 
     except:
         import json
-
         json.__version__ = ""
 
 
 import uuid
-from typing import List, Optional, Union
+from typing import Union, List, Optional
 
 from fastapi.encoders import jsonable_encoder
 from pydantic import BaseModel
 
 
 class titem(BaseModel):
     item_me: str = "Stefan"
 
 
 class test(BaseModel):
     info: str = "some information"
-    test_list: List[str] = ["a", "list"]
+    test_list: List[str] = ['a', 'list']
     test_item: titem = titem()
     test_item_list: List[titem] = [titem()]
     test_optional_item: Optional[titem] = None
     test_date: datetime.datetime = datetime.datetime.utcnow()
 
 
 class Metadata(BaseModel):
@@ -47,32 +46,33 @@
     created_at: datetime.datetime = datetime.datetime.utcnow()
     json_module: str = json.__name__
     json_version: str = json.__version__
     metaclass: str = ""
 
 
 class MSAAPIMessage:
+
     def __init__(self, metaClass: _T = Metadata, **kwargs):
         self.__dict__ = kwargs
         self.metadata: metaClass = metaClass()
         self.metadata.metaclass = metaClass.__name__
 
     def toDict(self) -> dict:
         return jsonable_encoder(self.__dict__)
 
     def fromDict(self, msg: dict):
         self.__dict__ = msg
 
     def toMsg(self) -> str:
-        classes = {}
+        classes={}
         for k, v in self.__dict__.items():
             classes[k] = v.__class__.__name__
-            # print("TOMSG:",k,v, type(v), v.__class__.__name__)
+            #print("TOMSG:",k,v, type(v), v.__class__.__name__)
         self.__dict__["classes"] = classes
-        return json.dumps(self, default=lambda x: jsonable_encoder(x.__dict__)).decode("utf8").replace("'", '"')
+        return json.dumps(self, default=lambda x: jsonable_encoder(x.__dict__)).decode('utf8').replace("'", '"')
 
     def fromMsg(self, message: str):
         self.__dict__ = json.loads(message)
 
     def fromMsgToClasses(self, message: str):
         self.fromMsg(message=message)
         if "metaclass" in self.metadata.keys():
@@ -94,19 +94,15 @@
     def schema_json(self) -> str:
         builder = SchemaBuilder()
         builder.add_object(self.toDict())
         return builder.to_json()
 
 
 if __name__ == "__main__":
-    m = MSAAPIMessage(
-        info="some information",
-        mylist=["a", "list"],
-        test=test(),
-    )
+    m = MSAAPIMessage(info="some information", mylist=['a', 'list'], test=test(), )
 
     print("m todict:", m.toDict())
     print("m tomsg:", m.toMsg())
     print("m str:", m.__str__())
     print("m api:", jsonable_encoder(m))
     print("m rep:", m.__repr__())
     print("m cls:", m.__class__)
```

### Comparing `msaDocModels-0.0.80/msaDocModels/scheduler.py` & `msaDocModels-0.0.9/msaDocModels/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
 from typing import Any, List, Optional, Union
-
 from pydantic import BaseModel
 
 
 class MSASchedulerRepoLogRecord(BaseModel):
     """**MSASchedulerRepoLogRecord** Pydantic Response Class"""
 
     task_name: str
```

### Comparing `msaDocModels-0.0.80/msaDocModels/utils/htmlutils.py` & `msaDocModels-0.0.9/msaDocModels/utils/htmlutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 from typing import Any, Optional
-
 from lxml.html.clean import Cleaner
 
 
 async def sanitize(dirty_html: Any) -> Optional[str]:
     """Clean/Sanitize HTML using lxml.html.clean.Cleaner
 
     Cleans the following:
```

### Comparing `msaDocModels-0.0.80/msaDocModels/wdc.py` & `msaDocModels-0.0.9/msaDocModels/wdc.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,17 @@
         lst = syn.entailments()
         self.entailments = [entry.name() for entry in lst]
         # sees
         lst = syn.also_sees()
         self.sees = [entry.name() for entry in lst]
         # domains
         lst = syn.topic_domains()
-        self.domains = [entry.name() for entry in lst if entry.name() not in self.domains]
+        self.domains = [
+            entry.name() for entry in lst if entry.name() not in self.domains
+        ]
         # root
         rn = syn.root_hypernyms()
         if len(rn) > 0:
             for rentry in rn:
                 if len(self.root) > 1:
                     self.root += "/"
                 self.root += str(rentry.name()).split(".")[0]
@@ -195,36 +197,56 @@
 
             self.ssid = str(syn.id)
             # lemmas
             self.lemmas = syn.lemmas()
 
             # hypernyms
             lst = syn.get_related("hypernym")
-            self.hypernyms.extend([nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0])
-            self.hypernyms.extend([nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0])
+            self.hypernyms.extend(
+                [nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0]
+            )
+            self.hypernyms.extend(
+                [nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0]
+            )
 
             # hyponyms
             lst = syn.get_related("hyponym")
-            self.hyponyms.extend([nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0])
-            self.hyponyms.extend([nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0])
+            self.hyponyms.extend(
+                [nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0]
+            )
+            self.hyponyms.extend(
+                [nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0]
+            )
 
             # holonyms
             lst = syn.get_related("holo_member")
-            self.holonyms.extend([nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0])
-            self.holonyms.extend([nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0])
+            self.holonyms.extend(
+                [nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0]
+            )
+            self.holonyms.extend(
+                [nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0]
+            )
 
             # meronyms
             lst = syn.get_related("mero_member")
-            self.meronyms.extend([nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0])
-            self.meronyms.extend([nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0])
+            self.meronyms.extend(
+                [nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0]
+            )
+            self.meronyms.extend(
+                [nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0]
+            )
 
             # entailments
             lst = syn.get_related("entails")
-            self.entailments.extend([nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0])
-            self.entailments.extend([nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0])
+            self.entailments.extend(
+                [nentry.lemmas()[0] for nentry in lst if len(nentry.lemmas()) > 0]
+            )
+            self.entailments.extend(
+                [nentry.words()[0].lemma() for nentry in lst if len(nentry.words()) > 0]
+            )
 
             # root
             rn = syn.hypernyms()
             if len(rn) > 0:
                 for nentry in rn:
                     if len(self.root) > 1:
                         self.root += "/"
@@ -369,15 +391,17 @@
         ret += (
             "<span><i><small><strong>Description</strong></small></i><hr><i><h6>"
             + html.escape(self.description.capitalize())
             + "<h6></i></span>"
         )
         # ret += "<hr>"
         ret += (
-            "<span><i><small><strong>Node</strong></small></i><hr><h6>" + html.escape(self.get_tree()) + "</h6></span>"
+            "<span><i><small><strong>Node</strong></small></i><hr><h6>"
+            + html.escape(self.get_tree())
+            + "</h6></span>"
         )
         ret += (
             "<span><i><small><strong>Tree</strong></small></i><hr><h6>"
             + html.escape(self.get_root_tree_names()).replace("\n", "<br><br>")
             + "</h6></span>"
         )
         # ret += "<hr>"
```

### Comparing `msaDocModels-0.0.80/msaDocModels/wfl.py` & `msaDocModels-0.0.9/msaDocModels/wfl.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,30 +27,60 @@
     class Config:
         orm_mode = False
 
 
 list_node_modules: List[WFLModule] = []
 list_node_types: List[WFLNodeType] = []
 
-list_node_modules.append(WFLModule(id=1, short="collect", name="Collect", description="", step="10000"))
-list_node_modules.append(WFLModule(id=2, short="convert", name="Convert", description="", step="20000"))
-list_node_modules.append(WFLModule(id=3, short="preprocessing", name="Pre-Processing", description="", step="30000"))
-list_node_modules.append(WFLModule(id=4, short="processing", name="Processing", description="", step="50000"))
+list_node_modules.append(
+    WFLModule(id=1, short="collect", name="Collect", description="", step="10000")
+)
+list_node_modules.append(
+    WFLModule(id=2, short="convert", name="Convert", description="", step="20000")
+)
+list_node_modules.append(
+    WFLModule(
+        id=3, short="preprocessing", name="Pre-Processing", description="", step="30000"
+    )
+)
+list_node_modules.append(
+    WFLModule(id=4, short="processing", name="Processing", description="", step="50000")
+)
 list_node_modules.append(
     WFLModule(
         id=5,
         short="postprocessing",
         name="Post-Processing",
         description="",
         step="70000",
     )
 )
-list_node_modules.append(WFLModule(id=6, short="format", name="Format", description="", step="80000"))
-list_node_modules.append(WFLModule(id=7, short="push", name="Push", description="", step="90000"))
+list_node_modules.append(
+    WFLModule(id=6, short="format", name="Format", description="", step="80000")
+)
+list_node_modules.append(
+    WFLModule(id=7, short="push", name="Push", description="", step="90000")
+)
 
-list_node_types.append(WFLNodeType(id=1, short="input", name="Input", description="", step="10000"))
-list_node_types.append(WFLNodeType(id=2, short="triggers", name="Triggers", description="", step="20000"))
-list_node_types.append(WFLNodeType(id=3, short="processors", name="Processors", description="", step="30000"))
-list_node_types.append(WFLNodeType(id=4, short="operators", name="Operators", description="", step="50000"))
-list_node_types.append(WFLNodeType(id=5, short="actions", name="Actions", description="", step="70000"))
-list_node_types.append(WFLNodeType(id=6, short="models", name="Models", description="", step="80000"))
-list_node_types.append(WFLNodeType(id=7, short="output", name="Output", description="", step="90000"))
+list_node_types.append(
+    WFLNodeType(id=1, short="input", name="Input", description="", step="10000")
+)
+list_node_types.append(
+    WFLNodeType(id=2, short="triggers", name="Triggers", description="", step="20000")
+)
+list_node_types.append(
+    WFLNodeType(
+        id=3, short="processors", name="Processors", description="", step="30000"
+    )
+)
+list_node_types.append(
+    WFLNodeType(id=4, short="operators", name="Operators", description="", step="50000")
+)
+list_node_types.append(
+    WFLNodeType(id=5, short="actions", name="Actions", description="", step="70000")
+)
+list_node_types.append(
+    WFLNodeType(id=6, short="models", name="Models", description="", step="80000")
+)
+list_node_types.append(
+    WFLNodeType(id=7, short="output", name="Output", description="", step="90000")
+)
```

### Comparing `msaDocModels-0.0.80/msaDocModels.egg-info/PKG-INFO` & `msaDocModels-0.0.9/msaDocModels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msaDocModels
-Version: 0.0.80
+Version: 0.0.9
 Summary: msaDocModels - MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and AI results for processed documents
 Home-page: https://github.com/swelcker/msaDocModels
 Download-URL: http://pypi.python.org/pypi/msaDocModels
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
 Project-URL: Documentation, http://msaDocModels.u2d.ai/
@@ -55,15 +55,14 @@
 
 ------
 
 ## Features
 - **Schema/Models for Document Understanding Result Data**: sdu.
 - **Schema/Models for General Document Handling Data**: wdc.
 - **Schema/Models for Workflow Definition and Processing Data**: wfl.
-- **Schema/Models for Work With Text**: spk.
 - **API Message class**: msg, allows generic API JSON message creation with capabilities to re-create original datatypes and class instances.
 
 
 ## Main Dependencies
 
 - msaUtils >= 0.0.2
 - Pydantic
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: msaDocModels Version: 0.0.80 Summary: msaDocModels
-- MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and
-AI results for processed documents Home-page: https://github.com/swelcker/
+Metadata-Version: 2.1 Name: msaDocModels Version: 0.0.9 Summary: msaDocModels -
+MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and AI
+results for processed documents Home-page: https://github.com/swelcker/
 msaDocModels Download-URL: http://pypi.python.org/pypi/msaDocModels Author:
 Stefan Welcker Author-email: stefan@u2d.ai License: MIT Project-URL:
 Documentation, http://msaDocModels.u2d.ai/ Project-URL: Source, https://
 github.com/swelcker/msaDocModels Project-URL: Tracker, https://github.com/
 swelcker/msaDocModels/issues Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: FastAPI Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -24,22 +24,21 @@
                NLP, NLU and AI results for processed documents
                    Optimized for use with FastAPI/Pydantic.
                  [Package_version] [Supported_Python_versions]
 ------ **Documentation**: msaDocModels_Documentation_(https://
 msaDocModels.u2d.ai/) ------ ## Features - **Schema/Models for Document
 Understanding Result Data**: sdu. - **Schema/Models for General Document
 Handling Data**: wdc. - **Schema/Models for Workflow Definition and Processing
-Data**: wfl. - **Schema/Models for Work With Text**: spk. - **API Message
-class**: msg, allows generic API JSON message creation with capabilities to re-
-create original datatypes and class instances. ## Main Dependencies - msaUtils
->= 0.0.2 - Pydantic ## License Agreement - `msaDocModels` is based on `MIT`
-open source and free to use, it is free for commercial use, but please show/
-list the copyright information about msaDocModels somewhere. ## How to create
-the documentation We use mkdocs and mkdocsstring. The code reference and nav
-entry get's created virtually by the triggered python script /docs/
-gen_ref_pages.py while ``mkdocs`` ``serve`` or ``build`` is executed. ###
-Requirements Install for the PDF creation option: PDF Export is using mainly
-weasyprint, if you get some errors here pls. check there documentation.
-Installation is part of the msaDocModels, so this should be fine. We can now
-test and view our documentation using: mkdocs serve Build static Site: mkdocs
-build ## Build and Publish Build: python setup.py sdist Publish to pypi: twine
-upload dist/*
+Data**: wfl. - **API Message class**: msg, allows generic API JSON message
+creation with capabilities to re-create original datatypes and class instances.
+## Main Dependencies - msaUtils >= 0.0.2 - Pydantic ## License Agreement -
+`msaDocModels` is based on `MIT` open source and free to use, it is free for
+commercial use, but please show/list the copyright information about
+msaDocModels somewhere. ## How to create the documentation We use mkdocs and
+mkdocsstring. The code reference and nav entry get's created virtually by the
+triggered python script /docs/gen_ref_pages.py while ``mkdocs`` ``serve`` or
+``build`` is executed. ### Requirements Install for the PDF creation option:
+PDF Export is using mainly weasyprint, if you get some errors here pls. check
+there documentation. Installation is part of the msaDocModels, so this should
+be fine. We can now test and view our documentation using: mkdocs serve Build
+static Site: mkdocs build ## Build and Publish Build: python setup.py sdist
+Publish to pypi: twine upload dist/*
```

