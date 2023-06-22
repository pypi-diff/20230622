# Comparing `tmp/django_gem-1.1.3.tar.gz` & `tmp/django_gem-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gem-1.1.3.tar", max compression
+gzip compressed data, was "django_gem-1.1.4.tar", max compression
```

## Comparing `django_gem-1.1.3.tar` & `django_gem-1.1.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1067 2023-06-22 11:40:46.138620 django_gem-1.1.3/LICENSE
--rw-r--r--   0        0        0     2786 2023-06-22 11:40:46.138620 django_gem-1.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/__init__.py
--rw-r--r--   0        0        0      257 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/apps.py
--rw-r--r--   0        0        0      535 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/constants.py
--rw-r--r--   0        0        0       71 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/context/__init__.py
--rw-r--r--   0        0        0      283 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/context/cutting_always_eager.py
--rw-r--r--   0        0        0      452 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/context/override_cutting_mode.py
--rw-r--r--   0        0        0      298 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/context/override_gem_setting.py
--rw-r--r--   0        0        0      225 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/core.py
--rw-r--r--   0        0        0        0 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/cutters/__init__.py
--rw-r--r--   0        0        0     1026 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/cutters/base.py
--rw-r--r--   0        0        0       54 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/decorators/__init__.py
--rw-r--r--   0        0        0      220 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/decorators/context.py
--rw-r--r--   0        0        0     1104 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/decorators/cutters.py
--rw-r--r--   0        0        0     1536 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/decorators/models.py
--rw-r--r--   0        0        0        0 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/entities/__init__.py
--rw-r--r--   0        0        0      207 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/entities/context.py
--rw-r--r--   0        0        0      737 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/entities/models.py
--rw-r--r--   0        0        0     1706 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/entities/registry.py
--rw-r--r--   0        0        0      132 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/entities/source.py
--rw-r--r--   0        0        0     1108 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/exceptions.py
--rw-r--r--   0        0        0       58 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/logger.py
--rw-r--r--   0        0        0        0 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/management/commands/__init__.py
--rw-r--r--   0        0        0      893 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/management/commands/cutmodel.py
--rw-r--r--   0        0        0      953 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/management/commands/cutqueryset.py
--rw-r--r--   0        0        0     2622 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/migrations/__init__.py
--rw-r--r--   0        0        0       56 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/models/__init__.py
--rw-r--r--   0        0        0     2077 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/models/base.py
--rw-r--r--   0        0        0     1432 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/models/gem_log_entry.py
--rw-r--r--   0        0        0        0 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/models/managers/__init__.py
--rw-r--r--   0        0        0     1297 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/models/managers/gem_log_entry_manager.py
--rw-r--r--   0        0        0     2938 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/models/mixins.py
--rw-r--r--   0        0        0      178 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/overrides/__init__.py
--rw-r--r--   0        0        0     1591 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/overrides/delete.py
--rw-r--r--   0        0        0     1260 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/overrides/m2m_changed.py
--rw-r--r--   0        0        0     2274 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/overrides/save.py
--rw-r--r--   0        0        0      937 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/overrides/utils.py
--rw-r--r--   0        0        0      184 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/tasks/__init__.py
--rw-r--r--   0        0        0      235 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/tasks/cut_content_type.py
--rw-r--r--   0        0        0      286 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/tasks/cut_models.py
--rw-r--r--   0        0        0      221 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/tasks/cut_queryset.py
--rw-r--r--   0        0        0      251 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/__init__.py
--rw-r--r--   0        0        0       57 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/anvils/__init__.py
--rw-r--r--   0        0        0      116 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/anvils/base.py
--rw-r--r--   0        0        0      353 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/anvils/celery.py
--rw-r--r--   0        0        0      337 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/anvils/eager.py
--rw-r--r--   0        0        0     2568 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/chest.py
--rw-r--r--   0        0        0     5072 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/forge.py
--rw-r--r--   0        0        0     7737 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/registry.py
--rw-r--r--   0        0        0     5948 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/saw.py
--rw-r--r--   0        0        0     1328 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/settings.py
--rw-r--r--   0        0        0     1859 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/toolkit/smith.py
--rw-r--r--   0        0        0     4198 2023-06-22 11:40:46.138620 django_gem-1.1.3/django_gem/validators.py
--rw-r--r--   0        0        0      811 2023-06-22 11:40:46.138620 django_gem-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 django_gem-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-22 15:28:50.750500 django_gem-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2786 2023-06-22 15:28:50.750500 django_gem-1.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/apps.py
+-rw-r--r--   0        0        0      535 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/constants.py
+-rw-r--r--   0        0        0       71 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/context/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/context/cutting_always_eager.py
+-rw-r--r--   0        0        0      452 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/context/override_cutting_mode.py
+-rw-r--r--   0        0        0      298 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/context/override_gem_setting.py
+-rw-r--r--   0        0        0      225 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/core.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/cutters/__init__.py
+-rw-r--r--   0        0        0     1026 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/cutters/base.py
+-rw-r--r--   0        0        0       54 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/decorators/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/decorators/context.py
+-rw-r--r--   0        0        0     1104 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/decorators/cutters.py
+-rw-r--r--   0        0        0     1536 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/decorators/models.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/entities/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/entities/context.py
+-rw-r--r--   0        0        0      737 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/entities/models.py
+-rw-r--r--   0        0        0     1706 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/entities/registry.py
+-rw-r--r--   0        0        0      132 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/entities/source.py
+-rw-r--r--   0        0        0     1108 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/exceptions.py
+-rw-r--r--   0        0        0       58 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/logger.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/management/commands/__init__.py
+-rw-r--r--   0        0        0      893 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/management/commands/cutmodel.py
+-rw-r--r--   0        0        0      953 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/management/commands/cutqueryset.py
+-rw-r--r--   0        0        0     2622 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/migrations/__init__.py
+-rw-r--r--   0        0        0       56 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/models/__init__.py
+-rw-r--r--   0        0        0     2077 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/models/base.py
+-rw-r--r--   0        0        0     1432 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/models/gem_log_entry.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/models/managers/__init__.py
+-rw-r--r--   0        0        0     1297 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/models/managers/gem_log_entry_manager.py
+-rw-r--r--   0        0        0     2843 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/models/mixins.py
+-rw-r--r--   0        0        0      178 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/overrides/__init__.py
+-rw-r--r--   0        0        0     1591 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/overrides/delete.py
+-rw-r--r--   0        0        0     1260 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/overrides/m2m_changed.py
+-rw-r--r--   0        0        0     2274 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/overrides/save.py
+-rw-r--r--   0        0        0      937 2023-06-22 15:28:50.750500 django_gem-1.1.4/django_gem/overrides/utils.py
+-rw-r--r--   0        0        0      184 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/tasks/__init__.py
+-rw-r--r--   0        0        0      235 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/tasks/cut_content_type.py
+-rw-r--r--   0        0        0      286 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/tasks/cut_models.py
+-rw-r--r--   0        0        0      221 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/tasks/cut_queryset.py
+-rw-r--r--   0        0        0      251 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/anvils/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/anvils/base.py
+-rw-r--r--   0        0        0      353 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/anvils/celery.py
+-rw-r--r--   0        0        0      337 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/anvils/eager.py
+-rw-r--r--   0        0        0     2568 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/chest.py
+-rw-r--r--   0        0        0     5072 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/forge.py
+-rw-r--r--   0        0        0     7737 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/registry.py
+-rw-r--r--   0        0        0     5948 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/saw.py
+-rw-r--r--   0        0        0     1328 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/settings.py
+-rw-r--r--   0        0        0     1859 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/toolkit/smith.py
+-rw-r--r--   0        0        0     4198 2023-06-22 15:28:50.754500 django_gem-1.1.4/django_gem/validators.py
+-rw-r--r--   0        0        0      811 2023-06-22 15:28:50.754500 django_gem-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 django_gem-1.1.4/PKG-INFO
```

### Comparing `django_gem-1.1.3/LICENSE` & `django_gem-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/README.md` & `django_gem-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/constants.py` & `django_gem-1.1.4/django_gem/constants.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/cutters/base.py` & `django_gem-1.1.4/django_gem/cutters/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/decorators/cutters.py` & `django_gem-1.1.4/django_gem/decorators/cutters.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/decorators/models.py` & `django_gem-1.1.4/django_gem/decorators/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/entities/models.py` & `django_gem-1.1.4/django_gem/entities/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/entities/registry.py` & `django_gem-1.1.4/django_gem/entities/registry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/exceptions.py` & `django_gem-1.1.4/django_gem/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/management/commands/cutmodel.py` & `django_gem-1.1.4/django_gem/management/commands/cutmodel.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/management/commands/cutqueryset.py` & `django_gem-1.1.4/django_gem/management/commands/cutqueryset.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/migrations/0001_initial.py` & `django_gem-1.1.4/django_gem/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/models/base.py` & `django_gem-1.1.4/django_gem/models/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/models/gem_log_entry.py` & `django_gem-1.1.4/django_gem/models/gem_log_entry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/models/managers/gem_log_entry_manager.py` & `django_gem-1.1.4/django_gem/models/managers/gem_log_entry_manager.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/models/mixins.py` & `django_gem-1.1.4/django_gem/models/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 
 
 class GemTriggerMixin(DirtyFieldsMixin):
     def is_any_field_changed(self, fields: list):
         dirty_fields = self.get_dirty_fields(check_relationship=True)
         if not dirty_fields:
             return False  # No fields changed - we don't recalculate
