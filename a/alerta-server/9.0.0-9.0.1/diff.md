# Comparing `tmp/alerta-server-9.0.0.tar.gz` & `tmp/alerta-server-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alerta-server-9.0.0.tar", last modified: Fri Mar 17 21:57:51 2023, max compression
+gzip compressed data, was "alerta-server-9.0.1.tar", last modified: Thu Jun 22 20:25:37 2023, max compression
```

## Comparing `alerta-server-9.0.0.tar` & `alerta-server-9.0.1.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.398382 alerta-server-9.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-17 21:57:42.000000 alerta-server-9.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-17 21:57:42.000000 alerta-server-9.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-17 21:57:42.000000 alerta-server-9.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-03-17 21:57:51.398382 alerta-server-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-03-17 21:57:42.000000 alerta-server-9.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-17 21:57:42.000000 alerta-server-9.0.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.378382 alerta-server-9.0.0/alerta/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/app.wsgi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.378382 alerta-server-9.0.0/alerta/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/basic_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/auth/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-17 21:57:51.000000 alerta-server-9.0.0/alerta/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.382382 alerta-server-9.0.0/alerta/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.382382 alerta-server-9.0.0/alerta/database/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.382382 alerta-server-9.0.0/alerta/database/backends/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/backends/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71226 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/backends/mongodb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/backends/mongodb/queryparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/backends/mongodb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.382382 alerta-server-9.0.0/alerta/database/backends/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/backends/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70216 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/backends/postgres/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/backends/postgres/queryparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/backends/postgres/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/database/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.382382 alerta-server-9.0.0/alerta/management/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/management/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.386382 alerta-server-9.0.0/alerta/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.386382 alerta-server-9.0.0/alerta/models/alarms/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/alarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/alarms/alerta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/alarms/isa_18_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25611 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/blackout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.386382 alerta-server-9.0.0/alerta/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/plugins/acked_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/plugins/blackout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/plugins/escalate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/plugins/forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/plugins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/plugins/reject.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/plugins/remote_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/plugins/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.386382 alerta-server-9.0.0/alerta/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/sql/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.386382 alerta-server-9.0.0/alerta/static/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/static/embed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.386382 alerta-server-9.0.0/alerta/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.386382 alerta-server-9.0.0/alerta/templates/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/templates/auth/saml2.html
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.386382 alerta-server-9.0.0/alerta/templates/management/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/templates/management/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/templates/management/switchboard.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.386382 alerta-server-9.0.0/alerta/templates/oembed/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/templates/oembed/counts.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.390382 alerta-server-9.0.0/alerta/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/mailer.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/paging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/utils/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.390382 alerta-server-9.0.0/alerta/views/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/blackouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/customers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/oembed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/views/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.394382 alerta-server-9.0.0/alerta/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/graylog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/newrelic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/pagerduty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/pingdom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/riemann.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/serverdensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/stackdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-03-17 21:57:42.000000 alerta-server-9.0.0/alerta/webhooks/telegram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.394382 alerta-server-9.0.0/alerta_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-03-17 21:57:51.000000 alerta-server-9.0.0/alerta_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-03-17 21:57:51.000000 alerta-server-9.0.0/alerta_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 21:57:51.000000 alerta-server-9.0.0/alerta_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-17 21:57:51.000000 alerta-server-9.0.0/alerta_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 21:57:51.000000 alerta-server-9.0.0/alerta_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-17 21:57:51.000000 alerta-server-9.0.0/alerta_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-17 21:57:51.000000 alerta-server-9.0.0/alerta_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-17 21:57:51.398382 alerta-server-9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-03-17 21:57:42.000000 alerta-server-9.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.398382 alerta-server-9.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:51.398382 alerta-server-9.0.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)    39105 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23677 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_authproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    35064 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_blackouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_cors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_customers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    36758 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_isa_18_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)    26434 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)   113133 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_queryparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_shelving.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    57492 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-03-17 21:57:42.000000 alerta-server-9.0.0/tests/test_zrouting.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 21:57:42.000000 alerta-server-9.0.0/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.316700 alerta-server-9.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 20:25:26.000000 alerta-server-9.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 20:25:26.000000 alerta-server-9.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-22 20:25:26.000000 alerta-server-9.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-22 20:25:37.316700 alerta-server-9.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-22 20:25:26.000000 alerta-server-9.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 20:25:26.000000 alerta-server-9.0.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.284699 alerta-server-9.0.1/alerta/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/app.wsgi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.288699 alerta-server-9.0.1/alerta/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/basic_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.288699 alerta-server-9.0.1/alerta/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.288699 alerta-server-9.0.1/alerta/database/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.292700 alerta-server-9.0.1/alerta/database/backends/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71239 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/mongodb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/mongodb/queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/mongodb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.292700 alerta-server-9.0.1/alerta/database/backends/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70404 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/postgres/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/postgres/queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/postgres/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14381 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.292700 alerta-server-9.0.1/alerta/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/management/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/models/alarms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/alarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/alarms/alerta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/alarms/isa_18_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25626 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/blackout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/acked_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/blackout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/escalate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/reject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/remote_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/sql/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/static/embed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/templates/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/auth/saml2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/templates/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/management/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/management/switchboard.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.300700 alerta-server-9.0.1/alerta/templates/oembed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/oembed/counts.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.300700 alerta-server-9.0.1/alerta/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/mailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/paging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.304700 alerta-server-9.0.1/alerta/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/blackouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/oembed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.308700 alerta-server-9.0.1/alerta/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/graylog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/newrelic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/pagerduty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/pingdom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/riemann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/serverdensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/stackdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/telegram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.308700 alerta-server-9.0.1/alerta_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-22 20:25:37.316700 alerta-server-9.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-22 20:25:26.000000 alerta-server-9.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.316700 alerta-server-9.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.316700 alerta-server-9.0.1/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39105 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23677 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_authproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35064 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_blackouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40388 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_isa_18_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26434 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113133 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_shelving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57492 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_zrouting.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 20:25:26.000000 alerta-server-9.0.1/wsgi.py
```

### Comparing `alerta-server-9.0.0/LICENSE` & `alerta-server-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/NOTICE` & `alerta-server-9.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/PKG-INFO` & `alerta-server-9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alerta-server
-Version: 9.0.0
+Version: 9.0.1
 Summary: Alerta server WSGI application
 Home-page: https://github.com/guardian/alerta
 Author: Nick Satterly
 Author-email: nfsatterly@gmail.com
 License: Apache License 2.0
 Keywords: alert monitoring system wsgi application api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alerta-server-9.0.0/README.md` & `alerta-server-9.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/__init__.py` & `alerta-server-9.0.1/alerta/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/app.py` & `alerta-server-9.0.1/alerta/app.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/auth/__init__.py` & `alerta-server-9.0.1/alerta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/auth/basic.py` & `alerta-server-9.0.1/alerta/auth/basic.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/auth/basic_ldap.py` & `alerta-server-9.0.1/alerta/auth/basic_ldap.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/auth/decorators.py` & `alerta-server-9.0.1/alerta/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/auth/github.py` & `alerta-server-9.0.1/alerta/auth/github.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/auth/hmac.py` & `alerta-server-9.0.1/alerta/auth/hmac.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/auth/oidc.py` & `alerta-server-9.0.1/alerta/auth/oidc.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,18 +72,19 @@
 
     data = {
         'grant_type': 'authorization_code',
         'code': request.json['code'],
         'redirect_uri': request.json['redirectUri'],
     }
 
