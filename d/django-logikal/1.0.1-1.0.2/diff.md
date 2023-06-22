# Comparing `tmp/django-logikal-1.0.1.tar.gz` & `tmp/django-logikal-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-logikal-1.0.1.tar", last modified: Mon Jun 19 17:36:30 2023, max compression
+gzip compressed data, was "django-logikal-1.0.2.tar", last modified: Thu Jun 22 09:40:17 2023, max compression
```

## Comparing `django-logikal-1.0.1.tar` & `django-logikal-1.0.2.tar`

### file list

```diff
@@ -1,134 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.049968 django-logikal-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-19 17:36:00.000000 django-logikal-1.0.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-06-19 17:36:00.000000 django-logikal-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-19 17:36:00.000000 django-logikal-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2512 2023-06-19 17:36:30.049968 django-logikal-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-19 17:36:00.000000 django-logikal-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-06-19 17:36:00.000000 django-logikal-1.0.1/compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.021968 django-logikal-1.0.1/django_logikal/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/babel/
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/babel/django.ini
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/babel/djangojs.ini
--rw-r--r--   0 runner    (1001) docker     (122)     6663 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/bibliography.py
--rw-r--r--   0 runner    (1001) docker     (122)     6453 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/email.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/env.py
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/local_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4602 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)      485 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/commands/syncdb.py
--rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/management/commands/translate.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/migrations.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/security.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4421 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3031 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/dynamic_site.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)      437 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/static_site.py
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/settings/testing.py
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.017968 django-logikal-1.0.1/django_logikal/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal/static/django_logikal/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   600856 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   309728 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (122)   184912 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   622572 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   323344 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (122)   193308 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   639388 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   328412 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (122)   195704 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)   617492 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   310884 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff
--rw-r--r--   0 runner    (1001) docker     (122)   181500 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   628640 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   325296 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff
--rw-r--r--   0 runner    (1001) docker     (122)   192916 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-README.txt
--rw-r--r--   0 runner    (1001) docker     (122)   607720 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   309192 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (122)   182708 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   614256 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   312952 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff
--rw-r--r--   0 runner    (1001) docker     (122)   184076 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   630852 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   327188 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (122)   195128 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   610876 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   306060 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff
--rw-r--r--   0 runner    (1001) docker     (122)   180576 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2
--rw-r--r--   0 runner    (1001) docker     (122)   628352 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)   323532 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff
--rw-r--r--   0 runner    (1001) docker     (122)   191804 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    87008 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    53528 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (122)    40688 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    94148 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    59380 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (122)    44824 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    93904 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    58800 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (122)    44544 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    11560 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)    86908 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (122)    53252 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (122)    40672 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (122)     3714 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/fonts.css
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static/django_logikal/validation_error.css
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/static.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/debug_toolbar/
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/debug_toolbar/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/django_logikal/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/django_logikal/base.html.j
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/django_logikal/templates/django_logikal/email/
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/django_logikal/email/base.html.j
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/django_logikal/validation_error.html.j
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     5460 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/jinja.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/processors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2718 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/template.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/templates/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2223 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-06-19 17:36:00.000000 django-logikal-1.0.1/django_logikal/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.025968 django-logikal-1.0.1/django_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2512 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-06-19 17:36:30.000000 django-logikal-1.0.1/django_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      473 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-19 17:36:29.000000 django-logikal-1.0.1/django_logikal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-06-19 17:36:00.000000 django-logikal-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.045968 django-logikal-1.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4425 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 17:36:30.049968 django-logikal-1.0.1/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/extras/bibliography.txt
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/extras/dynamic.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-19 17:36:00.000000 django-logikal-1.0.1/requirements/extras/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 17:36:30.049968 django-logikal-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:17.007406 django-logikal-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-22 09:39:47.000000 django-logikal-1.0.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-06-22 09:39:47.000000 django-logikal-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-22 09:39:47.000000 django-logikal-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2512 2023-06-22 09:40:17.007406 django-logikal-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-22 09:39:47.000000 django-logikal-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-06-22 09:39:47.000000 django-logikal-1.0.2/compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:16.975406 django-logikal-1.0.2/django_logikal/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:16.979406 django-logikal-1.0.2/django_logikal/babel/
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/babel/django.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/babel/djangojs.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     6663 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/bibliography.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6453 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/email.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/local_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4602 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:16.979406 django-logikal-1.0.2/django_logikal/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:16.979406 django-logikal-1.0.2/django_logikal/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/management/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/management/commands/syncdb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7639 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/management/commands/translate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/security.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:16.983406 django-logikal-1.0.2/django_logikal/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4420 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3031 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/settings/dynamic_site.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/settings/static_site.py
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/settings/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:16.971406 django-logikal-1.0.2/django_logikal/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:16.983406 django-logikal-1.0.2/django_logikal/static/django_logikal/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:17.003406 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   600856 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   309728 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   184912 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   622572 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   323344 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   193308 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   639388 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   328412 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   195704 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   617492 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   310884 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   181500 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   628640 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   325296 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   192916 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-README.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   607720 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   309192 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   182708 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   614256 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   312952 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   184076 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   630852 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   327188 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   195128 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   610876 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   306060 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Thin.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   180576 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   628352 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)   323532 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)   191804 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    87008 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    53528 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    40688 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    94148 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    59380 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    44824 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    93904 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    58800 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    44544 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)    11560 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    86908 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)    53252 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    40672 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)     3714 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static/django_logikal/validation_error.css
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/static.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:17.007406 django-logikal-1.0.2/django_logikal/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:17.007406 django-logikal-1.0.2/django_logikal/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:17.007406 django-logikal-1.0.2/django_logikal/templates/debug_toolbar/
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/debug_toolbar/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:17.007406 django-logikal-1.0.2/django_logikal/templates/django_logikal/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/django_logikal/base.html.j
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:17.007406 django-logikal-1.0.2/django_logikal/templates/django_logikal/email/
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/django_logikal/email/base.html.j
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/django_logikal/validation_error.html.j
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5460 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2718 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/template.py
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/templates/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-06-22 09:39:47.000000 django-logikal-1.0.2/django_logikal/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:16.979406 django-logikal-1.0.2/django_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2512 2023-06-22 09:40:16.000000 django-logikal-1.0.2/django_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5087 2023-06-22 09:40:16.000000 django-logikal-1.0.2/django_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 09:40:16.000000 django-logikal-1.0.2/django_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-22 09:40:16.000000 django-logikal-1.0.2/django_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-22 09:40:16.000000 django-logikal-1.0.2/django_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-22 09:40:16.000000 django-logikal-1.0.2/django_logikal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-06-22 09:39:47.000000 django-logikal-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:17.007406 django-logikal-1.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4442 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:40:17.007406 django-logikal-1.0.2/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/extras/bibliography.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/extras/dynamic.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-22 09:39:47.000000 django-logikal-1.0.2/requirements/extras/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 09:40:17.007406 django-logikal-1.0.2/setup.cfg
```

### Comparing `django-logikal-1.0.1/.copier-answers.yml` & `django-logikal-1.0.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/LICENSE.txt` & `django-logikal-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/PKG-INFO` & `django-logikal-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logikal
-Version: 1.0.1
+Version: 1.0.2
 Summary: Django utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `django-logikal-1.0.1/compose.yml` & `django-logikal-1.0.2/compose.yml`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/apps.py` & `django-logikal-1.0.2/django_logikal/apps.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/bibliography.py` & `django-logikal-1.0.2/django_logikal/bibliography.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/email.py` & `django-logikal-1.0.2/django_logikal/email.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/logging.py` & `django-logikal-1.0.2/django_logikal/logging.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/management/commands/generate.py` & `django-logikal-1.0.2/django_logikal/management/commands/generate.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/management/commands/syncdb.py` & `django-logikal-1.0.2/django_logikal/management/commands/syncdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Synchronize the local database.
 
 Clear the public schema, apply migrations and insert local application data.
 
