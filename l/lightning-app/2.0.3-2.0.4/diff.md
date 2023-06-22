# Comparing `tmp/lightning-app-2.0.3.tar.gz` & `tmp/lightning-app-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-app-2.0.3.tar", last modified: Wed Jun  7 17:10:57 2023, max compression
+gzip compressed data, was "lightning-app-2.0.4.tar", last modified: Thu Jun 22 18:24:49 2023, max compression
```

## Comparing `lightning-app-2.0.3.tar` & `lightning-app-2.0.4.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.924584 lightning-app-2.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/.actions/
--rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-06-07 17:10:40.000000 lightning-app-2.0.3/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-07 17:10:40.000000 lightning-app-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-07 17:10:57.920584 lightning-app-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-06-07 17:10:40.000000 lightning-app-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-07 17:10:40.000000 lightning-app-2.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.888584 lightning-app-2.0.3/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/requirements/app/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/cloud.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/components.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-07 17:10:40.000000 lightning-app-2.0.3/requirements/app/ui.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:10:57.924584 lightning-app-2.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-06-07 17:10:40.000000 lightning-app-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/src/lightning_app/
--rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/src/lightning_app/api/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.888584 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_a/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_b/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_react_ui_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/cmd_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/cd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/commands/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/component-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.888584 lightning-app-2.0.3/src/lightning_app/cli/component-template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/component-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.896584 lightning-app-2.0.3/src/lightning_app/cli/component-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/placeholdername/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/placeholdername/component.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/connect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/connect/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/connect/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/connect/maverick.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/.lightningignore
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.900584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/App.css
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)    55270 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/database/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/database/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/components/multi_node/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/pytorch_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/multi_node/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.904584 lightning-app-2.0.3/src/lightning_app/components/python/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30215 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-06-07 17:10:55.000000 lightning-app-2.0.3/src/lightning_app/components/serve/catimage.png
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/cold_start_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/gradio_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/python_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/core/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19322 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32847 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)    31224 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/frontend/just_py/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/just_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/just_py/just_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/just_py/just_py_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/perf/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/perf/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/plugin/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.908584 lightning-app-2.0.3/src/lightning_app/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    45732 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/runners/runtime_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/source_code/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.912584 lightning-app-2.0.3/src/lightning_app/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/css/main.bb0f092c.css
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/css/main.bb0f092c.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.3/src/lightning_app/ui/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.916584 lightning-app-2.0.3/src/lightning_app/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.3/src/lightning_app/ui/static/lightningState.js
--rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.3/src/lightning_app/ui/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.916584 lightning-app-2.0.3/src/lightning_app/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.3/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.3/src/lightning_app/ui/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.920584 lightning-app-2.0.3/src/lightning_app/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/app_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/cluster_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.920584 lightning-app-2.0.3/src/lightning_app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60255 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.920584 lightning-app-2.0.3/src/lightning_app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    30277 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/safe_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-07 17:10:56.000000 lightning-app-2.0.3/src/lightning_app/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/lightning_app/version.info
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:10:57.892584 lightning-app-2.0.3/src/lightning_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 17:10:57.000000 lightning-app-2.0.3/src/lightning_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 17:10:40.000000 lightning-app-2.0.3/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.249991 lightning-app-2.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-22 18:24:35.000000 lightning-app-2.0.4/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-22 18:24:35.000000 lightning-app-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-22 18:24:49.249991 lightning-app-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-06-22 18:24:35.000000 lightning-app-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-22 18:24:36.000000 lightning-app-2.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.217990 lightning-app-2.0.4/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/requirements/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/cloud.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/components.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 18:24:36.000000 lightning-app-2.0.4/requirements/app/ui.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 18:24:49.249991 lightning-app-2.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-06-22 18:24:36.000000 lightning-app-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/src/lightning_app/
+-rw-r--r--   0 runner    (1001) docker     (123)    34000 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/src/lightning_app/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.217990 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_b/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_react_ui_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/cmd_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/commands/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/component-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.217990 lightning-app-2.0.4/src/lightning_app/cli/component-template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/component-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/component-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/placeholdername/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/placeholdername/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.225990 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/connect/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/connect/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/connect/maverick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/.lightningignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.229990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    55291 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/database/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/database/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/multi_node/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/pytorch_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/multi_node/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.233990 lightning-app-2.0.4/src/lightning_app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30215 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-06-22 18:24:46.000000 lightning-app-2.0.4/src/lightning_app/components/serve/catimage.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/cold_start_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/gradio_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/python_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32847 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31224 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/frontend/just_py/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/just_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/just_py/just_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/just_py/just_py_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/perf/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/perf/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/plugin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.237990 lightning-app-2.0.4/src/lightning_app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45732 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/runners/runtime_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/css/main.bb0f092c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/css/main.bb0f092c.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.4/src/lightning_app/ui/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.241990 lightning-app-2.0.4/src/lightning_app/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.4/src/lightning_app/ui/static/lightningState.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.4/src/lightning_app/ui/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.245990 lightning-app-2.0.4/src/lightning_app/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.4/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.4/src/lightning_app/ui/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.249991 lightning-app-2.0.4/src/lightning_app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/cluster_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.249991 lightning-app-2.0.4/src/lightning_app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60255 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.249991 lightning-app-2.0.4/src/lightning_app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30277 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/safe_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-22 18:24:48.000000 lightning-app-2.0.4/src/lightning_app/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/lightning_app/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:24:49.221990 lightning-app-2.0.4/src/lightning_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 18:24:49.000000 lightning-app-2.0.4/src/lightning_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:24:36.000000 lightning-app-2.0.4/src/version.info
```

### Comparing `lightning-app-2.0.3/.actions/assistant.py` & `lightning-app-2.0.4/.actions/assistant.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import glob
+import logging
 import os
 import pathlib
 import re
 import shutil
 import tarfile
 import tempfile
 import urllib.request