-    if type(oidc_configuration['token_endpoint_auth_methods_supported']) == list:
-        token_endpoint_auth_methods = oidc_configuration['token_endpoint_auth_methods_supported']
-    else:
-        token_endpoint_auth_methods = [oidc_configuration['token_endpoint_auth_methods_supported']]
+    token_endpoint_auth_methods = oidc_configuration.get(
+        'token_endpoint_auth_methods_supported',
+        ['client_secret_basic'])
+    if type(token_endpoint_auth_methods) != list:
+        token_endpoint_auth_methods = [token_endpoint_auth_methods]
 
     preferred_token_auth_method = 'client_secret_post'
     for token_auth_method in current_app.config['OIDC_TOKEN_AUTH_METHODS']:
         if token_auth_method in token_endpoint_auth_methods:
             preferred_token_auth_method = token_auth_method
             break
```

### Comparing `alerta-server-9.0.0/alerta/auth/saml.py` & `alerta-server-9.0.1/alerta/auth/saml.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/auth/userinfo.py` & `alerta-server-9.0.1/alerta/auth/userinfo.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/auth/utils.py` & `alerta-server-9.0.1/alerta/auth/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/commands.py` & `alerta-server-9.0.1/alerta/commands.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/database/backends/mongodb/base.py` & `alerta-server-9.0.1/alerta/database/backends/mongodb/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # See https://github.com/MongoEngine/flask-mongoengine/blob/master/flask_mongoengine/__init__.py
 # See https://github.com/dcrosta/flask-pymongo/blob/master/flask_pymongo/__init__.py
 
 
 class Backend(Database):
 
