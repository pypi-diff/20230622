# Comparing `tmp/autodynatrace-1.1.1.tar.gz` & `tmp/autodynatrace-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodynatrace-1.1.1.tar", last modified: Thu Apr  6 14:11:57 2023, max compression
+gzip compressed data, was "autodynatrace-2.0.0.tar", last modified: Thu Jun 22 12:29:02 2023, max compression
```

## Comparing `autodynatrace-1.1.1.tar` & `autodynatrace-2.0.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.843391 autodynatrace-1.1.1/
--rw-rw-rw-   0        0        0    13107 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     1217 2023-04-06 14:11:57.844322 autodynatrace-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3124 2023-04-06 14:05:33.000000 autodynatrace-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.713250 autodynatrace-1.1.1/autodynatrace/
--rw-rw-rw-   0        0        0     4062 2023-04-06 14:05:33.000000 autodynatrace-1.1.1/autodynatrace/__init__.py
--rw-rw-rw-   0        0        0      333 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/log.py
--rw-rw-rw-   0        0        0      545 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/sdk.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.729153 autodynatrace-1.1.1/autodynatrace/wrappers/
--rw-rw-rw-   0        0        0        0 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.733230 autodynatrace-1.1.1/autodynatrace/wrappers/aiohttp/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/aiohttp/__init__.py
--rw-rw-rw-   0        0        0      963 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/aiohttp/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.736248 autodynatrace-1.1.1/autodynatrace/wrappers/bottle/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/bottle/__init__.py
--rw-rw-rw-   0        0        0     2090 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/bottle/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.740316 autodynatrace-1.1.1/autodynatrace/wrappers/celery/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/celery/__init__.py
--rw-rw-rw-   0        0        0     4582 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/celery/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.743765 autodynatrace-1.1.1/autodynatrace/wrappers/concurrent/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/concurrent/__init__.py
--rw-rw-rw-   0        0        0     1731 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/concurrent/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.748772 autodynatrace-1.1.1/autodynatrace/wrappers/confluent_kafka/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/confluent_kafka/__init__.py
--rw-rw-rw-   0        0        0     3644 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/confluent_kafka/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.754286 autodynatrace-1.1.1/autodynatrace/wrappers/custom/
--rw-rw-rw-   0        0        0       46 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/custom/__init__.py
--rw-rw-rw-   0        0        0     2558 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/custom/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.757284 autodynatrace-1.1.1/autodynatrace/wrappers/cx_Oracle/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/cx_Oracle/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-06 14:09:35.000000 autodynatrace-1.1.1/autodynatrace/wrappers/cx_Oracle/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.759287 autodynatrace-1.1.1/autodynatrace/wrappers/dbapi/
--rw-rw-rw-   0        0        0     2704 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/dbapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.774320 autodynatrace-1.1.1/autodynatrace/wrappers/django/
--rw-rw-rw-   0        0        0      157 2023-03-24 23:29:36.000000 autodynatrace-1.1.1/autodynatrace/wrappers/django/__init__.py
--rw-rw-rw-   0        0        0      276 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/django/apps.py
--rw-rw-rw-   0        0        0     1878 2023-03-24 23:29:36.000000 autodynatrace-1.1.1/autodynatrace/wrappers/django/db.py
--rw-rw-rw-   0        0        0     3494 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/django/middlewares.py
--rw-rw-rw-   0        0        0     1788 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/django/utils.py
--rw-rw-rw-   0        0        0      889 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/django/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.779330 autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/__init__.py
--rw-rw-rw-   0        0        0     2443 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/middleware.py
--rw-rw-rw-   0        0        0     1359 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.783374 autodynatrace-1.1.1/autodynatrace/wrappers/flask/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/flask/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/flask/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.788463 autodynatrace-1.1.1/autodynatrace/wrappers/grpc/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/grpc/__init__.py
--rw-rw-rw-   0        0        0     2415 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/grpc/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.791462 autodynatrace-1.1.1/autodynatrace/wrappers/paramiko/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/paramiko/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/paramiko/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.795670 autodynatrace-1.1.1/autodynatrace/wrappers/pika/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/pika/__init__.py
--rw-rw-rw-   0        0        0     3433 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/pika/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.798672 autodynatrace-1.1.1/autodynatrace/wrappers/psycopg2/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/psycopg2/__init__.py
--rw-rw-rw-   0        0        0     2245 2023-04-06 14:08:20.000000 autodynatrace-1.1.1/autodynatrace/wrappers/psycopg2/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.801669 autodynatrace-1.1.1/autodynatrace/wrappers/pymongo/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/pymongo/__init__.py
--rw-rw-rw-   0        0        0     2113 2023-04-06 14:09:35.000000 autodynatrace-1.1.1/autodynatrace/wrappers/pymongo/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.805688 autodynatrace-1.1.1/autodynatrace/wrappers/pysnmp/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/pysnmp/__init__.py
--rw-rw-rw-   0        0        0     4913 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/pysnmp/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.810696 autodynatrace-1.1.1/autodynatrace/wrappers/redis/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/redis/__init__.py
--rw-rw-rw-   0        0        0      747 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/redis/utils.py
--rw-rw-rw-   0        0        0     2111 2023-04-06 14:09:48.000000 autodynatrace-1.1.1/autodynatrace/wrappers/redis/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.815364 autodynatrace-1.1.1/autodynatrace/wrappers/ruxit/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/ruxit/__init__.py
--rw-rw-rw-   0        0        0      475 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/ruxit/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.818159 autodynatrace-1.1.1/autodynatrace/wrappers/sqlalchemy/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/sqlalchemy/__init__.py
--rw-rw-rw-   0        0        0     4496 2023-04-06 14:09:58.000000 autodynatrace-1.1.1/autodynatrace/wrappers/sqlalchemy/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.822168 autodynatrace-1.1.1/autodynatrace/wrappers/starlette/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/starlette/__init__.py
--rw-rw-rw-   0        0        0     1459 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/starlette/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.826767 autodynatrace-1.1.1/autodynatrace/wrappers/subprocess/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/subprocess/__init__.py
--rw-rw-rw-   0        0        0     1401 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/subprocess/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.829769 autodynatrace-1.1.1/autodynatrace/wrappers/suds/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/suds/__init__.py
--rw-rw-rw-   0        0        0      715 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/suds/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.834289 autodynatrace-1.1.1/autodynatrace/wrappers/tornado/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/tornado/__init__.py
--rw-rw-rw-   0        0        0     1744 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/tornado/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.837810 autodynatrace-1.1.1/autodynatrace/wrappers/urllib/
--rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/urllib/__init__.py
--rw-rw-rw-   0        0        0     1563 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/urllib/wrapper.py
--rw-rw-rw-   0        0        0      108 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/autodynatrace/wrappers/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.725853 autodynatrace-1.1.1/autodynatrace.egg-info/
--rw-rw-rw-   0        0        0     1217 2023-04-06 14:11:57.000000 autodynatrace-1.1.1/autodynatrace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2781 2023-04-06 14:11:57.000000 autodynatrace-1.1.1/autodynatrace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 14:11:57.000000 autodynatrace-1.1.1/autodynatrace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-06 14:11:57.000000 autodynatrace-1.1.1/autodynatrace.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       61 2023-04-06 14:11:57.000000 autodynatrace-1.1.1/autodynatrace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-06 14:11:57.000000 autodynatrace-1.1.1/autodynatrace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2023-04-06 14:11:57.845325 autodynatrace-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1628 2023-04-06 14:10:07.000000 autodynatrace-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:11:57.841806 autodynatrace-1.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     6901 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/tests/test_custom.py
--rw-rw-rw-   0        0        0     1365 2023-01-05 00:24:24.000000 autodynatrace-1.1.1/tests/test_django.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.559888 autodynatrace-2.0.0/
+-rw-rw-rw-   0        0        0    13107 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1185 2023-06-22 12:29:02.559888 autodynatrace-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3124 2023-04-06 14:05:33.000000 autodynatrace-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.494408 autodynatrace-2.0.0/autodynatrace/
+-rw-rw-rw-   0        0        0     4062 2023-04-06 14:05:33.000000 autodynatrace-2.0.0/autodynatrace/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/log.py
+-rw-rw-rw-   0        0        0      545 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/sdk.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.494408 autodynatrace-2.0.0/autodynatrace/wrappers/
+-rw-rw-rw-   0        0        0        0 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.494408 autodynatrace-2.0.0/autodynatrace/wrappers/aiohttp/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/aiohttp/__init__.py
+-rw-rw-rw-   0        0        0      963 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/aiohttp/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/bottle/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/bottle/__init__.py
+-rw-rw-rw-   0        0        0     2090 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/bottle/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/celery/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/celery/__init__.py
+-rw-rw-rw-   0        0        0     4582 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/celery/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/concurrent/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/concurrent/__init__.py
+-rw-rw-rw-   0        0        0     1731 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/concurrent/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/confluent_kafka/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/confluent_kafka/__init__.py
+-rw-rw-rw-   0        0        0     3644 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/confluent_kafka/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/custom/
+-rw-rw-rw-   0        0        0       46 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/custom/__init__.py
+-rw-rw-rw-   0        0        0     2558 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/custom/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/cx_Oracle/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/cx_Oracle/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-06 14:09:35.000000 autodynatrace-2.0.0/autodynatrace/wrappers/cx_Oracle/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.506415 autodynatrace-2.0.0/autodynatrace/wrappers/dbapi/
+-rw-rw-rw-   0        0        0     2880 2023-06-22 00:20:35.000000 autodynatrace-2.0.0/autodynatrace/wrappers/dbapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.522048 autodynatrace-2.0.0/autodynatrace/wrappers/django/
+-rw-rw-rw-   0        0        0      157 2023-03-24 23:29:36.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/apps.py
+-rw-rw-rw-   0        0        0     1878 2023-03-24 23:29:36.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/db.py
+-rw-rw-rw-   0        0        0     3494 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/middlewares.py
+-rw-rw-rw-   0        0        0     1788 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/utils.py
+-rw-rw-rw-   0        0        0      889 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/django/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.525559 autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     2443 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/middleware.py
+-rw-rw-rw-   0        0        0     1359 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.525559 autodynatrace-2.0.0/autodynatrace/wrappers/flask/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/flask/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/flask/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.525559 autodynatrace-2.0.0/autodynatrace/wrappers/grpc/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/grpc/__init__.py
+-rw-rw-rw-   0        0        0     2415 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/grpc/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.525559 autodynatrace-2.0.0/autodynatrace/wrappers/paramiko/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/paramiko/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/paramiko/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.535328 autodynatrace-2.0.0/autodynatrace/wrappers/pika/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pika/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pika/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.536996 autodynatrace-2.0.0/autodynatrace/wrappers/psycopg2/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/psycopg2/__init__.py
+-rw-rw-rw-   0        0        0     2248 2023-06-22 12:06:15.000000 autodynatrace-2.0.0/autodynatrace/wrappers/psycopg2/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.539740 autodynatrace-2.0.0/autodynatrace/wrappers/pymongo/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pymongo/__init__.py
+-rw-rw-rw-   0        0        0     2113 2023-04-06 14:09:35.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pymongo/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.541832 autodynatrace-2.0.0/autodynatrace/wrappers/pysnmp/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pysnmp/__init__.py
+-rw-rw-rw-   0        0        0     4913 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/pysnmp/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.544453 autodynatrace-2.0.0/autodynatrace/wrappers/redis/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/redis/__init__.py
+-rw-rw-rw-   0        0        0      747 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/redis/utils.py
+-rw-rw-rw-   0        0        0     2111 2023-04-06 14:09:48.000000 autodynatrace-2.0.0/autodynatrace/wrappers/redis/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.546513 autodynatrace-2.0.0/autodynatrace/wrappers/ruxit/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/ruxit/__init__.py
+-rw-rw-rw-   0        0        0      475 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/ruxit/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.548057 autodynatrace-2.0.0/autodynatrace/wrappers/sqlalchemy/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/sqlalchemy/__init__.py
+-rw-rw-rw-   0        0        0     4496 2023-04-06 14:09:58.000000 autodynatrace-2.0.0/autodynatrace/wrappers/sqlalchemy/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.550140 autodynatrace-2.0.0/autodynatrace/wrappers/starlette/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/starlette/__init__.py
+-rw-rw-rw-   0        0        0     1459 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/starlette/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.551168 autodynatrace-2.0.0/autodynatrace/wrappers/subprocess/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/subprocess/__init__.py
+-rw-rw-rw-   0        0        0     1401 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/subprocess/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.552903 autodynatrace-2.0.0/autodynatrace/wrappers/suds/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/suds/__init__.py
+-rw-rw-rw-   0        0        0      715 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/suds/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.552903 autodynatrace-2.0.0/autodynatrace/wrappers/tornado/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/tornado/__init__.py
+-rw-rw-rw-   0        0        0     1744 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/tornado/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.556930 autodynatrace-2.0.0/autodynatrace/wrappers/urllib/
+-rw-rw-rw-   0        0        0       33 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/urllib/__init__.py
+-rw-rw-rw-   0        0        0     1563 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/urllib/wrapper.py
+-rw-rw-rw-   0        0        0      108 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/autodynatrace/wrappers/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.494408 autodynatrace-2.0.0/autodynatrace.egg-info/
+-rw-rw-rw-   0        0        0     1185 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2781 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       61 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-22 12:29:02.000000 autodynatrace-2.0.0/autodynatrace.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2023-06-22 12:29:02.559888 autodynatrace-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1596 2023-06-21 23:57:15.000000 autodynatrace-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:29:02.559888 autodynatrace-2.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     6901 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/tests/test_custom.py
+-rw-rw-rw-   0        0        0     1365 2023-01-05 00:24:24.000000 autodynatrace-2.0.0/tests/test_django.py
```

### Comparing `autodynatrace-1.1.1/LICENSE` & `autodynatrace-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/PKG-INFO` & `autodynatrace-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodynatrace
-Version: 1.1.1
+Version: 2.0.0
 Summary: Auto instrumentation for the OneAgent SDK
 Home-page: https://github.com/dlopes7/autodynatrace
 Author: David Lopes
 Author-email: david.lopes@dynatrace.com
 Project-URL: Issue Tracker, https://github.com/dlopes7/autodynatrace/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,11 +17,11 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+Requires-Python: >=3.6
 License-File: LICENSE
 
 The autodynatrace package will auto instrument your python apps
