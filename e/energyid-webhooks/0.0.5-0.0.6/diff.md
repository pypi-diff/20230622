# Comparing `tmp/energyid-webhooks-0.0.5.tar.gz` & `tmp/energyid-webhooks-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyid-webhooks-0.0.5.tar", last modified: Wed Jun 21 11:48:45 2023, max compression
+gzip compressed data, was "energyid-webhooks-0.0.6.tar", last modified: Thu Jun 22 08:46:57 2023, max compression
```

## Comparing `energyid-webhooks-0.0.5.tar` & `energyid-webhooks-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-21 11:48:45.087475 energyid-webhooks-0.0.5/
--rw-r--r--   0 Jan        (504) staff       (20)     1074 2023-06-16 12:54:48.000000 energyid-webhooks-0.0.5/LICENSE
--rw-r--r--   0 Jan        (504) staff       (20)     2131 2023-06-21 11:48:45.087563 energyid-webhooks-0.0.5/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)     1574 2023-06-16 13:26:52.000000 energyid-webhooks-0.0.5/README.md
--rw-r--r--   0 Jan        (504) staff       (20)      103 2023-06-16 12:57:53.000000 energyid-webhooks-0.0.5/pyproject.toml
--rw-r--r--   0 Jan        (504) staff       (20)      720 2023-06-21 11:48:45.087951 energyid-webhooks-0.0.5/setup.cfg
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-21 11:48:45.083947 energyid-webhooks-0.0.5/src/
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-21 11:48:45.086206 energyid-webhooks-0.0.5/src/energyid_webhooks/
--rw-r--r--   0 Jan        (504) staff       (20)      111 2023-06-21 11:47:53.000000 energyid-webhooks-0.0.5/src/energyid_webhooks/__init__.py
--rw-r--r--   0 Jan        (504) staff       (20)     3038 2023-06-20 16:26:24.000000 energyid-webhooks-0.0.5/src/energyid_webhooks/client.py
--rw-r--r--   0 Jan        (504) staff       (20)     1393 2023-06-20 13:53:31.000000 energyid-webhooks-0.0.5/src/energyid_webhooks/metercatalog.py
--rw-r--r--   0 Jan        (504) staff       (20)     1123 2023-06-21 11:45:04.000000 energyid-webhooks-0.0.5/src/energyid_webhooks/payload.py
--rw-r--r--   0 Jan        (504) staff       (20)     1451 2023-06-20 16:28:19.000000 energyid-webhooks-0.0.5/src/energyid_webhooks/webhookpolicy.py
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-21 11:48:45.087309 energyid-webhooks-0.0.5/src/energyid_webhooks.egg-info/
--rw-r--r--   0 Jan        (504) staff       (20)     2131 2023-06-21 11:48:45.000000 energyid-webhooks-0.0.5/src/energyid_webhooks.egg-info/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)      442 2023-06-21 11:48:45.000000 energyid-webhooks-0.0.5/src/energyid_webhooks.egg-info/SOURCES.txt
--rw-r--r--   0 Jan        (504) staff       (20)        1 2023-06-21 11:48:45.000000 energyid-webhooks-0.0.5/src/energyid_webhooks.egg-info/dependency_links.txt
--rw-r--r--   0 Jan        (504) staff       (20)       17 2023-06-21 11:48:45.000000 energyid-webhooks-0.0.5/src/energyid_webhooks.egg-info/requires.txt
--rw-r--r--   0 Jan        (504) staff       (20)       18 2023-06-21 11:48:45.000000 energyid-webhooks-0.0.5/src/energyid_webhooks.egg-info/top_level.txt
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-22 08:46:57.718862 energyid-webhooks-0.0.6/
+-rw-r--r--   0 Jan        (504) staff       (20)     1074 2023-06-16 12:54:48.000000 energyid-webhooks-0.0.6/LICENSE
+-rw-r--r--   0 Jan        (504) staff       (20)     2131 2023-06-22 08:46:57.719011 energyid-webhooks-0.0.6/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)     1574 2023-06-16 13:26:52.000000 energyid-webhooks-0.0.6/README.md
+-rw-r--r--   0 Jan        (504) staff       (20)      103 2023-06-16 12:57:53.000000 energyid-webhooks-0.0.6/pyproject.toml
+-rw-r--r--   0 Jan        (504) staff       (20)      720 2023-06-22 08:46:57.721072 energyid-webhooks-0.0.6/setup.cfg
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-22 08:46:57.708435 energyid-webhooks-0.0.6/src/
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-22 08:46:57.712905 energyid-webhooks-0.0.6/src/energyid_webhooks/
+-rw-r--r--   0 Jan        (504) staff       (20)      149 2023-06-22 08:46:17.000000 energyid-webhooks-0.0.6/src/energyid_webhooks/__init__.py
+-rw-r--r--   0 Jan        (504) staff       (20)     4121 2023-06-22 08:46:17.000000 energyid-webhooks-0.0.6/src/energyid_webhooks/client.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2162 2023-06-22 08:46:17.000000 energyid-webhooks-0.0.6/src/energyid_webhooks/metercatalog.py
+-rw-r--r--   0 Jan        (504) staff       (20)     1238 2023-06-22 08:46:17.000000 energyid-webhooks-0.0.6/src/energyid_webhooks/payload.py
+-rw-r--r--   0 Jan        (504) staff       (20)     1791 2023-06-22 08:46:17.000000 energyid-webhooks-0.0.6/src/energyid_webhooks/webhookpolicy.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-22 08:46:57.717688 energyid-webhooks-0.0.6/src/energyid_webhooks.egg-info/
+-rw-r--r--   0 Jan        (504) staff       (20)     2131 2023-06-22 08:46:57.000000 energyid-webhooks-0.0.6/src/energyid_webhooks.egg-info/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)      442 2023-06-22 08:46:57.000000 energyid-webhooks-0.0.6/src/energyid_webhooks.egg-info/SOURCES.txt
+-rw-r--r--   0 Jan        (504) staff       (20)        1 2023-06-22 08:46:57.000000 energyid-webhooks-0.0.6/src/energyid_webhooks.egg-info/dependency_links.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       17 2023-06-22 08:46:57.000000 energyid-webhooks-0.0.6/src/energyid_webhooks.egg-info/requires.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       18 2023-06-22 08:46:57.000000 energyid-webhooks-0.0.6/src/energyid_webhooks.egg-info/top_level.txt
```

### Comparing `energyid-webhooks-0.0.5/LICENSE` & `energyid-webhooks-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `energyid-webhooks-0.0.5/PKG-INFO` & `energyid-webhooks-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyid-webhooks
-Version: 0.0.5
+Version: 0.0.6
 Summary: Light weight python package to interface with EnergyID webhooks
 Home-page: https://api.energyid.eu/docs.html#webhook
 Author: Jan Pecinovsky
 Author-email: jan@energieid.be
 Project-URL: Bug Tracker, https://github.com/EnergieID/energyid-webhooks-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `energyid-webhooks-0.0.5/README.md` & `energyid-webhooks-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `energyid-webhooks-0.0.5/setup.cfg` & `energyid-webhooks-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = energyid-webhooks
-version = 0.0.5
+version = 0.0.6
 author = Jan Pecinovsky
 author_email = jan@energieid.be
 description = Light weight python package to interface with EnergyID webhooks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://api.energyid.eu/docs.html#webhook
 project_urls =
```

