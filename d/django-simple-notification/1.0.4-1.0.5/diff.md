# Comparing `tmp/django-simple-notification-1.0.4.tar.gz` & `tmp/django-simple-notification-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-notification-1.0.4.tar", last modified: Tue Jun  6 14:59:59 2023, max compression
+gzip compressed data, was "django-simple-notification-1.0.5.tar", last modified: Thu Jun 22 15:25:51 2023, max compression
```

## Comparing `django-simple-notification-1.0.4.tar` & `django-simple-notification-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.932165 django-simple-notification-1.0.4/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1147 2023-06-02 16:15:30.000000 django-simple-notification-1.0.4/LICENSE
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     3177 2023-06-06 14:59:59.931967 django-simple-notification-1.0.4/PKG-INFO
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2200 2023-06-06 14:57:14.000000 django-simple-notification-1.0.4/README.md
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.927899 django-simple-notification-1.0.4/django_simple_notification.egg-info/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     3177 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/PKG-INFO
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      747 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/SOURCES.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        1 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/dependency_links.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       12 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/requires.txt
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       14 2023-06-06 14:59:59.000000 django-simple-notification-1.0.4/django_simple_notification.egg-info/top_level.txt
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.930574 django-simple-notification-1.0.4/notifications/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.4/notifications/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      102 2023-06-01 21:25:10.000000 django-simple-notification-1.0.4/notifications/admin.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      158 2023-06-02 16:11:57.000000 django-simple-notification-1.0.4/notifications/apps.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1549 2023-06-01 21:49:27.000000 django-simple-notification-1.0.4/notifications/consumers.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      666 2023-06-02 17:38:44.000000 django-simple-notification-1.0.4/notifications/handlers.py
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.931036 django-simple-notification-1.0.4/notifications/migrations/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      957 2023-06-02 17:38:47.000000 django-simple-notification-1.0.4/notifications/migrations/0001_initial.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.4/notifications/migrations/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      384 2023-06-02 17:29:47.000000 django-simple-notification-1.0.4/notifications/models.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      174 2023-06-03 21:11:38.000000 django-simple-notification-1.0.4/notifications/routing.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      206 2023-06-02 17:36:40.000000 django-simple-notification-1.0.4/notifications/serializers.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      470 2023-06-02 16:01:56.000000 django-simple-notification-1.0.4/notifications/setup.py
-drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-06 14:59:59.931600 django-simple-notification-1.0.4/notifications/tests/
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 17:30:34.000000 django-simple-notification-1.0.4/notifications/tests/__init__.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      983 2023-06-02 17:32:01.000000 django-simple-notification-1.0.4/notifications/tests/test_models.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2709 2023-06-02 17:36:15.000000 django-simple-notification-1.0.4/notifications/tests/test_views.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       60 2023-05-22 21:14:08.000000 django-simple-notification-1.0.4/notifications/tests.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)      378 2023-06-01 21:51:55.000000 django-simple-notification-1.0.4/notifications/urls.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1262 2023-06-02 17:34:37.000000 django-simple-notification-1.0.4/notifications/views.py
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)       38 2023-06-06 14:59:59.932231 django-simple-notification-1.0.4/setup.cfg
--rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1299 2023-06-06 14:59:58.000000 django-simple-notification-1.0.4/setup.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-22 15:25:51.559153 django-simple-notification-1.0.5/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1147 2023-06-02 16:15:30.000000 django-simple-notification-1.0.5/LICENSE
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     3250 2023-06-22 15:25:51.558963 django-simple-notification-1.0.5/PKG-INFO
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2273 2023-06-22 15:23:31.000000 django-simple-notification-1.0.5/README.md
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-22 15:25:51.555114 django-simple-notification-1.0.5/django_simple_notification.egg-info/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     3250 2023-06-22 15:25:51.000000 django-simple-notification-1.0.5/django_simple_notification.egg-info/PKG-INFO
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      747 2023-06-22 15:25:51.000000 django-simple-notification-1.0.5/django_simple_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        1 2023-06-22 15:25:51.000000 django-simple-notification-1.0.5/django_simple_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       12 2023-06-22 15:25:51.000000 django-simple-notification-1.0.5/django_simple_notification.egg-info/requires.txt
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       14 2023-06-22 15:25:51.000000 django-simple-notification-1.0.5/django_simple_notification.egg-info/top_level.txt
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-22 15:25:51.557714 django-simple-notification-1.0.5/notifications/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.5/notifications/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      102 2023-06-01 21:25:10.000000 django-simple-notification-1.0.5/notifications/admin.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      158 2023-06-02 16:11:57.000000 django-simple-notification-1.0.5/notifications/apps.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1549 2023-06-01 21:49:27.000000 django-simple-notification-1.0.5/notifications/consumers.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      666 2023-06-02 17:38:44.000000 django-simple-notification-1.0.5/notifications/handlers.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-22 15:25:51.558147 django-simple-notification-1.0.5/notifications/migrations/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      957 2023-06-02 17:38:47.000000 django-simple-notification-1.0.5/notifications/migrations/0001_initial.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-05-22 21:14:08.000000 django-simple-notification-1.0.5/notifications/migrations/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      384 2023-06-02 17:29:47.000000 django-simple-notification-1.0.5/notifications/models.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      174 2023-06-03 21:11:38.000000 django-simple-notification-1.0.5/notifications/routing.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      206 2023-06-02 17:36:40.000000 django-simple-notification-1.0.5/notifications/serializers.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      470 2023-06-02 16:01:56.000000 django-simple-notification-1.0.5/notifications/setup.py
+drwxr-xr-x   0 mahmoudnasser   (501) staff       (20)        0 2023-06-22 15:25:51.558674 django-simple-notification-1.0.5/notifications/tests/
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)        0 2023-06-02 17:30:34.000000 django-simple-notification-1.0.5/notifications/tests/__init__.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      983 2023-06-02 17:32:01.000000 django-simple-notification-1.0.5/notifications/tests/test_models.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     2709 2023-06-02 17:36:15.000000 django-simple-notification-1.0.5/notifications/tests/test_views.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       60 2023-05-22 21:14:08.000000 django-simple-notification-1.0.5/notifications/tests.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)      378 2023-06-01 21:51:55.000000 django-simple-notification-1.0.5/notifications/urls.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1262 2023-06-02 17:34:37.000000 django-simple-notification-1.0.5/notifications/views.py
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)       38 2023-06-22 15:25:51.559210 django-simple-notification-1.0.5/setup.cfg
+-rw-r--r--   0 mahmoudnasser   (501) staff       (20)     1299 2023-06-22 15:24:15.000000 django-simple-notification-1.0.5/setup.py
```

### Comparing `django-simple-notification-1.0.4/LICENSE` & `django-simple-notification-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.4/PKG-INFO` & `django-simple-notification-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-notification
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simple user notification management for the Django web framework
 Home-page: https://github.com/MahmoudNasser01/django_simple_notification
 Author: Mahmoud Nasser
 Author-email: mahmoud.nasser.abdulhamed@gmail.com
 License: MIT
 Keywords: django notification simple custom
 Classifier: Environment :: Web Environment
