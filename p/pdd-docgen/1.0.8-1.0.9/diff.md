# Comparing `tmp/pdd_docgen-1.0.8-py2.py3-none-any.whl.zip` & `tmp/pdd_docgen-1.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 4788 bytes, number of entries: 11
+Zip file size: 4815 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      132 b- defN 18-Jan-03 21:05 docgen/__init__.py
 -rw-rw-r--  2.0 unx      129 b- defN 18-Jan-03 20:47 docgen/description.py
 -rw-rw-r--  2.0 unx     2000 b- defN 18-Jan-03 21:00 docgen/run.py
--rw-rw-r--  2.0 unx     3742 b- defN 18-Feb-10 20:44 docgen/system_tests.py
+-rw-rw-r--  2.0 unx     3883 b- defN 18-Feb-10 23:28 docgen/system_tests.py
 -rw-rw-r--  2.0 unx      746 b- defN 18-Jan-03 21:03 docgen/test_runner.py
--rw-rw-r--  2.0 unx       10 b- defN 18-Feb-10 20:49 pdd_docgen-1.0.8.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx      632 b- defN 18-Feb-10 20:49 pdd_docgen-1.0.8.dist-info/metadata.json
--rw-rw-r--  2.0 unx        7 b- defN 18-Feb-10 20:49 pdd_docgen-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      110 b- defN 18-Feb-10 20:49 pdd_docgen-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx      407 b- defN 18-Feb-10 20:49 pdd_docgen-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      890 b- defN 18-Feb-10 20:49 pdd_docgen-1.0.8.dist-info/RECORD
-11 files, 8805 bytes uncompressed, 3296 bytes compressed:  62.6%
+-rw-rw-r--  2.0 unx       10 b- defN 18-Feb-10 23:28 pdd_docgen-1.0.9.dist-info/DESCRIPTION.rst
+-rw-rw-r--  2.0 unx      632 b- defN 18-Feb-10 23:28 pdd_docgen-1.0.9.dist-info/metadata.json
+-rw-rw-r--  2.0 unx        7 b- defN 18-Feb-10 23:28 pdd_docgen-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      110 b- defN 18-Feb-10 23:28 pdd_docgen-1.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      407 b- defN 18-Feb-10 23:28 pdd_docgen-1.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      890 b- defN 18-Feb-10 23:28 pdd_docgen-1.0.9.dist-info/RECORD
+11 files, 8946 bytes uncompressed, 3323 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: docgen/system_tests.py
 Comment: 
 
 Filename: docgen/test_runner.py
 Comment: 
 
-Filename: pdd_docgen-1.0.8.dist-info/DESCRIPTION.rst
+Filename: pdd_docgen-1.0.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: pdd_docgen-1.0.8.dist-info/metadata.json
+Filename: pdd_docgen-1.0.9.dist-info/metadata.json
 Comment: 
 
-Filename: pdd_docgen-1.0.8.dist-info/top_level.txt
+Filename: pdd_docgen-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pdd_docgen-1.0.8.dist-info/WHEEL
+Filename: pdd_docgen-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pdd_docgen-1.0.8.dist-info/METADATA
+Filename: pdd_docgen-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pdd_docgen-1.0.8.dist-info/RECORD
+Filename: pdd_docgen-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docgen/system_tests.py

```diff
@@ -18,21 +18,24 @@
     def include_description(self, description):
         self._docgen_description = description
 
     def include_description_from(self, location):
         with open(location) as f:
             self.include_description(f.read())
 
+    def _add_auth(self, kwargs):
+        headers = kwargs.get("headers", {})
+        for key, value in self.default_headers.items():
+            headers[key] = value
+        kwargs["headers"] = headers
+
     def query(
             self, method, uri, expected_status_code=200, auth=True, **kwargs):
         if auth:
-            headers = kwargs.get("headers", {})
-            for key, value in self.default_headers.items():
-                headers[key] = value
-            kwargs["headers"] = headers
+            self._add_auth(kwargs)
 
         response = self.client.open(uri, method=method, **kwargs)
         actual_status_code = int(response.status.split(" ")[0])
 
         if callable(expected_status_code):
             self.assertTrue(expected_status_code(actual_status_code))
         else:
@@ -48,14 +51,17 @@
 
     def post(self, uri, expected_status_code=200, **kwargs):
         return self.query("POST", uri, expected_status_code, **kwargs)[0]
 
     def check_call(
             self, method, uri, auth=True, include_example=False,
             additional_validation=None, **kwargs):
+        if auth:
+            self._add_auth(kwargs)
+
         response, contents = self.query(
             method, uri, self._expected_status, auth, **kwargs)
 
         if additional_validation:
             self.assertTrue(additional_validation(response))
 
         if self._expected_contents is None or self._expected_contents == "":
@@ -73,14 +79,15 @@
         route, variables = self._find_route(method, uri)
         self.docgen["route"] = route
         self.docgen["method"] = method
 
         if include_example:
             self.docgen["example"] = {
                 "uri": uri,
+                "options": kwargs,
                 "response": actual_contents
             }
 
         if self._docgen_description:
             if isinstance(self._docgen_description, str):
                 self.docgen["summary"] = self._docgen_description
             else:
```

