# Comparing `tmp/django-axes-6.0.3.tar.gz` & `tmp/django-axes-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-axes-6.0.3.tar", last modified: Sun Jun 18 11:18:46 2023, max compression
+gzip compressed data, was "django-axes-6.0.4.tar", last modified: Thu Jun 22 08:47:47 2023, max compression
```

## Comparing `django-axes-6.0.3.tar` & `django-axes-6.0.4.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.461895 django-axes-6.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.449895 django-axes-6.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.449895 django-axes-6.0.3/.github/ISSUE_TEMPLATES/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-18 11:18:33.000000 django-axes-6.0.3/.github/ISSUE_TEMPLATES/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-18 11:18:33.000000 django-axes-6.0.3/.github/ISSUE_TEMPLATES/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-18 11:18:33.000000 django-axes-6.0.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 11:18:33.000000 django-axes-6.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.449895 django-axes-6.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-18 11:18:33.000000 django-axes-6.0.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-18 11:18:33.000000 django-axes-6.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-18 11:18:33.000000 django-axes-6.0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-18 11:18:33.000000 django-axes-6.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 11:18:33.000000 django-axes-6.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-18 11:18:33.000000 django-axes-6.0.3/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    32534 2023-06-18 11:18:33.000000 django-axes-6.0.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-18 11:18:33.000000 django-axes-6.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-18 11:18:33.000000 django-axes-6.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-18 11:18:33.000000 django-axes-6.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-06-18 11:18:46.461895 django-axes-6.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-18 11:18:33.000000 django-axes-6.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.453895 django-axes-6.0.3/axes/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.453895 django-axes-6.0.3/axes/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/handlers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/handlers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/handlers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/handlers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.449895 django-axes-6.0.3/axes/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.445895 django-axes-6.0.3/axes/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.453895 django-axes-6.0.3/axes/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.445895 django-axes-6.0.3/axes/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.453895 django-axes-6.0.3/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.449895 django-axes-6.0.3/axes/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.453895 django-axes-6.0.3/axes/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.449895 django-axes-6.0.3/axes/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.453895 django-axes-6.0.3/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.449895 django-axes-6.0.3/axes/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.453895 django-axes-6.0.3/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.453895 django-axes-6.0.3/axes/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.457895 django-axes-6.0.3/axes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/management/commands/axes_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/management/commands/axes_reset_failure_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.457895 django-axes-6.0.3/axes/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/migrations/0007_alter_accessattempt_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/migrations/0008_accessfailurelog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-18 11:18:33.000000 django-axes-6.0.3/axes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-18 11:18:33.000000 django-axes-6.0.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.457895 django-axes-6.0.3/django_axes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-06-18 11:18:46.000000 django-axes-6.0.3/django_axes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-18 11:18:46.000000 django-axes-6.0.3/django_axes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:18:46.000000 django-axes-6.0.3/django_axes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:18:46.000000 django-axes-6.0.3/django_axes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 11:18:46.000000 django-axes-6.0.3/django_axes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 11:18:46.000000 django-axes-6.0.3/django_axes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.457895 django-axes-6.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/10_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/1_requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/2_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/3_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/4_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/5_customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/6_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/7_architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/8_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/9_contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.457895 django-axes-6.0.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/images/flow.png
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-18 11:18:33.000000 django-axes-6.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-18 11:18:33.000000 django-axes-6.0.3/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 11:18:33.000000 django-axes-6.0.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-18 11:18:33.000000 django-axes-6.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-18 11:18:33.000000 django-axes-6.0.3/requirements-qa.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-18 11:18:33.000000 django-axes-6.0.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-18 11:18:33.000000 django-axes-6.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 11:18:46.461895 django-axes-6.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-18 11:18:33.000000 django-axes-6.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:46.461895 django-axes-6.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 11:18:33.000000 django-axes-6.0.3/tests/urls_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.769328 django-axes-6.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.753328 django-axes-6.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.753328 django-axes-6.0.4/.github/ISSUE_TEMPLATES/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/ISSUE_TEMPLATES/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/ISSUE_TEMPLATES/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.753328 django-axes-6.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-22 08:47:27.000000 django-axes-6.0.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-22 08:47:27.000000 django-axes-6.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 08:47:27.000000 django-axes-6.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 08:47:27.000000 django-axes-6.0.4/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-06-22 08:47:27.000000 django-axes-6.0.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-22 08:47:27.000000 django-axes-6.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-22 08:47:27.000000 django-axes-6.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-22 08:47:27.000000 django-axes-6.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36853 2023-06-22 08:47:47.769328 django-axes-6.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-22 08:47:27.000000 django-axes-6.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.757328 django-axes-6.0.4/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.757328 django-axes-6.0.4/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.757328 django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.757328 django-axes-6.0.4/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.749328 django-axes-6.0.4/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset_failure_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.761329 django-axes-6.0.4/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/0008_accessfailurelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-22 08:47:27.000000 django-axes-6.0.4/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-22 08:47:27.000000 django-axes-6.0.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.765329 django-axes-6.0.4/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36853 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 08:47:47.000000 django-axes-6.0.4/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.765329 django-axes-6.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/9_contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.765329 django-axes-6.0.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-22 08:47:27.000000 django-axes-6.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-22 08:47:27.000000 django-axes-6.0.4/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-22 08:47:27.000000 django-axes-6.0.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-22 08:47:27.000000 django-axes-6.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 08:47:27.000000 django-axes-6.0.4/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-22 08:47:27.000000 django-axes-6.0.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 08:47:27.000000 django-axes-6.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 08:47:47.769328 django-axes-6.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-22 08:47:27.000000 django-axes-6.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:47.769328 django-axes-6.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38226 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 08:47:27.000000 django-axes-6.0.4/tests/urls_empty.py
```

### Comparing `django-axes-6.0.3/.github/ISSUE_TEMPLATES/bug_report.md` & `django-axes-6.0.4/.github/ISSUE_TEMPLATES/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/.github/ISSUE_TEMPLATES/feature_request.md` & `django-axes-6.0.4/.github/ISSUE_TEMPLATES/feature_request.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/.github/PULL_REQUEST_TEMPLATE.md` & `django-axes-6.0.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/.github/workflows/codeql.yml` & `django-axes-6.0.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/.github/workflows/release.yml` & `django-axes-6.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/.github/workflows/test.yml` & `django-axes-6.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/CHANGES.rst` & `django-axes-6.0.4/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 
 Changes
 =======
 
 
