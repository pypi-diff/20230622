# Comparing `tmp/django_willing_zg-0.5.1.tar.gz` & `tmp/django_willing_zg-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_willing_zg-0.5.1.tar", max compression
+gzip compressed data, was "django_willing_zg-0.5.2.tar", max compression
```

## Comparing `django_willing_zg-0.5.1.tar` & `django_willing_zg-0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      689 2023-04-06 16:35:36.667354 django_willing_zg-0.5.1/README.md
--rw-r--r--   0        0        0      657 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/__init__.py
--rw-r--r--   0        0        0       91 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/apps.py
--rw-r--r--   0        0        0     2136 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/mailer.py
--rw-r--r--   0        0        0      118 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/settings/__init__.py
--rw-r--r--   0        0        0      541 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/settings/cookies.py
--rw-r--r--   0        0        0      541 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/settings/email.py
--rw-r--r--   0        0        0      723 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/settings/jwt.py
--rw-r--r--   0        0        0     1147 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/settings/secrets.py
--rw-r--r--   0        0        0      446 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/templates/email/mlp_transactional_email.html
--rw-r--r--   0        0        0      356 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/templates/email/mlp_transactional_email.txt
--rw-r--r--   0        0        0      208 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/urls.py
--rw-r--r--   0        0        0      318 2023-04-06 16:35:36.671354 django_willing_zg-0.5.1/willing_zg/views.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 django_willing_zg-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      689 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/README.md
+-rw-r--r--   0        0        0      657 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/apps.py
+-rw-r--r--   0        0        0     2245 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/mailer.py
+-rw-r--r--   0        0        0      118 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/settings/__init__.py
+-rw-r--r--   0        0        0      541 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/settings/cookies.py
+-rw-r--r--   0        0        0      541 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/settings/email.py
+-rw-r--r--   0        0        0      723 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/settings/jwt.py
+-rw-r--r--   0        0        0     1147 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/settings/secrets.py
+-rw-r--r--   0        0        0      446 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/templates/email/mlp_transactional_email.html
+-rw-r--r--   0        0        0      356 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/templates/email/mlp_transactional_email.txt
+-rw-r--r--   0        0        0      208 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/urls.py
+-rw-r--r--   0        0        0      318 2023-06-22 16:43:22.560728 django_willing_zg-0.5.2/willing_zg/views.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 django_willing_zg-0.5.2/PKG-INFO
```

### Comparing `django_willing_zg-0.5.1/README.md` & `django_willing_zg-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `django_willing_zg-0.5.1/pyproject.toml` & `django_willing_zg-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-willing-zg"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 readme = "README.md"
 authors = ["Bequest, Inc. <oss@willing.com>"]
 packages = [
     { include = "willing_zg" },
 ]
```

### Comparing `django_willing_zg-0.5.1/willing_zg/mailer.py` & `django_willing_zg-0.5.2/willing_zg/mailer.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         subject,
         template,
         context,
         bcc=None,
         attachments=None,
         reply_to=None,
         from_email=None,
+        headers=None,
     ):
         if not len(to_emails):
             raise MailerError("no TO EMAIL provided")
 
         if not template:
             raise MailerError("no email template provided")
 
@@ -44,14 +45,15 @@
         message = EmailMultiAlternatives(
             subject=subject,
             body=email_text,
             from_email=from_email,
             to=to_emails,
             bcc=bcc,
             reply_to=reply_to,
+            headers=headers,
         )
 
         message.attach_alternative(email_html, "text/html")
         if attachments:
             for item in attachments:
                 message.attach(*item)
 
@@ -61,17 +63,19 @@
         # TODO: handle specific exceptions
         except Exception as e:
             # TODO: report exception
             print(e, vars(e))
             return False
 
     @classmethod
-    def send_account_notice(cls, user, subject, text):
+    def send_account_notice(cls, user, subject, text, *args, **kwargs):
         return cls.send_email(
             [user.email],
             f"Account Notice: {subject}",
             "mlp_transactional_email",
             {
                 "user": user,
                 "notice": text,
             },
+            *args,
+            **kwargs,
         )
```

### Comparing `django_willing_zg-0.5.1/willing_zg/settings/cookies.py` & `django_willing_zg-0.5.2/willing_zg/settings/cookies.py`

 * *Files identical despite different names*

### Comparing `django_willing_zg-0.5.1/willing_zg/settings/email.py` & `django_willing_zg-0.5.2/willing_zg/settings/email.py`

 * *Files identical despite different names*

### Comparing `django_willing_zg-0.5.1/willing_zg/settings/jwt.py` & `django_willing_zg-0.5.2/willing_zg/settings/jwt.py`

 * *Files identical despite different names*

### Comparing `django_willing_zg-0.5.1/willing_zg/settings/secrets.py` & `django_willing_zg-0.5.2/willing_zg/settings/secrets.py`

 * *Files identical despite different names*

### Comparing `django_willing_zg-0.5.1/PKG-INFO` & `django_willing_zg-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-willing-zg
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Author: Bequest, Inc.
 Author-email: oss@willing.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

