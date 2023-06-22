# Comparing `tmp/dbt-core-1.6.0b4.tar.gz` & `tmp/dbt-core-1.6.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.6.0b4.tar", last modified: Tue Jun 13 21:43:40 2023, max compression
+gzip compressed data, was "dbt-core-1.6.0b5.tar", last modified: Thu Jun 22 20:11:20 2023, max compression
```

## Comparing `dbt-core-1.6.0b4.tar` & `dbt-core-1.6.0b5.tar`

### file list

```diff
@@ -1,333 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.510118 dbt-core-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-13 21:43:40.510118 dbt-core-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.434117 dbt-core-1.6.0b4/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.438117 dbt-core-1.6.0b4/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.438117 dbt-core-1.6.0b4/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    56619 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.442117 dbt-core-1.6.0b4/dbt/adapters/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/relation_configs/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/relation_configs/config_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/relation_configs/config_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.442117 dbt-core-1.6.0b4/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.442117 dbt-core-1.6.0b4/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.446117 dbt-core-1.6.0b4/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22186 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.446117 dbt-core-1.6.0b4/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    25258 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.450117 dbt-core-1.6.0b4/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    59435 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.454117 dbt-core-1.6.0b4/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.454117 dbt-core-1.6.0b4/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51957 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    53202 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/semantic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22493 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/publication.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.458117 dbt-core-1.6.0b4/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.422117 dbt-core-1.6.0b4/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.458117 dbt-core-1.6.0b4/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.458117 dbt-core-1.6.0b4/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.462118 dbt-core-1.6.0b4/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    62857 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   105442 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    79884 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.462118 dbt-core-1.6.0b4/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.462118 dbt-core-1.6.0b4/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.466117 dbt-core-1.6.0b4/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.466117 dbt-core-1.6.0b4/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.426117 dbt-core-1.6.0b4/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.470117 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/drop_relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.470117 dbt-core-1.6.0b4/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.470117 dbt-core-1.6.0b4/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.474118 dbt-core-1.6.0b4/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.474118 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.426117 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.474118 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.478118 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.478118 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.478118 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.478118 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.482118 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.482118 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.482118 dbt-core-1.6.0b4/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.490118 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.426117 dbt-core-1.6.0b4/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.490118 dbt-core-1.6.0b4/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497953 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.490118 dbt-core-1.6.0b4/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.490118 dbt-core-1.6.0b4/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.490118 dbt-core-1.6.0b4/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.430117 dbt-core-1.6.0b4/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.490118 dbt-core-1.6.0b4/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.490118 dbt-core-1.6.0b4/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.494118 dbt-core-1.6.0b4/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.494118 dbt-core-1.6.0b4/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.498118 dbt-core-1.6.0b4/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    78441 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    51437 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19960 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38214 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.506118 dbt-core-1.6.0b4/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.506118 dbt-core-1.6.0b4/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.506118 dbt-core-1.6.0b4/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:40.510118 dbt-core-1.6.0b4/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-13 21:43:40.000000 dbt-core-1.6.0b4/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-06-13 21:43:40.000000 dbt-core-1.6.0b4/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:43:40.000000 dbt-core-1.6.0b4/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 21:43:40.000000 dbt-core-1.6.0b4/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:43:40.000000 dbt-core-1.6.0b4/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 21:43:40.000000 dbt-core-1.6.0b4/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 21:43:40.000000 dbt-core-1.6.0b4/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:43:40.510118 dbt-core-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-13 21:43:21.000000 dbt-core-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.467325 dbt-core-1.6.0b5/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.467325 dbt-core-1.6.0b5/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.471325 dbt-core-1.6.0b5/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56679 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.471325 dbt-core-1.6.0b5/dbt/adapters/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.471325 dbt-core-1.6.0b5/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.471325 dbt-core-1.6.0b5/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.475325 dbt-core-1.6.0b5/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22301 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.475325 dbt-core-1.6.0b5/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.475325 dbt-core-1.6.0b5/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59340 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.479325 dbt-core-1.6.0b5/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.479325 dbt-core-1.6.0b5/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51708 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/node_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52874 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/semantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/publication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.479325 dbt-core-1.6.0b5/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.459325 dbt-core-1.6.0b5/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62836 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115702 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80024 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.483325 dbt-core-1.6.0b5/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.463325 dbt-core-1.6.0b5/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/drop_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.487325 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.463325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.491325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.495325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.495325 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.495325 dbt-core-1.6.0b5/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.463325 dbt-core-1.6.0b5/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497953 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.463325 dbt-core-1.6.0b5/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.499325 dbt-core-1.6.0b5/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.503325 dbt-core-1.6.0b5/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70786 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51456 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18815 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 20:11:20.000000 dbt-core-1.6.0b5/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:11:20.507325 dbt-core-1.6.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-22 20:11:03.000000 dbt-core-1.6.0b5/setup.py
```

### Comparing `dbt-core-1.6.0b4/PKG-INFO` & `dbt-core-1.6.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b4
+Version: 1.6.0b5
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b4 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b5 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b4/README.md` & `dbt-core-1.6.0b5/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/base/__init__.py` & `dbt-core-1.6.0b5/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/base/column.py` & `dbt-core-1.6.0b5/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/base/connections.py` & `dbt-core-1.6.0b5/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/base/impl.py` & `dbt-core-1.6.0b5/dbt/adapters/base/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
         """Get the set of schema relations that the cache logic needs to
         populate. This means only executable nodes are included.
         """
         # the cache only cares about executable nodes
         return {
             self.Relation.create_from(self.config, node).without_identifier()
             for node in manifest.nodes.values()
-            if (node.is_relational and not node.is_ephemeral_model)
+            if (node.is_relational and not node.is_ephemeral_model and not node.is_external_node)
         }
 
     def _get_catalog_schemas(self, manifest: Manifest) -> SchemaSearchMap:
         """Get a mapping of each node's "information_schema" relations to a
         set of all schemas expected in that information_schema.
 
         There may be keys that are technically duplicates on the database side,
@@ -411,15 +411,15 @@
         # result is a map whose keys are information_schema Relations without
         # identifiers that have appropriate database prefixes, and whose values
         # are sets of lowercase schema names that are valid members of those
         # databases
         return info_schema_name_map
 
     def _relations_cache_for_schemas(
-        self, manifest: Manifest, cache_schemas: Set[BaseRelation] = None
+        self, manifest: Manifest, cache_schemas: Optional[Set[BaseRelation]] = None
     ) -> None:
         """Populate the relations cache for the given schemas. Returns an
         iterable of the schemas populated, as strings.
         """
         if not cache_schemas:
             cache_schemas = self._get_cache_schemas(manifest)
         with executor(self.config) as tpe:
@@ -447,15 +447,15 @@
             cache_update.add((relation.database, relation.schema))
         self.cache.update_schemas(cache_update)
 
     def set_relations_cache(
         self,
         manifest: Manifest,
         clear: bool = False,
-        required_schemas: Set[BaseRelation] = None,
+        required_schemas: Optional[Set[BaseRelation]] = None,
     ) -> None:
         """Run a query that gets a populated cache of the relations in the
         database and set the cache on this adapter.
         """
         with self.cache.lock:
             if clear:
                 self.cache.clear()
@@ -982,15 +982,15 @@
     ###
     def execute_macro(
         self,
         macro_name: str,
         manifest: Optional[Manifest] = None,
         project: Optional[str] = None,
         context_override: Optional[Dict[str, Any]] = None,
-        kwargs: Dict[str, Any] = None,
+        kwargs: Optional[Dict[str, Any]] = None,
         text_only_columns: Optional[Iterable[str]] = None,
     ) -> AttrDict:
         """Look macro_name up in the manifest and execute its results.
 
         :param macro_name: The name of the macro to execute.
         :param manifest: The manifest to use for generating the base macro
             execution context. If none is provided, use the internal manifest.
```

### Comparing `dbt-core-1.6.0b4/dbt/adapters/base/meta.py` & `dbt-core-1.6.0b5/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/base/plugin.py` & `dbt-core-1.6.0b5/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/base/query_headers.py` & `dbt-core-1.6.0b5/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/base/relation.py` & `dbt-core-1.6.0b5/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/cache.py` & `dbt-core-1.6.0b5/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/factory.py` & `dbt-core-1.6.0b5/dbt/adapters/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Type
 
 from dbt.adapters.base.plugin import AdapterPlugin
 from dbt.adapters.protocol import AdapterConfig, AdapterProtocol, RelationProtocol
 from dbt.contracts.connection import AdapterRequiredConfig, Credentials
 from dbt.events.functions import fire_event
-from dbt.events.types import AdapterImportError, PluginLoadError
+from dbt.events.types import AdapterImportError, PluginLoadError, AdapterRegistered
 from dbt.exceptions import DbtInternalError, DbtRuntimeError
 from dbt.include.global_project import PACKAGE_PATH as GLOBAL_PROJECT_PATH
 from dbt.include.global_project import PROJECT_NAME as GLOBAL_PROJECT_NAME
+from dbt.semver import VersionSpecifier
 
 Adapter = AdapterProtocol
 
 
 class AdapterContainer:
     def __init__(self):
         self.lock = threading.Lock()
@@ -85,15 +86,21 @@
             self.load_plugin(dep)
 
         return plugin.credentials
 
     def register_adapter(self, config: AdapterRequiredConfig) -> None:
         adapter_name = config.credentials.type
         adapter_type = self.get_adapter_class_by_name(adapter_name)
-
+        adapter_version = import_module(f".{adapter_name}.__version__", "dbt.adapters").version
+        adapter_version_specifier = VersionSpecifier.from_version_string(
+            adapter_version
+        ).to_version_string()
+        fire_event(
+            AdapterRegistered(adapter_name=adapter_name, adapter_version=adapter_version_specifier)
+        )
         with self.lock:
             if adapter_name in self.adapters:
                 # this shouldn't really happen...
                 return
 
             adapter: Adapter = adapter_type(config)  # type: ignore
             self.adapters[adapter_name] = adapter
```

### Comparing `dbt-core-1.6.0b4/dbt/adapters/protocol.py` & `dbt-core-1.6.0b5/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/reference_keys.py` & `dbt-core-1.6.0b5/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/relation_configs/config_base.py` & `dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/relation_configs/config_change.py` & `dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_change.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/relation_configs/config_validation.py` & `dbt-core-1.6.0b5/dbt/adapters/relation_configs/config_validation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/sql/connections.py` & `dbt-core-1.6.0b5/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/adapters/sql/impl.py` & `dbt-core-1.6.0b5/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/cli/exceptions.py` & `dbt-core-1.6.0b5/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/cli/flags.py` & `dbt-core-1.6.0b5/dbt/cli/flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,17 @@
     return sub_command_ctx
 
 
 @dataclass(frozen=True)
 class Flags:
     """Primary configuration artifact for running dbt"""
 
-    def __init__(self, ctx: Context = None, user_config: UserConfig = None) -> None:
+    def __init__(
+        self, ctx: Optional[Context] = None, user_config: Optional[UserConfig] = None
+    ) -> None:
 
         # Set the default flags.
         for key, value in FLAGS_DEFAULTS.items():
             object.__setattr__(self, key, value)
 
         if ctx is None:
             ctx = get_current_context()
```

### Comparing `dbt-core-1.6.0b4/dbt/cli/main.py` & `dbt-core-1.6.0b5/dbt/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     ] = None
 
 
 # Programmatic invocation
 class dbtRunner:
     def __init__(
         self,
-        manifest: Manifest = None,
-        callbacks: List[Callable[[EventMsg], None]] = None,
+        manifest: Optional[Manifest] = None,
+        callbacks: Optional[List[Callable[[EventMsg], None]]] = None,
     ):
         self.manifest = manifest
 
         if callbacks is None:
             callbacks = []
         self.callbacks = callbacks