+6.0.4 (2023-06-22)
+------------------
+
+- Remove unused methods from AxesStandaloneBackend.
+  [314eter]
+
+
 6.0.3 (2023-06-18)
 ------------------
 
 - Add username to admin fieldsets.
   [sevdog]
```

### Comparing `django-axes-6.0.3/CODE_OF_CONDUCT.md` & `django-axes-6.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/CONTRIBUTING.rst` & `django-axes-6.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/LICENSE` & `django-axes-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/PKG-INFO` & `django-axes-6.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.3
+Version: 6.0.4
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -123,14 +123,21 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.4 (2023-06-22)
+------------------
+
+- Remove unused methods from AxesStandaloneBackend.
+  [314eter]
+
+
 6.0.3 (2023-06-18)
 ------------------
 
 - Add username to admin fieldsets.
   [sevdog]
```

### Comparing `django-axes-6.0.3/README.rst` & `django-axes-6.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/admin.py` & `django-axes-6.0.4/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/apps.py` & `django-axes-6.0.4/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/attempts.py` & `django-axes-6.0.4/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/backends.py` & `django-axes-6.0.4/axes/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Optional
 from django.conf import settings
-from django.contrib.auth.backends import BaseBackend, ModelBackend
+from django.contrib.auth.backends import ModelBackend
 from django.http import HttpRequest
 
 from axes.exceptions import (
     AxesBackendPermissionDenied,
     AxesBackendRequestParameterRequired,
 )
 from axes.handlers.proxy import AxesProxyHandler
 from axes.helpers import get_credentials, get_lockout_message, toggleable
 
 