@@ -138,15 +139,15 @@
 
 
 def load_requirements(path_dir: str, file_name: str = "base.txt", unfreeze: str = "all") -> List[str]:
     """Loading requirements from a file.
 
     >>> path_req = os.path.join(_PROJECT_ROOT, "requirements")
     >>> load_requirements(path_req, "docs.txt", unfreeze="major")  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-    ['sphinx<6.0,>=4.0', ...]
+    ['sphinx<...]
     """
     assert unfreeze in {"none", "major", "all"}
     path = Path(path_dir) / file_name
     assert path.exists(), (path_dir, file_name, path)
     text = path.read_text()
     return [req.adjust(unfreeze) for req in _parse_requirements(text)]
 
@@ -417,12 +418,48 @@
         """Copy package content with import adjustments."""
         source_imports = source_import.strip().split(",")
         target_imports = target_import.strip().split(",")
         copy_replace_imports(
             source_dir, source_imports, target_imports, target_dir=target_dir, lightning_by=lightning_by
         )
 
+    @staticmethod
+    def pull_docs_files(
+        gh_user_repo: str,
+        target_dir: str = "docs/source-pytorch/XXX",
+        checkout: str = "tags/1.0.0",
+        source_dir: str = "docs/source",
+    ) -> None:
+        """Pull docs pages from external source and append to local docs."""
+        import zipfile
+
+        zip_url = f"https://github.com/{gh_user_repo}/archive/refs/{checkout}.zip"
+
+        with tempfile.TemporaryDirectory() as tmp:
+            zip_file = os.path.join(tmp, "repo.zip")
+            urllib.request.urlretrieve(zip_url, zip_file)
+
+            with zipfile.ZipFile(zip_file, "r") as zip_ref:
+                zip_ref.extractall(tmp)
+
+            zip_dirs = [d for d in glob.glob(os.path.join(tmp, "*")) if os.path.isdir(d)]
+            # check that the extracted archive has only repo folder
+            assert len(zip_dirs) == 1
+            repo_dir = zip_dirs[0]
+
+            ls_pages = glob.glob(os.path.join(repo_dir, source_dir, "*.rst"))
+            ls_pages += glob.glob(os.path.join(repo_dir, source_dir, "**", "*.rst"))
+            for rst in ls_pages:
+                rel_rst = rst.replace(os.path.join(repo_dir, source_dir) + os.path.sep, "")
+                rel_dir = os.path.dirname(rel_rst)
+                os.makedirs(os.path.join(_PROJECT_ROOT, target_dir, rel_dir), exist_ok=True)
+                new_rst = os.path.join(_PROJECT_ROOT, target_dir, rel_rst)
+                if os.path.isfile(new_rst):
+                    logging.warning(f"Page {new_rst} already exists in the local tree so it will be skipped.")
+                    continue
+                shutil.copy(rst, new_rst)
+
 
 if __name__ == "__main__":
     import jsonargparse
 
     jsonargparse.CLI(AssistantCLI, as_positional=False)
```

### Comparing `lightning-app-2.0.3/LICENSE` & `lightning-app-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/PKG-INFO` & `lightning-app-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.3
+Version: 2.0.4
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,18 +21,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: cloud
 Provides-Extra: ui
 Provides-Extra: components
-Provides-Extra: cloud
-Provides-Extra: test
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.3 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.4 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
@@ -10,16 +10,16 @@
 Language :: English Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: ui Provides-Extra: components
-Provides-Extra: cloud Provides-Extra: test Provides-Extra: extra Provides-
+Content-Type: text/markdown Provides-Extra: test Provides-Extra: cloud
+Provides-Extra: ui Provides-Extra: components Provides-Extra: extra Provides-
 Extra: all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
