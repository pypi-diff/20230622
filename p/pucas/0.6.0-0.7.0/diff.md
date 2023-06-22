# Comparing `tmp/pucas-0.6.0.tar.gz` & `tmp/pucas-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pucas-0.6.0.tar", last modified: Tue Aug  6 13:41:33 2019, max compression
+gzip compressed data, was "dist/pucas-0.7.0.tar", last modified: Mon Aug 31 18:19:48 2020, max compression
```

## Comparing `pucas-0.6.0.tar` & `pucas-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2019-08-06 13:41:33.000000 pucas-0.6.0/
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas/
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      467 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/signals.py
--rwxr-xr-x   0 rkoeser  (2011409658) admin       (80)     4780 2019-08-06 13:37:58.000000 pucas-0.6.0/pucas/ldap.py
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas/management/
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)        0 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/management/__init__.py
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas/management/commands/
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)        0 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/management/commands/__init__.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     2208 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/management/commands/createcasuser.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     1258 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/management/commands/ldapsearch.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      305 2019-08-06 13:39:02.000000 pucas-0.6.0/pucas/__init__.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      136 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/apps.py
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas/static/
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas/static/pucas/
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     1281 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/static/pucas/pu-login.css
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas/templates/
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas/templates/pucas/
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      297 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/templates/pucas/sample-admin-login.html
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      308 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/templates/pucas/pu-cas-login.html
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      364 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/templates/pucas/sample-pu-login.html
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      205 2017-07-27 20:33:12.000000 pucas-0.6.0/pucas/templates/pucas/cas-login.html
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      330 2019-08-06 13:37:58.000000 pucas-0.6.0/pucas/cas_urls.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)    13662 2019-08-06 13:37:58.000000 pucas-0.6.0/pucas/tests.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     9518 2019-08-06 13:41:33.000000 pucas-0.6.0/PKG-INFO
-drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas.egg-info/
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     9518 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas.egg-info/PKG-INFO
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      637 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas.egg-info/SOURCES.txt
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)       77 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas.egg-info/requires.txt
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)        6 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas.egg-info/top_level.txt
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)        1 2019-08-06 13:41:33.000000 pucas-0.6.0/pucas.egg-info/dependency_links.txt
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)    11357 2017-01-12 17:33:13.000000 pucas-0.6.0/LICENSE
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      103 2017-07-27 20:33:12.000000 pucas-0.6.0/MANIFEST.in
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     2157 2019-08-06 13:37:58.000000 pucas-0.6.0/setup.py
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)      129 2019-08-06 13:41:33.000000 pucas-0.6.0/setup.cfg
--rw-r--r--   0 rkoeser  (2011409658) admin       (80)     6535 2019-08-06 13:39:02.000000 pucas-0.6.0/README.rst
+drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-08-31 18:19:48.000000 pucas-0.7.0/
+drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas/
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      467 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/signals.py
+-rwxr-xr-x   0 rkoeser  (2011409658) admin       (80)     4780 2019-08-06 13:37:58.000000 pucas-0.7.0/pucas/ldap.py
+drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas/management/
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)        0 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/management/__init__.py
+drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas/management/commands/
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)        0 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/management/commands/__init__.py
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)     1987 2020-08-31 17:55:45.000000 pucas-0.7.0/pucas/management/commands/createcasuser.py
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)     1258 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/management/commands/ldapsearch.py
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      305 2020-08-31 18:19:39.000000 pucas-0.7.0/pucas/__init__.py
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      136 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/apps.py
+drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas/static/
+drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas/static/pucas/
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)     1281 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/static/pucas/pu-login.css
+drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas/templates/
+drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas/templates/pucas/
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      297 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/templates/pucas/sample-admin-login.html
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      308 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/templates/pucas/pu-cas-login.html
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      364 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/templates/pucas/sample-pu-login.html
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      205 2017-07-27 20:33:12.000000 pucas-0.7.0/pucas/templates/pucas/cas-login.html
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      330 2019-08-06 13:37:58.000000 pucas-0.7.0/pucas/cas_urls.py
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)    13574 2020-08-31 17:55:19.000000 pucas-0.7.0/pucas/tests.py
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)     9636 2020-08-31 18:19:48.000000 pucas-0.7.0/PKG-INFO
+drwxr-xr-x   0 rkoeser  (2011409658) admin       (80)        0 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas.egg-info/
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)     9636 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas.egg-info/PKG-INFO
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      637 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas.egg-info/SOURCES.txt
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)       77 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas.egg-info/requires.txt
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)        6 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas.egg-info/top_level.txt
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)        1 2020-08-31 18:19:48.000000 pucas-0.7.0/pucas.egg-info/dependency_links.txt
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)    11357 2017-01-12 17:33:13.000000 pucas-0.7.0/LICENSE
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      103 2017-07-27 20:33:12.000000 pucas-0.7.0/MANIFEST.in
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)     2126 2020-08-31 18:19:39.000000 pucas-0.7.0/setup.py
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)      129 2020-08-31 18:19:48.000000 pucas-0.7.0/setup.cfg
+-rw-r--r--   0 rkoeser  (2011409658) admin       (80)     6645 2020-08-31 17:55:46.000000 pucas-0.7.0/README.rst
```

### Comparing `pucas-0.6.0/pucas/ldap.py` & `pucas-0.7.0/pucas/ldap.py`

 * *Files identical despite different names*

### Comparing `pucas-0.6.0/pucas/management/commands/createcasuser.py` & `pucas-0.7.0/pucas/management/commands/createcasuser.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,23 +43,15 @@
                 if admin or staff:
                     user.is_staff = True
                     if admin:
                         user.is_superuser = True
                     user.save()
 
                 self.stdout.write(
-                    self.style_success("%s user '%s'"  \
+                    self.style.SUCCESS(
+                        "%s user '%s'"
                         % ('Created' if created else 'Updated', netid)))
 
             except LDAPSearchException:
                 self.stderr.write(
-                    self.style.ERROR("LDAP information for '%s' not found"  \
-                        % netid))
-
-    def style_success(self, msg):
-        # workaround to support django 1.8 - style.SUCCESS
-        # only added in django 1.9
-        if hasattr(self.style, 'SUCCESS'):
-            return self.style.SUCCESS(msg)
-        else:
-            return msg
-
+                    self.style.ERROR("LDAP information for '%s' not found"
+                                     % netid))
```

### Comparing `pucas-0.6.0/pucas/management/commands/ldapsearch.py` & `pucas-0.7.0/pucas/management/commands/ldapsearch.py`

 * *Files identical despite different names*

### Comparing `pucas-0.6.0/pucas/static/pucas/pu-login.css` & `pucas-0.7.0/pucas/static/pucas/pu-login.css`

 * *Files identical despite different names*

### Comparing `pucas-0.6.0/pucas/tests.py` & `pucas-0.7.0/pucas/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-try:
-    # python 3
-    from unittest import mock
-except ImportError:
-    # python 2.7
-    import mock
+from io import StringIO
+from unittest import mock
+
 from django.conf import settings
 from django.core.management import call_command
 from django.test import TestCase, override_settings