@@ -18,14 +18,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# install
+
+```shell
+pip install django-simple-notification
+```
+
 # Usage
 
 ## 1. create notification events
 
 ```python
 
 from notifications.handlers import send_message
@@ -36,15 +42,15 @@
 ```python
 # function interface
 send_message(message:str, user:User, type:str)
 
 # logic behind it
 message: the text message to be sent to the user
 user: an instance of User model (the one who will recieve the notification)
-type: is a notification tag (you should create difrrent types in your system for different events)
+type: is a notification tag or type (you should create difrrent types in your system for different events)
 ```
 ## 2.fetch notifications using REST APIs
 
 ``notifications/all/``:GET : get all the notifications
 
 <br/><br/>
 ``notifications/mark/``:PUT : mark all notifications as read
@@ -58,15 +64,15 @@
 
 ## 3.how the client side recieve the message from the server via websocket
 ![img.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img.png?raw=true)
 
 
 # configration
 
-Note: make sure that django chanels is up and runnnig and also you django serves under ASGI
+Note: make sure that django channels is up and running and also you django serves under ASGI
 check this [url](https://channels.readthedocs.io/en/stable/installation.html) to configure django channels in your project
 
 in ``settings.py``
 ``` python
 INSTALLED_APPS = [
     ...
     'channels', # django channels needs to be installed
```

### Comparing `django-simple-notification-1.0.4/README.md` & `django-simple-notification-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# install
+
+```shell
+pip install django-simple-notification
+```
+
 # Usage
 
 ## 1. create notification events
 
 ```python
 
 from notifications.handlers import send_message
@@ -12,15 +18,15 @@
 ```python
 # function interface
 send_message(message:str, user:User, type:str)
 
 # logic behind it
 message: the text message to be sent to the user
 user: an instance of User model (the one who will recieve the notification)
-type: is a notification tag (you should create difrrent types in your system for different events)
+type: is a notification tag or type (you should create difrrent types in your system for different events)
 ```
 ## 2.fetch notifications using REST APIs
 
 ``notifications/all/``:GET : get all the notifications
 
 <br/><br/>
 ``notifications/mark/``:PUT : mark all notifications as read
@@ -34,15 +40,15 @@
 
 ## 3.how the client side recieve the message from the server via websocket
 ![img.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img.png?raw=true)
 
 
 # configration
 
-Note: make sure that django chanels is up and runnnig and also you django serves under ASGI
+Note: make sure that django channels is up and running and also you django serves under ASGI
 check this [url](https://channels.readthedocs.io/en/stable/installation.html) to configure django channels in your project
 
 in ``settings.py``
 ``` python
 INSTALLED_APPS = [
     ...
     'channels', # django channels needs to be installed
```

### Comparing `django-simple-notification-1.0.4/django_simple_notification.egg-info/PKG-INFO` & `django-simple-notification-1.0.5/django_simple_notification.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-notification
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simple user notification management for the Django web framework
 Home-page: https://github.com/MahmoudNasser01/django_simple_notification
 Author: Mahmoud Nasser
 Author-email: mahmoud.nasser.abdulhamed@gmail.com
 License: MIT
 Keywords: django notification simple custom
 Classifier: Environment :: Web Environment
@@ -18,14 +18,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# install
+
+```shell
+pip install django-simple-notification
+```
+
 # Usage
 
 ## 1. create notification events
 
 ```python
 
 from notifications.handlers import send_message
@@ -36,15 +42,15 @@
 ```python
 # function interface
 send_message(message:str, user:User, type:str)
 
 # logic behind it
 message: the text message to be sent to the user
 user: an instance of User model (the one who will recieve the notification)
-type: is a notification tag (you should create difrrent types in your system for different events)
+type: is a notification tag or type (you should create difrrent types in your system for different events)
 ```
 ## 2.fetch notifications using REST APIs
 
 ``notifications/all/``:GET : get all the notifications
 
 <br/><br/>
 ``notifications/mark/``:PUT : mark all notifications as read
@@ -58,15 +64,15 @@
 
 ## 3.how the client side recieve the message from the server via websocket
 ![img.png](https://github.com/MahmoudNasser01/django_simple_notification/blob/master/read_me_media/img.png?raw=true)
 
 
 # configration
 
-Note: make sure that django chanels is up and runnnig and also you django serves under ASGI
+Note: make sure that django channels is up and running and also you django serves under ASGI
 check this [url](https://channels.readthedocs.io/en/stable/installation.html) to configure django channels in your project
 
 in ``settings.py``
 ``` python
 INSTALLED_APPS = [
     ...
     'channels', # django channels needs to be installed
```

### Comparing `django-simple-notification-1.0.4/django_simple_notification.egg-info/SOURCES.txt` & `django-simple-notification-1.0.5/django_simple_notification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.4/notifications/consumers.py` & `django-simple-notification-1.0.5/notifications/consumers.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.4/notifications/handlers.py` & `django-simple-notification-1.0.5/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.4/notifications/migrations/0001_initial.py` & `django-simple-notification-1.0.5/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.4/notifications/tests/test_models.py` & `django-simple-notification-1.0.5/notifications/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.4/notifications/tests/test_views.py` & `django-simple-notification-1.0.5/notifications/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.4/notifications/views.py` & `django-simple-notification-1.0.5/notifications/views.py`

 * *Files identical despite different names*

### Comparing `django-simple-notification-1.0.4/setup.py` & `django-simple-notification-1.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-simple-notification',
-    version='1.0.4',
+    version='1.0.5',
     author='Mahmoud Nasser',
     author_email='mahmoud.nasser.abdulhamed@gmail.com',
     description='Simple user notification management for the Django web framework',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/MahmoudNasser01/django_simple_notification',
     license='MIT',
```