```

### Comparing `dbt-core-1.6.0b4/dbt/cli/option_types.py` & `dbt-core-1.6.0b5/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/cli/options.py` & `dbt-core-1.6.0b5/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/cli/params.py` & `dbt-core-1.6.0b5/dbt/cli/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     help="Whether or not to run 'dbt compile' as part of docs generation",
     default=True,
 )
 
 config_dir = click.option(
     "--config-dir",
     envvar=None,
-    help="Show the configured location for the profiles.yml file and exit",
+    help="Print a system-specific command to access the directory that the current dbt project is searching for a profiles.yml. Then, exit. This flag renders other debug step flags no-ops.",
     is_flag=True,
 )
 
 debug = click.option(
     "--debug/--no-debug",
     "-d/ ",
     envvar="DBT_DEBUG",
```

### Comparing `dbt-core-1.6.0b4/dbt/cli/requires.py` & `dbt-core-1.6.0b5/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/cli/resolvers.py` & `dbt-core-1.6.0b5/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/cli/types.py` & `dbt-core-1.6.0b5/dbt/cli/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/clients/_jinja_blocks.py` & `dbt-core-1.6.0b5/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/clients/agate_helper.py` & `dbt-core-1.6.0b5/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/clients/git.py` & `dbt-core-1.6.0b5/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/clients/jinja.py` & `dbt-core-1.6.0b5/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/clients/jinja_static.py` & `dbt-core-1.6.0b5/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/clients/registry.py` & `dbt-core-1.6.0b5/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/clients/system.py` & `dbt-core-1.6.0b5/dbt/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/clients/yaml_helper.py` & `dbt-core-1.6.0b5/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/compilation.py` & `dbt-core-1.6.0b5/dbt/compilation.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,17 @@
                 self.dependency(node.unique_id, (manifest.metrics[dependency].unique_id))
             else:
                 raise GraphDependencyNotFoundError(node, dependency)
 
     def link_graph(self, manifest: Manifest):
         for source in manifest.sources.values():
             self.add_node(source.unique_id)
+        for semantic_node in manifest.semantic_nodes.values():
+            self.add_node(semantic_node.unique_id)
+
         for node in manifest.nodes.values():
             self.link_node(node, manifest)
         for exposure in manifest.exposures.values():
             self.link_node(exposure, manifest)
         for metric in manifest.metrics.values():
             self.link_node(metric, manifest)
```

### Comparing `dbt-core-1.6.0b4/dbt/config/profile.py` & `dbt-core-1.6.0b5/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/config/project.py` & `dbt-core-1.6.0b5/dbt/config/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from typing_extensions import Protocol, runtime_checkable
 
 import os
 
 from dbt.flags import get_flags
 from dbt import deprecations
+from dbt.constants import DEPENDENCIES_FILE_NAME, PACKAGES_FILE_NAME
 from dbt.clients.system import path_exists, resolve_path_from_base, load_file_contents
 from dbt.clients.yaml_helper import load_yaml_text
 from dbt.contracts.connection import QueryComment
 from dbt.exceptions import (
     DbtProjectError,
     SemverError,
     ProjectContractBrokenError,
@@ -34,14 +35,15 @@
 from dbt.node_types import NodeType
 from dbt.config.selectors import SelectorDict
 from dbt.contracts.project import (
     Project as ProjectContract,
     SemverString,
 )
 from dbt.contracts.project import PackageConfig, ProjectPackageMetadata
+from dbt.contracts.publication import ProjectDependencies
 from dbt.dataclass_schema import ValidationError
 from .renderer import DbtProjectYamlRenderer, PackageRenderer
 from .selectors import (
     selector_config_from_data,
     selector_data_from_root,
     SelectorConfig,
 )
@@ -89,36 +91,73 @@
 
 
 def _load_yaml(path):
     contents = load_file_contents(path)
     return load_yaml_text(contents)
 
 
-def package_data_from_root(project_root):
-    package_filepath = resolve_path_from_base("packages.yml", project_root)
+def package_and_project_data_from_root(project_root):
+    package_filepath = resolve_path_from_base(PACKAGES_FILE_NAME, project_root)
+    dependencies_filepath = resolve_path_from_base(DEPENDENCIES_FILE_NAME, project_root)
 
+    packages_yml_dict = {}
+    dependencies_yml_dict = {}
     if path_exists(package_filepath):
-        packages_dict = _load_yaml(package_filepath)
-    else:
-        packages_dict = None
-    return packages_dict
+        packages_yml_dict = _load_yaml(package_filepath) or {}
+    if path_exists(dependencies_filepath):
+        dependencies_yml_dict = _load_yaml(dependencies_filepath) or {}
+
+    if "packages" in packages_yml_dict and "packages" in dependencies_yml_dict:
+        msg = "The 'packages' key cannot be specified in both packages.yml and dependencies.yml"
+        raise DbtProjectError(msg)
+    if "projects" in packages_yml_dict:
+        msg = "The 'projects' key cannot be specified in packages.yml"
+        raise DbtProjectError(msg)
+
+    packages_specified_path = PACKAGES_FILE_NAME
+    packages_dict = {}
+    dependent_projects_dict = {}
+    if "packages" in dependencies_yml_dict:
+        packages_dict["packages"] = dependencies_yml_dict["packages"]
+        packages_specified_path = DEPENDENCIES_FILE_NAME
+    else:  # don't check for "packages" here so we capture invalid keys in packages.yml
+        packages_dict = packages_yml_dict
+    if "projects" in dependencies_yml_dict:
+        dependent_projects_dict["projects"] = dependencies_yml_dict["projects"]
 
+    return packages_dict, dependent_projects_dict, packages_specified_path
 
-def package_config_from_data(packages_data: Dict[str, Any]):
+
+def package_config_from_data(packages_data: Dict[str, Any]) -> PackageConfig:
     if not packages_data:
         packages_data = {"packages": []}
 
     try:
         PackageConfig.validate(packages_data)
         packages = PackageConfig.from_dict(packages_data)
     except ValidationError as e:
         raise DbtProjectError(MALFORMED_PACKAGE_ERROR.format(error=str(e.message))) from e
     return packages
 
 
+def dependent_project_config_from_data(
+    dependent_projects_data: Dict[str, Any]
+) -> ProjectDependencies:
+    if not dependent_projects_data:
+        dependent_projects_data = {"projects": []}
+
+    try:
+        ProjectDependencies.validate(dependent_projects_data)
+        dependent_projects = ProjectDependencies.from_dict(dependent_projects_data)
+    except ValidationError as e:
+        msg = f"Malformed dependencies.yml: {e}"
+        raise DbtProjectError(msg)
+    return dependent_projects
+
+
 def _parse_versions(versions: Union[List[str], str]) -> List[VersionSpecifier]:
     """Parse multiple versions as read from disk. The versions value may be any
     one of:
         - a single version string ('>0.12.1')
         - a single string specifying multiple comma-separated versions
             ('>0.11.1,<=0.12.2')
         - an array of single-version strings (['>0.11.1', '<=0.12.2'])
@@ -235,19 +274,23 @@
     return dbt_version
 
 
 @dataclass
 class RenderComponents:
     project_dict: Dict[str, Any] = field(metadata=dict(description="The project dictionary"))
     packages_dict: Dict[str, Any] = field(metadata=dict(description="The packages dictionary"))
+    dependent_projects_dict: Dict[str, Any] = field(
+        metadata=dict(description="The dependent projects dictionary")
+    )
     selectors_dict: Dict[str, Any] = field(metadata=dict(description="The selectors dictionary"))
 
 
 @dataclass
 class PartialProject(RenderComponents):
+    # This class includes the project_dict, packages_dict, selectors_dict, etc from RenderComponents
     profile_name: Optional[str] = field(
         metadata=dict(description="The unrendered profile name in the project, if set")
     )
     project_name: Optional[str] = field(
         metadata=dict(
             description=(
                 "The name of the project. This should always be set and will not be rendered"
@@ -256,36 +299,45 @@
     )
     project_root: str = field(
         metadata=dict(description="The root directory of the project"),
     )
     verify_version: bool = field(
         metadata=dict(description=("If True, verify the dbt version matches the required version"))
     )
+    packages_specified_path: str = field(
+        metadata=dict(description="The filename where packages were specified")
+    )
 
     def render_profile_name(self, renderer) -> Optional[str]:
         if self.profile_name is None:
             return None
         return renderer.render_value(self.profile_name)
 
     def get_rendered(
         self,
         renderer: DbtProjectYamlRenderer,
     ) -> RenderComponents:
 
         rendered_project = renderer.render_project(self.project_dict, self.project_root)
-        rendered_packages = renderer.render_packages(self.packages_dict)
+        rendered_packages = renderer.render_packages(
+            self.packages_dict, self.packages_specified_path
+        )
+        rendered_dependent_projects = renderer.render_dependent_projects(
+            self.dependent_projects_dict
+        )
         rendered_selectors = renderer.render_selectors(self.selectors_dict)
 
         return RenderComponents(
             project_dict=rendered_project,
             packages_dict=rendered_packages,
+            dependent_projects_dict=rendered_dependent_projects,
             selectors_dict=rendered_selectors,
         )
 
-    # Called by 'collect_parts' in RuntimeConfig
+    # Called by Project.from_project_root (not PartialProject.from_project_root!)
     def render(self, renderer: DbtProjectYamlRenderer) -> "Project":
         try:
             rendered = self.get_rendered(renderer)
             return self.create_project(rendered)
         except DbtProjectError as exc:
             if exc.path is None:
                 exc.path = os.path.join(self.project_root, "dbt_project.yml")
@@ -320,14 +372,15 @@
                     kwargs.update({"exp_path": expected_path})
                 deprecations.warn(f"project-config-{deprecated_path}", **kwargs)
 
     def create_project(self, rendered: RenderComponents) -> "Project":
         unrendered = RenderComponents(
             project_dict=self.project_dict,
             packages_dict=self.packages_dict,
+            dependent_projects_dict=self.dependent_projects_dict,
             selectors_dict=self.selectors_dict,
         )
         dbt_version = _get_required_version(
             rendered.project_dict,
             verify_version=self.verify_version,
         )
 
@@ -420,15 +473,18 @@
         # There will never be any project_env_vars when it's first created
         project_env_vars: Dict[str, Any] = {}
         on_run_start: List[str] = value_or(cfg.on_run_start, [])
         on_run_end: List[str] = value_or(cfg.on_run_end, [])
 
         query_comment = _query_comment_from_cfg(cfg.query_comment)
 
-        packages = package_config_from_data(rendered.packages_dict)
+        packages: PackageConfig = package_config_from_data(rendered.packages_dict)
+        dependent_projects: ProjectDependencies = dependent_project_config_from_data(
+            rendered.dependent_projects_dict
+        )
         selectors = selector_config_from_data(rendered.selectors_dict)
         manifest_selectors: Dict[str, Any] = {}
         if rendered.selectors_dict and rendered.selectors_dict["selectors"]:
             # this is a dict with a single key 'selectors' pointing to a list
             # of dicts.
             manifest_selectors = SelectorDict.parse_from_selectors_list(
                 rendered.selectors_dict["selectors"]
@@ -446,23 +502,25 @@
             docs_paths=docs_paths,
             asset_paths=asset_paths,
             target_path=target_path,
             snapshot_paths=snapshot_paths,
             clean_targets=clean_targets,
             log_path=log_path,
             packages_install_path=packages_install_path,
+            packages_specified_path=self.packages_specified_path,
             quoting=quoting,
             models=models,
             on_run_start=on_run_start,
             on_run_end=on_run_end,
             dispatch=dispatch,
             seeds=seeds,
             snapshots=snapshots,
             dbt_version=dbt_version,
             packages=packages,
+            dependent_projects=dependent_projects,
             manifest_selectors=manifest_selectors,
             selectors=selectors,
             query_comment=query_comment,
             sources=sources,
             tests=tests,
             metrics=metrics,
             exposures=exposures,
@@ -477,46 +535,57 @@
 
     @classmethod
     def from_dicts(
         cls,
         project_root: str,
         project_dict: Dict[str, Any],
         packages_dict: Dict[str, Any],
+        dependent_projects_dict: Dict[str, Any],
         selectors_dict: Dict[str, Any],
         *,
         verify_version: bool = False,
+        packages_specified_path: str = PACKAGES_FILE_NAME,
     ):
         """Construct a partial project from its constituent dicts."""
         project_name = project_dict.get("name")
         profile_name = project_dict.get("profile")
 
+        # Create a PartialProject
         return cls(
             profile_name=profile_name,
             project_name=project_name,
             project_root=project_root,
             project_dict=project_dict,
             packages_dict=packages_dict,
+            dependent_projects_dict=dependent_projects_dict,
             selectors_dict=selectors_dict,
             verify_version=verify_version,
+            packages_specified_path=packages_specified_path,
         )
 
     @classmethod
     def from_project_root(
         cls, project_root: str, *, verify_version: bool = False
     ) -> "PartialProject":
         project_root = os.path.normpath(project_root)
         project_dict = load_raw_project(project_root)
-        packages_dict = package_data_from_root(project_root)
+        (
+            packages_dict,
+            dependent_projects_dict,
+            packages_specified_path,
+        ) = package_and_project_data_from_root(project_root)
         selectors_dict = selector_data_from_root(project_root)
         return cls.from_dicts(
             project_root=project_root,
             project_dict=project_dict,
             selectors_dict=selectors_dict,
             packages_dict=packages_dict,
+            dependent_projects_dict=dependent_projects_dict,
             verify_version=verify_version,
+            packages_specified_path=packages_specified_path,
         )
 
 
 class VarProvider:
     """Var providers are tied to a particular Project."""
 
     def __init__(self, vars: Dict[str, Dict[str, Any]]) -> None:
@@ -548,28 +617,30 @@
     docs_paths: List[str]
     asset_paths: List[str]
     target_path: str
     snapshot_paths: List[str]
     clean_targets: List[str]
     log_path: str
     packages_install_path: str
+    packages_specified_path: str
     quoting: Dict[str, Any]
     models: Dict[str, Any]
     on_run_start: List[str]
     on_run_end: List[str]
     dispatch: List[Dict[str, Any]]
     seeds: Dict[str, Any]
     snapshots: Dict[str, Any]
     sources: Dict[str, Any]
     tests: Dict[str, Any]
     metrics: Dict[str, Any]
     exposures: Dict[str, Any]
     vars: VarProvider
     dbt_version: List[VersionSpecifier]
-    packages: Dict[str, Any]
+    packages: PackageConfig
+    dependent_projects: ProjectDependencies
     manifest_selectors: Dict[str, Any]
     selectors: SelectorConfig
     query_comment: QueryComment
     config_version: int
     unrendered: RenderComponents
     project_env_vars: Dict[str, Any]
 
@@ -659,14 +730,17 @@
     @classmethod
     def partial_load(cls, project_root: str, *, verify_version: bool = False) -> PartialProject:
         return PartialProject.from_project_root(
             project_root,
             verify_version=verify_version,
         )
 
+    # Called by:
+    # RtConfig.load_dependencies => RtConfig.load_projects => RtConfig.new_project => Project.from_project_root
+    # RtConfig.from_args => RtConfig.collect_parts => load_project => Project.from_project_root
     @classmethod
     def from_project_root(
         cls,
         project_root: str,
         renderer: DbtProjectYamlRenderer,
         *,
         verify_version: bool = False,
```

### Comparing `dbt-core-1.6.0b4/dbt/config/renderer.py` & `dbt-core-1.6.0b5/dbt/config/renderer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Any, Tuple, Optional, Union, Callable
 import re
 import os
 from datetime import date
 
 from dbt.clients.jinja import get_rendered, catch_jinja
-from dbt.constants import SECRET_ENV_PREFIX
+from dbt.constants import SECRET_ENV_PREFIX, DEPENDENCIES_FILE_NAME
 from dbt.context.target import TargetContext
 from dbt.context.secret import SecretContext, SECRET_PLACEHOLDER
 from dbt.context.base import BaseContext
 from dbt.contracts.connection import HasCredentials
 from dbt.exceptions import DbtProjectError, CompilationError, RecursionError
 from dbt.utils import deep_map_render
 
@@ -128,18 +128,27 @@
         project_root: str,
     ) -> Dict[str, Any]:
         """Render the project and insert the project root after rendering."""
         rendered_project = self.render_data(project)
         rendered_project["project-root"] = project_root
         return rendered_project
 
-    def render_packages(self, packages: Dict[str, Any]):
+    def render_packages(self, packages: Dict[str, Any], packages_specified_path: str):
         """Render the given packages dict"""
+        packages = packages or {}  # Sometimes this is none in tests
         package_renderer = self.get_package_renderer()
-        return package_renderer.render_data(packages)
+        if packages_specified_path == DEPENDENCIES_FILE_NAME:
+            # We don't want to render the "packages" dictionary that came from dependencies.yml
+            return packages
+        else:
+            return package_renderer.render_data(packages)
+
+    def render_dependent_projects(self, dependent_projects: Dict[str, Any]):
+        """This is a no-op to maintain regularity in the interfaces. We don't render dependencies.yml."""
+        return dependent_projects
 
     def render_selectors(self, selectors: Dict[str, Any]):
         return self.render_data(selectors)
 
     def render_entry(self, value: Any, keypath: Keypath) -> Any:
         result = super().render_entry(value, keypath)
         return self._KEYPATH_HANDLERS.postprocess(result, keypath)
```

### Comparing `dbt-core-1.6.0b4/dbt/config/runtime.py` & `dbt-core-1.6.0b5/dbt/config/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 )
 from dbt.helper_types import DictDefaultEmptyStr, FQNPath, PathSet
 from .profile import Profile
 from .project import Project
 from .renderer import DbtProjectYamlRenderer, ProfileRenderer
 
 
+# Called by RuntimeConfig.collect_parts class method
 def load_project(
     project_root: str,
     version_check: bool,
     profile: HasCredentials,
     cli_vars: Optional[Dict[str, Any]] = None,
 ) -> Project:
     # get the project with all of the provided information
@@ -146,23 +147,25 @@
             docs_paths=project.docs_paths,
             asset_paths=project.asset_paths,
             target_path=project.target_path,
             snapshot_paths=project.snapshot_paths,
             clean_targets=project.clean_targets,
             log_path=project.log_path,
             packages_install_path=project.packages_install_path,
+            packages_specified_path=project.packages_specified_path,
             quoting=quoting,
             models=project.models,
             on_run_start=project.on_run_start,
             on_run_end=project.on_run_end,
             dispatch=project.dispatch,
             seeds=project.seeds,
             snapshots=project.snapshots,
             dbt_version=project.dbt_version,
             packages=project.packages,
+            dependent_projects=project.dependent_projects,
             manifest_selectors=project.manifest_selectors,
             selectors=project.selectors,
             query_comment=project.query_comment,
             sources=project.sources,
             tests=project.tests,
             metrics=project.metrics,
             exposures=project.exposures,
@@ -232,29 +235,30 @@
         :raises DbtProjectError: If the configuration fails validation.
         """
         try:
             Configuration.validate(self.serialize())
         except ValidationError as e:
             raise ConfigContractBrokenError(e) from e
 
+    # Called by RuntimeConfig.from_args
     @classmethod
     def collect_parts(cls: Type["RuntimeConfig"], args: Any) -> Tuple[Project, Profile]:
         # profile_name from the project
         project_root = args.project_dir if args.project_dir else os.getcwd()
         cli_vars: Dict[str, Any] = getattr(args, "vars", {})
         profile = cls.get_profile(
             project_root,
             cli_vars,
             args,
         )
         flags = get_flags()
         project = load_project(project_root, bool(flags.VERSION_CHECK), profile, cli_vars)
         return project, profile
 
-    # Called in main.py, lib.py, task/base.py
+    # Called in task/base.py, in BaseTask.from_args
     @classmethod
     def from_args(cls, args: Any) -> "RuntimeConfig":
         """Given arguments, read in dbt_project.yml from the current directory,
         read in packages.yml if it exists, and use them to find the profile to
         load.
 
         :param args: The arguments as parsed from the cli.
@@ -358,14 +362,15 @@
                 # raise exception if fewer installed packages than in packages.yml
                 count_packages_specified = len(self.packages.packages)  # type: ignore
                 count_packages_installed = len(tuple(self._get_project_directories()))
                 if count_packages_specified > count_packages_installed:
                     raise UninstalledPackagesFoundError(
                         count_packages_specified,
                         count_packages_installed,
+                        self.packages_specified_path,
                         self.packages_install_path,
                     )
                 project_paths = itertools.chain(internal_packages, self._get_project_directories())
             for project_name, project in self.load_projects(project_paths):
                 if project_name in all_projects:
                     raise NonUniquePackageNameError(project_name)
                 all_projects[project_name] = project
```

### Comparing `dbt-core-1.6.0b4/dbt/config/selectors.py` & `dbt-core-1.6.0b5/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/config/utils.py` & `dbt-core-1.6.0b5/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/context/base.py` & `dbt-core-1.6.0b5/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/context/configured.py` & `dbt-core-1.6.0b5/dbt/context/configured.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,17 @@
 
     @contextproperty
     def var(self) -> ConfiguredVar:
         return ConfiguredVar(self._ctx, self.config, self.config.project_name)
 
 
 def generate_schema_yml_context(
-    config: AdapterRequiredConfig, project_name: str, schema_yaml_vars: SchemaYamlVars = None
+    config: AdapterRequiredConfig,
+    project_name: str,
+    schema_yaml_vars: Optional[SchemaYamlVars] = None,
 ) -> Dict[str, Any]:
     ctx = SchemaYamlContext(config, project_name, schema_yaml_vars)
     return ctx.to_dict()
 
 
 def generate_macro_context(
     config: AdapterRequiredConfig,
```

### Comparing `dbt-core-1.6.0b4/dbt/context/context_config.py` & `dbt-core-1.6.0b5/dbt/context/context_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import List, Iterator, Dict, Any, TypeVar, Generic
+from typing import List, Iterator, Dict, Any, TypeVar, Generic, Optional
 
 from dbt.config import RuntimeConfig, Project, IsFQNResource
 from dbt.contracts.graph.model_config import BaseConfig, get_config_for, _listify
 from dbt.exceptions import DbtInternalError
 from dbt.node_types import NodeType
 from dbt.utils import fqn_search
 
@@ -126,15 +126,15 @@
     def calculate_node_config(
         self,
         config_call_dict: Dict[str, Any],
         fqn: List[str],
         resource_type: NodeType,
         project_name: str,
         base: bool,
-        patch_config_dict: Dict[str, Any] = None,
+        patch_config_dict: Optional[Dict[str, Any]] = None,
     ) -> BaseConfig:
         own_config = self.get_node_project(project_name)
 
         result = self.initial_result(resource_type=resource_type, base=base)
 
         project_configs = self._project_configs(own_config, fqn, resource_type)
         for fqn_config in project_configs:
@@ -162,15 +162,15 @@
     def calculate_node_config_dict(
         self,
         config_call_dict: Dict[str, Any],
         fqn: List[str],
         resource_type: NodeType,
         project_name: str,
         base: bool,
-        patch_config_dict: Dict[str, Any],
+        patch_config_dict: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
         ...
 
 
 class ContextConfigGenerator(BaseContextConfigGenerator[C]):
     def __init__(self, active_project: RuntimeConfig):
         self._active_project = active_project
@@ -196,15 +196,15 @@
     def calculate_node_config_dict(
         self,
         config_call_dict: Dict[str, Any],
         fqn: List[str],
         resource_type: NodeType,
         project_name: str,
         base: bool,
-        patch_config_dict: dict = None,
+        patch_config_dict: Optional[dict] = None,
     ) -> Dict[str, Any]:
         config = self.calculate_node_config(
             config_call_dict=config_call_dict,
             fqn=fqn,
             resource_type=resource_type,
             project_name=project_name,
             base=base,
@@ -221,15 +221,15 @@
     def calculate_node_config_dict(
         self,
         config_call_dict: Dict[str, Any],
         fqn: List[str],
         resource_type: NodeType,
         project_name: str,
         base: bool,
-        patch_config_dict: dict = None,
+        patch_config_dict: Optional[dict] = None,
     ) -> Dict[str, Any]:
         # TODO CT-211
         return self.calculate_node_config(
             config_call_dict=config_call_dict,
             fqn=fqn,
             resource_type=resource_type,
             project_name=project_name,
@@ -314,15 +314,19 @@
                     # listify everything
                     for key, value in config_call_dict[k].items():
                         config_call_dict[k][key] = _listify(value)
             else:
                 config_call_dict[k] = v
 
     def build_config_dict(
-        self, base: bool = False, *, rendered: bool = True, patch_config_dict: dict = None
+        self,
+        base: bool = False,
+        *,
+        rendered: bool = True,
+        patch_config_dict: Optional[dict] = None,
     ) -> Dict[str, Any]:
         if rendered:
             # TODO CT-211
             src = ContextConfigGenerator(self._active_project)  # type: ignore[var-annotated]
         else:
             # TODO CT-211
             src = UnrenderedConfigGenerator(self._active_project)  # type: ignore[assignment]
```

### Comparing `dbt-core-1.6.0b4/dbt/context/docs.py` & `dbt-core-1.6.0b5/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/context/exceptions_jinja.py` & `dbt-core-1.6.0b5/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/context/macro_resolver.py` & `dbt-core-1.6.0b5/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/context/macros.py` & `dbt-core-1.6.0b5/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/context/manifest.py` & `dbt-core-1.6.0b5/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/context/providers.py` & `dbt-core-1.6.0b5/dbt/context/providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 from dbt.context.macros import MacroNamespaceBuilder, MacroNamespace
 from dbt.context.manifest import ManifestContext
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.graph.manifest import Manifest, Disabled
 from dbt.contracts.graph.nodes import (
     Macro,
     Exposure,
-    Metric,
     SeedNode,
     SourceDefinition,
     Resource,
     ManifestNode,
     RefArgs,
     AccessType,
+    SemanticModel,
 )
 from dbt.contracts.graph.metrics import MetricReference, ResolvedMetricReference
 from dbt.contracts.graph.unparsed import NodeVersion
 from dbt.events.functions import get_metadata_vars
 from dbt.exceptions import (
     CompilationError,
     ConflictingConfigKeysError,
@@ -281,14 +281,15 @@
         if len(args) != 2:
             raise NumberSourceArgsError(args, node=self.model)
         self.validate_args(args[0], args[1])
         return self.resolve(args[0], args[1])
 
 
 class BaseMetricResolver(BaseResolver):
+    @abc.abstractmethod
     def resolve(self, name: str, package: Optional[str] = None) -> MetricReference:
         ...
 
     def _repack_args(self, name: str, package: Optional[str]) -> List[str]:
         if package is None:
             return [name]
         else:
@@ -498,47 +499,43 @@
                 target_package=target_package,
                 target_version=target_version,
                 disabled=isinstance(target_model, Disabled),
             )
         elif (
             target_model.resource_type == NodeType.Model
             and target_model.access == AccessType.Private
+            # don't raise this reference error for ad hoc 'preview' queries
+            and self.model.resource_type != NodeType.SqlOperation
+            and self.model.resource_type != NodeType.RPCCall  # TODO: rm
         ):
             if not self.model.group or self.model.group != target_model.group:
                 raise DbtReferenceError(
                     unique_id=self.model.unique_id,
                     ref_unique_id=target_model.unique_id,
                     group=cast_to_str(target_model.group),
                 )
 
         self.validate(target_model, target_name, target_package, target_version)
         return self.create_relation(target_model)
 
     def create_relation(self, target_model: ManifestNode) -> RelationProxy:
-        if target_model.is_public_node:
-            # Get quoting from publication artifact
-            pub_metadata = self.manifest.publications[target_model.package_name].metadata
-            return self.Relation.create_from_node(pub_metadata, target_model)
-        elif target_model.is_ephemeral_model:
+        if target_model.is_ephemeral_model:
             self.model.set_cte(target_model.unique_id, None)
             return self.Relation.create_ephemeral_from_node(self.config, target_model)
         else:
             return self.Relation.create_from(self.config, target_model)
 
     def validate(
         self,
         resolved: ManifestNode,
         target_name: str,
         target_package: Optional[str],
         target_version: Optional[NodeVersion],
     ) -> None:
-        if (
-            resolved.unique_id not in self.model.depends_on.nodes
-            and resolved.unique_id not in self.model.depends_on.public_nodes
-        ):
+        if resolved.unique_id not in self.model.depends_on.nodes:
             args = self._repack_args(target_name, target_package, target_version)
             raise RefBadContextError(node=self.model, args=args)
 
 
 class OperationRefResolver(RuntimeRefResolver):
     def validate(
         self,
@@ -1530,55 +1527,52 @@
             exposure,
             project,
             manifest,
         ),
     }
 
 
-class MetricRefResolver(BaseResolver):
+# applies to SemanticModels
+class SemanticModelRefResolver(BaseResolver):
     def __call__(self, *args, **kwargs) -> str:
         package = None
         if len(args) == 1:
             name = args[0]
         elif len(args) == 2:
             package, name = args
         else:
             raise RefArgsError(node=self.model, args=args)
 
         version = kwargs.get("version") or kwargs.get("v")
         self.validate_args(name, package, version)
 
+        # "model" here is any node
         self.model.refs.append(RefArgs(package=package, name=name, version=version))
         return ""
 
     def validate_args(self, name, package, version):
         if not isinstance(name, str):
             raise ParsingError(
-                f"In a metrics section in {self.model.original_file_path} "
+                f"In a semantic model or metrics section in {self.model.original_file_path} "
                 "the name argument to ref() must be a string"
             )
 
 
-def generate_parse_metrics(
-    metric: Metric,
+# used for semantic models
+def generate_parse_semantic_models(
+    semantic_model: SemanticModel,
     config: RuntimeConfig,
     manifest: Manifest,
     package_name: str,
 ) -> Dict[str, Any]:
     project = config.load_dependencies()[package_name]
     return {
-        "ref": MetricRefResolver(
-            None,
-            metric,
-            project,
-            manifest,
-        ),
-        "metric": ParseMetricResolver(
+        "ref": SemanticModelRefResolver(
             None,
-            metric,
+            semantic_model,
             project,
             manifest,
         ),
     }
 
 
 # This class is currently used by the schema parser in order
```

### Comparing `dbt-core-1.6.0b4/dbt/context/secret.py` & `dbt-core-1.6.0b5/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/context/target.py` & `dbt-core-1.6.0b5/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/connection.py` & `dbt-core-1.6.0b5/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/files.py` & `dbt-core-1.6.0b5/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/graph/manifest.py` & `dbt-core-1.6.0b5/dbt/contracts/graph/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,26 +18,25 @@
     Generic,
     AbstractSet,
     ClassVar,
 )
 from typing_extensions import Protocol
 from uuid import UUID
 
-from dbt.contracts.publication import ProjectDependencies, PublicationConfig, PublicModel
+from dbt.contracts.publication import PublicationConfig
 
 from dbt.contracts.graph.nodes import (
     BaseNode,
     Documentation,
     Exposure,
     GenericTestNode,
     GraphMemberNode,
     Group,
     Macro,
     ManifestNode,
-    ManifestOrPublicNode,
     Metric,
     ModelNode,
     RelationalNode,
     ResultNode,
     SemanticModel,
     SourceDefinition,
     UnpatchedSourceDefinition,
@@ -158,15 +157,14 @@
     # model, seed, snapshot
     _lookup_types: ClassVar[set] = set(NodeType.refable())
     _versioned_types: ClassVar[set] = set(NodeType.versioned())
 
     def __init__(self, manifest: "Manifest"):
         self.storage: Dict[str, Dict[PackageName, UniqueID]] = {}
         self.populate(manifest)
-        self.populate_public_nodes(manifest)
 
     def get_unique_id(
         self,
         key: str,
         package: Optional[PackageName],
         version: Optional[NodeVersion],
         node: Optional[GraphMemberNode] = None,
@@ -202,15 +200,17 @@
                 and get_node_info()
             ):
                 # Check to see if newer versions are available, and log an "FYI" if so
                 max_version: UnparsedVersion = max(
                     [
                         UnparsedVersion(v.version)
                         for v in manifest.nodes.values()
-                        if v.name == node.name and v.version is not None
+                        if isinstance(v, ModelNode)
+                        and v.name == node.name
+                        and v.version is not None
                     ]
                 )
                 assert node.latest_version is not None  # for mypy, whenever i may find it
                 if max_version > UnparsedVersion(node.latest_version):
                     fire_event(
                         UnpinnedRefNewVersionAvailable(
                             node_info=get_node_info(),
@@ -220,15 +220,15 @@
                             ref_max_version=str(max_version.v),
                         )
                     )
 
             return node
         return None
 
-    def add_node(self, node: ManifestOrPublicNode):
+    def add_node(self, node: ManifestNode):
         if node.resource_type in self._lookup_types:
             if node.name not in self.storage:
                 self.storage[node.name] = {}
 
             if node.is_versioned:
                 if node.search_name not in self.storage:
                     self.storage[node.search_name] = {}
@@ -238,23 +238,17 @@
             else:
                 self.storage[node.name][node.package_name] = node.unique_id
 
     def populate(self, manifest):
         for node in manifest.nodes.values():
             self.add_node(node)
 
-    def populate_public_nodes(self, manifest):
-        for node in manifest.public_nodes.values():
-            self.add_node(node)
-
-    def perform_lookup(self, unique_id: UniqueID, manifest) -> ManifestOrPublicNode:
+    def perform_lookup(self, unique_id: UniqueID, manifest) -> ManifestNode:
         if unique_id in manifest.nodes:
             node = manifest.nodes[unique_id]
-        elif unique_id in manifest.public_nodes:
-            node = manifest.public_nodes[unique_id]
         else:
             raise dbt.exceptions.DbtInternalError(
                 f"Node {unique_id} found in cache but not found in manifest"
             )
         return node
 
     def _find_unique_ids_for_package(self, key, package: Optional[PackageName]) -> List[str]:
@@ -432,15 +426,14 @@
     lists of edges.
     """
     backward_edges: Dict[str, List[str]] = {}
     # pre-populate the forward edge dict for simplicity
     forward_edges: Dict[str, List[str]] = {n.unique_id: [] for n in nodes}
     for node in nodes:
         backward_edges[node.unique_id] = node.depends_on_nodes[:]
-        backward_edges[node.unique_id].extend(node.depends_on_public_nodes[:])
         for unique_id in backward_edges[node.unique_id]:
             if unique_id in forward_edges.keys():
                 forward_edges[unique_id].append(node.unique_id)
     return _sort_values(forward_edges), _sort_values(backward_edges)
 
 
 # Build a map of children of macros and generic tests
@@ -703,16 +696,14 @@
     files: MutableMapping[str, AnySourceFile] = field(default_factory=dict)
     metadata: ManifestMetadata = field(default_factory=ManifestMetadata)
     flat_graph: Dict[str, Any] = field(default_factory=dict)
     state_check: ManifestStateCheck = field(default_factory=ManifestStateCheck)
     source_patches: MutableMapping[SourceKey, SourcePatch] = field(default_factory=dict)
     disabled: MutableMapping[str, List[GraphMemberNode]] = field(default_factory=dict)
     env_vars: MutableMapping[str, str] = field(default_factory=dict)
-    public_nodes: MutableMapping[str, PublicModel] = field(default_factory=dict)
-    project_dependencies: Optional[ProjectDependencies] = None
     publications: MutableMapping[str, PublicationConfig] = field(default_factory=dict)
     semantic_nodes: MutableMapping[str, SemanticModel] = field(default_factory=dict)
 
     _doc_lookup: Optional[DocLookup] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
     _source_lookup: Optional[SourceLookup] = field(
@@ -758,15 +749,17 @@
         """
         self.flat_graph = {
             "exposures": {k: v.to_dict(omit_none=False) for k, v in self.exposures.items()},
             "groups": {k: v.to_dict(omit_none=False) for k, v in self.groups.items()},
             "metrics": {k: v.to_dict(omit_none=False) for k, v in self.metrics.items()},
             "nodes": {k: v.to_dict(omit_none=False) for k, v in self.nodes.items()},
             "sources": {k: v.to_dict(omit_none=False) for k, v in self.sources.items()},
-            "public_nodes": {k: v.to_dict(omit_none=False) for k, v in self.public_nodes.items()},
+            "semantic_nodes": {
+                k: v.to_dict(omit_none=False) for k, v in self.semantic_nodes.items()
+            },
         }
 
     def build_disabled_by_file_id(self):
         disabled_by_file_id = {}
         for node_list in self.disabled.values():
             for node in node_list:
                 disabled_by_file_id[node.file_id] = node
@@ -819,14 +812,15 @@
     def get_resource_fqns(self) -> Mapping[str, PathSet]:
         resource_fqns: Dict[str, Set[Tuple[str, ...]]] = {}
         all_resources = chain(
             self.exposures.values(),
             self.nodes.values(),
             self.sources.values(),
             self.metrics.values(),
+            self.semantic_nodes.values(),
         )
         for resource in all_resources:
             resource_type_plural = resource.resource_type.pluralize()
             if resource_type_plural not in resource_fqns:
                 resource_fqns[resource_type_plural] = set()
             resource_fqns[resource_type_plural].add(tuple(resource.fqn))
         return resource_fqns
@@ -851,29 +845,30 @@
             docs={k: _deepcopy(v) for k, v in self.docs.items()},
             exposures={k: _deepcopy(v) for k, v in self.exposures.items()},
             metrics={k: _deepcopy(v) for k, v in self.metrics.items()},
             groups={k: _deepcopy(v) for k, v in self.groups.items()},
             selectors={k: _deepcopy(v) for k, v in self.selectors.items()},
             metadata=self.metadata,
             disabled={k: _deepcopy(v) for k, v in self.disabled.items()},
-            public_nodes={k: _deepcopy(v) for k, v in self.public_nodes.items()},
             files={k: _deepcopy(v) for k, v in self.files.items()},
             state_check=_deepcopy(self.state_check),
+            publications={k: _deepcopy(v) for k, v in self.publications.items()},
+            semantic_nodes={k: _deepcopy(v) for k, v in self.semantic_nodes.items()},
         )
         copy.build_flat_graph()
         return copy
 
     def build_parent_and_child_maps(self):
         edge_members = list(
             chain(
                 self.nodes.values(),
                 self.sources.values(),
                 self.exposures.values(),
                 self.metrics.values(),
-                self.public_nodes.values(),
+                self.semantic_nodes.values(),
             )
         )
         forward_edges, backward_edges = build_node_edges(edge_members)
         self.child_map = forward_edges
         self.parent_map = backward_edges
 
     def build_macro_child_map(self):
@@ -909,15 +904,14 @@
             docs=self.docs,
             exposures=self.exposures,
             metrics=self.metrics,
             groups=self.groups,
             selectors=self.selectors,
             metadata=self.metadata,
             disabled=self.disabled,
-            public_nodes=self.public_nodes,
             child_map=self.child_map,
             parent_map=self.parent_map,
             group_map=self.group_map,
             semantic_nodes=self.semantic_nodes,
         )
 
     def write(self, path):
@@ -930,14 +924,16 @@
             return self.nodes[unique_id]
         elif unique_id in self.sources:
             return self.sources[unique_id]
         elif unique_id in self.exposures:
             return self.exposures[unique_id]
         elif unique_id in self.metrics:
             return self.metrics[unique_id]
+        elif unique_id in self.semantic_nodes:
+            return self.semantic_nodes[unique_id]
         else:
             # something terrible has happened
             raise dbt.exceptions.DbtInternalError(
                 "Expected node {} not found in manifest".format(unique_id)
             )
 
     @property
@@ -998,16 +994,22 @@
             )
 
         for metric in self.metrics.values():
             pydantic_semantic_manifest.metrics.append(PydanticMetric.parse_obj(metric.to_dict()))
 
         return pydantic_semantic_manifest
 
+    @property
+    def external_node_unique_ids(self):
+        return [node.unique_id for node in self.nodes.values() if node.is_external_node]
+
     def resolve_refs(
-        self, source_node: GraphMemberNode, current_project: str
+        self,
+        source_node: ModelNode,
+        current_project: str,  # TODO: ModelNode is overly restrictive typing
     ) -> List[MaybeNonSource]:
         resolved_refs: List[MaybeNonSource] = []
         for ref in source_node.refs:
             resolved = self.resolve_ref(
                 source_node,
                 ref.name,
                 ref.package,
@@ -1036,17 +1038,15 @@
 
         candidates = _packages_to_search(current_project, node_package, target_model_package)
         for pkg in candidates:
             node = self.ref_lookup.find(
                 target_model_name, pkg, target_model_version, self, source_node
             )
 
-            if node is not None and (
-                (hasattr(node, "config") and node.config.enabled) or node.is_public_node
-            ):
+            if node is not None and hasattr(node, "config") and node.config.enabled:
                 return node
 
             # it's possible that the node is disabled
             if disabled is None:
                 disabled = self.disabled_lookup.find(target_model_name, pkg, target_model_version)
 
         if disabled:
@@ -1293,15 +1293,16 @@
             self.files,
             self.metadata,
             self.flat_graph,
             self.state_check,
             self.source_patches,
             self.disabled,
             self.env_vars,
-            self.public_nodes,
+            self.publications,
+            self.semantic_nodes,
             self._doc_lookup,
             self._source_lookup,
             self._ref_lookup,
             self._metric_lookup,
             self._disabled_lookup,
             self._analysis_lookup,
         )
@@ -1363,17 +1364,14 @@
         )
     )
     group_map: Optional[NodeEdgeMap] = field(
         metadata=dict(
             description="A mapping from group names to their nodes",
         )
     )
-    public_nodes: Mapping[UniqueID, PublicModel] = field(
-        metadata=dict(description=("The public models used in the dbt project"))
-    )
     semantic_nodes: Mapping[UniqueID, SemanticModel] = field(
         metadata=dict(description=("The semantic models defined in the dbt project"))
     )
     metadata: ManifestMetadata = field(
         metadata=dict(
             description="Metadata about the manifest",
         )
```

### Comparing `dbt-core-1.6.0b4/dbt/contracts/graph/manifest_upgrade.py` & `dbt-core-1.6.0b5/dbt/contracts/graph/manifest_upgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,14 @@
             if node_content["resource_type"] == "seed":
                 upgrade_seed_content(node_content)
     # add group key
     if "groups" not in manifest:
         manifest["groups"] = {}
     if "group_map" not in manifest:
         manifest["group_map"] = {}
-    if "public_nodes" not in manifest:
-        manifest["public_nodes"] = {}
     for metric_content in manifest.get("metrics", {}).values():
         # handle attr renames + value translation ("expression" -> "derived")
         metric_content = upgrade_ref_content(metric_content)
         if "root_path" in metric_content:
             del metric_content["root_path"]
     for exposure_content in manifest.get("exposures", {}).values():
         exposure_content = upgrade_ref_content(exposure_content)
```

### Comparing `dbt-core-1.6.0b4/dbt/contracts/graph/metrics.py` & `dbt-core-1.6.0b5/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/graph/model_config.py` & `dbt-core-1.6.0b5/dbt/contracts/graph/model_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/graph/nodes.py` & `dbt-core-1.6.0b5/dbt/contracts/graph/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 import time
 from dataclasses import dataclass, field
 from enum import Enum
 import hashlib
 
 from mashumaro.types import SerializableType
-from typing import Optional, Union, List, Dict, Any, Sequence, Tuple, Iterator, Protocol
+from typing import Optional, Union, List, Dict, Any, Sequence, Tuple, Iterator
 
 from dbt.dataclass_schema import dbtClassMixin, ExtensibleDbtClassMixin
 
 from dbt.clients.system import write_file
 from dbt.contracts.files import FileHash
 from dbt.contracts.graph.semantic_models import (
     Defaults,
@@ -31,14 +31,15 @@
     Quoting,
     TestDef,
     NodeVersion,
     UnparsedSourceDefinition,
     UnparsedSourceTableDefinition,
     UnparsedColumn,
 )
+from dbt.contracts.graph.node_args import ModelNodeArgs
 from dbt.contracts.util import Replaceable, AdditionalPropertiesMixin
 from dbt.events.functions import warn_or_error
 from dbt.exceptions import ParsingError, ContractBreakingChangeError
 from dbt.events.types import (
     SeedIncreased,
     SeedExceedsLimitSamePath,
     SeedExceedsLimitAndPathChanged,
@@ -49,16 +50,15 @@
 from dbt.node_types import ModelLanguage, NodeType, AccessType
 from dbt_semantic_interfaces.references import (
     MeasureReference,
     LinkableElementReference,
     SemanticModelReference,
 )
 from dbt_semantic_interfaces.references import MetricReference as DSIMetricReference
-from dbt_semantic_interfaces.type_enums.metric_type import MetricType
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import MetricType, TimeGranularity
 
 from .model_config import (
     NodeConfig,
     SeedConfig,
     TestConfig,
     SourceConfig,
     MetricConfig,
@@ -265,24 +265,19 @@
     def identifier(self):
         return self.alias
 
 
 @dataclass
 class DependsOn(MacroDependsOn):
     nodes: List[str] = field(default_factory=list)
-    public_nodes: List[str] = field(default_factory=list)
 
     def add_node(self, value: str):
         if value not in self.nodes:
             self.nodes.append(value)
 
-    def add_public_node(self, value: str):
-        if value not in self.public_nodes:
-            self.public_nodes.append(value)
-
 
 @dataclass
 class StateRelation(dbtClassMixin):
     alias: str
     database: Optional[str]
     schema: str
 
@@ -484,15 +479,15 @@
             and self.same_fqn(old)
             and self.same_database_representation(old)
             and same_contract
             and True
         )
 
     @property
-    def is_public_node(self):
+    def is_external_node(self):
         return False
 
 
 @dataclass
 class InjectedCTE(dbtClassMixin, Replaceable):
     """Used in CompiledNodes as part of ephemeral model processing"""
 
@@ -550,18 +545,14 @@
         return dct
 
     @property
     def depends_on_nodes(self):
         return self.depends_on.nodes
 
     @property
-    def depends_on_public_nodes(self):
-        return self.depends_on.public_nodes
-
-    @property
     def depends_on_macros(self):
         return self.depends_on.macros
 
 
 # ====================================
 # CompiledNode subclasses
 # ====================================
@@ -584,14 +575,40 @@
     access: AccessType = AccessType.Protected
     constraints: List[ModelLevelConstraint] = field(default_factory=list)
     version: Optional[NodeVersion] = None
     latest_version: Optional[NodeVersion] = None
     deprecation_date: Optional[datetime] = None
     state_relation: Optional[StateRelation] = None
 
+    @classmethod
+    def from_args(cls, args: ModelNodeArgs) -> "ModelNode":
+        unique_id = f"{NodeType.Model}.{args.package_name}.{args.name}"
+
+        return cls(
+            resource_type=NodeType.Model,
+            name=args.name,
+            package_name=args.package_name,
+            unique_id=unique_id,
+            fqn=[args.package_name, args.name],
+            version=args.version,
+            latest_version=args.latest_version,
+            relation_name=args.relation_name,
+            database=args.database,
+            schema=args.schema,
+            alias=args.identifier,
+            deprecation_date=args.deprecation_date,
+            checksum=FileHash.from_contents(f"{unique_id},{args.generated_at}"),
+            original_file_path="",
+            path="",
+        )
+
+    @property
+    def is_external_node(self) -> bool:
+        return not self.original_file_path and not self.path
+
     @property
     def is_latest_version(self) -> bool:
         return self.version is not None and self.version == self.latest_version
 
     @property
     def search_name(self):
         if self.version is None:
@@ -847,18 +864,14 @@
         return self.same_seeds(other)
 
     @property
     def depends_on_nodes(self):
         return []
 
     @property
-    def depends_on_public_nodes(self):
-        return []
-
-    @property
     def depends_on_macros(self) -> List[str]:
         return self.depends_on.macros
 
     @property
     def extra_ctes(self):
         return []
 
@@ -1178,18 +1191,14 @@
         return False
 
     @property
     def depends_on_nodes(self):
         return []
 
     @property
-    def depends_on_public_nodes(self):
-        return []
-
-    @property
     def depends_on(self):
         return DependsOn(macros=[], nodes=[])
 
     @property
     def refs(self):
         return []
 
@@ -1231,18 +1240,14 @@
     created_at: float = field(default_factory=lambda: time.time())
 
     @property
     def depends_on_nodes(self):
         return self.depends_on.nodes
 
     @property
-    def depends_on_public_nodes(self):
-        return self.depends_on.public_nodes
-
-    @property
     def search_name(self):
         return self.name
 
     def same_depends_on(self, old: "Exposure") -> bool:
         return set(self.depends_on.nodes) == set(old.depends_on.nodes)
 
     def same_description(self, old: "Exposure") -> bool:
@@ -1284,14 +1289,18 @@
             and self.same_description(old)
             and self.same_label(old)
             and self.same_depends_on(old)
             and self.same_config(old)
             and True
         )
 
+    @property
+    def group(self):
+        return None
+
 
 # ====================================
 # Metric node
 # ====================================
 
 
 @dataclass
@@ -1304,15 +1313,15 @@
     name: str
     filter: Optional[WhereFilter] = None
     alias: Optional[str] = None
 
     def measure_reference(self) -> MeasureReference:
         return MeasureReference(element_name=self.name)
 
-    def post_aggregation_measure_referenc(self) -> MeasureReference:
+    def post_aggregation_measure_reference(self) -> MeasureReference:
         return MeasureReference(element_name=self.alias or self.name)
 
 
 @dataclass
 class MetricTimeWindow(dbtClassMixin):
     count: int
     granularity: TimeGranularity
@@ -1325,32 +1334,29 @@
     alias: Optional[str] = None
     offset_window: Optional[MetricTimeWindow] = None
     offset_to_grain: Optional[TimeGranularity] = None
 
     def as_reference(self) -> DSIMetricReference:
         return DSIMetricReference(element_name=self.name)
 
+    def post_aggregation_reference(self) -> DSIMetricReference:
+        return DSIMetricReference(element_name=self.alias or self.name)
+
 
 @dataclass
 class MetricTypeParams(dbtClassMixin):
     measure: Optional[MetricInputMeasure] = None
-    measures: Optional[List[MetricInputMeasure]] = None
-    numerator: Optional[MetricInputMeasure] = None
-    denominator: Optional[MetricInputMeasure] = None
+    input_measures: List[MetricInputMeasure] = field(default_factory=list)
+    numerator: Optional[MetricInput] = None
+    denominator: Optional[MetricInput] = None
     expr: Optional[str] = None
     window: Optional[MetricTimeWindow] = None
     grain_to_date: Optional[TimeGranularity] = None
     metrics: Optional[List[MetricInput]] = None
 
-    def numerator_measure_reference(self) -> Optional[MeasureReference]:
-        return self.numerator.measure_reference() if self.numerator else None
-
-    def denominator_measure_reference(self) -> Optional[MeasureReference]:
-        return self.denominator.measure_reference() if self.denominator else None
-
 
 @dataclass
 class MetricReference(dbtClassMixin, Replaceable):
     sql: Optional[Union[str, int]] = None
     unique_id: Optional[str] = None
 
 
@@ -1376,33 +1382,20 @@
     group: Optional[str] = None
 
     @property
     def depends_on_nodes(self):
         return self.depends_on.nodes
 
     @property
-    def depends_on_public_nodes(self):
-        return self.depends_on.public_nodes
-
-    @property
     def search_name(self):
         return self.name
 
     @property
     def input_measures(self) -> List[MetricInputMeasure]:
-        tp = self.type_params
-        res = tp.measures or []
-        if tp.measure:
-            res.append(tp.measure)
-        if tp.numerator:
-            res.append(tp.numerator)
-        if tp.denominator:
-            res.append(tp.denominator)
-
-        return res
+        return self.type_params.input_measures
 
     @property
     def measure_references(self) -> List[MeasureReference]:
         return [x.measure_reference() for x in self.input_measures]
 
     @property
     def input_metrics(self) -> List[MetricInput]:
@@ -1468,26 +1461,30 @@
 
 
 @dataclass
 class NodeRelation(dbtClassMixin):
     alias: str
     schema_name: str  # TODO: Could this be called simply "schema" so we could reuse StateRelation?
     database: Optional[str] = None
+    relation_name: Optional[str] = None
 
 
 @dataclass
 class SemanticModel(GraphNode):
     model: str
     node_relation: Optional[NodeRelation]
     description: Optional[str] = None
     defaults: Optional[Defaults] = None
     entities: Sequence[Entity] = field(default_factory=list)
     measures: Sequence[Measure] = field(default_factory=list)
     dimensions: Sequence[Dimension] = field(default_factory=list)
     metadata: Optional[SourceFileMetadata] = None
+    depends_on: DependsOn = field(default_factory=DependsOn)
+    refs: List[RefArgs] = field(default_factory=list)
+    created_at: float = field(default_factory=lambda: time.time())
 
     @property
     def entity_references(self) -> List[LinkableElementReference]:
         return [entity.reference for entity in self.entities]
 
     @property
     def dimension_references(self) -> List[LinkableElementReference]:
@@ -1530,14 +1527,22 @@
             return None
         return partitions[0]
 
     @property
     def reference(self) -> SemanticModelReference:
         return SemanticModelReference(semantic_model_name=self.name)
 
+    @property
+    def depends_on_nodes(self):
+        return self.depends_on.nodes
+
+    @property
+    def depends_on_macros(self):
+        return self.depends_on.macros
+
 
 # ====================================
 # Patches
 # ====================================
 
 
 @dataclass
@@ -1568,54 +1573,14 @@
 
 
 # ====================================
 # Node unions/categories
 # ====================================
 
 
-class ManifestOrPublicNode(Protocol):
-    name: str
-    package_name: str
-    unique_id: str
-    version: Optional[NodeVersion]
-    latest_version: Optional[NodeVersion]
-    relation_name: str
-    database: Optional[str]
-    schema: Optional[str]
-    identifier: Optional[str]
-
-    @property
-    def is_latest_version(self):
-        pass
-
-    @property
-    def resource_type(self):
-        pass
-
-    @property
-    def access(self):
-        pass
-
-    @property
-    def search_name(self):
-        pass
-
-    @property
-    def is_public_node(self):
-        pass
-
-    @property
-    def is_versioned(self):
-        pass
-
-    @property
-    def alias(self):
-        pass
-
-
 # ManifestNode without SeedNode, which doesn't have the
 # SQL related attributes
 ManifestSQLNode = Union[
     AnalysisNode,
     SingularTestNode,
     HookNode,
     ModelNode,
@@ -1637,14 +1602,15 @@
 ]
 
 # All nodes that can be in the DAG
 GraphMemberNode = Union[
     ResultNode,
     Exposure,
     Metric,
+    SemanticModel,
 ]
 
 # All "nodes" (or node-like objects) in this file
 Resource = Union[
     GraphMemberNode,
     Documentation,
     Macro,
```

### Comparing `dbt-core-1.6.0b4/dbt/contracts/graph/semantic_models.py` & `dbt-core-1.6.0b5/dbt/contracts/graph/semantic_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from dbt.dataclass_schema import dbtClassMixin
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     EntityReference,
     MeasureReference,
     TimeDimensionReference,
 )
-from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
-from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
-from dbt_semantic_interfaces.type_enums.entity_type import EntityType
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import (
+    AggregationType,
+    DimensionType,
+    EntityType,
+    TimeGranularity,
+)
 from typing import List, Optional
 
 
 @dataclass
 class FileSlice(dbtClassMixin):
     """Provides file slice level context about what something was created from.
```

### Comparing `dbt-core-1.6.0b4/dbt/contracts/graph/unparsed.py` & `dbt-core-1.6.0b5/dbt/contracts/graph/unparsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,17 +612,16 @@
     offset_window: Optional[str] = None
     offset_to_grain: Optional[str] = None  # str is really a TimeGranularity Enum
 
 
 @dataclass
 class UnparsedMetricTypeParams(dbtClassMixin):
     measure: Optional[Union[UnparsedMetricInputMeasure, str]] = None
-    measures: Optional[List[Union[UnparsedMetricInputMeasure, str]]] = None
-    numerator: Optional[Union[UnparsedMetricInputMeasure, str]] = None
-    denominator: Optional[Union[UnparsedMetricInputMeasure, str]] = None
+    numerator: Optional[Union[UnparsedMetricInput, str]] = None
+    denominator: Optional[Union[UnparsedMetricInput, str]] = None
     expr: Optional[str] = None
     window: Optional[str] = None
     grain_to_date: Optional[str] = None  # str is really a TimeGranularity Enum
     metrics: Optional[List[Union[UnparsedMetricInput, str]]] = None
 
 
 @dataclass
```

### Comparing `dbt-core-1.6.0b4/dbt/contracts/graph/utils.py` & `dbt-core-1.6.0b5/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/project.py` & `dbt-core-1.6.0b5/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/publication.py` & `dbt-core-1.6.0b5/dbt/contracts/publication.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from dbt.contracts.util import (
     AdditionalPropertiesMixin,
     ArtifactMixin,
     BaseArtifactMetadata,
     schema_version,
 )
 from dbt.contracts.graph.unparsed import NodeVersion
-from dbt.contracts.graph.nodes import ManifestOrPublicNode
 from dbt.dataclass_schema import dbtClassMixin, ExtensibleDbtClassMixin
-from dbt.node_types import AccessType, NodeType
 
 
 @dataclass
 class ProjectDependency(AdditionalPropertiesMixin, ExtensibleDbtClassMixin):
     name: str
     _extra: Dict[str, Any] = field(default_factory=dict)
 
@@ -33,72 +31,31 @@
         default_factory=lambda: str(PublicationArtifact.dbt_schema_version)
     )
     adapter_type: Optional[str] = None
     quoting: Dict[str, Any] = field(default_factory=dict)
 
 
 @dataclass
-class PublicModel(dbtClassMixin, ManifestOrPublicNode):
+class PublicModel(dbtClassMixin):
     """Used to represent cross-project models"""
 
     name: str
     package_name: str
     unique_id: str
     relation_name: str
+    identifier: str
+    schema: str
     database: Optional[str] = None
-    schema: Optional[str] = None
-    identifier: Optional[str] = None
     version: Optional[NodeVersion] = None
     latest_version: Optional[NodeVersion] = None
     # list of model unique_ids
     public_node_dependencies: List[str] = field(default_factory=list)
     generated_at: datetime = field(default_factory=datetime.utcnow)
     deprecation_date: Optional[datetime] = None
 
-    @property
-    def is_latest_version(self) -> bool:
-        return self.version is not None and self.version == self.latest_version
-
-    # Needed for ref resolution code
-    @property
-    def resource_type(self):
-        return NodeType.Model
-
-    # Needed for ref resolution code
-    @property
-    def access(self):
-        return AccessType.Public
-
-    @property
-    def search_name(self):
-        if self.version is None:
-            return self.name
-        else:
-            return f"{self.name}.v{self.version}"
-
-    @property
-    def depends_on_nodes(self):
-        return []
-
-    @property
-    def depends_on_public_nodes(self):
-        return []
-
-    @property
-    def is_public_node(self):
-        return True
-
-    @property
-    def is_versioned(self):
-        return self.version is not None
-
-    @property
-    def alias(self):
-        return self.identifier
-
 
 @dataclass
 class PublicationMandatory:
     project_name: str
 
 
 @dataclass
```

### Comparing `dbt-core-1.6.0b4/dbt/contracts/relation.py` & `dbt-core-1.6.0b5/dbt/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/results.py` & `dbt-core-1.6.0b5/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/selection.py` & `dbt-core-1.6.0b5/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/sql.py` & `dbt-core-1.6.0b5/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/state.py` & `dbt-core-1.6.0b5/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/contracts/util.py` & `dbt-core-1.6.0b5/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/dataclass_schema.py` & `dbt-core-1.6.0b5/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/deprecations.py` & `dbt-core-1.6.0b5/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/deps/base.py` & `dbt-core-1.6.0b5/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/deps/git.py` & `dbt-core-1.6.0b5/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/deps/local.py` & `dbt-core-1.6.0b5/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/deps/registry.py` & `dbt-core-1.6.0b5/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/deps/resolver.py` & `dbt-core-1.6.0b5/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/deps/tarball.py` & `dbt-core-1.6.0b5/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.6.0b5/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/docs/source/conf.py` & `dbt-core-1.6.0b5/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/events/adapter_endpoint.py` & `dbt-core-1.6.0b5/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/events/base_types.py` & `dbt-core-1.6.0b5/dbt/events/base_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import threading
 from dbt.events import types_pb2
 import sys
 from google.protobuf.json_format import ParseDict, MessageToDict, MessageToJson
 from google.protobuf.message import Message
 from dbt.events.helpers import get_json_string_utcnow
+from typing import Optional
 
 if sys.version_info >= (3, 8):
     from typing import Protocol
 else:
     from typing_extensions import Protocol
 
 
@@ -122,15 +123,15 @@
 
 
 class EventMsg(Protocol):
     info: EventInfo
     data: Message
 
 
-def msg_from_base_event(event: BaseEvent, level: EventLevel = None):
+def msg_from_base_event(event: BaseEvent, level: Optional[EventLevel] = None):
 
     msg_class_name = f"{type(event).__name__}Msg"
     msg_cls = getattr(types_pb2, msg_class_name)
 
     # level in EventInfo must be a string, not an EventLevel
     msg_level: str = level.value if level else event.level_tag().value
     assert msg_level is not None
```

### Comparing `dbt-core-1.6.0b4/dbt/events/contextvars.py` & `dbt-core-1.6.0b5/dbt/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/events/eventmgr.py` & `dbt-core-1.6.0b5/dbt/events/eventmgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 
 class EventManager:
     def __init__(self) -> None:
         self.loggers: List[_Logger] = []
         self.callbacks: List[Callable[[EventMsg], None]] = []
         self.invocation_id: str = str(uuid4())
 
-    def fire_event(self, e: BaseEvent, level: EventLevel = None) -> None:
+    def fire_event(self, e: BaseEvent, level: Optional[EventLevel] = None) -> None:
         msg = msg_from_base_event(e, level=level)
 
         if os.environ.get("DBT_TEST_BINARY_SERIALIZATION"):
             print(f"--- {msg.info.name}")
             try:
                 msg.SerializeToString()
             except Exception as exc:
```

### Comparing `dbt-core-1.6.0b4/dbt/events/format.py` & `dbt-core-1.6.0b5/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/events/functions.py` & `dbt-core-1.6.0b5/dbt/events/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,30 +243,32 @@
     else:
         fire_event(event)
 
 
 # an alternative to fire_event which only creates and logs the event value
 # if the condition is met. Does nothing otherwise.
 def fire_event_if(
-    conditional: bool, lazy_e: Callable[[], BaseEvent], level: EventLevel = None
+    conditional: bool, lazy_e: Callable[[], BaseEvent], level: Optional[EventLevel] = None
 ) -> None:
     if conditional:
         fire_event(lazy_e(), level=level)
 
 
 # a special case of fire_event_if, to only fire events in our unit/functional tests
-def fire_event_if_test(lazy_e: Callable[[], BaseEvent], level: EventLevel = None) -> None:
+def fire_event_if_test(
+    lazy_e: Callable[[], BaseEvent], level: Optional[EventLevel] = None
+) -> None:
     fire_event_if(conditional=("pytest" in sys.modules), lazy_e=lazy_e, level=level)
 
 
 # top-level method for accessing the new eventing system
 # this is where all the side effects happen branched by event type
 # (i.e. - mutating the event history, printing to stdout, logging
 # to files, etc.)
-def fire_event(e: BaseEvent, level: EventLevel = None) -> None:
+def fire_event(e: BaseEvent, level: Optional[EventLevel] = None) -> None:
     EVENT_MANAGER.fire_event(e, level=level)
 
 
 def get_metadata_vars() -> Dict[str, str]:
     global metadata_vars
     if metadata_vars is None:
         metadata_vars = {
```

### Comparing `dbt-core-1.6.0b4/dbt/events/helpers.py` & `dbt-core-1.6.0b5/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/events/types.py` & `dbt-core-1.6.0b5/dbt/events/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -651,14 +651,22 @@
     def message(self) -> str:
         return f"dump {self.before_after} {self.action} : {self.dump}"
 
 
 # Skipping E032, E033, E034
 
 
+class AdapterRegistered(InfoLevel):
+    def code(self):
+        return "E034"
+
+    def message(self) -> str:
+        return f"Registered adapter: {self.adapter_name}{self.adapter_version}"
+
+
 class AdapterImportError(InfoLevel):
     def code(self):
         return "E035"
 
     def message(self) -> str:
         return f"Error importing adapter: {self.exc}"
 
@@ -798,22 +806,14 @@
     def code(self):
         return "I001"
 
     def message(self) -> str:
         return f"Error processing file diff: {self.category}, {self.file_id}"
 
 
-class PublicationArtifactChanged(DebugLevel):
-    def code(self):
-        return "I002"
-
-    def message(self) -> str:
-        return f"The publication artifact for {self.project_name} has been {self.action}."
-
-
 # Skipping I003, I004, I005, I006, I007
 
 
 class InvalidValueForField(WarnLevel):
     def code(self):
         return "I008"
```

### Comparing `dbt-core-1.6.0b4/dbt/exceptions.py` & `dbt-core-1.6.0b5/dbt/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
         return (
             f"A dependency on project {self.project} was specified, "
             f"but a publication for {self.project} was not found."
         )
 
 
 class SemverError(Exception):
-    def __init__(self, msg: str = None):
+    def __init__(self, msg: Optional[str] = None):
         self.msg = msg
         if msg is not None:
             super().__init__(msg)
         else:
             super().__init__()
 
 
@@ -1839,25 +1839,27 @@
 
 
 class UninstalledPackagesFoundError(CompilationError):
     def __init__(
         self,
         count_packages_specified: int,
         count_packages_installed: int,
+        packages_specified_path: str,
         packages_install_path: str,
     ):
         self.count_packages_specified = count_packages_specified
         self.count_packages_installed = count_packages_installed
+        self.packages_specified_path = packages_specified_path
         self.packages_install_path = packages_install_path
         super().__init__(msg=self.get_message())
 
     def get_message(self) -> str:
         msg = (
             f"dbt found {self.count_packages_specified} package(s) "
-            "specified in packages.yml, but only "
+            f"specified in {self.packages_specified_path}, but only "
             f"{self.count_packages_installed} package(s) installed "
             f'in {self.packages_install_path}. Run "dbt deps" to '
             "install package dependencies."
         )
         return msg
 
 
@@ -2415,15 +2417,15 @@
         }
 
 
 class RPCCompiling(DbtRuntimeError):
     CODE = 10010
     MESSAGE = 'RPC server is compiling the project, call the "status" method for' " compile status"
 
-    def __init__(self, msg: str = None, node=None):
+    def __init__(self, msg: Optional[str] = None, node=None):
         if msg is None:
             msg = "compile in progress"
         super().__init__(msg, node)
 
 
 class RPCLoadException(DbtRuntimeError):
     CODE = 10011
```

### Comparing `dbt-core-1.6.0b4/dbt/flags.py` & `dbt-core-1.6.0b5/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/graph/cli.py` & `dbt-core-1.6.0b5/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/graph/graph.py` & `dbt-core-1.6.0b5/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/graph/queue.py` & `dbt-core-1.6.0b5/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/graph/selector.py` & `dbt-core-1.6.0b5/dbt/graph/selector.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,17 +39,19 @@
     """The node selector is aware of the graph and manifest"""
 
     def __init__(
         self,
         graph: Graph,
         manifest: Manifest,
         previous_state: Optional[PreviousState] = None,
+        include_empty_nodes: bool = False,
     ):
         super().__init__(manifest, previous_state)
         self.full_graph = graph
+        self.include_empty_nodes = include_empty_nodes
 
         # build a subgraph containing only non-empty, enabled nodes and enabled
         # sources.
         graph_members = {
             unique_id for unique_id in self.full_graph.nodes() if self._is_graph_member(unique_id)
         }
         self.graph = self.full_graph.subgraph(graph_members)
@@ -163,15 +165,19 @@
             return source.config.enabled
         elif unique_id in self.manifest.exposures:
             return True
         elif unique_id in self.manifest.metrics:
             metric = self.manifest.metrics[unique_id]
             return metric.config.enabled
         node = self.manifest.nodes[unique_id]
-        return not node.empty and node.config.enabled
+
+        if self.include_empty_nodes:
+            return node.config.enabled
+        else:
+            return not node.empty and node.config.enabled
 
     def node_is_match(self, node: GraphMemberNode) -> bool:
         """Determine if a node is a match for the selector. Non-match nodes
         will be excluded from results during filtering.
         """
         return True
 
@@ -309,17 +315,19 @@
 class ResourceTypeSelector(NodeSelector):
     def __init__(
         self,
         graph: Graph,
         manifest: Manifest,
         previous_state: Optional[PreviousState],
         resource_types: List[NodeType],
+        include_empty_nodes: bool = False,
     ):
         super().__init__(
             graph=graph,
             manifest=manifest,
             previous_state=previous_state,
+            include_empty_nodes=include_empty_nodes,
         )
         self.resource_types: Set[NodeType] = set(resource_types)
 
     def node_is_match(self, node):
         return node.resource_type in self.resource_types
```

### Comparing `dbt-core-1.6.0b4/dbt/graph/selector_methods.py` & `dbt-core-1.6.0b5/dbt/graph/selector_methods.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/graph/selector_spec.py` & `dbt-core-1.6.0b5/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/helper_types.py` & `dbt-core-1.6.0b5/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/README.md` & `dbt-core-1.6.0b5/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/docs/overview.md` & `dbt-core-1.6.0b5/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/columns.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/drop_relation.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/drop_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/relation.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/schema.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/etc/datetime.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/etc/statement.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/configs.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/table/table.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/models/view/view.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/python_model/python.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/data_types.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/listagg.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/macros/utils/split_part.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/global_project/tests/generic/builtin.sql` & `dbt-core-1.6.0b5/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/index.html` & `dbt-core-1.6.0b5/dbt/include/index.html`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/starter_project/README.md` & `dbt-core-1.6.0b5/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.6.0b5/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/internal_deprecations.py` & `dbt-core-1.6.0b5/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/logger.py` & `dbt-core-1.6.0b5/dbt/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
         return LogMessage.from_record_formatted(record, message)
 
 
 class ListLogHandler(LogMessageHandler):
     def __init__(
         self,
         level: int = logbook.NOTSET,
-        filter: Callable = None,
+        filter: Optional[Callable] = None,
         bubble: bool = False,
         lst: Optional[List[LogMessage]] = None,
     ) -> None:
         super().__init__(level, filter, bubble)
         if lst is None:
             lst = []
         self.records: List[LogMessage] = lst
```

### Comparing `dbt-core-1.6.0b4/dbt/node_types.py` & `dbt-core-1.6.0b5/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/__init__.py` & `dbt-core-1.6.0b5/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/analysis.py` & `dbt-core-1.6.0b5/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/base.py` & `dbt-core-1.6.0b5/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/common.py` & `dbt-core-1.6.0b5/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/docs.py` & `dbt-core-1.6.0b5/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/generic_test.py` & `dbt-core-1.6.0b5/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/generic_test_builders.py` & `dbt-core-1.6.0b5/dbt/parser/generic_test_builders.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     def __init__(
         self,
         test: Dict[str, Any],
         target: Testable,
         package_name: str,
         render_ctx: Dict[str, Any],
-        column_name: str = None,
+        column_name: Optional[str] = None,
         version: Optional[NodeVersion] = None,
     ) -> None:
         test_name, test_args = self.extract_test_args(test, column_name)
         self.args: Dict[str, Any] = test_args
         if "model" in self.args:
             raise TestArgIncludesModelError()
         self.package_name: str = package_name
```

### Comparing `dbt-core-1.6.0b4/dbt/parser/hooks.py` & `dbt-core-1.6.0b5/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/macros.py` & `dbt-core-1.6.0b5/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/manifest.py` & `dbt-core-1.6.0b5/dbt/parser/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     Callable,
     Any,
     List,
     Type,
     Union,
     Tuple,
     Set,
-    MutableMapping,
 )
 from itertools import chain
 import time
 from dbt.events.base_types import EventLevel
 import json
 import pprint
 import msgpack
@@ -31,53 +30,46 @@
 
 from dbt.adapters.factory import (
     get_adapter,
     get_relation_class_by_name,
     get_adapter_package_names,
 )
 from dbt.constants import (
-    DEPENDENCIES_FILE_NAME,
     MANIFEST_FILE_NAME,
     PARTIAL_PARSE_FILE_NAME,
     SEMANTIC_MANIFEST_FILE_NAME,
 )
 from dbt.helper_types import PathSet
-from dbt.clients.yaml_helper import load_yaml_text
 from dbt.events.functions import fire_event, get_invocation_id, warn_or_error
-from dbt.events.helpers import datetime_to_json_string
 from dbt.events.types import (
     PartialParsingErrorProcessingFile,
     PartialParsingError,
     ParsePerfInfoPath,
     PartialParsingSkipParsing,
     UnableToPartialParse,
     PartialParsingNotEnabled,
     ParsedFileLoadFailed,
     InvalidDisabledTargetInTestNode,
     NodeNotFoundOrDisabled,
     StateCheckVarsHash,
     Note,
-    PublicationArtifactChanged,
     PublicationArtifactAvailable,
     DeprecatedModel,
     DeprecatedReference,
     UpcomingReferenceDeprecation,
 )
-from dbt_extractor import py_extract_from_source  # type: ignore
 from dbt.logger import DbtProcessState
 from dbt.node_types import NodeType, AccessType
 from dbt.clients.jinja import get_rendered, MacroStack
 from dbt.clients.jinja_static import statically_extract_macro_calls
 from dbt.clients.system import (
     make_directory,
     path_exists,
     read_json,
     write_file,
-    resolve_path_from_base,
-    load_file_contents,
 )
 from dbt.config import Project, RuntimeConfig
 from dbt.context.docs import generate_runtime_docs_context
 from dbt.context.macro_resolver import MacroResolver, TestMacroNamespace
 from dbt.context.configured import generate_macro_context
 from dbt.context.providers import ParseProvider
 from dbt.contracts.files import FileHash, ParseFileType, SchemaSourceFile
@@ -103,22 +95,22 @@
     Metric,
     SeedNode,
     ManifestNode,
     ResultNode,
     ModelNode,
     NodeRelation,
 )
+from dbt.contracts.graph.node_args import ModelNodeArgs
 from dbt.contracts.graph.unparsed import NodeVersion
 from dbt.contracts.util import Writable
 from dbt.contracts.publication import (
     PublicationConfig,
     PublicationArtifact,
     PublicationMetadata,
     PublicModel,
-    ProjectDependencies,
 )
 from dbt.exceptions import (
     TargetNotFoundError,
     AmbiguousAliasError,
     PublicationConfigNotFound,
     ProjectDependencyCycleError,
     InvalidAccessTypeError,
@@ -520,49 +512,48 @@
             # We need to rebuild disabled in order to include disabled sources
             self.manifest.rebuild_disabled_lookup()
 
             # copy the selectors from the root_project to the manifest
             self.manifest.selectors = self.root_project.manifest_selectors
 
             # load manifest.dependencies and associated publication artifacts to create the external nodes
-            public_nodes_changed = self.build_public_nodes()
-            if public_nodes_changed:
+            external_nodes_modified = self.inject_external_nodes()
+            if external_nodes_modified:
                 self.manifest.rebuild_ref_lookup()
 
             # update the refs, sources, docs and metrics depends_on.nodes
             # These check the created_at time on the nodes to
             # determine whether they need processing.
             start_process = time.perf_counter()
             self.process_sources(self.root_project.project_name)
             self.process_refs(self.root_project.project_name)
             self.process_docs(self.root_project)
             self.process_metrics(self.root_project)
-            self.process_semantic_models()
             self.check_valid_group_config()
             self.check_valid_access_property()
 
             # update tracking data
             self._perf_info.process_manifest_elapsed = time.perf_counter() - start_process
             self._perf_info.static_analysis_parsed_path_count = (
                 self.manifest._parsing_info.static_analysis_parsed_path_count
             )
             self._perf_info.static_analysis_path_count = (
                 self.manifest._parsing_info.static_analysis_path_count
             )
 
         # Load dependencies, load the publication artifacts and create the external nodes.
         # Reprocess refs if changes.
-        public_nodes_changed = False
+        external_nodes_modified = False
         if skip_parsing:
             # If we didn't skip parsing, this will have already run because it must run
             # before process_refs. If we did skip parsing, then it's possible that only
             # publications have changed and we need to run this to capture that.
             self.manifest.build_parent_and_child_maps()
-            public_nodes_changed = self.build_public_nodes()
-            if public_nodes_changed:
+            external_nodes_modified = self.inject_external_nodes()
+            if external_nodes_modified:
                 self.manifest.rebuild_ref_lookup()
                 self.process_refs(self.root_project.project_name)
                 # parent and child maps will be rebuilt by write_manifest
 
         # Log the publication artifact for this project
         log_publication_artifact(self.root_project, self.manifest)
 
@@ -587,14 +578,15 @@
                             model_version=version_to_str(node.version),
                             deprecation_date=node.deprecation_date.isoformat(),
                         )
                     )
 
                 resolved_refs = self.manifest.resolve_refs(node, self.root_project.project_name)
                 resolved_model_refs = [r for r in resolved_refs if isinstance(r, ModelNode)]
+                node.depends_on
                 for resolved_ref in resolved_model_refs:
                     if resolved_ref.deprecation_date:
 
                         if resolved_ref.deprecation_date < datetime.datetime.now().astimezone():
                             event_cls = DeprecatedReference
                         else:
                             event_cls = UpcomingReferenceDeprecation
@@ -756,121 +748,64 @@
             manifest_msgpack = self.manifest.to_msgpack(extended_mashumaro_encoder)
             make_directory(os.path.dirname(path))
             with open(path, "wb") as fp:
                 fp.write(manifest_msgpack)
         except Exception:
             raise
 
-    def build_public_nodes(self) -> bool:
-        """This method loads the dependencies from dependencies.yml, reads in the
-        the publication artifacts and adds the PublicModels to the manifest
-        "public_nodes" dictionary. It returns a boolean that indicates that
-        public nodes have been rebuilt."""
-        public_nodes_changed = False
-
-        # Load the dependencies from the dependencies.yml file
-        # TODO: dependencies might be better in the RuntimeConfig and
-        # loaded somewhere earlier, but leaving this here for later refactoring.
-        # Loading it elsewhere would make it harder to detect that there were
-        # no dependencies previously and still are none, though that could be
-        # inferred from the manifest publication configs.
-        dependencies_filepath = resolve_path_from_base(
-            DEPENDENCIES_FILE_NAME, self.root_project.project_root
-        )
-        saved_manifest_dependencies = self.manifest.project_dependencies
-        if path_exists(dependencies_filepath):
-            contents = load_file_contents(dependencies_filepath)
-            dependencies_dict = load_yaml_text(contents)
-            dependencies = ProjectDependencies.from_dict(dependencies_dict)
-            self.manifest.project_dependencies = dependencies
-        else:
-            self.manifest.project_dependencies = None
-
-        # Return False if there weren't any dependencies before and aren't any now.
-        if saved_manifest_dependencies is None and self.manifest.project_dependencies is None:
-            return False
-
-        # collect the names of the projects for later use
-        project_dependency_names = []
-        if self.manifest.project_dependencies:
-            for project in self.manifest.project_dependencies.projects:
-                project_dependency_names.append(project.name)
-
-        # Save previous publications, for later removal of references
-        saved_manifest_publications: MutableMapping[str, PublicationConfig] = deepcopy(
-            self.manifest.publications
-        )
-        if self.manifest.publications:
-            for project_name, publication in self.manifest.publications.items():
-                if project_name not in project_dependency_names:
-                    remove_dependent_project_references(self.manifest, publication)
-                    saved_manifest_publications.pop(project_name)
-                    fire_event(
-                        PublicationArtifactChanged(
-                            action="removed",
-                            project_name=project_name,
-                            generated_at=datetime_to_json_string(
-                                publication.metadata.generated_at
-                            ),
-                        )
-                    )
-                    public_nodes_changed = True
-
-            # clean up previous publications that are no longer specified
-            self.manifest.publications = {}
-            # Empty public_nodes since we're re-generating them all
-            self.manifest.public_nodes = {}
-
-        if self.manifest.project_dependencies:
-            self.load_new_public_nodes()
-
-        # Now that we've loaded the current publications and public_nodes, look for
-        # changed publications so we can reset the public_nodes references
-        for project_name, publication in self.manifest.publications.items():
-            if (
-                project_name in saved_manifest_publications
-                and publication.metadata.generated_at
-                != saved_manifest_publications[project_name].metadata.generated_at
-            ):
-                remove_dependent_project_references(
-                    self.manifest, saved_manifest_publications[project_name]
-                )
-                fire_event(
-                    PublicationArtifactChanged(
-                        action="updated",
-                        project_name=project_name,
-                        generated_at=datetime_to_json_string(publication.metadata.generated_at),
-                    )
-                )
-                public_nodes_changed = True
-            elif project_name not in saved_manifest_publications:
-                fire_event(
-                    PublicationArtifactChanged(
-                        action="added",
-                        project_name=project_name,
-                        generated_at=datetime_to_json_string(publication.metadata.generated_at),
-                    )
-                )
-                public_nodes_changed = True
-
-        return public_nodes_changed
-
-    def load_new_public_nodes(self):
-        for project in self.manifest.project_dependencies.projects:
+    def build_external_nodes(self) -> List[ModelNodeArgs]:
+        external_node_args = []
+        for project in self.root_project.dependent_projects.projects:
             try:
                 publication = self.publications[project.name]
             except KeyError:
                 raise PublicationConfigNotFound(project=project.name)
 
             publication_config = PublicationConfig.from_publication(publication)
             self.manifest.publications[project.name] = publication_config
 
-            # Add to dictionary of public_nodes and save id in PublicationConfig
+            # Add public models to list of external nodes
             for public_node in publication.public_models.values():
-                self.manifest.public_nodes[public_node.unique_id] = public_node
+                external_node_args.append(
+                    ModelNodeArgs(
+                        name=public_node.name,
+                        package_name=public_node.package_name,
+                        version=public_node.version,
+                        latest_version=public_node.latest_version,
+                        relation_name=public_node.relation_name,
+                        database=public_node.database,
+                        schema=public_node.schema,
+                        identifier=public_node.identifier,
+                        deprecation_date=public_node.deprecation_date,
+                    )
+                )
+
+        return external_node_args
+
+    def inject_external_nodes(self) -> bool:
+        # TODO: remove manifest.publications
+        self.manifest.publications = {}
+
+        external_node_args = self.build_external_nodes()
+
+        # Remove previously existing external nodes since we are regenerating them
+        manifest_nodes_modified = False
+        for unique_id in self.manifest.external_node_unique_ids:
+            self.manifest.nodes.pop(unique_id)
+            remove_dependent_project_references(self.manifest, unique_id)
+            manifest_nodes_modified = True
+
+        for node_arg in external_node_args:
+            node = ModelNode.from_args(node_arg)
+            # node may already exist from package or running project - in which case we should avoid clobbering it with an external node
+            if node.unique_id not in self.manifest.nodes:
+                self.manifest.add_node_nofile(node)
+                manifest_nodes_modified = True
+
+        return manifest_nodes_modified
 
     def is_partial_parsable(self, manifest: Manifest) -> Tuple[bool, Optional[str]]:
         """Compare the global hashes of the read-in parse results' values to
         the known ones, and return if it is ok to re-use the results.
         """
         valid = True
         reparse_reason = None
@@ -1155,23 +1090,28 @@
 
     # Takes references in 'refs' array of nodes and exposures, finds the target
     # node, and updates 'depends_on.nodes' with the unique id
     def process_refs(self, current_project: str):
         for node in self.manifest.nodes.values():
             if node.created_at < self.started_at:
                 continue
-            _process_refs_for_node(self.manifest, current_project, node)
+            _process_refs(self.manifest, current_project, node)
         for exposure in self.manifest.exposures.values():
             if exposure.created_at < self.started_at:
                 continue
-            _process_refs_for_exposure(self.manifest, current_project, exposure)
+            _process_refs(self.manifest, current_project, exposure)
         for metric in self.manifest.metrics.values():
             if metric.created_at < self.started_at:
                 continue
-            _process_refs_for_metric(self.manifest, current_project, metric)
+            _process_refs(self.manifest, current_project, metric)
+        for semantic_model in self.manifest.semantic_nodes.values():
+            if semantic_model.created_at < self.started_at:
+                continue
+            _process_refs(self.manifest, current_project, semantic_model)
+            self.update_semantic_model(semantic_model)
 
     # Takes references in 'metrics' array of nodes and exposures, finds the target
     # node, and updates 'depends_on.nodes' with the unique id
     def process_metrics(self, config: RuntimeConfig):
         current_project = config.project_name
         for node in self.manifest.nodes.values():
             if node.created_at < self.started_at:
@@ -1184,35 +1124,25 @@
                 continue
             _process_metrics_for_node(self.manifest, current_project, metric)
         for exposure in self.manifest.exposures.values():
             if exposure.created_at < self.started_at:
                 continue
             _process_metrics_for_node(self.manifest, current_project, exposure)
 
-    def process_semantic_models(self) -> None:
-        for semantic_model in self.manifest.semantic_nodes.values():
-            if semantic_model.model:
-                statically_parsed = py_extract_from_source(f"{{{{ {semantic_model.model} }}}}")
-                if statically_parsed["refs"]:
-
-                    ref = statically_parsed["refs"][0]
-                    if len(ref) == 2:
-                        input_package_name, input_model_name = ref
-                    else:
-                        input_package_name, input_model_name = None, ref[0]
-
-                    refd_node = self.manifest.ref_lookup.find(
-                        input_model_name, input_package_name, None, self.manifest
-                    )
-                    if isinstance(refd_node, ModelNode):
-                        semantic_model.node_relation = NodeRelation(
-                            alias=refd_node.alias,
-                            schema_name=refd_node.schema,
-                            database=refd_node.database,
-                        )
+    def update_semantic_model(self, semantic_model) -> None:
+        # This has to be done at the end of parsing because the referenced model
+        # might have alias/schema/database fields that are updated by yaml config.
+        if semantic_model.depends_on_nodes[0]:
+            refd_node = self.manifest.nodes[semantic_model.depends_on_nodes[0]]
+            semantic_model.node_relation = NodeRelation(
+                relation_name=refd_node.relation_name,
+                alias=refd_node.alias,
+                schema_name=refd_node.schema,
+                database=refd_node.database,
+            )
 
     # nodes: node and column descriptions
     # sources: source and table descriptions, column descriptions
     # macros: macro argument descriptions
     # exposures: exposure descriptions
     def process_docs(self, config: RuntimeConfig):
         for node in self.manifest.nodes.values():
@@ -1490,111 +1420,70 @@
     exposure.description = get_rendered(exposure.description, context)
 
 
 def _process_docs_for_metrics(context: Dict[str, Any], metric: Metric) -> None:
     metric.description = get_rendered(metric.description, context)
 
 
-def _process_refs_for_exposure(manifest: Manifest, current_project: str, exposure: Exposure):
-    """Given a manifest and exposure in that manifest, process its refs"""
-    for ref in exposure.refs:
-        target_model: Optional[Union[Disabled, ManifestNode]] = None
-        target_model_name: str = ref.name
-        target_model_package: Optional[str] = ref.package
-        target_model_version: Optional[NodeVersion] = ref.version
-
-        if len(ref.positional_args) < 1 or len(ref.positional_args) > 2:
-            raise dbt.exceptions.DbtInternalError(
-                f"Refs should always be 1 or 2 arguments - got {len(ref.positional_args)}"
-            )
-
-        target_model = manifest.resolve_ref(
-            exposure,
-            target_model_name,
-            target_model_package,
-            target_model_version,
-            current_project,
-            exposure.package_name,
-        )
-
-        if target_model is None or isinstance(target_model, Disabled):
-            # This may raise. Even if it doesn't, we don't want to add
-            # this exposure to the graph b/c there is no destination exposure
-            exposure.config.enabled = False
-            invalid_target_fail_unless_test(
-                node=exposure,
-                target_name=target_model_name,
-                target_kind="node",
-                target_package=target_model_package,
-                target_version=target_model_version,
-                disabled=(isinstance(target_model, Disabled)),
-                should_warn_if_disabled=False,
-            )
-
-            continue
-        elif isinstance(target_model, ModelNode) and target_model.access == AccessType.Private:
-            # Exposures do not have a group and so can never reference private models
-            raise dbt.exceptions.DbtReferenceError(
-                unique_id=exposure.unique_id,
-                ref_unique_id=target_model.unique_id,
-                group=dbt.utils.cast_to_str(target_model.group),
-            )
-
-        target_model_id = target_model.unique_id
-
-        exposure.depends_on.add_node(target_model_id)
+def _process_refs(manifest: Manifest, current_project: str, node) -> None:
+    """Given a manifest and node in that manifest, process its refs"""
 
+    if isinstance(node, SeedNode):
+        return
 
-def _process_refs_for_metric(manifest: Manifest, current_project: str, metric: Metric):
-    """Given a manifest and a metric in that manifest, process its refs"""
-    for ref in metric.refs:
+    for ref in node.refs:
         target_model: Optional[Union[Disabled, ManifestNode]] = None
         target_model_name: str = ref.name
         target_model_package: Optional[str] = ref.package
         target_model_version: Optional[NodeVersion] = ref.version
 
         if len(ref.positional_args) < 1 or len(ref.positional_args) > 2:
             raise dbt.exceptions.DbtInternalError(
                 f"Refs should always be 1 or 2 arguments - got {len(ref.positional_args)}"
             )
 
         target_model = manifest.resolve_ref(
-            metric,
+            node,
             target_model_name,
             target_model_package,
             target_model_version,
             current_project,
-            metric.package_name,
+            node.package_name,
         )
 
         if target_model is None or isinstance(target_model, Disabled):
             # This may raise. Even if it doesn't, we don't want to add
-            # this metric to the graph b/c there is no destination metric
-            metric.config.enabled = False
+            # this exposure to the graph b/c there is no destination exposure
+            node.config.enabled = False
             invalid_target_fail_unless_test(
-                node=metric,
+                node=node,
                 target_name=target_model_name,
                 target_kind="node",
                 target_package=target_model_package,
                 target_version=target_model_version,
                 disabled=(isinstance(target_model, Disabled)),
                 should_warn_if_disabled=False,
             )
+
             continue
-        elif isinstance(target_model, ModelNode) and target_model.access == AccessType.Private:
-            if not metric.group or metric.group != target_model.group:
+        elif (
+            isinstance(target_model, ModelNode)
+            and target_model.access == AccessType.Private
+            and node.resource_type != NodeType.SqlOperation
+            and node.resource_type != NodeType.RPCCall  # TODO: rm
+        ):
+            if not node.group or node.group != target_model.group:
                 raise dbt.exceptions.DbtReferenceError(
-                    unique_id=metric.unique_id,
+                    unique_id=node.unique_id,
                     ref_unique_id=target_model.unique_id,
                     group=dbt.utils.cast_to_str(target_model.group),
                 )
 
         target_model_id = target_model.unique_id
-
-        metric.depends_on.add_node(target_model_id)
+        node.depends_on.add_node(target_model_id)
 
 
 def _process_metrics_for_node(
     manifest: Manifest,
     current_project: str,
     node: Union[ManifestNode, Metric, Exposure],
 ):
@@ -1638,80 +1527,21 @@
             continue
 
         target_metric_id = target_metric.unique_id
 
         node.depends_on.add_node(target_metric_id)
 
 
-def _process_refs_for_node(manifest: Manifest, current_project: str, node: ManifestNode):
-    """Given a manifest and a node in that manifest, process its refs"""
-
-    if isinstance(node, SeedNode):
-        return
-
-    for ref in node.refs:
-        target_model: Optional[Union[Disabled, ManifestNode]] = None
-        target_model_name: str = ref.name
-        target_model_package: Optional[str] = ref.package
-        target_model_version: Optional[NodeVersion] = ref.version
-
-        if len(ref.positional_args) < 1 or len(ref.positional_args) > 2:
-            raise dbt.exceptions.DbtInternalError(
-                f"Refs should always be 1 or 2 arguments - got {len(ref.positional_args)}"
-            )
-
-        target_model = manifest.resolve_ref(
-            node,
-            target_model_name,
-            target_model_package,
-            target_model_version,
-            current_project,
-            node.package_name,
-        )
-
-        if target_model is None or isinstance(target_model, Disabled):
-            # This may raise. Even if it doesn't, we don't want to add
-            # this node to the graph b/c there is no destination node
-            node.config.enabled = False
-            invalid_target_fail_unless_test(
-                node=node,
-                target_name=target_model_name,
-                target_kind="node",
-                target_package=target_model_package,
-                target_version=target_model_version,
-                disabled=(isinstance(target_model, Disabled)),
-                should_warn_if_disabled=False,
-            )
-            continue
-
-        # Handle references to models that are private
-        elif isinstance(target_model, ModelNode) and target_model.access == AccessType.Private:
-            if not node.group or node.group != target_model.group:
-                raise dbt.exceptions.DbtReferenceError(
-                    unique_id=node.unique_id,
-                    ref_unique_id=target_model.unique_id,
-                    group=dbt.utils.cast_to_str(target_model.group),
-                )
-
-        target_model_id = target_model.unique_id
-
-        if target_model.is_public_node:
-            node.depends_on.add_public_node(target_model_id)
-        else:
-            node.depends_on.add_node(target_model_id)
-
-
-def remove_dependent_project_references(manifest: Manifest, publication: PublicationConfig):
-    for unique_id in publication.public_node_ids:
-        for child_id in manifest.child_map[unique_id]:
-            node = manifest.expect(child_id)
-            if hasattr(node.depends_on, "public_nodes"):
-                node.depends_on.public_nodes.remove(unique_id)  # type: ignore
-                # set created_at so process_refs happens
-                node.created_at = time.time()
+def remove_dependent_project_references(manifest, external_node_unique_id):
+    for child_id in manifest.child_map[external_node_unique_id]:
+        node = manifest.expect(child_id)
+        # child node may have been modified and already recreated its depends_on.nodes list
+        if external_node_unique_id in node.depends_on_nodes:
+            node.depends_on_nodes.remove(external_node_unique_id)
+        node.created_at = time.time()
 
 
 def _process_sources_for_exposure(manifest: Manifest, current_project: str, exposure: Exposure):
     target_source: Optional[Union[Disabled, SourceDefinition]] = None
     for source_name, table_name in exposure.sources:
         target_source = manifest.resolve_source(
             source_name,
@@ -1795,15 +1625,15 @@
 
 
 # This is called in task.rpc.sql_commands when a "dynamic" node is
 # created in the manifest, in 'add_refs'
 def process_node(config: RuntimeConfig, manifest: Manifest, node: ManifestNode):
 
     _process_sources_for_node(manifest, config.project_name, node)
-    _process_refs_for_node(manifest, config.project_name, node)
+    _process_refs(manifest, config.project_name, node)
     ctx = generate_runtime_docs_context(config, node, manifest, config.project_name)
     _process_docs_for_node(ctx, node)
 
 
 def log_publication_artifact(root_project: RuntimeConfig, manifest: Manifest):
     # The manifest.json is written out in a task, so we're not writing it here
 
@@ -1848,16 +1678,16 @@
             generated_at=metadata.generated_at,
             deprecation_date=model.deprecation_date,
         )
         public_models[unique_id] = public_model
 
     dependencies = []
     # Get dependencies from dependencies.yml
-    if manifest.project_dependencies:
-        for dep_project in manifest.project_dependencies.projects:
+    if root_project.dependent_projects.projects:
+        for dep_project in root_project.dependent_projects.projects:
             dependencies.append(dep_project.name)
     # Get dependencies from publication dependencies
     for pub_project in manifest.publications.values():
         for project_name in pub_project.dependencies:
             if project_name == root_project.project_name:
                 raise ProjectDependencyCycleError(
                     pub_project_name=pub_project.project_name, project_name=project_name
```

### Comparing `dbt-core-1.6.0b4/dbt/parser/models.py` & `dbt-core-1.6.0b5/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/partial.py` & `dbt-core-1.6.0b5/dbt/parser/partial.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,15 +605,15 @@
         # Need to do the deleted/added/changed thing, just like the files lists
 
         env_var_changes = {}
         if schema_file.file_id in self.env_vars_changed_schema_files:
             env_var_changes = self.env_vars_changed_schema_files[schema_file.file_id]
 
         # models, seeds, snapshots, analyses
-        for dict_key in ["models", "seeds", "snapshots", "analyses"]:
+        for dict_key in ["models", "seeds", "snapshots", "analyses", "semantic_models"]:
             key_diff = self.get_diff_for(dict_key, saved_yaml_dict, new_yaml_dict)
             if key_diff["changed"]:
                 for elem in key_diff["changed"]:
                     self.delete_schema_mssa_links(schema_file, dict_key, elem)
                     self.merge_patch(schema_file, dict_key, elem)
             if key_diff["deleted"]:
                 for elem in key_diff["deleted"]:
```

### Comparing `dbt-core-1.6.0b4/dbt/parser/read_files.py` & `dbt-core-1.6.0b5/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/schema_generic_tests.py` & `dbt-core-1.6.0b5/dbt/parser/schema_generic_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     def resource_type(self) -> NodeType:
         return NodeType.Test
 
     @classmethod
     def get_compiled_path(cls, block: FileBlock) -> str:
         return block.path.relative_path
 
-    def parse_file(self, block: FileBlock, dct: Dict = None) -> None:
+    def parse_file(self, block: FileBlock, dct: Optional[Dict] = None) -> None:
         pass
 
     def parse_from_dict(self, dct, validate=True) -> GenericTestNode:
         if validate:
             GenericTestNode.validate(dct)
         return GenericTestNode.from_dict(dct)
```

### Comparing `dbt-core-1.6.0b4/dbt/parser/schema_renderer.py` & `dbt-core-1.6.0b5/dbt/parser/schema_renderer.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         elif self.key == "macros":
             if keypath[0] == "arguments":
                 if self._is_norender_key(keypath[1:]):
                     return False
             elif self._is_norender_key(keypath[0:]):
                 return False
         elif self.key == "metrics":
-            # back compat: "expression" is new name, "sql" is old name
-            if keypath[0] in ("expression", "sql"):
+            # This ensures all key paths that end in 'filter' for a metric are skipped
+            if keypath[-1] == "filter":
                 return False
             elif self._is_norender_key(keypath[0:]):
                 return False
         else:  # models, seeds, snapshots, analyses
             if self._is_norender_key(keypath[0:]):
                 return False
         return True
```

### Comparing `dbt-core-1.6.0b4/dbt/parser/schema_yaml_readers.py` & `dbt-core-1.6.0b5/dbt/parser/schema_yaml_readers.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,28 +30,31 @@
     Dimension,
     DimensionTypeParams,
     Entity,
     Measure,
     NonAdditiveDimension,
 )
 from dbt.exceptions import DbtInternalError, YamlParseDictError, JSONValidationError
-from dbt.context.providers import generate_parse_exposure
+from dbt.context.providers import generate_parse_exposure, generate_parse_semantic_models
+
 from dbt.contracts.graph.model_config import MetricConfig, ExposureConfig
 from dbt.context.context_config import (
     BaseContextConfigGenerator,
     ContextConfigGenerator,
     UnrenderedConfigGenerator,
 )
 from dbt.clients.jinja import get_rendered
 from dbt.dataclass_schema import ValidationError
-from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
-from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
-from dbt_semantic_interfaces.type_enums.entity_type import EntityType
-from dbt_semantic_interfaces.type_enums.metric_type import MetricType
-from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+from dbt_semantic_interfaces.type_enums import (
+    AggregationType,
+    DimensionType,
+    EntityType,
+    MetricType,
+    TimeGranularity,
+)
 from typing import List, Optional, Union
 
 
 class ExposureParser(YamlReader):
     def __init__(self, schema_parser: SchemaParser, yaml: YamlBlock):
         super().__init__(schema_parser, yaml, NodeType.Exposure.pluralize())
         self.schema_parser = schema_parser
@@ -237,60 +240,71 @@
             return MetricTimeWindow(
                 count=int(count),
                 granularity=TimeGranularity(granularity),
             )
         else:
             return None
 
+    def _get_metric_input(self, unparsed: Union[UnparsedMetricInput, str]) -> MetricInput:
+        if isinstance(unparsed, str):
+            return MetricInput(name=unparsed)
+        else:
+            offset_to_grain: Optional[TimeGranularity] = None
+            if unparsed.offset_to_grain is not None:
+                offset_to_grain = TimeGranularity(unparsed.offset_to_grain)
+
+            filter: Optional[WhereFilter] = None
+            if unparsed.filter is not None:
+                filter = WhereFilter(where_sql_template=unparsed.filter)
+
+            return MetricInput(
+                name=unparsed.name,
+                filter=filter,
+                alias=unparsed.alias,
+                offset_window=self._get_time_window(unparsed.offset_window),
+                offset_to_grain=offset_to_grain,
+            )
+
+    def _get_optional_metric_input(
+        self,
+        unparsed: Optional[Union[UnparsedMetricInput, str]],
+    ) -> Optional[MetricInput]:
+        if unparsed is not None:
+            return self._get_metric_input(unparsed)
+        else:
+            return None
+
     def _get_metric_inputs(
         self,
         unparsed_metric_inputs: Optional[List[Union[UnparsedMetricInput, str]]],
     ) -> List[MetricInput]:
         metric_inputs: List[MetricInput] = []
         if unparsed_metric_inputs is not None:
             for unparsed_metric_input in unparsed_metric_inputs:
-                if isinstance(unparsed_metric_input, str):
-                    metric_inputs.append(MetricInput(name=unparsed_metric_input))
-                else:
-                    offset_to_grain: Optional[TimeGranularity] = None
-                    if unparsed_metric_input.offset_to_grain is not None:
-                        offset_to_grain = TimeGranularity(unparsed_metric_input.offset_to_grain)
-
-                    filter: Optional[WhereFilter] = None
-                    if unparsed_metric_input.filter is not None:
-                        filter = WhereFilter(where_sql_template=unparsed_metric_input.filter)
-
-                    metric_inputs.append(
-                        MetricInput(
-                            name=unparsed_metric_input.name,
-                            filter=filter,
-                            alias=unparsed_metric_input.alias,
-                            offset_window=self._get_time_window(
-                                unparsed_window=unparsed_metric_input.offset_window
-                            ),
-                            offset_to_grain=offset_to_grain,
-                        )
-                    )
+                metric_inputs.append(self._get_metric_input(unparsed=unparsed_metric_input))
 
         return metric_inputs
 
     def _get_metric_type_params(self, type_params: UnparsedMetricTypeParams) -> MetricTypeParams:
         grain_to_date: Optional[TimeGranularity] = None
         if type_params.grain_to_date is not None:
             grain_to_date = TimeGranularity(type_params.grain_to_date)
 
         return MetricTypeParams(
             measure=self._get_optional_input_measure(type_params.measure),
-            measures=self._get_input_measures(type_params.measures),
-            numerator=self._get_optional_input_measure(type_params.numerator),
-            denominator=self._get_optional_input_measure(type_params.denominator),
+            numerator=self._get_optional_metric_input(type_params.numerator),
+            denominator=self._get_optional_metric_input(type_params.denominator),
             expr=type_params.expr,
             window=self._get_time_window(type_params.window),
             grain_to_date=grain_to_date,
             metrics=self._get_metric_inputs(type_params.metrics),
+            # TODO This is a compiled list of measure/numerator/denominator as
+            # well as the `input_measures` of included metrics. We're planning
+            # on doing this as part of CT-2707
+            # input_measures=?,
         )
 
     def parse_metric(self, unparsed: UnparsedMetric):
         package_name = self.project.project_name
         unique_id = f"{NodeType.Metric}.{package_name}.{unparsed.name}"
         path = self.yaml.path.relative_path
 
@@ -517,14 +531,27 @@
             unique_id=unique_id,
             entities=self._get_entities(unparsed.entities),
             measures=self._get_measures(unparsed.measures),
             dimensions=self._get_dimensions(unparsed.dimensions),
             defaults=unparsed.defaults,
         )
 
+        ctx = generate_parse_semantic_models(
+            parsed,
+            self.root_project,
+            self.schema_parser.manifest,
+            package_name,
+        )
+
+        if parsed.model is not None:
+            model_ref = "{{ " + parsed.model + " }}"
+            # This sets the "refs" in the SemanticModel from the MetricRefResolver in context/providers.py
+            get_rendered(model_ref, ctx, parsed)
+
+        # No ability to disable a semantic model at this time
         self.manifest.add_semantic_model(self.yaml.file, parsed)
 
     def parse(self):
         for data in self.get_key_dicts():
             try:
                 UnparsedSemanticModel.validate(data)
                 unparsed = UnparsedSemanticModel.from_dict(data)
```

### Comparing `dbt-core-1.6.0b4/dbt/parser/schemas.py` & `dbt-core-1.6.0b5/dbt/parser/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         # should this raise an error?
         return block.path.relative_path
 
     @property
     def resource_type(self) -> NodeType:
         return NodeType.Test
 
-    def parse_file(self, block: FileBlock, dct: Dict = None) -> None:
+    def parse_file(self, block: FileBlock, dct: Optional[Dict] = None) -> None:
         assert isinstance(block.file, SchemaSourceFile)
 
         # If partially parsing, dct should be from pp_dict, otherwise
         # dict_from_yaml
         if dct:
             # contains the FileBlock and the data (dictionary)
             yaml_block = YamlBlock.from_file_block(block, dct)
```

### Comparing `dbt-core-1.6.0b4/dbt/parser/search.py` & `dbt-core-1.6.0b5/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/seeds.py` & `dbt-core-1.6.0b5/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/singular_test.py` & `dbt-core-1.6.0b5/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/snapshots.py` & `dbt-core-1.6.0b5/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/sources.py` & `dbt-core-1.6.0b5/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/parser/sql.py` & `dbt-core-1.6.0b5/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/semver.py` & `dbt-core-1.6.0b5/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/base.py` & `dbt-core-1.6.0b5/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/build.py` & `dbt-core-1.6.0b5/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/clean.py` & `dbt-core-1.6.0b5/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/compile.py` & `dbt-core-1.6.0b5/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/debug.py` & `dbt-core-1.6.0b5/dbt/task/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,21 +98,22 @@
 
     @property
     def project_profile(self):
         if self.project is None:
             return None
         return self.project.profile_name
 
-    def path_info(self):
-        open_cmd = dbt.clients.system.open_dir_cmd()
-        fire_event(OpenCommand(open_cmd=open_cmd, profiles_dir=self.profiles_dir))
-
     def run(self) -> bool:
+        # WARN: this is a legacy workflow that is not compatible with other runtime flags
         if self.args.config_dir:
-            self.path_info()
+            fire_event(
+                OpenCommand(
+                    open_cmd=dbt.clients.system.open_dir_cmd(), profiles_dir=str(self.profiles_dir)
+                )
+            )
             return DebugRunStatus.SUCCESS.value
 
         version: str = get_installed_version().to_version_string(skip_matcher=True)
         fire_event(DebugCmdOut(msg="dbt version: {}".format(version)))
         fire_event(DebugCmdOut(msg="python version: {}".format(sys.version.split()[0])))
         fire_event(DebugCmdOut(msg="python path: {}".format(sys.executable)))
         fire_event(DebugCmdOut(msg="os info: {}".format(platform.platform())))
```

### Comparing `dbt-core-1.6.0b4/dbt/task/deps.py` & `dbt-core-1.6.0b5/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/freshness.py` & `dbt-core-1.6.0b5/dbt/task/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/generate.py` & `dbt-core-1.6.0b5/dbt/task/generate.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/init.py` & `dbt-core-1.6.0b5/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/list.py` & `dbt-core-1.6.0b5/dbt/task/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,12 +190,13 @@
             )
         else:
             return ResourceTypeSelector(
                 graph=self.graph,
                 manifest=self.manifest,
                 previous_state=self.previous_state,
                 resource_types=self.resource_types,
+                include_empty_nodes=True,
             )
 
     def interpret_results(self, results):
         # list command should always return 0 as exit code
         return True
```

### Comparing `dbt-core-1.6.0b4/dbt/task/printer.py` & `dbt-core-1.6.0b5/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/retry.py` & `dbt-core-1.6.0b5/dbt/task/retry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/run.py` & `dbt-core-1.6.0b5/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/run_operation.py` & `dbt-core-1.6.0b5/dbt/task/run_operation.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,34 +12,34 @@
 from dbt.contracts.results import RunResultsArtifact, RunResult, RunStatus, TimingInfo
 from dbt.events.functions import fire_event
 from dbt.events.types import (
     RunningOperationCaughtError,
     RunningOperationUncaughtError,
     LogDebugStackTrace,
 )
+from dbt.exceptions import DbtInternalError
 from dbt.node_types import NodeType
 from dbt.task.base import ConfiguredTask
 
 RESULT_FILE_NAME = "run_results.json"
 
 
 class RunOperationTask(ConfiguredTask):
     def _get_macro_parts(self):
         macro_name = self.args.macro
         if "." in macro_name:
             package_name, macro_name = macro_name.split(".", 1)
         else:
-            package_name = self.config.project_name
+            package_name = None
 
         return package_name, macro_name
 
-    def _run_unsafe(self) -> agate.Table:
+    def _run_unsafe(self, package_name, macro_name) -> agate.Table:
         adapter = get_adapter(self.config)
 
-        package_name, macro_name = self._get_macro_parts()
         macro_kwargs = self.args.args
 
         with adapter.connection_named("macro_{}".format(macro_name)):
             adapter.clear_transaction()
             res = adapter.execute_macro(
                 macro_name, project=package_name, kwargs=macro_kwargs, manifest=self.manifest
             )
@@ -48,30 +48,42 @@
 
     def run(self) -> RunResultsArtifact:
         start = datetime.utcnow()
         self.compile_manifest()
 
         success = True
 
+        package_name, macro_name = self._get_macro_parts()
+
         try:
-            self._run_unsafe()
+            self._run_unsafe(package_name, macro_name)
         except dbt.exceptions.Exception as exc:
             fire_event(RunningOperationCaughtError(exc=str(exc)))
             fire_event(LogDebugStackTrace(exc_info=traceback.format_exc()))
             success = False
         except Exception as exc:
             fire_event(RunningOperationUncaughtError(exc=str(exc)))
             fire_event(LogDebugStackTrace(exc_info=traceback.format_exc()))
             success = False
 
         end = datetime.utcnow()
 
-        package_name, macro_name = self._get_macro_parts()
-        fqn = [NodeType.Operation, package_name, macro_name]
-        unique_id = ".".join(fqn)
+        macro = (
+            self.manifest.find_macro_by_name(macro_name, self.config.project_name, package_name)
+            if self.manifest
+            else None
+        )
+
+        if macro:
+            unique_id = macro.unique_id
+            fqn = unique_id.split(".")
+        else:
+            raise DbtInternalError(
+                f"dbt could not find a macro with the name '{macro_name}' in any package"
+            )
 
         run_result = RunResult(
             adapter_response={},
             status=RunStatus.Success if success else RunStatus.Error,
             execution_time=(end - start).total_seconds(),
             failures=0 if success else 1,
             message=None,
```

### Comparing `dbt-core-1.6.0b4/dbt/task/runnable.py` & `dbt-core-1.6.0b5/dbt/task/runnable.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,17 @@
 
     def _mark_dependent_errors(self, node_id, result, cause):
         if self.graph is None:
             raise DbtInternalError("graph is None in _mark_dependent_errors")
         for dep_node_id in self.graph.get_dependent_nodes(node_id):
             self._skipped_children[dep_node_id] = cause
 
-    def populate_adapter_cache(self, adapter, required_schemas: Set[BaseRelation] = None):
+    def populate_adapter_cache(
+        self, adapter, required_schemas: Optional[Set[BaseRelation]] = None
+    ):
         if not self.args.populate_cache:
             return
 
         start_populate_cache = time.perf_counter()
         if get_flags().CACHE_SELECTED_ONLY is True:
             adapter.set_relations_cache(self.manifest, required_schemas=required_schemas)
         else:
```

### Comparing `dbt-core-1.6.0b4/dbt/task/seed.py` & `dbt-core-1.6.0b5/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/serve.py` & `dbt-core-1.6.0b5/dbt/task/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/show.py` & `dbt-core-1.6.0b5/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/snapshot.py` & `dbt-core-1.6.0b5/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/sql.py` & `dbt-core-1.6.0b5/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/task/test.py` & `dbt-core-1.6.0b5/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/tests/fixtures/project.py` & `dbt-core-1.6.0b5/dbt/tests/fixtures/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,14 +188,32 @@
         elif isinstance(project_config_update, str):
             updates = yaml.safe_load(project_config_update)
             project_config.update(updates)
     write_file(yaml.safe_dump(project_config), project_root, "dbt_project.yml")
     return project_config
 
 
+# Fixture to provide dependencies
+@pytest.fixture(scope="class")
+def dependencies():
+    return {}
+
+
+# Write out the dependencies.yml file
+# Write out the packages.yml file
+@pytest.fixture(scope="class")
+def dependencies_yml(project_root, dependencies):
+    if dependencies:
+        if isinstance(dependencies, str):
+            data = dependencies
+        else:
+            data = yaml.safe_dump(dependencies)
+        write_file(data, project_root, "dependencies.yml")
+
+
 # Fixture to provide packages as either yaml or dictionary
 @pytest.fixture(scope="class")
 def packages():
     return {}
 
 
 # Write out the packages.yml file
@@ -457,14 +475,15 @@
     project_root,
     profiles_root,
     request,
     unique_schema,
     profiles_yml,
     dbt_project_yml,
     packages_yml,
+    dependencies_yml,
     selectors_yml,
     adapter,
     project_files,
     shared_data_dir,
     test_data_dir,
     logs_dir,
     test_config,
```

### Comparing `dbt-core-1.6.0b4/dbt/tests/util.py` & `dbt-core-1.6.0b5/dbt/tests/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from io import StringIO
 import os
 import shutil
 import yaml
 import json
 import warnings
 from datetime import datetime
-from typing import Dict, List
+from typing import Dict, List, Optional
 from contextlib import contextmanager
 from dbt.adapters.factory import Adapter
 
 from dbt.cli.main import dbtRunner
 from dbt.logger import log_manager
 from dbt.contracts.graph.manifest import Manifest
 from dbt.events.functions import (
@@ -67,17 +67,17 @@
 # For a run command (and most other commands) it will return a list
 # of results. For the 'docs generate' command it returns a CatalogArtifact.
 # The first parameter is a list of dbt command line arguments, such as
 #   run_dbt(["run", "--vars", "seed_name: base"])
 # If the command is expected to fail, pass in "expect_pass=False"):
 #   run_dbt("test"], expect_pass=False)
 def run_dbt(
-    args: List[str] = None,
+    args: Optional[List[str]] = None,
     expect_pass: bool = True,
-    publications: List[PublicationArtifact] = None,
+    publications: Optional[List[PublicationArtifact]] = None,
 ):
     # Ignore logbook warnings
     warnings.filterwarnings("ignore", category=DeprecationWarning, module="logbook")
 
     # reset global vars
     reset_metadata_vars()
 
@@ -113,17 +113,17 @@
 
 
 # Use this if you need to capture the command logs in a test.
 # If you want the logs that are normally written to a file, you must
 # start with the "--debug" flag. The structured schema log CI test
 # will turn the logs into json, so you have to be prepared for that.
 def run_dbt_and_capture(
-    args: List[str] = None,
+    args: Optional[List[str]] = None,
     expect_pass: bool = True,
-    publications: List[PublicationArtifact] = None,
+    publications: Optional[List[PublicationArtifact]] = None,
 ):
     try:
         stringbuf = StringIO()
         capture_stdout_logs(stringbuf)
         res = run_dbt(args, expect_pass=expect_pass, publications=publications)
         stdout = stringbuf.getvalue()
```

### Comparing `dbt-core-1.6.0b4/dbt/tracking.py` & `dbt-core-1.6.0b5/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/ui.py` & `dbt-core-1.6.0b5/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/utils.py` & `dbt-core-1.6.0b5/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b4/dbt/version.py` & `dbt-core-1.6.0b5/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.6.0b4"
+__version__ = "1.6.0b5"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.6.0b4/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.6.0b5/dbt_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b4
+Version: 1.6.0b5
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b4 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b5 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b4/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.6.0b5/dbt_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 dbt/contracts/state.py
 dbt/contracts/util.py
 dbt/contracts/graph/__init__.py
 dbt/contracts/graph/manifest.py
 dbt/contracts/graph/manifest_upgrade.py
 dbt/contracts/graph/metrics.py
 dbt/contracts/graph/model_config.py
+dbt/contracts/graph/node_args.py
 dbt/contracts/graph/nodes.py
 dbt/contracts/graph/searcher.py
 dbt/contracts/graph/semantic_models.py
 dbt/contracts/graph/unparsed.py
 dbt/contracts/graph/utils.py
 dbt/deps/__init__.py
 dbt/deps/base.py
```