-class AxesStandaloneBackend(BaseBackend):
+class AxesStandaloneBackend:
     """
     Authentication backend class that forbids login attempts for locked out users.
 
     Use this class as the first item of ``AUTHENTICATION_BACKENDS`` to
     prevent locked out users from being logged in by the Django authentication flow.
 
     .. note:: This backend does not log your user in. It monitors login attempts.
```

### Comparing `django-axes-6.0.3/axes/checks.py` & `django-axes-6.0.4/axes/checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/conf.py` & `django-axes-6.0.4/axes/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/decorators.py` & `django-axes-6.0.4/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/handlers/base.py` & `django-axes-6.0.4/axes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/handlers/cache.py` & `django-axes-6.0.4/axes/handlers/cache.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/handlers/database.py` & `django-axes-6.0.4/axes/handlers/database.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/handlers/dummy.py` & `django-axes-6.0.4/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/handlers/proxy.py` & `django-axes-6.0.4/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/handlers/test.py` & `django-axes-6.0.4/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/helpers.py` & `django-axes-6.0.4/axes/helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/ar/LC_MESSAGES/django.mo` & `django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/ar/LC_MESSAGES/django.po` & `django-axes-6.0.4/axes/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-6.0.4/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-6.0.4/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/pl/LC_MESSAGES/django.mo` & `django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/pl/LC_MESSAGES/django.po` & `django-axes-6.0.4/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-6.0.4/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-6.0.4/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/management/commands/axes_reset_failure_logs.py` & `django-axes-6.0.4/axes/management/commands/axes_reset_failure_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/management/commands/axes_reset_ip.py` & `django-axes-6.0.4/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/management/commands/axes_reset_logs.py` & `django-axes-6.0.4/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/management/commands/axes_reset_username.py` & `django-axes-6.0.4/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/middleware.py` & `django-axes-6.0.4/axes/middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/migrations/0001_initial.py` & `django-axes-6.0.4/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-6.0.4/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-6.0.4/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-6.0.4/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/migrations/0007_alter_accessattempt_unique_together.py` & `django-axes-6.0.4/axes/migrations/0007_alter_accessattempt_unique_together.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/migrations/0008_accessfailurelog.py` & `django-axes-6.0.4/axes/migrations/0008_accessfailurelog.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/models.py` & `django-axes-6.0.4/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/signals.py` & `django-axes-6.0.4/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/axes/utils.py` & `django-axes-6.0.4/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/django_axes.egg-info/PKG-INFO` & `django-axes-6.0.4/django_axes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.3
+Version: 6.0.4
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -123,14 +123,21 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.4 (2023-06-22)
+------------------
+
+- Remove unused methods from AxesStandaloneBackend.
+  [314eter]
+
+
 6.0.3 (2023-06-18)
 ------------------
 
 - Add username to admin fieldsets.
   [sevdog]
```

### Comparing `django-axes-6.0.3/django_axes.egg-info/SOURCES.txt` & `django-axes-6.0.4/django_axes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/1_requirements.rst` & `django-axes-6.0.4/docs/1_requirements.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/2_installation.rst` & `django-axes-6.0.4/docs/2_installation.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/3_usage.rst` & `django-axes-6.0.4/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/4_configuration.rst` & `django-axes-6.0.4/docs/4_configuration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/5_customization.rst` & `django-axes-6.0.4/docs/5_customization.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/6_integration.rst` & `django-axes-6.0.4/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/7_architecture.rst` & `django-axes-6.0.4/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/Makefile` & `django-axes-6.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/conf.py` & `django-axes-6.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/docs/images/flow.png` & `django-axes-6.0.4/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/pyproject.toml` & `django-axes-6.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/setup.py` & `django-axes-6.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/base.py` & `django-axes-6.0.4/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/settings.py` & `django-axes-6.0.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_admin.py` & `django-axes-6.0.4/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_attempts.py` & `django-axes-6.0.4/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_backends.py` & `django-axes-6.0.4/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_checks.py` & `django-axes-6.0.4/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_decorators.py` & `django-axes-6.0.4/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_failures.py` & `django-axes-6.0.4/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_handlers.py` & `django-axes-6.0.4/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_helpers.py` & `django-axes-6.0.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_logging.py` & `django-axes-6.0.4/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_login.py` & `django-axes-6.0.4/tests/test_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         self.request = HttpRequest()
         self.request.session = engine.SessionStore()
 
         self.username = "john.doe"
         self.password = "hunter2"
 
-        self.user = get_user_model().objects.create(username=self.username)
+        self.user = get_user_model().objects.create(username=self.username, is_staff=True)
         self.user.set_password(self.password)
         self.user.save()
         self.user.backend = "django.contrib.auth.backends.ModelBackend"
 
 
 class DjangoContribAuthLoginTestCase(DjangoLoginTestCase):
     def test_login(self):
@@ -43,21 +43,27 @@
         logout(self.request)
 
 
 @override_settings(AXES_ENABLED=False)
 class DjangoTestClientLoginTestCase(DjangoLoginTestCase):
     def test_client_login(self):
         self.client.login(username=self.username, password=self.password)
+        response = self.client.get(reverse("admin:index"))
+        self.assertEqual(response.status_code, 200)
 
     def test_client_logout(self):
         self.client.login(username=self.username, password=self.password)
         self.client.logout()
+        response = self.client.get(reverse("admin:index"))
+        self.assertEqual(response.status_code, 302)
 
     def test_client_force_login(self):
         self.client.force_login(self.user)
+        response = self.client.get(reverse("admin:index"))
+        self.assertEqual(response.status_code, 200)
 
 
 class DatabaseLoginTestCase(AxesTestCase):
     """
     Test for lockouts under different configurations and circumstances to prevent false positives and false negatives.
 
     Always block attempted logins for the same user from the same IP.