-from django.utils.six import StringIO
-from ldap3.core.exceptions import LDAPException, LDAPCursorError
+from ldap3.core.exceptions import LDAPCursorError, LDAPException
 import pytest
 
 from pucas.ldap import LDAPSearch, LDAPSearchException, \
     user_info_from_ldap
+from pucas.management.commands import createcasuser, ldapsearch
 from pucas.signals import cas_login
-from pucas.management.commands import ldapsearch, createcasuser
 
 
 class MockLDAPInfo(object):
     '''Simulate ldap result object with ldap3 specific behavior for getattr'''
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
+
     def __getattr__(self, attr):
         # __getattr__ only gets called when the default attribute access
         # falls through, so in this case, we always want that to raise the
         # cursor error
         raise LDAPCursorError
 
+
 class TestMockLDAPInfo(TestCase):
 
     def test_init(self):
         mock_info = MockLDAPInfo(a=1, b=2)
         assert mock_info.a == 1
         assert mock_info.b == 2
```

### Comparing `pucas-0.6.0/PKG-INFO` & `pucas-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pucas
-Version: 0.6.0
+Version: 0.7.0
 Summary: Django app to login with CAS and populate user accounts with LDAP.
 Home-page: https://github.com/Princeton-CDH/django-pucas
 Author: CDH @ Princeton
 Author-email: digitalhumanities@princeton.edu
 License: Apache License, Version 2.0
 Description: django-pucas
         ============