+.. note:: Requires :ref:`pytest-logikal[django] <pytest-logikal:index:django>` to be installed.
 .. note:: Local data must be specified in the ``local_data.py`` submodule of a given application in
     classes inheriting from :class:`~django_logikal.local_data.LocalData`.
 
 .. autoclass:: django_logikal.local_data.LocalData
     :undoc-members:
 
 .. tip:: We recommend using :doc:`factory_boy <factory-boy:index>`'s
@@ -21,15 +22,14 @@
 from typing import Any
 
 from django.apps import apps
 from django.core.management import call_command
 from django.core.management.base import BaseCommand, CommandError, CommandParser
 from django.db import connections
 from factory import random as factory_random
-from pytest_logikal.django import DEFAULT_RANDOM_SEED
 
 from django_logikal.local_data import LocalData
 
 
 class Command(BaseCommand):
     help = ' '.join(__doc__.splitlines()[0:4])
 
@@ -62,15 +62,17 @@
             self.stdout.write(self.style.SUCCESS(' OK'))
 
         # Run migrations
         self.stdout.write('')
         call_command('migrate', **options)
 
         # Insert local data
-        factory_random.reseed_random(DEFAULT_RANDOM_SEED)  # for deterministic data
+        from pytest_logikal import django  # pylint: disable=import-outside-toplevel
+
+        factory_random.reseed_random(django.DEFAULT_RANDOM_SEED)  # for deterministic data
         for app in apps.get_app_configs():
             with suppress(ImportError):
                 if (module := getattr(app, 'module', None)):
                     import_module(f'{module.__name__}.local_data')  # register LocalData subclasses
         if LocalData.__subclasses__():
             self.stdout.write(self.style.MIGRATE_HEADING('\nInserting local data:'))
         for local_data in LocalData.__subclasses__():
