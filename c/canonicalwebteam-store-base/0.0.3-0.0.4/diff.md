# Comparing `tmp/canonicalwebteam_store_base-0.0.3.tar.gz` & `tmp/canonicalwebteam_store_base-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonicalwebteam_store_base-0.0.3.tar", max compression
+gzip compressed data, was "canonicalwebteam_store_base-0.0.4.tar", max compression
```

## Comparing `canonicalwebteam_store_base-0.0.3.tar` & `canonicalwebteam_store_base-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/LICENSE
--rw-r--r--   0        0        0     1304 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/__init__.py
--rw-r--r--   0        0        0     1424 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/app.py
--rw-r--r--   0        0        0        0 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/__init__.py
--rw-r--r--   0        0        0      385 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/authentication.py
--rw-r--r--   0        0        0     1656 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/logic.py
--rw-r--r--   0        0        0     3723 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/views.py
--rw-r--r--   0        0        0    27069 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/data/licenses.json
--rw-r--r--   0        0        0     2745 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/handlers.py
--rw-r--r--   0        0        0        0 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/__init__.py
--rw-r--r--   0        0        0    10405 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/logic.py
--rw-r--r--   0        0        0     2665 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/views.py
--rw-r--r--   0        0        0      201 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/sample_blueprint/views.py
--rw-r--r--   0        0        0        0 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/__init__.py
--rw-r--r--   0        0        0     1094 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/config.py
--rw-r--r--   0        0        0      166 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/constants.py
--rw-r--r--   0        0        0      434 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/decorators.py
--rw-r--r--   0        0        0       61 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/extensions.py
--rw-r--r--   0        0        0     4608 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/helpers.py
--rw-r--r--   0        0        0       25 2023-06-09 08:20:07.747096 canonicalwebteam_store_base-0.0.3/canonicalwebteam/templates/storebase.html
--rw-r--r--   0        0        0     1050 2023-06-09 08:20:07.751096 canonicalwebteam_store_base-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1304 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/__init__.py
+-rw-r--r--   0        0        0     1424 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/app.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/__init__.py
+-rw-r--r--   0        0        0      385 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/authentication.py
+-rw-r--r--   0        0        0     1656 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/logic.py
+-rw-r--r--   0        0        0     3723 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/views.py
+-rw-r--r--   0        0        0    27069 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/data/licenses.json
+-rw-r--r--   0        0        0     2745 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/__init__.py
+-rw-r--r--   0        0        0    10518 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/logic.py
+-rw-r--r--   0        0        0     2665 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/views.py
+-rw-r--r--   0        0        0      201 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/sample_blueprint/views.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/__init__.py
+-rw-r--r--   0        0        0     1094 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/config.py
+-rw-r--r--   0        0        0      166 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/constants.py
+-rw-r--r--   0        0        0      433 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/decorators.py
+-rw-r--r--   0        0        0       61 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/extensions.py
+-rw-r--r--   0        0        0     4608 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/helpers.py
+-rw-r--r--   0        0        0       25 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/canonicalwebteam/templates/storebase.html
+-rw-r--r--   0        0        0     1050 2023-06-22 14:34:56.755472 canonicalwebteam_store_base-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.4/PKG-INFO
```

### Comparing `canonicalwebteam_store_base-0.0.3/LICENSE` & `canonicalwebteam_store_base-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/README.md` & `canonicalwebteam_store_base-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/app.py` & `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/app.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/logic.py` & `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/logic.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/auth/views.py` & `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/auth/views.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/data/licenses.json` & `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/data/licenses.json`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/handlers.py` & `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/handlers.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/logic.py` & `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,29 +70,30 @@
 
     if store_name.startswith("charmhub"):
         result = package.get("result", {})
         publisher = result.get("publisher", {})
 
         resp["package"]["type"] = package.get("type", "")
         resp["package"]["name"] = package.get("name", "")
-        resp["package"]["description"] = result.get("summary", "")
+        resp["package"]["description"] = result.get("summary", "").split(".")[
+            0
+        ]
         resp["package"]["display_name"] = result.get(
             "title", format_slug(package.get("name", ""))
         )
         resp["package"]["platforms"] = result.get("deployable-on", [])
         resp["publisher"]["display_name"] = publisher.get("display-name", "")
         resp["publisher"]["validation"] = publisher.get("validation", "")
         resp["categories"] = result.get("categories", [])
         resp["package"]["icon_url"] = helpers.get_icon(result.get("media", []))
 
     if store_name.startswith("snapcraft"):
-        # pprint({package_type: package})
         snap = package.get("snap", {})
         publisher = snap.get("publisher", {})
-        resp["package"]["description"] = snap.get("summary", "")
+        resp["package"]["description"] = snap.get("summary", "").split(".")[0]
         resp["package"]["display_name"] = snap.get("title", "")
         resp["package"]["type"] = "snap"
         resp["package"]["name"] = package.get("name", "")
         # platform to be fetched
         resp["publisher"]["display_name"] = publisher.get("display-name", "")
         resp["publisher"]["name"] = publisher.get("username", "")
         resp["publisher"]["validation"] = publisher.get("validation", "")
@@ -163,16 +164,18 @@
     total_pages = -(len(packages) // -size)
 
     if filters:
         parsed_packages = []
         for package in packages:
             parsed_packages.append(parse_package_for_card(package, store_name))
         filtered_packages = filter_packages(parsed_packages, filters)
+        total_pages = -(len(filtered_packages) // -size)
         res = paginate(filtered_packages, page, size, total_pages)
     else:
+        total_pages = -(len(packages) // -size)
         packages_per_page = paginate(packages, page, size, total_pages)
         parsed_packages = []
         for package in packages_per_page:
             parsed_packages.append(parse_package_for_card(package, store_name))
         res = parsed_packages
 
     return {"packages": res, "total_pages": total_pages}
```

### Comparing `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/packages/views.py` & `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/packages/views.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/config.py` & `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/config.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/canonicalwebteam/store_base/utils/helpers.py` & `canonicalwebteam_store_base-0.0.4/canonicalwebteam/store_base/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.3/pyproject.toml` & `canonicalwebteam_store_base-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canonicalwebteam-store-base"
-version = "0.0.3"
+version = "0.0.4"
 description = "An application base for all stores"
 authors = ["Canonical Webteam <webteam@canonical.com>"]
 license = "GPL3"
 readme = "README.md"
 packages = [{include = "canonicalwebteam"}]
 
 [tool.poetry.dependencies]
```

### Comparing `canonicalwebteam_store_base-0.0.3/PKG-INFO` & `canonicalwebteam_store_base-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam-store-base
-Version: 0.0.3
+Version: 0.0.4
 Summary: An application base for all stores
 License: GPL3
 Author: Canonical Webteam
 Author-email: webteam@canonical.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