@@ -21,28 +21,34 @@
            :target: https://www.codefactor.io/repository/github/princeton-cdh/django-pucas
            :alt: CodeFactor
         
         .. image:: https://requires.io/github/Princeton-CDH/django-pucas/requirements.svg?branch=master
              :target: https://requires.io/github/Princeton-CDH/django-pucas/requirements/?branch=master
              :alt: Requirements Status
         
+        .. image:: https://img.shields.io/pypi/pyversions/viapy
+           :alt: PyPI - Python Version
+        
+        .. image:: https://img.shields.io/pypi/djversions/viapy
+           :alt: PyPI - Django Version
+        
         **django-pucas** is a reusable `Django`_ application to simplify logging
         into a Django application with CAS using `django-cas-ng`_.  Login and
         creation of user accounts is handled by django-cas-ng; pucas adds
         support for prepopulating user account data based on an LDAP search.
         
         *pucas* should be pronounced like *pookas* for the Celtic spirit creature.
         
         .. _Django: https://www.djangoproject.com/
         .. _django-cas-ng: https://github.com/mingchen/django-cas-ng
         
-        **django-pucas** is tested under:
+        **django-pucas** is tested against:
         
-        * Django ``1.8-2.2``
-        * Python ``2.7, 3.5-3.7`` (excluding ``2.7`` for Django ``2+``)
+        * Django ``1.11-3.1``
+        * Python ``3.5-3.8``
         
         **django-pucas** requires **django-cas-ng** 3.6 or greater.
         
         Installation
         ------------
         
         Use pip to install::
@@ -133,16 +139,15 @@
         ``admin/login.html`` within a valid template directory and modify
         as needed.
         
         An example of a login template with local branding is provided at
         ``pucas/templates/pucas/sample-pu-login.html`` using re-usable template
         snippets that can be adapted or re-used as appropriate.
         
-        For Django 1.8, you will need to override ``admin/login.html`` as a whole, as
-        extending the login template with itself causes a recursion error.
+        Note that login templates have not yet been updated for Django 3.x.
         
         Usage
         -----
         
         Users can login with CAS and have a Django user account automatically
         created and populated with LDAP data based on the settings.
         
@@ -155,15 +160,15 @@
           to login first, as an aid to managing accounts and permissions.
           The optional flag ``--admin`` will give the new account superuser
           permissions
         
         Development instructions
         ------------------------
         
-        This git repository uses git flow branching conventions.
+        This git repository uses git flow branching conventions, with **main** as the current production release branch.
         
         Initial setup and installation:
         
         - recommended: create and activate a python 3.5 virtualenv::
         
             virtualenv pucas -p python3.5
             source pucas/bin/activate
@@ -172,21 +177,21 @@
         
             pip install -e .
         
         
         Unit Testing
         ^^^^^^^^^^^^^
         