```

### Comparing `autodynatrace-1.1.1/README.md` & `autodynatrace-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/__init__.py` & `autodynatrace-2.0.0/autodynatrace/__init__.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/sdk.py` & `autodynatrace-2.0.0/autodynatrace/sdk.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/aiohttp/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/aiohttp/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/bottle/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/bottle/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/celery/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/celery/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/concurrent/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/concurrent/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/confluent_kafka/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/confluent_kafka/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/custom/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/custom/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/cx_Oracle/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/cx_Oracle/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/dbapi/__init__.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/dbapi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,33 @@
 from ...sdk import sdk
 from ..utils import normalize_vendor
 
 
 class TracedCursor(wrapt.ObjectProxy):
     def __init__(self, cursor, db_info):
         super(TracedCursor, self).__init__(cursor)
-        self.db_info = db_info
+        self.db_info = f"{db_info}"
         self._self_last_execute_operation = None
         self._original_cursor = cursor
 
     def _trace_method(self, method, query, *args, **kwargs):
 
         # It could be psycopg2.sql.Composable, but we don't want to import that here
         if not isinstance(query, str):
             try:
                 query = query.as_string(self._original_cursor)
             except Exception:
                 pass
         logger.debug("Tracing Database Call '{}' to {}".format(str(query), self.db_info))