-    def create_engine(self, app, uri, dbname=None, raise_on_error=True):
+    def create_engine(self, app, uri, dbname=None, schema=None, raise_on_error=True):
         self.uri = uri
         self.dbname = dbname
 
         db = self.connect()
 
         try:
             self._create_indexes(db)
```

### Comparing `alerta-server-9.0.0/alerta/database/backends/mongodb/queryparser.py` & `alerta-server-9.0.1/alerta/database/backends/mongodb/queryparser.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/database/backends/mongodb/utils.py` & `alerta-server-9.0.1/alerta/database/backends/mongodb/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/database/backends/postgres/base.py` & `alerta-server-9.0.1/alerta/database/backends/postgres/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,34 +58,36 @@
     'group', 'value', 'text', 'tags', 'attributes', 'origin', 'update_time',
     'user', 'timeout', 'type', 'customer'
 ])
 
 
 class Backend(Database):
 
-    def create_engine(self, app, uri, dbname=None, raise_on_error=True):
+    def create_engine(self, app, uri, dbname=None, schema='public', raise_on_error=True):
         self.uri = uri
         self.dbname = dbname
+        self.schema = schema
 
         lock = threading.Lock()
         with lock:
             conn = self.connect()
+
             with app.open_resource('sql/schema.sql') as f:
                 try:
                     conn.cursor().execute(f.read())
                     conn.commit()
                 except Exception as e:
                     if raise_on_error:
                         raise
                     app.logger.warning(e)
 
         register_adapter(dict, Json)
         register_adapter(datetime, self._adapt_datetime)
         register_composite(
-            'history',
+            schema + '.history' if schema else 'history',
             conn,
             globally=True
         )
         from alerta.models.alert import History
         register_adapter(History, HistoryAdapter)
 
     def connect(self):
@@ -93,28 +95,31 @@
         while True:
             try:
                 conn = psycopg2.connect(
                     dsn=self.uri,
                     dbname=self.dbname,
                     cursor_factory=NamedTupleCursor
                 )
+
                 conn.set_client_encoding('UTF8')
                 break
             except Exception as e:
                 print(e)  # FIXME - should log this error instead of printing, but current_app is unavailable here
                 retry += 1
                 if retry > MAX_RETRIES:
                     conn = None
                     break
                 else:
                     backoff = 2 ** retry
                     print(f'Retry attempt {retry}/{MAX_RETRIES} (wait={backoff}s)...')
                     time.sleep(backoff)
 
         if conn:
+            conn.cursor().execute('SET search_path TO {}'.format(self.schema))
+            conn.commit()
             return conn
         else:
             raise RuntimeError(f'Database connect error. Failed to connect after {MAX_RETRIES} retries.')
 
     @staticmethod
     def _adapt_datetime(dt):
         return AsIs(f'{adapt(DateTime.iso8601(dt))}')
```

### Comparing `alerta-server-9.0.0/alerta/database/backends/postgres/queryparser.py` & `alerta-server-9.0.1/alerta/database/backends/postgres/queryparser.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/database/backends/postgres/utils.py` & `alerta-server-9.0.1/alerta/database/backends/postgres/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/database/base.py` & `alerta-server-9.0.1/alerta/database/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,24 +52,24 @@
 
     def init_db(self, app):
         backend = get_backend(app)
         cls = load_backend(backend)
         self.__class__ = type('DatabaseImpl', (cls.Backend, Database), {})
 
         try:
-            self.create_engine(app, uri=app.config['DATABASE_URL'], dbname=app.config['DATABASE_NAME'],
+            self.create_engine(app, uri=app.config['DATABASE_URL'], dbname=app.config['DATABASE_NAME'], schema=app.config['DATABASE_SCHEMA'],
                                raise_on_error=app.config['DATABASE_RAISE_ON_ERROR'])
         except Exception as e:
             if app.config['DATABASE_RAISE_ON_ERROR']:
                 raise
             app.logger.warning(e)
 
         app.teardown_appcontext(self.teardown_db)
 
-    def create_engine(self, app, uri, dbname=None, raise_on_error=True):
+    def create_engine(self, app, uri, dbname=None, schema=None, raise_on_error=True):
         raise NotImplementedError('Database engine has no create_engine() method')
 
     def connect(self):
         raise NotImplementedError('Database engine has no connect() method')
 
     @property
     def name(self):
```

### Comparing `alerta-server-9.0.0/alerta/exceptions.py` & `alerta-server-9.0.1/alerta/exceptions.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/management/views.py` & `alerta-server-9.0.1/alerta/management/views.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/alarms/__init__.py` & `alerta-server-9.0.1/alerta/models/alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/alarms/alerta.py` & `alerta-server-9.0.1/alerta/models/alarms/alerta.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/alarms/isa_18_2.py` & `alerta-server-9.0.1/alerta/models/alarms/isa_18_2.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 }
 
 MORE_SEVERE = 'moreSevere'
 NO_CHANGE = 'noChange'
 LESS_SEVERE = 'lessSevere'
 
 ACTION_ACK = 'ack'
+ACTION_UNACK = 'unack'
 ACTION_SHELVE = 'shelve'
 ACTION_UNSHELVE = 'unshelve'
 
 
 class StateMachine(AlarmModel):
 
     def register(self, app):
@@ -131,14 +132,18 @@
         if state == A_NORM:
             if current_severity != StateMachine.DEFAULT_NORMAL_SEVERITY:
                 return next_state('Alarm Occurs, Normal (A) -> Unack (B)', current_severity, B_UNACK)
         # Operator Ack, Unack (B) -> Ack (C)
         if state == B_UNACK:
             if action == ACTION_ACK:
                 return next_state('Operator Ack, Unack (B) -> Ack (C)', current_severity, C_ACKED)
+        # Operator Unack, Ack (C) -> Unack (B)
+        if state == C_ACKED:
+            if action == ACTION_UNACK:
+                return next_state('Operator Unack, Ack (C) -> Unack (B)', current_severity, B_UNACK)
         # Re-Alarm, Ack (C) -> Unack (B)
         if state == C_ACKED:
             if self.trend(previous_severity, current_severity) == MORE_SEVERE:
                 if previous_severity != StateMachine.DEFAULT_PREVIOUS_SEVERITY:
                     return next_state('Re-Alarm, Ack (C) -> Unack (B)', current_severity, B_UNACK)
         # Process RTN Alarm Clears, Ack (C) -> Normal (A)
         if state == C_ACKED:
```

### Comparing `alerta-server-9.0.0/alerta/models/alert.py` & `alerta-server-9.0.1/alerta/models/alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,15 +438,15 @@
             value=self.value,
             text=text,
             change_type=ChangeType.status,
             update_time=now,
             user=g.login,
             timeout=self.timeout
         )
-        return db.set_status(self.id, status, timeout, update_time=now, history=history)
+        return Alert.from_db(db.set_status(self.id, status, timeout, update_time=now, history=history))
 
     # tag an alert
     def tag(self, tags: List[str]) -> bool:
         return db.tag_alert(self.id, tags)
 
     # untag an alert
     def untag(self, tags: List[str]) -> bool:
```

### Comparing `alerta-server-9.0.0/alerta/models/blackout.py` & `alerta-server-9.0.1/alerta/models/blackout.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/customer.py` & `alerta-server-9.0.1/alerta/models/customer.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/enums.py` & `alerta-server-9.0.1/alerta/models/enums.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/group.py` & `alerta-server-9.0.1/alerta/models/group.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/heartbeat.py` & `alerta-server-9.0.1/alerta/models/heartbeat.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/history.py` & `alerta-server-9.0.1/alerta/models/history.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/key.py` & `alerta-server-9.0.1/alerta/models/key.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/metrics.py` & `alerta-server-9.0.1/alerta/models/metrics.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/note.py` & `alerta-server-9.0.1/alerta/models/note.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/permission.py` & `alerta-server-9.0.1/alerta/models/permission.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/switch.py` & `alerta-server-9.0.1/alerta/models/switch.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/token.py` & `alerta-server-9.0.1/alerta/models/token.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/models/user.py` & `alerta-server-9.0.1/alerta/models/user.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/plugins/__init__.py` & `alerta-server-9.0.1/alerta/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/plugins/acked_by.py` & `alerta-server-9.0.1/alerta/plugins/acked_by.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/plugins/blackout.py` & `alerta-server-9.0.1/alerta/plugins/blackout.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/plugins/escalate.py` & `alerta-server-9.0.1/alerta/plugins/escalate.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/plugins/forwarder.py` & `alerta-server-9.0.1/alerta/plugins/forwarder.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/plugins/heartbeat.py` & `alerta-server-9.0.1/alerta/plugins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/plugins/reject.py` & `alerta-server-9.0.1/alerta/plugins/reject.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/plugins/remote_ip.py` & `alerta-server-9.0.1/alerta/plugins/remote_ip.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/plugins/timeout.py` & `alerta-server-9.0.1/alerta/plugins/timeout.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/settings.py` & `alerta-server-9.0.1/alerta/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 POSTGRES_URI = 'postgres://localhost:5432/monitoring'  # not used (use DATABASE_URL)
 POSTGRES_DB = None
 
 # Database
 DATABASE_URL = MONGO_URI  # default: MongoDB
 DATABASE_NAME = MONGO_DATABASE or POSTGRES_DB
 DATABASE_RAISE_ON_ERROR = MONGO_RAISE_ON_ERROR  # True - terminate, False - ignore and continue
+DATABASE_SCHEMA = 'public'  # default: None to use default schema
 
 # Search
 DEFAULT_FIELD = 'text'  # default field if no search prefix specified (Postgres only)
 
 # Bulk API
 BULK_QUERY_LIMIT = 100000  # max number of alerts for bulk endpoints
 CELERY_BROKER_URL = None
@@ -171,16 +172,16 @@
 AUDIT_LOG_REDACT = True  # redact sensitive data before logging
 AUDIT_LOG_JSON = False  # log alert data as JSON object
 AUDIT_URL = None  # send audit log events via webhook URL
 
 # CORS settings
 CORS_ALLOW_HEADERS = ['Content-Type', 'Authorization', 'Access-Control-Allow-Origin', 'X-Request-ID']
 CORS_ORIGINS = [
-    # 'http://try.alerta.io',
-    # 'http://explorer.alerta.io',
+    # 'https://try.alerta.io',
+    # 'https://explorer.alerta.io',
     'http://localhost',
     'http://localhost:8000',
     r'https?://\w*\.?local\.alerta\.io:?\d*/?.*'  # => http(s)://*.local.alerta.io:<port>
 ]
 CORS_SUPPORTS_CREDENTIALS = AUTH_REQUIRED
 
 # Serverity settings
@@ -251,14 +252,17 @@
 # List of custom actions
 ACTIONS = []  # type: List[str]
 
 SERVER_VERSION = 'full'  # show/hide server version eg. full, major, off
 GOOGLE_TRACKING_ID = None
 AUTO_REFRESH_INTERVAL = 5000  # ms
 
+# Routing
+ROUTING_DIST = 'alerta-routing'
+
 # Plugins
 PLUGINS = ['remote_ip', 'reject', 'heartbeat', 'blackout', 'forwarder']
 PLUGINS_RAISE_ON_ERROR = True  # raise RuntimeError exception on first failure
 
 # reject plugin settings
 ORIGIN_BLACKLIST = []  # type: List[str]
 # ORIGIN_BLACKLIST = ['foo/bar$', '.*/qux']  # reject all foo alerts from bar, and everything from qux
```

### Comparing `alerta-server-9.0.0/alerta/sql/schema.sql` & `alerta-server-9.0.1/alerta/sql/schema.sql`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 DO $$
 BEGIN
-    IF NOT EXISTS (SELECT 1 FROM pg_type WHERE typname = 'history') THEN
+    IF NOT EXISTS (SELECT 1 FROM pg_type WHERE typname = 'history' AND typnamespace = (SELECT oid FROM pg_namespace WHERE nspname = current_schema())) THEN
         CREATE TYPE history AS (
             id text,
             event text,
             severity text,
             status text,
             value text,
             text text,
```