-        if not fields:
-            return True  # No affected fields provided - we recalculate
         return any(field in dirty_fields for field in fields)
 
 
 class GemAuditLogMixin(DirtyFieldsMixin):
     @classmethod
     def field_value(cls, instance, field_name):
         if not instance:
```

### Comparing `django_gem-1.1.3/django_gem/overrides/delete.py` & `django_gem-1.1.4/django_gem/overrides/delete.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/overrides/m2m_changed.py` & `django_gem-1.1.4/django_gem/overrides/m2m_changed.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/overrides/save.py` & `django_gem-1.1.4/django_gem/overrides/save.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/overrides/utils.py` & `django_gem-1.1.4/django_gem/overrides/utils.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/toolkit/chest.py` & `django_gem-1.1.4/django_gem/toolkit/chest.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/toolkit/forge.py` & `django_gem-1.1.4/django_gem/toolkit/forge.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/toolkit/registry.py` & `django_gem-1.1.4/django_gem/toolkit/registry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/toolkit/saw.py` & `django_gem-1.1.4/django_gem/toolkit/saw.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/toolkit/settings.py` & `django_gem-1.1.4/django_gem/toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/toolkit/smith.py` & `django_gem-1.1.4/django_gem/toolkit/smith.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/django_gem/validators.py` & `django_gem-1.1.4/django_gem/validators.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.1.3/pyproject.toml` & `django_gem-1.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 profile = "black"
 
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "django-gem"
-version = "1.1.3"
+version = "1.1.4"
 description = "Distrubited calculations for Django models"
 authors = ["Artur Veres <artur8118@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_gem"}]
 
 [tool.poetry.dependencies]
```

### Comparing `django_gem-1.1.3/PKG-INFO` & `django_gem-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gem
-Version: 1.1.3
+Version: 1.1.4
 Summary: Distrubited calculations for Django models
 License: MIT
 Author: Artur Veres
 Author-email: artur8118@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

