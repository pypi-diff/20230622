# Comparing `tmp/esi-leap-0.2.6.tar.gz` & `tmp/esi-leap-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tzumainn/development/esi-leap/dist/tmp4qovt1bn/esi-leap-0.2.6.tar", last modified: Tue Nov  1 21:39:46 2022, max compression
+gzip compressed data, was "/home/tzumainn/development/esi-leap/dist/tmp7k6dlkp1/esi-leap-0.2.7.tar", last modified: Thu Jun 22 18:19:04 2023, max compression
```

## Comparing `esi-leap-0.2.6.tar` & `esi-leap-0.2.7.tar`

### file list

```diff
@@ -1,155 +1,165 @@
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      456 2022-11-01 21:39:42.000000 esi-leap-0.2.6/AUTHORS
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5204 2022-11-01 21:39:46.000000 esi-leap-0.2.6/PKG-INFO
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       63 2022-05-25 19:28:05.000000 esi-leap-0.2.6/.stestr.conf
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap.egg-info/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5204 2022-11-01 21:39:42.000000 esi-leap-0.2.6/esi_leap.egg-info/PKG-INFO
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2022-11-01 21:39:42.000000 esi-leap-0.2.6/esi_leap.egg-info/pbr.json
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-05-25 19:49:35.000000 esi-leap-0.2.6/esi_leap.egg-info/not-zip-safe
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      508 2022-11-01 21:39:42.000000 esi-leap-0.2.6/esi_leap.egg-info/entry_points.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3806 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap.egg-info/SOURCES.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        9 2022-11-01 21:39:42.000000 esi-leap-0.2.6/esi_leap.egg-info/top_level.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-11-01 21:39:42.000000 esi-leap-0.2.6/esi_leap.egg-info/dependency_links.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      756 2022-11-01 21:39:42.000000 esi-leap-0.2.6/esi_leap.egg-info/requires.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      597 2022-06-16 17:07:25.000000 esi-leap-0.2.6/setup.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       17 2022-05-25 19:28:05.000000 esi-leap-0.2.6/babel.cfg
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/etc/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/etc/esi-leap/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      395 2022-05-25 19:28:05.000000 esi-leap-0.2.6/etc/esi-leap/esi-leap-config-generator.conf
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       77 2022-05-25 19:28:05.000000 esi-leap-0.2.6/etc/esi-leap/esi-leap-policy-generator.conf
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1605 2022-06-16 17:07:25.000000 esi-leap-0.2.6/tox.ini
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8975 2022-11-01 21:39:42.000000 esi-leap-0.2.6/ChangeLog
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4188 2022-07-25 14:12:31.000000 esi-leap-0.2.6/README.md
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/.github/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/.github/workflows/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      589 2022-05-26 14:27:40.000000 esi-leap-0.2.6/.github/workflows/tests.yml
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      719 2022-06-16 17:07:25.000000 esi-leap-0.2.6/test-requirements.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10143 2022-05-25 19:28:05.000000 esi-leap-0.2.6/LICENSE
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1364 2022-11-01 21:39:46.000000 esi-leap-0.2.6/setup.cfg
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/docs/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8983 2022-07-25 14:12:31.000000 esi-leap-0.2.6/docs/esi-leap-requirements.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1176 2022-07-25 14:12:31.000000 esi-leap-0.2.6/docs/esi-leap-reporting.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5962 2022-07-25 14:12:31.000000 esi-leap-0.2.6/docs/esi-leap-policy.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5858 2022-07-25 14:12:31.000000 esi-leap-0.2.6/docs/esi-leap-api-ref.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1312 2022-07-08 14:49:10.000000 esi-leap-0.2.6/requirements.txt
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/resource_objects/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1977 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/resource_objects/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1405 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/resource_objects/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2580 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/resource_objects/dummy_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1386 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/resource_objects/test_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3711 2022-11-01 21:35:38.000000 esi-leap-0.2.6/esi_leap/resource_objects/ironic_node.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/api/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2060 2022-11-01 21:35:38.000000 esi-leap-0.2.6/esi_leap/api/app.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/api/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/api/controllers/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      928 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/api/controllers/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2014 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/api/controllers/types.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/api/controllers/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/api/controllers/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4199 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/api/controllers/v1/node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6583 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/api/controllers/v1/utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10320 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/api/controllers/v1/lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/api/controllers/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1509 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/api/controllers/v1/root.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11072 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/api/controllers/v1/offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1424 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/api/controllers/root.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1380 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/api/service.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1032 2022-11-01 21:35:38.000000 esi-leap-0.2.6/esi_leap/api/wsgi.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/objects/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1578 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/objects/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8708 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/objects/lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      102 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/objects/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1577 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/objects/fields.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7616 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/objects/offer.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/manager/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      944 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/manager/utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/manager/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5406 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/manager/service.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      994 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/manager/rpcapi.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/common/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4773 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/common/exception.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      783 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/common/utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/common/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4899 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/common/policy.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1956 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/common/ironic.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1253 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/common/service.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      770 2022-11-01 21:35:38.000000 esi-leap-0.2.6/esi_leap/common/i18n.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      603 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/common/constants.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      874 2022-08-19 19:29:16.000000 esi-leap-0.2.6/esi_leap/common/statuses.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2509 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/common/keystone.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/db/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      766 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/db/base.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4044 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/models.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      494 2022-07-08 14:49:10.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic/script.py.mako
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-07-08 14:49:10.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      622 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic/README.md
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic/versions/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-07-08 14:49:10.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic/versions/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1873 2022-07-08 14:49:10.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic/env.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2180 2022-07-08 14:49:10.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic.ini
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    14151 2022-08-19 19:29:16.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3140 2022-07-08 14:49:10.000000 esi-leap-0.2.6/esi_leap/db/sqlalchemy/migration.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/db/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3994 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/db/api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1437 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/db/migration.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      645 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/version.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/conf/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      921 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/conf/opts.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1038 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/conf/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      984 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/conf/pecan.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      819 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/conf/dummy_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1058 2022-08-19 19:29:16.000000 esi-leap-0.2.6/esi_leap/conf/api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2138 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/conf/ironic.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2154 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/conf/keystone.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      732 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/conf/netconf.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2563 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/base.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/resource_objects/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1371 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/resource_objects/test_base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/resource_objects/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3082 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/resource_objects/test_test_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5188 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/resource_objects/test_dummy_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4002 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/resource_objects/test_resource_objects.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8858 2022-11-01 21:35:38.000000 esi-leap-0.2.6/esi_leap/tests/resource_objects/test_ironic_node.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/api/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6213 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/api/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/api/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/api/controllers/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/api/controllers/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    34020 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/test_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2313 2022-08-19 19:29:16.000000 esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/test_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    28966 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/test_utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    30769 2022-08-19 19:29:16.000000 esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/test_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1646 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/api/controllers/test_types.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/objects/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    21525 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/objects/test_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1614 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/objects/test_fields.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/objects/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13516 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/objects/test_offer.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/manager/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8677 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/manager/test_service.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/manager/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/common/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1676 2022-09-19 15:54:31.000000 esi-leap-0.2.6/esi_leap/tests/common/test_ironic.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/common/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      968 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/common/test_utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3594 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/common/test_keystone.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1576 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/tests/common/test_policy.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/db/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/tests/db/sqlalchemy/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    29705 2022-08-19 19:29:16.000000 esi-leap-0.2.6/esi_leap/tests/db/sqlalchemy/test_api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/db/sqlalchemy/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/tests/db/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-11-01 21:39:46.000000 esi-leap-0.2.6/esi_leap/cmd/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2928 2022-07-25 14:12:31.000000 esi-leap-0.2.6/esi_leap/cmd/dbsync.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       49 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/cmd/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1073 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/cmd/api.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      962 2022-05-25 19:28:05.000000 esi-leap-0.2.6/esi_leap/cmd/manager.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/.github/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/.github/workflows/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      604 2023-05-18 17:47:59.000000 esi-leap-0.2.7/.github/workflows/tests.yml
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/docs/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5858 2022-07-25 14:12:31.000000 esi-leap-0.2.7/docs/esi-leap-api-ref.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5962 2022-07-25 14:12:31.000000 esi-leap-0.2.7/docs/esi-leap-policy.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1176 2022-07-25 14:12:31.000000 esi-leap-0.2.7/docs/esi-leap-reporting.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8983 2022-07-25 14:12:31.000000 esi-leap-0.2.7/docs/esi-leap-requirements.md
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/api/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/api/controllers/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/api/controllers/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/api/controllers/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10348 2023-06-15 16:56:57.000000 esi-leap-0.2.7/esi_leap/api/controllers/v1/lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4199 2022-09-19 15:54:31.000000 esi-leap-0.2.7/esi_leap/api/controllers/v1/node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11054 2023-05-25 15:41:42.000000 esi-leap-0.2.7/esi_leap/api/controllers/v1/offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1509 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/api/controllers/v1/root.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6501 2023-05-25 15:41:42.000000 esi-leap-0.2.7/esi_leap/api/controllers/v1/utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/api/controllers/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      928 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/api/controllers/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1424 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/api/controllers/root.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2014 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/api/controllers/types.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/api/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2060 2022-11-01 21:35:38.000000 esi-leap-0.2.7/esi_leap/api/app.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1380 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/api/service.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1032 2022-11-01 21:35:38.000000 esi-leap-0.2.7/esi_leap/api/wsgi.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/cmd/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       49 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/cmd/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1073 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/cmd/api.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2928 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/cmd/dbsync.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      962 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/cmd/manager.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/common/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/common/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      603 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/common/constants.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5509 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/common/exception.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      770 2022-11-01 21:35:38.000000 esi-leap-0.2.7/esi_leap/common/i18n.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1956 2022-09-19 15:54:31.000000 esi-leap-0.2.7/esi_leap/common/ironic.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2509 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/common/keystone.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6116 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/common/notification_utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4899 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/common/policy.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3221 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/common/rpc.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1304 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/common/service.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      874 2022-08-19 19:29:16.000000 esi-leap-0.2.7/esi_leap/common/statuses.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      783 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/common/utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/conf/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1110 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/conf/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1058 2022-08-19 19:29:16.000000 esi-leap-0.2.7/esi_leap/conf/api.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      819 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/conf/dummy_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2138 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/conf/ironic.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2154 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/conf/keystone.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      732 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/conf/netconf.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1638 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/conf/notification.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      976 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/conf/opts.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      984 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/conf/pecan.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/db/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-07-08 14:49:10.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic/versions/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      622 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-07-08 14:49:10.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1873 2022-07-08 14:49:10.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic/env.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      494 2022-07-08 14:49:10.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic/script.py.mako
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2180 2022-07-08 14:49:10.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic.ini
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    14151 2022-08-19 19:29:16.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/api.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3140 2022-07-08 14:49:10.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/migration.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4093 2023-06-15 16:56:57.000000 esi-leap-0.2.7/esi_leap/db/sqlalchemy/models.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/db/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3994 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/db/api.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      766 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/db/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1437 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/db/migration.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/manager/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/manager/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      994 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/manager/rpcapi.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5406 2022-09-19 15:54:31.000000 esi-leap-0.2.7/esi_leap/manager/service.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      944 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/manager/utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/objects/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      102 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/objects/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1578 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/objects/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2393 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/objects/fields.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13235 2023-06-22 18:18:25.000000 esi-leap-0.2.7/esi_leap/objects/lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6520 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/objects/notification.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7616 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/objects/offer.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/resource_objects/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1405 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/resource_objects/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2261 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/resource_objects/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4240 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/resource_objects/dummy_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      910 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/resource_objects/error.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5599 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/resource_objects/ironic_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1491 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/resource_objects/test_node.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/api/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/api/controllers/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    34059 2023-06-15 16:56:57.000000 esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/test_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2313 2022-08-19 19:29:16.000000 esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/test_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    30769 2022-08-19 19:29:16.000000 esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/test_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    28120 2023-05-25 15:41:42.000000 esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/test_utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/api/controllers/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1646 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/tests/api/controllers/test_types.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/api/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6213 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/tests/api/base.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/common/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/common/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1676 2022-09-19 15:54:31.000000 esi-leap-0.2.7/esi_leap/tests/common/test_ironic.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3594 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/tests/common/test_keystone.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3233 2023-06-22 18:18:25.000000 esi-leap-0.2.7/esi_leap/tests/common/test_notification_utils.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1576 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/tests/common/test_policy.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6450 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/tests/common/test_rpc.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      968 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/common/test_utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/db/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/db/sqlalchemy/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    29945 2023-06-15 16:56:57.000000 esi-leap-0.2.7/esi_leap/tests/db/sqlalchemy/test_api.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/db/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/manager/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/manager/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8677 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/tests/manager/test_service.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/objects/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/objects/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2715 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/tests/objects/test_fields.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    31005 2023-06-22 18:18:25.000000 esi-leap-0.2.7/esi_leap/tests/objects/test_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    12357 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/tests/objects/test_notification.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13516 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/tests/objects/test_offer.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap/tests/resource_objects/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/resource_objects/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1950 2023-05-25 15:41:42.000000 esi-leap-0.2.7/esi_leap/tests/resource_objects/test_base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6019 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/tests/resource_objects/test_dummy_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9414 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/tests/resource_objects/test_ironic_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3966 2023-05-25 15:41:42.000000 esi-leap-0.2.7/esi_leap/tests/resource_objects/test_resource_objects.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2986 2023-06-08 21:26:09.000000 esi-leap-0.2.7/esi_leap/tests/resource_objects/test_test_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/tests/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2563 2022-07-25 14:12:31.000000 esi-leap-0.2.7/esi_leap/tests/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      645 2022-05-25 19:28:05.000000 esi-leap-0.2.7/esi_leap/version.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap.egg-info/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6494 2023-06-22 18:19:03.000000 esi-leap-0.2.7/esi_leap.egg-info/PKG-INFO
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4122 2023-06-22 18:19:04.000000 esi-leap-0.2.7/esi_leap.egg-info/SOURCES.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2023-06-22 18:19:03.000000 esi-leap-0.2.7/esi_leap.egg-info/dependency_links.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      508 2023-06-22 18:19:03.000000 esi-leap-0.2.7/esi_leap.egg-info/entry_points.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-05-25 19:49:35.000000 esi-leap-0.2.7/esi_leap.egg-info/not-zip-safe
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2023-06-22 18:19:03.000000 esi-leap-0.2.7/esi_leap.egg-info/pbr.json
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      805 2023-06-22 18:19:03.000000 esi-leap-0.2.7/esi_leap.egg-info/requires.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        9 2023-06-22 18:19:03.000000 esi-leap-0.2.7/esi_leap.egg-info/top_level.txt
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/etc/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 18:19:04.000000 esi-leap-0.2.7/etc/esi-leap/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      395 2022-05-25 19:28:05.000000 esi-leap-0.2.7/etc/esi-leap/esi-leap-config-generator.conf
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       77 2022-05-25 19:28:05.000000 esi-leap-0.2.7/etc/esi-leap/esi-leap-policy-generator.conf
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       63 2022-05-25 19:28:05.000000 esi-leap-0.2.7/.stestr.conf
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      548 2023-06-22 18:19:03.000000 esi-leap-0.2.7/AUTHORS
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9452 2023-06-22 18:19:03.000000 esi-leap-0.2.7/ChangeLog
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      680 2023-05-25 15:41:42.000000 esi-leap-0.2.7/Containerfile
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10143 2022-05-25 19:28:05.000000 esi-leap-0.2.7/LICENSE
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5478 2023-05-25 15:41:42.000000 esi-leap-0.2.7/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       17 2022-05-25 19:28:05.000000 esi-leap-0.2.7/babel.cfg
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1410 2023-06-22 18:18:25.000000 esi-leap-0.2.7/requirements.txt
+-rwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)      777 2023-05-25 15:41:42.000000 esi-leap-0.2.7/run_services.sh
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1364 2023-06-22 18:19:04.000000 esi-leap-0.2.7/setup.cfg
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      597 2022-06-16 17:07:25.000000 esi-leap-0.2.7/setup.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      750 2023-06-08 21:26:09.000000 esi-leap-0.2.7/test-requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1648 2023-05-18 17:47:59.000000 esi-leap-0.2.7/tox.ini
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6494 2023-06-22 18:19:04.000000 esi-leap-0.2.7/PKG-INFO
```

### Comparing `esi-leap-0.2.6/PKG-INFO` & `esi-leap-0.2.7/esi_leap.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-leap
-Version: 0.2.6
+Version: 0.2.7
 Summary: ESI provider
 Home-page: UNKNOWN
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -24,19 +24,21 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # esi-leap
 