```

### Comparing `django-logikal-1.0.1/django_logikal/management/commands/translate.py` & `django-logikal-1.0.2/django_logikal/management/commands/translate.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from importlib import metadata
 from pathlib import Path
 from typing import Any, Optional, Sequence, cast
 
 import django
 from babel.messages.frontend import CommandLineInterface
 from django.core.management.base import BaseCommand, CommandError, CommandParser
-
-from django_logikal.pyproject import DJANGO_LOGIKAL_CONFIG, PYPROJECT
+from logikal_utils.project import PYPROJECT, tool_config
 
 TEMPLATE_HEADER = """
 # Translation template for project "PROJECT"
 # Copyright 2023 ORGANIZATION
 """
 DEFAULT_WIDTH = 76
 DOMAINS = ('django', 'djangojs')
@@ -49,15 +48,15 @@
             if record.msg.lower() == 'extracting messages from %s%s':
                 record.args = (record.args[0], '')  # type: ignore[index]
             return True
 
         logging.getLogger().handlers = []  # to avoid double logging
         logging.getLogger('babel').addFilter(remove_config_info)
 
-        default_apps = DJANGO_LOGIKAL_CONFIG.get('translate', {}).get('apps', [])
+        default_apps = tool_config('django_logikal').get('translate', {}).get('apps', [])
         if not (apps := [App(app) for app in options.get('app') or default_apps]):
             raise CommandError('At least one app name must be provided')
 
         output = cast(Optional[Path], options.get('output'))  # wrong typing
 
         if options.get('init'):
             if not (locale := cast(Optional[str], options.get('locale'))):
@@ -80,15 +79,15 @@
                 # Configuration
                 '--mapping-file', Path(__file__).parents[2] / f'babel/{domain}.ini',
                 '--width', DEFAULT_WIDTH,
                 '--add-comments', 'Translators:',
                 # Metadata
                 '--project', app.name.replace('_', '-'),
                 '--version', f'v{metadata.version(PYPROJECT["project"]["name"])}',
