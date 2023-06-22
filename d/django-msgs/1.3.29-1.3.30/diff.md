# Comparing `tmp/django_msgs-1.3.29.tar.gz` & `tmp/django_msgs-1.3.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_msgs-1.3.29.tar", last modified: Thu Jun 22 15:48:11 2023, max compression
+gzip compressed data, was "django_msgs-1.3.30.tar", last modified: Thu Jun 22 19:07:26 2023, max compression
```

## Comparing `django_msgs-1.3.29.tar` & `django_msgs-1.3.30.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 15:48:11.582058 django_msgs-1.3.29/
--rw-r--r--   0 alexander   (501) staff       (20)     1073 2020-12-07 15:50:01.000000 django_msgs-1.3.29/LICENSE
--rw-r--r--   0 alexander   (501) staff       (20)       17 2020-12-07 15:39:16.000000 django_msgs-1.3.29/MANIFEST.in
--rw-r--r--   0 alexander   (501) staff       (20)     3910 2023-06-22 15:48:11.582184 django_msgs-1.3.29/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     3323 2021-09-23 06:41:03.000000 django_msgs-1.3.29/README.md
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 15:48:11.559882 django_msgs-1.3.29/config/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 19:37:37.000000 django_msgs-1.3.29/config/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.29/config/asgi.py
--rw-r--r--   0 alexander   (501) staff       (20)     4673 2022-05-30 08:36:00.000000 django_msgs-1.3.29/config/settings.py
--rw-r--r--   0 alexander   (501) staff       (20)      746 2021-07-13 19:50:10.000000 django_msgs-1.3.29/config/urls.py
--rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.29/config/wsgi.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 15:48:11.561458 django_msgs-1.3.29/django_msgs.egg-info/
--rw-r--r--   0 alexander   (501) staff       (20)     3910 2023-06-22 15:48:11.000000 django_msgs-1.3.29/django_msgs.egg-info/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     1512 2023-06-22 15:48:11.000000 django_msgs-1.3.29/django_msgs.egg-info/SOURCES.txt
--rw-r--r--   0 alexander   (501) staff       (20)        1 2023-06-22 15:48:11.000000 django_msgs-1.3.29/django_msgs.egg-info/dependency_links.txt
--rw-r--r--   0 alexander   (501) staff       (20)       19 2023-06-22 15:48:11.000000 django_msgs-1.3.29/django_msgs.egg-info/requires.txt
--rw-r--r--   0 alexander   (501) staff       (20)       12 2023-06-22 15:48:11.000000 django_msgs-1.3.29/django_msgs.egg-info/top_level.txt
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 15:48:11.567319 django_msgs-1.3.29/msgs/
--rw-r--r--   0 alexander   (501) staff       (20)       43 2021-11-07 20:03:56.000000 django_msgs-1.3.29/msgs/__init__.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 15:48:11.568947 django_msgs-1.3.29/msgs/abstract/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 18:45:04.000000 django_msgs-1.3.29/msgs/abstract/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      748 2022-03-28 10:36:36.000000 django_msgs-1.3.29/msgs/abstract/admin.py
--rw-r--r--   0 alexander   (501) staff       (20)     6470 2023-06-22 15:45:30.000000 django_msgs-1.3.29/msgs/abstract/models.py
--rw-r--r--   0 alexander   (501) staff       (20)      811 2021-11-07 20:06:22.000000 django_msgs-1.3.29/msgs/admin.py
--rw-r--r--   0 alexander   (501) staff       (20)      213 2021-11-07 20:03:56.000000 django_msgs-1.3.29/msgs/app.py
--rw-r--r--   0 alexander   (501) staff       (20)      201 2022-06-07 11:19:07.000000 django_msgs-1.3.29/msgs/exceptions.py
--rw-r--r--   0 alexander   (501) staff       (20)      255 2021-09-28 19:56:53.000000 django_msgs-1.3.29/msgs/helpers.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 15:48:11.576265 django_msgs-1.3.29/msgs/migrations/
--rw-r--r--   0 alexander   (501) staff       (20)     2344 2020-12-08 11:49:48.000000 django_msgs-1.3.29/msgs/migrations/0001_initial.py
--rw-r--r--   0 alexander   (501) staff       (20)      692 2021-02-20 16:00:18.000000 django_msgs-1.3.29/msgs/migrations/0002_timestamped_messages.py
--rw-r--r--   0 alexander   (501) staff       (20)      795 2021-03-03 16:57:06.000000 django_msgs-1.3.29/msgs/migrations/0003_provider_fields_and_statuses.py
--rw-r--r--   0 alexander   (501) staff       (20)      883 2021-03-26 16:56:33.000000 django_msgs-1.3.29/msgs/migrations/0004_default_templates_datamigration.py
--rw-r--r--   0 alexander   (501) staff       (20)      778 2021-07-13 18:33:23.000000 django_msgs-1.3.29/msgs/migrations/0005_tpl_name_and_type.py
--rw-r--r--   0 alexander   (501) staff       (20)      596 2021-07-13 18:33:23.000000 django_msgs-1.3.29/msgs/migrations/0006_tpl_fields_changed.py
--rw-r--r--   0 alexander   (501) staff       (20)     7855 2021-07-15 16:08:11.000000 django_msgs-1.3.29/msgs/migrations/0007_auto_20210715_1608.py
--rw-r--r--   0 alexander   (501) staff       (20)     1301 2021-08-25 12:50:02.000000 django_msgs-1.3.29/msgs/migrations/0008_auto_20210825_1250.py
--rw-r--r--   0 alexander   (501) staff       (20)     2061 2022-02-06 11:05:48.000000 django_msgs-1.3.29/msgs/migrations/0009_auto_20220206_1105.py
--rw-r--r--   0 alexander   (501) staff       (20)      719 2022-03-28 11:09:32.000000 django_msgs-1.3.29/msgs/migrations/0010_auto_20220328_1109.py
--rw-r--r--   0 alexander   (501) staff       (20)     1706 2022-06-13 09:02:27.000000 django_msgs-1.3.29/msgs/migrations/0011_auto_20220613_0857.py
--rw-r--r--   0 alexander   (501) staff       (20)      764 2023-06-22 13:29:37.000000 django_msgs-1.3.29/msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py
--rw-r--r--   0 alexander   (501) staff       (20)      767 2023-06-22 15:46:47.000000 django_msgs-1.3.29/msgs/migrations/0013_email_service_context_message_service_context_and_more.py
--rw-r--r--   0 alexander   (501) staff       (20)        0 2020-07-14 09:53:30.000000 django_msgs-1.3.29/msgs/migrations/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     1997 2022-02-06 12:18:56.000000 django_msgs-1.3.29/msgs/mixins.py
--rw-r--r--   0 alexander   (501) staff       (20)     1276 2022-02-06 14:19:53.000000 django_msgs-1.3.29/msgs/models.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 15:48:11.581638 django_msgs-1.3.29/msgs/providers/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2020-10-02 08:58:26.000000 django_msgs-1.3.29/msgs/providers/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     2698 2022-06-07 12:48:29.000000 django_msgs-1.3.29/msgs/providers/base.py
--rw-r--r--   0 alexander   (501) staff       (20)      601 2021-07-15 17:03:12.000000 django_msgs-1.3.29/msgs/providers/dummy.py
--rw-r--r--   0 alexander   (501) staff       (20)     1826 2022-06-03 11:18:00.000000 django_msgs-1.3.29/msgs/providers/plivo.py
--rw-r--r--   0 alexander   (501) staff       (20)     1724 2021-07-15 17:11:26.000000 django_msgs-1.3.29/msgs/providers/sendgrid.py
--rw-r--r--   0 alexander   (501) staff       (20)     1709 2021-11-07 20:32:25.000000 django_msgs-1.3.29/msgs/providers/sendinblue.py
--rw-r--r--   0 alexander   (501) staff       (20)     2029 2021-04-16 12:11:11.000000 django_msgs-1.3.29/msgs/providers/sendinblue_sdk.py
--rw-r--r--   0 alexander   (501) staff       (20)     2235 2021-08-25 12:13:40.000000 django_msgs-1.3.29/msgs/providers/sendpulse.py
--rw-r--r--   0 alexander   (501) staff       (20)     1822 2022-05-12 11:04:22.000000 django_msgs-1.3.29/msgs/providers/telegram.py
--rw-r--r--   0 alexander   (501) staff       (20)      482 2021-04-16 12:11:11.000000 django_msgs-1.3.29/msgs/providers/twilio.py
--rw-r--r--   0 alexander   (501) staff       (20)      589 2021-04-16 12:11:11.000000 django_msgs-1.3.29/msgs/providers/voximplant.py
--rw-r--r--   0 alexander   (501) staff       (20)     1028 2022-06-07 12:15:13.000000 django_msgs-1.3.29/msgs/signals.py
--rw-r--r--   0 alexander   (501) staff       (20)       60 2020-07-14 09:53:30.000000 django_msgs-1.3.29/msgs/tests.py
--rw-r--r--   0 alexander   (501) staff       (20)      944 2021-07-16 15:56:46.000000 django_msgs-1.3.29/msgs/utils.py
--rw-r--r--   0 alexander   (501) staff       (20)       63 2020-07-14 09:53:30.000000 django_msgs-1.3.29/msgs/views.py
--rw-r--r--   0 alexander   (501) staff       (20)       79 2023-06-22 15:48:11.582624 django_msgs-1.3.29/setup.cfg
--rw-r--r--   0 alexander   (501) staff       (20)      908 2023-06-22 15:48:02.000000 django_msgs-1.3.29/setup.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 19:07:26.834042 django_msgs-1.3.30/
+-rw-r--r--   0 alexander   (501) staff       (20)     1073 2020-12-07 15:50:01.000000 django_msgs-1.3.30/LICENSE
+-rw-r--r--   0 alexander   (501) staff       (20)       17 2020-12-07 15:39:16.000000 django_msgs-1.3.30/MANIFEST.in
+-rw-r--r--   0 alexander   (501) staff       (20)     3910 2023-06-22 19:07:26.834170 django_msgs-1.3.30/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     3323 2021-09-23 06:41:03.000000 django_msgs-1.3.30/README.md
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 19:07:26.785476 django_msgs-1.3.30/config/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 19:37:37.000000 django_msgs-1.3.30/config/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.30/config/asgi.py
+-rw-r--r--   0 alexander   (501) staff       (20)     4673 2022-05-30 08:36:00.000000 django_msgs-1.3.30/config/settings.py
+-rw-r--r--   0 alexander   (501) staff       (20)      746 2021-07-13 19:50:10.000000 django_msgs-1.3.30/config/urls.py
+-rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.30/config/wsgi.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 19:07:26.787333 django_msgs-1.3.30/django_msgs.egg-info/
+-rw-r--r--   0 alexander   (501) staff       (20)     3910 2023-06-22 19:07:26.000000 django_msgs-1.3.30/django_msgs.egg-info/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     1512 2023-06-22 19:07:26.000000 django_msgs-1.3.30/django_msgs.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander   (501) staff       (20)        1 2023-06-22 19:07:26.000000 django_msgs-1.3.30/django_msgs.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander   (501) staff       (20)       19 2023-06-22 19:07:26.000000 django_msgs-1.3.30/django_msgs.egg-info/requires.txt
+-rw-r--r--   0 alexander   (501) staff       (20)       12 2023-06-22 19:07:26.000000 django_msgs-1.3.30/django_msgs.egg-info/top_level.txt
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 19:07:26.792813 django_msgs-1.3.30/msgs/
+-rw-r--r--   0 alexander   (501) staff       (20)       43 2021-11-07 20:03:56.000000 django_msgs-1.3.30/msgs/__init__.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 19:07:26.794077 django_msgs-1.3.30/msgs/abstract/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 18:45:04.000000 django_msgs-1.3.30/msgs/abstract/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      748 2022-03-28 10:36:36.000000 django_msgs-1.3.30/msgs/abstract/admin.py
+-rw-r--r--   0 alexander   (501) staff       (20)     6515 2023-06-22 19:07:00.000000 django_msgs-1.3.30/msgs/abstract/models.py
+-rw-r--r--   0 alexander   (501) staff       (20)      811 2021-11-07 20:06:22.000000 django_msgs-1.3.30/msgs/admin.py
+-rw-r--r--   0 alexander   (501) staff       (20)      213 2021-11-07 20:03:56.000000 django_msgs-1.3.30/msgs/app.py
+-rw-r--r--   0 alexander   (501) staff       (20)      201 2022-06-07 11:19:07.000000 django_msgs-1.3.30/msgs/exceptions.py
+-rw-r--r--   0 alexander   (501) staff       (20)      255 2021-09-28 19:56:53.000000 django_msgs-1.3.30/msgs/helpers.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 19:07:26.810482 django_msgs-1.3.30/msgs/migrations/
+-rw-r--r--   0 alexander   (501) staff       (20)     2344 2020-12-08 11:49:48.000000 django_msgs-1.3.30/msgs/migrations/0001_initial.py
+-rw-r--r--   0 alexander   (501) staff       (20)      692 2021-02-20 16:00:18.000000 django_msgs-1.3.30/msgs/migrations/0002_timestamped_messages.py
+-rw-r--r--   0 alexander   (501) staff       (20)      795 2021-03-03 16:57:06.000000 django_msgs-1.3.30/msgs/migrations/0003_provider_fields_and_statuses.py
+-rw-r--r--   0 alexander   (501) staff       (20)      883 2021-03-26 16:56:33.000000 django_msgs-1.3.30/msgs/migrations/0004_default_templates_datamigration.py
+-rw-r--r--   0 alexander   (501) staff       (20)      778 2021-07-13 18:33:23.000000 django_msgs-1.3.30/msgs/migrations/0005_tpl_name_and_type.py
+-rw-r--r--   0 alexander   (501) staff       (20)      596 2021-07-13 18:33:23.000000 django_msgs-1.3.30/msgs/migrations/0006_tpl_fields_changed.py
+-rw-r--r--   0 alexander   (501) staff       (20)     7855 2021-07-15 16:08:11.000000 django_msgs-1.3.30/msgs/migrations/0007_auto_20210715_1608.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1301 2021-08-25 12:50:02.000000 django_msgs-1.3.30/msgs/migrations/0008_auto_20210825_1250.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2061 2022-02-06 11:05:48.000000 django_msgs-1.3.30/msgs/migrations/0009_auto_20220206_1105.py
+-rw-r--r--   0 alexander   (501) staff       (20)      719 2022-03-28 11:09:32.000000 django_msgs-1.3.30/msgs/migrations/0010_auto_20220328_1109.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1706 2022-06-13 09:02:27.000000 django_msgs-1.3.30/msgs/migrations/0011_auto_20220613_0857.py
+-rw-r--r--   0 alexander   (501) staff       (20)      764 2023-06-22 13:29:37.000000 django_msgs-1.3.30/msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py
+-rw-r--r--   0 alexander   (501) staff       (20)      767 2023-06-22 15:46:47.000000 django_msgs-1.3.30/msgs/migrations/0013_email_service_context_message_service_context_and_more.py
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2020-07-14 09:53:30.000000 django_msgs-1.3.30/msgs/migrations/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1997 2022-02-06 12:18:56.000000 django_msgs-1.3.30/msgs/mixins.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1276 2022-02-06 14:19:53.000000 django_msgs-1.3.30/msgs/models.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 19:07:26.830725 django_msgs-1.3.30/msgs/providers/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2020-10-02 08:58:26.000000 django_msgs-1.3.30/msgs/providers/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2698 2022-06-07 12:48:29.000000 django_msgs-1.3.30/msgs/providers/base.py
+-rw-r--r--   0 alexander   (501) staff       (20)      601 2021-07-15 17:03:12.000000 django_msgs-1.3.30/msgs/providers/dummy.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1826 2022-06-03 11:18:00.000000 django_msgs-1.3.30/msgs/providers/plivo.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1724 2021-07-15 17:11:26.000000 django_msgs-1.3.30/msgs/providers/sendgrid.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1709 2021-11-07 20:32:25.000000 django_msgs-1.3.30/msgs/providers/sendinblue.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2029 2021-04-16 12:11:11.000000 django_msgs-1.3.30/msgs/providers/sendinblue_sdk.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2235 2021-08-25 12:13:40.000000 django_msgs-1.3.30/msgs/providers/sendpulse.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1822 2022-05-12 11:04:22.000000 django_msgs-1.3.30/msgs/providers/telegram.py
+-rw-r--r--   0 alexander   (501) staff       (20)      482 2021-04-16 12:11:11.000000 django_msgs-1.3.30/msgs/providers/twilio.py
+-rw-r--r--   0 alexander   (501) staff       (20)      589 2021-04-16 12:11:11.000000 django_msgs-1.3.30/msgs/providers/voximplant.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1028 2022-06-07 12:15:13.000000 django_msgs-1.3.30/msgs/signals.py
+-rw-r--r--   0 alexander   (501) staff       (20)       60 2020-07-14 09:53:30.000000 django_msgs-1.3.30/msgs/tests.py
+-rw-r--r--   0 alexander   (501) staff       (20)      944 2021-07-16 15:56:46.000000 django_msgs-1.3.30/msgs/utils.py
+-rw-r--r--   0 alexander   (501) staff       (20)       63 2020-07-14 09:53:30.000000 django_msgs-1.3.30/msgs/views.py
+-rw-r--r--   0 alexander   (501) staff       (20)       79 2023-06-22 19:07:26.834582 django_msgs-1.3.30/setup.cfg
+-rw-r--r--   0 alexander   (501) staff       (20)      908 2023-06-22 19:07:00.000000 django_msgs-1.3.30/setup.py
```

### Comparing `django_msgs-1.3.29/LICENSE` & `django_msgs-1.3.30/LICENSE`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/PKG-INFO` & `django_msgs-1.3.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_msgs
-Version: 1.3.29
+Version: 1.3.30
 Summary: Emails and SMSs managing framework for Django
 Home-page: https://github.com/san4ezy/django_msgs
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django_msgs-1.3.29/README.md` & `django_msgs-1.3.30/README.md`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/config/settings.py` & `django_msgs-1.3.30/config/settings.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/config/urls.py` & `django_msgs-1.3.30/config/urls.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/django_msgs.egg-info/PKG-INFO` & `django_msgs-1.3.30/django_msgs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-msgs
-Version: 1.3.29
+Version: 1.3.30
 Summary: Emails and SMSs managing framework for Django
 Home-page: https://github.com/san4ezy/django_msgs
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django_msgs-1.3.29/django_msgs.egg-info/SOURCES.txt` & `django_msgs-1.3.30/django_msgs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/abstract/admin.py` & `django_msgs-1.3.30/msgs/abstract/admin.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/abstract/models.py` & `django_msgs-1.3.30/msgs/abstract/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     ):
         """Returns not saved instance"""
         template = cls.get_template(key=template)
         instance = cls(
             recipient=recipient,
             template=template,
             context=context,
+            service_context=service_context,
         )
         if related_to:
             instance.related_to = related_to
         cls.send_signal(BUILT_SIGNAL, instance=instance)
         return instance
 
     @classmethod
