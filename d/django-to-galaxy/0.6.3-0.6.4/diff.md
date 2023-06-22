# Comparing `tmp/django_to_galaxy-0.6.3.tar.gz` & `tmp/django_to_galaxy-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_to_galaxy-0.6.3.tar", max compression
+gzip compressed data, was "django_to_galaxy-0.6.4.tar", max compression
```

## Comparing `django_to_galaxy-0.6.3.tar` & `django_to_galaxy-0.6.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    34498 2023-03-08 17:25:44.148268 django_to_galaxy-0.6.3/LICENSE
--rw-r--r--   0        0        0       41 2023-03-08 17:25:44.148268 django_to_galaxy-0.6.3/django_to_galaxy/__init__.py
--rw-r--r--   0        0        0      369 2023-03-08 17:25:44.149268 django_to_galaxy-0.6.3/django_to_galaxy/admin/__init__.py
--rw-r--r--   0        0        0      159 2023-03-08 17:25:44.149268 django_to_galaxy-0.6.3/django_to_galaxy/admin/galaxy_element.py
--rw-r--r--   0        0        0      834 2023-03-08 17:25:44.149268 django_to_galaxy-0.6.3/django_to_galaxy/admin/galaxy_instance.py
--rw-r--r--   0        0        0     2321 2023-03-08 17:25:44.149268 django_to_galaxy-0.6.3/django_to_galaxy/admin/galaxy_output_file.py
--rw-r--r--   0        0        0     7278 2023-03-08 17:25:44.149268 django_to_galaxy-0.6.3/django_to_galaxy/admin/galaxy_user.py
--rw-r--r--   0        0        0     2562 2023-03-08 17:25:44.149268 django_to_galaxy-0.6.3/django_to_galaxy/admin/history.py
--rw-r--r--   0        0        0     4821 2023-03-08 17:25:44.149268 django_to_galaxy-0.6.3/django_to_galaxy/admin/invocation.py
--rw-r--r--   0        0        0      315 2023-03-08 17:25:44.149268 django_to_galaxy-0.6.3/django_to_galaxy/admin/tag.py
--rw-r--r--   0        0        0     1360 2023-03-08 23:23:39.965821 django_to_galaxy-0.6.3/django_to_galaxy/admin/workflow.py
--rw-r--r--   0        0        0        0 2023-03-08 17:25:44.149268 django_to_galaxy-0.6.3/django_to_galaxy/api/__init__.py
--rw-r--r--   0        0        0     1079 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/asymetricslugrelatedfield.py
--rw-r--r--   0        0        0      257 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/galaxy_instance.py
--rw-r--r--   0        0        0      428 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/galaxy_output_file.py
--rw-r--r--   0        0        0      674 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/galaxy_user.py
--rw-r--r--   0        0        0      387 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/history.py
--rw-r--r--   0        0        0      396 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/invocation.py
--rw-r--r--   0        0        0      657 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/invoke_workflow.py
--rw-r--r--   0        0        0      883 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/upload_to_history.py
--rw-r--r--   0        0        0      981 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/workflow.py
--rw-r--r--   0        0        0     1661 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/urls.py
--rw-r--r--   0        0        0      748 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/views/create_history.py
--rw-r--r--   0        0        0      434 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/views/galaxy_instance.py
--rw-r--r--   0        0        0      439 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/views/galaxy_output_file.py
--rw-r--r--   0        0        0      420 2023-03-08 17:25:44.150268 django_to_galaxy-0.6.3/django_to_galaxy/api/views/galaxy_user.py
--rw-r--r--   0        0        0      394 2023-03-08 17:25:44.151268 django_to_galaxy-0.6.3/django_to_galaxy/api/views/history.py
--rw-r--r--   0        0        0     1318 2023-03-08 17:25:44.151268 django_to_galaxy-0.6.3/django_to_galaxy/api/views/invocation.py
--rw-r--r--   0        0        0     6530 2023-03-08 17:25:44.151268 django_to_galaxy-0.6.3/django_to_galaxy/api/views/invoke_workflow.py
--rw-r--r--   0        0        0     2972 2023-03-08 17:25:44.151268 django_to_galaxy-0.6.3/django_to_galaxy/api/views/upload_to_history.py
--rw-r--r--   0        0        0      401 2023-03-08 17:25:44.151268 django_to_galaxy-0.6.3/django_to_galaxy/api/views/workflow.py
--rw-r--r--   0        0        0      143 2023-03-08 17:25:44.151268 django_to_galaxy-0.6.3/django_to_galaxy/apps.py
--rw-r--r--   0        0        0     5954 2023-03-08 17:25:44.151268 django_to_galaxy-0.6.3/django_to_galaxy/migrations/0001_new_initial.py
--rw-r--r--   0        0        0      965 2023-03-08 17:25:44.151268 django_to_galaxy-0.6.3/django_to_galaxy/migrations/0002_rename_state_history_galaxy_state_and_more.py
--rw-r--r--   0        0        0      515 2023-03-08 17:25:44.151268 django_to_galaxy-0.6.3/django_to_galaxy/migrations/0003_invocation_create_time.py
--rw-r--r--   0        0        0     1506 2023-03-08 17:25:44.152268 django_to_galaxy-0.6.3/django_to_galaxy/migrations/0004_alter_galaxyuser_email_galaxyoutputfile.py
--rw-r--r--   0        0        0     1052 2023-03-08 17:25:44.152268 django_to_galaxy-0.6.3/django_to_galaxy/migrations/0005_alter_galaxyoutputfile_invocation_and_more.py
--rw-r--r--   0        0        0     1180 2023-03-08 17:25:44.152268 django_to_galaxy-0.6.3/django_to_galaxy/migrations/0006_tag_history_tags_workflow_tags.py
--rw-r--r--   0        0        0     2000 2023-03-08 17:25:44.152268 django_to_galaxy-0.6.3/django_to_galaxy/migrations/0007_format_alter_history_tags_alter_workflow_tags_and_more.py
--rw-r--r--   0        0        0      481 2023-03-08 17:25:44.152268 django_to_galaxy-0.6.3/django_to_galaxy/migrations/0008_workflowinput_label.py
--rw-r--r--   0        0        0        0 2023-03-08 17:25:44.152268 django_to_galaxy-0.6.3/django_to_galaxy/migrations/__init__.py
--rw-r--r--   0        0        0      370 2023-03-09 10:35:53.952605 django_to_galaxy-0.6.3/django_to_galaxy/models/__init__.py
--rw-r--r--   0        0        0      698 2023-03-08 17:25:44.152268 django_to_galaxy-0.6.3/django_to_galaxy/models/accepted_input.py
--rw-r--r--   0        0        0     1425 2023-03-08 17:25:44.152268 django_to_galaxy-0.6.3/django_to_galaxy/models/galaxy_element.py
--rw-r--r--   0        0        0      723 2023-03-08 17:25:44.152268 django_to_galaxy-0.6.3/django_to_galaxy/models/galaxy_instance.py
--rw-r--r--   0        0        0     1646 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/models/galaxy_output_file.py
--rw-r--r--   0        0        0     3264 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/models/galaxy_user.py
--rw-r--r--   0        0        0     2635 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/models/history.py
--rw-r--r--   0        0        0     6588 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/models/invocation.py
--rw-r--r--   0        0        0     1891 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/models/workflow.py
--rw-r--r--   0        0        0        0 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/schemas/__init__.py
--rw-r--r--   0        0        0      396 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/schemas/dataset.py
--rw-r--r--   0        0        0      138 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/settings.py
--rw-r--r--   0        0        0     2389 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/templates/admin/import_workflows.html
--rw-r--r--   0        0        0      106 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/urls.py
--rw-r--r--   0        0        0     1625 2023-03-08 17:25:44.153268 django_to_galaxy-0.6.3/django_to_galaxy/utils.py
--rw-r--r--   0        0        0      111 2023-03-09 14:03:50.714270 django_to_galaxy-0.6.3/django_to_galaxy/version.py
--rw-r--r--   0        0        0      771 2023-03-09 14:03:50.714270 django_to_galaxy-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 django_to_galaxy-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    34498 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/LICENSE
+-rw-r--r--   0        0        0       41 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/__init__.py
+-rw-r--r--   0        0        0      369 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/admin/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/admin/galaxy_element.py
+-rw-r--r--   0        0        0      834 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/admin/galaxy_instance.py
+-rw-r--r--   0        0        0     2321 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/admin/galaxy_output_file.py
+-rw-r--r--   0        0        0     7278 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/admin/galaxy_user.py
+-rw-r--r--   0        0        0     2562 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/admin/history.py
+-rw-r--r--   0        0        0     4821 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/admin/invocation.py
+-rw-r--r--   0        0        0      315 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/admin/tag.py
+-rw-r--r--   0        0        0     1360 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/admin/workflow.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/__init__.py
+-rw-r--r--   0        0        0     1079 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/asymetricslugrelatedfield.py
+-rw-r--r--   0        0        0      257 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/galaxy_instance.py
+-rw-r--r--   0        0        0      428 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/galaxy_output_file.py
+-rw-r--r--   0        0        0      674 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/galaxy_user.py
+-rw-r--r--   0        0        0      387 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/history.py
+-rw-r--r--   0        0        0      396 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/invocation.py
+-rw-r--r--   0        0        0      657 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/invoke_workflow.py
+-rw-r--r--   0        0        0      883 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/upload_to_history.py
+-rw-r--r--   0        0        0      981 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/workflow.py
+-rw-r--r--   0        0        0     1661 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/urls.py
+-rw-r--r--   0        0        0      748 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/views/create_history.py
+-rw-r--r--   0        0        0      434 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/views/galaxy_instance.py
+-rw-r--r--   0        0        0      439 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/views/galaxy_output_file.py
+-rw-r--r--   0        0        0      420 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/views/galaxy_user.py
+-rw-r--r--   0        0        0      394 2023-06-22 13:21:56.566480 django_to_galaxy-0.6.4/django_to_galaxy/api/views/history.py
+-rw-r--r--   0        0        0     1318 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/api/views/invocation.py
+-rw-r--r--   0        0        0     6530 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/api/views/invoke_workflow.py
+-rw-r--r--   0        0        0     2972 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/api/views/upload_to_history.py
+-rw-r--r--   0        0        0      401 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/api/views/workflow.py
+-rw-r--r--   0        0        0      143 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/apps.py
+-rw-r--r--   0        0        0     5954 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/migrations/0001_new_initial.py
+-rw-r--r--   0        0        0      965 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/migrations/0002_rename_state_history_galaxy_state_and_more.py
+-rw-r--r--   0        0        0      515 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/migrations/0003_invocation_create_time.py
+-rw-r--r--   0        0        0     1506 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/migrations/0004_alter_galaxyuser_email_galaxyoutputfile.py
+-rw-r--r--   0        0        0     1052 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/migrations/0005_alter_galaxyoutputfile_invocation_and_more.py
+-rw-r--r--   0        0        0     1180 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/migrations/0006_tag_history_tags_workflow_tags.py
+-rw-r--r--   0        0        0     2000 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/migrations/0007_format_alter_history_tags_alter_workflow_tags_and_more.py
+-rw-r--r--   0        0        0      481 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/migrations/0008_workflowinput_label.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/migrations/__init__.py
+-rw-r--r--   0        0        0      370 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/models/__init__.py
+-rw-r--r--   0        0        0      889 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/models/accepted_input.py
+-rw-r--r--   0        0        0     1537 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/models/galaxy_element.py
+-rw-r--r--   0        0        0      723 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/models/galaxy_instance.py
+-rw-r--r--   0        0        0     1646 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/models/galaxy_output_file.py
+-rw-r--r--   0        0        0     3264 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/models/galaxy_user.py
+-rw-r--r--   0        0        0     2635 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/models/history.py
+-rw-r--r--   0        0        0     6588 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/models/invocation.py
+-rw-r--r--   0        0        0     1891 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/models/workflow.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/schemas/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/schemas/dataset.py
+-rw-r--r--   0        0        0      138 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/settings.py
+-rw-r--r--   0        0        0     2389 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/templates/admin/import_workflows.html
+-rw-r--r--   0        0        0      106 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/urls.py
+-rw-r--r--   0        0        0     1625 2023-06-22 13:21:56.570480 django_to_galaxy-0.6.4/django_to_galaxy/utils.py
+-rw-r--r--   0        0        0      111 2023-06-22 13:37:29.881690 django_to_galaxy-0.6.4/django_to_galaxy/version.py
+-rw-r--r--   0        0        0      771 2023-06-22 13:37:29.881690 django_to_galaxy-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 django_to_galaxy-0.6.4/PKG-INFO
```

### Comparing `django_to_galaxy-0.6.3/LICENSE` & `django_to_galaxy-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/admin/galaxy_instance.py` & `django_to_galaxy-0.6.4/django_to_galaxy/admin/galaxy_instance.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/admin/galaxy_output_file.py` & `django_to_galaxy-0.6.4/django_to_galaxy/admin/galaxy_output_file.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/admin/galaxy_user.py` & `django_to_galaxy-0.6.4/django_to_galaxy/admin/galaxy_user.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/admin/history.py` & `django_to_galaxy-0.6.4/django_to_galaxy/admin/history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/admin/invocation.py` & `django_to_galaxy-0.6.4/django_to_galaxy/admin/invocation.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/admin/workflow.py` & `django_to_galaxy-0.6.4/django_to_galaxy/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/asymetricslugrelatedfield.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/asymetricslugrelatedfield.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/galaxy_user.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/galaxy_user.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/invoke_workflow.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/invoke_workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/upload_to_history.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/upload_to_history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/serializers/workflow.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/serializers/workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/urls.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/urls.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/views/create_history.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/views/create_history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/views/invocation.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/views/invocation.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/views/invoke_workflow.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/views/invoke_workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/api/views/upload_to_history.py` & `django_to_galaxy-0.6.4/django_to_galaxy/api/views/upload_to_history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/migrations/0001_new_initial.py` & `django_to_galaxy-0.6.4/django_to_galaxy/migrations/0001_new_initial.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/migrations/0002_rename_state_history_galaxy_state_and_more.py` & `django_to_galaxy-0.6.4/django_to_galaxy/migrations/0002_rename_state_history_galaxy_state_and_more.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/migrations/0003_invocation_create_time.py` & `django_to_galaxy-0.6.4/django_to_galaxy/migrations/0003_invocation_create_time.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/migrations/0004_alter_galaxyuser_email_galaxyoutputfile.py` & `django_to_galaxy-0.6.4/django_to_galaxy/migrations/0004_alter_galaxyuser_email_galaxyoutputfile.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/migrations/0005_alter_galaxyoutputfile_invocation_and_more.py` & `django_to_galaxy-0.6.4/django_to_galaxy/migrations/0005_alter_galaxyoutputfile_invocation_and_more.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/migrations/0006_tag_history_tags_workflow_tags.py` & `django_to_galaxy-0.6.4/django_to_galaxy/migrations/0006_tag_history_tags_workflow_tags.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/migrations/0007_format_alter_history_tags_alter_workflow_tags_and_more.py` & `django_to_galaxy-0.6.4/django_to_galaxy/migrations/0007_format_alter_history_tags_alter_workflow_tags_and_more.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/models/galaxy_element.py` & `django_to_galaxy-0.6.4/django_to_galaxy/models/galaxy_element.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 from django.db import models
 
 
 class Tag(models.Model):
     label = models.CharField(null=False, max_length=200, unique=True)
 
