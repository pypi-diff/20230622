# Comparing `tmp/django_snitch-3.1.7.tar.gz` & `tmp/django_snitch-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_snitch-3.1.7.tar", max compression
+gzip compressed data, was "django_snitch-3.1.8.tar", max compression
```

## Comparing `django_snitch-3.1.7.tar` & `django_snitch-3.1.8.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0     1080 2020-09-07 08:02:23.557749 django_snitch-3.1.7/LICENSE
--rw-r--r--   0        0        0     3439 2023-02-24 16:13:58.840348 django_snitch-3.1.7/README.rst
--rw-r--r--   0        0        0     1447 2023-03-31 09:54:31.754746 django_snitch-3.1.7/pyproject.toml
--rw-r--r--   0        0        0     1038 2023-02-22 09:16:00.135066 django_snitch-3.1.7/snitch/__init__.py
--rw-r--r--   0        0        0     1472 2023-02-20 17:52:40.888230 django_snitch-3.1.7/snitch/admin.py
--rw-r--r--   0        0        0      473 2021-12-10 08:08:01.361618 django_snitch-3.1.7/snitch/apps.py
--rw-r--r--   0        0        0     9770 2023-03-09 12:55:56.850331 django_snitch-3.1.7/snitch/backends.py
--rw-r--r--   0        0        0      102 2023-02-20 17:52:40.889249 django_snitch-3.1.7/snitch/constants.py
--rw-r--r--   0        0        0     4946 2023-03-28 17:31:50.535180 django_snitch-3.1.7/snitch/cooldowns.py
--rw-r--r--   0        0        0     3690 2023-02-20 17:52:40.890228 django_snitch-3.1.7/snitch/decorators.py
--rw-r--r--   0        0        0     6376 2023-03-31 09:51:50.555410 django_snitch-3.1.7/snitch/emails.py
--rw-r--r--   0        0        0      230 2023-02-02 08:53:23.849891 django_snitch-3.1.7/snitch/exceptions.py
--rw-r--r--   0        0        0     8662 2023-03-28 15:52:50.420831 django_snitch-3.1.7/snitch/handlers.py
--rw-r--r--   0        0        0     3780 2023-02-20 17:52:40.893941 django_snitch-3.1.7/snitch/helpers.py
--rw-r--r--   0        0        0     2449 2020-09-07 08:02:23.561974 django_snitch-3.1.7/snitch/locale/es_ES/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      754 2023-02-20 17:52:40.894303 django_snitch-3.1.7/snitch/managers.py
--rw-r--r--   0        0        0     6807 2023-02-20 17:52:40.895022 django_snitch-3.1.7/snitch/migrations/0001_initial.py
--rw-r--r--   0        0        0      411 2023-02-20 17:52:40.895426 django_snitch-3.1.7/snitch/migrations/0002_alter_eventtype_verb.py
--rw-r--r--   0        0        0      412 2023-02-20 17:52:40.895825 django_snitch-3.1.7/snitch/migrations/0003_alter_eventtype_verb.py
--rw-r--r--   0        0        0      961 2023-02-20 17:52:40.896240 django_snitch-3.1.7/snitch/migrations/0004_alter_event_id_alter_eventtype_id_and_more.py
--rw-r--r--   0        0        0     1569 2023-02-20 17:52:40.896607 django_snitch-3.1.7/snitch/migrations/0005_notification_receiver_content_type_and_more.py
--rw-r--r--   0        0        0      954 2023-02-20 17:52:40.897148 django_snitch-3.1.7/snitch/migrations/0006_auto_20230220_0641.py
--rw-r--r--   0        0        0      330 2023-03-09 16:09:06.083211 django_snitch-3.1.7/snitch/migrations/0007_remove_notification_user.py
--rw-r--r--   0        0        0        0 2020-09-07 08:02:23.562234 django_snitch-3.1.7/snitch/migrations/__init__.py
--rw-r--r--   0        0        0     7892 2023-03-28 16:18:15.071750 django_snitch-3.1.7/snitch/models.py
--rw-r--r--   0        0        0      117 2021-12-10 08:09:38.609164 django_snitch-3.1.7/snitch/schedules/__init__.py
--rw-r--r--   0        0        0      517 2020-09-07 08:02:23.562658 django_snitch-3.1.7/snitch/schedules/admin.py
--rw-r--r--   0        0        0      227 2021-12-10 09:54:12.898108 django_snitch-3.1.7/snitch/schedules/apps.py
--rw-r--r--   0        0        0     7511 2023-02-20 17:52:40.898181 django_snitch-3.1.7/snitch/schedules/migrations/0001_initial.py
--rw-r--r--   0        0        0      687 2023-02-20 17:52:40.898918 django_snitch-3.1.7/snitch/schedules/migrations/0002_auto_20191118_0940.py
--rw-r--r--   0        0        0      420 2023-02-20 17:52:40.899653 django_snitch-3.1.7/snitch/schedules/migrations/0003_alter_schedule_verb.py
--rw-r--r--   0        0        0      477 2023-02-20 17:52:40.900213 django_snitch-3.1.7/snitch/schedules/migrations/0004_alter_schedule_id.py
--rw-r--r--   0        0        0        0 2020-09-07 08:02:23.563198 django_snitch-3.1.7/snitch/schedules/migrations/__init__.py
--rw-r--r--   0        0        0     8257 2023-02-20 17:52:40.900856 django_snitch-3.1.7/snitch/schedules/models.py
--rw-r--r--   0        0        0      915 2023-02-20 17:52:40.901490 django_snitch-3.1.7/snitch/schedules/tasks.py
--rw-r--r--   0        0        0      636 2021-03-11 10:12:34.048659 django_snitch-3.1.7/snitch/settings.py
--rw-r--r--   0        0        0     1903 2023-02-24 15:50:58.778937 django_snitch-3.1.7/snitch/tasks.py
--rw-r--r--   0        0        0     4621 1970-01-01 00:00:00.000000 django_snitch-3.1.7/setup.py
--rw-r--r--   0        0        0     4401 1970-01-01 00:00:00.000000 django_snitch-3.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-22 07:22:18.142706 django_snitch-3.1.8/LICENSE
+-rw-r--r--   0        0        0     3439 2023-06-22 07:22:18.142994 django_snitch-3.1.8/README.rst
+-rw-r--r--   0        0        0     1447 2023-06-22 07:42:45.817058 django_snitch-3.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1038 2023-06-22 07:22:18.146624 django_snitch-3.1.8/snitch/__init__.py
+-rw-r--r--   0        0        0     1472 2023-06-22 07:22:18.146801 django_snitch-3.1.8/snitch/admin.py
+-rw-r--r--   0        0        0      473 2023-06-22 07:22:18.147081 django_snitch-3.1.8/snitch/apps.py
+-rw-r--r--   0        0        0     9770 2023-06-22 07:22:18.147386 django_snitch-3.1.8/snitch/backends.py
+-rw-r--r--   0        0        0      102 2023-06-22 07:22:18.147603 django_snitch-3.1.8/snitch/constants.py
+-rw-r--r--   0        0        0     4946 2023-06-22 07:22:18.147874 django_snitch-3.1.8/snitch/cooldowns.py
+-rw-r--r--   0        0        0     3690 2023-06-22 07:22:18.148106 django_snitch-3.1.8/snitch/decorators.py
+-rw-r--r--   0        0        0     6362 2023-06-22 07:22:18.148400 django_snitch-3.1.8/snitch/emails.py
+-rw-r--r--   0        0        0      230 2023-06-22 07:22:18.150757 django_snitch-3.1.8/snitch/exceptions.py
+-rw-r--r--   0        0        0     8662 2023-06-22 07:22:18.151012 django_snitch-3.1.8/snitch/handlers.py
+-rw-r--r--   0        0        0     3799 2023-06-22 07:41:30.401217 django_snitch-3.1.8/snitch/helpers.py
+-rw-r--r--   0        0        0     2449 2023-06-22 07:22:18.151887 django_snitch-3.1.8/snitch/locale/es_ES/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      754 2023-06-22 07:22:18.152118 django_snitch-3.1.8/snitch/managers.py
+-rw-r--r--   0        0        0     6807 2023-06-22 07:22:18.152494 django_snitch-3.1.8/snitch/migrations/0001_initial.py
+-rw-r--r--   0        0        0      411 2023-06-22 07:22:18.152725 django_snitch-3.1.8/snitch/migrations/0002_alter_eventtype_verb.py
+-rw-r--r--   0        0        0      412 2023-06-22 07:22:18.152981 django_snitch-3.1.8/snitch/migrations/0003_alter_eventtype_verb.py
+-rw-r--r--   0        0        0      961 2023-06-22 07:22:18.153211 django_snitch-3.1.8/snitch/migrations/0004_alter_event_id_alter_eventtype_id_and_more.py
+-rw-r--r--   0        0        0     1569 2023-06-22 07:22:18.153514 django_snitch-3.1.8/snitch/migrations/0005_notification_receiver_content_type_and_more.py
+-rw-r--r--   0        0        0      963 2023-06-22 09:38:11.467558 django_snitch-3.1.8/snitch/migrations/0006_auto_20230220_0641.py
+-rw-r--r--   0        0        0      330 2023-06-22 07:22:18.153983 django_snitch-3.1.8/snitch/migrations/0007_remove_notification_user.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:22:18.154070 django_snitch-3.1.8/snitch/migrations/__init__.py
+-rw-r--r--   0        0        0     7892 2023-06-22 07:22:18.154363 django_snitch-3.1.8/snitch/models.py
+-rw-r--r--   0        0        0      117 2023-06-22 07:22:18.154791 django_snitch-3.1.8/snitch/schedules/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-22 07:22:18.154995 django_snitch-3.1.8/snitch/schedules/admin.py
+-rw-r--r--   0        0        0      227 2023-06-22 07:22:18.155217 django_snitch-3.1.8/snitch/schedules/apps.py
+-rw-r--r--   0        0        0     7511 2023-06-22 07:22:18.155550 django_snitch-3.1.8/snitch/schedules/migrations/0001_initial.py
+-rw-r--r--   0        0        0      687 2023-06-22 07:22:18.155788 django_snitch-3.1.8/snitch/schedules/migrations/0002_auto_20191118_0940.py
+-rw-r--r--   0        0        0      420 2023-06-22 07:22:18.156014 django_snitch-3.1.8/snitch/schedules/migrations/0003_alter_schedule_verb.py
+-rw-r--r--   0        0        0      477 2023-06-22 07:22:18.156224 django_snitch-3.1.8/snitch/schedules/migrations/0004_alter_schedule_id.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:22:18.156346 django_snitch-3.1.8/snitch/schedules/migrations/__init__.py
+-rw-r--r--   0        0        0     8257 2023-06-22 07:22:18.156694 django_snitch-3.1.8/snitch/schedules/models.py
+-rw-r--r--   0        0        0      915 2023-06-22 07:22:18.156968 django_snitch-3.1.8/snitch/schedules/tasks.py
+-rw-r--r--   0        0        0      636 2023-06-22 07:22:18.157193 django_snitch-3.1.8/snitch/settings.py
+-rw-r--r--   0        0        0     1903 2023-06-22 07:22:18.157484 django_snitch-3.1.8/snitch/tasks.py
+-rw-r--r--   0        0        0     4401 1970-01-01 00:00:00.000000 django_snitch-3.1.8/PKG-INFO
```

### Comparing `django_snitch-3.1.7/LICENSE` & `django_snitch-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/README.rst` & `django_snitch-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/pyproject.toml` & `django_snitch-3.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-snitch"
-version = "3.1.7"
+version = "3.1.8"
 description = "Django app made to integrate generic events that create notifications that can be sent to users using several backends."
 readme = "README.rst"
 authors = ["Marcos Gabarda <hey@marcosgabarda.com>"]
 license = "MIT"
 homepage = "https://github.com/marcosgabarda/django-snitch"
 packages = [
     { include = "snitch" },
```

### Comparing `django_snitch-3.1.7/snitch/__init__.py` & `django_snitch-3.1.8/snitch/__init__.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/admin.py` & `django_snitch-3.1.8/snitch/admin.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/backends.py` & `django_snitch-3.1.8/snitch/backends.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/cooldowns.py` & `django_snitch-3.1.8/snitch/cooldowns.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/decorators.py` & `django_snitch-3.1.8/snitch/decorators.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/emails.py` & `django_snitch-3.1.8/snitch/emails.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import bleach
 from django.conf import settings
 from django.contrib.sites.models import Site
 from django.core.mail import EmailMultiAlternatives
 from django.template.loader import render_to_string
 from django.utils import translation
 
-from snitch.settings import ENABLED_SEND_NOTIFICATIONS
+from snitch.settings import ENABLED_SEND_EMAILS
 from snitch.tasks import send_email_asynchronously
 
 
 class TemplateEmailMessage:
     """An object to handle emails based on templates, with automatic plain
     alternatives.
     """
@@ -133,15 +133,15 @@
             for attach in self.attaches:
                 attach_file_name, attach_content, attach_content_type = attach
                 email.attach(attach_file_name, attach_content, attach_content_type)
             email.send()
 
     def send(self, use_async: bool = True, language: str | None = None):
         """Sends the email at the moment or using a Celery task."""
-        if not ENABLED_SEND_NOTIFICATIONS:
+        if not ENABLED_SEND_EMAILS:
             return
 
         use_async = not self.attaches and use_async
         if self.use_i18n and settings.USE_I18N:
             language = self.get_language()
             translation.activate(language)
         self.subject = "%s" % self.subject
```

### Comparing `django_snitch-3.1.7/snitch/handlers.py` & `django_snitch-3.1.8/snitch/handlers.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/helpers.py` & `django_snitch-3.1.8/snitch/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from snitch.settings import NOTIFICATION_MODEL
 
 if TYPE_CHECKING:
     from snitch.handlers import EventHandler
     from snitch.models import Event
 
 
-def get_notification_model():
+def get_notification_model(apps=None):
     """Return the Notification model that is active in this project."""
     try:
-        return django_apps.get_model(NOTIFICATION_MODEL, require_ready=False)
+        return (apps or django_apps).get_model(NOTIFICATION_MODEL, require_ready=False)
     except ValueError:
         raise ImproperlyConfigured(
             "NOTIFICATION_MODEL must be of the form 'app_label.model_name'"
         )
     except LookupError:
         raise ImproperlyConfigured(
             "NOTIFICATION_MODEL refers to model '%s' that has not been installed"
```

### Comparing `django_snitch-3.1.7/snitch/locale/es_ES/LC_MESSAGES/django.po` & `django_snitch-3.1.8/snitch/locale/es_ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/managers.py` & `django_snitch-3.1.8/snitch/managers.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/migrations/0001_initial.py` & `django_snitch-3.1.8/snitch/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/migrations/0004_alter_event_id_alter_eventtype_id_and_more.py` & `django_snitch-3.1.8/snitch/migrations/0004_alter_event_id_alter_eventtype_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/migrations/0005_notification_receiver_content_type_and_more.py` & `django_snitch-3.1.8/snitch/migrations/0005_notification_receiver_content_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/migrations/0006_auto_20230220_0641.py` & `django_snitch-3.1.8/snitch/migrations/0006_auto_20230220_0641.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.db import migrations, models
 
 from snitch.helpers import get_notification_model
 
 
 def migrate_users_to_receiver(apps, schema_editor):
     """Gets the user field and uses it to complete the receiver."""
-    Notification = get_notification_model()
+    Notification = get_notification_model(apps=apps)
     User = get_user_model()
     ContentType = apps.get_model("contenttypes", "contenttype")
     try:
         Notification.objects.filter(user__isnull=False).update(
             receiver_id=models.F("user__pk"),
             receiver_content_type=ContentType.objects.get_for_model(User),
         )
```

### Comparing `django_snitch-3.1.7/snitch/models.py` & `django_snitch-3.1.8/snitch/models.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/schedules/admin.py` & `django_snitch-3.1.8/snitch/schedules/admin.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/schedules/migrations/0001_initial.py` & `django_snitch-3.1.8/snitch/schedules/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/schedules/migrations/0002_auto_20191118_0940.py` & `django_snitch-3.1.8/snitch/schedules/migrations/0002_auto_20191118_0940.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/schedules/models.py` & `django_snitch-3.1.8/snitch/schedules/models.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/schedules/tasks.py` & `django_snitch-3.1.8/snitch/schedules/tasks.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/settings.py` & `django_snitch-3.1.8/snitch/settings.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/snitch/tasks.py` & `django_snitch-3.1.8/snitch/tasks.py`

 * *Files identical despite different names*

### Comparing `django_snitch-3.1.7/setup.py` & `django_snitch-3.1.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,151 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-snitch
+Version: 3.1.8
+Summary: Django app made to integrate generic events that create notifications that can be sent to users using several backends.
+Home-page: https://github.com/marcosgabarda/django-snitch
+License: MIT
+Author: Marcos Gabarda
+Author-email: hey@marcosgabarda.com
+Requires-Python: >=3.10,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bleach (>=4.1.0)
+Requires-Dist: celery (>=5.0.0,<6.0.0)
+Requires-Dist: django (>=3.0.0)
+Requires-Dist: django-celery-beat (>=2.4.0,<3.0.0)
+Requires-Dist: django-model-utils (>=4.1.1,<5.0.0)
+Requires-Dist: django-push-notifications (>=2.0.0)
+Requires-Dist: single-source (>=0.3.0,<0.4.0)
+Description-Content-Type: text/x-rst
 
-packages = \
-['snitch',
- 'snitch.migrations',
- 'snitch.schedules',
- 'snitch.schedules.migrations']
-
-package_data = \
-{'': ['*'], 'snitch': ['locale/es_ES/LC_MESSAGES/*']}
-
-install_requires = \
-['bleach>=4.1.0',
- 'celery>=5.0.0,<6.0.0',
- 'django-celery-beat>=2.4.0,<3.0.0',
- 'django-model-utils>=4.1.1,<5.0.0',
- 'django-push-notifications>=2.0.0',
- 'django>=3.0.0',
- 'single-source>=0.3.0,<0.4.0']
-
-setup_kwargs = {
-    'name': 'django-snitch',
-    'version': '3.1.7',
-    'description': 'Django app made to integrate generic events that create notifications that can be sent to users using several backends.',
-    'long_description': '=============\nDjango Snitch\n=============\n\n.. image:: https://img.shields.io/pypi/v/django-snitch\n    :target: https://pypi.org/project/django-snitch/\n    :alt: PyPI\n\n.. image:: https://codecov.io/gh/marcosgabarda/django-snitch/branch/main/graph/badge.svg?token=YKC608Q1HX \n    :target: https://codecov.io/gh/marcosgabarda/django-snitch\n\n.. image:: https://img.shields.io/badge/code_style-black-000000.svg\n    :target: https://github.com/ambv/black\n\n.. image:: https://readthedocs.org/projects/django-snitch/badge/?version=latest\n    :target: https://django-snitch.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\nDjango app made to integrate generic events that create notifications that\ncan be sent to users using several backends.\n\nBy default, it integrates **push notifications** and **email** to send the\nnotifications.\n\nMade with Python 3 and Django with :heart:.\n\nQuick start\n-----------\n\n**1** Install using pip:\n\n.. code-block:: bash\n\n    pip install django-snitch\n\n**2** Add "snitch" to your INSTALLED_APPS settings like this:\n\n.. code-block:: python\n\n    INSTALLED_APPS += (\'snitch\',)\n\n**3** Create an ``events.py`` file in your app to register the events:\n\n.. code-block:: python\n\n    import snitch\n    from snitch.backends import PushNotificationBackend, EmailNotificationBackend\n\n    ACTIVATED_EVENT = "activated"\n    CONFIRMED_EVENT = "confirmed"\n\n\n    @snitch.register(ACTIVATED_EVENT)\n    class ActivatedHandler(snitch.EventHandler):\n        title = "Activated!"\n\n\n    @snitch.register(CONFIRMED_EVENT)\n    class ConfirmedHandler(snitch.EventHandler):\n        title = "Confirmed!"\n        notification_backends = [PushNotificationBackend, EmailNotificationBackend]\n\n        # Custom configuration for email backend\n        template_email_kwargs = {"template_name": "email.html"}\n        template_email_async = False\n\n        def audience(self):\n            return get_user_model().objects.all()\n\n\n**4** Use ``dispatch`` decorator to dispatch the event when a function is called:\n\n.. code-block:: python\n\n    from django.db import models\n    from django.utils import timezone\n\n    import snitch\n    from snitch.models import AbstractNotification\n    from tests.app.events import ACTIVATED_EVENT, CONFIRMED_EVENT\n\n\n    class Stuff(models.Model):\n        """Simple stuff model with status."""\n\n        IDLE, ACTIVE, CONFIRMED = 0, 1, 2\n        status = models.PositiveIntegerField(default=IDLE)\n        activated_at = models.DateTimeField(null=True, blank=True)\n        confirmed_at = models.DateTimeField(null=True, blank=True)\n\n        @snitch.dispatch(ACTIVATED_EVENT)\n        def activate(self):\n            self.activated_at = timezone.now()\n\n        @snitch.dispatch(CONFIRMED_EVENT)\n        def confirm(self):\n            self.confirmed_at = timezone.now()\n\n\nCustom Notification model\n-------------------------\n\nYou can, in the same way that ``django.contrib.auth.model.User`` works, swap the\nNotification model, to customize it.\n\nIn order to do that, you should create a model that inherits from\n``AbstractNotification``:\n\n.. code-block:: python\n\n    from django.db import models\n\n    from snitch.models import AbstractNotification\n\n\n    class Notification(AbstractNotification):\n        """Custom notification."""\n\n        extra_field = models.BooleanField(default=False)\n\n\nAnd after that, specify it in the settings:\n\n.. code-block:: python\n\n    SNITCH_NOTIFICATION_MODEL = "app.Notification"\n',
-    'author': 'Marcos Gabarda',
-    'author_email': 'hey@marcosgabarda.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/marcosgabarda/django-snitch',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+=============
+Django Snitch
+=============
 
+.. image:: https://img.shields.io/pypi/v/django-snitch
+    :target: https://pypi.org/project/django-snitch/
+    :alt: PyPI
+
+.. image:: https://codecov.io/gh/marcosgabarda/django-snitch/branch/main/graph/badge.svg?token=YKC608Q1HX 
+    :target: https://codecov.io/gh/marcosgabarda/django-snitch
+
+.. image:: https://img.shields.io/badge/code_style-black-000000.svg
+    :target: https://github.com/ambv/black
+
+.. image:: https://readthedocs.org/projects/django-snitch/badge/?version=latest
+    :target: https://django-snitch.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+Django app made to integrate generic events that create notifications that
+can be sent to users using several backends.
+
+By default, it integrates **push notifications** and **email** to send the
+notifications.
+
+Made with Python 3 and Django with :heart:.
+
+Quick start
+-----------
+
+**1** Install using pip:
+
+.. code-block:: bash
+
+    pip install django-snitch
+
+**2** Add "snitch" to your INSTALLED_APPS settings like this:
+
+.. code-block:: python
+
+    INSTALLED_APPS += ('snitch',)
+
+**3** Create an ``events.py`` file in your app to register the events:
+
+.. code-block:: python
+
+    import snitch
+    from snitch.backends import PushNotificationBackend, EmailNotificationBackend
+
+    ACTIVATED_EVENT = "activated"
+    CONFIRMED_EVENT = "confirmed"
+
+
+    @snitch.register(ACTIVATED_EVENT)
+    class ActivatedHandler(snitch.EventHandler):
+        title = "Activated!"
+
+
+    @snitch.register(CONFIRMED_EVENT)
+    class ConfirmedHandler(snitch.EventHandler):
+        title = "Confirmed!"
+        notification_backends = [PushNotificationBackend, EmailNotificationBackend]
+
+        # Custom configuration for email backend
+        template_email_kwargs = {"template_name": "email.html"}
+        template_email_async = False
+
+        def audience(self):
+            return get_user_model().objects.all()
+
+
+**4** Use ``dispatch`` decorator to dispatch the event when a function is called:
+
+.. code-block:: python
+
+    from django.db import models
+    from django.utils import timezone
+
+    import snitch
+    from snitch.models import AbstractNotification
+    from tests.app.events import ACTIVATED_EVENT, CONFIRMED_EVENT
+
+
+    class Stuff(models.Model):
+        """Simple stuff model with status."""
+
+        IDLE, ACTIVE, CONFIRMED = 0, 1, 2
+        status = models.PositiveIntegerField(default=IDLE)
+        activated_at = models.DateTimeField(null=True, blank=True)
+        confirmed_at = models.DateTimeField(null=True, blank=True)
+
+        @snitch.dispatch(ACTIVATED_EVENT)
+        def activate(self):
+            self.activated_at = timezone.now()
+
+        @snitch.dispatch(CONFIRMED_EVENT)
+        def confirm(self):
+            self.confirmed_at = timezone.now()
+
+
+Custom Notification model
+-------------------------
+
+You can, in the same way that ``django.contrib.auth.model.User`` works, swap the
+Notification model, to customize it.
+
+In order to do that, you should create a model that inherits from
+``AbstractNotification``:
+
+.. code-block:: python
+
+    from django.db import models
+
+    from snitch.models import AbstractNotification
+
+
+    class Notification(AbstractNotification):
+        """Custom notification."""
+
+        extra_field = models.BooleanField(default=False)
+
+
+And after that, specify it in the settings:
+
+.. code-block:: python
+
+    SNITCH_NOTIFICATION_MODEL = "app.Notification"
 
-setup(**setup_kwargs)
```