### Comparing `alerta-server-9.0.0/alerta/static/embed.js` & `alerta-server-9.0.1/alerta/static/embed.js`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/tasks.py` & `alerta-server-9.0.1/alerta/tasks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/templates/index.html` & `alerta-server-9.0.1/alerta/templates/index.html`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/templates/management/switchboard.html` & `alerta-server-9.0.1/alerta/templates/management/switchboard.html`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/templates/oembed/counts.html` & `alerta-server-9.0.1/alerta/templates/oembed/counts.html`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/api.py` & `alerta-server-9.0.1/alerta/utils/api.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/audit.py` & `alerta-server-9.0.1/alerta/utils/audit.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/client.py` & `alerta-server-9.0.1/alerta/utils/client.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/config.py` & `alerta-server-9.0.1/alerta/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             or os.environ.get('MONGODB_URI', None)
             or os.environ.get('MONGOHQ_URL', None)
             or os.environ.get('MONGOLAB_URI', None)
         )
         # Use app config for DATABASE_URL if no env var from above override it
         config['DATABASE_URL'] = get_config('DATABASE_URL', default=database_url, type=str, config=config)
         config['DATABASE_NAME'] = get_config('DATABASE_NAME', default=None, type=str, config=config)
+        config['DATABASE_SCHEMA'] = get_config('DATABASE_SCHEMA', default='public', type=str, config=config)
 
         config['AUTH_REQUIRED'] = get_config('AUTH_REQUIRED', default=None, type=bool, config=config)
         config['AUTH_PROVIDER'] = get_config('AUTH_PROVIDER', default=None, type=str, config=config)
         config['ADMIN_USERS'] = get_config('ADMIN_USERS', default=[], type=list, config=config)
         config['SIGNUP_ENABLED'] = get_config('SIGNUP_ENABLED', default=True, type=bool, config=config)
         config['CUSTOMER_VIEWS'] = get_config('CUSTOMER_VIEWS', default=False, type=bool, config=config)
```

### Comparing `alerta-server-9.0.0/alerta/utils/format.py` & `alerta-server-9.0.1/alerta/utils/format.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/hooks.py` & `alerta-server-9.0.1/alerta/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/key.py` & `alerta-server-9.0.1/alerta/utils/key.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/logging.py` & `alerta-server-9.0.1/alerta/utils/logging.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/mailer.py` & `alerta-server-9.0.1/alerta/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/paging.py` & `alerta-server-9.0.1/alerta/utils/paging.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/plugin.py` & `alerta-server-9.0.1/alerta/utils/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
                 if plugin:
                     self.plugins[name] = plugin()
                     LOG.info(f"Server plugin '{name}' loaded.")
             except Exception as e:
                 LOG.error(f"Failed to load plugin '{name}': {str(e)}")
         LOG.info(f"All server plugins enabled: {', '.join(self.plugins.keys())}")
         try:
-            self.rules = load_entry_point('alerta-routing', 'alerta.routing', 'rules')  # type: ignore
+            routing_dist = self.config['ROUTING_DIST']
+            self.rules = load_entry_point(routing_dist, 'alerta.routing', 'rules')  # type: ignore
         except (DistributionNotFound, ImportError):
             LOG.info('No plugin routing rules found. All plugins will be evaluated.')
 
     def routing(self, alert: 'Alert') -> 'Tuple[Iterable[PluginBase], Config]':
         try:
             if self.plugins and self.rules:
                 try:
```

### Comparing `alerta-server-9.0.0/alerta/utils/response.py` & `alerta-server-9.0.1/alerta/utils/response.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/tracing.py` & `alerta-server-9.0.1/alerta/utils/tracing.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/utils/webhook.py` & `alerta-server-9.0.1/alerta/utils/webhook.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/__init__.py` & `alerta-server-9.0.1/alerta/views/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/alerts.py` & `alerta-server-9.0.1/alerta/views/alerts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/blackouts.py` & `alerta-server-9.0.1/alerta/views/blackouts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/bulk.py` & `alerta-server-9.0.1/alerta/views/bulk.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/config.py` & `alerta-server-9.0.1/alerta/views/config.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/customers.py` & `alerta-server-9.0.1/alerta/views/customers.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/groups.py` & `alerta-server-9.0.1/alerta/views/groups.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/heartbeats.py` & `alerta-server-9.0.1/alerta/views/heartbeats.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/keys.py` & `alerta-server-9.0.1/alerta/views/keys.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/oembed.py` & `alerta-server-9.0.1/alerta/views/oembed.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/permissions.py` & `alerta-server-9.0.1/alerta/views/permissions.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/views/users.py` & `alerta-server-9.0.1/alerta/views/users.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/__init__.py` & `alerta-server-9.0.1/alerta/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/cloudwatch.py` & `alerta-server-9.0.1/alerta/webhooks/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/custom.py` & `alerta-server-9.0.1/alerta/webhooks/custom.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/grafana.py` & `alerta-server-9.0.1/alerta/webhooks/grafana.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/graylog.py` & `alerta-server-9.0.1/alerta/webhooks/graylog.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/newrelic.py` & `alerta-server-9.0.1/alerta/webhooks/newrelic.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/pagerduty.py` & `alerta-server-9.0.1/alerta/webhooks/pagerduty.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/pingdom.py` & `alerta-server-9.0.1/alerta/webhooks/pingdom.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/prometheus.py` & `alerta-server-9.0.1/alerta/webhooks/prometheus.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/riemann.py` & `alerta-server-9.0.1/alerta/webhooks/riemann.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/serverdensity.py` & `alerta-server-9.0.1/alerta/webhooks/serverdensity.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/slack.py` & `alerta-server-9.0.1/alerta/webhooks/slack.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/stackdriver.py` & `alerta-server-9.0.1/alerta/webhooks/stackdriver.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta/webhooks/telegram.py` & `alerta-server-9.0.1/alerta/webhooks/telegram.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta_server.egg-info/PKG-INFO` & `alerta-server-9.0.1/alerta_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alerta-server
-Version: 9.0.0
+Version: 9.0.1
 Summary: Alerta server WSGI application
 Home-page: https://github.com/guardian/alerta
 Author: Nick Satterly
 Author-email: nfsatterly@gmail.com
 License: Apache License 2.0
 Keywords: alert monitoring system wsgi application api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alerta-server-9.0.0/alerta_server.egg-info/SOURCES.txt` & `alerta-server-9.0.1/alerta_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/alerta_server.egg-info/entry_points.txt` & `alerta-server-9.0.1/alerta_server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/setup.py` & `alerta-server-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/helpers/utils.py` & `alerta-server-9.0.1/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_actions.py` & `alerta-server-9.0.1/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_aggregations.py` & `alerta-server-9.0.1/tests/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_alerts.py` & `alerta-server-9.0.1/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_auth.py` & `alerta-server-9.0.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_authproxy.py` & `alerta-server-9.0.1/tests/test_authproxy.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_blackouts.py` & `alerta-server-9.0.1/tests/test_blackouts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_builtins.py` & `alerta-server-9.0.1/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_commands.py` & `alerta-server-9.0.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_config.py` & `alerta-server-9.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_cors.py` & `alerta-server-9.0.1/tests/test_cors.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_customers.py` & `alerta-server-9.0.1/tests/test_customers.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_forwarder.py` & `alerta-server-9.0.1/tests/test_forwarder.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_groups.py` & `alerta-server-9.0.1/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_heartbeats.py` & `alerta-server-9.0.1/tests/test_heartbeats.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_hooks.py` & `alerta-server-9.0.1/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_isa_18_2.py` & `alerta-server-9.0.1/tests/test_isa_18_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,14 +362,88 @@
         self.assertEqual(response.status_code, 200)
         response = self.client.get('/alert/' + alert_id)
         self.assertEqual(response.status_code, 200)
         data = json.loads(response.data.decode('utf-8'))
         self.assertEqual(data['alert']['severity'], 'OK')
         self.assertEqual(data['alert']['status'], 'NORM')
 