## Comparing `pdd_docgen-1.0.8.dist-info/metadata.json` & `pdd_docgen-1.0.9.dist-info/metadata.json`

 * *Files 0% similar despite different names*

### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'1.0.9'"}*

```diff
@@ -30,9 +30,9 @@
         {
             "requires": [
                 "requests (==2.18.4)"
             ]
         }
     ],
     "summary": "The test runner which generates API documentation by running tests, and an exporter of documentation to JSON format.",
-    "version": "1.0.8"
+    "version": "1.0.9"
 }
```

## Comparing `pdd_docgen-1.0.8.dist-info/RECORD` & `pdd_docgen-1.0.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 docgen/__init__.py,sha256=Noun0LQBHCTZRZBCqSSj54Gg1V7pTmT6tUXPhoKxFio,132
 docgen/description.py,sha256=6WCwhrBz6SjEqIE_ZXyL2Go4oK0lJ5FRoFvBdqPAA3U,129
 docgen/run.py,sha256=Kb0OlXo3mATaaCDXPrs3aCJ8zhJifW3Nfzk9RfwF7Rk,2000
-docgen/system_tests.py,sha256=2CLw_KhK4BUfHUeVfmfnv_0ntR23nq5u-G1AfAmfDCI,3742
+docgen/system_tests.py,sha256=Q1RFt6vx1HNil2xMfSHdPLlfUzqJoBzFGQuyq-Tye9E,3883
 docgen/test_runner.py,sha256=snSpY_sstzmcmQVwfhVldoNnzDaZDanL3YVbDR9AoxA,746
-pdd_docgen-1.0.8.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-pdd_docgen-1.0.8.dist-info/METADATA,sha256=BjbzkIlWcbrfExLBVd422tKjpNahowUzvyQAmdNqgt0,407
-pdd_docgen-1.0.8.dist-info/RECORD,,
-pdd_docgen-1.0.8.dist-info/WHEEL,sha256=kdsN-5OJAZIiHN-iO4Rhl82KyS0bDWf4uBwMbkNafr8,110
-pdd_docgen-1.0.8.dist-info/metadata.json,sha256=nju-L0Rfmdv2d9Dy9oqQUoSc-A0Qvn6y80qYmQCz1xE,632
-pdd_docgen-1.0.8.dist-info/top_level.txt,sha256=ow-Fj1rHRtV5_ySxXSRA2q32ZL__Gmpj0WieZ5_niXs,7
+pdd_docgen-1.0.9.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+pdd_docgen-1.0.9.dist-info/METADATA,sha256=1xboMxmaA8d5LPfLO9zoQIbFTOM0nNrsLwDXcZ8rA7E,407
+pdd_docgen-1.0.9.dist-info/RECORD,,
+pdd_docgen-1.0.9.dist-info/WHEEL,sha256=kdsN-5OJAZIiHN-iO4Rhl82KyS0bDWf4uBwMbkNafr8,110
+pdd_docgen-1.0.9.dist-info/metadata.json,sha256=dLDJ2lCkF8M2XGuoRZSqUOBhI2rc75S9Zp5rF89P-pk,632
+pdd_docgen-1.0.9.dist-info/top_level.txt,sha256=ow-Fj1rHRtV5_ySxXSRA2q32ZL__Gmpj0WieZ5_niXs,7
```

