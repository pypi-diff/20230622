# Comparing `tmp/formkit_ninja-0.3.3.tar.gz` & `tmp/formkit_ninja-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formkit_ninja-0.3.3.tar", max compression
+gzip compressed data, was "formkit_ninja-0.3.4.tar", max compression
```

## Comparing `formkit_ninja-0.3.3.tar` & `formkit_ninja-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.3/formkit_ninja/__init__.py
--rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.3.3/formkit_ninja/__main__.py
--rw-r--r--   0        0        0    14860 2023-05-09 05:40:10.838963 formkit_ninja-0.3.3/formkit_ninja/admin.py
--rw-r--r--   0        0        0     2568 2023-05-09 05:38:40.651974 formkit_ninja-0.3.3/formkit_ninja/api.py
--rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.3.3/formkit_ninja/fields.py
--rw-r--r--   0        0        0    13579 2023-05-09 06:28:06.199476 formkit_ninja-0.3.3/formkit_ninja/formkit_schema.py
--rw-r--r--   0        0        0        0 2023-04-23 01:43:59.588049 formkit_ninja-0.3.3/formkit_ninja/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.3/formkit_ninja/management/commands/__init__.py
--rw-r--r--   0        0        0     3807 2023-05-09 05:37:21.012799 formkit_ninja-0.3.3/formkit_ninja/management/commands/common_nodes.py
--rw-r--r--   0        0        0    19033 2023-05-09 05:17:09.351553 formkit_ninja-0.3.3/formkit_ninja/management/commands/create_sf11_form.py
--rw-r--r--   0        0        0     3190 2023-04-26 06:36:11.021575 formkit_ninja-0.3.3/formkit_ninja/management/commands/create_sf12_form.py
--rw-r--r--   0        0        0     1360 2023-04-26 06:10:12.411087 formkit_ninja-0.3.3/formkit_ninja/management/commands/create_sf13_form.py
--rw-r--r--   0        0        0    15059 2023-05-09 05:38:40.671974 formkit_ninja-0.3.3/formkit_ninja/migrations/0001_initial.py
--rw-r--r--   0        0        0      605 2023-05-09 05:15:03.707613 formkit_ninja-0.3.3/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py
--rw-r--r--   0        0        0      339 2023-05-09 05:37:27.484727 formkit_ninja-0.3.3/formkit_ninja/migrations/0003_delete_translatable.py
--rw-r--r--   0        0        0        0 2023-04-13 11:58:36.247052 formkit_ninja-0.3.3/formkit_ninja/migrations/__init__.py
--rw-r--r--   0        0        0     9588 2023-05-09 05:38:40.647974 formkit_ninja-0.3.3/formkit_ninja/models.py
--rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.3.3/formkit_ninja/urls.py
--rw-r--r--   0        0        0     1199 2023-05-09 06:27:44.938413 formkit_ninja-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1572 1970-01-01 00:00:00.000000 formkit_ninja-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.4/formkit_ninja/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.3.4/formkit_ninja/__main__.py
+-rw-r--r--   0        0        0    14860 2023-05-09 05:40:10.838963 formkit_ninja-0.3.4/formkit_ninja/admin.py
+-rw-r--r--   0        0        0     2568 2023-05-09 05:38:40.651974 formkit_ninja-0.3.4/formkit_ninja/api.py
+-rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.3.4/formkit_ninja/fields.py
+-rw-r--r--   0        0        0    13644 2023-06-22 13:58:55.603624 formkit_ninja-0.3.4/formkit_ninja/formkit_schema.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:43:59.588049 formkit_ninja-0.3.4/formkit_ninja/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.4/formkit_ninja/management/commands/__init__.py
+-rw-r--r--   0        0        0     3807 2023-05-09 05:37:21.012799 formkit_ninja-0.3.4/formkit_ninja/management/commands/common_nodes.py
+-rw-r--r--   0        0        0    19033 2023-05-09 05:17:09.351553 formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf11_form.py
+-rw-r--r--   0        0        0     3190 2023-04-26 06:36:11.021575 formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf12_form.py
+-rw-r--r--   0        0        0     1360 2023-04-26 06:10:12.411087 formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf13_form.py
+-rw-r--r--   0        0        0    15059 2023-05-09 05:38:40.671974 formkit_ninja-0.3.4/formkit_ninja/migrations/0001_initial.py
+-rw-r--r--   0        0        0      605 2023-05-09 05:15:03.707613 formkit_ninja-0.3.4/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py
+-rw-r--r--   0        0        0      339 2023-05-09 05:37:27.484727 formkit_ninja-0.3.4/formkit_ninja/migrations/0003_delete_translatable.py
+-rw-r--r--   0        0        0        0 2023-04-13 11:58:36.247052 formkit_ninja-0.3.4/formkit_ninja/migrations/__init__.py
+-rw-r--r--   0        0        0     9588 2023-05-09 05:38:40.647974 formkit_ninja-0.3.4/formkit_ninja/models.py
+-rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.3.4/formkit_ninja/urls.py
+-rw-r--r--   0        0        0     1199 2023-06-22 13:59:00.359823 formkit_ninja-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1572 1970-01-01 00:00:00.000000 formkit_ninja-0.3.4/PKG-INFO
```

### Comparing `formkit_ninja-0.3.3/README.md` & `formkit_ninja-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/admin.py` & `formkit_ninja-0.3.4/formkit_ninja/admin.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/api.py` & `formkit_ninja-0.3.4/formkit_ninja/api.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/fields.py` & `formkit_ninja-0.3.4/formkit_ninja/fields.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/formkit_schema.py` & `formkit_ninja-0.3.4/formkit_ninja/formkit_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,16 @@
 
 class DatePickerNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["datepicker"] = "datepicker"
     dollar_formkit: str = Field(default="datepicker", alias="$formkit")
     calendarIcon: str = "calendar"
     format: str = 'DD/MM/YY'
+    nextIcon: str = 'angleRight'
+    prevIcon: str = 'angleLeft'
 
 
 class CheckBoxNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["checkbox"] = "checkbox"
     dollar_formkit: str = Field(default="checkbox", alias="$formkit")
```

### Comparing `formkit_ninja-0.3.3/formkit_ninja/management/commands/common_nodes.py` & `formkit_ninja-0.3.4/formkit_ninja/management/commands/common_nodes.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/management/commands/create_sf11_form.py` & `formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf11_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/management/commands/create_sf12_form.py` & `formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf12_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/management/commands/create_sf13_form.py` & `formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf13_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/migrations/0001_initial.py` & `formkit_ninja-0.3.4/formkit_ninja/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py` & `formkit_ninja-0.3.4/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/formkit_ninja/models.py` & `formkit_ninja-0.3.4/formkit_ninja/models.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.3/pyproject.toml` & `formkit_ninja-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formkit-ninja"
-version = "0.3.3"
+version = "0.3.4"
 description = "A Django-Ninja backend to specify FormKit schemas"
 authors = ["Josh Brooks <josh@catalpa.io>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/catalpainternational/formkit-ninja"
 repository = "https://github.com/catalpainternational/formkit-ninja"
 packages = [{include = "formkit_ninja"}]
```

### Comparing `formkit_ninja-0.3.3/PKG-INFO` & `formkit_ninja-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formkit-ninja
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Django-Ninja backend to specify FormKit schemas
 Home-page: https://github.com/catalpainternational/formkit-ninja
 License: GPLv3
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