@@ -279,15 +285,15 @@
         # Test he is locked by ip:
         response = self._login("username2", self.VALID_PASSWORD, ip_addr=self.IP_1, user_agent="test-browser2")
         self.assertEqual(response.status_code, self.BLOCKED)
 
         # Test he is locked by user_agent:
         response = self._login("username2", self.VALID_PASSWORD, ip_addr=self.IP_2, user_agent="test-browser")
         self.assertEqual(response.status_code, self.BLOCKED)
-       
+
         # Test he is allowed to login with different username, ip and user_agent
         response = self._login("username2", self.VALID_PASSWORD, ip_addr=self.IP_2, user_agent="test-browser2")
         self.assertEqual(response.status_code, self.ATTEMPT_NOT_BLOCKED)
 
     @override_settings(AXES_LOCKOUT_PARAMETERS=[["ip_address", "username", "user_agent"]])
     def test_lockout_by_combination_of_all_parameters(self):
         # User is locked out with "test-browser" user agent.
@@ -304,15 +310,15 @@
         # Test he is allowed to login with different IP:
         response = self._login("username", self.VALID_PASSWORD, ip_addr=self.IP_2, user_agent="test-browser")
         self.assertEqual(response.status_code, self.ATTEMPT_NOT_BLOCKED)
 
         # Test he is allowed to login with different user_agent:
         response = self._login("username", self.VALID_PASSWORD, ip_addr=self.IP_1, user_agent="test-browser2")
         self.assertEqual(response.status_code, self.ATTEMPT_NOT_BLOCKED)
-       
+
         # Test he is allowed to login with different username, ip and user_agent
         response = self._login("username2", self.VALID_PASSWORD, ip_addr=self.IP_2, user_agent="test-browser2")
         self.assertEqual(response.status_code, self.ATTEMPT_NOT_BLOCKED)
 
     @override_settings(AXES_LOCKOUT_PARAMETERS=["ip_address", ["username", "user_agent"]])
     def test_lockout_by_ip_or_username_and_user_agent(self):
         # User is locked out with "test-browser" user agent.
```

### Comparing `django-axes-6.0.3/tests/test_management.py` & `django-axes-6.0.4/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_middleware.py` & `django-axes-6.0.4/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.3/tests/test_models.py` & `django-axes-6.0.4/tests/test_models.py`

 * *Files identical despite different names*

