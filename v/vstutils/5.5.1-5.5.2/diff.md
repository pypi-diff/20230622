# Comparing `tmp/vstutils-5.5.1.tar.gz` & `tmp/vstutils-5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.5.1.tar", last modified: Wed Jun 21 00:21:18 2023, max compression
+gzip compressed data, was "vstutils-5.5.2.tar", last modified: Wed Jun 21 03:13:45 2023, max compression
```

## Comparing `vstutils-5.5.1.tar` & `vstutils-5.5.2.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.283280 vstutils-5.5.1/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.5.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.5.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.5.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4431 2023-06-21 00:21:18.283280 vstutils-5.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-19 05:43:06.000000 vstutils-5.5.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 04:31:00.000000 vstutils-5.5.1/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.5.1/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.5.1/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-13 04:11:10.000000 vstutils-5.5.1/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-07 23:11:01.000000 vstutils-5.5.1/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-20 04:07:06.000000 vstutils-5.5.1/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-14 22:04:13.000000 vstutils-5.5.1/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-20 04:07:06.000000 vstutils-5.5.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-21 00:21:18.283280 vstutils-5.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.239279 vstutils-5.5.1/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-21 00:04:50.000000 vstutils-5.5.1/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.247279 vstutils-5.5.1/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-14 22:04:13.000000 vstutils-5.5.1/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.5.1/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:54.000000 vstutils-5.5.1/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    29374 2023-06-14 22:04:13.000000 vstutils-5.5.1/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:43.000000 vstutils-5.5.1/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.5.1/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-14 22:04:13.000000 vstutils-5.5.1/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:43.000000 vstutils-5.5.1/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    13792 2023-06-15 03:16:13.000000 vstutils-5.5.1/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:17:53.000000 vstutils-5.5.1/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.247279 vstutils-5.5.1/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-14 22:04:13.000000 vstutils-5.5.1/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.5.1/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.5.1/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.247279 vstutils-5.5.1/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.5.1/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.5.1/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    28263 2023-06-15 03:16:13.000000 vstutils-5.5.1/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)     9995 2023-06-15 03:16:13.000000 vstutils-5.5.1/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-14 22:04:13.000000 vstutils-5.5.1/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:17:53.000000 vstutils-5.5.1/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3219 2023-06-14 22:04:13.000000 vstutils-5.5.1/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-02-13 06:24:20.000000 vstutils-5.5.1/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:04.000000 vstutils-5.5.1/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.5.1/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.5.1/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.227279 vstutils-5.5.1/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.247279 vstutils-5.5.1/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.247279 vstutils-5.5.1/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.5.1/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.251279 vstutils-5.5.1/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-06-01 04:31:00.000000 vstutils-5.5.1/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.5.1/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.5.1/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.251279 vstutils-5.5.1/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.251279 vstutils-5.5.1/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.5.1/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.5.1/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.5.1/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.5.1/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-07 00:01:28.000000 vstutils-5.5.1/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.255279 vstutils-5.5.1/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:54.000000 vstutils-5.5.1/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25943 2023-06-14 22:04:13.000000 vstutils-5.5.1/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-02-06 06:25:26.000000 vstutils-5.5.1/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:54.000000 vstutils-5.5.1/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.5.1/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:17:53.000000 vstutils-5.5.1/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    55747 2023-06-21 00:04:50.000000 vstutils-5.5.1/vstutils/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:31:00.000000 vstutils-5.5.1/vstutils/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.227279 vstutils-5.5.1/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.263279 vstutils-5.5.1/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126295 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38336 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    71086 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536206 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    89997 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355788 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1798980 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/959.js
--rw-r--r--   0 root         (0) root         (0)     2191 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/959.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    77026 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   303656 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3597 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   434535 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.263279 vstutils-5.5.1/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.267279 vstutils-5.5.1/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5182 2023-05-29 08:17:53.000000 vstutils-5.5.1/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.267279 vstutils-5.5.1/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.5.1/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.5.1/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.5.1/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.5.1/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.267279 vstutils-5.5.1/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.5.1/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.5.1/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.267279 vstutils-5.5.1/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.267279 vstutils-5.5.1/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.5.1/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.271279 vstutils-5.5.1/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.275279 vstutils-5.5.1/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.275279 vstutils-5.5.1/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.275279 vstutils-5.5.1/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.275279 vstutils-5.5.1/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.275279 vstutils-5.5.1/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.5.1/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.279279 vstutils-5.5.1/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.5.1/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.279279 vstutils-5.5.1/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.279279 vstutils-5.5.1/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.279279 vstutils-5.5.1/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.283280 vstutils-5.5.1/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.5.1/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.5.1/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    18153 2023-06-14 22:04:13.000000 vstutils-5.5.1/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.283280 vstutils-5.5.1/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.5.1/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.5.1/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.5.1/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.5.1/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-14 22:04:13.000000 vstutils-5.5.1/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-06-06 00:37:44.000000 vstutils-5.5.1/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.5.1/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:21:18.239279 vstutils-5.5.1/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4431 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7664 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1812 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-21 00:21:18.000000 vstutils-5.5.1/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.440330 vstutils-5.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:36:10.000000 vstutils-5.5.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-05-24 07:40:20.000000 vstutils-5.5.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-05-24 07:40:20.000000 vstutils-5.5.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-06-21 03:13:45.440330 vstutils-5.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2023-05-24 07:40:20.000000 vstutils-5.5.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 04:30:58.000000 vstutils-5.5.2/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:36:10.000000 vstutils-5.5.2/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:36:10.000000 vstutils-5.5.2/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-24 07:40:21.000000 vstutils-5.5.2/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-07 23:11:01.000000 vstutils-5.5.2/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-20 04:07:06.000000 vstutils-5.5.2/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-15 03:16:12.000000 vstutils-5.5.2/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-20 04:07:06.000000 vstutils-5.5.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-21 03:13:45.440330 vstutils-5.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.380330 vstutils-5.5.2/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-21 03:04:37.000000 vstutils-5.5.2/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.388330 vstutils-5.5.2/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:53.000000 vstutils-5.5.2/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    29374 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:44.000000 vstutils-5.5.2/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:44.000000 vstutils-5.5.2/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    13792 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:14:38.000000 vstutils-5.5.2/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.388330 vstutils-5.5.2/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.392330 vstutils-5.5.2/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    28263 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     9995 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:14:38.000000 vstutils-5.5.2/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5660 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:04.000000 vstutils-5.5.2/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.364330 vstutils-5.5.2/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.392330 vstutils-5.5.2/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.392330 vstutils-5.5.2/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.392330 vstutils-5.5.2/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-06-01 04:30:58.000000 vstutils-5.5.2/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.392330 vstutils-5.5.2/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.396330 vstutils-5.5.2/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7832 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-07 00:01:28.000000 vstutils-5.5.2/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.396330 vstutils-5.5.2/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:54.000000 vstutils-5.5.2/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25943 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:54.000000 vstutils-5.5.2/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.5.2/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:14:38.000000 vstutils-5.5.2/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    55747 2023-06-21 00:04:50.000000 vstutils-5.5.2/vstutils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:30:58.000000 vstutils-5.5.2/vstutils/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.368330 vstutils-5.5.2/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.412330 vstutils-5.5.2/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126295 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38336 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    71086 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536206 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    89997 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355788 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1798980 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/959.js
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/959.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    77026 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   303656 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   434535 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.416330 vstutils-5.5.2/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.416330 vstutils-5.5.2/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5182 2023-05-29 08:14:38.000000 vstutils-5.5.2/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.416330 vstutils-5.5.2/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.420330 vstutils-5.5.2/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 07:56:30.000000 vstutils-5.5.2/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.420330 vstutils-5.5.2/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.420330 vstutils-5.5.2/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.424330 vstutils-5.5.2/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.428330 vstutils-5.5.2/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.428330 vstutils-5.5.2/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.428330 vstutils-5.5.2/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.428330 vstutils-5.5.2/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.432330 vstutils-5.5.2/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.436330 vstutils-5.5.2/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.436330 vstutils-5.5.2/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.436330 vstutils-5.5.2/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.436330 vstutils-5.5.2/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.440330 vstutils-5.5.2/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18153 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.440330 vstutils-5.5.2/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    23941 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-05-24 07:40:21.000000 vstutils-5.5.2/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.5.2/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-15 03:16:12.000000 vstutils-5.5.2/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.5.2/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:36:10.000000 vstutils-5.5.2/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 03:13:45.380330 vstutils-5.5.2/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7664 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-21 03:13:45.000000 vstutils-5.5.2/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.5.1/LICENSE` & `vstutils-5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/MANIFEST.in` & `vstutils-5.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/NOTICE` & `vstutils-5.5.2/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/PKG-INFO` & `vstutils-5.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.5.1
+Version: 5.5.2
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.5.1/README.rst` & `vstutils-5.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/requirements.txt` & `vstutils-5.5.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/setup.cfg` & `vstutils-5.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/setup.py` & `vstutils-5.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/actions.py` & `vstutils-5.5.2/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/admin.py` & `vstutils-5.5.2/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/auth.py` & `vstutils-5.5.2/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/base.py` & `vstutils-5.5.2/vstutils/api/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/decorators.py` & `vstutils-5.5.2/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/decorators.pyi` & `vstutils-5.5.2/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/doc_generator.py` & `vstutils-5.5.2/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/endpoint.py` & `vstutils-5.5.2/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/fields.py` & `vstutils-5.5.2/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/filter_backends.py` & `vstutils-5.5.2/vstutils/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/filters.py` & `vstutils-5.5.2/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/health.py` & `vstutils-5.5.2/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/meta.py` & `vstutils-5.5.2/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/metrics.py` & `vstutils-5.5.2/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/migrations/0001_initial.py` & `vstutils-5.5.2/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.5.2/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.5.2/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.5.2/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.5.2/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.5.2/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/models.py` & `vstutils-5.5.2/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/pagination.py` & `vstutils-5.5.2/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/parsers.py` & `vstutils-5.5.2/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/permissions.py` & `vstutils-5.5.2/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/renderers.py` & `vstutils-5.5.2/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/responses.py` & `vstutils-5.5.2/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/responses.pyi` & `vstutils-5.5.2/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/routers.py` & `vstutils-5.5.2/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/routers.pyi` & `vstutils-5.5.2/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/schema/generators.py` & `vstutils-5.5.2/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/schema/info.py` & `vstutils-5.5.2/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/schema/inspectors.py` & `vstutils-5.5.2/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/schema/schema.py` & `vstutils-5.5.2/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/serializers.py` & `vstutils-5.5.2/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/throttling.py` & `vstutils-5.5.2/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/validators.py` & `vstutils-5.5.2/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/api/views.py` & `vstutils-5.5.2/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/asgi.py` & `vstutils-5.5.2/vstutils/asgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/asgi_worker.py` & `vstutils-5.5.2/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/auth.py` & `vstutils-5.5.2/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/auth.pyi` & `vstutils-5.5.2/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/celery_beat_scheduler.py` & `vstutils-5.5.2/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.5.2/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/environment.py` & `vstutils-5.5.2/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/exceptions.py` & `vstutils-5.5.2/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/gui/context.py` & `vstutils-5.5.2/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/gui/forms.py` & `vstutils-5.5.2/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/gui/pwa_manifest.py` & `vstutils-5.5.2/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/gui/views.py` & `vstutils-5.5.2/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/ldap_utils.py` & `vstutils-5.5.2/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/management/commands/_base.py` & `vstutils-5.5.2/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/management/commands/celery_inspect.py` & `vstutils-5.5.2/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/management/commands/dockerrun.py` & `vstutils-5.5.2/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/management/commands/newproject.py` & `vstutils-5.5.2/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/management/commands/run_task.py` & `vstutils-5.5.2/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/management/commands/runrpc.py` & `vstutils-5.5.2/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/management/commands/runserver.py` & `vstutils-5.5.2/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/management/commands/web.py` & `vstutils-5.5.2/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/middleware.py` & `vstutils-5.5.2/vstutils/middleware.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/models/__init__.py` & `vstutils-5.5.2/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/models/base.py` & `vstutils-5.5.2/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/models/cent_notify.py` & `vstutils-5.5.2/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/models/custom_model.py` & `vstutils-5.5.2/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/models/custom_model.pyi` & `vstutils-5.5.2/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/models/decorators.py` & `vstutils-5.5.2/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/models/fields.py` & `vstutils-5.5.2/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/models/queryset.py` & `vstutils-5.5.2/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/settings.ini` & `vstutils-5.5.2/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/settings.py` & `vstutils-5.5.2/vstutils/settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/281.chunk.js` & `vstutils-5.5.2/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/296.chunk.js` & `vstutils-5.5.2/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/345.chunk.js` & `vstutils-5.5.2/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/368.chunk.js` & `vstutils-5.5.2/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/421.js` & `vstutils-5.5.2/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.5.2/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/618.js` & `vstutils-5.5.2/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/683.chunk.js` & `vstutils-5.5.2/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/686.js` & `vstutils-5.5.2/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/742.chunk.js` & `vstutils-5.5.2/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.5.2/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/755.js` & `vstutils-5.5.2/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/826.chunk.js` & `vstutils-5.5.2/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.5.2/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/844.js` & `vstutils-5.5.2/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/959.js` & `vstutils-5.5.2/vstutils/static/bundle/959.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/959.js.LICENSE.txt` & `vstutils-5.5.2/vstutils/static/bundle/959.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/app_loader.js` & `vstutils-5.5.2/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/base.js` & `vstutils-5.5.2/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.5.2/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.5.2/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/output.json` & `vstutils-5.5.2/vstutils/static/bundle/output.json`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/spa.js` & `vstutils-5.5.2/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/bundle/vstutils.js` & `vstutils-5.5.2/vstutils/static/bundle/vstutils.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static/img/anonymous.png` & `vstutils-5.5.2/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/static_files.py` & `vstutils-5.5.2/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/tasks.py` & `vstutils-5.5.2/vstutils/tasks.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/auth/base.html` & `vstutils-5.5.2/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/auth/language_selector.html` & `vstutils-5.5.2/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/auth/tfa.html` & `vstutils-5.5.2/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/base.html` & `vstutils-5.5.2/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/gui/base.html` & `vstutils-5.5.2/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/gui/offline.html` & `vstutils-5.5.2/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/gui/service-worker.js` & `vstutils-5.5.2/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.5.2/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.5.2/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/package.json.template` & `vstutils-5.5.2/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.5.2/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.5.2/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/setup.py.template` & `vstutils-5.5.2/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/test.py.template` & `vstutils-5.5.2/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.5.2/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.5.2/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.5.2/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/registration/confirm_email.html` & `vstutils-5.5.2/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.5.2/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.5.2/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/registration/user_registration.html` & `vstutils-5.5.2/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/rest_framework/admin.html` & `vstutils-5.5.2/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.5.2/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.5.2/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templatetags/request_static.py` & `vstutils-5.5.2/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templatetags/translation.py` & `vstutils-5.5.2/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.5.2/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.5.2/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/templatetags/vstconfigs.py` & `vstutils-5.5.2/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/tests.py` & `vstutils-5.5.2/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/tools.py` & `vstutils-5.5.2/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/translations/cn.py` & `vstutils-5.5.2/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/translations/ru.py` & `vstutils-5.5.2/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/translations/vi.py` & `vstutils-5.5.2/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/urls.py` & `vstutils-5.5.2/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/utils.py` & `vstutils-5.5.2/vstutils/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils/web.ini` & `vstutils-5.5.2/vstutils/web.ini`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # enable threads if it not specified
 if-not-opt = single-interpreter
 single-interpreter = false
 endif =
 
 # use master-mode if it not specified
 if-not-opt = master
-master = false
+master = true
 endif =
 
 # number of workers
 if-not-opt = processes
 processes = %k
 endif =
```

### Comparing `vstutils-5.5.1/vstutils/wsgi.py` & `vstutils-5.5.2/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils.egg-info/PKG-INFO` & `vstutils-5.5.2/vstutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.5.1
+Version: 5.5.2
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.5.1/vstutils.egg-info/SOURCES.txt` & `vstutils-5.5.2/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.1/vstutils.egg-info/requires.txt` & `vstutils-5.5.2/vstutils.egg-info/requires.txt`

 * *Files identical despite different names*