-                '--msgid-bugs-address', DJANGO_LOGIKAL_CONFIG['translate']['contact'],
+                '--msgid-bugs-address', tool_config('django_logikal')['translate']['contact'],
                 '--copyright-holder', PYPROJECT['project']['authors'][0]['name'],
                 '--header-comment', TEMPLATE_HEADER,
                 # Input and output file
                 '--output-file', str(locale_path / f'{domain}.pot'),
                 str(app.path),
             ])
         self.stdout.write()
```

### Comparing `django-logikal-1.0.1/django_logikal/run.py` & `django-logikal-1.0.2/django_logikal/run.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 import argparse
 import sys
 from os import environ
 from typing import Sequence
 
 from django.core.management import execute_from_command_line
+from logikal_utils.project import tool_config
 
 from django_logikal.env import set_option
-from django_logikal.pyproject import DJANGO_LOGIKAL_CONFIG
 
 
 def main(args: Sequence[str] = tuple(sys.argv[1:])) -> int:
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument('-d', '--debug', action='store_true', help='use debug logging level')
     parser.add_argument('-t', '--toolbar', action='store_true', help='enable the debug toolbar')
     parser.add_argument('--cloud-logging', action='store_true', help='use cloud logging')
@@ -26,10 +26,13 @@
     if util_args.cloud_logging:
         set_option('cloud_logging')
     if util_args.send_emails:
         set_option('send_emails')
 
     sys.path.insert(0, '.')
     set_option('local_run')
-    environ.setdefault('DJANGO_SETTINGS_MODULE', DJANGO_LOGIKAL_CONFIG['DJANGO_SETTINGS_MODULE'])
+    environ.setdefault(
+        'DJANGO_SETTINGS_MODULE',
+        tool_config('django_logikal')['DJANGO_SETTINGS_MODULE'],
+    )
     execute_from_command_line(['manage', 'runserver'] + manage_args)
     return 0
```

### Comparing `django-logikal-1.0.1/django_logikal/security.py` & `django-logikal-1.0.2/django_logikal/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     .. warning:: When this middleware is used, you must mark all public views explicitly, including
         views included from applications like :mod:`django.contrib.admin`. You may use the
         :ref:`URL utility functions <urls:URLs & Paths>` which provide such explicitly marked
         public views where necessary.
 
     .. note:: All :ref:`standard settings modules <settings:Settings>` include this middleware by
         default.