-esi-leap is an OpenStack service for acting as a FLOCX provider to communicate with a FLOCX
-marketplace. It is intended to work on top of the
-[esi-common library](https://github.com/CCI-MOC/esi-common), which supports an OpenStack
-install that simulates Ironic multi-tenancy through the use of `project_owner_id` and
-`project_id` property attributes.
+esi-leap is an OpenStack service for leasing baremetal nodes, designed to run
+on top of [multi-tenant
+Ironic](https://docs.openstack.org/ironic/latest/admin/node-multitenancy.html).
+It consists of an API that provides endpoints for leasing operations and a
+manager service that updates the status of leases and offers as required. See
+the [documentation](https://esi.readthedocs.io/en/latest/index.html) for
+more info on ESI.
 
 
 ### Installation
 
 To install as a package:
  - `pip install esi-leap`
 
@@ -53,50 +55,54 @@
 
 esi-leap has a command line client which can be found here:
 https://github.com/CCI-MOC/python-esileapclient
 
 
 ### Create the esi-leap Database
 
-The esi-leap service requires a database to store its information. To set this up using
-the MySQL database used by other OpenStack services, run the following, replacing
-\<PASSWORD\> with a suitable password and \<DATABASE\_IP\> with the IP address of your
-MySQL database (if you're not sure, use localhost or 127.0.0.1).
+The esi-leap service requires a database to store its information. To set this
+up using the MySQL database used by other OpenStack services, run the following
+commands, replacing \<PASSWORD\> with a suitable password and \<DATABASE\_IP\>
+with the IP address of your MySQL database (if you're not sure, use localhost
+or 127.0.0.1).
 
 ```
     $ mysql -u root -p
     mysql> CREATE USER 'esi_leap'@'<DATABASE_IP>' IDENTIFIED BY '<PASSWORD>';
+    mysql> CREATE USER 'esi_leap'@'%' IDENTIFIED BY '<PASSWORD>';
     mysql> CREATE DATABASE esi_leap CHARACTER SET utf8;
     mysql> GRANT ALL PRIVILEGES ON esi_leap.* TO 'esi_leap'@'<DATABASE_IP>';
+    mysql> GRANT ALL PRIVILEGES ON esi_leap.* TO 'esi_leap'@'%';
     mysql> FLUSH PRIVILEGES;
 ```
 
 If you use this method, the resulting database connection string should be:
 
 ```
     mysql+pymysql://esi_leap:PASSWORD@DATABASE_IP/esi_leap
 ```
 
 
 ### Configuration
 
-Run the following to generate the configuration file and copy it to the right place:
+Run the following commands to generate the configuration file and copy it to
+the right place:
 
 ```
     $ tox -egenconfig
     $ sudo mkdir /etc/esi-leap
     $ sudo cp etc/esi-leap/esi-leap.conf.sample /etc/esi-leap/esi-leap.conf
 ```
 
-Edit `/etc/esi-leap/esi-leap.conf` with the proper values. Some useful values include:
+Edit `/etc/esi-leap/esi-leap.conf` with the proper values. (see sample config
+template below):
 
 ```
 [DEFAULT]
 
-debug=True
 log_dir=/var/log/esi-leap
 transport_url=<transport URL for messaging>
 
 [database]
 connection=<db connection string>
 
 # End-user authentication configuration
@@ -111,29 +117,28 @@
 project_domain_name=Default
 
 # esi-leap internal authentication configuration
 [keystone]
 api_endpoint=<admin Keystone endpoint>
 auth_type=password
 auth_url=<keystone auth URL>
-username=admin
+username=esi-leap
 password=<password>
 user_domain_name=Default
-project_name=admin
+project_name=service
 project_domain_name=Default
 
 [oslo_concurrency]
 lock_path=<lock dir>
 
 [oslo_messaging_notifications]
 driver=messagingv2
 transport_url=<transport URL for messaging>
 
 [ironic]                              # ONLY NECESSARY IF USING IRONIC NODES
-
 auth_type = password
 api_endpoint = <ironic API endpoint>
 auth_url = <keystone auth URL>
 project_name = service
 project_domain_name = Default
 user_domain_name = Default
 username = ironic
@@ -143,16 +148,18 @@
 dummy_node_dir=/tmp/nodes
 ```
 
 
 ### Create the OpenStack Service
 
 ```
+    $ openstack user create --domain default --password-prompt esi-leap
+    $ openstack role add --project service --user esi-leap admin
     $ openstack service create --name esi-leap lease
-    $ openstack endpoint create esi-leap --region RegionOne public http://localhost:7777
+    $ openstack endpoint create esi-leap --region RegionOne public http://<YOUR_IP>:7777
 ```
 
 
 ### Run the Services
 
 Start by instantiating the database:
 
@@ -164,14 +171,34 @@
 
 
 ```
     $ sudo esi-leap-manager
     $ sudo esi-leap-api
 ```
 
+### Installation using Containerization
+
+By encapsulating the ESI Leap into a container, all the necessary dependencies, configurations and services are bundled into a single package.
+
+Please make sure to follow the instructions in the [Configuration](#configuration) section to generate the esi-leap.conf file.
+
+Make sure to follow the instructions in the [Create Openstack Service](#create-the-openstack-service) to create the OpenStack service and endpoint. 
+
+After that build the container image using the podman build command, as Containerfile is located in the current directory. The syntax is as follows:
+
+```
+    $ podman build -t <image-name> -f Containerfile . 
+```
+
+Once the container image is built, you can run it using the podman run command. The syntax is as follows:
+
+```
+    $ podman run --name <container-name> -p <host-port>:<container-port> -d -v <path-to-esi-leap.conf-file>:/etc/esi-leap <image-name>
+```
+
 
 ### Using Dummy Nodes
 
 If you wish to use dummy nodes instead of Ironic nodes, simply specify the `dummy_node_dir`
 as specified above. Once you do so, add dummy nodes as follows:
 
 ```
```

### Comparing `esi-leap-0.2.6/esi_leap.egg-info/PKG-INFO` & `esi-leap-0.2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-leap
-Version: 0.2.6
+Version: 0.2.7
 Summary: ESI provider
 Home-page: UNKNOWN
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -24,19 +24,21 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # esi-leap
 
-esi-leap is an OpenStack service for acting as a FLOCX provider to communicate with a FLOCX
-marketplace. It is intended to work on top of the
-[esi-common library](https://github.com/CCI-MOC/esi-common), which supports an OpenStack
-install that simulates Ironic multi-tenancy through the use of `project_owner_id` and
-`project_id` property attributes.
+esi-leap is an OpenStack service for leasing baremetal nodes, designed to run
+on top of [multi-tenant
+Ironic](https://docs.openstack.org/ironic/latest/admin/node-multitenancy.html).
+It consists of an API that provides endpoints for leasing operations and a
+manager service that updates the status of leases and offers as required. See
+the [documentation](https://esi.readthedocs.io/en/latest/index.html) for
+more info on ESI.
 
 
 ### Installation
 
 To install as a package:
  - `pip install esi-leap`
 
@@ -53,50 +55,54 @@
 
 esi-leap has a command line client which can be found here:
 https://github.com/CCI-MOC/python-esileapclient
 
 
 ### Create the esi-leap Database
 
-The esi-leap service requires a database to store its information. To set this up using
-the MySQL database used by other OpenStack services, run the following, replacing
-\<PASSWORD\> with a suitable password and \<DATABASE\_IP\> with the IP address of your
-MySQL database (if you're not sure, use localhost or 127.0.0.1).
+The esi-leap service requires a database to store its information. To set this
+up using the MySQL database used by other OpenStack services, run the following
+commands, replacing \<PASSWORD\> with a suitable password and \<DATABASE\_IP\>
+with the IP address of your MySQL database (if you're not sure, use localhost
+or 127.0.0.1).
 
 ```
     $ mysql -u root -p
     mysql> CREATE USER 'esi_leap'@'<DATABASE_IP>' IDENTIFIED BY '<PASSWORD>';
+    mysql> CREATE USER 'esi_leap'@'%' IDENTIFIED BY '<PASSWORD>';
     mysql> CREATE DATABASE esi_leap CHARACTER SET utf8;
     mysql> GRANT ALL PRIVILEGES ON esi_leap.* TO 'esi_leap'@'<DATABASE_IP>';
+    mysql> GRANT ALL PRIVILEGES ON esi_leap.* TO 'esi_leap'@'%';
     mysql> FLUSH PRIVILEGES;
 ```
 
 If you use this method, the resulting database connection string should be:
 
 ```
     mysql+pymysql://esi_leap:PASSWORD@DATABASE_IP/esi_leap
 ```
 
 
 ### Configuration
 
-Run the following to generate the configuration file and copy it to the right place:
+Run the following commands to generate the configuration file and copy it to
+the right place:
 
 ```
     $ tox -egenconfig
     $ sudo mkdir /etc/esi-leap
     $ sudo cp etc/esi-leap/esi-leap.conf.sample /etc/esi-leap/esi-leap.conf
 ```
 
-Edit `/etc/esi-leap/esi-leap.conf` with the proper values. Some useful values include:
+Edit `/etc/esi-leap/esi-leap.conf` with the proper values. (see sample config
+template below):
 
 ```
 [DEFAULT]
 
-debug=True
 log_dir=/var/log/esi-leap
 transport_url=<transport URL for messaging>
 
 [database]
 connection=<db connection string>
 
 # End-user authentication configuration
@@ -111,29 +117,28 @@
 project_domain_name=Default
 
 # esi-leap internal authentication configuration
 [keystone]
 api_endpoint=<admin Keystone endpoint>
 auth_type=password
 auth_url=<keystone auth URL>
-username=admin
+username=esi-leap
 password=<password>
 user_domain_name=Default
-project_name=admin
+project_name=service
 project_domain_name=Default
 
 [oslo_concurrency]
 lock_path=<lock dir>
 
 [oslo_messaging_notifications]
 driver=messagingv2
 transport_url=<transport URL for messaging>
 
 [ironic]                              # ONLY NECESSARY IF USING IRONIC NODES
-
 auth_type = password
 api_endpoint = <ironic API endpoint>
 auth_url = <keystone auth URL>
 project_name = service
 project_domain_name = Default
 user_domain_name = Default
 username = ironic
@@ -143,16 +148,18 @@
 dummy_node_dir=/tmp/nodes
 ```
 
 
 ### Create the OpenStack Service
 
 ```
+    $ openstack user create --domain default --password-prompt esi-leap
+    $ openstack role add --project service --user esi-leap admin
     $ openstack service create --name esi-leap lease
-    $ openstack endpoint create esi-leap --region RegionOne public http://localhost:7777
+    $ openstack endpoint create esi-leap --region RegionOne public http://<YOUR_IP>:7777
 ```
 
 
 ### Run the Services
 
 Start by instantiating the database:
 
@@ -164,14 +171,34 @@
 
 
 ```
     $ sudo esi-leap-manager
     $ sudo esi-leap-api
 ```
 
+### Installation using Containerization
+
+By encapsulating the ESI Leap into a container, all the necessary dependencies, configurations and services are bundled into a single package.
+
+Please make sure to follow the instructions in the [Configuration](#configuration) section to generate the esi-leap.conf file.
+
+Make sure to follow the instructions in the [Create Openstack Service](#create-the-openstack-service) to create the OpenStack service and endpoint. 
+
+After that build the container image using the podman build command, as Containerfile is located in the current directory. The syntax is as follows:
+
+```
+    $ podman build -t <image-name> -f Containerfile . 
+```
+
+Once the container image is built, you can run it using the podman run command. The syntax is as follows:
+
+```
+    $ podman run --name <container-name> -p <host-port>:<container-port> -d -v <path-to-esi-leap.conf-file>:/etc/esi-leap <image-name>
+```
+
 
 ### Using Dummy Nodes
 
 If you wish to use dummy nodes instead of Ironic nodes, simply specify the `dummy_node_dir`
 as specified above. Once you do so, add dummy nodes as follows:
 
 ```
```

### Comparing `esi-leap-0.2.6/esi_leap.egg-info/SOURCES.txt` & `esi-leap-0.2.7/esi_leap.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .stestr.conf
 AUTHORS
 ChangeLog
+Containerfile
 LICENSE
 README.md
 babel.cfg
 requirements.txt
+run_services.sh
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
 .github/workflows/tests.yml
 docs/esi-leap-api-ref.md
 docs/esi-leap-policy.md
@@ -44,24 +46,27 @@
 esi_leap/cmd/manager.py
 esi_leap/common/__init__.py
 esi_leap/common/constants.py
 esi_leap/common/exception.py
 esi_leap/common/i18n.py
 esi_leap/common/ironic.py
 esi_leap/common/keystone.py
+esi_leap/common/notification_utils.py
 esi_leap/common/policy.py
+esi_leap/common/rpc.py
 esi_leap/common/service.py
 esi_leap/common/statuses.py
 esi_leap/common/utils.py
 esi_leap/conf/__init__.py
 esi_leap/conf/api.py
 esi_leap/conf/dummy_node.py
 esi_leap/conf/ironic.py
 esi_leap/conf/keystone.py
 esi_leap/conf/netconf.py
+esi_leap/conf/notification.py
 esi_leap/conf/opts.py
 esi_leap/conf/pecan.py
 esi_leap/db/__init__.py
 esi_leap/db/api.py
 esi_leap/db/base.py
 esi_leap/db/migration.py
 esi_leap/db/sqlalchemy/__init__.py
@@ -78,18 +83,20 @@
 esi_leap/manager/rpcapi.py
 esi_leap/manager/service.py
 esi_leap/manager/utils.py
 esi_leap/objects/__init__.py
 esi_leap/objects/base.py
 esi_leap/objects/fields.py
 esi_leap/objects/lease.py
+esi_leap/objects/notification.py
 esi_leap/objects/offer.py
 esi_leap/resource_objects/__init__.py
 esi_leap/resource_objects/base.py
 esi_leap/resource_objects/dummy_node.py
+esi_leap/resource_objects/error.py
 esi_leap/resource_objects/ironic_node.py
 esi_leap/resource_objects/test_node.py
 esi_leap/tests/__init__.py
 esi_leap/tests/base.py
 esi_leap/tests/api/__init__.py
 esi_leap/tests/api/base.py
 esi_leap/tests/api/controllers/__init__.py
@@ -98,24 +105,27 @@
 esi_leap/tests/api/controllers/v1/test_lease.py
 esi_leap/tests/api/controllers/v1/test_node.py
 esi_leap/tests/api/controllers/v1/test_offer.py
 esi_leap/tests/api/controllers/v1/test_utils.py
 esi_leap/tests/common/__init__.py
 esi_leap/tests/common/test_ironic.py
 esi_leap/tests/common/test_keystone.py
+esi_leap/tests/common/test_notification_utils.py
 esi_leap/tests/common/test_policy.py
+esi_leap/tests/common/test_rpc.py
 esi_leap/tests/common/test_utils.py
 esi_leap/tests/db/__init__.py
 esi_leap/tests/db/sqlalchemy/__init__.py
 esi_leap/tests/db/sqlalchemy/test_api.py
 esi_leap/tests/manager/__init__.py
 esi_leap/tests/manager/test_service.py
 esi_leap/tests/objects/__init__.py
 esi_leap/tests/objects/test_fields.py
 esi_leap/tests/objects/test_lease.py
+esi_leap/tests/objects/test_notification.py
 esi_leap/tests/objects/test_offer.py
 esi_leap/tests/resource_objects/__init__.py
 esi_leap/tests/resource_objects/test_base.py
 esi_leap/tests/resource_objects/test_dummy_node.py
 esi_leap/tests/resource_objects/test_ironic_node.py
 esi_leap/tests/resource_objects/test_resource_objects.py
 esi_leap/tests/resource_objects/test_test_node.py
```

### Comparing `esi-leap-0.2.6/esi_leap.egg-info/requires.txt` & `esi-leap-0.2.7/esi_leap.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 pbr!=2.1.0,>=2.0.0
 alembic>=1.4.2
 Babel!=2.4.0,>=2.3.4
-eventlet!=0.18.3,!=0.20.1,>=0.18.2
+eventlet>=0.33.3
+importlib-metadata<5.0.0
 iso8601>=0.1.11
 keystoneauth1>=3.4.0
 keystonemiddleware>=4.17.0
 kombu!=4.0.2,>=4.0.0
+openstacksdk<1.3.0
 oslo.concurrency>=3.26.0
 oslo.config>=5.2.0
 oslo.db>=4.27.0
 oslo.i18n>=3.15.3
 oslo.log>=3.36.0
 oslo.messaging>=5.29.0
 oslo.middleware>=3.31.0
 oslo.policy>=1.30.0
 oslo.serialization!=2.19.1,>=2.18.0
 oslo.service!=1.28.1,>=1.24.0
 oslo.upgradecheck>=0.1.0
 oslo.utils>=3.33.0
 oslo.versionedobjects>=1.31.2
+osprofiler>=1.5.0
 netaddr>=0.7.18
 python-ironicclient>=2.3.0
 python-keystoneclient>=3.8.0
 pecan!=1.0.2,!=1.0.3,!=1.0.4,!=1.2,>=1.0.0
 sqlalchemy-migrate>=0.11.0
 requests>=2.18.4
 Routes>=2.3.1
 six>=1.10.0
-SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10
+SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,<2.0,>=1.0.10
 stevedore>=1.20.0
 WebOb>=1.7.1
 WSME>=0.8.0
```

### Comparing `esi-leap-0.2.6/setup.py` & `esi-leap-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/tox.ini` & `esi-leap-0.2.7/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 install_command = pip install -U {opts} {packages}
 setenv = VIRTUAL_ENV={envdir}
          PYTHONDONTWRITEBYTECODE = 1
          LANGUAGE=en_US
          LC_ALL=en_US.UTF-8
          PYTHONWARNINGS=default::DeprecationWarning
          TESTS_DIR=./esi_leap/tests/
+         SQLALCHEMY_SILENCE_UBER_WARNING=1
 deps =
   -r{toxinidir}/requirements.txt
   -r{toxinidir}/test-requirements.txt
 commands = stestr run {posargs}
 
 [testenv:pep8]
 commands = flake8 esi_leap {posargs}
```

### Comparing `esi-leap-0.2.6/ChangeLog` & `esi-leap-0.2.7/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 CHANGES
 =======
 
+0.2.7
+-----
+
+* Enforce openstacksdk<1.3.0
+* Add lease expire notification
+* Add purpose field to lease notification
+* Lease purpose field should be nullable
+* add-purpose-field-to-esi-lease
+* Add notifications for leases
+* Fix various issues with esi-leap Containerfile
+* dockerize-esi-leap
+* Resource object interface refactoring
+* Updated exception handling for resource objects
+* Update README
+* Updated CI, fixed dependency issues
+* Remove python 3.6 from CI and add 3.10
+
 0.2.6
 -----
 
 * This change is related to setting resource value to 'unknown' if a node is not found for the lease
 * Fixed ESI-Leap API WSGI script
 
 0.2.5
```

### Comparing `esi-leap-0.2.6/README.md` & `esi-leap-0.2.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # esi-leap
 
-esi-leap is an OpenStack service for acting as a FLOCX provider to communicate with a FLOCX
-marketplace. It is intended to work on top of the
-[esi-common library](https://github.com/CCI-MOC/esi-common), which supports an OpenStack
-install that simulates Ironic multi-tenancy through the use of `project_owner_id` and
-`project_id` property attributes.
+esi-leap is an OpenStack service for leasing baremetal nodes, designed to run
+on top of [multi-tenant
+Ironic](https://docs.openstack.org/ironic/latest/admin/node-multitenancy.html).
+It consists of an API that provides endpoints for leasing operations and a
+manager service that updates the status of leases and offers as required. See
+the [documentation](https://esi.readthedocs.io/en/latest/index.html) for
+more info on ESI.
 
 
 ### Installation
 
 To install as a package:
  - `pip install esi-leap`
 
@@ -25,50 +27,54 @@
 
 esi-leap has a command line client which can be found here:
 https://github.com/CCI-MOC/python-esileapclient
 
 
 ### Create the esi-leap Database
 
-The esi-leap service requires a database to store its information. To set this up using
-the MySQL database used by other OpenStack services, run the following, replacing
-\<PASSWORD\> with a suitable password and \<DATABASE\_IP\> with the IP address of your
-MySQL database (if you're not sure, use localhost or 127.0.0.1).
+The esi-leap service requires a database to store its information. To set this
+up using the MySQL database used by other OpenStack services, run the following
+commands, replacing \<PASSWORD\> with a suitable password and \<DATABASE\_IP\>
+with the IP address of your MySQL database (if you're not sure, use localhost
+or 127.0.0.1).
 
 ```
     $ mysql -u root -p
     mysql> CREATE USER 'esi_leap'@'<DATABASE_IP>' IDENTIFIED BY '<PASSWORD>';
+    mysql> CREATE USER 'esi_leap'@'%' IDENTIFIED BY '<PASSWORD>';
     mysql> CREATE DATABASE esi_leap CHARACTER SET utf8;
     mysql> GRANT ALL PRIVILEGES ON esi_leap.* TO 'esi_leap'@'<DATABASE_IP>';
+    mysql> GRANT ALL PRIVILEGES ON esi_leap.* TO 'esi_leap'@'%';
     mysql> FLUSH PRIVILEGES;
 ```
 
 If you use this method, the resulting database connection string should be:
 
 ```
     mysql+pymysql://esi_leap:PASSWORD@DATABASE_IP/esi_leap
 ```
 
 
 ### Configuration
 
-Run the following to generate the configuration file and copy it to the right place:
+Run the following commands to generate the configuration file and copy it to
+the right place:
 
 ```
     $ tox -egenconfig
     $ sudo mkdir /etc/esi-leap
     $ sudo cp etc/esi-leap/esi-leap.conf.sample /etc/esi-leap/esi-leap.conf
 ```
 
-Edit `/etc/esi-leap/esi-leap.conf` with the proper values. Some useful values include:
+Edit `/etc/esi-leap/esi-leap.conf` with the proper values. (see sample config
+template below):
 
 ```
 [DEFAULT]
 
-debug=True
 log_dir=/var/log/esi-leap
 transport_url=<transport URL for messaging>
 
 [database]
 connection=<db connection string>
 
 # End-user authentication configuration
@@ -83,29 +89,28 @@
 project_domain_name=Default
 
 # esi-leap internal authentication configuration
 [keystone]
 api_endpoint=<admin Keystone endpoint>
 auth_type=password
 auth_url=<keystone auth URL>
-username=admin
+username=esi-leap
 password=<password>
 user_domain_name=Default
-project_name=admin
+project_name=service
 project_domain_name=Default
 
 [oslo_concurrency]
 lock_path=<lock dir>
 
 [oslo_messaging_notifications]
 driver=messagingv2
 transport_url=<transport URL for messaging>
 
 [ironic]                              # ONLY NECESSARY IF USING IRONIC NODES
-
 auth_type = password
 api_endpoint = <ironic API endpoint>
 auth_url = <keystone auth URL>
 project_name = service
 project_domain_name = Default
 user_domain_name = Default
 username = ironic
@@ -115,16 +120,18 @@
 dummy_node_dir=/tmp/nodes
 ```
 
 
 ### Create the OpenStack Service
 
 ```
+    $ openstack user create --domain default --password-prompt esi-leap
+    $ openstack role add --project service --user esi-leap admin
     $ openstack service create --name esi-leap lease
-    $ openstack endpoint create esi-leap --region RegionOne public http://localhost:7777
+    $ openstack endpoint create esi-leap --region RegionOne public http://<YOUR_IP>:7777
 ```
 
 
 ### Run the Services
 
 Start by instantiating the database:
 
@@ -136,14 +143,34 @@
 
 
 ```
     $ sudo esi-leap-manager
     $ sudo esi-leap-api
 ```
 
+### Installation using Containerization
+
+By encapsulating the ESI Leap into a container, all the necessary dependencies, configurations and services are bundled into a single package.
+
+Please make sure to follow the instructions in the [Configuration](#configuration) section to generate the esi-leap.conf file.
+
+Make sure to follow the instructions in the [Create Openstack Service](#create-the-openstack-service) to create the OpenStack service and endpoint. 
+
+After that build the container image using the podman build command, as Containerfile is located in the current directory. The syntax is as follows:
+
+```
+    $ podman build -t <image-name> -f Containerfile . 
+```
+
+Once the container image is built, you can run it using the podman run command. The syntax is as follows:
+
+```
+    $ podman run --name <container-name> -p <host-port>:<container-port> -d -v <path-to-esi-leap.conf-file>:/etc/esi-leap <image-name>
+```
+
 
 ### Using Dummy Nodes
 
 If you wish to use dummy nodes instead of Ironic nodes, simply specify the `dummy_node_dir`
 as specified above. Once you do so, add dummy nodes as follows:
 
 ```
```

### Comparing `esi-leap-0.2.6/.github/workflows/tests.yml` & `esi-leap-0.2.7/.github/workflows/tests.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 name: esi-leap
 
 on: [push, pull_request]
 
 jobs:
   build:
 
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8", "3.9"]
+        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Lint
```

### Comparing `esi-leap-0.2.6/test-requirements.txt` & `esi-leap-0.2.7/test-requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 doc8>=0.6.0 # Apache-2.0
 fixtures>=3.0.0 # Apache-2.0/BSD
 mock>=2.0.0 # BSD
 Babel!=2.4.0,>=2.3.4 # BSD
 PyMySQL>=0.7.6 # MIT License
 iso8601>=0.1.11 # MIT
 oslotest>=3.2.0 # Apache-2.0
+osprofiler>=1.5.0 # Apache-2.0
 stestr>=1.0.0 # Apache-2.0
 psycopg2>=2.6.2 # LGPL/ZPL
 testtools>=2.2.0 # MIT
 testresources>=2.0.0 # Apache-2.0/BSD
 testscenarios>=0.4 # Apache-2.0/BSD
 WebTest>=2.0.27 # MIT
 bashate>=0.5.1 # Apache-2.0
```

### Comparing `esi-leap-0.2.6/LICENSE` & `esi-leap-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/setup.cfg` & `esi-leap-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/docs/esi-leap-requirements.md` & `esi-leap-0.2.7/docs/esi-leap-requirements.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/docs/esi-leap-reporting.md` & `esi-leap-0.2.7/docs/esi-leap-reporting.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/docs/esi-leap-policy.md` & `esi-leap-0.2.7/docs/esi-leap-policy.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/docs/esi-leap-api-ref.md` & `esi-leap-0.2.7/docs/esi-leap-api-ref.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/requirements.txt` & `esi-leap-0.2.7/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # The order of packages is significant, because pip processes them in the order
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
 pbr!=2.1.0,>=2.0.0 # Apache-2.0
 
 alembic>=1.4.2 # MIT
 Babel!=2.4.0,>=2.3.4 # BSD
-eventlet!=0.18.3,!=0.20.1,>=0.18.2 # MIT
+eventlet>=0.33.3 # MIT
+importlib-metadata<5.0.0; python_version<'3.8' # Apache-2.0
 iso8601>=0.1.11 # MIT
 keystoneauth1>=3.4.0 # Apache-2.0
 keystonemiddleware>=4.17.0 # Apache-2.0
 kombu!=4.0.2,>=4.0.0 # BSD
+openstacksdk<1.3.0
 oslo.concurrency>=3.26.0 # Apache-2.0
 oslo.config>=5.2.0 # Apache-2.0
 oslo.db>=4.27.0 # Apache-2.0
 oslo.i18n>=3.15.3 # Apache-2.0
 oslo.log>=3.36.0 # Apache-2.0
 oslo.messaging>=5.29.0 # Apache-2.0
 oslo.middleware>=3.31.0 # Apache-2.0
 oslo.policy>=1.30.0 # Apache-2.0
 oslo.serialization!=2.19.1,>=2.18.0 # Apache-2.0
 oslo.service!=1.28.1,>=1.24.0 # Apache-2.0
 oslo.upgradecheck>=0.1.0 # Apache-2.0
 oslo.utils>=3.33.0 # Apache-2.0
 oslo.versionedobjects>=1.31.2 # Apache-2.0
+osprofiler>=1.5.0 # Apache-2.0
 netaddr>=0.7.18 # BSD
 python-ironicclient>=2.3.0 # Apache-2.0
 python-keystoneclient>=3.8.0 # Apache-2.0
 pecan!=1.0.2,!=1.0.3,!=1.0.4,!=1.2,>=1.0.0 # BSD
 sqlalchemy-migrate>=0.11.0 # Apache-2.0
 requests>=2.18.4 # Apache-2.0
 Routes>=2.3.1 # MIT
 six>=1.10.0 # MIT
-SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10 # MIT
+SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10, <2.0 # MIT
 stevedore>=1.20.0 # Apache-2.0
 WebOb>=1.7.1 # MIT
 WSME>=0.8.0 # MIT
```

### Comparing `esi-leap-0.2.6/esi_leap/resource_objects/__init__.py` & `esi-leap-0.2.7/esi_leap/resource_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/resource_objects/test_node.py` & `esi-leap-0.2.7/esi_leap/resource_objects/test_node.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,33 +17,39 @@
 
     resource_type = 'test_node'
 
     def __init__(self, uuid, project_id='12345'):
         self._uuid = uuid
         self._project_id = project_id
 
-    def get_resource_uuid(self):
+    def get_uuid(self):
         return self._uuid
 
-    def get_resource_name(self, resource_list=None):
+    def get_name(self, resource_list=None):
         return 'test-node-%s' % self._uuid
 
+    def get_resource_class(self, resource_list=None):
+        return 'fake'
+
+    def get_config(self):
+        return {}
+
+    def get_owner_project_id(self):
+        return self._project_id
+
     def get_lease_uuid(self):
         return '12345'
 
-    def get_project_id(self):
+    def get_lessee_project_id(self):
         return self._project_id
 
-    def get_node_config(self):
-        return {}
+    def get_node_power_state(self):
+        return 'Off'
 
-    def get_resource_class(self, resource_list=None):
-        return 'fake'
+    def get_node_provision_state(self):
+        return 'available'
 
     def set_lease(self, lease):
         return
 
-    def expire_lease(self, lease):
+    def remove_lease(self, lease):
         return
-
-    def resource_admin_project_id(self):
-        return self._project_id
```

### Comparing `esi-leap-0.2.6/esi_leap/api/app.py` & `esi-leap-0.2.7/esi_leap/api/app.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/api/controllers/base.py` & `esi-leap-0.2.7/esi_leap/api/controllers/base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/api/controllers/types.py` & `esi-leap-0.2.7/esi_leap/api/controllers/types.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/api/controllers/v1/node.py` & `esi-leap-0.2.7/esi_leap/api/controllers/v1/node.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/api/controllers/v1/utils.py` & `esi-leap-0.2.7/esi_leap/api/controllers/v1/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,44 +17,42 @@
 from esi_leap.common import keystone
 from esi_leap.common import policy
 from esi_leap.objects import lease as lease_obj
 from esi_leap.objects import offer as offer_obj
 
 
 def check_resource_admin(cdict, resource, project_id):
-    if project_id != resource.resource_admin_project_id():
+    if project_id != resource.get_owner_project_id():
         resource_policy_authorize('esi_leap:offer:offer_admin',
                                   cdict, cdict,
                                   resource.resource_type,
-                                  resource.get_resource_uuid())
+                                  resource.get_uuid())
 
 
 def check_resource_lease_admin(cdict, resource, project_id,
                                start_time, end_time):
     # check to see if project is current lessee
-    if project_id == resource.get_project_id():
+    if project_id == resource.get_lessee_project_id():
         parent_lease_uuid = resource.get_lease_uuid()
         if parent_lease_uuid is not None:
             parent_lease = lease_obj.Lease.get(parent_lease_uuid)
 
             # don't allow sub-sub-leases
             if parent_lease.parent_lease_uuid is None:
                 # check if offer is within start and end time bounds
                 if ((start_time >= parent_lease.start_time) and
                         (end_time <= parent_lease.end_time)):
                     return parent_lease_uuid
                 else:
                     raise exception.ResourceNoPermissionTime(
                         resource_type=resource.resource_type,
-                        resource_uuid=resource.get_resource_uuid(),
+                        resource_uuid=resource.get_uuid(),
                         start_time=start_time,
                         end_time=end_time)
 
-    return
-
 
 def get_offer(uuid_or_name, status_filters=[]):
     if uuidutils.is_uuid_like(uuid_or_name):
         o = offer_obj.Offer.get(uuid_or_name)
         if not status_filters or o.status in status_filters:
             return o
         else:
@@ -143,30 +141,29 @@
     if offer.lessee_id not in keystone.get_parent_project_id_tree(project_id):
         resource_policy_authorize(
             'esi_leap:offer:offer_admin',
             cdict, cdict, 'offer', offer.uuid)
 
 
 def offer_get_dict_with_added_info(offer, project_list=None, node_list=None):
-    availabilities = offer.get_availabilities()
     resource = offer.resource_object()
 
     o = offer.to_dict()
-    o['availabilities'] = availabilities
+    o['availabilities'] = offer.get_availabilities()
     o['project'] = keystone.get_project_name(offer.project_id, project_list)
     o['lessee'] = keystone.get_project_name(offer.lessee_id, project_list)
-    o['resource'] = resource.get_resource_name(node_list)
+    o['resource'] = resource.get_name(node_list)
     o['resource_class'] = resource.get_resource_class(node_list)
     return o
 
 
 def lease_get_dict_with_added_info(lease, project_list=None, node_list=None):
     resource = lease.resource_object()
 
     lease_dict = lease.to_dict()
     lease_dict['project'] = keystone.get_project_name(lease.project_id,
                                                       project_list)
     lease_dict['owner'] = keystone.get_project_name(lease.owner_id,
                                                     project_list)
-    lease_dict['resource'] = resource.get_resource_name(node_list)
+    lease_dict['resource'] = resource.get_name(node_list)
     lease_dict['resource_class'] = resource.get_resource_class(node_list)
     return lease_dict
```

### Comparing `esi-leap-0.2.6/esi_leap/api/controllers/v1/lease.py` & `esi-leap-0.2.7/esi_leap/api/controllers/v1/lease.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     resource = wsme.wsattr(wtypes.text, readonly=True)
     start_time = wsme.wsattr(datetime.datetime)
     fulfill_time = wsme.wsattr(datetime.datetime, readonly=True)
     expire_time = wsme.wsattr(datetime.datetime, readonly=True)
     end_time = wsme.wsattr(datetime.datetime)
     status = wsme.wsattr(wtypes.text, readonly=True)
     properties = {wtypes.text: types.jsontype}
+    purpose = wsme.wsattr(wtypes.text)
     offer_uuid = wsme.wsattr(wtypes.text, readonly=True)
     parent_lease_uuid = wsme.wsattr(wtypes.text, readonly=True)
 
     def __init__(self, **kwargs):
         self.fields = lease_obj.Lease.fields
         for field in self.fields:
             setattr(self, field, kwargs.get(field, wtypes.Unset))
@@ -100,15 +101,15 @@
             owner_id = keystone.get_project_uuid_from_ident(owner_id)
 
         if resource_uuid is not None:
             if resource_type is None:
                 resource_type = CONF.api.default_resource_type
 
             resource = get_resource_object(resource_type, resource_uuid)
-            resource_uuid = resource.get_resource_uuid()
+            resource_uuid = resource.get_uuid()
 
         filters = LeasesController._lease_get_all_authorize_filters(
             cdict, project_id=project_id, owner_id=owner_id,
             start_time=start_time, end_time=end_time,
             status=status, offer_uuid=offer_uuid, view=view,
             resource_type=resource_type, resource_uuid=resource_uuid)
 
@@ -149,15 +150,15 @@
         lease_dict = new_lease.to_dict()
         lease_dict['owner_id'] = request.project_id
         lease_dict['uuid'] = uuidutils.generate_uuid()
         if 'resource_type' not in lease_dict:
             lease_dict['resource_type'] = CONF.api.default_resource_type
         resource = get_resource_object(lease_dict['resource_type'],
                                        lease_dict['resource_uuid'])
-        lease_dict['resource_uuid'] = resource.get_resource_uuid()
+        lease_dict['resource_uuid'] = resource.get_uuid()
 
         if 'project_id' in lease_dict:
             lease_dict['project_id'] = keystone.get_project_uuid_from_ident(
                 lease_dict['project_id'])
 
         if 'start_time' not in lease_dict:
             lease_dict['start_time'] = datetime.datetime.now()
@@ -186,15 +187,15 @@
     def delete(self, lease_id):
         request = pecan.request.context
 
         lease = utils.check_lease_policy_and_retrieve(
             request, 'esi_leap:lease:get', lease_id,
             statuses.LEASE_CAN_DELETE)
 
-        lease.cancel()
+        lease.cancel(request)
 
     @staticmethod
     def _lease_get_all_authorize_filters(cdict,
                                          start_time=None, end_time=None,
                                          status=None, offer_uuid=None,
                                          project_id=None, view=None,
                                          owner_id=None, resource_type=None,
```

### Comparing `esi-leap-0.2.6/esi_leap/api/controllers/v1/root.py` & `esi-leap-0.2.7/esi_leap/api/controllers/v1/root.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/api/controllers/v1/offer.py` & `esi-leap-0.2.7/esi_leap/api/controllers/v1/offer.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         if project_id is not None:
             project_id = keystone.get_project_uuid_from_ident(project_id)
 
         if resource_uuid is not None:
             if resource_type is None:
                 resource_type = CONF.api.default_resource_type
             resource = get_resource_object(resource_type, resource_uuid)
-            resource_uuid = resource.get_resource_uuid()
+            resource_uuid = resource.get_uuid()
 
         # either both are defined or both are None
         if bool(start_time) != bool(end_time):
             raise exception.InvalidTimeAPICommand(resource='an offer',
                                                   start_time=str(start_time),
                                                   end_time=str(end_time))
         if (start_time or end_time) and (end_time <= start_time):
@@ -200,15 +200,15 @@
         offer_dict = new_offer.to_dict()
         offer_dict['project_id'] = request.project_id
         offer_dict['uuid'] = uuidutils.generate_uuid()
         if 'resource_type' not in offer_dict:
             offer_dict['resource_type'] = CONF.api.default_resource_type
         resource = get_resource_object(offer_dict['resource_type'],
                                        offer_dict['resource_uuid'])
-        offer_dict['resource_uuid'] = resource.get_resource_uuid()
+        offer_dict['resource_uuid'] = resource.get_uuid()
 
         if 'lessee_id' in offer_dict:
             offer_dict['lessee_id'] = keystone.get_project_uuid_from_ident(
                 offer_dict['lessee_id'])
 
         if 'start_time' not in offer_dict:
             offer_dict['start_time'] = datetime.datetime.now()
```

### Comparing `esi-leap-0.2.6/esi_leap/api/controllers/root.py` & `esi-leap-0.2.7/esi_leap/api/controllers/root.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/api/service.py` & `esi-leap-0.2.7/esi_leap/api/service.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/api/wsgi.py` & `esi-leap-0.2.7/esi_leap/api/wsgi.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/objects/base.py` & `esi-leap-0.2.7/esi_leap/objects/base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/objects/lease.py` & `esi-leap-0.2.7/esi_leap/objects/lease.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,40 +9,122 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import datetime
 
 from esi_leap.common import exception
+from esi_leap.common import notification_utils as notify
 from esi_leap.common import statuses
 from esi_leap.common import utils
 from esi_leap.db import api as dbapi
 from esi_leap.objects import base
 from esi_leap.objects import fields
+from esi_leap.objects import notification
 from esi_leap.objects import offer as offer_obj
 from esi_leap.resource_objects import get_resource_object
 
 from oslo_config import cfg
 from oslo_log import log as logging
 from oslo_versionedobjects import base as versioned_objects_base
 
 CONF = cfg.CONF
 LOG = logging.getLogger(__name__)
 
 
 @versioned_objects_base.VersionedObjectRegistry.register
+class LeaseCRUDNotification(notification.NotificationBase):
+    """Notification emitted when a lease is created or deleted."""
+
+    fields = {
+        'payload': fields.ObjectField('LeaseCRUDPayload')
+    }
+
+
+@versioned_objects_base.VersionedObjectRegistry.register
+class LeaseCRUDPayload(notification.NotificationPayloadBase):
+    """Payload schema for when a lease is created or deleted."""
+    # Version 1.0: Initial version
+    VERSION = '1.0'
+
+    SCHEMA = {
+        'id': ('lease', 'id'),
+        'name': ('lease', 'name'),
+        'uuid': ('lease', 'uuid'),
+        'project_id': ('lease', 'project_id'),
+        'owner_id': ('lease', 'owner_id'),
+        'resource_type': ('lease', 'resource_type'),
+        'resource_uuid': ('lease', 'resource_uuid'),
+        'start_time': ('lease', 'start_time'),
+        'end_time': ('lease', 'end_time'),
+        'fulfill_time': ('lease', 'fulfill_time'),
+        'expire_time': ('lease', 'expire_time'),
+        'status': ('lease', 'status'),
+        'properties': ('lease', 'properties'),
+        'purpose': ('lease', 'purpose'),
+        'offer_uuid': ('lease', 'offer_uuid'),
+        'parent_lease_uuid': ('lease', 'parent_lease_uuid'),
+        'node_name': ('node', 'node_name'),
+        'node_uuid': ('node', '_uuid'),
+        'node_provision_state': ('node', 'node_provision_state'),
+        'node_power_state': ('node', 'node_power_state'),
+        'node_properties': ('node', 'node_properties'),
+    }
+
+    fields = {
+        'id': fields.IntegerField(),
+        'name': fields.StringField(nullable=True),
+        'uuid': fields.UUIDField(),
+        'project_id': fields.StringField(),
+        'owner_id': fields.StringField(),
+        'purpose': fields.StringField(nullable=True),
+        'resource_type': fields.StringField(),
+        'resource_uuid': fields.StringField(),
+        'start_time': fields.DateTimeField(nullable=True),
+        'end_time': fields.DateTimeField(nullable=True),
+        'fulfill_time': fields.DateTimeField(nullable=True),
+        'expire_time': fields.DateTimeField(nullable=True),
+        'status': fields.StringField(),
+        'properties': fields.FlexibleDictField(nullable=True),
+        'offer_uuid': fields.UUIDField(nullable=True),
+        'parent_lease_uuid': fields.UUIDField(nullable=True),
+        'node_name': fields.StringField(nullable=True),
+        'node_uuid': fields.UUIDField(),
+        'node_provision_state': fields.StringField(),
+        'node_power_state': fields.StringField(),
+        'node_properties': fields.FlexibleDictField(nullable=True),
+    }
+
+    def __init__(self, lease, node):
+        super(LeaseCRUDPayload, self).__init__()
+
+        setattr(node, 'node_name', node.get_name())
+        setattr(node, 'node_provision_state', node.get_node_provision_state())
+        setattr(node, 'node_power_state', node.get_node_power_state())
+        setattr(node, 'node_properties', node.get_config())
+
+        self.populate_schema(lease=lease, node=node)
+
+
+CRUD_NOTIFY_OBJ = {
+    'lease': (LeaseCRUDNotification, LeaseCRUDPayload),
+}
+
+
+@versioned_objects_base.VersionedObjectRegistry.register
 class Lease(base.ESILEAPObject):
     dbapi = dbapi.get_instance()
 
     fields = {
         'id': fields.IntegerField(),
         'name': fields.StringField(nullable=True),
         'uuid': fields.UUIDField(),
         'project_id': fields.StringField(),
         'owner_id': fields.StringField(),
+        'purpose': fields.StringField(nullable=True),
         'resource_type': fields.StringField(),
         'resource_uuid': fields.StringField(),
         'start_time': fields.DateTimeField(nullable=True),
         'end_time': fields.DateTimeField(nullable=True),
         'fulfill_time': fields.DateTimeField(nullable=True),
         'expire_time': fields.DateTimeField(nullable=True),
         'status': fields.StringField(),
@@ -102,15 +184,15 @@
                                          updates['resource_uuid'])
                 ro.verify_availability(updates['start_time'],
                                        updates['end_time'])
 
             db_lease = self.dbapi.lease_create(updates)
             self._from_db_object(context, self, db_lease)
 
-    def cancel(self):
+    def cancel(self, context=None):
         leases = Lease.get_all(
             {'parent_lease_uuid': self.uuid,
              'status': statuses.LEASE_CAN_DELETE},
             None)
         for lease in leases:
             lease.cancel()
         offers = offer_obj.Offer.get_all(
@@ -122,28 +204,24 @@
 
         with utils.lock(utils.get_resource_lock_name(self.resource_type,
                                                      self.resource_uuid),
                         external=True):
             LOG.info('Deleting lease %s', self.uuid)
             try:
                 resource = self.resource_object()
-                if resource.get_lease_uuid() == self.uuid:
-                    resource.expire_lease(self)
-                    if self.parent_lease_uuid is not None:
-                        parent_lease = Lease.get(self.parent_lease_uuid)
-                        resource.set_lease(parent_lease)
-
+                self.deactivate(context, resource)
                 self.status = statuses.DELETED
                 self.expire_time = datetime.datetime.now()
+
             except Exception as e:
                 LOG.info('Error canceling lease: %s: %s' %
                          (type(e).__name__, e))
                 LOG.info('Setting lease status to WAIT')
                 self.status = statuses.WAIT_CANCEL
-            self.save(None)
+            self.save(context)
 
     def destroy(self):
         self.dbapi.lease_destroy(self.uuid)
         self.obj_reset_changes()
 
     def save(self, context=None):
         updates = self.obj_get_changes()
@@ -154,19 +232,33 @@
     def fulfill(self, context=None):
         with utils.lock(utils.get_resource_lock_name(self.resource_type,
                                                      self.resource_uuid),
                         external=True):
             LOG.info('Fulfilling lease %s', self.uuid)
             try:
                 resource = self.resource_object()
-                resource.set_lease(self)
+                notify.emit_start_notification(context, self,
+                                               'fulfill',
+                                               CRUD_NOTIFY_OBJ,
+                                               node=resource)
+                with notify.handle_error_notification(context,
+                                                      self,
+                                                      'fulfill',
+                                                      CRUD_NOTIFY_OBJ,
+                                                      node=resource):
+                    resource.set_lease(self)
+
+                notify.emit_end_notification(context, self,
+                                             'fulfill',
+                                             CRUD_NOTIFY_OBJ,
+                                             node=resource)
 
-                # activate lease
                 self.status = statuses.ACTIVE
                 self.fulfill_time = datetime.datetime.now()
+
             except Exception as e:
                 LOG.info('Error fulfilling lease: %s: %s' %
                          (type(e).__name__, e))
                 LOG.info('Setting lease status to WAIT')
                 self.status = statuses.WAIT_FULFILL
             self.save(context)
 
@@ -185,29 +277,47 @@
             offer.expire(context)
 
         with utils.lock(utils.get_resource_lock_name(self.resource_type,
                                                      self.resource_uuid),
                         external=True):
             LOG.info('Expiring lease %s', self.uuid)
             try:
-                resource = self.resource_object()
-                if resource.get_lease_uuid() == self.uuid:
-                    resource.expire_lease(self)
-                    if self.parent_lease_uuid is not None:
-                        parent_lease = Lease.get(self.parent_lease_uuid)
-                        resource.set_lease(parent_lease)
                 # expire lease
+                resource = self.resource_object()
+                self.deactivate(context, resource)
                 self.status = statuses.EXPIRED
                 self.expire_time = datetime.datetime.now()
+
             except Exception as e:
                 LOG.info('Error expiring lease: %s: %s' %
                          (type(e).__name__, e))
                 LOG.info('Setting lease status to WAIT')
                 self.status = statuses.WAIT_EXPIRE
             self.save(context)
 
     def resource_object(self):
         return get_resource_object(self.resource_type, self.resource_uuid)
 
     def verify_child_availability(self, start_time, end_time):
         return self.dbapi.lease_verify_child_availability(
             self, start_time, end_time)
+
+    def deactivate(self, context, resource):
+        notify.emit_start_notification(context, self,
+                                       'delete', CRUD_NOTIFY_OBJ,
+                                       node=resource)
+
+        with notify.handle_error_notification(context,
+                                              self,
+                                              'delete',
+                                              CRUD_NOTIFY_OBJ,
+                                              node=resource):
+            if resource.get_lease_uuid() == self.uuid:
+                resource.remove_lease(self)
+
+                if self.parent_lease_uuid is not None:
+                    parent_lease = Lease.get(self.parent_lease_uuid)
+                    resource.set_lease(parent_lease)
+
+        notify.emit_end_notification(context, self,
+                                     'delete', CRUD_NOTIFY_OBJ,
+                                     node=resource)
```

### Comparing `esi-leap-0.2.6/esi_leap/objects/offer.py` & `esi-leap-0.2.7/esi_leap/objects/offer.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/manager/utils.py` & `esi-leap-0.2.7/esi_leap/manager/utils.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/manager/service.py` & `esi-leap-0.2.7/esi_leap/manager/service.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/manager/rpcapi.py` & `esi-leap-0.2.7/esi_leap/manager/rpcapi.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/common/exception.py` & `esi-leap-0.2.7/esi_leap/common/exception.py`

 * *Files 11% similar despite different names*

```diff
@@ -140,7 +140,28 @@
                 'Got %(a_start)s, %(a_end)s.')
 
 
 class InvalidTimeRange(ESILeapException):
     msg_fmt = _('Attempted to create %(resource)s resource with an invalid '
                 'Start Time and End Time. Start Time must be strictly less '
                 'than End Time. Got %(start_time)s, %(end_time)s.')
+
+
+class NodeNotFound(ESILeapException):
+    msg_fmt = _('Encountered an error fetching info for node %(uuid)s '
+                '(%(resource_type)s): %(err)s')
+
+
+class NotificationPayloadError(ESILeapException):
+    _msg_fmt = _("Payload not populated when trying to send notification "
+                 "\"%(class_name)s\"")
+
+
+class NotificationSchemaObjectError(ESILeapException):
+    _msg_fmt = _("Expected object %(obj)s when populating notification payload"
+                 " but got object %(source)s")
+
+
+class NotificationSchemaKeyError(ESILeapException):
+    _msg_fmt = _("Object %(obj)s doesn't have the field \"%(field)s\" "
+                 "required for populating notification schema key "
+                 "\"%(key)s\"")
```

### Comparing `esi-leap-0.2.6/esi_leap/common/utils.py` & `esi-leap-0.2.7/esi_leap/common/utils.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/common/policy.py` & `esi-leap-0.2.7/esi_leap/common/policy.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/common/ironic.py` & `esi-leap-0.2.7/esi_leap/common/ironic.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/common/service.py` & `esi-leap-0.2.7/esi_leap/common/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from oslo_db import options as db_options
 from oslo_log import log
 from oslo_service import service
 
+from esi_leap.common import rpc
 import esi_leap.conf
 from esi_leap import objects
 from esi_leap import version
 
 CONF = esi_leap.conf.CONF
 
 
@@ -26,12 +27,13 @@
     log.register_options(CONF)
     CONF(argv[1:],
          project='esi-leap',
          version=version.version_info.release_string(),
          default_config_files=default_config_files)
     db_options.set_defaults(CONF)
     log.setup(CONF, 'esi-leap')
+    rpc.init(CONF)
     objects.register_all()
 
 
 def process_launcher():
     return service.ProcessLauncher(CONF, restart_method='mutate')
```

### Comparing `esi-leap-0.2.6/esi_leap/common/i18n.py` & `esi-leap-0.2.7/esi_leap/common/i18n.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/common/constants.py` & `esi-leap-0.2.7/esi_leap/common/constants.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/common/statuses.py` & `esi-leap-0.2.7/esi_leap/common/statuses.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/common/keystone.py` & `esi-leap-0.2.7/esi_leap/common/keystone.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/db/base.py` & `esi-leap-0.2.7/esi_leap/db/base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/db/sqlalchemy/models.py` & `esi-leap-0.2.7/esi_leap/db/sqlalchemy/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     )
 
     id = Column(Integer, primary_key=True, nullable=False, autoincrement=True)
     uuid = Column(String(36), nullable=False, unique=True)
     name = Column(String(35), nullable=True, unique=False)
     project_id = Column(String(255), nullable=False)
     owner_id = Column(String(255), nullable=False)
+    purpose = Column(String(255), nullable=True)
     resource_type = Column(String(36), nullable=False)
     resource_uuid = Column(String(36), nullable=False)
     start_time = Column(DateTime)
     end_time = Column(DateTime)
     fulfill_time = Column(DateTime)
     expire_time = Column(DateTime)
     status = Column(String(15), nullable=False, default=statuses.CREATED)
```

### Comparing `esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic/README.md` & `esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic/README.md`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic/env.py` & `esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/db/sqlalchemy/alembic.ini` & `esi-leap-0.2.7/esi_leap/db/sqlalchemy/alembic.ini`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/db/sqlalchemy/api.py` & `esi-leap-0.2.7/esi_leap/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/db/sqlalchemy/migration.py` & `esi-leap-0.2.7/esi_leap/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/db/api.py` & `esi-leap-0.2.7/esi_leap/db/api.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/db/migration.py` & `esi-leap-0.2.7/esi_leap/db/migration.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/version.py` & `esi-leap-0.2.7/esi_leap/version.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/conf/opts.py` & `esi-leap-0.2.7/esi_leap/conf/opts.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 _opts = [
     ('DEFAULT', esi_leap.conf.netconf.opts),
     ('api', esi_leap.conf.api.opts),
     ('dummy_node', esi_leap.conf.dummy_node.opts),
     ('ironic', esi_leap.conf.ironic.list_opts()),
     ('keystone', esi_leap.conf.keystone.list_opts()),
     ('pecan', esi_leap.conf.pecan.opts),
+    ('notification', esi_leap.conf.notification.opts),
 ]
 
 
 def list_opts():
     return _opts
```

### Comparing `esi-leap-0.2.6/esi_leap/conf/__init__.py` & `esi-leap-0.2.7/esi_leap/conf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 
 
 from esi_leap.conf import api
 from esi_leap.conf import dummy_node
 from esi_leap.conf import ironic
 from esi_leap.conf import keystone
 from esi_leap.conf import netconf
+from esi_leap.conf import notification
 from esi_leap.conf import pecan
 from oslo_config import cfg
 
 CONF = cfg.CONF
 
 
 CONF.register_group(cfg.OptGroup(name='database'))
 api.register_opts(CONF)
 dummy_node.register_opts(CONF)
 ironic.register_opts(CONF)
 keystone.register_opts(CONF)
 netconf.register_opts(CONF)
+notification.register_opts(CONF)
 pecan.register_opts(CONF)
```

### Comparing `esi-leap-0.2.6/esi_leap/conf/pecan.py` & `esi-leap-0.2.7/esi_leap/conf/pecan.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/conf/dummy_node.py` & `esi-leap-0.2.7/esi_leap/conf/dummy_node.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/conf/api.py` & `esi-leap-0.2.7/esi_leap/conf/api.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/conf/ironic.py` & `esi-leap-0.2.7/esi_leap/conf/ironic.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/conf/keystone.py` & `esi-leap-0.2.7/esi_leap/conf/keystone.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/conf/netconf.py` & `esi-leap-0.2.7/esi_leap/conf/netconf.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/base.py` & `esi-leap-0.2.7/esi_leap/tests/base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/resource_objects/test_test_node.py` & `esi-leap-0.2.7/esi_leap/tests/resource_objects/test_test_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,49 +37,47 @@
 
 
 class TestTestNode(base.TestCase):
 
     def setUp(self):
         super(TestTestNode, self).setUp()
         self.fake_test_node = test_node.TestNode('1111', '123456')
-        self.fake_admin_project_id_1 = '123'
-        self.fake_admin_project_id_2 = '123456'
 
     def test_resource_type(self):
         resource_type = self.fake_test_node.resource_type
         self.assertEqual(resource_type, 'test_node')
 
-    def test_get_resource_uuid(self):
-        resource_uuid = self.fake_test_node.get_resource_uuid()
-        self.assertEqual(resource_uuid, '1111')
-
-    def test_get_resource_name(self):
-        self.assertEqual('test-node-1111',
-                         self.fake_test_node.get_resource_name())
+    def test_get_uuid(self):
+        self.assertEqual(self.fake_test_node.get_uuid(), '1111')
 
-    def test_get_lease_uuid(self):
-        lease_uuid = self.fake_test_node.get_lease_uuid()
-        self.assertEqual(lease_uuid, '12345')
-
-    def test_get_project_id(self):
-        project_id = self.fake_test_node.get_project_id()
-        self.assertEqual(project_id, '123456')
-
-    def test_get_node_config(self):
-        config = self.fake_test_node.get_node_config()
-        self.assertEqual(config, {})
+    def test_get_name(self):
+        self.assertEqual(self.fake_test_node.get_name(), 'test-node-1111')
 
     def test_get_resource_class(self):
-        resource_class = self.fake_test_node.get_resource_class()
-        self.assertEqual(resource_class, 'fake')
+        self.assertEqual(self.fake_test_node.get_resource_class(), 'fake')
+
+    def test_get_config(self):
+        self.assertEqual(self.fake_test_node.get_config(), {})
+
+    def test_get_owner_project_id(self):
+        self.assertEqual(self.fake_test_node.get_owner_project_id(), '123456')
+
+    def test_get_lease_uuid(self):
+        self.assertEqual(self.fake_test_node.get_lease_uuid(), '12345')
+
+    def test_get_lessee_project_id(self):
+        self.assertEqual(self.fake_test_node.get_lessee_project_id(), '123456')
 
     def test_set_lease(self):
         fake_lease = get_test_lease()
         self.assertEqual(self.fake_test_node.set_lease(fake_lease), None)
 
-    def test_expire_lease(self):
+    def test_remove_lease(self):
         fake_lease = get_test_lease()
-        self.assertEqual(self.fake_test_node.expire_lease(fake_lease), None)
+        self.assertEqual(self.fake_test_node.remove_lease(fake_lease), None)
+
+    def test_get_node_power_state(self):
+        self.assertEqual(self.fake_test_node.get_node_power_state(), 'Off')
 
-    def test_resource_admin_project_id(self):
-        self.assertEqual(self.fake_admin_project_id_2,
-                         self.fake_test_node.resource_admin_project_id())
+    def test_get_node_provision_state(self):
+        self.assertEqual(self.fake_test_node.get_node_provision_state(),
+                         'available')
```

### Comparing `esi-leap-0.2.6/esi_leap/tests/resource_objects/test_dummy_node.py` & `esi-leap-0.2.7/esi_leap/tests/resource_objects/test_dummy_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,129 +5,148 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
+
 import datetime
+import json
+
+import mock
+
 from esi_leap.common import statuses
 from esi_leap.resource_objects import dummy_node
 from esi_leap.tests import base
-import json
-import mock
 
 
 start = datetime.datetime(2016, 7, 16, 19, 20, 30)
 
 
-def get_test_dummy_node_1():
-    return {
+class FakeLease(object):
+    def __init__(self):
+        self.uuid = '001'
+        self.project_id = '654321'
+        self.start_time = start + datetime.timedelta(days=5)
+        self.end_time = start + datetime.timedelta(days=10)
+        self.status = statuses.CREATED
+        self.offer_uuid = '534653c9-880d-4c2d-6d6d-f4f2a09e384'
+
+
+class TestDummyNode(base.TestCase):
+
+    test_node_1 = {
         'project_owner_id': '123456',
         'project_id': '654321',
         'lease_uuid': '001',
         'resource_class': 'fake',
+        'power_state': 'off',
+        'provision_state': 'enroll',
         'server_config': {
             'new attribute XYZ': 'new attribute XYZ',
             'cpu_type': 'Intel Xeon',
             'cores': 16,
             'ram_gb': 512,
             'storage_type': 'samsung SSD',
             'storage_size_gb': 204
         }
     }
 
-
-def get_test_dummy_node_2():
-    return {
+    test_node_2 = {
         'project_owner_id': '123456',
         'resource_class': 'fake',
         'server_config': {
             'new attribute XYZ': 'new attribute XYZ',
             'cpu_type': 'Intel Xeon',
             'cores': 16,
             'ram_gb': 512,
             'storage_type': 'samsung SSD',
             'storage_size_gb': 204
         }
     }
 
-
-class FakeLease(object):
-    def __init__(self):
-        self.uuid = '001'
-        self.project_id = '654321'
-        self.start_time = start + datetime.timedelta(days=5)
-        self.end_time = start + datetime.timedelta(days=10)
-        self.status = statuses.CREATED
-        self.offer_uuid = '534653c9-880d-4c2d-6d6d-f4f2a09e384'
-
-
-class TestDummyNode(base.TestCase):
-
     def setUp(self):
         super(TestDummyNode, self).setUp()
         self.fake_dummy_node = dummy_node.DummyNode('1111')
-        self.fake_admin_project_id_1 = '123'
-        self.fake_admin_project_id_2 = '123456'
-        self.fake_read_data_1 = json.dumps(get_test_dummy_node_1())
-        self.fake_read_data_2 = json.dumps(get_test_dummy_node_2())
+        self.fake_read_data_1 = json.dumps(self.test_node_1)
+        self.fake_read_data_2 = json.dumps(self.test_node_2)
 
     def test_resource_type(self):
         self.assertEqual('dummy_node', self.fake_dummy_node.resource_type)
 
-    def test_get_resource_uuid(self):
-        self.assertEqual('1111', self.fake_dummy_node.get_resource_uuid())
+    def test_get_uuid(self):
+        self.assertEqual('1111', self.fake_dummy_node.get_uuid())
 
-    def test_get_resource_name(self):
+    def test_get_name(self):
         self.assertEqual('dummy-node-1111',
-                         self.fake_dummy_node.get_resource_name())
+                         self.fake_dummy_node.get_name())
+
+    def test_get_resource_class(self):
+        mock_open = mock.mock_open(read_data=self.fake_read_data_1)
+        with mock.patch('builtins.open', mock_open) as mock_file_open:
+            resource_class = self.fake_dummy_node.get_resource_class()
+            self.assertEqual(resource_class,
+                             self.test_node_1['resource_class'])
+            mock_file_open.assert_called_once()
+
+    def test_get_config(self):
+        mock_open = mock.mock_open(read_data=self.fake_read_data_1)
+        with mock.patch('builtins.open', mock_open) as mock_file_open:
+            config = self.fake_dummy_node.get_config()
+            self.assertEqual(config, self.test_node_1['server_config'])
+            mock_file_open.assert_called_once()
+
+    def test_get_owner_project_id(self):
+        mock_open = mock.mock_open(read_data=self.fake_read_data_1)
+        with mock.patch('builtins.open', mock_open) as mock_file_open:
+            self.assertEqual(self.fake_dummy_node.get_owner_project_id(),
+                             self.test_node_1['project_owner_id'])
+            self.assertEqual(mock_file_open.call_count, 1)
 
     def test_get_lease_uuid(self):
         mock_open = mock.mock_open(read_data=self.fake_read_data_1)
         with mock.patch('builtins.open', mock_open) as mock_file_open:
             lease_uuid = self.fake_dummy_node.get_lease_uuid()
             self.assertEqual(lease_uuid, '001')
             mock_file_open.assert_called_once()
 
-    def test_get_project_id(self):
+    def test_get_lessee_project_id(self):
         mock_open = mock.mock_open(read_data=self.fake_read_data_1)
         with mock.patch('builtins.open', mock_open) as mock_file_open:
-            project_id = self.fake_dummy_node.get_project_id()
+            project_id = self.fake_dummy_node.get_lessee_project_id()
             self.assertEqual(project_id, '654321')
             mock_file_open.assert_called_once()
 
-    def test_get_node_config(self):
+    def test_get_node_power_state(self):
         mock_open = mock.mock_open(read_data=self.fake_read_data_1)
         with mock.patch('builtins.open', mock_open) as mock_file_open:
-            config = self.fake_dummy_node.get_node_config()
-            self.assertEqual(config, get_test_dummy_node_1()['server_config'])
+            power_state = self.fake_dummy_node.get_node_power_state()
+            self.assertEqual(power_state, 'off')
             mock_file_open.assert_called_once()
 
-    def test_get_resource_class(self):
+    def test_get_node_provision_state(self):
         mock_open = mock.mock_open(read_data=self.fake_read_data_1)
         with mock.patch('builtins.open', mock_open) as mock_file_open:
-            resource_class = self.fake_dummy_node.get_resource_class()
-            self.assertEqual(resource_class,
-                             get_test_dummy_node_1()['resource_class'])
+            provision_state = self.fake_dummy_node.get_node_provision_state()
+            self.assertEqual(provision_state, 'enroll')
             mock_file_open.assert_called_once()
 
     def test_set_lease(self):
         mock_open = mock.mock_open(read_data=self.fake_read_data_2)
         with mock.patch('builtins.open', mock_open) as mock_file_open:
             fake_lease = FakeLease()
             self.fake_dummy_node.set_lease(fake_lease)
             self.assertEqual(mock_file_open.call_count, 2)
 
-    def test_expire_lease(self):
+    def test_remove_lease(self):
         mock_open = mock.mock_open(read_data=self.fake_read_data_1)
         with mock.patch('builtins.open', mock_open) as mock_file_open:
             fake_lease = FakeLease()
-            self.fake_dummy_node.expire_lease(fake_lease)
+            self.fake_dummy_node.remove_lease(fake_lease)
             self.assertEqual(mock_file_open.call_count, 2)
 
-    def test_resource_admin_project_id(self):
-        mock_open = mock.mock_open(read_data=self.fake_read_data_1)
-        with mock.patch('builtins.open', mock_open) as mock_file_open:
-            self.assertEqual(self.fake_admin_project_id_2,
-                             self.fake_dummy_node.resource_admin_project_id())
-            self.assertEqual(mock_file_open.call_count, 1)
+    @mock.patch('builtins.open')
+    def test_get_deleted_node_info(self, mock_open):
+        mock_open.side_effect = FileNotFoundError
+        self.assertEqual(self.fake_dummy_node.get_resource_class(),
+                         'unknown-class')
```

### Comparing `esi-leap-0.2.6/esi_leap/tests/resource_objects/test_resource_objects.py` & `esi-leap-0.2.7/esi_leap/tests/resource_objects/test_resource_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     @mock.patch('esi_leap.resource_objects.ironic_node.is_uuid_like')
     def test_ironic_node(self, mock_iul):
         mock_iul.return_value = True
         node = resource_objects.get_resource_object('ironic_node', '1111')
 
         mock_iul.assert_called_once_with('1111')
         self.assertIsInstance(node, resource_objects.ironic_node.IronicNode)
-        self.assertEqual('1111', node.get_resource_uuid())
+        self.assertEqual('1111', node.get_uuid())
 
     @mock.patch('esi_leap.resource_objects.ironic_node.get_ironic_client')
     @mock.patch('esi_leap.resource_objects.ironic_node.is_uuid_like')
     def test_ironic_node_by_name(self, mock_iul, mock_gic):
         mock_ironic_client = mock.MagicMock()
         mock_ironic_node = mock.MagicMock()
         mock_uuid = mock.PropertyMock()
@@ -69,25 +69,25 @@
         node = resource_objects.get_resource_object('ironic_node', 'node-name')
 
         mock_iul.assert_called_with('node-name')
         mock_gic.assert_called_once_with()
         mock_uuid.assert_called_once_with()
         mock_ironic_client.node.get.assert_called_once_with('node-name')
         self.assertIsInstance(node, resource_objects.ironic_node.IronicNode)
-        self.assertEqual('1111', node.get_resource_uuid())
+        self.assertEqual('1111', node.get_uuid())
 
     def test_dummy_node(self):
         node = resource_objects.get_resource_object('dummy_node', '1111')
 
         self.assertIsInstance(node, resource_objects.dummy_node.DummyNode)
-        self.assertEqual('1111', node.get_resource_uuid())
+        self.assertEqual('1111', node.get_uuid())
 
     def test_test_node(self):
         node = resource_objects.get_resource_object('test_node', '1111')
 
         self.assertIsInstance(node, resource_objects.test_node.TestNode)
-        self.assertEqual('1111', node.get_resource_uuid())
+        self.assertEqual('1111', node.get_uuid())
 
     def test_unknown_resource_type(self):
         self.assertRaises(exception.ResourceTypeUnknown,
                           resource_objects.get_resource_object,
                           'foo_node', '1111')
```

### Comparing `esi-leap-0.2.6/esi_leap/tests/resource_objects/test_ironic_node.py` & `esi-leap-0.2.7/esi_leap/tests/resource_objects/test_ironic_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import datetime
+
+from ironicclient.common.apiclient import exceptions as ir_exception
+import mock
+
+from esi_leap.common import exception
 from esi_leap.common import statuses
 from esi_leap.resource_objects import ironic_node
 from esi_leap.tests import base
-from ironicclient.common.apiclient import exceptions
-import mock
 
 start = datetime.datetime(2016, 7, 16, 19, 20, 30)
 fake_uuid = '13921c8d-ce11-4b6d-99ed-10e19d184e5f'
 
 
 class FakeIronicNode(object):
     def __init__(self):
@@ -27,183 +30,201 @@
         self.lessee = 'abcdef'
         self.owner = '123456'
         self.name = 'fake-node'
         self.properties = {'lease_uuid': '001'}
         self.provision_state = 'available'
         self.uuid = fake_uuid
         self.resource_class = 'baremetal'
+        self.power_state = 'off'
 
 
 class FakeLease(object):
     def __init__(self):
         self.uuid = '001'
         self.project_id = '654321'
         self.start_time = start + datetime.timedelta(days=5)
         self.end_time = start + datetime.timedelta(days=10)
         self.status = statuses.ACTIVE
         self.offer_uuid = '534653c9-880d-4c2d-6d6d-f4f2a09e384'
 
 
 class TestIronicNode(base.TestCase):
 
-    def setUp(self):
-        super(TestIronicNode, self).setUp()
-        self.fake_admin_project_id_1 = '123'
-        self.fake_admin_project_id_2 = '123456'
-
     def test_resource_type(self):
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
         self.assertEqual('ironic_node', test_ironic_node.resource_type)
 
-    def test_get_resource_uuid(self):
+    def test_get_uuid(self):
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
-        self.assertEqual(fake_uuid, test_ironic_node.get_resource_uuid())
+        self.assertEqual(fake_uuid, test_ironic_node.get_uuid())
 
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
-    def test_get_resource_name(self, mock_gn):
+    def test_get_name(self, mock_gn):
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
         fake_get_node = FakeIronicNode()
         mock_gn.return_value = fake_get_node
 
-        name = test_ironic_node.get_resource_name()
-
-        self.assertEqual('fake-node', name)
+        self.assertEqual(fake_get_node.name, test_ironic_node.get_name())
         mock_gn.assert_called_once()
 
     @mock.patch.object(ironic_node, 'get_ironic_client', autospec=True)
-    def test_get_by_name(self, mock_gn):
+    def test_init_with_name(self, mock_gn):
         fake_get_node = FakeIronicNode()
         mock_gn.return_value.node.get.return_value = fake_get_node
         test_ironic_node = ironic_node.IronicNode('node-name')
-        self.assertEqual(fake_uuid, test_ironic_node.get_resource_uuid())
+
+        self.assertEqual(fake_uuid, test_ironic_node.get_uuid())
         mock_gn.assert_called_once()
         mock_gn.return_value.node.get.assert_called_once_with('node-name')
 
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
-    def test_get_lease_uuid(self, mock_gn):
+    def test_get_resource_class(self, mock_gn):
+        test_ironic_node = ironic_node.IronicNode(fake_uuid)
+        fake_get_node = FakeIronicNode()
+        mock_gn.return_value = fake_get_node
+
+        resource_class = test_ironic_node.get_resource_class()
+        self.assertEqual('baremetal', resource_class)
+        mock_gn.assert_called_once()
+
+    @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
+    def test_get_config(self, mock_gn):
         fake_get_node = FakeIronicNode()
         mock_gn.return_value = fake_get_node
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
-        lease_uuid = test_ironic_node.get_lease_uuid()
-        expected_lease_uuid = fake_get_node.properties.get('lease_uuid')
-        self.assertEqual(lease_uuid, expected_lease_uuid)
+
+        config = test_ironic_node.get_config()
+        expected_config = fake_get_node.properties
+        expected_config.pop('lease_uuid', None)
+        self.assertEqual(config, expected_config)
         mock_gn.assert_called_once()
 
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
-    def test_get_project_id(self, mock_gn):
+    def test_get_owner_project_id(self, mock_gn):
         fake_get_node = FakeIronicNode()
         mock_gn.return_value = fake_get_node
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
-        project_id = test_ironic_node.get_project_id()
-        expected_project_id = fake_get_node.lessee
-        self.assertEqual(project_id, expected_project_id)
+
+        self.assertEqual(test_ironic_node.get_owner_project_id(),
+                         fake_get_node.owner)
         mock_gn.assert_called_once()
 
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
-    def test_get_node_config(self, mock_gn):
+    def test_get_lease_uuid(self, mock_gn):
         fake_get_node = FakeIronicNode()
         mock_gn.return_value = fake_get_node
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
-        config = test_ironic_node.get_node_config()
-        expected_config = fake_get_node.properties
-        expected_config.pop('lease_uuid', None)
-        self.assertEqual(config, expected_config)
+
+        self.assertEqual(test_ironic_node.get_lease_uuid(),
+                         fake_get_node.properties.get('lease_uuid'))
         mock_gn.assert_called_once()
 
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
-    def test_get_resource_class(self, mock_gn):
+    def test_get_lessee_project_id(self, mock_gn):
+        fake_get_node = FakeIronicNode()
+        mock_gn.return_value = fake_get_node
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
+
+        self.assertEqual(test_ironic_node.get_lessee_project_id(),
+                         fake_get_node.lessee)
+        mock_gn.assert_called_once()
+
+    @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
+    def test_get_node_power_state(self, mock_gn):
         fake_get_node = FakeIronicNode()
         mock_gn.return_value = fake_get_node
+        test_ironic_node = ironic_node.IronicNode(fake_uuid)
 
-        resource_class = test_ironic_node.get_resource_class()
+        self.assertEqual(test_ironic_node.get_node_power_state(),
+                         fake_get_node.power_state)
+        mock_gn.assert_called_once()
 
-        self.assertEqual('baremetal', resource_class)
+    @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
+    def test_get_node_provision_state(self, mock_gn):
+        fake_get_node = FakeIronicNode()
+        mock_gn.return_value = fake_get_node
+        test_ironic_node = ironic_node.IronicNode(fake_uuid)
+
+        self.assertEqual(test_ironic_node.get_node_provision_state(),
+                         fake_get_node.provision_state)
         mock_gn.assert_called_once()
 
     @mock.patch.object(ironic_node, 'get_ironic_client', autospec=True)
     def test_set_lease(self, client_mock):
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
         fake_lease = FakeLease()
+
         test_ironic_node.set_lease(fake_lease)
         client_mock.assert_called_once()
         client_mock.return_value.node.update.assert_called_once_with(
-            fake_uuid, [
-                {'op': 'add',
-                 'path': '/properties/lease_uuid', 'value': '001'},
-                {'op': 'add', 'path': '/lessee', 'value': '654321'}])
+            fake_uuid, [{'op': 'add',
+                         'path': '/properties/lease_uuid',
+                         'value': fake_lease.uuid},
+                        {'op': 'add',
+                         'path': '/lessee',
+                         'value': fake_lease.project_id}])
 
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode.'
-                'get_project_id')
+                'get_lessee_project_id')
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode.'
                 'get_lease_uuid')
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
     @mock.patch.object(ironic_node, 'get_ironic_client', autospec=True)
-    def test_expire_lease(self, mock_client, mock_gn, mock_glu, mock_gpi):
+    def test_remove_lease(self, mock_client, mock_gn, mock_glu, mock_glpi):
         fake_get_node = FakeIronicNode()
         fake_get_node.provision_state = 'active'
         fake_lease = FakeLease()
 
         mock_gn.return_value = fake_get_node
         mock_glu.return_value = fake_lease.uuid
-        mock_gpi.return_value = fake_lease.project_id
+        mock_glpi.return_value = fake_lease.project_id
 
-        fake_lease = FakeLease()
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
-        test_ironic_node.expire_lease(fake_lease)
+        test_ironic_node.remove_lease(fake_lease)
 
-        mock_gpi.assert_called_once()
+        mock_glpi.assert_called_once()
         mock_glu.assert_called_once()
         self.assertEqual(mock_gn.call_count, 1)
         self.assertEqual(mock_client.call_count, 2)
         mock_client.return_value.node.update.assert_called_once_with(
-            fake_uuid, [
-                {'op': 'remove', 'path': '/properties/lease_uuid'},
-                {'op': 'remove', 'path': '/lessee'}])
+            fake_uuid, [{'op': 'remove', 'path': '/properties/lease_uuid'},
+                        {'op': 'remove', 'path': '/lessee'}])
         mock_client.return_value.node.set_provision_state. \
             assert_called_once_with(fake_uuid, 'deleted')
 
     @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode.'
                 'get_lease_uuid')
     def test_expire_lease_no_match(self, mock_glu):
         mock_glu.return_value = 'none'
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
         fake_lease = FakeLease()
-        test_ironic_node.expire_lease(fake_lease)
-        mock_glu.assert_called_once()
 
-    @mock.patch('esi_leap.resource_objects.ironic_node.IronicNode._get_node')
-    def test_resource_admin_project_id(self, mock_gn):
-        fake_get_node = FakeIronicNode()
-        mock_gn.return_value = fake_get_node
-        test_ironic_node = ironic_node.IronicNode(fake_uuid)
-        self.assertEqual(self.fake_admin_project_id_2,
-                         test_ironic_node.resource_admin_project_id())
-        mock_gn.assert_called_once()
+        test_ironic_node.remove_lease(fake_lease)
+        mock_glu.assert_called_once()
 
     @mock.patch('esi_leap.common.ironic.get_node')
     def test_get_node(self, mock_gn):
         fake_get_node = FakeIronicNode()
         mock_gn.return_value = fake_get_node
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
-        self.assertEqual(fake_get_node,
-                         test_ironic_node._get_node())
+
+        self.assertEqual(test_ironic_node._get_node(), fake_get_node)
         mock_gn.assert_called_once_with(fake_uuid, None)
 
     @mock.patch('esi_leap.common.ironic.get_node')
     def test_get_node_cache(self, mock_gn):
         fake_get_node = FakeIronicNode()
         mock_gn.return_value = fake_get_node
         test_ironic_node = ironic_node.IronicNode(fake_uuid)
         test_ironic_node._node = fake_get_node
+
         self.assertEqual(fake_get_node,
                          test_ironic_node._get_node())
-        mock_gn.assert_not_called
+        mock_gn.assert_not_called()
 
     @mock.patch('esi_leap.common.ironic.get_node')
     def test_get_unknown_node(self, mock_gn):
-        unknown_get_node = ironic_node.UnknownIronicNode()
-        mock_gn.side_effect = exceptions.NotFound
+        mock_gn.side_effect = ir_exception.NotFound
         test_unknown_node = ironic_node.IronicNode(fake_uuid)
-        test_unknown_node._node = unknown_get_node
-        self.assertEqual(type(unknown_get_node),
-                         type(ironic_node.UnknownIronicNode()))
+
+        self.assertRaises(exception.NodeNotFound,
+                          test_unknown_node._get_node)
```

### Comparing `esi-leap-0.2.6/esi_leap/tests/api/base.py` & `esi-leap-0.2.7/esi_leap/tests/api/base.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/test_lease.py` & `esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/test_lease.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,16 @@
                   mock_gpufi, mock_gro, mock_lgdwai):
         resource = TestNode('1234567890')
         data = {
             'project_id': 'lesseeid',
             'resource_type': 'test_node',
             'resource_uuid': '1234567890',
             'start_time': '2016-07-16T19:20:30',
-            'end_time': '2016-08-16T19:20:30'
+            'end_time': '2016-08-16T19:20:30',
+            'purpose': 'test_purpose'
         }
         return_data = data.copy()
         return_data['owner_id'] = self.context.project_id
         return_data['uuid'] = self.test_lease.uuid
         lgdwai_return_data = return_data.copy()
         lgdwai_return_data['start_time'] = datetime.datetime(
             2016, 7, 16, 19, 20, 30)
```

### Comparing `esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/test_node.py` & `esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/test_node.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/test_utils.py` & `esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -150,62 +150,57 @@
         self.assertEqual(res, test_offer)
 
         mock_is_uuid_like.assert_called_once_with(test_offer.uuid)
         mock_offer_get.assert_called_once_with(test_offer.uuid)
 
     @mock.patch('oslo_utils.uuidutils.is_uuid_like')
     @mock.patch('esi_leap.objects.offer.Offer.get')
-    def test_get_offer_uuid_available(self,
-                                      mock_offer_get,
-                                      mock_is_uuid_like):
+    def test_get_offer_uuid_available(self, mock_offer_get, mock_is_uuid_like):
 
         mock_is_uuid_like.return_value = True
         mock_offer_get.return_value = test_offer
 
         res = utils.get_offer(test_offer.uuid, statuses.AVAILABLE)
 
         self.assertEqual(res, test_offer)
 
         mock_is_uuid_like.assert_called_once_with(test_offer.uuid)
         mock_offer_get.assert_called_once_with(test_offer.uuid)
 
     @mock.patch('oslo_utils.uuidutils.is_uuid_like')
     @mock.patch('esi_leap.objects.offer.Offer.get')
-    def test_get_offer_uuid_bad_status(self,
-                                       mock_offer_get,
+    def test_get_offer_uuid_bad_status(self, mock_offer_get,
                                        mock_is_uuid_like):
 
         mock_is_uuid_like.return_value = True
         mock_offer_get.return_value = test_offer
 
         self.assertRaises(exception.OfferNotFound,
                           utils.get_offer,
                           test_offer.uuid, statuses.DELETED)
 
         mock_is_uuid_like.assert_called_once_with(test_offer.uuid)
         mock_offer_get.assert_called_once_with(test_offer.uuid)
 
     @mock.patch('oslo_utils.uuidutils.is_uuid_like')
     @mock.patch('esi_leap.objects.offer.Offer.get_all')
-    def test_get_offer_name_available(self,
-                                      mock_offer_get_all,
+    def test_get_offer_name_available(self, mock_offer_get_all,
                                       mock_is_uuid_like):
 
         mock_is_uuid_like.return_value = False
         mock_offer_get_all.return_value = [test_offer]
 
         res = utils.get_offer(test_offer.name, statuses.AVAILABLE)
 
         self.assertEqual(res, test_offer)
 
         mock_is_uuid_like.assert_called_once_with(test_offer.name)
         mock_offer_get_all.assert_called_once_with(
             {'name': test_offer.name,
-             'status': statuses.AVAILABLE}
-        )
+             'status': statuses.AVAILABLE})
 
     @mock.patch('oslo_utils.uuidutils.is_uuid_like')
     @mock.patch('esi_leap.objects.lease.Lease.get')
     def test_get_lease_uuid(self, mock_lease_get, mock_is_uuid_like):
 
         mock_is_uuid_like.return_value = True
         mock_lease_get.return_value = test_lease
@@ -215,109 +210,98 @@
         self.assertEqual(res, test_lease)
 
         mock_is_uuid_like.assert_called_once_with(test_lease.uuid)
         mock_lease_get.assert_called_once_with(test_lease.uuid)
 
     @mock.patch('oslo_utils.uuidutils.is_uuid_like')
     @mock.patch('esi_leap.objects.lease.Lease.get')
-    def test_get_lease_uuid_available(self,
-                                      mock_lease_get,
-                                      mock_is_uuid_like):
+    def test_get_lease_uuid_available(self, mock_lease_get, mock_is_uuid_like):
 
         mock_is_uuid_like.return_value = True
         mock_lease_get.return_value = test_lease
 
         res = utils.get_lease(test_lease.uuid, [statuses.CREATED])
 
         self.assertEqual(res, test_lease)
 
         mock_is_uuid_like.assert_called_once_with(test_lease.uuid)
         mock_lease_get.assert_called_once_with(test_lease.uuid)
 
     @mock.patch('oslo_utils.uuidutils.is_uuid_like')
     @mock.patch('esi_leap.objects.lease.Lease.get')
-    def test_get_lease_uuid_bad_status(self,
-                                       mock_lease_get,
+    def test_get_lease_uuid_bad_status(self, mock_lease_get,
                                        mock_is_uuid_like):
 
         mock_is_uuid_like.return_value = True
         mock_lease_get.return_value = test_lease
 
         self.assertRaises(exception.LeaseNotFound,
                           utils.get_lease,
                           test_lease.uuid, statuses.DELETED)
 
         mock_is_uuid_like.assert_called_once_with(test_lease.uuid)
         mock_lease_get.assert_called_once_with(test_lease.uuid)
 
     @mock.patch('oslo_utils.uuidutils.is_uuid_like')
     @mock.patch('esi_leap.objects.lease.Lease.get_all')
-    def test_get_lease_name_active(self,
-                                   mock_lease_get_all,
+    def test_get_lease_name_active(self, mock_lease_get_all,
                                    mock_is_uuid_like):
 
         mock_is_uuid_like.return_value = False
         mock_lease_get_all.return_value = [test_lease]
 
         res = utils.get_lease(test_lease.name, statuses.ACTIVE)
 
         self.assertEqual(res, test_lease)
 
         mock_is_uuid_like.assert_called_once_with(test_lease.name)
         mock_lease_get_all.assert_called_once_with(
             {'name': test_lease.name,
-             'status': statuses.ACTIVE}
-        )
+             'status': statuses.ACTIVE})
 
 
 class TestCheckResourceAdminUtils(testtools.TestCase):
 
-    @mock.patch.object(test_node_1, 'resource_admin_project_id')
+    @mock.patch.object(test_node_1, 'get_owner_project_id')
     @mock.patch('esi_leap.api.controllers.v1.utils.resource_policy_authorize')
-    def test_check_resource_admin_owner(self,
-                                        mock_authorize,
-                                        mock_ra):
-        mock_ra.return_value = owner_ctx.project_id
+    def test_check_resource_admin_owner(self, mock_authorize, mock_gopi):
+        mock_gopi.return_value = owner_ctx.project_id
 
         utils.check_resource_admin(owner_ctx.to_policy_values(),
                                    test_node_1,
                                    test_offer.project_id)
+        mock_gopi.assert_called_once()
+        mock_authorize.assert_not_called()
 
-        mock_ra.assert_called_once()
-        assert not mock_authorize.called
-
-    @mock.patch.object(test_node_2, 'resource_admin_project_id')
+    @mock.patch.object(test_node_2, 'get_owner_project_id')
     @mock.patch('esi_leap.api.controllers.v1.utils.resource_policy_authorize')
-    def test_check_resource_admin_admin(self,
-                                        mock_authorize,
-                                        mock_ra):
-        mock_ra.return_value = owner_ctx_2.project_id
+    def test_check_resource_admin_admin(self, mock_authorize, mock_gopi):
+        mock_gopi.return_value = owner_ctx_2.project_id
 
         bad_test_offer = offer.Offer(
             resource_type='test_node',
             resource_uuid=test_node_2._uuid,
             project_id=owner_ctx.project_id
         )
 
         utils.check_resource_admin(admin_ctx.to_policy_values(),
                                    test_node_2,
                                    bad_test_offer.project_id)
 
-        mock_ra.assert_called_once()
+        mock_gopi.assert_called_once()
         mock_authorize.assert_called_once_with('esi_leap:offer:offer_admin',
                                                admin_ctx.to_policy_values(),
                                                admin_ctx.to_policy_values(),
                                                'test_node', test_node_2._uuid)
 
-    @mock.patch.object(test_node_2, 'resource_admin_project_id')
+    @mock.patch.object(test_node_2, 'get_owner_project_id')
     @mock.patch('esi_leap.api.controllers.v1.utils.resource_policy_authorize')
-    def test_check_resource_admin_invalid_owner(self,
-                                                mock_authorize,
-                                                mock_ra):
-        mock_ra.return_value = owner_ctx_2.project_id
+    def test_check_resource_admin_invalid_owner(self, mock_authorize,
+                                                mock_gopi):
+        mock_gopi.return_value = owner_ctx_2.project_id
         mock_authorize.side_effect = exception.HTTPResourceForbidden(
             resource_type='test_node', resource=test_node_2._uuid)
 
         bad_test_offer = offer.Offer(
             resource_type='test_node',
             resource_uuid=test_node_2._uuid,
             project_id=owner_ctx.project_id
@@ -325,15 +309,15 @@
 
         self.assertRaises(exception.HTTPResourceForbidden,
                           utils.check_resource_admin,
                           owner_ctx_2.to_policy_values(),
                           test_node_2,
                           bad_test_offer.project_id)
 
-        mock_ra.assert_called_once()
+        mock_gopi.assert_called_once()
         mock_authorize.assert_called_once_with('esi_leap:offer:offer_admin',
                                                owner_ctx_2.to_policy_values(),
                                                owner_ctx_2.to_policy_values(),
                                                'test_node', test_node_2._uuid)
 
 
 class TestCheckResourceLeaseAdminUtils(testtools.TestCase):
@@ -353,118 +337,111 @@
             end_time=datetime.datetime(2016, 8, 16, 19, 20, 30),
             parent_lease_uuid='parent-lease-uuid'
         )
 
     @mock.patch('esi_leap.objects.lease.Lease.get')
     @mock.patch.object(test_node_1, 'get_lease_uuid',
                        return_value='a-lease-uuid')
-    @mock.patch.object(test_node_1, 'get_project_id',
+    @mock.patch.object(test_node_1, 'get_lessee_project_id',
                        return_value=test_offer.project_id)
-    def test_check_resource_lease_admin_okay(self,
-                                             mock_gpi,
-                                             mock_glu,
+    def test_check_resource_lease_admin_okay(self, mock_glpi, mock_glu,
                                              mock_lease_get):
         mock_lease_get.return_value = self.test_lease
         parent_lease_uuid = utils.check_resource_lease_admin(
             owner_ctx.to_policy_values(),
             test_node_1,
             test_offer.project_id,
             datetime.datetime(2016, 7, 16, 19, 20, 30),
             datetime.datetime(2016, 8, 16, 19, 20, 30))
 
-        mock_gpi.assert_called_once()
+        mock_glpi.assert_called_once()
         mock_glu.assert_called_once()
         mock_lease_get.assert_called_once_with('a-lease-uuid')
         self.assertEqual('a-lease-uuid', parent_lease_uuid)
 
     @mock.patch('esi_leap.objects.lease.Lease.get')
     @mock.patch.object(test_node_1, 'get_lease_uuid',
                        return_value='a-lease-uuid')
-    @mock.patch.object(test_node_1, 'get_project_id',
+    @mock.patch.object(test_node_1, 'get_lessee_project_id',
                        return_value='other-lessee')
-    def test_check_resource_lease_admin_not_lessee(self,
-                                                   mock_gpi,
-                                                   mock_glu,
+    def test_check_resource_lease_admin_not_lessee(self, mock_glpi, mock_glu,
                                                    mock_lease_get):
         mock_lease_get.return_value = self.test_lease
         parent_lease_uuid = utils.check_resource_lease_admin(
             owner_ctx.to_policy_values(),
             test_node_1,
             test_offer.project_id,
             datetime.datetime(2016, 7, 16, 19, 20, 30),
             datetime.datetime(2016, 8, 16, 19, 20, 30))
 
-        mock_gpi.assert_called_once()
+        mock_glpi.assert_called_once()
         mock_glu.assert_not_called()
         mock_lease_get.assert_not_called()
         self.assertIsNone(parent_lease_uuid)
 
     @mock.patch('esi_leap.objects.lease.Lease.get')
     @mock.patch.object(test_node_1, 'get_lease_uuid',
                        return_value=None)
-    @mock.patch.object(test_node_1, 'get_project_id',
+    @mock.patch.object(test_node_1, 'get_lessee_project_id',
                        return_value=test_offer.project_id)
     def test_check_resource_lease_admin_not_lease(self,
-                                                  mock_gpi,
+                                                  mock_glpi,
                                                   mock_glu,
                                                   mock_lease_get):
         mock_lease_get.return_value = self.test_lease
         parent_lease_uuid = utils.check_resource_lease_admin(
             owner_ctx.to_policy_values(),
             test_node_1,
             test_offer.project_id,
             datetime.datetime(2016, 7, 16, 19, 20, 30),
             datetime.datetime(2016, 8, 16, 19, 20, 30))
 
-        mock_gpi.assert_called_once()
+        mock_glpi.assert_called_once()
         mock_glu.assert_called_once()
         mock_lease_get.assert_not_called()
         self.assertIsNone(parent_lease_uuid)
 
     @mock.patch('esi_leap.objects.lease.Lease.get')
     @mock.patch.object(test_node_1, 'get_lease_uuid',
                        return_value='a-lease-uuid')
-    @mock.patch.object(test_node_1, 'get_project_id',
+    @mock.patch.object(test_node_1, 'get_lessee_project_id',
                        return_value=test_offer.project_id)
     def test_check_resource_lease_admin_parent_lease(self,
-                                                     mock_gpi,
+                                                     mock_glpi,
                                                      mock_glu,
                                                      mock_lease_get):
         mock_lease_get.return_value = self.test_lease_with_parent
         parent_lease_uuid = utils.check_resource_lease_admin(
             owner_ctx.to_policy_values(),
             test_node_1,
             test_offer.project_id,
             datetime.datetime(2016, 7, 16, 19, 20, 30),
             datetime.datetime(2016, 8, 16, 19, 20, 30))
 
-        mock_gpi.assert_called_once()
+        mock_glpi.assert_called_once()
         mock_glu.assert_called_once()
         mock_lease_get.assert_called_once_with('a-lease-uuid')
         self.assertIsNone(parent_lease_uuid)
 
     @mock.patch('esi_leap.objects.lease.Lease.get')
     @mock.patch.object(test_node_1, 'get_lease_uuid',
                        return_value='a-lease-uuid')
-    @mock.patch.object(test_node_1, 'get_project_id',
+    @mock.patch.object(test_node_1, 'get_lessee_project_id',
                        return_value=test_offer.project_id)
-    def test_check_resource_lease_admin_bad_time(self,
-                                                 mock_gpi,
-                                                 mock_glu,
+    def test_check_resource_lease_admin_bad_time(self, mock_glpi, mock_glu,
                                                  mock_lease_get):
         mock_lease_get.return_value = self.test_lease
         self.assertRaises(exception.ResourceNoPermissionTime,
                           utils.check_resource_lease_admin,
                           owner_ctx.to_policy_values(),
                           test_node_1,
                           test_offer.project_id,
                           datetime.datetime(2016, 7, 15, 19, 20, 30),
                           datetime.datetime(2016, 8, 16, 19, 20, 30))
-
-        mock_gpi.assert_called_once()
+        mock_glpi.assert_called_once()
         mock_glu.assert_called_once()
         mock_lease_get.assert_called_once_with('a-lease-uuid')
 
 
 class TestOfferPolicyAndRetrieveUtils(testtools.TestCase):
 
     @mock.patch('esi_leap.api.controllers.v1.utils.resource_policy_authorize')
@@ -693,29 +670,27 @@
             resource_type='test_node',
             resource_uuid='111',
             project_id='lesseeid',
             owner_id='ownerid',
             parent_lease_uuid=None
         )
 
-    @mock.patch('esi_leap.resource_objects.test_node.TestNode.'
-                'get_resource_name')
+    @mock.patch('esi_leap.resource_objects.test_node.TestNode.get_name')
     @mock.patch('esi_leap.common.keystone.get_project_name')
     @mock.patch('esi_leap.objects.lease.get_resource_object')
-    def test_lease_get_dict_with_added_info(self, mock_gro, mock_gpn,
-                                            mock_grn):
+    def test_lease_get_dict_with_added_info(self, mock_gro, mock_gpn, mock_gn):
         mock_gro.return_value = TestNode('111')
         mock_gpn.return_value = 'project-name'
-        mock_grn.return_value = 'resource-name'
+        mock_gn.return_value = 'resource-name'
 
         output_dict = utils.lease_get_dict_with_added_info(self.test_lease)
 
         expected_output_dict = self.test_lease.to_dict()
         expected_output_dict['resource'] = 'resource-name'
         expected_output_dict['project'] = 'project-name'
         expected_output_dict['owner'] = 'project-name'
         expected_output_dict['resource_class'] = 'fake'
 
         mock_gro.assert_called_once()
         self.assertEqual(2, mock_gpn.call_count)
-        mock_grn.assert_called_once()
+        mock_gn.assert_called_once()
         self.assertEqual(expected_output_dict, output_dict)
```

### Comparing `esi-leap-0.2.6/esi_leap/tests/api/controllers/v1/test_offer.py` & `esi-leap-0.2.7/esi_leap/tests/api/controllers/v1/test_offer.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/api/controllers/test_types.py` & `esi-leap-0.2.7/esi_leap/tests/api/controllers/test_types.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/objects/test_offer.py` & `esi-leap-0.2.7/esi_leap/tests/objects/test_offer.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/manager/test_service.py` & `esi-leap-0.2.7/esi_leap/tests/manager/test_service.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/common/test_ironic.py` & `esi-leap-0.2.7/esi_leap/tests/common/test_ironic.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/common/test_utils.py` & `esi-leap-0.2.7/esi_leap/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/common/test_keystone.py` & `esi-leap-0.2.7/esi_leap/tests/common/test_keystone.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/common/test_policy.py` & `esi-leap-0.2.7/esi_leap/tests/common/test_policy.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/tests/db/sqlalchemy/test_api.py` & `esi-leap-0.2.7/esi_leap/tests/db/sqlalchemy/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,78 +88,84 @@
 test_lease_1 = dict(
     uuid='11111',
     project_id='1e5533',
     owner_id='0wn3r',
     name='l1',
     resource_uuid='1111',
     resource_type='dummy_node',
+    purpose='test_purpose',
     start_time=now + datetime.timedelta(days=10),
     end_time=now + datetime.timedelta(days=20),
     properties={},
     status=statuses.CREATED,
 )
 
 test_lease_2 = dict(
     uuid='22222',
     project_id='1e5533',
     owner_id='0wn3r',
     name='l1',
     resource_uuid='1111',
     resource_type='dummy_node',
+    purpose='test_purpose',
     start_time=now + datetime.timedelta(days=20),
     end_time=now + datetime.timedelta(days=30),
     properties={},
     status=statuses.CREATED,
 )
 
 test_lease_3 = dict(
     uuid='33333',
     project_id='1e5533_2',
     owner_id='0wn3r_2',
     name='l1',
     resource_uuid='1111',
     resource_type='dummy_node',
+    purpose='test_purpose',
     start_time=now + datetime.timedelta(days=50),
     end_time=now + datetime.timedelta(days=60),
     properties={},
     status=statuses.ACTIVE,
 )
 
 test_lease_4 = dict(
     uuid='44444',
     project_id='1e5533_2',
     owner_id='0wn3r_2',
     name='l4',
     resource_uuid='1111',
     resource_type='dummy_node',
+    purpose='test_purpose',
     start_time=now + datetime.timedelta(days=85),
     end_time=now + datetime.timedelta(days=90),
     properties={},
     status=statuses.DELETED,
 )
 
 test_lease_5 = dict(
     project_id='0wn3r',
     owner_id='0wn3r_2',
     name='l5',
     resource_uuid='1111',
     resource_type='dummy_node',
+    purpose='test_purpose',
     start_time=now + datetime.timedelta(days=90),
     end_time=now + datetime.timedelta(days=100),
     uuid='55555',
     properties={},
     status=statuses.EXPIRED,
 )
 
 test_lease_6 = dict(
     project_id='0wn3r',
     owner_id='0wn3r_2',
     name='l6',
     resource_uuid='2222',
     resource_type='dummy_node',
+    purpose='test_purpose',
     start_time=now + datetime.timedelta(days=5),
     end_time=now + datetime.timedelta(days=30),
     uuid='6666',
     properties={},
     status=statuses.EXPIRED,
 )
 
@@ -585,25 +591,27 @@
 
         self.parent_lease_data = dict(
             uuid=uuidutils.generate_uuid(),
             project_id=uuidutils.generate_uuid(),
             owner_id=uuidutils.generate_uuid(),
             resource_uuid='1111',
             resource_type='dummy_node',
+            purpose='test_purpose',
             start_time=now + datetime.timedelta(days=50),
             end_time=now + datetime.timedelta(days=100),
             status=statuses.ACTIVE,
         )
         self.child_lease_data = dict(
             uuid=uuidutils.generate_uuid(),
             project_id=uuidutils.generate_uuid(),
             owner_id=uuidutils.generate_uuid(),
             parent_lease_uuid=self.parent_lease_data['uuid'],
             resource_uuid='1111',
             resource_type='dummy_node',
+            purpose='test_purpose',
             start_time=now + datetime.timedelta(days=60),
             end_time=now + datetime.timedelta(days=70),
             status=statuses.ACTIVE,
         )
         self.child_offer_data = dict(
             uuid=uuidutils.generate_uuid(),
             project_id=uuidutils.generate_uuid(),
```

### Comparing `esi-leap-0.2.6/esi_leap/cmd/dbsync.py` & `esi-leap-0.2.7/esi_leap/cmd/dbsync.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/cmd/api.py` & `esi-leap-0.2.7/esi_leap/cmd/api.py`

 * *Files identical despite different names*

### Comparing `esi-leap-0.2.6/esi_leap/cmd/manager.py` & `esi-leap-0.2.7/esi_leap/cmd/manager.py`

 * *Files identical despite different names*