### Comparing `energyid-webhooks-0.0.5/src/energyid_webhooks/webhookpolicy.py` & `energyid-webhooks-0.0.6/src/energyid_webhooks/webhookpolicy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,66 @@
+"""Objects for representing webhook policies."""
+
 from typing import Dict, List
 
+
 class WebhookPolicy:
-    def __init__(self, policy: Dict):
+    """Object representation of a webhook policy."""
+
+    def __init__(self, policy: Dict) -> None:
         self.policy = policy
-    
+
     @property
     def allowed_metrics(self) -> List[str]:
-        return self.policy['allowedMetrics']
-    
+        """Get the allowed metrics for this policy."""
+        return self.policy["allowedMetrics"]
+
     @property
     def allowed_interval(self) -> str:
-        return self.policy['allowedInterval']
-    
+        """Get the shortest allowed interval for this policy."""
+        return self.policy["allowedInterval"]
+
     @property
     def description(self) -> str:
-        return self.policy['description']
-    
+        """Get the description of this policy."""
+        return self.policy["description"]
+
     @property
     def display_name(self) -> str:
-        return self.policy['displayName']
-    
+        """Get the display name of this policy."""
+        return self.policy["displayName"]
+
     def __repr__(self):
         return str(self.policy)
-    
+
     def __str__(self):
         return self.__repr__()
-    
+
     def __eq__(self, other):
         return self.policy == other.policy
-    
+
     def __ne__(self, other):
         return not self.__eq__(other)
-    
+
     def __hash__(self):
         return hash(self.policy)
-    
+
     def to_dict(self) -> Dict:
+        """Convert the policy to a dictionary."""
         return self.policy
-    
+
     @property
     def allowed_intervals(self) -> List[str]:
         """
         Returns a list of allowed intervals for this policy.
         The list is
             P1M - monthly
             P1D - daily
             PT1H - hourly
             PT15M - quarter-hourly
             PT5M - five-minute
 
-        The policy allows all intervals that are higher up the list than the allowed interval.
+        The policy allows all intervals that are higher
+        than the allowed interval.
         """
-        intervals = ['P1M', 'P1D', 'PT1H', 'PT15M', 'PT5M']
-        return intervals[:intervals.index(self.allowed_interval)+1]
+        intervals = ["P1M", "P1D", "PT1H", "PT15M", "PT5M"]
+        return intervals[: intervals.index(self.allowed_interval) + 1]
```

### Comparing `energyid-webhooks-0.0.5/src/energyid_webhooks.egg-info/PKG-INFO` & `energyid-webhooks-0.0.6/src/energyid_webhooks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyid-webhooks
-Version: 0.0.5
+Version: 0.0.6
 Summary: Light weight python package to interface with EnergyID webhooks
 Home-page: https://api.energyid.eu/docs.html#webhook
 Author: Jan Pecinovsky
 Author-email: jan@energieid.be
 Project-URL: Bug Tracker, https://github.com/EnergieID/energyid-webhooks-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