-
     """
     @staticmethod
     def process_view(
         request: HttpRequest,
         view_func: Callable[..., Any],
         view_args: List[Any],
         view_kwargs: Dict[str, Any],
```

### Comparing `django-logikal-1.0.1/django_logikal/settings/base.py` & `django-logikal-1.0.2/django_logikal/settings/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from importlib.util import find_spec
 from pathlib import Path
 
 from django.utils.translation import gettext_lazy
-from pytest_logikal.docker import Service
+from logikal_utils.docker import Service
 
 from django_logikal.env import get_option, option_is_set
 from django_logikal.logging import logging_config
 
 # Logging
 logging.captureWarnings(capture=True)
 logging.getLogger('blib2to3').setLevel(logging.WARNING)  # used during Black migration formatting
```

### Comparing `django-logikal-1.0.1/django_logikal/settings/dynamic_site.py` & `django-logikal-1.0.2/django_logikal/settings/dynamic_site.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/settings/production.py` & `django-logikal-1.0.2/django_logikal/settings/production.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/sitemap.py` & `django-logikal-1.0.2/django_logikal/sitemap.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Light.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Light.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-README.txt` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-README.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Thin.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/fonts.css` & `django-logikal-1.0.2/django_logikal/static/django_logikal/fonts.css`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static/django_logikal/validation_error.css` & `django-logikal-1.0.2/django_logikal/static/django_logikal/validation_error.css`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/static.py` & `django-logikal-1.0.2/django_logikal/static.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/templates/django_logikal/base.html.j` & `django-logikal-1.0.2/django_logikal/templates/django_logikal/base.html.j`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/templates/django_logikal/validation_error.html.j` & `django-logikal-1.0.2/django_logikal/templates/django_logikal/validation_error.html.j`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/templates/extensions.py` & `django-logikal-1.0.2/django_logikal/templates/extensions.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/templates/filters.py` & `django-logikal-1.0.2/django_logikal/templates/filters.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/templates/functions.py` & `django-logikal-1.0.2/django_logikal/templates/functions.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/templates/jinja.py` & `django-logikal-1.0.2/django_logikal/templates/jinja.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/templates/template.py` & `django-logikal-1.0.2/django_logikal/templates/template.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/urls.py` & `django-logikal-1.0.2/django_logikal/urls.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal/validation.py` & `django-logikal-1.0.2/django_logikal/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 
 from django.http import HttpRequest, HttpResponse
 from django.shortcuts import render
 from django.utils.safestring import mark_safe
 from pygments import highlight
 from pygments.formatters.html import HtmlFormatter
 from pygments.lexers.html import HtmlLexer
-from pytest_logikal.validator import Validator
 
 from django_logikal.middleware import Middleware
 
 logger = getLogger(__name__)
 
 
 class ValidationMiddleware(Middleware):
+    """
+    Validate HTML responses for all requests.
+
+    .. note:: Requires :ref:`pytest-logikal <pytest-logikal:index:Installation>` to be installed.
+    """
     def __init__(self, *args: Any, **kwargs: Any):
+        from pytest_logikal.validator import Validator  # pylint: disable=import-outside-toplevel
+
         super().__init__(*args, **kwargs)
         self._validator = Validator()
 
     def __call__(self, request: HttpRequest) -> HttpResponse:
         response = super().__call__(request)
         resolver_match = getattr(request, 'resolver_match', None)
         app_name = getattr(resolver_match, 'app_name', None)
```

### Comparing `django-logikal-1.0.1/django_logikal/views.py` & `django-logikal-1.0.2/django_logikal/views.py`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/django_logikal.egg-info/PKG-INFO` & `django-logikal-1.0.2/django_logikal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logikal
-Version: 1.0.1
+Version: 1.0.2
 Summary: Django utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `django-logikal-1.0.1/django_logikal.egg-info/SOURCES.txt` & `django-logikal-1.0.2/django_logikal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 django_logikal/local_data.py
 django_logikal/logging.py
 django_logikal/manage.py
 django_logikal/middleware.py
 django_logikal/migrations.py
 django_logikal/models.py
 django_logikal/py.typed
-django_logikal/pyproject.py
 django_logikal/run.py
 django_logikal/security.py
 django_logikal/sitemap.py
 django_logikal/static.py
 django_logikal/urls.py
 django_logikal/validation.py
 django_logikal/views.py
```

### Comparing `django-logikal-1.0.1/pyproject.toml` & `django-logikal-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/requirements/build.txt.lock` & `django-logikal-1.0.2/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `django-logikal-1.0.1/requirements/dev.txt.lock` & `django-logikal-1.0.2/requirements/docs.txt.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 12183ed76906dc100f496e030bc93661a4a90bae1e8a02bac0644b2455769ff4
+##  Requirements hash: 802065ad4e7538fc226b41b489bab6d50e0ffe586e4a11a34fed55f44cc63e5b
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 antimarkdown==1.0.2
 appdirs==1.4.4
 asgiref==3.7.2
 astroid==2.15.5
-async-generator==1.10
 attrs==23.1.0
 Babel==2.12.1
 backports.zoneinfo==0.2.1
 bandit==1.7.5
 black==23.3.0
-bleach==6.0.0
 boto3==1.26.130
 boto3-stubs==1.26.130
-botocore==1.29.155
-botocore-stubs==1.29.155
+botocore==1.29.158
+botocore-stubs==1.29.158
 Bottleneck==1.3.7
-build==0.10.0
 cachetools==5.3.1
 certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
 coverage==7.2.7
@@ -51,18 +48,16 @@
 djlint==1.30.0
 docker==6.1.3
 docutils==0.17.1
 EditorConfig==0.12.3
 exceptiongroup==1.1.1
 execnet==1.9.0
 factory-boy==3.2.1
-Faker==18.10.1
+Faker==18.11.1
 filelock==3.12.2
-flaky==3.7.0
-freezegun==1.2.2
 gitdb==4.0.10
 GitPython==3.1.31
 google-api-core==2.11.1
 google-api-python-client==2.86.0
 google-api-python-client-stubs==1.16.0
 google-auth==2.17.3
 google-auth-httplib2==0.1.0
@@ -76,108 +71,91 @@
 google-crc32c==1.5.0
 google-resumable-media==2.5.0
 googleapis-common-protos==1.59.1
 grpc-google-iam-v1==0.12.6
 grpc-stubs==1.53.0.2
 grpcio==1.54.2
 grpcio-status==1.54.2
-h11==0.14.0
 html-tag-names==0.1.2
 html-void-elements==0.1.0
 httplib2==0.22.0
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.6.0
-importlib-resources==5.12.0
+importlib-metadata==6.7.0
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.12.0
-jaraco.classes==3.2.3
-jeepney==0.8.0
 Jinja2==3.1.2
 jmespath==1.0.1
 jsbeautifier==1.14.8
 json5==0.9.14
-keyring==23.13.1
 latexcodec==2.0.1
 lazy-object-proxy==1.9.0
-llvmlite==0.40.1rc1
+llvmlite==0.40.1
 logikal-docs==1.1.3
+logikal-utils==1.0.0
 lxml==4.9.2
 markdown-it-py==3.0.0
 MarkupSafe==2.1.3
 mccabe==0.7.0
 mdurl==0.1.2
-more-itertools==9.1.0
 mypy==1.3.0
 mypy-extensions==1.0.0
-numba==0.57.0
+numba==0.57.1
 numexpr==2.8.4
 numpy==1.24.3
-outcome==1.2.0
 packaging==23.1
 pandas==2.0.2
 pandas-stubs==2.0.2.230605
 pathspec==0.11.1
 pbr==5.11.1
 Pillow==9.5.0
 pip==23.1.2
 pip-licenses==4.3.2
-pkginfo==1.9.6
-platformdirs==3.5.3
-pluggy==1.0.0
+platformdirs==3.7.0
+pluggy==1.2.0
 premailer==3.10.0
 prettytable==3.8.0
 proto-plus==1.22.2
 protobuf==4.23.3
-psutil==5.9.4
+psutil==5.9.5
 psycopg==3.1.9
 pyarrow==12.0.1
 pyasn1==0.5.0
 pyasn1-modules==0.3.0
 pybtex==0.24.0
 pycodestyle==2.10.0
 pycparser==2.21
 pydocstyle==6.3.0
 Pygments==2.15.1
 pylint==2.17.4
 pylint-django==2.5.3
 pylint-plugin-utils==0.8.2
 pyorbs==2.0.0
-pyparsing==3.0.9
-pyproject_hooks==1.0.0
-PySocks==1.7.1
+pyparsing==3.1.0
 pytest==7.3.1
 pytest-cov==4.1.0
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
-pytest-logikal==1.10.3
+pytest-logikal==1.10.4
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
 pytest-xdist==3.3.1
-pytest_freezer==0.4.6
 python-dateutil==2.8.2
 pytz==2023.3
 PyYAML==6.0
-readme-renderer==37.3
 regex==2023.6.3
 requests==2.31.0
-requests-toolbelt==1.0.0
-rfc3986==2.0.0
 rich==13.4.2
 rsa==4.9
 s3transfer==0.6.1
-SecretStorage==3.3.3
-selenium==4.9.1
-setuptools==67.8.0
+setuptools==68.0.0
 six==1.16.0
 smmap==5.0.0
-sniffio==1.3.0
 snowballstemmer==2.2.0
-sortedcontainers==2.4.0
 Sphinx==5.3.0
 sphinx-rtd-theme==1.1.1
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
@@ -186,32 +164,26 @@
 stevedore==5.1.0
 stormware==1.2.0
 termcolor==2.3.0
 toml==0.10.2
 tomli==2.0.1
 tomlkit==0.11.8
 tqdm==4.65.0
-trio==0.22.0
-trio-websocket==0.10.3
-twine==4.0.2
 types-awscrt==0.16.19
 types-docutils==0.20.0.1
-types-psutil==5.9.5.11
 types-Pygments==2.15.0.1
 types-pytz==2023.3.0.0
 types-PyYAML==6.0.12.10
 types-requests==2.31.0.1
 types-s3transfer==0.6.1
-types-setuptools==67.8.0.0
+types-setuptools==68.0.0.0
 types-urllib3==1.26.25.13
 typing_extensions==4.6.3
 tzdata==2023.3
 uritemplate==4.1.1
 urllib3==1.26.16
 wcwidth==0.2.6
-webencodings==0.5.1
 websocket-client==1.6.0
 wheel==0.40.0
 wrapt==1.15.0
-wsproto==1.2.0
 xdg==5.1.1
 zipp==3.15.0
```

### Comparing `django-logikal-1.0.1/requirements/docs.txt.lock` & `django-logikal-1.0.2/requirements/dev.txt.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 5e3871fb856b5c74e021a2218bf50701e2c7d667f43f5fc9d8cfae8775b1f394
+##  Requirements hash: d78b24ec7a15574bd053eab152888943438415a08afc84d240a3f581fb62a040
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 antimarkdown==1.0.2
 appdirs==1.4.4
 asgiref==3.7.2
 astroid==2.15.5
+async-generator==1.10
 attrs==23.1.0
 Babel==2.12.1
 backports.zoneinfo==0.2.1
 bandit==1.7.5
 black==23.3.0
+bleach==6.0.0
 boto3==1.26.130
 boto3-stubs==1.26.130
-botocore==1.29.155
-botocore-stubs==1.29.155
+botocore==1.29.158
+botocore-stubs==1.29.158
 Bottleneck==1.3.7
+build==0.10.0
 cachetools==5.3.1
 certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
 coverage==7.2.7
@@ -48,16 +51,18 @@
 djlint==1.30.0
 docker==6.1.3
 docutils==0.17.1
 EditorConfig==0.12.3
 exceptiongroup==1.1.1
 execnet==1.9.0
 factory-boy==3.2.1
-Faker==18.10.1
+Faker==18.11.1
 filelock==3.12.2
+flaky==3.7.0
+freezegun==1.2.2
 gitdb==4.0.10
 GitPython==3.1.31
 google-api-core==2.11.1
 google-api-python-client==2.86.0
 google-api-python-client-stubs==1.16.0
 google-auth==2.17.3
 google-auth-httplib2==0.1.0
@@ -71,51 +76,60 @@
 google-crc32c==1.5.0
 google-resumable-media==2.5.0
 googleapis-common-protos==1.59.1
 grpc-google-iam-v1==0.12.6
 grpc-stubs==1.53.0.2
 grpcio==1.54.2
 grpcio-status==1.54.2
+h11==0.14.0
 html-tag-names==0.1.2
 html-void-elements==0.1.0
 httplib2==0.22.0
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.6.0
+importlib-metadata==6.7.0
+importlib-resources==5.12.0
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.12.0
+jaraco.classes==3.2.3
+jeepney==0.8.0
 Jinja2==3.1.2
 jmespath==1.0.1
 jsbeautifier==1.14.8
 json5==0.9.14
+keyring==24.0.1
 latexcodec==2.0.1
 lazy-object-proxy==1.9.0
-llvmlite==0.40.1rc1
+llvmlite==0.40.1
 logikal-docs==1.1.3
+logikal-utils==1.0.0
 lxml==4.9.2
 markdown-it-py==3.0.0
 MarkupSafe==2.1.3
 mccabe==0.7.0
 mdurl==0.1.2
+more-itertools==9.1.0
 mypy==1.3.0
 mypy-extensions==1.0.0
-numba==0.57.0
+numba==0.57.1
 numexpr==2.8.4
 numpy==1.24.3
+outcome==1.2.0
 packaging==23.1
 pandas==2.0.2
 pandas-stubs==2.0.2.230605
 pathspec==0.11.1
 pbr==5.11.1
 Pillow==9.5.0
 pip==23.1.2
 pip-licenses==4.3.2
-platformdirs==3.5.3
-pluggy==1.0.0
+pkginfo==1.9.6
+platformdirs==3.7.0
+pluggy==1.2.0
 premailer==3.10.0
 prettytable==3.8.0
 proto-plus==1.22.2
 protobuf==4.23.3
 psutil==5.9.5
 psycopg==3.1.9
 pyarrow==12.0.1
@@ -126,35 +140,45 @@
 pycparser==2.21
 pydocstyle==6.3.0
 Pygments==2.15.1
 pylint==2.17.4
 pylint-django==2.5.3
 pylint-plugin-utils==0.8.2
 pyorbs==2.0.0
-pyparsing==3.0.9
+pyparsing==3.1.0
+pyproject_hooks==1.0.0
+PySocks==1.7.1
 pytest==7.3.1
 pytest-cov==4.1.0
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
-pytest-logikal==1.10.3
+pytest-logikal==1.10.4
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
 pytest-xdist==3.3.1
+pytest_freezer==0.4.6
 python-dateutil==2.8.2
 pytz==2023.3
 PyYAML==6.0
+readme-renderer==40.0
 regex==2023.6.3
 requests==2.31.0
+requests-toolbelt==1.0.0
+rfc3986==2.0.0
 rich==13.4.2
 rsa==4.9
 s3transfer==0.6.1
-setuptools==67.8.0
+SecretStorage==3.3.3
+selenium==4.9.1
+setuptools==68.0.0
 six==1.16.0
 smmap==5.0.0
+sniffio==1.3.0
 snowballstemmer==2.2.0
+sortedcontainers==2.4.0
 Sphinx==5.3.0
 sphinx-rtd-theme==1.1.1
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
@@ -163,26 +187,32 @@
 stevedore==5.1.0
 stormware==1.2.0
 termcolor==2.3.0
 toml==0.10.2
 tomli==2.0.1
 tomlkit==0.11.8
 tqdm==4.65.0
+trio==0.22.0
+trio-websocket==0.10.3
+twine==4.0.2
 types-awscrt==0.16.19
 types-docutils==0.20.0.1
+types-psutil==5.9.5.15
 types-Pygments==2.15.0.1
 types-pytz==2023.3.0.0
 types-PyYAML==6.0.12.10
 types-requests==2.31.0.1
 types-s3transfer==0.6.1
-types-setuptools==67.8.0.0
+types-setuptools==68.0.0.0
 types-urllib3==1.26.25.13
 typing_extensions==4.6.3
 tzdata==2023.3
 uritemplate==4.1.1
 urllib3==1.26.16
 wcwidth==0.2.6
+webencodings==0.5.1
 websocket-client==1.6.0
 wheel==0.40.0
 wrapt==1.15.0
+wsproto==1.2.0
 xdg==5.1.1
 zipp==3.15.0
```

