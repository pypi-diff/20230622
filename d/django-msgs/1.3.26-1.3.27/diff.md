# Comparing `tmp/django_msgs-1.3.26.tar.gz` & `tmp/django_msgs-1.3.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_msgs-1.3.26.tar", last modified: Sat Jun 18 17:35:23 2022, max compression
+gzip compressed data, was "django_msgs-1.3.27.tar", last modified: Thu Jun 22 14:01:59 2023, max compression
```

## Comparing `django_msgs-1.3.26.tar` & `django_msgs-1.3.27.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-06-18 17:35:23.472031 django_msgs-1.3.26/
--rw-r--r--   0 alexander   (501) staff       (20)     1073 2020-12-07 15:50:01.000000 django_msgs-1.3.26/LICENSE
--rw-r--r--   0 alexander   (501) staff       (20)       17 2020-12-07 15:39:16.000000 django_msgs-1.3.26/MANIFEST.in
--rw-r--r--   0 alexander   (501) staff       (20)     4815 2022-06-18 17:35:23.472184 django_msgs-1.3.26/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     3323 2021-09-23 06:41:03.000000 django_msgs-1.3.26/README.md
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-06-18 17:35:23.448140 django_msgs-1.3.26/config/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 19:37:37.000000 django_msgs-1.3.26/config/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.26/config/asgi.py
--rw-r--r--   0 alexander   (501) staff       (20)     4673 2022-05-30 08:36:00.000000 django_msgs-1.3.26/config/settings.py
--rw-r--r--   0 alexander   (501) staff       (20)      746 2021-07-13 19:50:10.000000 django_msgs-1.3.26/config/urls.py
--rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.26/config/wsgi.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-06-18 17:35:23.449646 django_msgs-1.3.26/django_msgs.egg-info/
--rw-r--r--   0 alexander   (501) staff       (20)     4815 2022-06-18 17:35:23.000000 django_msgs-1.3.26/django_msgs.egg-info/PKG-INFO
--rw-r--r--   0 alexander   (501) staff       (20)     1354 2022-06-18 17:35:23.000000 django_msgs-1.3.26/django_msgs.egg-info/SOURCES.txt
--rw-r--r--   0 alexander   (501) staff       (20)        1 2022-06-18 17:35:23.000000 django_msgs-1.3.26/django_msgs.egg-info/dependency_links.txt
--rw-r--r--   0 alexander   (501) staff       (20)       19 2022-06-18 17:35:23.000000 django_msgs-1.3.26/django_msgs.egg-info/requires.txt
--rw-r--r--   0 alexander   (501) staff       (20)       12 2022-06-18 17:35:23.000000 django_msgs-1.3.26/django_msgs.egg-info/top_level.txt
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-06-18 17:35:23.455943 django_msgs-1.3.26/msgs/
--rw-r--r--   0 alexander   (501) staff       (20)       43 2021-11-07 20:03:56.000000 django_msgs-1.3.26/msgs/__init__.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-06-18 17:35:23.457097 django_msgs-1.3.26/msgs/abstract/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 18:45:04.000000 django_msgs-1.3.26/msgs/abstract/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)      748 2022-03-28 10:36:36.000000 django_msgs-1.3.26/msgs/abstract/admin.py
--rw-r--r--   0 alexander   (501) staff       (20)     6281 2022-06-18 17:35:07.000000 django_msgs-1.3.26/msgs/abstract/models.py
--rw-r--r--   0 alexander   (501) staff       (20)      811 2021-11-07 20:06:22.000000 django_msgs-1.3.26/msgs/admin.py
--rw-r--r--   0 alexander   (501) staff       (20)      213 2021-11-07 20:03:56.000000 django_msgs-1.3.26/msgs/app.py
--rw-r--r--   0 alexander   (501) staff       (20)      201 2022-06-07 11:19:07.000000 django_msgs-1.3.26/msgs/exceptions.py
--rw-r--r--   0 alexander   (501) staff       (20)      255 2021-09-28 19:56:53.000000 django_msgs-1.3.26/msgs/helpers.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-06-18 17:35:23.465910 django_msgs-1.3.26/msgs/migrations/
--rw-r--r--   0 alexander   (501) staff       (20)     2344 2020-12-08 11:49:48.000000 django_msgs-1.3.26/msgs/migrations/0001_initial.py
--rw-r--r--   0 alexander   (501) staff       (20)      692 2021-02-20 16:00:18.000000 django_msgs-1.3.26/msgs/migrations/0002_timestamped_messages.py
--rw-r--r--   0 alexander   (501) staff       (20)      795 2021-03-03 16:57:06.000000 django_msgs-1.3.26/msgs/migrations/0003_provider_fields_and_statuses.py
--rw-r--r--   0 alexander   (501) staff       (20)      883 2021-03-26 16:56:33.000000 django_msgs-1.3.26/msgs/migrations/0004_default_templates_datamigration.py
--rw-r--r--   0 alexander   (501) staff       (20)      778 2021-07-13 18:33:23.000000 django_msgs-1.3.26/msgs/migrations/0005_tpl_name_and_type.py
--rw-r--r--   0 alexander   (501) staff       (20)      596 2021-07-13 18:33:23.000000 django_msgs-1.3.26/msgs/migrations/0006_tpl_fields_changed.py
--rw-r--r--   0 alexander   (501) staff       (20)     7855 2021-07-15 16:08:11.000000 django_msgs-1.3.26/msgs/migrations/0007_auto_20210715_1608.py
--rw-r--r--   0 alexander   (501) staff       (20)     1301 2021-08-25 12:50:02.000000 django_msgs-1.3.26/msgs/migrations/0008_auto_20210825_1250.py
--rw-r--r--   0 alexander   (501) staff       (20)     2061 2022-02-06 11:05:48.000000 django_msgs-1.3.26/msgs/migrations/0009_auto_20220206_1105.py
--rw-r--r--   0 alexander   (501) staff       (20)      719 2022-03-28 11:09:32.000000 django_msgs-1.3.26/msgs/migrations/0010_auto_20220328_1109.py
--rw-r--r--   0 alexander   (501) staff       (20)     1706 2022-06-13 09:02:27.000000 django_msgs-1.3.26/msgs/migrations/0011_auto_20220613_0857.py
--rw-r--r--   0 alexander   (501) staff       (20)        0 2020-07-14 09:53:30.000000 django_msgs-1.3.26/msgs/migrations/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     1997 2022-02-06 12:18:56.000000 django_msgs-1.3.26/msgs/mixins.py
--rw-r--r--   0 alexander   (501) staff       (20)     1276 2022-02-06 14:19:53.000000 django_msgs-1.3.26/msgs/models.py
-drwxr-xr-x   0 alexander   (501) staff       (20)        0 2022-06-18 17:35:23.471511 django_msgs-1.3.26/msgs/providers/
--rw-r--r--   0 alexander   (501) staff       (20)        0 2020-10-02 08:58:26.000000 django_msgs-1.3.26/msgs/providers/__init__.py
--rw-r--r--   0 alexander   (501) staff       (20)     2698 2022-06-07 12:48:29.000000 django_msgs-1.3.26/msgs/providers/base.py
--rw-r--r--   0 alexander   (501) staff       (20)      601 2021-07-15 17:03:12.000000 django_msgs-1.3.26/msgs/providers/dummy.py
--rw-r--r--   0 alexander   (501) staff       (20)     1826 2022-06-03 11:18:00.000000 django_msgs-1.3.26/msgs/providers/plivo.py
--rw-r--r--   0 alexander   (501) staff       (20)     1724 2021-07-15 17:11:26.000000 django_msgs-1.3.26/msgs/providers/sendgrid.py
--rw-r--r--   0 alexander   (501) staff       (20)     1709 2021-11-07 20:32:25.000000 django_msgs-1.3.26/msgs/providers/sendinblue.py
--rw-r--r--   0 alexander   (501) staff       (20)     2029 2021-04-16 12:11:11.000000 django_msgs-1.3.26/msgs/providers/sendinblue_sdk.py
--rw-r--r--   0 alexander   (501) staff       (20)     2235 2021-08-25 12:13:40.000000 django_msgs-1.3.26/msgs/providers/sendpulse.py
--rw-r--r--   0 alexander   (501) staff       (20)     1822 2022-05-12 11:04:22.000000 django_msgs-1.3.26/msgs/providers/telegram.py
--rw-r--r--   0 alexander   (501) staff       (20)      482 2021-04-16 12:11:11.000000 django_msgs-1.3.26/msgs/providers/twilio.py
--rw-r--r--   0 alexander   (501) staff       (20)      589 2021-04-16 12:11:11.000000 django_msgs-1.3.26/msgs/providers/voximplant.py
--rw-r--r--   0 alexander   (501) staff       (20)     1028 2022-06-07 12:15:13.000000 django_msgs-1.3.26/msgs/signals.py
--rw-r--r--   0 alexander   (501) staff       (20)       60 2020-07-14 09:53:30.000000 django_msgs-1.3.26/msgs/tests.py
--rw-r--r--   0 alexander   (501) staff       (20)      944 2021-07-16 15:56:46.000000 django_msgs-1.3.26/msgs/utils.py
--rw-r--r--   0 alexander   (501) staff       (20)       63 2020-07-14 09:53:30.000000 django_msgs-1.3.26/msgs/views.py
--rw-r--r--   0 alexander   (501) staff       (20)       79 2022-06-18 17:35:23.472590 django_msgs-1.3.26/setup.cfg
--rw-r--r--   0 alexander   (501) staff       (20)      908 2022-06-18 17:35:20.000000 django_msgs-1.3.26/setup.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 14:01:59.219743 django_msgs-1.3.27/
+-rw-r--r--   0 alexander   (501) staff       (20)     1073 2020-12-07 15:50:01.000000 django_msgs-1.3.27/LICENSE
+-rw-r--r--   0 alexander   (501) staff       (20)       17 2020-12-07 15:39:16.000000 django_msgs-1.3.27/MANIFEST.in
+-rw-r--r--   0 alexander   (501) staff       (20)     3910 2023-06-22 14:01:59.220173 django_msgs-1.3.27/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     3323 2021-09-23 06:41:03.000000 django_msgs-1.3.27/README.md
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 14:01:59.145712 django_msgs-1.3.27/config/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 19:37:37.000000 django_msgs-1.3.27/config/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.27/config/asgi.py
+-rw-r--r--   0 alexander   (501) staff       (20)     4673 2022-05-30 08:36:00.000000 django_msgs-1.3.27/config/settings.py
+-rw-r--r--   0 alexander   (501) staff       (20)      746 2021-07-13 19:50:10.000000 django_msgs-1.3.27/config/urls.py
+-rw-r--r--   0 alexander   (501) staff       (20)      387 2021-07-13 21:02:06.000000 django_msgs-1.3.27/config/wsgi.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 14:01:59.147379 django_msgs-1.3.27/django_msgs.egg-info/
+-rw-r--r--   0 alexander   (501) staff       (20)     3910 2023-06-22 14:01:59.000000 django_msgs-1.3.27/django_msgs.egg-info/PKG-INFO
+-rw-r--r--   0 alexander   (501) staff       (20)     1433 2023-06-22 14:01:59.000000 django_msgs-1.3.27/django_msgs.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander   (501) staff       (20)        1 2023-06-22 14:01:59.000000 django_msgs-1.3.27/django_msgs.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander   (501) staff       (20)       19 2023-06-22 14:01:59.000000 django_msgs-1.3.27/django_msgs.egg-info/requires.txt
+-rw-r--r--   0 alexander   (501) staff       (20)       12 2023-06-22 14:01:59.000000 django_msgs-1.3.27/django_msgs.egg-info/top_level.txt
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 14:01:59.154192 django_msgs-1.3.27/msgs/
+-rw-r--r--   0 alexander   (501) staff       (20)       43 2021-11-07 20:03:56.000000 django_msgs-1.3.27/msgs/__init__.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 14:01:59.155651 django_msgs-1.3.27/msgs/abstract/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2021-07-13 18:45:04.000000 django_msgs-1.3.27/msgs/abstract/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)      748 2022-03-28 10:36:36.000000 django_msgs-1.3.27/msgs/abstract/admin.py
+-rw-r--r--   0 alexander   (501) staff       (20)     6285 2023-06-22 12:41:17.000000 django_msgs-1.3.27/msgs/abstract/models.py
+-rw-r--r--   0 alexander   (501) staff       (20)      811 2021-11-07 20:06:22.000000 django_msgs-1.3.27/msgs/admin.py
+-rw-r--r--   0 alexander   (501) staff       (20)      213 2021-11-07 20:03:56.000000 django_msgs-1.3.27/msgs/app.py
+-rw-r--r--   0 alexander   (501) staff       (20)      201 2022-06-07 11:19:07.000000 django_msgs-1.3.27/msgs/exceptions.py
+-rw-r--r--   0 alexander   (501) staff       (20)      255 2021-09-28 19:56:53.000000 django_msgs-1.3.27/msgs/helpers.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 14:01:59.164466 django_msgs-1.3.27/msgs/migrations/
+-rw-r--r--   0 alexander   (501) staff       (20)     2344 2020-12-08 11:49:48.000000 django_msgs-1.3.27/msgs/migrations/0001_initial.py
+-rw-r--r--   0 alexander   (501) staff       (20)      692 2021-02-20 16:00:18.000000 django_msgs-1.3.27/msgs/migrations/0002_timestamped_messages.py
+-rw-r--r--   0 alexander   (501) staff       (20)      795 2021-03-03 16:57:06.000000 django_msgs-1.3.27/msgs/migrations/0003_provider_fields_and_statuses.py
+-rw-r--r--   0 alexander   (501) staff       (20)      883 2021-03-26 16:56:33.000000 django_msgs-1.3.27/msgs/migrations/0004_default_templates_datamigration.py
+-rw-r--r--   0 alexander   (501) staff       (20)      778 2021-07-13 18:33:23.000000 django_msgs-1.3.27/msgs/migrations/0005_tpl_name_and_type.py
+-rw-r--r--   0 alexander   (501) staff       (20)      596 2021-07-13 18:33:23.000000 django_msgs-1.3.27/msgs/migrations/0006_tpl_fields_changed.py
+-rw-r--r--   0 alexander   (501) staff       (20)     7855 2021-07-15 16:08:11.000000 django_msgs-1.3.27/msgs/migrations/0007_auto_20210715_1608.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1301 2021-08-25 12:50:02.000000 django_msgs-1.3.27/msgs/migrations/0008_auto_20210825_1250.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2061 2022-02-06 11:05:48.000000 django_msgs-1.3.27/msgs/migrations/0009_auto_20220206_1105.py
+-rw-r--r--   0 alexander   (501) staff       (20)      719 2022-03-28 11:09:32.000000 django_msgs-1.3.27/msgs/migrations/0010_auto_20220328_1109.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1706 2022-06-13 09:02:27.000000 django_msgs-1.3.27/msgs/migrations/0011_auto_20220613_0857.py
+-rw-r--r--   0 alexander   (501) staff       (20)      764 2023-06-22 13:29:37.000000 django_msgs-1.3.27/msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2020-07-14 09:53:30.000000 django_msgs-1.3.27/msgs/migrations/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1997 2022-02-06 12:18:56.000000 django_msgs-1.3.27/msgs/mixins.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1276 2022-02-06 14:19:53.000000 django_msgs-1.3.27/msgs/models.py
+drwxr-xr-x   0 alexander   (501) staff       (20)        0 2023-06-22 14:01:59.212812 django_msgs-1.3.27/msgs/providers/
+-rw-r--r--   0 alexander   (501) staff       (20)        0 2020-10-02 08:58:26.000000 django_msgs-1.3.27/msgs/providers/__init__.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2698 2022-06-07 12:48:29.000000 django_msgs-1.3.27/msgs/providers/base.py
+-rw-r--r--   0 alexander   (501) staff       (20)      601 2021-07-15 17:03:12.000000 django_msgs-1.3.27/msgs/providers/dummy.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1826 2022-06-03 11:18:00.000000 django_msgs-1.3.27/msgs/providers/plivo.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1724 2021-07-15 17:11:26.000000 django_msgs-1.3.27/msgs/providers/sendgrid.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1709 2021-11-07 20:32:25.000000 django_msgs-1.3.27/msgs/providers/sendinblue.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2029 2021-04-16 12:11:11.000000 django_msgs-1.3.27/msgs/providers/sendinblue_sdk.py
+-rw-r--r--   0 alexander   (501) staff       (20)     2235 2021-08-25 12:13:40.000000 django_msgs-1.3.27/msgs/providers/sendpulse.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1822 2022-05-12 11:04:22.000000 django_msgs-1.3.27/msgs/providers/telegram.py
+-rw-r--r--   0 alexander   (501) staff       (20)      482 2021-04-16 12:11:11.000000 django_msgs-1.3.27/msgs/providers/twilio.py
+-rw-r--r--   0 alexander   (501) staff       (20)      589 2021-04-16 12:11:11.000000 django_msgs-1.3.27/msgs/providers/voximplant.py
+-rw-r--r--   0 alexander   (501) staff       (20)     1028 2022-06-07 12:15:13.000000 django_msgs-1.3.27/msgs/signals.py
+-rw-r--r--   0 alexander   (501) staff       (20)       60 2020-07-14 09:53:30.000000 django_msgs-1.3.27/msgs/tests.py
+-rw-r--r--   0 alexander   (501) staff       (20)      944 2021-07-16 15:56:46.000000 django_msgs-1.3.27/msgs/utils.py
+-rw-r--r--   0 alexander   (501) staff       (20)       63 2020-07-14 09:53:30.000000 django_msgs-1.3.27/msgs/views.py
+-rw-r--r--   0 alexander   (501) staff       (20)       79 2023-06-22 14:01:59.220858 django_msgs-1.3.27/setup.cfg
+-rw-r--r--   0 alexander   (501) staff       (20)      908 2023-06-22 13:30:09.000000 django_msgs-1.3.27/setup.py
```

### Comparing `django_msgs-1.3.26/LICENSE` & `django_msgs-1.3.27/LICENSE`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/PKG-INFO` & `django_msgs-1.3.27/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,128 +1,128 @@
 Metadata-Version: 2.1
 Name: django_msgs
-Version: 1.3.26
+Version: 1.3.27
 Summary: Emails and SMSs managing framework for Django
 Home-page: https://github.com/san4ezy/django_msgs
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
-License: UNKNOWN
-Description: # Django MSGS
-        
-        This small framework provides you with a set of flexible tools for implementing the message sending functionality. \
-        Any type of informational messaging are available: emails, sms, telegram...
-        
-        ## Installation
-        
-        ```
-        pip install django-msgs
-        ```
-        
-        settings.py:
-        ```
-        INSTALLED_APPS = [
-        ...
-        'msgs',
-        ]
-        ```
-        
-        Apply the migrations for creation the tables at your database:
-        ```
-        ./manage.py migrate msgs
-        ```
-        
-        ## Structure
-        
-        Django MSGS contains two common data models: Message and Template. The first one stores your messages, the second 
-        one describes the messaging templates. \
-        If you need new type of email, you should create new Tpl with the HTML inside. After that you can use it for sending 
-        messages with this template. \
-        By default Django MSGS provide you with three proxy models: `Email`, `SMS` and `Message`. You can customize them on your taste. \
-        Also you can find a template model for any type of message: `EmailTemplate`, `SMSTemplate` and `MessageTemplate`.
-        
-        ## Quick example
-        
-        Look at the admin interface and create some templates for your messages.
-        
-        Now we can use them for sending messages:
-        
-        ```python
-        from msgs.models import Email
-        
-        template_key = 'registration'  # a unique key for search the template
-        Email.create(
-            template=template_key,
-            recipient='john.doe@example.com',
-            context={
-                'name': 'John Doe',
-                'link': 'https://example.com/registration',
-            },
-        ).send()
-        ```
-        
-        If you need i18n options, you can just inherit the existing template models with adding the 
-        needed language fields and use the `send` method with a language prefix as you need.
-        
-        Let's look at the one more very useful attribute -- `related_to`. This library uses a generic foreign key for linking messages with another objects. You should provide this object when you create a message.
-        
-        ```python
-        from msgs.models import SMS
-        
-        instance = new_user  # this is an object you want to link with the email
-        
-        SMS.create(
-            template='registration',
-            recipient='1234567890',
-            context={
-                'name': 'John Doe',
-                'link': 'https://example.com/registration',
-            },
-            related_to=instance,  # it does the trick
-        ).send()
-        ```
-        
-        ## Providers
-        
-        The Django MSGS works with multiple providers. All of them are placed at the `providers` folder. 
-        So you can discover them and choose what you need.
-        
-        You can find the `BaseProvider` class, hence nobody can stop you to build your own provider. 
-        
-        ## Settings
-        
-        ```python
-        MSGS = {
-            'providers': {
-                'sendgrid': {
-                    'backend': 'msgs.providers.sendgrid.SendgridProvider',  # use SendGrid Provider
-                    'options': {
-                        'is_active': True,  # turn on/off sending messages
-                        'api_key': 'api-key',
-                        'sender': 'sender@email.com',
-                    },
-                },
-                'telegram': {
-                    'backend': 'msgs.providers.telegram.TelegramProvider',
-                    'options': {
-                        'is_active': False,
-                        'token': 'telegram-bot-token',
-                        'chat': 'chat-id',
-                    },
-                },
-            },
-            'options': {
-                'default_language': 'en',
-            },
-            'development': 'telegram',  # what use on development (not works properly, be careful)
-            'email': 'sendgrid',  # use SendGrid Provider for sending emails
-            'sms': 'telegram',  # use Telegram Provider for sending sms
-        }
-        ```
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django MSGS
+
+This small framework provides you with a set of flexible tools for implementing the message sending functionality. \
+Any type of informational messaging are available: emails, sms, telegram...
+
+## Installation
+
+```
+pip install django-msgs
+```
+
+settings.py:
+```
+INSTALLED_APPS = [
+...
+'msgs',
+]
+```
+
+Apply the migrations for creation the tables at your database:
+```
+./manage.py migrate msgs
+```
+
+## Structure
+
+Django MSGS contains two common data models: Message and Template. The first one stores your messages, the second 
+one describes the messaging templates. \
+If you need new type of email, you should create new Tpl with the HTML inside. After that you can use it for sending 
+messages with this template. \
+By default Django MSGS provide you with three proxy models: `Email`, `SMS` and `Message`. You can customize them on your taste. \
+Also you can find a template model for any type of message: `EmailTemplate`, `SMSTemplate` and `MessageTemplate`.
+
+## Quick example
+
+Look at the admin interface and create some templates for your messages.
+
+Now we can use them for sending messages:
+
+```python
+from msgs.models import Email
+
+template_key = 'registration'  # a unique key for search the template
+Email.create(
+    template=template_key,
+    recipient='john.doe@example.com',
+    context={
+        'name': 'John Doe',
+        'link': 'https://example.com/registration',
+    },
+).send()
+```
+
+If you need i18n options, you can just inherit the existing template models with adding the 
+needed language fields and use the `send` method with a language prefix as you need.
+
+Let's look at the one more very useful attribute -- `related_to`. This library uses a generic foreign key for linking messages with another objects. You should provide this object when you create a message.
+
+```python
+from msgs.models import SMS
+
+instance = new_user  # this is an object you want to link with the email
+
+SMS.create(
+    template='registration',
+    recipient='1234567890',
+    context={
+        'name': 'John Doe',
+        'link': 'https://example.com/registration',
+    },
+    related_to=instance,  # it does the trick
+).send()
+```
+
+## Providers
+
+The Django MSGS works with multiple providers. All of them are placed at the `providers` folder. 
+So you can discover them and choose what you need.
+
+You can find the `BaseProvider` class, hence nobody can stop you to build your own provider. 
+
+## Settings
+
+```python
+MSGS = {
+    'providers': {
+        'sendgrid': {
+            'backend': 'msgs.providers.sendgrid.SendgridProvider',  # use SendGrid Provider
+            'options': {
+                'is_active': True,  # turn on/off sending messages
+                'api_key': 'api-key',
+                'sender': 'sender@email.com',
+            },
+        },
+        'telegram': {
+            'backend': 'msgs.providers.telegram.TelegramProvider',
+            'options': {
+                'is_active': False,
+                'token': 'telegram-bot-token',
+                'chat': 'chat-id',
+            },
+        },
+    },
+    'options': {
+        'default_language': 'en',
+    },
+    'development': 'telegram',  # what use on development (not works properly, be careful)
+    'email': 'sendgrid',  # use SendGrid Provider for sending emails
+    'sms': 'telegram',  # use Telegram Provider for sending sms
+}
+```
```