```

### Comparing `lightning-app-2.0.3/README.md` & `lightning-app-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/pyproject.toml` & `lightning-app-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/requirements/app/base.txt` & `lightning-app-2.0.4/requirements/app/base.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 deepdiff >=5.7.0, <6.3.1
 starsessions >=1.2.1, <2.0 # strict
 fsspec >=2022.5.0, <=2022.7.1
 croniter >=1.3.0, <1.4.0  # strict; TODO: for now until we find something more robust.
 traitlets >=5.3.0, <5.10.0
 arrow >=1.2.0, <1.2.4
 lightning-utilities >=0.7.0, <0.9.0
-beautifulsoup4 >=4.8.0, <4.11.2
+beautifulsoup4 >=4.8.0, <4.12.3
 inquirer >=2.10.0, <=3.1.3
 psutil <5.9.5
 click <=8.1.3
 python-multipart>=0.0.5, <=0.0.6
 
-fastapi >=0.69.0, <0.89.0  # strict; TODO: broken serializations
+fastapi >=0.92.0, <0.98.0
 starlette  # https://fastapi.tiangolo.com/deployment/versions/#about-starlette
 pydantic >=1.7.4, <2.0.0  # https://fastapi.tiangolo.com/deployment/versions/#about-pydantic
 
 dateutils <=0.6.12
 Jinja2 <=3.1.2
 PyYAML <=6.0
-requests <2.28.3
-rich >=12.3.0, <=13.0.1
-urllib3 <=1.26.13
+requests <2.31.1
+rich >=12.3.0, <=13.4.2
+urllib3 <=2.0.2
 uvicorn <=0.22.0
-websocket-client <1.5.2
+websocket-client <1.5.3
 websockets <=10.4