```

### Comparing `django_msgs-1.3.29/msgs/admin.py` & `django_msgs-1.3.30/msgs/admin.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0001_initial.py` & `django_msgs-1.3.30/msgs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0002_timestamped_messages.py` & `django_msgs-1.3.30/msgs/migrations/0002_timestamped_messages.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0003_provider_fields_and_statuses.py` & `django_msgs-1.3.30/msgs/migrations/0003_provider_fields_and_statuses.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0004_default_templates_datamigration.py` & `django_msgs-1.3.30/msgs/migrations/0004_default_templates_datamigration.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0005_tpl_name_and_type.py` & `django_msgs-1.3.30/msgs/migrations/0005_tpl_name_and_type.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0006_tpl_fields_changed.py` & `django_msgs-1.3.30/msgs/migrations/0006_tpl_fields_changed.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0007_auto_20210715_1608.py` & `django_msgs-1.3.30/msgs/migrations/0007_auto_20210715_1608.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0008_auto_20210825_1250.py` & `django_msgs-1.3.30/msgs/migrations/0008_auto_20210825_1250.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0009_auto_20220206_1105.py` & `django_msgs-1.3.30/msgs/migrations/0009_auto_20220206_1105.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0010_auto_20220328_1109.py` & `django_msgs-1.3.30/msgs/migrations/0010_auto_20220328_1109.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0011_auto_20220613_0857.py` & `django_msgs-1.3.30/msgs/migrations/0011_auto_20220613_0857.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py` & `django_msgs-1.3.30/msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/migrations/0013_email_service_context_message_service_context_and_more.py` & `django_msgs-1.3.30/msgs/migrations/0013_email_service_context_message_service_context_and_more.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/mixins.py` & `django_msgs-1.3.30/msgs/mixins.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/models.py` & `django_msgs-1.3.30/msgs/models.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/providers/base.py` & `django_msgs-1.3.30/msgs/providers/base.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/providers/dummy.py` & `django_msgs-1.3.30/msgs/providers/dummy.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/providers/plivo.py` & `django_msgs-1.3.30/msgs/providers/plivo.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/providers/sendgrid.py` & `django_msgs-1.3.30/msgs/providers/sendgrid.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/providers/sendinblue.py` & `django_msgs-1.3.30/msgs/providers/sendinblue.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/providers/sendinblue_sdk.py` & `django_msgs-1.3.30/msgs/providers/sendinblue_sdk.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/providers/sendpulse.py` & `django_msgs-1.3.30/msgs/providers/sendpulse.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/providers/telegram.py` & `django_msgs-1.3.30/msgs/providers/telegram.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/providers/voximplant.py` & `django_msgs-1.3.30/msgs/providers/voximplant.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/signals.py` & `django_msgs-1.3.30/msgs/signals.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/msgs/utils.py` & `django_msgs-1.3.30/msgs/utils.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.29/setup.py` & `django_msgs-1.3.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django_msgs",
-    version="1.3.29",
+    version="1.3.30",
     author="Alexander Yudkin",
     author_email="san4ezy@gmail.com",
     description="Emails and SMSs managing framework for Django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/san4ezy/django_msgs",
     packages=setuptools.find_packages(),
```