### Comparing `django_msgs-1.3.26/README.md` & `django_msgs-1.3.27/README.md`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/config/settings.py` & `django_msgs-1.3.27/config/settings.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/config/urls.py` & `django_msgs-1.3.27/config/urls.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/django_msgs.egg-info/PKG-INFO` & `django_msgs-1.3.27/django_msgs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,128 +1,128 @@
 Metadata-Version: 2.1
 Name: django-msgs
-Version: 1.3.26
+Version: 1.3.27
 Summary: Emails and SMSs managing framework for Django
 Home-page: https://github.com/san4ezy/django_msgs
 Author: Alexander Yudkin
 Author-email: san4ezy@gmail.com
-License: UNKNOWN
-Description: # Django MSGS
-        
-        This small framework provides you with a set of flexible tools for implementing the message sending functionality. \
-        Any type of informational messaging are available: emails, sms, telegram...
-        
-        ## Installation
-        
-        ```
-        pip install django-msgs
-        ```
-        
-        settings.py:
-        ```
-        INSTALLED_APPS = [
-        ...
-        'msgs',
-        ]
-        ```
-        
-        Apply the migrations for creation the tables at your database:
-        ```
-        ./manage.py migrate msgs
-        ```
-        
-        ## Structure
-        
-        Django MSGS contains two common data models: Message and Template. The first one stores your messages, the second 
-        one describes the messaging templates. \
-        If you need new type of email, you should create new Tpl with the HTML inside. After that you can use it for sending 
-        messages with this template. \
-        By default Django MSGS provide you with three proxy models: `Email`, `SMS` and `Message`. You can customize them on your taste. \
-        Also you can find a template model for any type of message: `EmailTemplate`, `SMSTemplate` and `MessageTemplate`.
-        
-        ## Quick example
-        
-        Look at the admin interface and create some templates for your messages.
-        
-        Now we can use them for sending messages:
-        
-        ```python
-        from msgs.models import Email
-        
-        template_key = 'registration'  # a unique key for search the template
-        Email.create(
-            template=template_key,
-            recipient='john.doe@example.com',
-            context={
-                'name': 'John Doe',
-                'link': 'https://example.com/registration',
-            },
-        ).send()
-        ```
-        
-        If you need i18n options, you can just inherit the existing template models with adding the 
-        needed language fields and use the `send` method with a language prefix as you need.
-        
-        Let's look at the one more very useful attribute -- `related_to`. This library uses a generic foreign key for linking messages with another objects. You should provide this object when you create a message.
-        
-        ```python
-        from msgs.models import SMS
-        
-        instance = new_user  # this is an object you want to link with the email
-        
-        SMS.create(
-            template='registration',
-            recipient='1234567890',
-            context={
-                'name': 'John Doe',
-                'link': 'https://example.com/registration',
-            },
-            related_to=instance,  # it does the trick
-        ).send()
-        ```
-        
-        ## Providers
-        
-        The Django MSGS works with multiple providers. All of them are placed at the `providers` folder. 
-        So you can discover them and choose what you need.
-        
-        You can find the `BaseProvider` class, hence nobody can stop you to build your own provider. 
-        
-        ## Settings
-        
-        ```python
-        MSGS = {
-            'providers': {
-                'sendgrid': {
-                    'backend': 'msgs.providers.sendgrid.SendgridProvider',  # use SendGrid Provider
-                    'options': {
-                        'is_active': True,  # turn on/off sending messages
-                        'api_key': 'api-key',
-                        'sender': 'sender@email.com',
-                    },
-                },
-                'telegram': {
-                    'backend': 'msgs.providers.telegram.TelegramProvider',
-                    'options': {
-                        'is_active': False,
-                        'token': 'telegram-bot-token',
-                        'chat': 'chat-id',
-                    },
-                },
-            },
-            'options': {
-                'default_language': 'en',
-            },
-            'development': 'telegram',  # what use on development (not works properly, be careful)
-            'email': 'sendgrid',  # use SendGrid Provider for sending emails
-            'sms': 'telegram',  # use Telegram Provider for sending sms
-        }
-        ```
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django MSGS
+
+This small framework provides you with a set of flexible tools for implementing the message sending functionality. \
+Any type of informational messaging are available: emails, sms, telegram...
+
+## Installation
+
+```
+pip install django-msgs
+```
+
+settings.py:
+```
+INSTALLED_APPS = [
+...
+'msgs',
+]
+```
+
+Apply the migrations for creation the tables at your database:
+```
+./manage.py migrate msgs
+```
+
+## Structure
+
+Django MSGS contains two common data models: Message and Template. The first one stores your messages, the second 
+one describes the messaging templates. \
+If you need new type of email, you should create new Tpl with the HTML inside. After that you can use it for sending 
+messages with this template. \
+By default Django MSGS provide you with three proxy models: `Email`, `SMS` and `Message`. You can customize them on your taste. \
+Also you can find a template model for any type of message: `EmailTemplate`, `SMSTemplate` and `MessageTemplate`.
+
+## Quick example
+
+Look at the admin interface and create some templates for your messages.
+
+Now we can use them for sending messages:
+
+```python
+from msgs.models import Email
+
+template_key = 'registration'  # a unique key for search the template
+Email.create(
+    template=template_key,
+    recipient='john.doe@example.com',
+    context={
+        'name': 'John Doe',
+        'link': 'https://example.com/registration',
+    },
+).send()
+```
+
+If you need i18n options, you can just inherit the existing template models with adding the 
+needed language fields and use the `send` method with a language prefix as you need.
+
+Let's look at the one more very useful attribute -- `related_to`. This library uses a generic foreign key for linking messages with another objects. You should provide this object when you create a message.
+
+```python
+from msgs.models import SMS
+
+instance = new_user  # this is an object you want to link with the email
+
+SMS.create(
+    template='registration',
+    recipient='1234567890',
+    context={
+        'name': 'John Doe',
+        'link': 'https://example.com/registration',
+    },
+    related_to=instance,  # it does the trick
+).send()
+```
+
+## Providers
+
+The Django MSGS works with multiple providers. All of them are placed at the `providers` folder. 
+So you can discover them and choose what you need.
+
+You can find the `BaseProvider` class, hence nobody can stop you to build your own provider. 
+
+## Settings
+
+```python
+MSGS = {
+    'providers': {
+        'sendgrid': {
+            'backend': 'msgs.providers.sendgrid.SendgridProvider',  # use SendGrid Provider
+            'options': {
+                'is_active': True,  # turn on/off sending messages
+                'api_key': 'api-key',
+                'sender': 'sender@email.com',
+            },
+        },
+        'telegram': {
+            'backend': 'msgs.providers.telegram.TelegramProvider',
+            'options': {
+                'is_active': False,
+                'token': 'telegram-bot-token',
+                'chat': 'chat-id',
+            },
+        },
+    },
+    'options': {
+        'default_language': 'en',
+    },
+    'development': 'telegram',  # what use on development (not works properly, be careful)
+    'email': 'sendgrid',  # use SendGrid Provider for sending emails
+    'sms': 'telegram',  # use Telegram Provider for sending sms
+}
+```
```

### Comparing `django_msgs-1.3.26/django_msgs.egg-info/SOURCES.txt` & `django_msgs-1.3.27/django_msgs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 msgs/migrations/0005_tpl_name_and_type.py
 msgs/migrations/0006_tpl_fields_changed.py
 msgs/migrations/0007_auto_20210715_1608.py
 msgs/migrations/0008_auto_20210825_1250.py
 msgs/migrations/0009_auto_20220206_1105.py
 msgs/migrations/0010_auto_20220328_1109.py
 msgs/migrations/0011_auto_20220613_0857.py