```

### Comparing `lightning-app-2.0.3/setup.py` & `lightning-app-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/CHANGELOG.md` & `lightning-app-2.0.4/src/lightning_app/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.0.4] - 2023-06-22
+
+### Fixed
+
+- bumped several dependencies to address security volnebilities.
+
+
 ## [2.0.3] - 2023-06-07
 
 - Added the property `LightningWork.public_ip` that exposes the public IP of the `LightningWork` instance ([#17742](https://github.com/Lightning-AI/lightning/pull/17742))
 - Add missing python-multipart dependency ([#17244](https://github.com/Lightning-AI/lightning/pull/17244))
 
 ### Changed
```

### Comparing `lightning-app-2.0.3/src/lightning_app/README.md` & `lightning-app-2.0.4/src/lightning_app/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/__about__.py` & `lightning-app-2.0.4/src/lightning_app/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/__init__.py` & `lightning-app-2.0.4/src/lightning_app/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/__setup__.py` & `lightning-app-2.0.4/src/lightning_app/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/api/http_methods.py` & `lightning-app-2.0.4/src/lightning_app/api/http_methods.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/api/request_types.py` & `lightning-app-2.0.4/src/lightning_app/api/request_types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/app-template/.gitignore` & `lightning-app-2.0.4/src/lightning_app/cli/app-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/app-template/LICENSE` & `lightning-app-2.0.4/src/lightning_app/cli/app-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/app-template/README.md` & `lightning-app-2.0.4/src/lightning_app/cli/app-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py` & `lightning-app-2.0.4/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/cmd_apps.py` & `lightning-app-2.0.4/src/lightning_app/cli/cmd_apps.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/cmd_clusters.py` & `lightning-app-2.0.4/src/lightning_app/cli/cmd_clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/cmd_init.py` & `lightning-app-2.0.4/src/lightning_app/cli/cmd_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/cmd_install.py` & `lightning-app-2.0.4/src/lightning_app/cli/cmd_install.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/cmd_pl_init.py` & `lightning-app-2.0.4/src/lightning_app/cli/cmd_pl_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/cmd_react_ui_init.py` & `lightning-app-2.0.4/src/lightning_app/cli/cmd_react_ui_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/cmd_ssh_keys.py` & `lightning-app-2.0.4/src/lightning_app/cli/cmd_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/commands/app_commands.py` & `lightning-app-2.0.4/src/lightning_app/cli/commands/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/commands/cd.py` & `lightning-app-2.0.4/src/lightning_app/cli/commands/cd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/commands/cp.py` & `lightning-app-2.0.4/src/lightning_app/cli/commands/cp.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/commands/logs.py` & `lightning-app-2.0.4/src/lightning_app/cli/commands/logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/commands/ls.py` & `lightning-app-2.0.4/src/lightning_app/cli/commands/ls.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/commands/pwd.py` & `lightning-app-2.0.4/src/lightning_app/cli/commands/pwd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/commands/rm.py` & `lightning-app-2.0.4/src/lightning_app/cli/commands/rm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml` & `lightning-app-2.0.4/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/component-template/.gitignore` & `lightning-app-2.0.4/src/lightning_app/cli/component-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/component-template/LICENSE` & `lightning-app-2.0.4/src/lightning_app/cli/component-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/component-template/README.md` & `lightning-app-2.0.4/src/lightning_app/cli/component-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/connect/app.py` & `lightning-app-2.0.4/src/lightning_app/cli/connect/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/connect/data.py` & `lightning-app-2.0.4/src/lightning_app/cli/connect/data.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/connect/maverick.py` & `lightning-app-2.0.4/src/lightning_app/cli/connect/maverick.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/core.py` & `lightning-app-2.0.4/src/lightning_app/cli/core.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/lightning_cli.py` & `lightning-app-2.0.4/src/lightning_app/cli/lightning_cli.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_create.py` & `lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_create.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_delete.py` & `lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_delete.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/lightning_cli_list.py` & `lightning-app-2.0.4/src/lightning_app/cli/lightning_cli_list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/app.py` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/callbacks.py` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/core/state.py` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/core/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/setup.py` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/.prettierrc` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/.prettierrc`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/craco.config.js` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/craco.config.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/package.json` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/public/index.html` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/public/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/App.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/index.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/pl-app-template/ui/tsconfig.json` & `lightning-app-2.0.4/src/lightning_app/cli/pl-app-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/README.md` & `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/example_app.py` & `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/example_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/package.json` & `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/package.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'devDependencies'": "{'vite': '^2.9.16'}"}*

```diff
@@ -12,15 +12,15 @@
     "devDependencies": {
         "@types/lodash": "^4.14.179",
         "@types/react": "^18.0.1",
         "@types/react-dom": "^18.0.0",
         "@vitejs/plugin-react": "^1.0.7",
         "prettier": "^2.5.1",
         "typescript": "^4.5.4",
-        "vite": "^2.8.6"
+        "vite": "^2.9.16"
     },
     "license": "MIT",
     "main": "index.js",
     "name": "hello-world",
     "private": true,
     "scripts": {
         "build": "tsc --noEmit && vite build",
```

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/App.tsx` & `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg` & `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts` & `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/tsconfig.json` & `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/cli/react-ui-template/ui/yarn.lock` & `lightning-app-2.0.4/src/lightning_app/cli/react-ui-template/ui/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1046,18 +1046,18 @@
   resolved "https://registry.yarnpkg.com/resolve/-/resolve-1.22.1.tgz#27cb2ebb53f91abb49470a928bba7558066ac177"
   integrity sha512-nBpuuYuY5jFsli/JIs1oldw6fOQCBioohqWZg/2hiaOybXOft4lonv85uDOKXdf8rhyK159cxU5cDcK/NKk8zw==
   dependencies:
     is-core-module "^2.9.0"
     path-parse "^1.0.7"
     supports-preserve-symlinks-flag "^1.0.0"
 
-rollup@^2.59.0:
-  version "2.75.7"
-  resolved "https://registry.yarnpkg.com/rollup/-/rollup-2.75.7.tgz#221ff11887ae271e37dcc649ba32ce1590aaa0b9"
-  integrity sha512-VSE1iy0eaAYNCxEXaleThdFXqZJ42qDBatAwrfnPlENEZ8erQ+0LYX4JXOLPceWfZpV1VtZwZ3dFCuOZiSyFtQ==
+"rollup@>=2.59.0 <2.78.0":
+  version "2.77.3"
+  resolved "https://registry.yarnpkg.com/rollup/-/rollup-2.77.3.tgz#8f00418d3a2740036e15deb653bed1a90ee0cc12"
+  integrity sha512-/qxNTG7FbmefJWoeeYJFbHehJ2HNWnjkAFRKzWN/45eNBBF/r8lo992CwcJXEzyVxs5FmfId+vTSTQDb+bxA+g==
   optionalDependencies:
     fsevents "~2.3.2"
 
 safe-buffer@~5.1.1:
   version "5.1.2"
   resolved "https://registry.yarnpkg.com/safe-buffer/-/safe-buffer-5.1.2.tgz#991ec69d296e0313747d59bdfd2b745c35f8828d"
   integrity sha512-Gd2UZBJDkXlY7GbJxfsE8/nvKkUEU1G38c1siN6QP6a9PT9MmHB8GnpscSmMJSoF8LOIrt8ud/wPtojys4G6+g==
@@ -1116,23 +1116,23 @@
   version "1.0.4"
   resolved "https://registry.yarnpkg.com/update-browserslist-db/-/update-browserslist-db-1.0.4.tgz#dbfc5a789caa26b1db8990796c2c8ebbce304824"
   integrity sha512-jnmO2BEGUjsMOe/Fg9u0oczOe/ppIDZPebzccl1yDWGLFP16Pa1/RM5wEoKYPG2zstNcDuAStejyxsOuKINdGA==
   dependencies:
     escalade "^3.1.1"
     picocolors "^1.0.0"
 
-vite@^2.8.6:
-  version "2.9.13"
-  resolved "https://registry.yarnpkg.com/vite/-/vite-2.9.13.tgz#859cb5d4c316c0d8c6ec9866045c0f7858ca6abc"
-  integrity sha512-AsOBAaT0AD7Mhe8DuK+/kE4aWYFMx/i0ZNi98hJclxb4e0OhQcZYUrvLjIaQ8e59Ui7txcvKMiJC1yftqpQoDw==
+vite@^2.9.16:
+  version "2.9.16"
+  resolved "https://registry.yarnpkg.com/vite/-/vite-2.9.16.tgz#daf7ba50f5cc37a7bf51b118ba06bc36e97898e9"
+  integrity sha512-X+6q8KPyeuBvTQV8AVSnKDvXoBMnTx8zxh54sOwmmuOdxkjMmEJXH2UEchA+vTMps1xw9vL64uwJOWryULg7nA==
   dependencies:
     esbuild "^0.14.27"
     postcss "^8.4.13"
     resolve "^1.22.0"
-    rollup "^2.59.0"
+    rollup ">=2.59.0 <2.78.0"
   optionalDependencies:
     fsevents "~2.3.2"
 
 yaml@^1.7.2:
   version "1.10.2"
   resolved "https://registry.yarnpkg.com/yaml/-/yaml-1.10.2.tgz#2301c5ffbf12b467de8da2333a459e29e7920e4b"
   integrity sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==
```

### Comparing `lightning-app-2.0.3/src/lightning_app/components/__init__.py` & `lightning-app-2.0.4/src/lightning_app/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/database/client.py` & `lightning-app-2.0.4/src/lightning_app/components/database/client.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/database/server.py` & `lightning-app-2.0.4/src/lightning_app/components/database/server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/database/utilities.py` & `lightning-app-2.0.4/src/lightning_app/components/database/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/multi_node/base.py` & `lightning-app-2.0.4/src/lightning_app/components/multi_node/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/multi_node/fabric.py` & `lightning-app-2.0.4/src/lightning_app/components/multi_node/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/multi_node/pytorch_spawn.py` & `lightning-app-2.0.4/src/lightning_app/components/multi_node/pytorch_spawn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/multi_node/trainer.py` & `lightning-app-2.0.4/src/lightning_app/components/multi_node/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/python/popen.py` & `lightning-app-2.0.4/src/lightning_app/components/python/popen.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/python/tracer.py` & `lightning-app-2.0.4/src/lightning_app/components/python/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/__init__.py` & `lightning-app-2.0.4/src/lightning_app/components/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/auto_scaler.py` & `lightning-app-2.0.4/src/lightning_app/components/serve/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/catimage.png` & `lightning-app-2.0.4/src/lightning_app/components/serve/catimage.png`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/cold_start_proxy.py` & `lightning-app-2.0.4/src/lightning_app/components/serve/cold_start_proxy.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/gradio_server.py` & `lightning-app-2.0.4/src/lightning_app/components/serve/gradio_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/python_server.py` & `lightning-app-2.0.4/src/lightning_app/components/serve/python_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/serve.py` & `lightning-app-2.0.4/src/lightning_app/components/serve/serve.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/streamlit.py` & `lightning-app-2.0.4/src/lightning_app/components/serve/streamlit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/types/image.py` & `lightning-app-2.0.4/src/lightning_app/components/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/serve/types/type.py` & `lightning-app-2.0.4/src/lightning_app/components/serve/types/type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/components/training.py` & `lightning-app-2.0.4/src/lightning_app/components/training.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/core/api.py` & `lightning-app-2.0.4/src/lightning_app/core/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,24 +227,24 @@
     if isinstance(child["vars"]["_layout"], list):
         assert len(child["vars"]["_layout"]) == 1
         return child["vars"]["_layout"][0]["target"]
     return child["vars"]["_layout"]["target"]
 
 
 @fastapi_service.get("/api/v1/layout", response_class=JSONResponse)
-async def get_layout() -> Mapping:
+async def get_layout() -> str:
     with lock:
         x_lightning_session_uuid = TEST_SESSION_UUID
         state = global_app_state_store.get_app_state(x_lightning_session_uuid)
         global_app_state_store.set_served_state(x_lightning_session_uuid, state)
         layout = deepcopy(state["vars"]["_layout"])
         for la in layout:
             if la["content"].startswith("root."):
                 la["content"] = _get_component_by_name(la["content"], state)
-        return layout
+        return json.dumps(layout)
 
 
 @fastapi_service.get("/api/v1/spec", response_class=JSONResponse)
 async def get_spec(
     response: Response,
     x_lightning_session_uuid: Optional[str] = Header(None),  # type: ignore[assignment]
     x_lightning_session_id: Optional[str] = Header(None),  # type: ignore[assignment]
```

### Comparing `lightning-app-2.0.3/src/lightning_app/core/app.py` & `lightning-app-2.0.4/src/lightning_app/core/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/core/constants.py` & `lightning-app-2.0.4/src/lightning_app/core/constants.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/core/flow.py` & `lightning-app-2.0.4/src/lightning_app/core/flow.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/core/queues.py` & `lightning-app-2.0.4/src/lightning_app/core/queues.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/core/work.py` & `lightning-app-2.0.4/src/lightning_app/core/work.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/frontend.py` & `lightning-app-2.0.4/src/lightning_app/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/just_py/just_py.py` & `lightning-app-2.0.4/src/lightning_app/frontend/just_py/just_py.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/just_py/just_py_base.py` & `lightning-app-2.0.4/src/lightning_app/frontend/just_py/just_py_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/panel/app_state_comm.py` & `lightning-app-2.0.4/src/lightning_app/frontend/panel/app_state_comm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/panel/app_state_watcher.py` & `lightning-app-2.0.4/src/lightning_app/frontend/panel/app_state_watcher.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/panel/panel_frontend.py` & `lightning-app-2.0.4/src/lightning_app/frontend/panel/panel_frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/panel/panel_serve_render_fn.py` & `lightning-app-2.0.4/src/lightning_app/frontend/panel/panel_serve_render_fn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/stream_lit.py` & `lightning-app-2.0.4/src/lightning_app/frontend/stream_lit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/streamlit_base.py` & `lightning-app-2.0.4/src/lightning_app/frontend/streamlit_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/utils.py` & `lightning-app-2.0.4/src/lightning_app/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/frontend/web.py` & `lightning-app-2.0.4/src/lightning_app/frontend/web.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/perf/pdb.py` & `lightning-app-2.0.4/src/lightning_app/perf/pdb.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/plugin/actions.py` & `lightning-app-2.0.4/src/lightning_app/plugin/actions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/plugin/plugin.py` & `lightning-app-2.0.4/src/lightning_app/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/runners/backends/__init__.py` & `lightning-app-2.0.4/src/lightning_app/runners/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/runners/backends/backend.py` & `lightning-app-2.0.4/src/lightning_app/runners/backends/backend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/runners/backends/cloud.py` & `lightning-app-2.0.4/src/lightning_app/runners/backends/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/runners/backends/docker.py` & `lightning-app-2.0.4/src/lightning_app/runners/backends/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/runners/backends/mp_process.py` & `lightning-app-2.0.4/src/lightning_app/runners/backends/mp_process.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/runners/cloud.py` & `lightning-app-2.0.4/src/lightning_app/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/runners/multiprocess.py` & `lightning-app-2.0.4/src/lightning_app/runners/multiprocess.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/runners/runtime.py` & `lightning-app-2.0.4/src/lightning_app/runners/runtime.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/runners/runtime_type.py` & `lightning-app-2.0.4/src/lightning_app/runners/runtime_type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/source_code/copytree.py` & `lightning-app-2.0.4/src/lightning_app/source_code/copytree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/source_code/hashing.py` & `lightning-app-2.0.4/src/lightning_app/source_code/hashing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/source_code/local.py` & `lightning-app-2.0.4/src/lightning_app/source_code/local.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/source_code/tar.py` & `lightning-app-2.0.4/src/lightning_app/source_code/tar.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/source_code/uploader.py` & `lightning-app-2.0.4/src/lightning_app/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/storage/copier.py` & `lightning-app-2.0.4/src/lightning_app/storage/copier.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/storage/drive.py` & `lightning-app-2.0.4/src/lightning_app/storage/drive.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/storage/filesystem.py` & `lightning-app-2.0.4/src/lightning_app/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/storage/mount.py` & `lightning-app-2.0.4/src/lightning_app/storage/mount.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/storage/orchestrator.py` & `lightning-app-2.0.4/src/lightning_app/storage/orchestrator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/storage/path.py` & `lightning-app-2.0.4/src/lightning_app/storage/path.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/storage/payload.py` & `lightning-app-2.0.4/src/lightning_app/storage/payload.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/storage/requests.py` & `lightning-app-2.0.4/src/lightning_app/storage/requests.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/structures/dict.py` & `lightning-app-2.0.4/src/lightning_app/structures/dict.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/structures/list.py` & `lightning-app-2.0.4/src/lightning_app/structures/list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/testing/config.py` & `lightning-app-2.0.4/src/lightning_app/testing/config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/testing/helpers.py` & `lightning-app-2.0.4/src/lightning_app/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/testing/testing.py` & `lightning-app-2.0.4/src/lightning_app/testing/testing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/asset-manifest.json` & `lightning-app-2.0.4/src/lightning_app/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/index.html` & `lightning-app-2.0.4/src/lightning_app/ui/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/css/main.bb0f092c.css` & `lightning-app-2.0.4/src/lightning_app/ui/static/css/main.bb0f092c.css`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/css/main.bb0f092c.css.map` & `lightning-app-2.0.4/src/lightning_app/ui/static/css/main.bb0f092c.css.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/favicon.ico` & `lightning-app-2.0.4/src/lightning_app/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js` & `lightning-app-2.0.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map` & `lightning-app-2.0.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js` & `lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt` & `lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/js/main.2b242b99.js.map` & `lightning-app-2.0.4/src/lightning_app/ui/static/js/main.2b242b99.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/lightningState.js` & `lightning-app-2.0.4/src/lightning_app/ui/static/lightningState.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2` & `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff` & `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff` & `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2` & `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2` & `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff` & `lightning-app-2.0.4/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg` & `lightning-app-2.0.4/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg` & `lightning-app-2.0.4/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/app_commands.py` & `lightning-app-2.0.4/src/lightning_app/utilities/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/app_helpers.py` & `lightning-app-2.0.4/src/lightning_app/utilities/app_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/app_logs.py` & `lightning-app-2.0.4/src/lightning_app/utilities/app_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/app_status.py` & `lightning-app-2.0.4/src/lightning_app/utilities/app_status.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/auth.py` & `lightning-app-2.0.4/src/lightning_app/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/cli_helpers.py` & `lightning-app-2.0.4/src/lightning_app/utilities/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/cloud.py` & `lightning-app-2.0.4/src/lightning_app/utilities/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/cluster_logs.py` & `lightning-app-2.0.4/src/lightning_app/utilities/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/clusters.py` & `lightning-app-2.0.4/src/lightning_app/utilities/clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/commands/base.py` & `lightning-app-2.0.4/src/lightning_app/utilities/commands/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/component.py` & `lightning-app-2.0.4/src/lightning_app/utilities/component.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/data_structures.py` & `lightning-app-2.0.4/src/lightning_app/utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/dependency_caching.py` & `lightning-app-2.0.4/src/lightning_app/utilities/dependency_caching.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/enum.py` & `lightning-app-2.0.4/src/lightning_app/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/exceptions.py` & `lightning-app-2.0.4/src/lightning_app/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/frontend.py` & `lightning-app-2.0.4/src/lightning_app/utilities/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/git.py` & `lightning-app-2.0.4/src/lightning_app/utilities/git.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/imports.py` & `lightning-app-2.0.4/src/lightning_app/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/introspection.py` & `lightning-app-2.0.4/src/lightning_app/utilities/introspection.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/layout.py` & `lightning-app-2.0.4/src/lightning_app/utilities/layout.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/load_app.py` & `lightning-app-2.0.4/src/lightning_app/utilities/load_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/log.py` & `lightning-app-2.0.4/src/lightning_app/utilities/log.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/log_helpers.py` & `lightning-app-2.0.4/src/lightning_app/utilities/log_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/login.py` & `lightning-app-2.0.4/src/lightning_app/utilities/login.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/logs_socket_api.py` & `lightning-app-2.0.4/src/lightning_app/utilities/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/name_generator.py` & `lightning-app-2.0.4/src/lightning_app/utilities/name_generator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/network.py` & `lightning-app-2.0.4/src/lightning_app/utilities/network.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/openapi.py` & `lightning-app-2.0.4/src/lightning_app/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/packaging/app_config.py` & `lightning-app-2.0.4/src/lightning_app/utilities/packaging/app_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/packaging/build_config.py` & `lightning-app-2.0.4/src/lightning_app/utilities/packaging/build_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/packaging/cloud_compute.py` & `lightning-app-2.0.4/src/lightning_app/utilities/packaging/cloud_compute.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/packaging/docker.py` & `lightning-app-2.0.4/src/lightning_app/utilities/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/packaging/lightning_utils.py` & `lightning-app-2.0.4/src/lightning_app/utilities/packaging/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/packaging/tarfile.py` & `lightning-app-2.0.4/src/lightning_app/utilities/packaging/tarfile.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/port.py` & `lightning-app-2.0.4/src/lightning_app/utilities/port.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/proxies.py` & `lightning-app-2.0.4/src/lightning_app/utilities/proxies.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/redis.py` & `lightning-app-2.0.4/src/lightning_app/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/safe_pickle.py` & `lightning-app-2.0.4/src/lightning_app/utilities/safe_pickle.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/scheduler.py` & `lightning-app-2.0.4/src/lightning_app/utilities/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/secrets.py` & `lightning-app-2.0.4/src/lightning_app/utilities/secrets.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/state.py` & `lightning-app-2.0.4/src/lightning_app/utilities/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/tracer.py` & `lightning-app-2.0.4/src/lightning_app/utilities/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/tree.py` & `lightning-app-2.0.4/src/lightning_app/utilities/tree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/types.py` & `lightning-app-2.0.4/src/lightning_app/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app/utilities/warnings.py` & `lightning-app-2.0.4/src/lightning_app/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app.egg-info/PKG-INFO` & `lightning-app-2.0.4/src/lightning_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.3
+Version: 2.0.4
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,18 +21,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: cloud
 Provides-Extra: ui
 Provides-Extra: components
-Provides-Extra: cloud
-Provides-Extra: test
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.3 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.4 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
@@ -10,16 +10,16 @@
 Language :: English Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: ui Provides-Extra: components
-Provides-Extra: cloud Provides-Extra: test Provides-Extra: extra Provides-
+Content-Type: text/markdown Provides-Extra: test Provides-Extra: cloud
+Provides-Extra: ui Provides-Extra: components Provides-Extra: extra Provides-
 Extra: all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
```

### Comparing `lightning-app-2.0.3/src/lightning_app.egg-info/SOURCES.txt` & `lightning-app-2.0.4/src/lightning_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.3/src/lightning_app.egg-info/requires.txt` & `lightning-app-2.0.4/src/lightning_app.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,97 +9,97 @@
 arrow<2.0,>=1.2.0
 lightning-utilities<1.0,>=0.7.0
 beautifulsoup4<5.0,>=4.8.0
 inquirer<4.0,>=2.10.0
 psutil<6.0
 click<9.0
 python-multipart<1.0,>=0.0.5
-fastapi<0.89.0,>=0.69.0
+fastapi<1.0,>=0.92.0
 starlette
 pydantic<3.0,>=1.7.4
 dateutils<1.0
 Jinja2<4.0
 PyYAML<7.0
 requests<3.0
 rich<14.0,>=12.3.0
-urllib3<2.0
+urllib3<3.0
 uvicorn<1.0
 websocket-client<2.0
 websockets<11.0
 
 [all]
 redis<5.0,>=4.0.1
 docker<7.0,>=5.0.0
-s3fs<2023.0,>=2022.5.0
+s3fs<2024.0,>=2022.5.0
 streamlit<2.0,>=1.13.0
-panel<1.0,>=0.12.7
+panel<2.0,>=1.0.0
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
 
 [cloud]
 redis<5.0,>=4.0.1
 docker<7.0,>=5.0.0
-s3fs<2023.0,>=2022.5.0
+s3fs<2024.0,>=2022.5.0
 
 [components]
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
 
 [dev]
 redis<5.0,>=4.0.1
 docker<7.0,>=5.0.0
-s3fs<2023.0,>=2022.5.0
+s3fs<2024.0,>=2022.5.0
 streamlit<2.0,>=1.13.0
-panel<1.0,>=0.12.7
+panel<2.0,>=1.0.0
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
 coverage==7.2.5
 pytest==7.3.1
 pytest-timeout==2.1.0
 pytest-cov==4.0.0
 pytest-doctestplus>=0.9.0
-pytest-asyncio==0.20.3
+pytest-asyncio==0.21.0
 pytest-rerunfailures<12.0
-playwright==1.32.1
-httpx
+playwright==1.35.0
+httpx==0.24.1
 trio<0.22.0
 pympler
 psutil
 setuptools<68.0
 requests-mock
 
 [extra]
 redis<5.0,>=4.0.1
 docker<7.0,>=5.0.0
-s3fs<2023.0,>=2022.5.0
+s3fs<2024.0,>=2022.5.0
 streamlit<2.0,>=1.13.0
-panel<1.0,>=0.12.7
+panel<2.0,>=1.0.0
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
 
 [test]
 coverage==7.2.5
 pytest==7.3.1
 pytest-timeout==2.1.0
 pytest-cov==4.0.0
 pytest-doctestplus>=0.9.0
-pytest-asyncio==0.20.3
+pytest-asyncio==0.21.0
 pytest-rerunfailures<12.0
-playwright==1.32.1
-httpx
+playwright==1.35.0
+httpx==0.24.1
 trio<0.22.0
 pympler
 psutil
 setuptools<68.0
 requests-mock
 
 [ui]
 streamlit<2.0,>=1.13.0
-panel<1.0,>=0.12.7
+panel<2.0,>=1.0.0
```