+    def test_operator_unack(self):
+
+        # Create OK alarm
+        response = self.client.post('/alert', data=json.dumps(self.ok_alarm), content_type='application/json')
+        self.assertEqual(response.status_code, 201)
+        data = json.loads(response.data.decode('utf-8'))
+
+        alert_id = data['id']
+
+        # Alarm Occurs, Normal (A) -> Unack (B)
+        response = self.client.post('/alert', data=json.dumps(self.high_alarm), content_type='application/json')
+        self.assertEqual(response.status_code, 201)
+        data = json.loads(response.data.decode('utf-8'))
+        self.assertIn(alert_id, data['alert']['id'])
+        self.assertEqual(data['alert']['resource'], 'LIC_101')
+        self.assertEqual(data['alert']['event'], 'HI_ALM')
+        self.assertEqual(data['alert']['environment'], 'Production')
+        self.assertEqual(data['alert']['severity'], 'High')
+        self.assertEqual(data['alert']['status'], 'UNACK')
+        self.assertEqual(data['alert']['service'], ['REACTORS'])
+        self.assertEqual(data['alert']['group'], 'PROCESS')
+        self.assertEqual(data['alert']['value'], '13')
+        self.assertEqual(data['alert']['text'], 'High Alarm Limit 10')
+        self.assertEqual(data['alert']['tags'], [])
+        self.assertEqual(data['alert']['attributes'], {})
+        self.assertEqual(data['alert']['origin'], 'PID1')
+        self.assertEqual(data['alert']['type'], 'ALARM')
+        self.assertEqual(data['alert']['duplicateCount'], 0)
+        self.assertEqual(data['alert']['repeat'], False)
+        self.assertEqual(data['alert']['previousSeverity'], alarm_model.DEFAULT_PREVIOUS_SEVERITY)
+        self.assertEqual(data['alert']['trendIndication'], 'moreSevere')
+
+        # Operator Ack, Unack (B) -> Ack (C)
+        data = {
+            'action': 'ack',
+            'text': 'operator ack'
+        }
+        response = self.client.put('/alert/' + alert_id + '/action',
+                                   data=json.dumps(data), content_type='application/json')
+        self.assertEqual(response.status_code, 200)
+        response = self.client.get('/alert/' + alert_id)
+        self.assertEqual(response.status_code, 200)
+        data = json.loads(response.data.decode('utf-8'))
+        self.assertEqual(data['alert']['severity'], 'High')
+        self.assertEqual(data['alert']['status'], 'ACKED')
+
+        # Operator Unack, Ack (C) -> Unack (B)
+        data = {
+            'action': 'unack',
+            'text': 'operator unack'
+        }
+        response = self.client.put('/alert/' + alert_id + '/action',
+                                   data=json.dumps(data), content_type='application/json')
+        self.assertEqual(response.status_code, 200)
+        response = self.client.get('/alert/' + alert_id)
+        self.assertEqual(response.status_code, 200)
+        data = json.loads(response.data.decode('utf-8'))
+        self.assertEqual(data['alert']['severity'], 'High')
+        self.assertEqual(data['alert']['status'], 'UNACK')
+
+        # Operator Ack (again), Unack (B) -> Ack (C)
+        data = {
+            'action': 'ack',
+            'text': 'operator ack'
+        }
+        response = self.client.put('/alert/' + alert_id + '/action',
+                                   data=json.dumps(data), content_type='application/json')
+        self.assertEqual(response.status_code, 200)
+        response = self.client.get('/alert/' + alert_id)
+        self.assertEqual(response.status_code, 200)
+        data = json.loads(response.data.decode('utf-8'))
+        self.assertEqual(data['alert']['severity'], 'High')
+        self.assertEqual(data['alert']['status'], 'ACKED')
+
     def test_operator_shelve(self):
 
         # Create OK alarm
         response = self.client.post('/alert', data=json.dumps(self.ok_alarm), content_type='application/json')
         self.assertEqual(response.status_code, 201)
         data = json.loads(response.data.decode('utf-8'))
```

### Comparing `alerta-server-9.0.0/tests/test_logging.py` & `alerta-server-9.0.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_management.py` & `alerta-server-9.0.1/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_metrics.py` & `alerta-server-9.0.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_notes.py` & `alerta-server-9.0.1/tests/test_notes.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_plugins.py` & `alerta-server-9.0.1/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_providers.py` & `alerta-server-9.0.1/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_queryparser.py` & `alerta-server-9.0.1/tests/test_queryparser.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_response.py` & `alerta-server-9.0.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_scopes.py` & `alerta-server-9.0.1/tests/test_scopes.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_search.py` & `alerta-server-9.0.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_severity.py` & `alerta-server-9.0.1/tests/test_severity.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_shelving.py` & `alerta-server-9.0.1/tests/test_shelving.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_tags.py` & `alerta-server-9.0.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_users.py` & `alerta-server-9.0.1/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_webhooks.py` & `alerta-server-9.0.1/tests/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.0/tests/test_zrouting.py` & `alerta-server-9.0.1/tests/test_zrouting.py`

 * *Files identical despite different names*