-        Unit tests are written with [py.test](http://doc.pytest.org/) but use some
+        Unit tests are written with `py.test <http://doc.pytest.org/>`_ but use some
         Django test classes for compatibility with django test suites.  Running
         the tests requires a minimal settings file for Django required configurations.
         
         - Copy sample test settings and add a secret key::
         
-            cp ci/testsettings.py.sample testsettings.py
+            cp ci/testsettings.py testsettings.py
         
         - To run the tests, either use the configured setup.py test command::
         
             python setup.py test
         
         - Or install test requirements and use py.test directly::
         
@@ -204,28 +209,27 @@
         Princeton Docket #18-3398-1 for distribution online under a standard Open Source
         license.  Ownership rights transferred to Rebecca Koeser provided software
         is distributed online via open source.
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 1.9
-Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 Provides-Extra: test
```

### Comparing `pucas-0.6.0/pucas.egg-info/PKG-INFO` & `pucas-0.7.0/pucas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pucas
-Version: 0.6.0
+Version: 0.7.0
 Summary: Django app to login with CAS and populate user accounts with LDAP.
 Home-page: https://github.com/Princeton-CDH/django-pucas
 Author: CDH @ Princeton
 Author-email: digitalhumanities@princeton.edu
 License: Apache License, Version 2.0
 Description: django-pucas
         ============
@@ -21,28 +21,34 @@
            :target: https://www.codefactor.io/repository/github/princeton-cdh/django-pucas
            :alt: CodeFactor
         
         .. image:: https://requires.io/github/Princeton-CDH/django-pucas/requirements.svg?branch=master
              :target: https://requires.io/github/Princeton-CDH/django-pucas/requirements/?branch=master
              :alt: Requirements Status
         
+        .. image:: https://img.shields.io/pypi/pyversions/viapy
+           :alt: PyPI - Python Version
+        
+        .. image:: https://img.shields.io/pypi/djversions/viapy
+           :alt: PyPI - Django Version
+        
         **django-pucas** is a reusable `Django`_ application to simplify logging
         into a Django application with CAS using `django-cas-ng`_.  Login and
         creation of user accounts is handled by django-cas-ng; pucas adds
         support for prepopulating user account data based on an LDAP search.
         
         *pucas* should be pronounced like *pookas* for the Celtic spirit creature.
         
         .. _Django: https://www.djangoproject.com/
         .. _django-cas-ng: https://github.com/mingchen/django-cas-ng
         
-        **django-pucas** is tested under:
+        **django-pucas** is tested against:
         
-        * Django ``1.8-2.2``
-        * Python ``2.7, 3.5-3.7`` (excluding ``2.7`` for Django ``2+``)
+        * Django ``1.11-3.1``
+        * Python ``3.5-3.8``
         
         **django-pucas** requires **django-cas-ng** 3.6 or greater.
         
         Installation
         ------------
         
         Use pip to install::
@@ -133,16 +139,15 @@
         ``admin/login.html`` within a valid template directory and modify
         as needed.
         
         An example of a login template with local branding is provided at
         ``pucas/templates/pucas/sample-pu-login.html`` using re-usable template
         snippets that can be adapted or re-used as appropriate.
         
-        For Django 1.8, you will need to override ``admin/login.html`` as a whole, as
-        extending the login template with itself causes a recursion error.
+        Note that login templates have not yet been updated for Django 3.x.
         
         Usage
         -----
         
         Users can login with CAS and have a Django user account automatically
         created and populated with LDAP data based on the settings.
         
@@ -155,15 +160,15 @@
           to login first, as an aid to managing accounts and permissions.
           The optional flag ``--admin`` will give the new account superuser
           permissions
         
         Development instructions
         ------------------------
         
-        This git repository uses git flow branching conventions.
+        This git repository uses git flow branching conventions, with **main** as the current production release branch.
         
         Initial setup and installation:
         
         - recommended: create and activate a python 3.5 virtualenv::
         
             virtualenv pucas -p python3.5
             source pucas/bin/activate
@@ -172,21 +177,21 @@
         
             pip install -e .
         
         
         Unit Testing
         ^^^^^^^^^^^^^
         
-        Unit tests are written with [py.test](http://doc.pytest.org/) but use some
+        Unit tests are written with `py.test <http://doc.pytest.org/>`_ but use some
         Django test classes for compatibility with django test suites.  Running
         the tests requires a minimal settings file for Django required configurations.
         
         - Copy sample test settings and add a secret key::
         
-            cp ci/testsettings.py.sample testsettings.py
+            cp ci/testsettings.py testsettings.py
         
         - To run the tests, either use the configured setup.py test command::
         
             python setup.py test
         
         - Or install test requirements and use py.test directly::
         
@@ -204,28 +209,27 @@
         Princeton Docket #18-3398-1 for distribution online under a standard Open Source
         license.  Ownership rights transferred to Rebecca Koeser provided software
         is distributed online via open source.
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 1.9
-Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP
 Provides-Extra: test
```

### Comparing `pucas-0.6.0/pucas.egg-info/SOURCES.txt` & `pucas-0.7.0/pucas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pucas-0.6.0/LICENSE` & `pucas-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pucas-0.6.0/setup.py` & `pucas-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,29 +31,28 @@
         'test': TEST_REQUIREMENTS,
     },
     author='CDH @ Princeton',
     author_email='digitalhumanities@princeton.edu',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
-        'Framework :: Django :: 1.8',
-        'Framework :: Django :: 1.9',
-        'Framework :: Django :: 1.10',
         'Framework :: Django :: 1.11',
         'Framework :: Django :: 2.0',
         'Framework :: Django :: 2.1',
         'Framework :: Django :: 2.2',
+        'Framework :: Django :: 3.0',
+        'Framework :: Django :: 3.1',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: System :: Systems Administration :: Authentication/Directory',
         'Topic :: System :: Systems Administration :: Authentication/Directory :: LDAP',
     ],
 )
