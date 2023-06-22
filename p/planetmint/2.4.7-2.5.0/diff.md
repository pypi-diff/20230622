# Comparing `tmp/planetmint-2.4.7.tar.gz` & `tmp/planetmint-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint-2.4.7.tar", max compression
+gzip compressed data, was "planetmint-2.5.0.tar", max compression
```

## Comparing `planetmint-2.4.7.tar` & `planetmint-2.5.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    34523 2023-05-24 19:51:59.714740 planetmint-2.4.7/LICENSE
--rw-r--r--   0        0        0     1614 2023-05-24 19:51:59.714740 planetmint-2.4.7/LICENSES.md
--rw-r--r--   0        0        0     3126 2023-05-24 19:51:59.714740 planetmint-2.4.7/README.md
--rw-r--r--   0        0        0     1796 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/README.md
--rw-r--r--   0        0        0      205 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/abci/__init__.py
--rw-r--r--   0        0        0    10923 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/abci/application_logic.py
--rw-r--r--   0        0        0      104 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/abci/block.py
--rw-r--r--   0        0        0     4896 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/abci/parallel_validation.py
--rw-r--r--   0        0        0     2994 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/abci/rpc.py
--rw-r--r--   0        0        0     5260 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/abci/utils.py
--rw-r--r--   0        0        0       86 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/application/__init__.py
--rw-r--r--   0        0        0      833 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/application/basevalidationrules.py
--rw-r--r--   0        0        0    23610 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/application/validator.py
--rw-r--r--   0        0        0     2319 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/README.md
--rw-r--r--   0        0        0      705 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/__init__.py
--rw-r--r--   0        0        0     4464 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/connection.py
--rw-r--r--   0        0        0      891 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/exceptions.py
--rw-r--r--   0        0        0     1192 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/localmongodb/__init__.py
--rw-r--r--   0        0        0     6300 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/localmongodb/connection.py
--rw-r--r--   0        0        0     9498 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/localmongodb/query.py
--rw-r--r--   0        0        0     2995 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/localmongodb/schema.py
--rw-r--r--   0        0        0      438 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/models/__init__.py
--rw-r--r--   0        0        0      938 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/models/asset.py
--rw-r--r--   0        0        0      727 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/models/block.py
--rw-r--r--   0        0        0     3050 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/models/dbtransaction.py
--rw-r--r--   0        0        0      446 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/models/fulfills.py
--rw-r--r--   0        0        0     1971 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/models/input.py
--rw-r--r--   0        0        0      603 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/models/metadata.py
--rw-r--r--   0        0        0     3597 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/models/output.py
--rw-r--r--   0        0        0      600 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/models/script.py
--rw-r--r--   0        0        0    10645 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/query.py
--rw-r--r--   0        0        0     4516 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/schema.py
--rw-r--r--   0        0        0      127 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/tarantool/__init__.py
--rw-r--r--   0        0        0      917 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/tarantool/const.py
--rw-r--r--   0        0        0    13774 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/tarantool/opt/init.lua
--rw-r--r--   0        0        0        0 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/tarantool/sync_io/__init__.py
--rw-r--r--   0        0        0     2714 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/tarantool/sync_io/connection.py
--rw-r--r--   0        0        0    19154 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/tarantool/sync_io/query.py
--rw-r--r--   0        0        0     1154 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/tarantool/sync_io/schema.py
--rw-r--r--   0        0        0      916 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/tarantool/tarantool.md
--rw-r--r--   0        0        0     1123 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/backend/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/commands/__init__.py
--rw-r--r--   0        0        0     1015 2023-05-24 19:51:59.730740 planetmint-2.4.7/planetmint/commands/election_types.py
--rw-r--r--   0        0        0    14264 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/commands/planetmint.py
--rw-r--r--   0        0        0     4976 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/commands/utils.py
--rw-r--r--   0        0        0     6645 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/config.py
--rw-r--r--   0        0        0    12361 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/config_utils.py
--rw-r--r--   0        0        0      401 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/const.py
--rw-r--r--   0        0        0      390 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/ipc/__init__.py
--rw-r--r--   0        0        0      951 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/ipc/events.py
--rw-r--r--   0        0        0     2195 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/ipc/exchange.py
--rw-r--r--   0        0        0        0 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/model/__init__.py
--rw-r--r--   0        0        0    14133 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/model/dataaccessor.py
--rw-r--r--   0        0        0     3461 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/start.py
--rw-r--r--   0        0        0        0 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/utils/__init__.py
--rw-r--r--   0        0        0     1153 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/utils/lazy.py
--rw-r--r--   0        0        0     2253 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/utils/processes.py
--rw-r--r--   0        0        0      261 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/utils/python.py
--rw-r--r--   0        0        0      239 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/utils/singleton.py
--rw-r--r--   0        0        0      327 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/version.py
--rw-r--r--   0        0        0        0 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/__init__.py
--rw-r--r--   0        0        0     1341 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/routes.py
--rw-r--r--   0        0        0     3671 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/server.py
--rw-r--r--   0        0        0      947 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/strip_content_type_middleware.py
--rw-r--r--   0        0        0        0 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/assets.py
--rw-r--r--   0        0        0     1525 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/base.py
--rw-r--r--   0        0        0     2345 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/blocks.py
--rw-r--r--   0        0        0     1817 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/info.py
--rw-r--r--   0        0        0     1428 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/metadata.py
--rw-r--r--   0        0        0     1464 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/outputs.py
--rw-r--r--   0        0        0     1631 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/parameters.py
--rw-r--r--   0        0        0     4789 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/transactions.py
--rw-r--r--   0        0        0      677 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/views/validators.py
--rw-r--r--   0        0        0     3548 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/websocket_dispatcher.py
--rw-r--r--   0        0        0     4906 2023-05-24 19:51:59.734740 planetmint-2.4.7/planetmint/web/websocket_server.py
--rw-r--r--   0        0        0     2664 2023-05-24 19:51:59.734740 planetmint-2.4.7/pyproject.toml
--rw-r--r--   0        0        0     4926 1970-01-01 00:00:00.000000 planetmint-2.4.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-21 10:17:03.586302 planetmint-2.5.0/LICENSE
+-rw-r--r--   0        0        0     1614 2023-06-21 10:17:03.586302 planetmint-2.5.0/LICENSES.md
+-rw-r--r--   0        0        0     3126 2023-06-21 10:17:03.586302 planetmint-2.5.0/README.md
+-rw-r--r--   0        0        0     1796 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/README.md
+-rw-r--r--   0        0        0      205 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/abci/__init__.py
+-rw-r--r--   0        0        0    10923 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/abci/application_logic.py
+-rw-r--r--   0        0        0      104 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/abci/block.py
+-rw-r--r--   0        0        0     4896 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/abci/parallel_validation.py
+-rw-r--r--   0        0        0     2994 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/abci/rpc.py
+-rw-r--r--   0        0        0     5260 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/abci/utils.py
+-rw-r--r--   0        0        0       86 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/application/__init__.py
+-rw-r--r--   0        0        0      833 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/application/basevalidationrules.py
+-rw-r--r--   0        0        0    23610 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/application/validator.py
+-rw-r--r--   0        0        0     2319 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/README.md
+-rw-r--r--   0        0        0      705 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/__init__.py
+-rw-r--r--   0        0        0     4464 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/connection.py
+-rw-r--r--   0        0        0      891 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/localmongodb/__init__.py
+-rw-r--r--   0        0        0     6300 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/localmongodb/connection.py
+-rw-r--r--   0        0        0     9498 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/localmongodb/query.py
+-rw-r--r--   0        0        0     2995 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/localmongodb/schema.py
+-rw-r--r--   0        0        0      438 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/models/__init__.py
+-rw-r--r--   0        0        0      938 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/models/asset.py
+-rw-r--r--   0        0        0      727 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/models/block.py
+-rw-r--r--   0        0        0     3050 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/models/dbtransaction.py
+-rw-r--r--   0        0        0      446 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/models/fulfills.py
+-rw-r--r--   0        0        0     1971 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/models/input.py
+-rw-r--r--   0        0        0      603 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/models/metadata.py
+-rw-r--r--   0        0        0     3597 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/models/output.py
+-rw-r--r--   0        0        0      600 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/models/script.py
+-rw-r--r--   0        0        0    10645 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/query.py
+-rw-r--r--   0        0        0     4516 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/schema.py
+-rw-r--r--   0        0        0      127 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/tarantool/__init__.py
+-rw-r--r--   0        0        0      917 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/tarantool/const.py
+-rw-r--r--   0        0        0    13774 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/tarantool/opt/init.lua
+-rw-r--r--   0        0        0        0 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/tarantool/sync_io/__init__.py
+-rw-r--r--   0        0        0     2714 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/tarantool/sync_io/connection.py
+-rw-r--r--   0        0        0    19154 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/tarantool/sync_io/query.py
+-rw-r--r--   0        0        0     1154 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/tarantool/sync_io/schema.py
+-rw-r--r--   0        0        0      916 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/tarantool/tarantool.md
+-rw-r--r--   0        0        0     1123 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/backend/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/commands/__init__.py
+-rw-r--r--   0        0        0     1015 2023-06-21 10:17:03.602302 planetmint-2.5.0/planetmint/commands/election_types.py
+-rw-r--r--   0        0        0    14264 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/commands/planetmint.py
+-rw-r--r--   0        0        0     4976 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/commands/utils.py
+-rw-r--r--   0        0        0     6645 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/config.py
+-rw-r--r--   0        0        0    12361 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/config_utils.py
+-rw-r--r--   0        0        0      401 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/const.py
+-rw-r--r--   0        0        0      390 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/ipc/__init__.py
+-rw-r--r--   0        0        0      951 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/ipc/events.py
+-rw-r--r--   0        0        0     2195 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/ipc/exchange.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/model/__init__.py
+-rw-r--r--   0        0        0    14133 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/model/dataaccessor.py
+-rw-r--r--   0        0        0     3461 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/start.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/utils/lazy.py
+-rw-r--r--   0        0        0     2253 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/utils/processes.py
+-rw-r--r--   0        0        0      261 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/utils/python.py
+-rw-r--r--   0        0        0      239 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/utils/singleton.py
+-rw-r--r--   0        0        0      327 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/version.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/__init__.py
+-rw-r--r--   0        0        0     1341 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/routes.py
+-rw-r--r--   0        0        0     3671 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/server.py
+-rw-r--r--   0        0        0      947 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/strip_content_type_middleware.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/__init__.py
+-rw-r--r--   0        0        0     1240 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/assets.py
+-rw-r--r--   0        0        0     1525 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/base.py
+-rw-r--r--   0        0        0     2345 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/blocks.py
+-rw-r--r--   0        0        0     1817 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/info.py
+-rw-r--r--   0        0        0     1428 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/metadata.py
+-rw-r--r--   0        0        0     1464 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/outputs.py
+-rw-r--r--   0        0        0     1631 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/parameters.py
+-rw-r--r--   0        0        0     4789 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/transactions.py
+-rw-r--r--   0        0        0      677 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/views/validators.py
+-rw-r--r--   0        0        0     3548 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/websocket_dispatcher.py
+-rw-r--r--   0        0        0     4906 2023-06-21 10:17:03.606302 planetmint-2.5.0/planetmint/web/websocket_server.py
+-rw-r--r--   0        0        0     2696 2023-06-21 10:17:03.606302 planetmint-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4937 1970-01-01 00:00:00.000000 planetmint-2.5.0/PKG-INFO
```

### Comparing `planetmint-2.4.7/LICENSE` & `planetmint-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/LICENSES.md` & `planetmint-2.5.0/LICENSES.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/README.md` & `planetmint-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/README.md` & `planetmint-2.5.0/planetmint/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/abci/application_logic.py` & `planetmint-2.5.0/planetmint/abci/application_logic.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/abci/parallel_validation.py` & `planetmint-2.5.0/planetmint/abci/parallel_validation.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/abci/rpc.py` & `planetmint-2.5.0/planetmint/abci/rpc.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/abci/utils.py` & `planetmint-2.5.0/planetmint/abci/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/application/basevalidationrules.py` & `planetmint-2.5.0/planetmint/application/basevalidationrules.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/application/validator.py` & `planetmint-2.5.0/planetmint/application/validator.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/README.md` & `planetmint-2.5.0/planetmint/backend/README.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/__init__.py` & `planetmint-2.5.0/planetmint/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/connection.py` & `planetmint-2.5.0/planetmint/backend/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/exceptions.py` & `planetmint-2.5.0/planetmint/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/localmongodb/__init__.py` & `planetmint-2.5.0/planetmint/backend/localmongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/localmongodb/connection.py` & `planetmint-2.5.0/planetmint/backend/localmongodb/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/localmongodb/query.py` & `planetmint-2.5.0/planetmint/backend/localmongodb/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/localmongodb/schema.py` & `planetmint-2.5.0/planetmint/backend/localmongodb/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/models/asset.py` & `planetmint-2.5.0/planetmint/backend/models/asset.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/models/block.py` & `planetmint-2.5.0/planetmint/backend/models/block.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/models/dbtransaction.py` & `planetmint-2.5.0/planetmint/backend/models/dbtransaction.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/models/input.py` & `planetmint-2.5.0/planetmint/backend/models/input.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/models/metadata.py` & `planetmint-2.5.0/planetmint/backend/models/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/models/output.py` & `planetmint-2.5.0/planetmint/backend/models/output.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/models/script.py` & `planetmint-2.5.0/planetmint/backend/models/script.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/query.py` & `planetmint-2.5.0/planetmint/backend/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/schema.py` & `planetmint-2.5.0/planetmint/backend/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/tarantool/const.py` & `planetmint-2.5.0/planetmint/backend/tarantool/const.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/tarantool/opt/init.lua` & `planetmint-2.5.0/planetmint/backend/tarantool/opt/init.lua`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/tarantool/sync_io/connection.py` & `planetmint-2.5.0/planetmint/backend/tarantool/sync_io/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/tarantool/sync_io/query.py` & `planetmint-2.5.0/planetmint/backend/tarantool/sync_io/query.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/tarantool/sync_io/schema.py` & `planetmint-2.5.0/planetmint/backend/tarantool/sync_io/schema.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/tarantool/tarantool.md` & `planetmint-2.5.0/planetmint/backend/tarantool/tarantool.md`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/backend/utils.py` & `planetmint-2.5.0/planetmint/backend/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/commands/election_types.py` & `planetmint-2.5.0/planetmint/commands/election_types.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/commands/planetmint.py` & `planetmint-2.5.0/planetmint/commands/planetmint.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/commands/utils.py` & `planetmint-2.5.0/planetmint/commands/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/config.py` & `planetmint-2.5.0/planetmint/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 "advertised_scheme": "ws",
                 "advertised_host": "localhost",
                 "advertised_port": 9985,
             },
             "tendermint": {
                 "host": "localhost",
                 "port": 26657,
-                "version": "v0.34.15",  # look for __tm_supported_versions__
+                "version": "v0.34.24",  # look for __tm_supported_versions__
             },
             "database": self.__private_database_map,
             "log": {
                 "file": self.log_config["handlers"]["file"]["filename"],
                 "error_file": self.log_config["handlers"]["errors"]["filename"],
                 "level_console": logging.getLevelName(self.log_config["handlers"]["console"]["level"]).lower(),
                 "level_logfile": logging.getLevelName(self.log_config["handlers"]["file"]["level"]).lower(),
```

### Comparing `planetmint-2.4.7/planetmint/config_utils.py` & `planetmint-2.5.0/planetmint/config_utils.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/ipc/events.py` & `planetmint-2.5.0/planetmint/ipc/events.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/ipc/exchange.py` & `planetmint-2.5.0/planetmint/ipc/exchange.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/model/dataaccessor.py` & `planetmint-2.5.0/planetmint/model/dataaccessor.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/start.py` & `planetmint-2.5.0/planetmint/start.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/utils/lazy.py` & `planetmint-2.5.0/planetmint/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/utils/processes.py` & `planetmint-2.5.0/planetmint/utils/processes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/routes.py` & `planetmint-2.5.0/planetmint/web/routes.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/server.py` & `planetmint-2.5.0/planetmint/web/server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/strip_content_type_middleware.py` & `planetmint-2.5.0/planetmint/web/strip_content_type_middleware.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/views/assets.py` & `planetmint-2.5.0/planetmint/web/views/assets.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/views/base.py` & `planetmint-2.5.0/planetmint/web/views/base.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/views/blocks.py` & `planetmint-2.5.0/planetmint/web/views/blocks.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/views/info.py` & `planetmint-2.5.0/planetmint/web/views/info.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/views/metadata.py` & `planetmint-2.5.0/planetmint/web/views/metadata.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/views/outputs.py` & `planetmint-2.5.0/planetmint/web/views/outputs.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/views/parameters.py` & `planetmint-2.5.0/planetmint/web/views/parameters.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/views/transactions.py` & `planetmint-2.5.0/planetmint/web/views/transactions.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/views/validators.py` & `planetmint-2.5.0/planetmint/web/views/validators.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/websocket_dispatcher.py` & `planetmint-2.5.0/planetmint/web/websocket_dispatcher.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/planetmint/web/websocket_server.py` & `planetmint-2.5.0/planetmint/web/websocket_server.py`

 * *Files identical despite different names*

### Comparing `planetmint-2.4.7/pyproject.toml` & `planetmint-2.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "planetmint"
-version = "2.4.7"
+version = "2.5.0"
 description = "Planetmint: The Blockchain Database"
 authors = ["Planetmint contributors"]
 license = "AGPLv3"
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -43,15 +43,15 @@
 nest-asyncio = "1.5.5"
 protobuf = "3.20.2"
 planetmint-ipld = ">=0.0.3"
 pyasn1 = ">=0.4.8"
 python-decouple = "^3.7"
 planetmint-transactions = ">=0.8.1"
 asynctnt = "^2.0.1"
-abci = "^0.8.3"
+planetmint-abci = "^0.8.4"
 
 [tool.poetry.group.dev.dependencies]
 aafigure = "0.6"
 alabaster = "0.7.12"
 babel = "2.10.1"
 certifi = "2022.12.7"
 charset-normalizer = "2.0.12"
@@ -103,11 +103,12 @@
 pytest = ">=3.0.0"
 pytest-cov = "2.8.1"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.1.0"
 pytest-flask = "^1.2.0"
 pytest-aiohttp = "^1.0.4"
 pytest-asyncio = "^0.20.3"
+pip-audit = "^2.5.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `planetmint-2.4.7/PKG-INFO` & `planetmint-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmint
-Version: 2.4.7
+Version: 2.5.0
 Summary: Planetmint: The Blockchain Database
 License: AGPLv3
 Author: Planetmint contributors
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,27 +15,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development
-Requires-Dist: abci (>=0.8.3,<0.9.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asynctnt (>=2.0.1,<3.0.0)
 Requires-Dist: base58 (==2.1.1)
 Requires-Dist: chardet (==3.0.4)
 Requires-Dist: flask (==2.1.2)
 Requires-Dist: flask-cors (==3.0.10)
 Requires-Dist: flask-restful (==0.3.9)
 Requires-Dist: gunicorn (==20.1.0)
 Requires-Dist: jsonschema (==4.16.0)
 Requires-Dist: logstats (==0.3.0)
 Requires-Dist: nest-asyncio (==1.5.5)
 Requires-Dist: packaging (>=22.0)
+Requires-Dist: planetmint-abci (>=0.8.4,<0.9.0)
 Requires-Dist: planetmint-ipld (>=0.0.3)
 Requires-Dist: planetmint-transactions (>=0.8.1)
 Requires-Dist: protobuf (==3.20.2)
 Requires-Dist: pyasn1 (>=0.4.8)
 Requires-Dist: pymongo (==3.11.4)
 Requires-Dist: python-decouple (>=3.7,<4.0)
 Requires-Dist: python-rapidjson (>=1.0)
```