+msgs/migrations/0012_alter_email_object_id_alter_message_object_id_and_more.py
 msgs/migrations/__init__.py
 msgs/providers/__init__.py
 msgs/providers/base.py
 msgs/providers/dummy.py
 msgs/providers/plivo.py
 msgs/providers/sendgrid.py
 msgs/providers/sendinblue.py
```

### Comparing `django_msgs-1.3.26/msgs/abstract/admin.py` & `django_msgs-1.3.27/msgs/abstract/admin.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/abstract/models.py` & `django_msgs-1.3.27/msgs/abstract/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     provider_response = models.CharField(max_length=256, **NULLABLE)
 
     created_at = models.DateTimeField(auto_now_add=True, **NULLABLE)
     modified_at = models.DateTimeField(auto_now=True, **NULLABLE)
     sent_at = models.DateTimeField(**NULLABLE)
 
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE, **NULLABLE)
-    object_id = models.PositiveIntegerField(**NULLABLE)
+    object_id = models.CharField(max_length=64, **NULLABLE)
     related_to = GenericForeignKey('content_type', 'object_id')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__origin_status = self.status
 
     def __str__(self):
```

### Comparing `django_msgs-1.3.26/msgs/admin.py` & `django_msgs-1.3.27/msgs/admin.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0001_initial.py` & `django_msgs-1.3.27/msgs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0002_timestamped_messages.py` & `django_msgs-1.3.27/msgs/migrations/0002_timestamped_messages.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0003_provider_fields_and_statuses.py` & `django_msgs-1.3.27/msgs/migrations/0003_provider_fields_and_statuses.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0004_default_templates_datamigration.py` & `django_msgs-1.3.27/msgs/migrations/0004_default_templates_datamigration.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0005_tpl_name_and_type.py` & `django_msgs-1.3.27/msgs/migrations/0005_tpl_name_and_type.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0006_tpl_fields_changed.py` & `django_msgs-1.3.27/msgs/migrations/0006_tpl_fields_changed.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0007_auto_20210715_1608.py` & `django_msgs-1.3.27/msgs/migrations/0007_auto_20210715_1608.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0008_auto_20210825_1250.py` & `django_msgs-1.3.27/msgs/migrations/0008_auto_20210825_1250.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0009_auto_20220206_1105.py` & `django_msgs-1.3.27/msgs/migrations/0009_auto_20220206_1105.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0010_auto_20220328_1109.py` & `django_msgs-1.3.27/msgs/migrations/0010_auto_20220328_1109.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/migrations/0011_auto_20220613_0857.py` & `django_msgs-1.3.27/msgs/migrations/0011_auto_20220613_0857.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/mixins.py` & `django_msgs-1.3.27/msgs/mixins.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/models.py` & `django_msgs-1.3.27/msgs/models.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/providers/base.py` & `django_msgs-1.3.27/msgs/providers/base.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/providers/dummy.py` & `django_msgs-1.3.27/msgs/providers/dummy.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/providers/plivo.py` & `django_msgs-1.3.27/msgs/providers/plivo.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/providers/sendgrid.py` & `django_msgs-1.3.27/msgs/providers/sendgrid.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/providers/sendinblue.py` & `django_msgs-1.3.27/msgs/providers/sendinblue.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/providers/sendinblue_sdk.py` & `django_msgs-1.3.27/msgs/providers/sendinblue_sdk.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/providers/sendpulse.py` & `django_msgs-1.3.27/msgs/providers/sendpulse.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/providers/telegram.py` & `django_msgs-1.3.27/msgs/providers/telegram.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/providers/voximplant.py` & `django_msgs-1.3.27/msgs/providers/voximplant.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/signals.py` & `django_msgs-1.3.27/msgs/signals.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/msgs/utils.py` & `django_msgs-1.3.27/msgs/utils.py`

 * *Files identical despite different names*

### Comparing `django_msgs-1.3.26/setup.py` & `django_msgs-1.3.27/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django_msgs",
-    version="1.3.26",
+    version="1.3.27",
     author="Alexander Yudkin",
     author_email="san4ezy@gmail.com",
     description="Emails and SMSs managing framework for Django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/san4ezy/django_msgs",
     packages=setuptools.find_packages(),
```