+    def __str__(self):
+        return f"{self.label}"
+
+    def __repr__(self):
+        return f"Tag: {self!s}"
+
 
 class GalaxyElement(models.Model):
     """Base class for all Galaxy elements with galaxy id that are likely to evolve or change."""
 
     galaxy_id = models.CharField(null=False, max_length=50)
     """Invocation id used on the galaxy side."""
     name = models.CharField(null=False, max_length=200)
```

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/models/galaxy_instance.py` & `django_to_galaxy-0.6.4/django_to_galaxy/models/galaxy_instance.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/models/galaxy_output_file.py` & `django_to_galaxy-0.6.4/django_to_galaxy/models/galaxy_output_file.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/models/galaxy_user.py` & `django_to_galaxy-0.6.4/django_to_galaxy/models/galaxy_user.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/models/history.py` & `django_to_galaxy-0.6.4/django_to_galaxy/models/history.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/models/invocation.py` & `django_to_galaxy-0.6.4/django_to_galaxy/models/invocation.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/models/workflow.py` & `django_to_galaxy-0.6.4/django_to_galaxy/models/workflow.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/templates/admin/import_workflows.html` & `django_to_galaxy-0.6.4/django_to_galaxy/templates/admin/import_workflows.html`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/django_to_galaxy/utils.py` & `django_to_galaxy-0.6.4/django_to_galaxy/utils.py`

 * *Files identical despite different names*

### Comparing `django_to_galaxy-0.6.3/pyproject.toml` & `django_to_galaxy-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-to-galaxy"
-version = "0.6.3"
+version = "0.6.4"
 description = "Django extension that eases communication with Galaxy instance to execute workflows."
 authors = ["Kenzo-Hugo Hillion <hillion.kenzo@posteo.net>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Django = "^4.0.3"
 bioblend = "^0.16.0"
```

### Comparing `django_to_galaxy-0.6.3/PKG-INFO` & `django_to_galaxy-0.6.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-to-galaxy
-Version: 0.6.3
+Version: 0.6.4
 Summary: Django extension that eases communication with Galaxy instance to execute workflows.
 Author: Kenzo-Hugo Hillion
 Author-email: hillion.kenzo@posteo.net
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