```

### Comparing `pucas-0.6.0/README.rst` & `pucas-0.7.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -13,28 +13,34 @@
    :target: https://www.codefactor.io/repository/github/princeton-cdh/django-pucas
    :alt: CodeFactor
 
 .. image:: https://requires.io/github/Princeton-CDH/django-pucas/requirements.svg?branch=master
      :target: https://requires.io/github/Princeton-CDH/django-pucas/requirements/?branch=master
      :alt: Requirements Status
 
+.. image:: https://img.shields.io/pypi/pyversions/viapy
+   :alt: PyPI - Python Version
+
+.. image:: https://img.shields.io/pypi/djversions/viapy
+   :alt: PyPI - Django Version
+
 **django-pucas** is a reusable `Django`_ application to simplify logging
 into a Django application with CAS using `django-cas-ng`_.  Login and
 creation of user accounts is handled by django-cas-ng; pucas adds
 support for prepopulating user account data based on an LDAP search.
 
 *pucas* should be pronounced like *pookas* for the Celtic spirit creature.
 
 .. _Django: https://www.djangoproject.com/
 .. _django-cas-ng: https://github.com/mingchen/django-cas-ng
 
-**django-pucas** is tested under:
+**django-pucas** is tested against:
 
-* Django ``1.8-2.2``
-* Python ``2.7, 3.5-3.7`` (excluding ``2.7`` for Django ``2+``)
+* Django ``1.11-3.1``
+* Python ``3.5-3.8``
 
 **django-pucas** requires **django-cas-ng** 3.6 or greater.
 
 Installation
 ------------
 
 Use pip to install::
@@ -125,16 +131,15 @@
 ``admin/login.html`` within a valid template directory and modify
 as needed.
 
 An example of a login template with local branding is provided at
 ``pucas/templates/pucas/sample-pu-login.html`` using re-usable template
 snippets that can be adapted or re-used as appropriate.
 
-For Django 1.8, you will need to override ``admin/login.html`` as a whole, as
-extending the login template with itself causes a recursion error.
+Note that login templates have not yet been updated for Django 3.x.
 
 Usage
 -----
 
 Users can login with CAS and have a Django user account automatically
 created and populated with LDAP data based on the settings.
 
@@ -147,15 +152,15 @@
   to login first, as an aid to managing accounts and permissions.
   The optional flag ``--admin`` will give the new account superuser
   permissions
 
 Development instructions
 ------------------------
 
-This git repository uses git flow branching conventions.
+This git repository uses git flow branching conventions, with **main** as the current production release branch.
 
 Initial setup and installation:
 
 - recommended: create and activate a python 3.5 virtualenv::
 
     virtualenv pucas -p python3.5
     source pucas/bin/activate
@@ -164,21 +169,21 @@
 
     pip install -e .
 
 
 Unit Testing
 ^^^^^^^^^^^^^
 
-Unit tests are written with [py.test](http://doc.pytest.org/) but use some
+Unit tests are written with `py.test <http://doc.pytest.org/>`_ but use some
 Django test classes for compatibility with django test suites.  Running
 the tests requires a minimal settings file for Django required configurations.
 
 - Copy sample test settings and add a secret key::
 
-    cp ci/testsettings.py.sample testsettings.py
+    cp ci/testsettings.py testsettings.py
 
 - To run the tests, either use the configured setup.py test command::
 
     python setup.py test
 
 - Or install test requirements and use py.test directly::
```