-        with sdk.trace_sql_database_request(self.db_info, query):
+
+        try:
+            with sdk.trace_sql_database_request(self.db_info, f"{query}"):
+                return method(*args, **kwargs)
+        except Exception as e:
+            logger.warning(f"Error instrumenting database: {e}")
             return method(*args, **kwargs)
 
     def executemany(self, query, *args, **kwargs):
         self._self_last_execute_operation = query
         return self._trace_method(self.__wrapped__.executemany, query, query, *args, **kwargs)
 
     def execute(self, query, *args, **kwargs):
```

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/django/db.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/django/db.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/django/middlewares.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/django/utils.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/django/utils.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/django/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/django/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/middleware.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/fastapi/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/flask/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/flask/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/grpc/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/grpc/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/paramiko/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/paramiko/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/pika/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/pika/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/psycopg2/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/psycopg2/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ...sdk import sdk
 
 
 def instrument():
     def parse_dsn(dsn):
         return {c.split("=")[0]: c.split("=")[1] for c in dsn.split() if "=" in c}
 
-    class DynatraceCursor(psycopg2.extensions.cursor):
+    class DynatraceCursor(psycopg2.extra.DictCursorBase):
         def __init__(self, *args, **kwargs):
             self._dynatrace_db_info = kwargs.pop("dynatrace_db_info", None)
             super(DynatraceCursor, self).__init__(*args, **kwargs)
 
         def execute(self, query, vars=None):
             if hasattr(self, "_dynatrace_db_info") and self._dynatrace_db_info is not None:
                 with sdk.trace_sql_database_request(self._dynatrace_db_info, "{}".format(query)) as tracer:
```

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/pymongo/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/pymongo/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/pysnmp/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/pysnmp/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/redis/utils.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/redis/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/redis/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/sqlalchemy/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/sqlalchemy/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/starlette/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/starlette/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/subprocess/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/subprocess/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/suds/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/suds/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/tornado/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/tornado/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace/wrappers/urllib/wrapper.py` & `autodynatrace-2.0.0/autodynatrace/wrappers/urllib/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/autodynatrace.egg-info/PKG-INFO` & `autodynatrace-2.0.0/autodynatrace.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodynatrace
-Version: 1.1.1
+Version: 2.0.0
 Summary: Auto instrumentation for the OneAgent SDK
 Home-page: https://github.com/dlopes7/autodynatrace
 Author: David Lopes
 Author-email: david.lopes@dynatrace.com
 Project-URL: Issue Tracker, https://github.com/dlopes7/autodynatrace/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,11 +17,11 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+Requires-Python: >=3.6
 License-File: LICENSE
 
 The autodynatrace package will auto instrument your python apps
```

### Comparing `autodynatrace-1.1.1/autodynatrace.egg-info/SOURCES.txt` & `autodynatrace-2.0.0/autodynatrace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/setup.py` & `autodynatrace-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="autodynatrace",
-    version="1.1.1",
+    version="2.0.0",
     packages=find_packages(),
     package_data={"autodynatrace": ["wrappers/*"]},
     install_requires=["wrapt>=1.11.2", "oneagent-sdk>=1.3.0", "six>=1.10.0", "autowrapt>=1.0"],
     tests_require=["pytest", "mock", "tox", "django"],
     entry_points={"autodynatrace": ["string = autodynatrace:load"]},
-    python_requires=">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*",
+    python_requires=">=3.6",
     author="David Lopes",
     author_email="david.lopes@dynatrace.com",
     description="Auto instrumentation for the OneAgent SDK",
     long_description="The autodynatrace package will auto instrument your python apps",
     url="https://github.com/dlopes7/autodynatrace",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `autodynatrace-1.1.1/tests/test_custom.py` & `autodynatrace-2.0.0/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-1.1.1/tests/test_django.py` & `autodynatrace-2.0.0/tests/test_django.py`

 * *Files identical despite different names*

