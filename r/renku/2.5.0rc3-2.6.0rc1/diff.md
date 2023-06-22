# Comparing `tmp/renku-2.5.0rc3.tar.gz` & `tmp/renku-2.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renku-2.5.0rc3.tar", max compression
+gzip compressed data, was "renku-2.6.0rc1.tar", max compression
```

## Comparing `renku-2.5.0rc3.tar` & `renku-2.6.0rc1.tar`

### file list

```diff
@@ -1,676 +1,679 @@
--rw-r--r--   0        0        0      900 2023-06-14 08:18:31.715133 renku-2.5.0rc3/AUTHORS.rst
--rw-r--r--   0        0        0   181751 2023-06-14 08:18:31.715133 renku-2.5.0rc3/CHANGES.rst
--rw-r--r--   0        0        0    11358 2023-06-14 08:18:31.715133 renku-2.5.0rc3/LICENSE
--rw-r--r--   0        0        0    12889 2023-06-14 08:18:31.715133 renku-2.5.0rc3/README.rst
--rw-r--r--   0        0        0    10490 2023-06-14 08:19:27.206626 renku-2.5.0rc3/pyproject.toml
--rw-r--r--   0        0        0     4391 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/__init__.py
--rw-r--r--   0        0        0      784 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/__init__.py
--rw-r--r--   0        0        0      209 2023-06-14 08:19:22.230670 renku-2.5.0rc3/renku/command/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      437 2023-06-14 08:19:22.230670 renku-2.5.0rc3/renku/command/__pycache__/options.cpython-39.pyc
--rw-r--r--   0        0        0     1057 2023-06-14 08:19:25.354642 renku-2.5.0rc3/renku/command/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     1343 2023-06-14 08:19:22.230670 renku-2.5.0rc3/renku/command/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0      593 2023-06-14 08:19:22.230670 renku-2.5.0rc3/renku/command/__pycache__/version.cpython-39.pyc
--rw-r--r--   0        0        0     2096 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/checks/__init__.py
--rw-r--r--   0        0        0     4808 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/checks/activities.py
--rw-r--r--   0        0        0     8408 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/checks/datasets.py
--rw-r--r--   0        0        0     2797 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/checks/githooks.py
--rw-r--r--   0        0        0     1548 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/checks/migration.py
--rw-r--r--   0        0        0     2448 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/checks/project.py
--rw-r--r--   0        0        0     1572 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/checks/storage.py
--rw-r--r--   0        0        0     4124 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/checks/validate_shacl.py
--rw-r--r--   0        0        0     5025 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/checks/workflow.py
--rw-r--r--   0        0        0     3872 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/clone.py
--rw-r--r--   0        0        0      828 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/command_builder/__init__.py
--rw-r--r--   0        0        0      301 2023-06-14 08:19:22.838664 renku-2.5.0rc3/renku/command/command_builder/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    15431 2023-06-14 08:19:22.838664 renku-2.5.0rc3/renku/command/command_builder/__pycache__/command.cpython-39.pyc
--rw-r--r--   0        0        0    16678 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/command_builder/command.py
--rw-r--r--   0        0        0     1951 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/command_builder/communication.py
--rw-r--r--   0        0        0     5325 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/command_builder/database.py
--rw-r--r--   0        0        0     1701 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/command_builder/lock.py
--rw-r--r--   0        0        0     1481 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/command_builder/migration.py
--rw-r--r--   0        0        0     7694 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/command_builder/repo.py
--rw-r--r--   0        0        0     4803 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/config.py
--rw-r--r--   0        0        0     5640 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/dataset.py
--rw-r--r--   0        0        0     2835 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/doctor.py
--rw-r--r--   0        0        0      775 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/format/__init__.py
--rw-r--r--   0        0        0      220 2023-06-14 08:19:22.438668 renku-2.5.0rc3/renku/command/format/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5765 2023-06-14 08:19:22.442668 renku-2.5.0rc3/renku/command/format/__pycache__/dataset_files.cpython-39.pyc
--rw-r--r--   0        0        0     1508 2023-06-14 08:19:22.442668 renku-2.5.0rc3/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc
--rw-r--r--   0        0        0     2884 2023-06-14 08:19:22.442668 renku-2.5.0rc3/renku/command/format/__pycache__/datasets.cpython-39.pyc
--rw-r--r--   0        0        0      817 2023-06-14 08:19:24.498650 renku-2.5.0rc3/renku/command/format/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0     1754 2023-06-14 08:19:25.370642 renku-2.5.0rc3/renku/command/format/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     1929 2023-06-14 08:19:24.498650 renku-2.5.0rc3/renku/command/format/__pycache__/tabulate.cpython-39.pyc
--rw-r--r--   0        0        0     2416 2023-06-14 08:19:24.498650 renku-2.5.0rc3/renku/command/format/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0        0        0     2643 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/format/activity.py
--rw-r--r--   0        0        0     6230 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/format/dataset_files.py
--rw-r--r--   0        0        0     2098 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/format/dataset_tags.py
--rw-r--r--   0        0        0     3236 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/format/datasets.py
--rw-r--r--   0        0        0     1212 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/format/json.py
--rw-r--r--   0        0        0     2402 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/format/session.py
--rw-r--r--   0        0        0     2769 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/format/tabulate.py
--rw-r--r--   0        0        0     2728 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/format/workflow.py
--rw-r--r--   0        0        0     1012 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/gc.py
--rw-r--r--   0        0        0     1154 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/githooks.py
--rw-r--r--   0        0        0     9880 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/graph.py
--rw-r--r--   0        0        0     1081 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/group.py
--rw-r--r--   0        0        0     1203 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/init.py
--rw-r--r--   0        0        0     3124 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/log.py
--rw-r--r--   0        0        0     1241 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/login.py
--rw-r--r--   0        0        0     2822 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/mergetool.py
--rw-r--r--   0        0        0    10732 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/migrate.py
--rw-r--r--   0        0        0     9141 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/move.py
--rw-r--r--   0        0        0     1015 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/options.py
--rw-r--r--   0        0        0     1362 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/project.py
--rw-r--r--   0        0        0     4748 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/remove.py
--rw-r--r--   0        0        0     3146 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/rerun.py
--rw-r--r--   0        0        0    10987 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/rollback.py
--rw-r--r--   0        0        0     1600 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/run.py
--rw-r--r--   0        0        0     3375 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/save.py
--rw-r--r--   0        0        0      766 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/schema/__init__.py
--rw-r--r--   0        0        0      211 2023-06-14 08:19:22.646666 renku-2.5.0rc3/renku/command/schema/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2040 2023-06-14 08:19:22.650666 renku-2.5.0rc3/renku/command/schema/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0      977 2023-06-14 08:19:22.790665 renku-2.5.0rc3/renku/command/schema/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     6652 2023-06-14 08:19:22.782665 renku-2.5.0rc3/renku/command/schema/__pycache__/calamus.cpython-39.pyc
--rw-r--r--   0        0        0     7584 2023-06-14 08:19:22.646666 renku-2.5.0rc3/renku/command/schema/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0     1345 2023-06-14 08:19:22.794665 renku-2.5.0rc3/renku/command/schema/__pycache__/entity.cpython-39.pyc
--rw-r--r--   0        0        0     5615 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/schema/activity.py
--rw-r--r--   0        0        0     2478 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/schema/agent.py
--rw-r--r--   0        0        0     1235 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/schema/annotation.py
--rw-r--r--   0        0        0     8986 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/schema/calamus.py
--rw-r--r--   0        0        0     3186 2023-06-14 08:18:31.775133 renku-2.5.0rc3/renku/command/schema/composite_plan.py
--rw-r--r--   0        0        0     8210 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/schema/dataset.py
--rw-r--r--   0        0        0     1445 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/schema/entity.py
--rw-r--r--   0        0        0     4016 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/schema/parameter.py
--rw-r--r--   0        0        0     3427 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/schema/plan.py
--rw-r--r--   0        0        0     3406 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/schema/project.py
--rw-r--r--   0        0        0     3065 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/schema/workflow_file.py
--rw-r--r--   0        0        0     2039 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/session.py
--rw-r--r--   0        0        0     1036 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/status.py
--rw-r--r--   0        0        0     3944 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/storage.py
--rw-r--r--   0        0        0     1919 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/template.py
--rw-r--r--   0        0        0     1254 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/update.py
--rw-r--r--   0        0        0     1726 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/util.py
--rw-r--r--   0        0        0     1088 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/version.py
--rw-r--r--   0        0        0      768 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/__init__.py
--rw-r--r--   0        0        0      217 2023-06-14 08:19:22.938664 renku-2.5.0rc3/renku/command/view_model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13290 2023-06-14 08:19:24.502650 renku-2.5.0rc3/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc
--rw-r--r--   0        0        0     1350 2023-06-14 08:19:24.534649 renku-2.5.0rc3/renku/command/view_model/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0     8157 2023-06-14 08:19:24.534649 renku-2.5.0rc3/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc
--rw-r--r--   0        0        0     1848 2023-06-14 08:19:22.938664 renku-2.5.0rc3/renku/command/view_model/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0    11145 2023-06-14 08:19:25.318642 renku-2.5.0rc3/renku/command/view_model/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0     7823 2023-06-14 08:19:24.534649 renku-2.5.0rc3/renku/command/view_model/__pycache__/plan.cpython-39.pyc
--rw-r--r--   0        0        0    14258 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/activity_graph.py
--rw-r--r--   0        0        0     1657 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/agent.py
--rw-r--r--   0        0        0     8768 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/composite_plan.py
--rw-r--r--   0        0        0     2138 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/dataset.py
--rw-r--r--   0        0        0     7850 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/graph.py
--rw-r--r--   0        0        0    12497 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/log.py
--rw-r--r--   0        0        0     9377 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/plan.py
--rw-r--r--   0        0        0     3306 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/project.py
--rw-r--r--   0        0        0     5947 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/template.py
--rw-r--r--   0        0        0    15885 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/text_canvas.py
--rw-r--r--   0        0        0     4792 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/view_model/workflow_file.py
--rw-r--r--   0        0        0     4114 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/command/workflow.py
--rw-r--r--   0        0        0      745 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/__init__.py
--rw-r--r--   0        0        0      180 2023-06-14 08:19:22.230670 renku-2.5.0rc3/renku/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4501 2023-06-14 08:19:22.462668 renku-2.5.0rc3/renku/core/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     1707 2023-06-14 08:19:22.238670 renku-2.5.0rc3/renku/core/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0    34603 2023-06-14 08:19:22.234670 renku-2.5.0rc3/renku/core/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     4854 2023-06-14 08:19:24.538649 renku-2.5.0rc3/renku/core/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0     8039 2023-06-14 08:19:22.846664 renku-2.5.0rc3/renku/core/__pycache__/login.cpython-39.pyc
--rw-r--r--   0        0        0    14579 2023-06-14 08:19:22.814665 renku-2.5.0rc3/renku/core/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0        0        0     6170 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/config.py
--rw-r--r--   0        0        0     2717 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/constant.py
--rw-r--r--   0        0        0      765 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/__init__.py
--rw-r--r--   0        0        0      208 2023-06-14 08:19:22.446668 renku-2.5.0rc3/renku/core/dataset/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2042 2023-06-14 08:19:22.914664 renku-2.5.0rc3/renku/core/dataset/__pycache__/context.cpython-39.pyc
--rw-r--r--   0        0        0    38317 2023-06-14 08:19:22.922664 renku-2.5.0rc3/renku/core/dataset/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0    15656 2023-06-14 08:19:22.914664 renku-2.5.0rc3/renku/core/dataset/__pycache__/dataset_add.cpython-39.pyc
--rw-r--r--   0        0        0     7431 2023-06-14 08:19:22.838664 renku-2.5.0rc3/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc
--rw-r--r--   0        0        0     3355 2023-06-14 08:19:22.810665 renku-2.5.0rc3/renku/core/dataset/__pycache__/pointer_file.cpython-39.pyc
--rw-r--r--   0        0        0     2737 2023-06-14 08:19:22.938664 renku-2.5.0rc3/renku/core/dataset/__pycache__/request_model.cpython-39.pyc
--rw-r--r--   0        0        0     5280 2023-06-14 08:19:22.942664 renku-2.5.0rc3/renku/core/dataset/__pycache__/tag.cpython-39.pyc
--rw-r--r--   0        0        0     2954 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/context.py
--rw-r--r--   0        0        0    50044 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/dataset.py
--rw-r--r--   0        0        0    21429 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/dataset_add.py
--rw-r--r--   0        0        0     9747 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/datasets_provenance.py
--rw-r--r--   0        0        0     4296 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/pointer_file.py
--rw-r--r--   0        0        0      760 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/__init__.py
--rw-r--r--   0        0        0      213 2023-06-14 08:19:22.446668 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    18159 2023-06-14 08:19:22.450668 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc
--rw-r--r--   0        0        0     6734 2023-06-14 08:19:22.634666 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc
--rw-r--r--   0        0        0     1646 2023-06-14 08:19:22.634666 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc
--rw-r--r--   0        0        0    19710 2023-06-14 08:19:22.806665 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc
--rw-r--r--   0        0        0     3221 2023-06-14 08:19:22.806665 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc
--rw-r--r--   0        0        0     5087 2023-06-14 08:19:22.806665 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc
--rw-r--r--   0        0        0     5963 2023-06-14 08:19:22.810665 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc
--rw-r--r--   0        0        0     5562 2023-06-14 08:19:22.446668 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0        0        0     7710 2023-06-14 08:19:22.810665 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0    10821 2023-06-14 08:19:22.830664 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc
--rw-r--r--   0        0        0     6644 2023-06-14 08:19:22.638666 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     9573 2023-06-14 08:19:22.830664 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc
--rw-r--r--   0        0        0    17180 2023-06-14 08:19:22.834664 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc
--rw-r--r--   0        0        0     2538 2023-06-14 08:19:22.806665 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc
--rw-r--r--   0        0        0     6260 2023-06-14 08:19:22.906664 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc
--rw-r--r--   0        0        0     7131 2023-06-14 08:19:22.910664 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc
--rw-r--r--   0        0        0    18001 2023-06-14 08:19:22.974663 renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc
--rw-r--r--   0        0        0    16174 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/api.py
--rw-r--r--   0        0        0     6987 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/azure.py
--rw-r--r--   0        0        0     2225 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/common.py
--rw-r--r--   0        0        0    21202 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/dataverse.py
--rw-r--r--   0        0        0     3742 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/dataverse_metadata_templates.py
--rw-r--r--   0        0        0     4829 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/doi.py
--rw-r--r--   0        0        0     5623 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/external.py
--rw-r--r--   0        0        0     5764 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/factory.py
--rw-r--r--   0        0        0    10563 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/git.py
--rw-r--r--   0        0        0    14308 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/local.py
--rw-r--r--   0        0        0     6292 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/models.py
--rw-r--r--   0        0        0    10118 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/olos.py
--rw-r--r--   0        0        0    22167 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/renku.py
--rw-r--r--   0        0        0     2553 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/repository.py
--rw-r--r--   0        0        0     6413 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/s3.py
--rw-r--r--   0        0        0     9427 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/web.py
--rw-r--r--   0        0        0    18757 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/providers/zenodo.py
--rw-r--r--   0        0        0     3973 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/request_model.py
--rw-r--r--   0        0        0     5361 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/dataset/tag.py
--rw-r--r--   0        0        0    25658 2023-06-14 08:18:31.779133 renku-2.5.0rc3/renku/core/errors.py
--rw-r--r--   0        0        0     1115 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/gc.py
--rw-r--r--   0        0        0     7394 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/git.py
--rw-r--r--   0        0        0     2151 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/githooks.py
--rw-r--r--   0        0        0    16526 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/init.py
--rw-r--r--   0        0        0      775 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/interface/__init__.py
--rw-r--r--   0        0        0      207 2023-06-14 08:19:22.798665 renku-2.5.0rc3/renku/core/interface/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4269 2023-06-14 08:19:24.502650 renku-2.5.0rc3/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     1246 2023-06-14 08:19:24.538649 renku-2.5.0rc3/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     2159 2023-06-14 08:19:22.846664 renku-2.5.0rc3/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     2057 2023-06-14 08:19:24.490650 renku-2.5.0rc3/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc
--rw-r--r--   0        0        0      959 2023-06-14 08:19:24.494650 renku-2.5.0rc3/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc
--rw-r--r--   0        0        0     4402 2023-06-14 08:19:22.798665 renku-2.5.0rc3/renku/core/interface/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0        0        0     1579 2023-06-14 08:19:24.418650 renku-2.5.0rc3/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc
--rw-r--r--   0        0        0     3741 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/interface/activity_gateway.py
--rw-r--r--   0        0        0     1418 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/interface/database_gateway.py
--rw-r--r--   0        0        0     2095 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/interface/dataset_gateway.py
--rw-r--r--   0        0        0     1996 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/interface/plan_gateway.py
--rw-r--r--   0        0        0     1212 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/interface/project_gateway.py
--rw-r--r--   0        0        0     4226 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/interface/storage.py
--rw-r--r--   0        0        0     1780 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/interface/workflow_file_parser.py
--rw-r--r--   0        0        0    10639 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/login.py
--rw-r--r--   0        0        0      764 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/__init__.py
--rw-r--r--   0        0        0      196 2023-06-14 08:19:22.586667 renku-2.5.0rc3/renku/core/migration/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1122 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0003__0_pyld2.py
--rw-r--r--   0        0        0    15324 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0003__1_jsonld.py
--rw-r--r--   0        0        0     9570 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0003__2_initial.py
--rw-r--r--   0        0        0     1122 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0004__0_pyld2.py
--rw-r--r--   0        0        0     5318 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0004__submodules.py
--rw-r--r--   0        0        0     1548 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0005__1_pyld2.py
--rw-r--r--   0        0        0    16075 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0005__2_cwl.py
--rw-r--r--   0        0        0     1015 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0006__dataset_context.py
--rw-r--r--   0        0        0     1430 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0007__source_url.py
--rw-r--r--   0        0        0     1175 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0008__dataset_metadata.py
--rw-r--r--   0        0        0    30683 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0009__new_metadata_storage.py
--rw-r--r--   0        0        0    14077 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/m_0010__metadata_fixes.py
--rw-r--r--   0        0        0    10163 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/migrate.py
--rw-r--r--   0        0        0      770 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/models/__init__.py
--rw-r--r--   0        0        0     5830 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/models/migration.py
--rw-r--r--   0        0        0     3861 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/models/refs.py
--rw-r--r--   0        0        0     5091 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/models/v10.py
--rw-r--r--   0        0        0    11828 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/models/v3.py
--rw-r--r--   0        0        0     2422 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/models/v7.py
--rw-r--r--   0        0        0     4587 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/models/v8.py
--rw-r--r--   0        0        0    74094 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/models/v9.py
--rw-r--r--   0        0        0     7945 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/utils/__init__.py
--rw-r--r--   0        0        0     6660 2023-06-14 08:19:22.586667 renku-2.5.0rc3/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8121 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/migration/utils/conversion.py
--rw-r--r--   0        0        0      824 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/plugin/__init__.py
--rw-r--r--   0        0        0      265 2023-06-14 08:19:22.450668 renku-2.5.0rc3/renku/core/plugin/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1033 2023-06-14 08:19:22.630666 renku-2.5.0rc3/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc
--rw-r--r--   0        0        0     1049 2023-06-14 08:19:22.634666 renku-2.5.0rc3/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc
--rw-r--r--   0        0        0     3246 2023-06-14 08:19:23.706657 renku-2.5.0rc3/renku/core/plugin/__pycache__/provider.cpython-39.pyc
--rw-r--r--   0        0        0     1467 2023-06-14 08:19:25.238643 renku-2.5.0rc3/renku/core/plugin/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     1170 2023-06-14 08:19:25.370642 renku-2.5.0rc3/renku/core/plugin/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     4177 2023-06-14 08:19:24.914646 renku-2.5.0rc3/renku/core/plugin/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0        0        0     2978 2023-06-14 08:19:24.510650 renku-2.5.0rc3/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc
--rw-r--r--   0        0        0     1467 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/plugin/dataset_provider.py
--rw-r--r--   0        0        0     3046 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/plugin/implementations/__init__.py
--rw-r--r--   0        0        0     2540 2023-06-14 08:19:22.634666 renku-2.5.0rc3/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1790 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/plugin/pluginmanager.py
--rw-r--r--   0        0        0     3357 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/plugin/provider.py
--rw-r--r--   0        0        0     1839 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/plugin/run.py
--rw-r--r--   0        0        0     1515 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/plugin/session.py
--rw-r--r--   0        0        0     4195 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/plugin/workflow.py
--rw-r--r--   0        0        0     3065 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/plugin/workflow_file_parser.py
--rw-r--r--   0        0        0     3355 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/project.py
--rw-r--r--   0        0        0      770 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/session/__init__.py
--rw-r--r--   0        0        0      210 2023-06-14 08:19:22.974663 renku-2.5.0rc3/renku/core/session/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    16099 2023-06-14 08:19:22.978663 renku-2.5.0rc3/renku/core/session/__pycache__/docker.cpython-39.pyc
--rw-r--r--   0        0        0    16431 2023-06-14 08:19:23.134662 renku-2.5.0rc3/renku/core/session/__pycache__/renkulab.cpython-39.pyc
--rw-r--r--   0        0        0     1449 2023-06-14 08:19:23.134662 renku-2.5.0rc3/renku/core/session/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0    22065 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/session/docker.py
--rw-r--r--   0        0        0    21512 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/session/renkulab.py
--rw-r--r--   0        0        0    13503 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/session/session.py
--rw-r--r--   0        0        0     2206 2023-06-14 08:18:31.783133 renku-2.5.0rc3/renku/core/session/utils.py
--rw-r--r--   0        0        0    19478 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/storage.py
--rw-r--r--   0        0        0      760 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/template/__init__.py
--rw-r--r--   0        0        0    22043 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/template/template.py
--rw-r--r--   0        0        0    14612 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/template/usecase.py
--rw-r--r--   0        0        0      756 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/__init__.py
--rw-r--r--   0        0        0      196 2023-06-14 08:19:22.242670 renku-2.5.0rc3/renku/core/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11124 2023-06-14 08:19:22.462668 renku-2.5.0rc3/renku/core/util/__pycache__/communication.cpython-39.pyc
--rw-r--r--   0        0        0     6320 2023-06-14 08:19:24.538649 renku-2.5.0rc3/renku/core/util/__pycache__/contexts.cpython-39.pyc
--rw-r--r--   0        0        0     1801 2023-06-14 08:19:22.582667 renku-2.5.0rc3/renku/core/util/__pycache__/datetime8601.cpython-39.pyc
--rw-r--r--   0        0        0      933 2023-06-14 08:19:22.630666 renku-2.5.0rc3/renku/core/util/__pycache__/doi.cpython-39.pyc
--rw-r--r--   0        0        0    33652 2023-06-14 08:19:22.246670 renku-2.5.0rc3/renku/core/util/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0      669 2023-06-14 08:19:23.134662 renku-2.5.0rc3/renku/core/util/__pycache__/jwt.cpython-39.pyc
--rw-r--r--   0        0        0     6008 2023-06-14 08:19:22.586667 renku-2.5.0rc3/renku/core/util/__pycache__/metadata.cpython-39.pyc
--rw-r--r--   0        0        0    11013 2023-06-14 08:19:22.418668 renku-2.5.0rc3/renku/core/util/__pycache__/os.cpython-39.pyc
--rw-r--r--   0        0        0     6893 2023-06-14 08:19:22.970663 renku-2.5.0rc3/renku/core/util/__pycache__/requests.cpython-39.pyc
--rw-r--r--   0        0        0     5971 2023-06-14 08:19:23.194661 renku-2.5.0rc3/renku/core/util/__pycache__/ssh.cpython-39.pyc
--rw-r--r--   0        0        0     1736 2023-06-14 08:19:22.942664 renku-2.5.0rc3/renku/core/util/__pycache__/tabulate.cpython-39.pyc
--rw-r--r--   0        0        0     4943 2023-06-14 08:19:22.462668 renku-2.5.0rc3/renku/core/util/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0        0        0     3737 2023-06-14 08:19:22.946663 renku-2.5.0rc3/renku/core/util/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     2663 2023-06-14 08:19:22.586667 renku-2.5.0rc3/renku/core/util/__pycache__/yaml.cpython-39.pyc
--rw-r--r--   0        0        0    10282 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/communication.py
--rw-r--r--   0        0        0     6617 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/contexts.py
--rw-r--r--   0        0        0     2313 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/datetime8601.py
--rw-r--r--   0        0        0     1376 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/doi.py
--rw-r--r--   0        0        0    40689 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/git.py
--rw-r--r--   0        0        0     1244 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/jwt.py
--rw-r--r--   0        0        0     7036 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/metadata.py
--rw-r--r--   0        0        0    12140 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/os.py
--rw-r--r--   0        0        0     7626 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/requests.py
--rw-r--r--   0        0        0     1611 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/shacl.py
--rw-r--r--   0        0        0     6871 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/ssh.py
--rw-r--r--   0        0        0     2158 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/tabulate.py
--rw-r--r--   0        0        0     6228 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/urls.py
--rw-r--r--   0        0        0     3878 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/util.py
--rw-r--r--   0        0        0     2836 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/util/yaml.py
--rw-r--r--   0        0        0      773 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/__init__.py
--rw-r--r--   0        0        0      204 2023-06-14 08:19:23.194661 renku-2.5.0rc3/renku/core/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    18165 2023-06-14 08:19:24.542649 renku-2.5.0rc3/renku/core/workflow/__pycache__/activity.cpython-39.pyc
--rw-r--r--   0        0        0    14583 2023-06-14 08:19:25.358642 renku-2.5.0rc3/renku/core/workflow/__pycache__/execute.cpython-39.pyc
--rw-r--r--   0        0        0    26495 2023-06-14 08:19:24.498650 renku-2.5.0rc3/renku/core/workflow/__pycache__/plan.cpython-39.pyc
--rw-r--r--   0        0        0    23623 2023-06-14 08:19:24.550649 renku-2.5.0rc3/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc
--rw-r--r--   0        0        0    10067 2023-06-14 08:19:24.530650 renku-2.5.0rc3/renku/core/workflow/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     1660 2023-06-14 08:19:24.550649 renku-2.5.0rc3/renku/core/workflow/__pycache__/types.cpython-39.pyc
--rw-r--r--   0        0        0     8676 2023-06-14 08:19:24.510650 renku-2.5.0rc3/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc
--rw-r--r--   0        0        0     4780 2023-06-14 08:19:25.354642 renku-2.5.0rc3/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc
--rw-r--r--   0        0        0    22713 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/activity.py
--rw-r--r--   0        0        0      773 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/converters/__init__.py
--rw-r--r--   0        0        0      215 2023-06-14 08:19:23.194661 renku-2.5.0rc3/renku/core/workflow/converters/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11079 2023-06-14 08:19:23.198661 renku-2.5.0rc3/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc
--rw-r--r--   0        0        0     4668 2023-06-14 08:19:24.414651 renku-2.5.0rc3/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc
--rw-r--r--   0        0        0    17937 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/converters/cwl.py
--rw-r--r--   0        0        0     5142 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/converters/renku.py
--rw-r--r--   0        0        0    18756 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/execute.py
--rw-r--r--   0        0        0      769 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/model/__init__.py
--rw-r--r--   0        0        0      206 2023-06-14 08:19:23.706657 renku-2.5.0rc3/renku/core/workflow/model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4825 2023-06-14 08:19:23.706657 renku-2.5.0rc3/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc
--rw-r--r--   0        0        0    26172 2023-06-14 08:19:24.422650 renku-2.5.0rc3/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc
--rw-r--r--   0        0        0     6530 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/model/concrete_execution_graph.py
--rw-r--r--   0        0        0    37866 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/model/workflow_file.py
--rw-r--r--   0        0        0      775 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/parser/__init__.py
--rw-r--r--   0        0        0      213 2023-06-14 08:19:24.414651 renku-2.5.0rc3/renku/core/workflow/parser/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8620 2023-06-14 08:19:24.418650 renku-2.5.0rc3/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc
--rw-r--r--   0        0        0    10631 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/parser/renku.py
--rw-r--r--   0        0        0    34209 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/plan.py
--rw-r--r--   0        0        0    33046 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/plan_factory.py
--rw-r--r--   0        0        0      772 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/providers/__init__.py
--rw-r--r--   0        0        0      213 2023-06-14 08:19:24.558649 renku-2.5.0rc3/renku/core/workflow/providers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4631 2023-06-14 08:19:24.558649 renku-2.5.0rc3/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc
--rw-r--r--   0        0        0     3918 2023-06-14 08:19:24.914646 renku-2.5.0rc3/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc
--rw-r--r--   0        0        0    11194 2023-06-14 08:19:24.918646 renku-2.5.0rc3/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc
--rw-r--r--   0        0        0     5999 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/providers/cwltool.py
--rw-r--r--   0        0        0     4271 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/providers/local.py
--rw-r--r--   0        0        0    13372 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/providers/toil.py
--rw-r--r--   0        0        0    13562 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/run.py
--rw-r--r--   0        0        0     1681 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/types.py
--rw-r--r--   0        0        0     2869 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/update.py
--rw-r--r--   0        0        0     8335 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/value_resolution.py
--rw-r--r--   0        0        0     5089 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/core/workflow/workflow_file.py
--rw-r--r--   0        0        0      767 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/data/__init__.py
--rw-r--r--   0        0        0      114 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/data/defaults.ini
--rw-r--r--   0        0        0     3364 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/data/gitignore.default
--rwxr-xr-x   0        0        0     4474 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/data/pre-commit.sh
--rw-r--r--   0        0        0    48383 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/data/shacl_shape.json
--rw-r--r--   0        0        0      767 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/domain_model/__init__.py
--rw-r--r--   0        0        0      210 2023-06-14 08:19:22.422668 renku-2.5.0rc3/renku/domain_model/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      388 2023-06-14 08:19:22.446668 renku-2.5.0rc3/renku/domain_model/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0    26295 2023-06-14 08:19:22.470668 renku-2.5.0rc3/renku/domain_model/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0      988 2023-06-14 08:19:22.630666 renku-2.5.0rc3/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc
--rw-r--r--   0        0        0     2204 2023-06-14 08:19:24.550649 renku-2.5.0rc3/renku/domain_model/__pycache__/datastructures.cpython-39.pyc
--rw-r--r--   0        0        0     2539 2023-06-14 08:19:22.794665 renku-2.5.0rc3/renku/domain_model/__pycache__/entity.cpython-39.pyc
--rw-r--r--   0        0        0      575 2023-06-14 08:19:22.462668 renku-2.5.0rc3/renku/domain_model/__pycache__/enums.cpython-39.pyc
--rw-r--r--   0        0        0     6097 2023-06-14 08:19:24.410651 renku-2.5.0rc3/renku/domain_model/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0    12164 2023-06-14 08:19:22.426668 renku-2.5.0rc3/renku/domain_model/__pycache__/project_context.cpython-39.pyc
--rw-r--r--   0        0        0     7426 2023-06-14 08:19:23.130662 renku-2.5.0rc3/renku/domain_model/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     1092 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/domain_model/constant.py
--rw-r--r--   0        0        0    29611 2023-06-14 08:18:31.787134 renku-2.5.0rc3/renku/domain_model/dataset.py
--rw-r--r--   0        0        0     1267 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/dataset_provider.py
--rw-r--r--   0        0        0     2754 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/datastructures.py
--rw-r--r--   0        0        0     2499 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/entity.py
--rw-r--r--   0        0        0      971 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/enums.py
--rw-r--r--   0        0        0     5059 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/git.py
--rw-r--r--   0        0        0     8329 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/project.py
--rw-r--r--   0        0        0    11817 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/project_context.py
--rw-r--r--   0        0        0      829 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/provenance/__init__.py
--rw-r--r--   0        0        0      283 2023-06-14 08:19:22.790665 renku-2.5.0rc3/renku/domain_model/provenance/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11882 2023-06-14 08:19:24.506650 renku-2.5.0rc3/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc
--rw-r--r--   0        0        0     4946 2023-06-14 08:19:22.790665 renku-2.5.0rc3/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc
--rw-r--r--   0        0        0     1092 2023-06-14 08:19:22.790665 renku-2.5.0rc3/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     1363 2023-06-14 08:19:24.506650 renku-2.5.0rc3/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc
--rw-r--r--   0        0        0    13200 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/provenance/activity.py
--rw-r--r--   0        0        0     5155 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/provenance/agent.py
--rw-r--r--   0        0        0     1268 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/provenance/annotation.py
--rw-r--r--   0        0        0     1530 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/provenance/parameter.py
--rw-r--r--   0        0        0     6871 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/session.py
--rw-r--r--   0        0        0     1471 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/sort.py
--rw-r--r--   0        0        0    27042 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/template.py
--rw-r--r--   0        0        0      782 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/workflow/__init__.py
--rw-r--r--   0        0        0      234 2023-06-14 08:19:23.706657 renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13527 2023-06-14 08:19:24.118653 renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc
--rw-r--r--   0        0        0    15243 2023-06-14 08:19:24.122653 renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc
--rw-r--r--   0        0        0    15096 2023-06-14 08:19:24.126653 renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc
--rw-r--r--   0        0        0     1483 2023-06-14 08:19:23.706657 renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc
--rw-r--r--   0        0        0     4523 2023-06-14 08:19:24.506650 renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc
--rw-r--r--   0        0        0    15917 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/workflow/composite_plan.py
--rw-r--r--   0        0        0     1531 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/workflow/converters/__init__.py
--rw-r--r--   0        0        0     1391 2023-06-14 08:19:24.414651 renku-2.5.0rc3/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    18124 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/workflow/parameter.py
--rw-r--r--   0        0        0    16602 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/workflow/plan.py
--rw-r--r--   0        0        0     1639 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/workflow/provider.py
--rw-r--r--   0        0        0     4660 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/domain_model/workflow/workflow_file.py
--rw-r--r--   0        0        0      780 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/__init__.py
--rw-r--r--   0        0        0      212 2023-06-14 08:19:22.246670 renku-2.5.0rc3/renku/infrastructure/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    34957 2023-06-14 08:19:24.234652 renku-2.5.0rc3/renku/infrastructure/__pycache__/database.cpython-39.pyc
--rw-r--r--   0        0        0     5073 2023-06-14 08:19:22.442668 renku-2.5.0rc3/renku/infrastructure/__pycache__/immutable.cpython-39.pyc
--rw-r--r--   0        0        0     2259 2023-06-14 08:19:22.590667 renku-2.5.0rc3/renku/infrastructure/__pycache__/persistent.cpython-39.pyc
--rw-r--r--   0        0        0    67803 2023-06-14 08:19:22.266669 renku-2.5.0rc3/renku/infrastructure/__pycache__/repository.cpython-39.pyc
--rw-r--r--   0        0        0    41333 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/database.py
--rw-r--r--   0        0        0      786 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/gateway/__init__.py
--rw-r--r--   0        0        0      226 2023-06-14 08:19:22.942664 renku-2.5.0rc3/renku/infrastructure/gateway/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3238 2023-06-14 08:19:22.942664 renku-2.5.0rc3/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-39.pyc
--rw-r--r--   0        0        0    12730 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/gateway/activity_gateway.py
--rw-r--r--   0        0        0     5845 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/gateway/database_gateway.py
--rw-r--r--   0        0        0     3743 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/gateway/dataset_gateway.py
--rw-r--r--   0        0        0     3529 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/gateway/plan_gateway.py
--rw-r--r--   0        0        0     1711 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/gateway/project_gateway.py
--rw-r--r--   0        0        0    18006 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/git_merger.py
--rw-r--r--   0        0        0     4969 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/immutable.py
--rw-r--r--   0        0        0     2394 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/persistent.py
--rw-r--r--   0        0        0    72047 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/repository.py
--rw-r--r--   0        0        0      784 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/storage/__init__.py
--rw-r--r--   0        0        0      224 2023-06-14 08:19:22.802665 renku-2.5.0rc3/renku/infrastructure/storage/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1523 2023-06-14 08:19:22.802665 renku-2.5.0rc3/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc
--rw-r--r--   0        0        0     1989 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/storage/factory.py
--rw-r--r--   0        0        0     8859 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/infrastructure/storage/rclone.py
--rw-r--r--   0        0        0      913 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      553 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      637 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      523 2023-06-14 08:19:26.506632 renku-2.5.0rc3/renku/templates/.github/dependabot.yml
--rw-r--r--   0        0        0      396 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/.github/workflows/github-project.yml
--rw-r--r--   0        0        0     3940 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/.gitignore
--rw-r--r--   0        0        0       27 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       37 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      984 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2087 2023-06-14 08:19:26.506632 renku-2.5.0rc3/renku/templates/R-minimal/Dockerfile
--rw-r--r--   0        0        0     1603 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/README.md
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/environment.yml
--rw-r--r--   0        0        0      360 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/install.R
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0      205 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal/{{ __sanitized_project_name__ }}.Rproj
--rw-r--r--   0        0        0    14286 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/R-minimal.png
--rw-r--r--   0        0        0     4846 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/README.md
--rw-r--r--   0        0        0       27 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/bioc-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-06-14 08:19:26.498632 renku-2.5.0rc3/renku/templates/bioc-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       37 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2077 2023-06-14 08:19:26.506632 renku-2.5.0rc3/renku/templates/bioc-minimal/Dockerfile
--rw-r--r--   0        0        0     1603 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/README.md
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/install.R
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0      205 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioc-minimal/{{ __sanitized_project_name__ }}.Rproj
--rw-r--r--   0        0        0    44589 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/bioconductor.png
--rw-r--r--   0        0        0       27 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/.dockerignore
--rw-r--r--   0        0        0     6018 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       50 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2469 2023-06-14 08:19:26.506632 renku-2.5.0rc3/renku/templates/julia-minimal/Dockerfile
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/Manifest.toml
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/Project.toml
--rw-r--r--   0        0        0     1842 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/README.md
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julia-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0    13782 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/julialang.png
--rw-r--r--   0        0        0     1174 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/manifest.yaml
--rw-r--r--   0        0        0       17 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/minimal/.dockerignore
--rw-r--r--   0        0        0       77 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       33 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/minimal/.renkulfsignore
--rw-r--r--   0        0        0     2414 2023-06-14 08:19:26.506632 renku-2.5.0rc3/renku/templates/minimal/Dockerfile
--rw-r--r--   0        0        0     1439 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0       27 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/.dockerignore
--rw-r--r--   0        0        0     5401 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/.gitignore
--rw-r--r--   0        0        0      450 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/.gitlab-ci.yml
--rw-r--r--   0        0        0       33 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/.renku/renku.ini
--rw-r--r--   0        0        0      976 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/.renkulfsignore
--rw-r--r--   0        0        0     2159 2023-06-14 08:19:26.506632 renku-2.5.0rc3/renku/templates/python-minimal/Dockerfile
--rw-r--r--   0        0        0     1597 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/README.md
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/data/.gitkeep
--rw-r--r--   0        0        0      112 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/environment.yml
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/notebooks/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/requirements.txt
--rw-r--r--   0        0        0     1439 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal/workflows/my-workflow.yaml
--rw-r--r--   0        0        0    25599 2023-06-14 08:19:26.502632 renku-2.5.0rc3/renku/templates/python-minimal.png
--rw-r--r--   0        0        0      763 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/__init__.py
--rw-r--r--   0        0        0      184 2023-06-14 08:19:22.118671 renku-2.5.0rc3/renku/ui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1268 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/__init__.py
--rw-r--r--   0        0        0      763 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/graph/__init__.py
--rw-r--r--   0        0        0     2519 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/graph/rdf.py
--rw-r--r--   0        0        0      764 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/models/__init__.py
--rw-r--r--   0        0        0    16448 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/models/activity.py
--rw-r--r--   0        0        0     4648 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/models/dataset.py
--rw-r--r--   0        0        0    10361 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/models/parameter.py
--rw-r--r--   0        0        0     9227 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/models/plan.py
--rw-r--r--   0        0        0     3643 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/models/project.py
--rw-r--r--   0        0        0     2519 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/api/util.py
--rw-r--r--   0        0        0     9319 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/cli/__init__.py
--rw-r--r--   0        0        0      922 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/cli/__main__.py
--rw-r--r--   0        0        0     8150 2023-06-14 08:19:22.118671 renku-2.5.0rc3/renku/ui/cli/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2117 2023-06-14 08:19:22.426668 renku-2.5.0rc3/renku/ui/cli/__pycache__/clone.cpython-39.pyc
--rw-r--r--   0        0        0     7029 2023-06-14 08:19:22.430668 renku-2.5.0rc3/renku/ui/cli/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0    36275 2023-06-14 08:19:22.434668 renku-2.5.0rc3/renku/ui/cli/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0     1787 2023-06-14 08:19:25.298643 renku-2.5.0rc3/renku/ui/cli/__pycache__/doctor.cpython-39.pyc
--rw-r--r--   0        0        0      964 2023-06-14 08:19:25.298643 renku-2.5.0rc3/renku/ui/cli/__pycache__/env.cpython-39.pyc
--rw-r--r--   0        0        0     7957 2023-06-14 08:19:25.298643 renku-2.5.0rc3/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc
--rw-r--r--   0        0        0      645 2023-06-14 08:19:25.310643 renku-2.5.0rc3/renku/ui/cli/__pycache__/gc.cpython-39.pyc
--rw-r--r--   0        0        0     2168 2023-06-14 08:19:25.310643 renku-2.5.0rc3/renku/ui/cli/__pycache__/githooks.cpython-39.pyc
--rw-r--r--   0        0        0     4041 2023-06-14 08:19:25.310643 renku-2.5.0rc3/renku/ui/cli/__pycache__/graph.cpython-39.pyc
--rw-r--r--   0        0        0     9637 2023-06-14 08:19:25.310643 renku-2.5.0rc3/renku/ui/cli/__pycache__/init.cpython-39.pyc
--rw-r--r--   0        0        0     7264 2023-06-14 08:19:25.314643 renku-2.5.0rc3/renku/ui/cli/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0     4296 2023-06-14 08:19:25.322642 renku-2.5.0rc3/renku/ui/cli/__pycache__/login.cpython-39.pyc
--rw-r--r--   0        0        0     2066 2023-06-14 08:19:25.346642 renku-2.5.0rc3/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc
--rw-r--r--   0        0        0     4585 2023-06-14 08:19:25.350642 renku-2.5.0rc3/renku/ui/cli/__pycache__/migrate.cpython-39.pyc
--rw-r--r--   0        0        0     2306 2023-06-14 08:19:25.350642 renku-2.5.0rc3/renku/ui/cli/__pycache__/move.cpython-39.pyc
--rw-r--r--   0        0        0     4028 2023-06-14 08:19:25.350642 renku-2.5.0rc3/renku/ui/cli/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0     1283 2023-06-14 08:19:25.350642 renku-2.5.0rc3/renku/ui/cli/__pycache__/remove.cpython-39.pyc
--rw-r--r--   0        0        0     3485 2023-06-14 08:19:25.350642 renku-2.5.0rc3/renku/ui/cli/__pycache__/rerun.cpython-39.pyc
--rw-r--r--   0        0        0     2761 2023-06-14 08:19:25.354642 renku-2.5.0rc3/renku/ui/cli/__pycache__/rollback.cpython-39.pyc
--rw-r--r--   0        0        0    23646 2023-06-14 08:19:25.354642 renku-2.5.0rc3/renku/ui/cli/__pycache__/run.cpython-39.pyc
--rw-r--r--   0        0        0     2890 2023-06-14 08:19:25.366642 renku-2.5.0rc3/renku/ui/cli/__pycache__/save.cpython-39.pyc
--rw-r--r--   0        0        0    10362 2023-06-14 08:19:25.366642 renku-2.5.0rc3/renku/ui/cli/__pycache__/service.cpython-39.pyc
--rw-r--r--   0        0        0    13046 2023-06-14 08:19:25.370642 renku-2.5.0rc3/renku/ui/cli/__pycache__/session.cpython-39.pyc
--rw-r--r--   0        0        0     3715 2023-06-14 08:19:25.374642 renku-2.5.0rc3/renku/ui/cli/__pycache__/status.cpython-39.pyc
--rw-r--r--   0        0        0     5061 2023-06-14 08:19:25.378642 renku-2.5.0rc3/renku/ui/cli/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0        0        0    10944 2023-06-14 08:19:25.378642 renku-2.5.0rc3/renku/ui/cli/__pycache__/template.cpython-39.pyc
--rw-r--r--   0        0        0     5790 2023-06-14 08:19:25.378642 renku-2.5.0rc3/renku/ui/cli/__pycache__/update.cpython-39.pyc
--rw-r--r--   0        0        0    41570 2023-06-14 08:19:25.382642 renku-2.5.0rc3/renku/ui/cli/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0        0        0     2594 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/cli/clone.py
--rw-r--r--   0        0        0     7953 2023-06-14 08:18:31.791133 renku-2.5.0rc3/renku/ui/cli/config.py
--rw-r--r--   0        0        0    42787 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/dataset.py
--rw-r--r--   0        0        0     2333 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/doctor.py
--rw-r--r--   0        0        0     1587 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/env.py
--rw-r--r--   0        0        0     7931 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/exception_handler.py
--rw-r--r--   0        0        0     1139 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/gc.py
--rw-r--r--   0        0        0     2538 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/githooks.py
--rw-r--r--   0        0        0     4950 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/graph.py
--rw-r--r--   0        0        0    11113 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/init.py
--rw-r--r--   0        0        0     8581 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/log.py
--rw-r--r--   0        0        0     4845 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/login.py
--rw-r--r--   0        0        0     2499 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/mergetool.py
--rw-r--r--   0        0        0     5894 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/migrate.py
--rw-r--r--   0        0        0     2881 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/move.py
--rw-r--r--   0        0        0     5768 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/project.py
--rw-r--r--   0        0        0     1754 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/remove.py
--rw-r--r--   0        0        0     4227 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/rerun.py
--rw-r--r--   0        0        0     3249 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/rollback.py
--rw-r--r--   0        0        0    26417 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/run.py
--rw-r--r--   0        0        0     3510 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/save.py
--rw-r--r--   0        0        0    11927 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/service.py
--rw-r--r--   0        0        0    14738 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/session.py
--rw-r--r--   0        0        0     5489 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/status.py
--rw-r--r--   0        0        0     5604 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/storage.py
--rw-r--r--   0        0        0    13434 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/template.py
--rw-r--r--   0        0        0     6723 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/update.py
--rw-r--r--   0        0        0      760 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/utils/__init__.py
--rw-r--r--   0        0        0      203 2023-06-14 08:19:22.426668 renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5720 2023-06-14 08:19:25.322642 renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc
--rw-r--r--   0        0        0     5071 2023-06-14 08:19:22.430668 renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc
--rw-r--r--   0        0        0      301 2023-06-14 08:19:22.426668 renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/color.cpython-39.pyc
--rw-r--r--   0        0        0      998 2023-06-14 08:19:25.350642 renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc
--rw-r--r--   0        0        0     7369 2023-06-14 08:19:25.322642 renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc
--rw-r--r--   0        0        0     5409 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/utils/callback.py
--rw-r--r--   0        0        0     5473 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/utils/click.py
--rw-r--r--   0        0        0      842 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/utils/color.py
--rw-r--r--   0        0        0    14521 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/utils/curses.py
--rw-r--r--   0        0        0     1375 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/utils/plugins.py
--rw-r--r--   0        0        0     9917 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/utils/terminal.py
--rw-r--r--   0        0        0    47787 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/cli/workflow.py
--rw-r--r--   0        0        0      843 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/.env-example
--rw-r--r--   0        0        0      756 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/__init__.py
--rw-r--r--   0        0        0      189 2023-06-14 08:19:25.298643 renku-2.5.0rc3/renku/ui/service/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2012 2023-06-14 08:19:25.302643 renku-2.5.0rc3/renku/ui/service/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     1535 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/__init__.py
--rw-r--r--   0        0        0     2917 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/base.py
--rw-r--r--   0        0        0     1168 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/config.py
--rw-r--r--   0        0        0     3315 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/files.py
--rw-r--r--   0        0        0     2333 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/jobs.py
--rw-r--r--   0        0        0      769 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/models/__init__.py
--rw-r--r--   0        0        0     4356 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/models/file.py
--rw-r--r--   0        0        0     2298 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/models/job.py
--rw-r--r--   0        0        0     4043 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/models/project.py
--rw-r--r--   0        0        0     1127 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/models/user.py
--rw-r--r--   0        0        0     2558 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/projects.py
--rw-r--r--   0        0        0      774 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/serializers/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/serializers/file.py
--rw-r--r--   0        0        0     1711 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/serializers/job.py
--rw-r--r--   0        0        0     1812 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/serializers/project.py
--rw-r--r--   0        0        0     1227 2023-06-14 08:18:31.795133 renku-2.5.0rc3/renku/ui/service/cache/serializers/user.py
--rw-r--r--   0        0        0     1657 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/cache/users.py
--rw-r--r--   0        0        0     2931 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/config.py
--rw-r--r--   0        0        0      773 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/__init__.py
--rw-r--r--   0        0        0      777 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/api/__init__.py
--rw-r--r--   0        0        0     1085 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/api/abstract.py
--rw-r--r--   0        0        0    15665 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/api/mixins.py
--rw-r--r--   0        0        0     2647 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/cache_files_delete_chunks.py
--rw-r--r--   0        0        0     7478 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/cache_files_upload.py
--rw-r--r--   0        0        0     2239 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/cache_list_projects.py
--rw-r--r--   0        0        0     1927 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/cache_list_uploaded.py
--rw-r--r--   0        0        0     4823 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/cache_migrate_project.py
--rw-r--r--   0        0        0     4905 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/cache_migrations_check.py
--rw-r--r--   0        0        0     2350 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/cache_project_clone.py
--rw-r--r--   0        0        0     2649 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/config_set.py
--rw-r--r--   0        0        0     2333 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/config_show.py
--rw-r--r--   0        0        0     5682 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/datasets_add_file.py
--rw-r--r--   0        0        0     3916 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/datasets_create.py
--rw-r--r--   0        0        0     5359 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/datasets_edit.py
--rw-r--r--   0        0        0     2132 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/datasets_files_list.py
--rw-r--r--   0        0        0     3333 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/datasets_import.py
--rw-r--r--   0        0        0     2065 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/datasets_list.py
--rw-r--r--   0        0        0     2637 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/datasets_remove.py
--rw-r--r--   0        0        0     3290 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/datasets_unlink.py
--rw-r--r--   0        0        0     5370 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/graph_export.py
--rw-r--r--   0        0        0     3936 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/project_edit.py
--rw-r--r--   0        0        0     3180 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/project_lock_status.py
--rw-r--r--   0        0        0     2096 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/project_show.py
--rw-r--r--   0        0        0     8049 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/templates_create_project.py
--rw-r--r--   0        0        0     3103 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/templates_read_manifest.py
--rw-r--r--   0        0        0      773 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/utils/__init__.py
--rw-r--r--   0        0        0     1083 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/utils/datasets.py
--rw-r--r--   0        0        0     3233 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/utils/project_clone.py
--rw-r--r--   0        0        0     2664 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/utils/remote_project.py
--rw-r--r--   0        0        0     1641 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/version.py
--rw-r--r--   0        0        0     2441 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/workflow_plans_export.py
--rw-r--r--   0        0        0     2257 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/workflow_plans_list.py
--rw-r--r--   0        0        0     2146 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/controllers/workflow_plans_show.py
--rw-r--r--   0        0        0     6150 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/entrypoint.py
--rw-r--r--   0        0        0    32144 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/errors.py
--rw-r--r--   0        0        0      774 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/gateways/__init__.py
--rw-r--r--   0        0        0     4083 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/gateways/gitlab_api_provider.py
--rw-r--r--   0        0        0      793 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/interfaces/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/interfaces/git_api_provider.py
--rw-r--r--   0        0        0      766 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/jobs/__init__.py
--rw-r--r--   0        0        0     3035 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/jobs/cleanup.py
--rw-r--r--   0        0        0      756 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/jobs/constants.py
--rw-r--r--   0        0        0     1186 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/jobs/contexts.py
--rw-r--r--   0        0        0     5244 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/jobs/datasets.py
--rw-r--r--   0        0        0     1829 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/jobs/delayed_ctrl.py
--rw-r--r--   0        0        0     2665 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/jobs/queues.py
--rw-r--r--   0        0        0     1269 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/logger.py
--rw-r--r--   0        0        0      644 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/logging.yaml
--rw-r--r--   0        0        0     2742 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/scheduler.py
--rw-r--r--   0        0        0      768 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/__init__.py
--rw-r--r--   0        0        0    14561 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/cache.py
--rw-r--r--   0        0        0     4843 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/common.py
--rw-r--r--   0        0        0     2228 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/config.py
--rw-r--r--   0        0        0     8503 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/datasets.py
--rw-r--r--   0        0        0     2195 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/graph.py
--rw-r--r--   0        0        0     5362 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/headers.py
--rw-r--r--   0        0        0     1961 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/jobs.py
--rw-r--r--   0        0        0     4510 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/project.py
--rw-r--r--   0        0        0      911 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/rpc.py
--rw-r--r--   0        0        0     5815 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/templates.py
--rw-r--r--   0        0        0      773 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/v1/__init__.py
--rw-r--r--   0        0        0     4212 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/v1/cache.py
--rw-r--r--   0        0        0     1880 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/v1/templates.py
--rw-r--r--   0        0        0     1170 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/version.py
--rw-r--r--   0        0        0     6907 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/serializers/workflows.py
--rw-r--r--   0        0        0     2186 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/utils/__init__.py
--rw-r--r--   0        0        0     2220 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/utils/callback.py
--rw-r--r--   0        0        0     1323 2023-06-14 08:18:31.799134 renku-2.5.0rc3/renku/ui/service/utils/json_encoder.py
--rw-r--r--   0        0        0     1260 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/utils/squash.py
--rw-r--r--   0        0        0     1427 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/utils/timeout.py
--rw-r--r--   0        0        0     1761 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/__init__.py
--rw-r--r--   0        0        0     2438 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/api_versions.py
--rw-r--r--   0        0        0     4767 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/apispec.py
--rw-r--r--   0        0        0     7427 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/cache.py
--rw-r--r--   0        0        0     2957 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/config.py
--rw-r--r--   0        0        0     8187 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/datasets.py
--rw-r--r--   0        0        0     2961 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/decorators.py
--rw-r--r--   0        0        0    15114 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/error_handlers.py
--rw-r--r--   0        0        0     2084 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/graph.py
--rw-r--r--   0        0        0     3267 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/jobs.py
--rw-r--r--   0        0        0     3805 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/project.py
--rw-r--r--   0        0        0     3592 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/templates.py
--rw-r--r--   0        0        0      767 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/v1/__init__.py
--rw-r--r--   0        0        0     4775 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/v1/cache.py
--rw-r--r--   0        0        0     2634 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/v1/templates.py
--rw-r--r--   0        0        0     1702 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/version.py
--rw-r--r--   0        0        0     3873 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/views/workflow_plans.py
--rw-r--r--   0        0        0     2890 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/ui/service/worker.py
--rw-r--r--   0        0        0     1614 2023-06-14 08:18:31.803134 renku-2.5.0rc3/renku/version.py
--rw-r--r--   0        0        0    17131 1970-01-01 00:00:00.000000 renku-2.5.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-06-22 14:43:37.012647 renku-2.6.0rc1/AUTHORS.rst
+-rw-r--r--   0        0        0   182553 2023-06-22 14:43:37.012647 renku-2.6.0rc1/CHANGES.rst
+-rw-r--r--   0        0        0    11358 2023-06-22 14:43:37.012647 renku-2.6.0rc1/LICENSE
+-rw-r--r--   0        0        0    12889 2023-06-22 14:43:37.016647 renku-2.6.0rc1/README.rst
+-rw-r--r--   0        0        0    10490 2023-06-22 14:44:47.313028 renku-2.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4391 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/__init__.py
+-rw-r--r--   0        0        0      209 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/command/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      437 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/command/__pycache__/options.cpython-39.pyc
+-rw-r--r--   0        0        0     1057 2023-06-22 14:44:45.241017 renku-2.6.0rc1/renku/command/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     1343 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/command/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0      593 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/command/__pycache__/version.cpython-39.pyc
+-rw-r--r--   0        0        0     2096 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/__init__.py
+-rw-r--r--   0        0        0     4808 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/activities.py
+-rw-r--r--   0        0        0     8408 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/datasets.py
+-rw-r--r--   0        0        0     2797 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/githooks.py
+-rw-r--r--   0        0        0     1548 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/migration.py
+-rw-r--r--   0        0        0     2448 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/project.py
+-rw-r--r--   0        0        0     1572 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/storage.py
+-rw-r--r--   0        0        0     4124 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/validate_shacl.py
+-rw-r--r--   0        0        0     5025 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/checks/workflow.py
+-rw-r--r--   0        0        0     3872 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/clone.py
+-rw-r--r--   0        0        0      828 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-22 14:44:42.069000 renku-2.6.0rc1/renku/command/command_builder/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    15431 2023-06-22 14:44:42.073000 renku-2.6.0rc1/renku/command/command_builder/__pycache__/command.cpython-39.pyc
+-rw-r--r--   0        0        0    16678 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/command.py
+-rw-r--r--   0        0        0     1951 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/communication.py
+-rw-r--r--   0        0        0     5325 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/database.py
+-rw-r--r--   0        0        0     1701 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/lock.py
+-rw-r--r--   0        0        0     1481 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/migration.py
+-rw-r--r--   0        0        0     7694 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/command_builder/repo.py
+-rw-r--r--   0        0        0     4803 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/config.py
+-rw-r--r--   0        0        0     5640 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/dataset.py
+-rw-r--r--   0        0        0     2835 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/doctor.py
+-rw-r--r--   0        0        0      775 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/format/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-22 14:44:41.616998 renku-2.6.0rc1/renku/command/format/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5765 2023-06-22 14:44:41.620998 renku-2.6.0rc1/renku/command/format/__pycache__/dataset_files.cpython-39.pyc
+-rw-r--r--   0        0        0     1508 2023-06-22 14:44:41.620998 renku-2.6.0rc1/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc
+-rw-r--r--   0        0        0     2884 2023-06-22 14:44:41.620998 renku-2.6.0rc1/renku/command/format/__pycache__/datasets.cpython-39.pyc
+-rw-r--r--   0        0        0      817 2023-06-22 14:44:44.129011 renku-2.6.0rc1/renku/command/format/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0     1754 2023-06-22 14:44:45.265017 renku-2.6.0rc1/renku/command/format/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     1929 2023-06-22 14:44:44.129011 renku-2.6.0rc1/renku/command/format/__pycache__/tabulate.cpython-39.pyc
+-rw-r--r--   0        0        0     2416 2023-06-22 14:44:44.129011 renku-2.6.0rc1/renku/command/format/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0        0        0     2643 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/format/activity.py
+-rw-r--r--   0        0        0     6230 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/format/dataset_files.py
+-rw-r--r--   0        0        0     2098 2023-06-22 14:43:37.076648 renku-2.6.0rc1/renku/command/format/dataset_tags.py
+-rw-r--r--   0        0        0     3236 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/datasets.py
+-rw-r--r--   0        0        0     1212 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/json.py
+-rw-r--r--   0        0        0     2402 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/session.py
+-rw-r--r--   0        0        0     2769 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/tabulate.py
+-rw-r--r--   0        0        0     2728 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/format/workflow.py
+-rw-r--r--   0        0        0     1012 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/gc.py
+-rw-r--r--   0        0        0     1154 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/githooks.py
+-rw-r--r--   0        0        0     9880 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/graph.py
+-rw-r--r--   0        0        0     1081 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/group.py
+-rw-r--r--   0        0        0     1203 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/init.py
+-rw-r--r--   0        0        0     3124 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/log.py
+-rw-r--r--   0        0        0     1241 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/login.py
+-rw-r--r--   0        0        0     2822 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/mergetool.py
+-rw-r--r--   0        0        0    10732 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/migrate.py
+-rw-r--r--   0        0        0     9141 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/move.py
+-rw-r--r--   0        0        0     1015 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/options.py
+-rw-r--r--   0        0        0     1362 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/project.py
+-rw-r--r--   0        0        0     4748 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/remove.py
+-rw-r--r--   0        0        0     3146 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/rerun.py
+-rw-r--r--   0        0        0    10987 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/rollback.py
+-rw-r--r--   0        0        0     1600 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/run.py
+-rw-r--r--   0        0        0     3375 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/save.py
+-rw-r--r--   0        0        0      766 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-22 14:44:41.824999 renku-2.6.0rc1/renku/command/schema/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2040 2023-06-22 14:44:41.828999 renku-2.6.0rc1/renku/command/schema/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0      977 2023-06-22 14:44:42.009000 renku-2.6.0rc1/renku/command/schema/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     6652 2023-06-22 14:44:41.997000 renku-2.6.0rc1/renku/command/schema/__pycache__/calamus.cpython-39.pyc
+-rw-r--r--   0        0        0     7584 2023-06-22 14:44:41.828999 renku-2.6.0rc1/renku/command/schema/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     1345 2023-06-22 14:44:42.009000 renku-2.6.0rc1/renku/command/schema/__pycache__/entity.cpython-39.pyc
+-rw-r--r--   0        0        0     5615 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/activity.py
+-rw-r--r--   0        0        0     2478 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/agent.py
+-rw-r--r--   0        0        0     1235 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/annotation.py
+-rw-r--r--   0        0        0     8986 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/calamus.py
+-rw-r--r--   0        0        0     3186 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/composite_plan.py
+-rw-r--r--   0        0        0     8210 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/dataset.py
+-rw-r--r--   0        0        0     1445 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/entity.py
+-rw-r--r--   0        0        0     4016 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/parameter.py
+-rw-r--r--   0        0        0     3427 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/plan.py
+-rw-r--r--   0        0        0     3406 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/project.py
+-rw-r--r--   0        0        0     3065 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/schema/workflow_file.py
+-rw-r--r--   0        0        0     2039 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/session.py
+-rw-r--r--   0        0        0     1036 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/status.py
+-rw-r--r--   0        0        0     3944 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/storage.py
+-rw-r--r--   0        0        0     1919 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/template.py
+-rw-r--r--   0        0        0     1254 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/update.py
+-rw-r--r--   0        0        0     1726 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/util.py
+-rw-r--r--   0        0        0     1088 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/version.py
+-rw-r--r--   0        0        0      768 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-22 14:44:42.197001 renku-2.6.0rc1/renku/command/view_model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13290 2023-06-22 14:44:44.133011 renku-2.6.0rc1/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc
+-rw-r--r--   0        0        0     1350 2023-06-22 14:44:44.177011 renku-2.6.0rc1/renku/command/view_model/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0     8157 2023-06-22 14:44:44.177011 renku-2.6.0rc1/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc
+-rw-r--r--   0        0        0     1848 2023-06-22 14:44:42.201001 renku-2.6.0rc1/renku/command/view_model/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0    11145 2023-06-22 14:44:45.193017 renku-2.6.0rc1/renku/command/view_model/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0     7823 2023-06-22 14:44:44.177011 renku-2.6.0rc1/renku/command/view_model/__pycache__/plan.cpython-39.pyc
+-rw-r--r--   0        0        0    14258 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/activity_graph.py
+-rw-r--r--   0        0        0     1657 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/agent.py
+-rw-r--r--   0        0        0     8768 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/composite_plan.py
+-rw-r--r--   0        0        0     2138 2023-06-22 14:43:37.080648 renku-2.6.0rc1/renku/command/view_model/dataset.py
+-rw-r--r--   0        0        0     7850 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/graph.py
+-rw-r--r--   0        0        0    12497 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/log.py
+-rw-r--r--   0        0        0     9377 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/plan.py
+-rw-r--r--   0        0        0     3306 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/project.py
+-rw-r--r--   0        0        0     5947 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/template.py
+-rw-r--r--   0        0        0    15885 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/text_canvas.py
+-rw-r--r--   0        0        0     4792 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/view_model/workflow_file.py
+-rw-r--r--   0        0        0     4114 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/command/workflow.py
+-rw-r--r--   0        0        0      745 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-22 14:44:41.360996 renku-2.6.0rc1/renku/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4501 2023-06-22 14:44:41.648998 renku-2.6.0rc1/renku/core/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     1707 2023-06-22 14:44:41.368996 renku-2.6.0rc1/renku/core/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0    34603 2023-06-22 14:44:41.364997 renku-2.6.0rc1/renku/core/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     4854 2023-06-22 14:44:44.181011 renku-2.6.0rc1/renku/core/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0     8039 2023-06-22 14:44:42.081000 renku-2.6.0rc1/renku/core/__pycache__/login.cpython-39.pyc
+-rw-r--r--   0        0        0    14579 2023-06-22 14:44:42.037000 renku-2.6.0rc1/renku/core/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0        0        0     6170 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/config.py
+-rw-r--r--   0        0        0     2717 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/constant.py
+-rw-r--r--   0        0        0      765 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/__init__.py
+-rw-r--r--   0        0        0      208 2023-06-22 14:44:41.624998 renku-2.6.0rc1/renku/core/dataset/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2042 2023-06-22 14:44:42.169001 renku-2.6.0rc1/renku/core/dataset/__pycache__/context.cpython-39.pyc
+-rw-r--r--   0        0        0    38317 2023-06-22 14:44:42.181001 renku-2.6.0rc1/renku/core/dataset/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0    15656 2023-06-22 14:44:42.169001 renku-2.6.0rc1/renku/core/dataset/__pycache__/dataset_add.cpython-39.pyc
+-rw-r--r--   0        0        0     7431 2023-06-22 14:44:42.069000 renku-2.6.0rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc
+-rw-r--r--   0        0        0     3355 2023-06-22 14:44:42.033000 renku-2.6.0rc1/renku/core/dataset/__pycache__/pointer_file.cpython-39.pyc
+-rw-r--r--   0        0        0     2737 2023-06-22 14:44:42.201001 renku-2.6.0rc1/renku/core/dataset/__pycache__/request_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5280 2023-06-22 14:44:42.205001 renku-2.6.0rc1/renku/core/dataset/__pycache__/tag.cpython-39.pyc
+-rw-r--r--   0        0        0     2954 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/context.py
+-rw-r--r--   0        0        0    50044 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/dataset.py
+-rw-r--r--   0        0        0    21429 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/dataset_add.py
+-rw-r--r--   0        0        0     9747 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/datasets_provenance.py
+-rw-r--r--   0        0        0     4296 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/pointer_file.py
+-rw-r--r--   0        0        0      760 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-22 14:44:41.624998 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    18159 2023-06-22 14:44:41.628998 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc
+-rw-r--r--   0        0        0     6734 2023-06-22 14:44:41.808999 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc
+-rw-r--r--   0        0        0     1646 2023-06-22 14:44:41.812999 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0        0        0    19710 2023-06-22 14:44:42.025000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc
+-rw-r--r--   0        0        0     3221 2023-06-22 14:44:42.025000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc
+-rw-r--r--   0        0        0     5087 2023-06-22 14:44:42.029000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc
+-rw-r--r--   0        0        0     5963 2023-06-22 14:44:42.029000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc
+-rw-r--r--   0        0        0     5562 2023-06-22 14:44:41.628998 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc
+-rw-r--r--   0        0        0     7710 2023-06-22 14:44:42.033000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0    10821 2023-06-22 14:44:42.057000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc
+-rw-r--r--   0        0        0     6644 2023-06-22 14:44:41.812999 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     9573 2023-06-22 14:44:42.061000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc
+-rw-r--r--   0        0        0    17180 2023-06-22 14:44:42.069000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc
+-rw-r--r--   0        0        0     2538 2023-06-22 14:44:42.029000 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc
+-rw-r--r--   0        0        0     6260 2023-06-22 14:44:42.161001 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc
+-rw-r--r--   0        0        0     7131 2023-06-22 14:44:42.165001 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc
+-rw-r--r--   0        0        0    18001 2023-06-22 14:44:42.253001 renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc
+-rw-r--r--   0        0        0    16174 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/api.py
+-rw-r--r--   0        0        0     6987 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/azure.py
+-rw-r--r--   0        0        0     2225 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/common.py
+-rw-r--r--   0        0        0    21202 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/dataverse.py
+-rw-r--r--   0        0        0     3742 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/dataverse_metadata_templates.py
+-rw-r--r--   0        0        0     4829 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/doi.py
+-rw-r--r--   0        0        0     5623 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/external.py
+-rw-r--r--   0        0        0     5764 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/factory.py
+-rw-r--r--   0        0        0    10563 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/git.py
+-rw-r--r--   0        0        0    14308 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/local.py
+-rw-r--r--   0        0        0     6292 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/models.py
+-rw-r--r--   0        0        0    10118 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/olos.py
+-rw-r--r--   0        0        0    22167 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/renku.py
+-rw-r--r--   0        0        0     2553 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/repository.py
+-rw-r--r--   0        0        0     6413 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/s3.py
+-rw-r--r--   0        0        0     9427 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/web.py
+-rw-r--r--   0        0        0    18757 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/providers/zenodo.py
+-rw-r--r--   0        0        0     3973 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/request_model.py
+-rw-r--r--   0        0        0     5361 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/dataset/tag.py
+-rw-r--r--   0        0        0    25658 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/errors.py
+-rw-r--r--   0        0        0     1115 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/gc.py
+-rw-r--r--   0        0        0     7394 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/git.py
+-rw-r--r--   0        0        0     2151 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/githooks.py
+-rw-r--r--   0        0        0    16526 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/init.py
+-rw-r--r--   0        0        0      775 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/interface/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-22 14:44:42.017000 renku-2.6.0rc1/renku/core/interface/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4269 2023-06-22 14:44:44.133011 renku-2.6.0rc1/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     1246 2023-06-22 14:44:44.181011 renku-2.6.0rc1/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     2159 2023-06-22 14:44:42.081000 renku-2.6.0rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     2057 2023-06-22 14:44:44.121011 renku-2.6.0rc1/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0      959 2023-06-22 14:44:44.121011 renku-2.6.0rc1/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0     4402 2023-06-22 14:44:42.017000 renku-2.6.0rc1/renku/core/interface/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0        0        0     1579 2023-06-22 14:44:44.029011 renku-2.6.0rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc
+-rw-r--r--   0        0        0     3741 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/interface/activity_gateway.py
+-rw-r--r--   0        0        0     1418 2023-06-22 14:43:37.084648 renku-2.6.0rc1/renku/core/interface/database_gateway.py
+-rw-r--r--   0        0        0     2095 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/dataset_gateway.py
+-rw-r--r--   0        0        0     1996 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/plan_gateway.py
+-rw-r--r--   0        0        0     1212 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/project_gateway.py
+-rw-r--r--   0        0        0     4226 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/storage.py
+-rw-r--r--   0        0        0     1780 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/interface/workflow_file_parser.py
+-rw-r--r--   0        0        0    10639 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/login.py
+-rw-r--r--   0        0        0      764 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-22 14:44:41.748998 renku-2.6.0rc1/renku/core/migration/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1122 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0003__0_pyld2.py
+-rw-r--r--   0        0        0    15324 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0003__1_jsonld.py
+-rw-r--r--   0        0        0     9570 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0003__2_initial.py
+-rw-r--r--   0        0        0     1122 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0004__0_pyld2.py
+-rw-r--r--   0        0        0     5318 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0004__submodules.py
+-rw-r--r--   0        0        0     1548 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0005__1_pyld2.py
+-rw-r--r--   0        0        0    16075 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0005__2_cwl.py
+-rw-r--r--   0        0        0     1015 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0006__dataset_context.py
+-rw-r--r--   0        0        0     1430 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0007__source_url.py
+-rw-r--r--   0        0        0     1175 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0008__dataset_metadata.py
+-rw-r--r--   0        0        0    30683 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0009__new_metadata_storage.py
+-rw-r--r--   0        0        0    14077 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/m_0010__metadata_fixes.py
+-rw-r--r--   0        0        0    10163 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/migrate.py
+-rw-r--r--   0        0        0      770 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/__init__.py
+-rw-r--r--   0        0        0     5830 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/migration.py
+-rw-r--r--   0        0        0     3861 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/refs.py
+-rw-r--r--   0        0        0     5091 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v10.py
+-rw-r--r--   0        0        0    11828 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v3.py
+-rw-r--r--   0        0        0     2422 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v7.py
+-rw-r--r--   0        0        0     4587 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v8.py
+-rw-r--r--   0        0        0    74094 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/models/v9.py
+-rw-r--r--   0        0        0     7945 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/utils/__init__.py
+-rw-r--r--   0        0        0     6660 2023-06-22 14:44:41.748998 renku-2.6.0rc1/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8121 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/migration/utils/conversion.py
+-rw-r--r--   0        0        0      824 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/__init__.py
+-rw-r--r--   0        0        0      265 2023-06-22 14:44:41.632998 renku-2.6.0rc1/renku/core/plugin/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1033 2023-06-22 14:44:41.804999 renku-2.6.0rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc
+-rw-r--r--   0        0        0     1049 2023-06-22 14:44:41.808999 renku-2.6.0rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc
+-rw-r--r--   0        0        0     3246 2023-06-22 14:44:43.137006 renku-2.6.0rc1/renku/core/plugin/__pycache__/provider.cpython-39.pyc
+-rw-r--r--   0        0        0     1467 2023-06-22 14:44:45.081016 renku-2.6.0rc1/renku/core/plugin/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     1170 2023-06-22 14:44:45.265017 renku-2.6.0rc1/renku/core/plugin/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     4177 2023-06-22 14:44:44.689014 renku-2.6.0rc1/renku/core/plugin/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0        0        0     2978 2023-06-22 14:44:44.141011 renku-2.6.0rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc
+-rw-r--r--   0        0        0     1467 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/dataset_provider.py
+-rw-r--r--   0        0        0     3046 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/implementations/__init__.py
+-rw-r--r--   0        0        0     2540 2023-06-22 14:44:41.808999 renku-2.6.0rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1790 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/pluginmanager.py
+-rw-r--r--   0        0        0     3357 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/provider.py
+-rw-r--r--   0        0        0     1839 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/run.py
+-rw-r--r--   0        0        0     1515 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/session.py
+-rw-r--r--   0        0        0     4195 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/workflow.py
+-rw-r--r--   0        0        0     3065 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/plugin/workflow_file_parser.py
+-rw-r--r--   0        0        0     3355 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/project.py
+-rw-r--r--   0        0        0      770 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/session/__init__.py
+-rw-r--r--   0        0        0      210 2023-06-22 14:44:42.253001 renku-2.6.0rc1/renku/core/session/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    16099 2023-06-22 14:44:42.257001 renku-2.6.0rc1/renku/core/session/__pycache__/docker.cpython-39.pyc
+-rw-r--r--   0        0        0    16431 2023-06-22 14:44:42.453002 renku-2.6.0rc1/renku/core/session/__pycache__/renkulab.cpython-39.pyc
+-rw-r--r--   0        0        0     1449 2023-06-22 14:44:42.457002 renku-2.6.0rc1/renku/core/session/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0    22065 2023-06-22 14:43:37.088648 renku-2.6.0rc1/renku/core/session/docker.py
+-rw-r--r--   0        0        0    21512 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/session/renkulab.py
+-rw-r--r--   0        0        0    13503 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/session/session.py
+-rw-r--r--   0        0        0     2206 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/session/utils.py
+-rw-r--r--   0        0        0    19478 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/storage.py
+-rw-r--r--   0        0        0      760 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/template/__init__.py
+-rw-r--r--   0        0        0    22043 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/template/template.py
+-rw-r--r--   0        0        0    14612 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/template/usecase.py
+-rw-r--r--   0        0        0      756 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-22 14:44:41.372996 renku-2.6.0rc1/renku/core/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11124 2023-06-22 14:44:41.644998 renku-2.6.0rc1/renku/core/util/__pycache__/communication.cpython-39.pyc
+-rw-r--r--   0        0        0     6320 2023-06-22 14:44:44.181011 renku-2.6.0rc1/renku/core/util/__pycache__/contexts.cpython-39.pyc
+-rw-r--r--   0        0        0     1801 2023-06-22 14:44:41.744999 renku-2.6.0rc1/renku/core/util/__pycache__/datetime8601.cpython-39.pyc
+-rw-r--r--   0        0        0      933 2023-06-22 14:44:41.808999 renku-2.6.0rc1/renku/core/util/__pycache__/doi.cpython-39.pyc
+-rw-r--r--   0        0        0    33652 2023-06-22 14:44:41.380997 renku-2.6.0rc1/renku/core/util/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0      669 2023-06-22 14:44:42.457002 renku-2.6.0rc1/renku/core/util/__pycache__/jwt.cpython-39.pyc
+-rw-r--r--   0        0        0     6008 2023-06-22 14:44:41.748998 renku-2.6.0rc1/renku/core/util/__pycache__/metadata.cpython-39.pyc
+-rw-r--r--   0        0        0    11013 2023-06-22 14:44:41.588998 renku-2.6.0rc1/renku/core/util/__pycache__/os.cpython-39.pyc
+-rw-r--r--   0        0        0     6893 2023-06-22 14:44:42.245001 renku-2.6.0rc1/renku/core/util/__pycache__/requests.cpython-39.pyc
+-rw-r--r--   0        0        0     5971 2023-06-22 14:44:42.489002 renku-2.6.0rc1/renku/core/util/__pycache__/ssh.cpython-39.pyc
+-rw-r--r--   0        0        0     1736 2023-06-22 14:44:42.209001 renku-2.6.0rc1/renku/core/util/__pycache__/tabulate.cpython-39.pyc
+-rw-r--r--   0        0        0     4943 2023-06-22 14:44:41.644998 renku-2.6.0rc1/renku/core/util/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0        0        0     3737 2023-06-22 14:44:42.209001 renku-2.6.0rc1/renku/core/util/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     2663 2023-06-22 14:44:41.752998 renku-2.6.0rc1/renku/core/util/__pycache__/yaml.cpython-39.pyc
+-rw-r--r--   0        0        0    10282 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/communication.py
+-rw-r--r--   0        0        0     6617 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/contexts.py
+-rw-r--r--   0        0        0     2313 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/datetime8601.py
+-rw-r--r--   0        0        0     1376 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/doi.py
+-rw-r--r--   0        0        0    40689 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/git.py
+-rw-r--r--   0        0        0     1244 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/jwt.py
+-rw-r--r--   0        0        0     7036 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/metadata.py
+-rw-r--r--   0        0        0    12140 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/os.py
+-rw-r--r--   0        0        0     7626 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/requests.py
+-rw-r--r--   0        0        0     1611 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/shacl.py
+-rw-r--r--   0        0        0     6871 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/ssh.py
+-rw-r--r--   0        0        0     2158 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/tabulate.py
+-rw-r--r--   0        0        0     6228 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/urls.py
+-rw-r--r--   0        0        0     3878 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/util.py
+-rw-r--r--   0        0        0     2836 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/util/yaml.py
+-rw-r--r--   0        0        0      773 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/__init__.py
+-rw-r--r--   0        0        0      204 2023-06-22 14:44:42.489002 renku-2.6.0rc1/renku/core/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    18165 2023-06-22 14:44:44.189011 renku-2.6.0rc1/renku/core/workflow/__pycache__/activity.cpython-39.pyc
+-rw-r--r--   0        0        0    14583 2023-06-22 14:44:45.249017 renku-2.6.0rc1/renku/core/workflow/__pycache__/execute.cpython-39.pyc
+-rw-r--r--   0        0        0    26495 2023-06-22 14:44:44.129011 renku-2.6.0rc1/renku/core/workflow/__pycache__/plan.cpython-39.pyc
+-rw-r--r--   0        0        0    23623 2023-06-22 14:44:44.197011 renku-2.6.0rc1/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc
+-rw-r--r--   0        0        0    10263 2023-06-22 14:44:44.173011 renku-2.6.0rc1/renku/core/workflow/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     1660 2023-06-22 14:44:44.197011 renku-2.6.0rc1/renku/core/workflow/__pycache__/types.cpython-39.pyc
+-rw-r--r--   0        0        0     8676 2023-06-22 14:44:44.145011 renku-2.6.0rc1/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc
+-rw-r--r--   0        0        0     4780 2023-06-22 14:44:45.245017 renku-2.6.0rc1/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc
+-rw-r--r--   0        0        0    22713 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/activity.py
+-rw-r--r--   0        0        0      773 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/converters/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-22 14:44:42.493003 renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11079 2023-06-22 14:44:42.493003 renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc
+-rw-r--r--   0        0        0     4668 2023-06-22 14:44:44.025010 renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc
+-rw-r--r--   0        0        0    17937 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/converters/cwl.py
+-rw-r--r--   0        0        0     5142 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/converters/renku.py
+-rw-r--r--   0        0        0    18756 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/execute.py
+-rw-r--r--   0        0        0      769 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/model/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-22 14:44:43.141006 renku-2.6.0rc1/renku/core/workflow/model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4825 2023-06-22 14:44:43.141006 renku-2.6.0rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc
+-rw-r--r--   0        0        0    26172 2023-06-22 14:44:44.037011 renku-2.6.0rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc
+-rw-r--r--   0        0        0     6530 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/model/concrete_execution_graph.py
+-rw-r--r--   0        0        0    37866 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/model/workflow_file.py
+-rw-r--r--   0        0        0      775 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/parser/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-22 14:44:44.025010 renku-2.6.0rc1/renku/core/workflow/parser/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8620 2023-06-22 14:44:44.029011 renku-2.6.0rc1/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc
+-rw-r--r--   0        0        0    10631 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/parser/renku.py
+-rw-r--r--   0        0        0    34209 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/plan.py
+-rw-r--r--   0        0        0    33046 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/plan_factory.py
+-rw-r--r--   0        0        0      772 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/providers/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-22 14:44:44.205011 renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4631 2023-06-22 14:44:44.205011 renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc
+-rw-r--r--   0        0        0     3918 2023-06-22 14:44:44.689014 renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc
+-rw-r--r--   0        0        0    11194 2023-06-22 14:44:44.693014 renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc
+-rw-r--r--   0        0        0     5999 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/providers/cwltool.py
+-rw-r--r--   0        0        0     4271 2023-06-22 14:43:37.092648 renku-2.6.0rc1/renku/core/workflow/providers/local.py
+-rw-r--r--   0        0        0    13372 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/providers/toil.py
+-rw-r--r--   0        0        0    14384 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/run.py
+-rw-r--r--   0        0        0     1681 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/types.py
+-rw-r--r--   0        0        0     2869 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/update.py
+-rw-r--r--   0        0        0     8335 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/value_resolution.py
+-rw-r--r--   0        0        0     5089 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/core/workflow/workflow_file.py
+-rw-r--r--   0        0        0      767 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/__init__.py
+-rw-r--r--   0        0        0      114 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/defaults.ini
+-rw-r--r--   0        0        0     3364 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/gitignore.default
+-rwxr-xr-x   0        0        0     4474 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/pre-commit.sh
+-rw-r--r--   0        0        0    48383 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/data/shacl_shape.json
+-rw-r--r--   0        0        0      767 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/__init__.py
+-rw-r--r--   0        0        0      210 2023-06-22 14:44:41.596998 renku-2.6.0rc1/renku/domain_model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      388 2023-06-22 14:44:41.624998 renku-2.6.0rc1/renku/domain_model/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0    26295 2023-06-22 14:44:41.656998 renku-2.6.0rc1/renku/domain_model/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0      988 2023-06-22 14:44:41.804999 renku-2.6.0rc1/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc
+-rw-r--r--   0        0        0     2204 2023-06-22 14:44:44.197011 renku-2.6.0rc1/renku/domain_model/__pycache__/datastructures.cpython-39.pyc
+-rw-r--r--   0        0        0     2539 2023-06-22 14:44:42.009000 renku-2.6.0rc1/renku/domain_model/__pycache__/entity.cpython-39.pyc
+-rw-r--r--   0        0        0      575 2023-06-22 14:44:41.648998 renku-2.6.0rc1/renku/domain_model/__pycache__/enums.cpython-39.pyc
+-rw-r--r--   0        0        0     6097 2023-06-22 14:44:44.017011 renku-2.6.0rc1/renku/domain_model/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0    12164 2023-06-22 14:44:41.600998 renku-2.6.0rc1/renku/domain_model/__pycache__/project_context.cpython-39.pyc
+-rw-r--r--   0        0        0     7426 2023-06-22 14:44:42.449002 renku-2.6.0rc1/renku/domain_model/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     1092 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/constant.py
+-rw-r--r--   0        0        0    29611 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/dataset.py
+-rw-r--r--   0        0        0     1267 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/dataset_provider.py
+-rw-r--r--   0        0        0     2754 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/datastructures.py
+-rw-r--r--   0        0        0     2499 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/entity.py
+-rw-r--r--   0        0        0      971 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/enums.py
+-rw-r--r--   0        0        0     5059 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/git.py
+-rw-r--r--   0        0        0     8329 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/project.py
+-rw-r--r--   0        0        0    11817 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/project_context.py
+-rw-r--r--   0        0        0      829 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-22 14:44:42.005000 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11882 2023-06-22 14:44:44.137011 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc
+-rw-r--r--   0        0        0     4946 2023-06-22 14:44:42.005000 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc
+-rw-r--r--   0        0        0     1092 2023-06-22 14:44:42.009000 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     1363 2023-06-22 14:44:44.137011 renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc
+-rw-r--r--   0        0        0    13200 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/activity.py
+-rw-r--r--   0        0        0     5155 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/agent.py
+-rw-r--r--   0        0        0     1268 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/annotation.py
+-rw-r--r--   0        0        0     1530 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/provenance/parameter.py
+-rw-r--r--   0        0        0     6871 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/session.py
+-rw-r--r--   0        0        0     1471 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/sort.py
+-rw-r--r--   0        0        0    27042 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/template.py
+-rw-r--r--   0        0        0      782 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-22 14:44:43.137006 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13527 2023-06-22 14:44:43.657009 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc
+-rw-r--r--   0        0        0    15243 2023-06-22 14:44:43.661008 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc
+-rw-r--r--   0        0        0    15096 2023-06-22 14:44:43.665009 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc
+-rw-r--r--   0        0        0     1483 2023-06-22 14:44:43.137006 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc
+-rw-r--r--   0        0        0     4523 2023-06-22 14:44:44.141011 renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc
+-rw-r--r--   0        0        0    15917 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/composite_plan.py
+-rw-r--r--   0        0        0     1531 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/converters/__init__.py
+-rw-r--r--   0        0        0     1391 2023-06-22 14:44:44.025010 renku-2.6.0rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    18124 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/parameter.py
+-rw-r--r--   0        0        0    16602 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/plan.py
+-rw-r--r--   0        0        0     1639 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/provider.py
+-rw-r--r--   0        0        0     4660 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/domain_model/workflow/workflow_file.py
+-rw-r--r--   0        0        0      780 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-22 14:44:41.380997 renku-2.6.0rc1/renku/infrastructure/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    34957 2023-06-22 14:44:43.797009 renku-2.6.0rc1/renku/infrastructure/__pycache__/database.cpython-39.pyc
+-rw-r--r--   0        0        0     5073 2023-06-22 14:44:41.624998 renku-2.6.0rc1/renku/infrastructure/__pycache__/immutable.cpython-39.pyc
+-rw-r--r--   0        0        0     2259 2023-06-22 14:44:41.752998 renku-2.6.0rc1/renku/infrastructure/__pycache__/persistent.cpython-39.pyc
+-rw-r--r--   0        0        0    67803 2023-06-22 14:44:41.400997 renku-2.6.0rc1/renku/infrastructure/__pycache__/repository.cpython-39.pyc
+-rw-r--r--   0        0        0    41333 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/database.py
+-rw-r--r--   0        0        0      786 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/__init__.py
+-rw-r--r--   0        0        0      226 2023-06-22 14:44:42.205001 renku-2.6.0rc1/renku/infrastructure/gateway/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3238 2023-06-22 14:44:42.205001 renku-2.6.0rc1/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-39.pyc
+-rw-r--r--   0        0        0    12730 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/activity_gateway.py
+-rw-r--r--   0        0        0     5845 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/database_gateway.py
+-rw-r--r--   0        0        0     3743 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/dataset_gateway.py
+-rw-r--r--   0        0        0     3529 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/plan_gateway.py
+-rw-r--r--   0        0        0     1711 2023-06-22 14:43:37.096649 renku-2.6.0rc1/renku/infrastructure/gateway/project_gateway.py
+-rw-r--r--   0        0        0    18006 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/git_merger.py
+-rw-r--r--   0        0        0     4969 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/immutable.py
+-rw-r--r--   0        0        0     2394 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/persistent.py
+-rw-r--r--   0        0        0    72047 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/repository.py
+-rw-r--r--   0        0        0      784 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/storage/__init__.py
+-rw-r--r--   0        0        0      224 2023-06-22 14:44:42.021000 renku-2.6.0rc1/renku/infrastructure/storage/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1523 2023-06-22 14:44:42.021000 renku-2.6.0rc1/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc
+-rw-r--r--   0        0        0     1989 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/storage/factory.py
+-rw-r--r--   0        0        0     8859 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/infrastructure/storage/rclone.py
+-rw-r--r--   0        0        0      913 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      553 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      637 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      523 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/.github/dependabot.yml
+-rw-r--r--   0        0        0      396 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.github/workflows/github-project.yml
+-rw-r--r--   0        0        0     3940 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/.gitignore
+-rw-r--r--   0        0        0       27 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       37 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      984 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2087 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/R-minimal/Dockerfile
+-rw-r--r--   0        0        0     1603 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/environment.yml
+-rw-r--r--   0        0        0      360 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/install.R
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0      205 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal/{{ __sanitized_project_name__ }}.Rproj
+-rw-r--r--   0        0        0    14286 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/R-minimal.png
+-rw-r--r--   0        0        0     4846 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/README.md
+-rw-r--r--   0        0        0       27 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       37 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2077 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/bioc-minimal/Dockerfile
+-rw-r--r--   0        0        0     1603 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/install.R
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0      205 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioc-minimal/{{ __sanitized_project_name__ }}.Rproj
+-rw-r--r--   0        0        0    44589 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/bioconductor.png
+-rw-r--r--   0        0        0       27 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.dockerignore
+-rw-r--r--   0        0        0     6018 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       50 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2469 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/julia-minimal/Dockerfile
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/Manifest.toml
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/Project.toml
+-rw-r--r--   0        0        0     1842 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0    13782 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/julialang.png
+-rw-r--r--   0        0        0     1174 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/manifest.yaml
+-rw-r--r--   0        0        0       17 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.dockerignore
+-rw-r--r--   0        0        0       77 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       33 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2414 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/minimal/Dockerfile
+-rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0       27 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/python-minimal/.dockerignore
+-rw-r--r--   0        0        0     5401 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/python-minimal/.gitignore
+-rw-r--r--   0        0        0      450 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/python-minimal/.gitlab-ci.yml
+-rw-r--r--   0        0        0       33 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/.renku/renku.ini
+-rw-r--r--   0        0        0      976 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/.renkulfsignore
+-rw-r--r--   0        0        0     2159 2023-06-22 14:44:46.349023 renku-2.6.0rc1/renku/templates/python-minimal/Dockerfile
+-rw-r--r--   0        0        0     1597 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/data/.gitkeep
+-rw-r--r--   0        0        0      112 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/environment.yml
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/notebooks/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/requirements.txt
+-rw-r--r--   0        0        0     1439 2023-06-22 14:44:46.345023 renku-2.6.0rc1/renku/templates/python-minimal/workflows/my-workflow.yaml
+-rw-r--r--   0        0        0    25599 2023-06-22 14:44:46.341023 renku-2.6.0rc1/renku/templates/python-minimal.png
+-rw-r--r--   0        0        0      763 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/__init__.py
+-rw-r--r--   0        0        0      184 2023-06-22 14:44:41.212996 renku-2.6.0rc1/renku/ui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1268 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/__init__.py
+-rw-r--r--   0        0        0      763 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/graph/__init__.py
+-rw-r--r--   0        0        0     2519 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/graph/rdf.py
+-rw-r--r--   0        0        0      764 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/__init__.py
+-rw-r--r--   0        0        0    16448 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/activity.py
+-rw-r--r--   0        0        0     4648 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/dataset.py
+-rw-r--r--   0        0        0    10361 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/parameter.py
+-rw-r--r--   0        0        0     9227 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/plan.py
+-rw-r--r--   0        0        0     3643 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/models/project.py
+-rw-r--r--   0        0        0     2519 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/api/util.py
+-rw-r--r--   0        0        0     9319 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/__init__.py
+-rw-r--r--   0        0        0      922 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/__main__.py
+-rw-r--r--   0        0        0     8150 2023-06-22 14:44:41.216996 renku-2.6.0rc1/renku/ui/cli/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2117 2023-06-22 14:44:41.600998 renku-2.6.0rc1/renku/ui/cli/__pycache__/clone.cpython-39.pyc
+-rw-r--r--   0        0        0     7029 2023-06-22 14:44:41.604998 renku-2.6.0rc1/renku/ui/cli/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0    36275 2023-06-22 14:44:41.612998 renku-2.6.0rc1/renku/ui/cli/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     1787 2023-06-22 14:44:45.157016 renku-2.6.0rc1/renku/ui/cli/__pycache__/doctor.cpython-39.pyc
+-rw-r--r--   0        0        0      964 2023-06-22 14:44:45.157016 renku-2.6.0rc1/renku/ui/cli/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0        0        0     7957 2023-06-22 14:44:45.161017 renku-2.6.0rc1/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc
+-rw-r--r--   0        0        0      645 2023-06-22 14:44:45.185017 renku-2.6.0rc1/renku/ui/cli/__pycache__/gc.cpython-39.pyc
+-rw-r--r--   0        0        0     2168 2023-06-22 14:44:45.185017 renku-2.6.0rc1/renku/ui/cli/__pycache__/githooks.cpython-39.pyc
+-rw-r--r--   0        0        0     4041 2023-06-22 14:44:45.185017 renku-2.6.0rc1/renku/ui/cli/__pycache__/graph.cpython-39.pyc
+-rw-r--r--   0        0        0     9637 2023-06-22 14:44:45.189017 renku-2.6.0rc1/renku/ui/cli/__pycache__/init.cpython-39.pyc
+-rw-r--r--   0        0        0     7264 2023-06-22 14:44:45.189017 renku-2.6.0rc1/renku/ui/cli/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0     4296 2023-06-22 14:44:45.201017 renku-2.6.0rc1/renku/ui/cli/__pycache__/login.cpython-39.pyc
+-rw-r--r--   0        0        0     2066 2023-06-22 14:44:45.233017 renku-2.6.0rc1/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc
+-rw-r--r--   0        0        0     4585 2023-06-22 14:44:45.233017 renku-2.6.0rc1/renku/ui/cli/__pycache__/migrate.cpython-39.pyc
+-rw-r--r--   0        0        0     2306 2023-06-22 14:44:45.233017 renku-2.6.0rc1/renku/ui/cli/__pycache__/move.cpython-39.pyc
+-rw-r--r--   0        0        0     4028 2023-06-22 14:44:45.237017 renku-2.6.0rc1/renku/ui/cli/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0     1283 2023-06-22 14:44:45.237017 renku-2.6.0rc1/renku/ui/cli/__pycache__/remove.cpython-39.pyc
+-rw-r--r--   0        0        0     3485 2023-06-22 14:44:45.237017 renku-2.6.0rc1/renku/ui/cli/__pycache__/rerun.cpython-39.pyc
+-rw-r--r--   0        0        0     2761 2023-06-22 14:44:45.241017 renku-2.6.0rc1/renku/ui/cli/__pycache__/rollback.cpython-39.pyc
+-rw-r--r--   0        0        0    23646 2023-06-22 14:44:45.241017 renku-2.6.0rc1/renku/ui/cli/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0        0        0     2890 2023-06-22 14:44:45.257017 renku-2.6.0rc1/renku/ui/cli/__pycache__/save.cpython-39.pyc
+-rw-r--r--   0        0        0    10362 2023-06-22 14:44:45.261017 renku-2.6.0rc1/renku/ui/cli/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0        0        0    13046 2023-06-22 14:44:45.265017 renku-2.6.0rc1/renku/ui/cli/__pycache__/session.cpython-39.pyc
+-rw-r--r--   0        0        0     3715 2023-06-22 14:44:45.269017 renku-2.6.0rc1/renku/ui/cli/__pycache__/status.cpython-39.pyc
+-rw-r--r--   0        0        0     5061 2023-06-22 14:44:45.273017 renku-2.6.0rc1/renku/ui/cli/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0        0        0    10944 2023-06-22 14:44:45.277017 renku-2.6.0rc1/renku/ui/cli/__pycache__/template.cpython-39.pyc
+-rw-r--r--   0        0        0     5790 2023-06-22 14:44:45.277017 renku-2.6.0rc1/renku/ui/cli/__pycache__/update.cpython-39.pyc
+-rw-r--r--   0        0        0    41570 2023-06-22 14:44:45.281017 renku-2.6.0rc1/renku/ui/cli/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0        0        0     2594 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/clone.py
+-rw-r--r--   0        0        0     7953 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/config.py
+-rw-r--r--   0        0        0    42787 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/dataset.py
+-rw-r--r--   0        0        0     2333 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/doctor.py
+-rw-r--r--   0        0        0     1587 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/env.py
+-rw-r--r--   0        0        0     7931 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/exception_handler.py
+-rw-r--r--   0        0        0     1139 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/gc.py
+-rw-r--r--   0        0        0     2538 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/githooks.py
+-rw-r--r--   0        0        0     4950 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/graph.py
+-rw-r--r--   0        0        0    11113 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/init.py
+-rw-r--r--   0        0        0     8581 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/log.py
+-rw-r--r--   0        0        0     4845 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/login.py
+-rw-r--r--   0        0        0     2499 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/mergetool.py
+-rw-r--r--   0        0        0     5894 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/migrate.py
+-rw-r--r--   0        0        0     2881 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/move.py
+-rw-r--r--   0        0        0     5768 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/project.py
+-rw-r--r--   0        0        0     1754 2023-06-22 14:43:37.100648 renku-2.6.0rc1/renku/ui/cli/remove.py
+-rw-r--r--   0        0        0     4227 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/rerun.py
+-rw-r--r--   0        0        0     3249 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/rollback.py
+-rw-r--r--   0        0        0    26417 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/run.py
+-rw-r--r--   0        0        0     3510 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/save.py
+-rw-r--r--   0        0        0    11927 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/service.py
+-rw-r--r--   0        0        0    14738 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/session.py
+-rw-r--r--   0        0        0     5489 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/status.py
+-rw-r--r--   0        0        0     5604 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/storage.py
+-rw-r--r--   0        0        0    13434 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/template.py
+-rw-r--r--   0        0        0     6723 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/update.py
+-rw-r--r--   0        0        0      760 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-22 14:44:41.600998 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5720 2023-06-22 14:44:45.201017 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc
+-rw-r--r--   0        0        0     5071 2023-06-22 14:44:41.604998 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc
+-rw-r--r--   0        0        0      301 2023-06-22 14:44:41.604998 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/color.cpython-39.pyc
+-rw-r--r--   0        0        0      998 2023-06-22 14:44:45.237017 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc
+-rw-r--r--   0        0        0     7369 2023-06-22 14:44:45.197017 renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc
+-rw-r--r--   0        0        0     5409 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/callback.py
+-rw-r--r--   0        0        0     5473 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/click.py
+-rw-r--r--   0        0        0      842 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/color.py
+-rw-r--r--   0        0        0    14521 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/curses.py
+-rw-r--r--   0        0        0     1375 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/plugins.py
+-rw-r--r--   0        0        0     9917 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/utils/terminal.py
+-rw-r--r--   0        0        0    47787 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/cli/workflow.py
+-rw-r--r--   0        0        0      843 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/.env-example
+-rw-r--r--   0        0        0      756 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/__init__.py
+-rw-r--r--   0        0        0      189 2023-06-22 14:44:45.161017 renku-2.6.0rc1/renku/ui/service/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2109 2023-06-22 14:44:45.161017 renku-2.6.0rc1/renku/ui/service/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     1535 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/__init__.py
+-rw-r--r--   0        0        0     2917 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/base.py
+-rw-r--r--   0        0        0     1168 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/config.py
+-rw-r--r--   0        0        0     3315 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/files.py
+-rw-r--r--   0        0        0     2333 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/jobs.py
+-rw-r--r--   0        0        0      769 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/__init__.py
+-rw-r--r--   0        0        0     4356 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/file.py
+-rw-r--r--   0        0        0     2298 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/job.py
+-rw-r--r--   0        0        0     4043 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/project.py
+-rw-r--r--   0        0        0     1127 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/models/user.py
+-rw-r--r--   0        0        0     2558 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/projects.py
+-rw-r--r--   0        0        0      774 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/file.py
+-rw-r--r--   0        0        0     1711 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/job.py
+-rw-r--r--   0        0        0     1812 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/project.py
+-rw-r--r--   0        0        0     1227 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/serializers/user.py
+-rw-r--r--   0        0        0     1657 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/cache/users.py
+-rw-r--r--   0        0        0     3091 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/config.py
+-rw-r--r--   0        0        0      773 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/__init__.py
+-rw-r--r--   0        0        0      777 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/api/__init__.py
+-rw-r--r--   0        0        0     1085 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/api/abstract.py
+-rw-r--r--   0        0        0    15665 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/api/mixins.py
+-rw-r--r--   0        0        0     2647 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/cache_files_delete_chunks.py
+-rw-r--r--   0        0        0     7478 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/cache_files_upload.py
+-rw-r--r--   0        0        0     2239 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/cache_list_projects.py
+-rw-r--r--   0        0        0     1927 2023-06-22 14:43:37.104649 renku-2.6.0rc1/renku/ui/service/controllers/cache_list_uploaded.py
+-rw-r--r--   0        0        0     4823 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/cache_migrate_project.py
+-rw-r--r--   0        0        0     4905 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/cache_migrations_check.py
+-rw-r--r--   0        0        0     2350 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/cache_project_clone.py
+-rw-r--r--   0        0        0     2649 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/config_set.py
+-rw-r--r--   0        0        0     2333 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/config_show.py
+-rw-r--r--   0        0        0     5682 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_add_file.py
+-rw-r--r--   0        0        0     3916 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_create.py
+-rw-r--r--   0        0        0     5359 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_edit.py
+-rw-r--r--   0        0        0     2132 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_files_list.py
+-rw-r--r--   0        0        0     3333 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_import.py
+-rw-r--r--   0        0        0     2065 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_list.py
+-rw-r--r--   0        0        0     2637 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_remove.py
+-rw-r--r--   0        0        0     3290 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/datasets_unlink.py
+-rw-r--r--   0        0        0     5370 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/graph_export.py
+-rw-r--r--   0        0        0     3936 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/project_edit.py
+-rw-r--r--   0        0        0     3180 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/project_lock_status.py
+-rw-r--r--   0        0        0     2096 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/project_show.py
+-rw-r--r--   0        0        0     8049 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/templates_create_project.py
+-rw-r--r--   0        0        0     3103 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/templates_read_manifest.py
+-rw-r--r--   0        0        0      773 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/utils/__init__.py
+-rw-r--r--   0        0        0     1083 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/utils/datasets.py
+-rw-r--r--   0        0        0     3233 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/utils/project_clone.py
+-rw-r--r--   0        0        0     2664 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/utils/remote_project.py
+-rw-r--r--   0        0        0     1641 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/version.py
+-rw-r--r--   0        0        0     1389 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/versions_list.py
+-rw-r--r--   0        0        0     2441 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_export.py
+-rw-r--r--   0        0        0     2257 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_list.py
+-rw-r--r--   0        0        0     2146 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_show.py
+-rw-r--r--   0        0        0     6275 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/entrypoint.py
+-rw-r--r--   0        0        0    32144 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/errors.py
+-rw-r--r--   0        0        0      774 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/gateways/__init__.py
+-rw-r--r--   0        0        0     4083 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/gateways/gitlab_api_provider.py
+-rw-r--r--   0        0        0      793 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/interfaces/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/interfaces/git_api_provider.py
+-rw-r--r--   0        0        0      766 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/__init__.py
+-rw-r--r--   0        0        0     3035 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/cleanup.py
+-rw-r--r--   0        0        0      756 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/constants.py
+-rw-r--r--   0        0        0     1186 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/contexts.py
+-rw-r--r--   0        0        0     5288 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/datasets.py
+-rw-r--r--   0        0        0     1829 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/delayed_ctrl.py
+-rw-r--r--   0        0        0     2665 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/jobs/queues.py
+-rw-r--r--   0        0        0     1269 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/logger.py
+-rw-r--r--   0        0        0      644 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/logging.yaml
+-rw-r--r--   0        0        0     2742 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/scheduler.py
+-rw-r--r--   0        0        0      768 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/__init__.py
+-rw-r--r--   0        0        0    14561 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/cache.py
+-rw-r--r--   0        0        0     4843 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/common.py
+-rw-r--r--   0        0        0     2228 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/config.py
+-rw-r--r--   0        0        0     8503 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/datasets.py
+-rw-r--r--   0        0        0     2195 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/graph.py
+-rw-r--r--   0        0        0     5362 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/headers.py
+-rw-r--r--   0        0        0     1961 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/jobs.py
+-rw-r--r--   0        0        0     4510 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/project.py
+-rw-r--r--   0        0        0      911 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/rpc.py
+-rw-r--r--   0        0        0     5815 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/templates.py
+-rw-r--r--   0        0        0      773 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/v1/__init__.py
+-rw-r--r--   0        0        0     4212 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/v1/cache.py
+-rw-r--r--   0        0        0     1880 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/v1/templates.py
+-rw-r--r--   0        0        0     1171 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/version.py
+-rw-r--r--   0        0        0     1365 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/versions_list.py
+-rw-r--r--   0        0        0     6907 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/serializers/workflows.py
+-rw-r--r--   0        0        0     2186 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/utils/__init__.py
+-rw-r--r--   0        0        0     2220 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/utils/callback.py
+-rw-r--r--   0        0        0     1323 2023-06-22 14:43:37.108649 renku-2.6.0rc1/renku/ui/service/utils/json_encoder.py
+-rw-r--r--   0        0        0     1260 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/utils/squash.py
+-rw-r--r--   0        0        0     1427 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/utils/timeout.py
+-rw-r--r--   0        0        0     1761 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/__init__.py
+-rw-r--r--   0        0        0     2438 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/api_versions.py
+-rw-r--r--   0        0        0     4767 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/apispec.py
+-rw-r--r--   0        0        0     7427 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/cache.py
+-rw-r--r--   0        0        0     2957 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/config.py
+-rw-r--r--   0        0        0     8187 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/datasets.py
+-rw-r--r--   0        0        0     2961 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/decorators.py
+-rw-r--r--   0        0        0    15114 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/error_handlers.py
+-rw-r--r--   0        0        0     2084 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/graph.py
+-rw-r--r--   0        0        0     3267 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/jobs.py
+-rw-r--r--   0        0        0     3805 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/project.py
+-rw-r--r--   0        0        0     3592 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/templates.py
+-rw-r--r--   0        0        0      767 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/v1/__init__.py
+-rw-r--r--   0        0        0     4775 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/v1/cache.py
+-rw-r--r--   0        0        0     2634 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/v1/templates.py
+-rw-r--r--   0        0        0     1702 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/version.py
+-rw-r--r--   0        0        0     1676 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/versions_list.py
+-rw-r--r--   0        0        0     3873 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/views/workflow_plans.py
+-rw-r--r--   0        0        0     2890 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/ui/service/worker.py
+-rw-r--r--   0        0        0     1614 2023-06-22 14:43:37.112649 renku-2.6.0rc1/renku/version.py
+-rw-r--r--   0        0        0    17131 1970-01-01 00:00:00.000000 renku-2.6.0rc1/PKG-INFO
```

### Comparing `renku-2.5.0rc3/AUTHORS.rst` & `renku-2.6.0rc1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/CHANGES.rst` & `renku-2.6.0rc1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,32 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
 Changes
 =======
 
+`2.6.0 <https://github.com/SwissDataScienceCenter/renku-python/compare/v2.5.0...v2.6.0>`__ (2023-06-20)
+-------------------------------------------------------------------------------------------------------
+
+Bug Fixes
+~~~~~~~~~
+
+-  **service:** fixes importing private datasets in deployments with
+   external gitlab
+   (`#3523 <https://github.com/SwissDataScienceCenter/renku-python/issues/3523>`__)
+   (`d64c179 <https://github.com/SwissDataScienceCenter/renku-python/commit/d64c179857d0f1faa08c11a0cf0149eec97b4e46>`__)
+
+Features
+~~~~~~~~
+
+-  **service:** add support for horizontal scaling
+   (`#3178 <https://github.com/SwissDataScienceCenter/renku-python/issues/3178>`__)
+   (`fab2b58 <https://github.com/SwissDataScienceCenter/renku-python/commit/fab2b583f3c36fa179b6388ca7a28fa68b2aad8b>`__)
+
 `2.5.0 <https://github.com/SwissDataScienceCenter/renku-python/compare/v2.4.1...v2.5.0>`__ (2023-06-02)
 -------------------------------------------------------------------------------------------------------
 
 Bug Fixes
 ~~~~~~~~~
 
 -  **cli:** fix dataset update with external files
```

### Comparing `renku-2.5.0rc3/LICENSE` & `renku-2.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/README.rst` & `renku-2.6.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/pyproject.toml` & `renku-2.6.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool]
 
 [tool.poetry]
 name = "renku"
-version = "2.5.0rc3" # placeholder, see poetry-dynamic-versioning
+version = "2.6.0rc1" # placeholder, see poetry-dynamic-versioning
 description = "Python SDK and CLI for the Renku platform."
 license = "Apache License 2.0"
 keywords = ["Renku", "CLI"]
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -56,15 +56,15 @@
 attrs = ">=21.1.0,<23.2.0"
 bashlex = ">=0.16,<0.17"
 calamus = ">=0.3.13,<0.5"
 click = ">=8.0,<8.1.4"
 click-option-group = "<0.6.0,>=0.5.2"
 click-plugins = "==1.1.1"
 coverage = { version = "<6.5,>=4.5.3", extras=["toml"], optional = true }
-cryptography = ">=38.0.0,<41.0.0"
+cryptography = ">=38.0.0,<42.0.0"
 cwl-utils = ">=0.27,<0.28"
 cwltool = "==3.1.20230425144158"
 deal = ">=4.24.0,<5.0.0"
 deepdiff = ">=5.8,<7.0"
 deepmerge = "==1.0.1"
 docker = "<6,>=3.7.2"
 filelock = ">=3.3.0,<3.12.1"
@@ -93,15 +93,15 @@
 pyyaml = "<6.1.0,>=5.4"
 rdflib = "<7.0,>=6.0.0"
 requests = ">=2.23.0,<2.31.1"
 rich = ">=9.3.0,<13.4.0"
 shellingham = "1.5.0.post1"
 tabulate = ">=0.7.7,<0.9.1"
 toil = "==5.10.0"
-tqdm = "<4.62.4,>=4.48.1"
+tqdm = ">=4.48.1,<4.65.1"
 werkzeug = ">=1.0.0,<2.2.4"
 yagup = ">=0.1.1"
 yaspin = "==2.1.0"
 "zc.relation" = ">=1.1,<2.1"
 zodb = "==5.8.0"
 zstandard = ">=0.16.0,<0.22.0"
 
@@ -113,17 +113,17 @@
 flask = { version = "==2.2.5", optional = true }
 gunicorn = { version = "*", optional = true }
 marshmallow = { version = ">=3.18.0,<3.20.0", optional = true }
 marshmallow-oneofschema = { version = ">=3.0.1,<4.0.0", optional = true }
 pillow = { version = ">=9.0.0,<9.6", optional = true }
 python-dotenv = { version = ">=0.19.0,<0.21.0", optional = true }
 redis = { version = ">=3.5.3,<4.6.0", optional = true }
-rq = { version = "==1.14.1", optional = true }
+rq = { version = "==1.15.0", optional = true }
 rq-scheduler = { version = "==0.13.1", optional = true }
-sentry-sdk = { version = ">=1.5.11,<1.24.0", extras = ["flask"],  optional = true }
+sentry-sdk = { version = ">=1.5.11,<1.26.0", extras = ["flask"],  optional = true }
 walrus = { version = ">=0.8.2,<0.10.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "==23.1.0"
 flake8 = ">=6.0.0,<7.0.0"
 Flake8-pyproject = "==1.2.2"
 isort = "<5.10.2,>=5.3.2"
@@ -352,9 +352,9 @@
 requires = ["poetry-core>=1.3.0<1.7.0", "poetry-dynamic-versioning==0.21.5", "gitpython==3.1.24"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 
 [tool.coverage.paths]
 source = [
     "renku/",
-    "/opt/hostedtoolcache/Python/3.9.16/x64/lib/python3.9/site-packages/renku/"
+    "/opt/hostedtoolcache/Python/3.9.17/x64/lib/python3.9/site-packages/renku/"
 ]
```

### Comparing `renku-2.5.0rc3/renku/__init__.py` & `renku-2.6.0rc1/renku/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/__init__.py` & `renku-2.6.0rc1/renku/command/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/__pycache__/run.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1600 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 4006 0000  a........w.d@...
+00000000: 610d 0d0a 0000 0000 195e 9464 4006 0000  a........^.d@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6406 6407 8400 5a0a 650b  m.Z...d.d...Z.e.
 00000070: 6503 6502 650c 1900 1900 6408 9c02 6409  e.e.e.....d...d.
```

### Comparing `renku-2.5.0rc3/renku/command/__pycache__/util.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/__pycache__/util.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 be06 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 be06 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6503 6a04 6403  Z.d.d.l.Z.e.j.d.
 00000050: 6404 6405 6406 8d03 5a05 6503 6a04 6407  d.d.d...Z.e.j.d.
 00000060: 6404 6408 6406 8d03 5a06 6503 6a04 6409  d.d.d...Z.e.j.d.
 00000070: 6404 640a 6406 8d03 5a07 640b 640c 8400  d.d.d...Z.d.d...
```

### Comparing `renku-2.5.0rc3/renku/command/checks/__init__.py` & `renku-2.6.0rc1/renku/command/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/checks/activities.py` & `renku-2.6.0rc1/renku/command/checks/activities.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/checks/datasets.py` & `renku-2.6.0rc1/renku/command/checks/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/checks/githooks.py` & `renku-2.6.0rc1/renku/command/checks/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/checks/migration.py` & `renku-2.6.0rc1/renku/command/checks/migration.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/checks/project.py` & `renku-2.6.0rc1/renku/command/checks/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/checks/storage.py` & `renku-2.6.0rc1/renku/command/checks/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/checks/validate_shacl.py` & `renku-2.6.0rc1/renku/command/checks/validate_shacl.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/checks/workflow.py` & `renku-2.6.0rc1/renku/command/checks/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/clone.py` & `renku-2.6.0rc1/renku/command/clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/command_builder/__init__.py` & `renku-2.6.0rc1/renku/command/command_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/command_builder/__pycache__/command.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/command_builder/__pycache__/command.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 16678 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 2641 0000  a........w.d&A..
+00000000: 610d 0d0a 0000 0000 195e 9464 2641 0000  a........^.d&A..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/command/command_builder/command.py` & `renku-2.6.0rc1/renku/command/command_builder/command.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/command_builder/communication.py` & `renku-2.6.0rc1/renku/command/command_builder/communication.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/command_builder/database.py` & `renku-2.6.0rc1/renku/command/command_builder/database.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/command_builder/lock.py` & `renku-2.6.0rc1/renku/command/command_builder/lock.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/command_builder/migration.py` & `renku-2.6.0rc1/renku/command/command_builder/migration.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/command_builder/repo.py` & `renku-2.6.0rc1/renku/command/command_builder/repo.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/config.py` & `renku-2.6.0rc1/renku/command/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/dataset.py` & `renku-2.6.0rc1/renku/command/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/doctor.py` & `renku-2.6.0rc1/renku/command/doctor.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/format/__init__.py` & `renku-2.6.0rc1/renku/command/format/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/format/__pycache__/dataset_files.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/format/__pycache__/dataset_files.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6230 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 5618 0000  a........w.dV...
+00000000: 610d 0d0a 0000 0000 195e 9464 5618 0000  a........^.dV...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 b800 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 6d05 5a05 0100  l.m.Z.m.Z.m.Z...
 00000050: 6401 6404 6c06 6d07 5a07 6d08 5a08 6d09  d.d.l.m.Z.m.Z.m.
 00000060: 5a09 6d0a 5a0a 0100 6401 6405 6c0b 6d0c  Z.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6402 6406 9c01 6407 6408 8402  Z...d.d...d.d...
```

### Comparing `renku-2.5.0rc3/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/format/__pycache__/dataset_tags.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2098 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 3208 0000  a........w.d2...
+00000000: 610d 0d0a 0000 0000 195e 9464 3208 0000  a........^.d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 5500  .....@...sP...U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 0100  d.Z.d.d.l.m.Z...
 00000040: 6401 6403 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6404 6405 8400 5a06 6406 6407 8400 5a07  d.d...Z.d.d...Z.
 00000060: 6506 6507 6408 9c02 5a08 6505 6509 6504  e.e.d...Z.e.e.e.
 00000070: 6602 1900 650a 6409 3c00 640a 5300 290b  f...e.d.<.d.S.).
```

### Comparing `renku-2.5.0rc3/renku/command/format/__pycache__/datasets.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/format/__pycache__/datasets.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3236 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 a40c 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 a40c 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 9200 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6402 6405 9c01 6406  l.m.Z...d.d...d.
 00000060: 6407 8402 5a07 6408 6409 8400 5a08 640a  d...Z.d.d...Z.d.
 00000070: 640b 8400 5a09 640c 640d 8400 5a0a 6507  d...Z.d.d...Z.e.
```

### Comparing `renku-2.5.0rc3/renku/command/format/__pycache__/json.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/format/__pycache__/json.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 bc04 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 bc04 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6503 6a06 8303 5a06 6502 6a07 6503 6a08  e.j...Z.e.j.e.j.
 00000070: 6506 6406 8d02 5a08 6402 5300 2907 7a1b  e.d...Z.d.S.).z.
```

### Comparing `renku-2.5.0rc3/renku/command/format/__pycache__/session.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/format/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2402 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6209 0000  a........w.db...
+00000000: 610d 0d0a 0000 0000 195e 9464 6209 0000  a........^.db...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6405 6406 9c01  d.l.m.Z...d.d...
 00000060: 6502 6507 1900 6503 6508 1900 6407 9c02  e.e...e.e...d...
 00000070: 6408 6409 8406 5a09 6405 6406 9c01 6502  d.d...Z.d.d...e.
```

### Comparing `renku-2.5.0rc3/renku/command/format/__pycache__/tabulate.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/format/__pycache__/tabulate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2769 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 d10a 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 d10a 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 640d 6507 6408 9c01 6409  m.Z...d.e.d...d.
 00000060: 640a 8405 5a08 640b 640c 8400 5a09 6405  d...Z.d.d...Z.d.
 00000070: 5300 290e 7a20 5461 6275 6c61 7220 666f  S.).z Tabular fo
```

### Comparing `renku-2.5.0rc3/renku/command/format/__pycache__/workflow.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/format/__pycache__/workflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2728 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 a80a 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 a80a 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9600 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 6d04 5a04 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6401 6405 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a08 0100 6402 6406 9c01 6407 6408 8402  Z...d.d...d.d...
 00000070: 5a09 6409 640a 8400 5a0a 640b 640c 8400  Z.d.d...Z.d.d...
```

### Comparing `renku-2.5.0rc3/renku/command/format/activity.py` & `renku-2.6.0rc1/renku/command/format/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/format/dataset_files.py` & `renku-2.6.0rc1/renku/command/format/dataset_files.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/format/dataset_tags.py` & `renku-2.6.0rc1/renku/command/format/dataset_tags.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/format/datasets.py` & `renku-2.6.0rc1/renku/command/format/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/format/json.py` & `renku-2.6.0rc1/renku/command/format/json.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/format/session.py` & `renku-2.6.0rc1/renku/command/format/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/format/tabulate.py` & `renku-2.6.0rc1/renku/command/format/tabulate.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/format/workflow.py` & `renku-2.6.0rc1/renku/command/format/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/gc.py` & `renku-2.6.0rc1/renku/command/gc.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/githooks.py` & `renku-2.6.0rc1/renku/command/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/graph.py` & `renku-2.6.0rc1/renku/command/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/group.py` & `renku-2.6.0rc1/renku/command/group.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/init.py` & `renku-2.6.0rc1/renku/command/init.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/log.py` & `renku-2.6.0rc1/renku/command/log.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/login.py` & `renku-2.6.0rc1/renku/command/login.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/mergetool.py` & `renku-2.6.0rc1/renku/command/mergetool.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/migrate.py` & `renku-2.6.0rc1/renku/command/migrate.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/move.py` & `renku-2.6.0rc1/renku/command/move.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/options.py` & `renku-2.6.0rc1/renku/command/options.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/project.py` & `renku-2.6.0rc1/renku/command/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/remove.py` & `renku-2.6.0rc1/renku/command/remove.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/rerun.py` & `renku-2.6.0rc1/renku/command/rerun.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/rollback.py` & `renku-2.6.0rc1/renku/command/rollback.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/run.py` & `renku-2.6.0rc1/renku/command/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/save.py` & `renku-2.6.0rc1/renku/command/save.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/__init__.py` & `renku-2.6.0rc1/renku/command/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/__pycache__/agent.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/schema/__pycache__/agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2478 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 ae09 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 ae09 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 6d0d 5a0d 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
```

### Comparing `renku-2.5.0rc3/renku/command/schema/__pycache__/annotation.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/schema/__pycache__/annotation.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1235 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 d304 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 d304 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a0a 6407 5300 2908 7a1a 416e 6e6f 7461  Z.d.S.).z.Annota
```

### Comparing `renku-2.5.0rc3/renku/command/schema/__pycache__/calamus.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/schema/__pycache__/calamus.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 8986 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 1a23 0000  a........w.d.#..
+00000000: 610d 0d0a 0000 0000 195e 9464 1a23 0000  a........^.d.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6406 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/command/schema/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/schema/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 8210 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 1220 0000  a........w.d. ..
+00000000: 610d 0d0a 0000 0000 195e 9464 1220 0000  a........^.d. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/command/schema/__pycache__/entity.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/schema/__pycache__/entity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1445 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 a505 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 a505 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c07 6d08 5a08 6d09 5a09 0100 4700  d.l.m.Z.m.Z...G.
 00000060: 6404 6405 8400 6405 6502 8303 5a0a 4700  d.d...d.e...Z.G.
 00000070: 6406 6407 8400 6407 650a 8303 5a0b 6408  d.d...d.e...Z.d.
```

### Comparing `renku-2.5.0rc3/renku/command/schema/activity.py` & `renku-2.6.0rc1/renku/command/schema/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/agent.py` & `renku-2.6.0rc1/renku/command/schema/agent.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/annotation.py` & `renku-2.6.0rc1/renku/command/schema/annotation.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/calamus.py` & `renku-2.6.0rc1/renku/command/schema/calamus.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/composite_plan.py` & `renku-2.6.0rc1/renku/command/schema/composite_plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/dataset.py` & `renku-2.6.0rc1/renku/command/schema/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/entity.py` & `renku-2.6.0rc1/renku/command/schema/entity.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/parameter.py` & `renku-2.6.0rc1/renku/command/schema/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/plan.py` & `renku-2.6.0rc1/renku/command/schema/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/project.py` & `renku-2.6.0rc1/renku/command/schema/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/schema/workflow_file.py` & `renku-2.6.0rc1/renku/command/schema/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/session.py` & `renku-2.6.0rc1/renku/command/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/status.py` & `renku-2.6.0rc1/renku/command/status.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/storage.py` & `renku-2.6.0rc1/renku/command/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/template.py` & `renku-2.6.0rc1/renku/command/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/update.py` & `renku-2.6.0rc1/renku/command/update.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/util.py` & `renku-2.6.0rc1/renku/command/util.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/version.py` & `renku-2.6.0rc1/renku/command/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/__init__.py` & `renku-2.6.0rc1/renku/command/view_model/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/view_model/__pycache__/activity_graph.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 14258 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 b237 0000  a........w.d.7..
+00000000: 610d 0d0a 0000 0000 195e 9464 b237 0000  a........^.d.7..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6401 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/command/view_model/__pycache__/agent.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/view_model/__pycache__/agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1657 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 7906 0000  a........w.dy...
+00000000: 610d 0d0a 0000 0000 195e 9464 7906 0000  a........^.dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 8302 5a05 6406 5300 2907 7a11  ..d...Z.d.S.).z.
 00000060: 4167 656e 7420 7669 6577 206d 6f64 656c  Agent view model
 00000070: 2ee9 0000 0000 2901 da08 4f70 7469 6f6e  ......)...Option
```

### Comparing `renku-2.5.0rc3/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/view_model/__pycache__/composite_plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 8768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 4022 0000  a........w.d@"..
+00000000: 610d 0d0a 0000 0000 195e 9464 4022 0000  a........^.d@"..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 3001 0000 5500  .....@...s0...U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d02 5a02 6d03 5a03 0100 6401 6404  l.m.Z.m.Z...d.d.
 00000050: 6c04 6d05 5a05 6d06 5a06 6d07 5a07 6d08  l.m.Z.m.Z.m.Z.m.
 00000060: 5a08 6d09 5a09 6d0a 5a0a 0100 6401 6405  Z.m.Z.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 6401 6406 6c0d 6d0e  l.m.Z...d.d.l.m.
```

### Comparing `renku-2.5.0rc3/renku/command/view_model/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/view_model/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2138 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 5a08 0000  a........w.dZ...
+00000000: 610d 0d0a 0000 0000 195e 9464 5a08 0000  a........^.dZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 4700  d.l.m.Z.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a06 4700 6406  d.d...d...Z.G.d.
 00000060: 6407 8400 6407 8302 5a07 6408 5300 2909  d...d...Z.d.S.).
 00000070: 7a1f 4461 7461 7365 742f 4461 7461 7365  z.Dataset/Datase
```

### Comparing `renku-2.5.0rc3/renku/command/view_model/__pycache__/log.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/view_model/__pycache__/log.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 12497 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 d130 0000  a........w.d.0..
+00000000: 610d 0d0a 0000 0000 195e 9464 d130 0000  a........^.d.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d04 5a04 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6406 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/command/view_model/__pycache__/plan.cpython-39.pyc` & `renku-2.6.0rc1/renku/command/view_model/__pycache__/plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 9377 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 a124 0000  a........w.d.$..
+00000000: 610d 0d0a 0000 0000 195e 9464 a124 0000  a........^.d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 e400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6401 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6401 6407 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/command/view_model/activity_graph.py` & `renku-2.6.0rc1/renku/command/view_model/activity_graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/agent.py` & `renku-2.6.0rc1/renku/command/view_model/agent.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/composite_plan.py` & `renku-2.6.0rc1/renku/command/view_model/composite_plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/dataset.py` & `renku-2.6.0rc1/renku/command/view_model/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/graph.py` & `renku-2.6.0rc1/renku/command/view_model/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/log.py` & `renku-2.6.0rc1/renku/command/view_model/log.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/plan.py` & `renku-2.6.0rc1/renku/command/view_model/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/project.py` & `renku-2.6.0rc1/renku/command/view_model/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/template.py` & `renku-2.6.0rc1/renku/command/view_model/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/text_canvas.py` & `renku-2.6.0rc1/renku/command/view_model/text_canvas.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/view_model/workflow_file.py` & `renku-2.6.0rc1/renku/command/view_model/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/command/workflow.py` & `renku-2.6.0rc1/renku/command/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/__init__.py` & `renku-2.6.0rc1/renku/core/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/__pycache__/config.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/__pycache__/config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6170 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 1a18 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 1a18 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6407 6408 8400 5a0b 6409 640a 8400  ..d.d...Z.d.d...
```

### Comparing `renku-2.5.0rc3/renku/core/__pycache__/constant.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/__pycache__/constant.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2717 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9d0a 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 9d0a 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 d200 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6401 6404 6c04 6d05  l.m.Z...d.d.l.m.
 00000050: 5a05 0100 6405 5a06 6406 5a07 6407 5a08  Z...d.Z.d.Z.d.Z.
 00000060: 6408 5a09 6409 5a0a 6501 6a0b a00c 6507  d.Z.d.Z.e.j...e.
 00000070: 650a a102 5a0d 640a 5a0e 640b 5a0f 6510  e...Z.d.Z.d.Z.e.
```

### Comparing `renku-2.5.0rc3/renku/core/__pycache__/errors.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/__pycache__/errors.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 25658 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 3a64 0000  a........w.d:d..
+00000000: 610d 0d0a 0000 0000 195e 9464 3a64 0000  a........^.d:d..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5c06 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6401 6404 6c07 5a07 6401 6405 6c08  ..d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 650c 8303  ..G.d.d...d.e...
```

### Comparing `renku-2.5.0rc3/renku/core/__pycache__/git.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 7394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 e21c 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 e21c 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/__pycache__/login.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/__pycache__/login.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 10639 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8f29 0000  a........w.d.)..
+00000000: 610d 0d0a 0000 0000 195e 9464 8f29 0000  a........^.d.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 b201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 0100 6401 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/__pycache__/storage.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/__pycache__/storage.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 19478 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 164c 0000  a........w.d.L..
+00000000: 610d 0d0a 0000 0000 195e 9464 164c 0000  a........^.d.L..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2203 0000 6400  .....@...s"...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6403 6c07 6d08 5a08 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6404 6c09 6d0a 5a0a 0100 6401 6405 6c0b  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/config.py` & `renku-2.6.0rc1/renku/core/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/constant.py` & `renku-2.6.0rc1/renku/core/constant.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/__init__.py` & `renku-2.6.0rc1/renku/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/__pycache__/context.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/__pycache__/context.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2954 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8a0b 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 8a0b 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 50044 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 7cc3 0000  a........w.d|...
+00000000: 610d 0d0a 0000 0000 195e 9464 7cc3 0000  a........^.d|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0013 0000 0040 0000 0073 1807 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/__pycache__/dataset_add.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/__pycache__/dataset_add.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 21429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 b553 0000  a........w.d.S..
+00000000: 610d 0d0a 0000 0000 195e 9464 b553 0000  a........^.d.S..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0011 0000 0040 0000 0073 6403 0000 6400  .....@...sd...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 5a04 6401 6402 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 5a05 6401 6403 6c06 6d07 5a07 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/__pycache__/datasets_provenance.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 9747 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 1326 0000  a........w.d.&..
+00000000: 610d 0d0a 0000 0000 195e 9464 1326 0000  a........^.d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6401 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/__pycache__/pointer_file.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/__pycache__/pointer_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4296 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 c810 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 c810 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2001 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/__pycache__/request_model.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/__pycache__/request_model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3973 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 850f 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 850f 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6401 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/__pycache__/tag.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/__pycache__/tag.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5361 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 f114 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 f114 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/context.py` & `renku-2.6.0rc1/renku/core/dataset/context.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/dataset.py` & `renku-2.6.0rc1/renku/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/dataset_add.py` & `renku-2.6.0rc1/renku/core/dataset/dataset_add.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/datasets_provenance.py` & `renku-2.6.0rc1/renku/core/dataset/datasets_provenance.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/pointer_file.py` & `renku-2.6.0rc1/renku/core/dataset/pointer_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__init__.py` & `renku-2.6.0rc1/renku/core/dataset/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/api.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 16174 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 2e3f 0000  a........w.d.?..
+00000000: 610d 0d0a 0000 0000 195e 9464 2e3f 0000  a........^.d.?..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/azure.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6987 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 4b1b 0000  a........w.dK...
+00000000: 610d 0d0a 0000 0000 195e 9464 4b1b 0000  a........^.dK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1401 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/common.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2225 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 b108 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 b108 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6408 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/dataverse.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 21202 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 d252 0000  a........w.d.R..
+00000000: 610d 0d0a 0000 0000 195e 9464 d252 0000  a........^.d.R..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 de01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/dataverse_metadata_templates.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3742 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9e0e 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 9e0e 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5300 2906 7a1d 4461 7461 7665  Z.d.S.).z.Datave
 00000050: 7273 6520 6d65 7461 6461 7461 2074 656d  rse metadata tem
 00000060: 706c 6174 6573 2e61 e007 0000 0a7b 0a20  plates.a.....{. 
 00000070: 2020 2022 6461 7461 7365 7456 6572 7369     "datasetVersi
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/doi.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4829 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 dd12 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 dd12 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6407 5a0e 4700  m.Z.m.Z...d.Z.G.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/external.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5623 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 f715 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 f715 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0173 1001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6401 6407 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/factory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5764 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8416 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 8416 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6404 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 0100 6401 6406 6c0f  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 10563 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 4329 0000  a........w.dC)..
+00000000: 610d 0d0a 0000 0000 195e 9464 4329 0000  a........^.dC)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3001 0000 6400  .....@...s0...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/local.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 14308 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 e437 0000  a........w.d.7..
+00000000: 610d 0d0a 0000 0000 195e 9464 e437 0000  a........^.d.7..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6405 6c0c 6d0d 5a0d 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6292 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9418 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 9418 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3601 0000 6400  .....@...s6...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/olos.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 10118 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8627 0000  a........w.d.'..
+00000000: 610d 0d0a 0000 0000 195e 9464 8627 0000  a........^.d.'..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 f000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c02 6d09 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6401  d.l.m.Z.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/renku.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 22167 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9756 0000  a........w.d.V..
+00000000: 610d 0d0a 0000 0000 195e 9464 9756 0000  a........^.d.V..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/repository.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2553 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 f909 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 f909 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6401  d.l.m.Z.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6506 7258 6401  d.l.m.Z...e.rXd.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6401 6407 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/s3.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6413 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 0d19 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 0d19 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  d.l.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/web.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 9427 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 d324 0000  a........w.d.$..
+00000000: 610d 0d0a 0000 0000 195e 9464 d324 0000  a........^.d.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 5c01 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6401 6405 6c0c  m.Z.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 6401 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/dataset/providers/__pycache__/zenodo.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 18757 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 4549 0000  a........w.dEI..
+00000000: 610d 0d0a 0000 0000 195e 9464 4549 0000  a........^.dEI..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8801 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/api.py` & `renku-2.6.0rc1/renku/core/dataset/providers/api.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/azure.py` & `renku-2.6.0rc1/renku/core/dataset/providers/azure.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/common.py` & `renku-2.6.0rc1/renku/core/dataset/providers/common.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/dataverse.py` & `renku-2.6.0rc1/renku/core/dataset/providers/dataverse.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/dataverse_metadata_templates.py` & `renku-2.6.0rc1/renku/core/dataset/providers/dataverse_metadata_templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/doi.py` & `renku-2.6.0rc1/renku/core/dataset/providers/doi.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/external.py` & `renku-2.6.0rc1/renku/core/dataset/providers/external.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/factory.py` & `renku-2.6.0rc1/renku/core/dataset/providers/factory.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/git.py` & `renku-2.6.0rc1/renku/core/dataset/providers/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/local.py` & `renku-2.6.0rc1/renku/core/dataset/providers/local.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/models.py` & `renku-2.6.0rc1/renku/core/dataset/providers/models.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/olos.py` & `renku-2.6.0rc1/renku/core/dataset/providers/olos.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/renku.py` & `renku-2.6.0rc1/renku/core/dataset/providers/renku.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/repository.py` & `renku-2.6.0rc1/renku/core/dataset/providers/repository.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/s3.py` & `renku-2.6.0rc1/renku/core/dataset/providers/s3.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/web.py` & `renku-2.6.0rc1/renku/core/dataset/providers/web.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/providers/zenodo.py` & `renku-2.6.0rc1/renku/core/dataset/providers/zenodo.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/request_model.py` & `renku-2.6.0rc1/renku/core/dataset/request_model.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/dataset/tag.py` & `renku-2.6.0rc1/renku/core/dataset/tag.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/errors.py` & `renku-2.6.0rc1/renku/core/errors.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/gc.py` & `renku-2.6.0rc1/renku/core/gc.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/git.py` & `renku-2.6.0rc1/renku/core/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/githooks.py` & `renku-2.6.0rc1/renku/core/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/init.py` & `renku-2.6.0rc1/renku/core/init.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/interface/__init__.py` & `renku-2.6.0rc1/renku/core/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/interface/__pycache__/activity_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3741 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9d0e 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 9d0e 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 6d0d 5a0d 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
```

### Comparing `renku-2.5.0rc3/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/interface/__pycache__/database_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1418 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8a05 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 8a05 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6504  d.l.m.Z.m.Z...e.
 00000050: 7230 6401 6404 6c06 6d07 5a07 0100 4700  r0d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6502 8303 5a08 6407  d.d...d.e...Z.d.
 00000070: 5300 2908 7a21 5265 6e6b 7520 6461 7461  S.).z!Renku data
```

### Comparing `renku-2.5.0rc3/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/interface/__pycache__/dataset_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2095 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 2f08 0000  a........w.d/...
+00000000: 610d 0d0a 0000 0000 195e 9464 2f08 0000  a........^.d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6504 7238 6401 6404 6c07 6d08 5a08  ..e.r8d.d.l.m.Z.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6502 8303 5a0a 6407 5300 2908 7a20 5265  e...Z.d.S.).z Re
```

### Comparing `renku-2.5.0rc3/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/interface/__pycache__/plan_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1996 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 cc07 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 cc07 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6401 6404 6c07 6d08 5a08 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6502 8303 5a09 6407  d.d...d.e...Z.d.
 00000070: 5300 2908 7a1d 5265 6e6b 7520 706c 616e  S.).z.Renku plan
```

### Comparing `renku-2.5.0rc3/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/interface/__pycache__/project_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 bc04 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 bc04 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6504 722c 6401  d.l.m.Z...e.r,d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6502 8303 5a07 6407 5300 2908  ..d.e...Z.d.S.).
 00000070: 7a20 5265 6e6b 7520 7072 6f6a 6563 7420  z Renku project
```

### Comparing `renku-2.5.0rc3/renku/core/interface/__pycache__/storage.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/interface/__pycache__/storage.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4226 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8210 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 8210 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6507  m.Z.m.Z.m.Z...e.
 00000070: 7254 6401 6406 6c0c 6d0d 5a0d 6d0e 5a0e  rTd.d.l.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/interface/__pycache__/workflow_file_parser.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1780 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 f406 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 f406 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6509  m.Z.m.Z.m.Z...e.
 00000070: 7250 6401 6406 6c0c 6d0d 5a0d 0100 4700  rPd.d.l.m.Z...G.
```

### Comparing `renku-2.5.0rc3/renku/core/interface/activity_gateway.py` & `renku-2.6.0rc1/renku/core/interface/activity_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/interface/database_gateway.py` & `renku-2.6.0rc1/renku/core/interface/database_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/interface/dataset_gateway.py` & `renku-2.6.0rc1/renku/core/interface/dataset_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/interface/plan_gateway.py` & `renku-2.6.0rc1/renku/core/interface/plan_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/interface/project_gateway.py` & `renku-2.6.0rc1/renku/core/interface/project_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/interface/storage.py` & `renku-2.6.0rc1/renku/core/interface/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/interface/workflow_file_parser.py` & `renku-2.6.0rc1/renku/core/interface/workflow_file_parser.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/login.py` & `renku-2.6.0rc1/renku/core/login.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/__init__.py` & `renku-2.6.0rc1/renku/core/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0003__0_pyld2.py` & `renku-2.6.0rc1/renku/core/migration/m_0003__0_pyld2.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0003__1_jsonld.py` & `renku-2.6.0rc1/renku/core/migration/m_0003__1_jsonld.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0003__2_initial.py` & `renku-2.6.0rc1/renku/core/migration/m_0003__2_initial.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0004__0_pyld2.py` & `renku-2.6.0rc1/renku/core/migration/m_0004__0_pyld2.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0004__submodules.py` & `renku-2.6.0rc1/renku/core/migration/m_0004__submodules.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0005__1_pyld2.py` & `renku-2.6.0rc1/renku/core/migration/m_0005__1_pyld2.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0005__2_cwl.py` & `renku-2.6.0rc1/renku/core/migration/m_0005__2_cwl.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0006__dataset_context.py` & `renku-2.6.0rc1/renku/core/migration/m_0006__dataset_context.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0007__source_url.py` & `renku-2.6.0rc1/renku/core/migration/m_0007__source_url.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0008__dataset_metadata.py` & `renku-2.6.0rc1/renku/core/migration/m_0008__dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0009__new_metadata_storage.py` & `renku-2.6.0rc1/renku/core/migration/m_0009__new_metadata_storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/m_0010__metadata_fixes.py` & `renku-2.6.0rc1/renku/core/migration/m_0010__metadata_fixes.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/migrate.py` & `renku-2.6.0rc1/renku/core/migration/migrate.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/models/__init__.py` & `renku-2.6.0rc1/renku/core/migration/models/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/models/migration.py` & `renku-2.6.0rc1/renku/core/migration/models/migration.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/models/refs.py` & `renku-2.6.0rc1/renku/core/migration/models/refs.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/models/v10.py` & `renku-2.6.0rc1/renku/core/migration/models/v10.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/models/v3.py` & `renku-2.6.0rc1/renku/core/migration/models/v3.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/models/v7.py` & `renku-2.6.0rc1/renku/core/migration/models/v7.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/models/v8.py` & `renku-2.6.0rc1/renku/core/migration/models/v8.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/models/v9.py` & `renku-2.6.0rc1/renku/core/migration/models/v9.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/utils/__init__.py` & `renku-2.6.0rc1/renku/core/migration/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/migration/utils/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 7945 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 091f 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 091f 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 0c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6401 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/migration/utils/conversion.py` & `renku-2.6.0rc1/renku/core/migration/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/plugin/__init__.py` & `renku-2.6.0rc1/renku/core/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/plugin/__pycache__/dataset_provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1467 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 bb05 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 bb05 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6401 6403 6c05 5a05 6502  m.Z...d.d.l.Z.e.
 00000050: 7230 6401 6404 6c06 6d07 5a07 0100 6505  r0d.d.l.m.Z...e.
 00000060: a008 6405 a101 5a09 6509 6406 6407 9c01  ..d...Z.e.d.d...
 00000070: 6408 6409 8404 8301 5a0a 640a 6407 9c01  d.d.....Z.d.d...
```

### Comparing `renku-2.5.0rc3/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/plugin/__pycache__/pluginmanager.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1790 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 fe06 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 fe06 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6502 6403 8301 6404 6405  d.l.Z.e.d...d.d.
 00000050: 8400 8301 5a04 6403 5300 2906 7a14 706c  ....Z.d.S.).z.pl
 00000060: 7567 6779 2050 6c75 6769 6e20 7365 7475  uggy Plugin setu
 00000070: 702e e900 0000 0029 01da 096c 7275 5f63  p......)...lru_c
```

### Comparing `renku-2.5.0rc3/renku/core/plugin/__pycache__/provider.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/plugin/__pycache__/provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3357 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 1d0d 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 1d0d 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6504 7238 6401  m.Z.m.Z...e.r8d.
 00000060: 6404 6c09 5a0a 6401 6404 6c0b 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6401 6406 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/plugin/__pycache__/run.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/plugin/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1839 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 2f07 0000  a........w.d/...
+00000000: 610d 0d0a 0000 0000 195e 9464 2f07 0000  a........^.d/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 6403  Z.d.d.l.Z.e...d.
 00000040: a101 5a03 6503 6404 6405 8400 8301 5a04  ..Z.e.d.d.....Z.
 00000050: 6503 6406 6407 8400 8301 5a05 6503 6408  e.d.d.....Z.e.d.
 00000060: 6409 8400 8301 5a06 6402 5300 290a 7a29  d.....Z.d.S.).z)
 00000070: 506c 7567 696e 2068 6f6f 6b73 2066 6f72  Plugin hooks for
```

### Comparing `renku-2.5.0rc3/renku/core/plugin/__pycache__/session.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/plugin/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1515 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 eb05 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 eb05 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a04 6401 6404 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6504 a007 6405 a101 5a08  m.Z...e...d...Z.
 00000060: 6508 6503 6506 6509 6602 1900 6406 9c01  e.e.e.e.f...d...
 00000070: 6407 6408 8404 8301 5a0a 6502 6506 1900  d.d.....Z.e.e...
```

### Comparing `renku-2.5.0rc3/renku/core/plugin/__pycache__/workflow.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/plugin/__pycache__/workflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6310 0000  a........w.dc...
+00000000: 610d 0d0a 0000 0000 195e 9464 6310 0000  a........^.dc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 de00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/plugin/__pycache__/workflow_file_parser.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3065 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 f90b 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 f90b 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 0100 6401 6404 6c08 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6504 7258 6401 6407 6c0d  m.Z...e.rXd.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/plugin/dataset_provider.py` & `renku-2.6.0rc1/renku/core/plugin/dataset_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/plugin/implementations/__init__.py` & `renku-2.6.0rc1/renku/core/plugin/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/plugin/implementations/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3046 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 e60b 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 e60b 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 ca01 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 6d02 5a02 6d03  d.Z.d.d.l.m.Z.m.
 00000040: 5a03 6d04 5a04 0100 6401 6403 6c05 6d06  Z.m.Z...d.d.l.m.
 00000050: 5a06 0100 6401 6404 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 6401 6405 6c09 6d0a 5a0a 0100 6401 6406  d.d.l.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 6401 6407 6c0d 6d0e  l.m.Z...d.d.l.m.
```

### Comparing `renku-2.5.0rc3/renku/core/plugin/pluginmanager.py` & `renku-2.6.0rc1/renku/core/plugin/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/plugin/provider.py` & `renku-2.6.0rc1/renku/core/plugin/provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/plugin/run.py` & `renku-2.6.0rc1/renku/core/plugin/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/plugin/session.py` & `renku-2.6.0rc1/renku/core/plugin/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/plugin/workflow.py` & `renku-2.6.0rc1/renku/core/plugin/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/plugin/workflow_file_parser.py` & `renku-2.6.0rc1/renku/core/plugin/workflow_file_parser.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/project.py` & `renku-2.6.0rc1/renku/core/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/session/__init__.py` & `renku-2.6.0rc1/renku/core/session/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/session/__pycache__/docker.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/session/__pycache__/docker.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 22065 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 3156 0000  a........w.d1V..
+00000000: 610d 0d0a 0000 0000 195e 9464 3156 0000  a........^.d1V..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/session/__pycache__/renkulab.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/session/__pycache__/renkulab.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 21512 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 0854 0000  a........w.d.T..
+00000000: 610d 0d0a 0000 0000 195e 9464 0854 0000  a........^.d.T..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6406 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/session/__pycache__/utils.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/session/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2206 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9e08 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 9e08 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 650b 6407 9c01 6408 6409 8404 5a0c  ..e.d...d.d...Z.
```

### Comparing `renku-2.5.0rc3/renku/core/session/docker.py` & `renku-2.6.0rc1/renku/core/session/docker.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/session/renkulab.py` & `renku-2.6.0rc1/renku/core/session/renkulab.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/session/session.py` & `renku-2.6.0rc1/renku/core/session/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/session/utils.py` & `renku-2.6.0rc1/renku/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/storage.py` & `renku-2.6.0rc1/renku/core/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/template/__init__.py` & `renku-2.6.0rc1/renku/core/template/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/template/template.py` & `renku-2.6.0rc1/renku/core/template/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/template/usecase.py` & `renku-2.6.0rc1/renku/core/template/usecase.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/__init__.py` & `renku-2.6.0rc1/renku/core/util/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/communication.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/communication.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 10282 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 2a28 0000  a........w.d*(..
+00000000: 610d 0d0a 0000 0000 195e 9464 2a28 0000  a........^.d*(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 5201 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 8302 5a08 6407 6408 8400 5a09  ..d...Z.d.d...Z.
 00000070: 6409 640a 8400 5a0a 4700 640b 640c 8400  d.d...Z.G.d.d...
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/contexts.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/contexts.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6617 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 d919 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 d919 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 5601 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6401 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/datetime8601.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/datetime8601.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2313 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 0909 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 0909 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a02 6d03 5a03 0100 6401 6404 6c04  m.Z.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6405 5a06 6501 a007 6506  m.Z...d.Z.e...e.
 00000060: a101 6a08 5a09 6406 6407 8400 5a0a 6408  ..j.Z.d.d...Z.d.
 00000070: 6409 8400 5a0b 6505 6502 1900 640a 9c01  d...Z.e.e...d...
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/doi.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/doi.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1376 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6005 0000  a........w.d`...
+00000000: 610d 0d0a 0000 0000 195e 9464 6005 0000  a........^.d`...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6501 6a03 6403 6501 6a04 6404 8d02  Z.e.j.d.e.j.d...
 00000050: 5a05 6405 6406 8400 5a06 6407 6408 8400  Z.d.d...Z.d.d...
 00000060: 5a07 6508 6409 9c01 640a 640b 8404 5a09  Z.e.d...d.d...Z.
 00000070: 6402 5300 290c 7a23 4865 6c70 6572 2075  d.S.).z#Helper u
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/git.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 40689 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 f19e 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 f19e 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 5c04 0000 5500  .....@...s\...U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6402 6c03 5a03 6401 6402  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 5a04 6401 6402 6c05 5a05 6401 6402  l.Z.d.d.l.Z.d.d.
 00000060: 6c06 5a06 6401 6402 6c07 5a07 6401 6402  l.Z.d.d.l.Z.d.d.
 00000070: 6c08 5a08 6401 6403 6c09 6d0a 5a0a 0100  l.Z.d.d.l.m.Z...
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/jwt.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/jwt.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1244 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 dc04 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 dc04 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 6d02 5a02  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c03 5a03 6504 6505 6404  ..d.d.l.Z.e.e.d.
 00000050: 9c02 6405 6406 8404 5a06 6403 5300 2907  ..d.d...Z.d.S.).
 00000060: 7a0e 4a57 5420 7574 696c 6974 6965 732e  z.JWT utilities.
 00000070: e900 0000 0029 02da 0864 6174 6574 696d  .....)...datetim
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/metadata.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/metadata.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 7036 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 7c1b 0000  a........w.d|...
+00000000: 610d 0d0a 0000 0000 195e 9464 7c1b 0000  a........^.d|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1e02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/os.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/os.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 12140 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6c2f 0000  a........w.dl/..
+00000000: 610d 0d0a 0000 0000 195e 9464 6c2f 0000  a........^.dl/..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0015 0000 0040 0000 0073 5a03 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6402 6c07 5a07 6401 6402 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 5a08 6401 6403 6c09 6d0a 5a0a 0100 6401  Z.d.d.l.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/requests.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/requests.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 7626 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 ca1d 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 ca1d 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5801 0000 6400  .....@...sX...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6402 6c0a 5a0a 6401 6402 6c0b 5a0b 6401  d.l.Z.d.d.l.Z.d.
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/ssh.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/ssh.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6871 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 d71a 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 d71a 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6403 6c04 6d05 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 6d09 5a09  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 6d0b 5a0c 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0d 6d0e 5a0e 0100 6401 6407 6c0f  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/tabulate.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/tabulate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2158 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6e08 0000  a........w.dn...
+00000000: 610d 0d0a 0000 0000 195e 9464 6e08 0000  a........^.dn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 640c 6405 6406  d.l.m.Z...d.d.d.
 00000050: 8401 5a04 640d 6408 6409 8401 5a05 640a  ..Z.d.d.d...Z.d.
 00000060: 640b 8400 5a06 6404 5300 290e 7a1e 5072  d...Z.d.S.).z.Pr
 00000070: 696e 7420 6120 636f 6c6c 6563 7469 6f6e  int a collection
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/urls.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/urls.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6228 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 5418 0000  a........w.dT...
+00000000: 610d 0d0a 0000 0000 195e 9464 5418 0000  a........^.dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4601 0000 6400  .....@...sF...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6405 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/util.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/util.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3878 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 260f 0000  a........w.d&...
+00000000: 610d 0d0a 0000 0000 195e 9464 260f 0000  a........^.d&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 f200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 5a04 6401 6403 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6401 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 0100 6401 6402 6c0e 5a0e 6401  m.Z...d.d.l.Z.d.
```

### Comparing `renku-2.5.0rc3/renku/core/util/__pycache__/yaml.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/util/__pycache__/yaml.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2836 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 140b 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 140b 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 5a05 7a1c 6401 6405 6c05 6d06 5a07 0100  Z.z.d.d.l.m.Z...
 00000060: 6401 6406 6c05 6d08 5a09 0100 5700 6e22  d.d.l.m.Z...W.n"
 00000070: 0400 650a 7962 0100 0100 0100 6401 6407  ..e.yb......d.d.
```

### Comparing `renku-2.5.0rc3/renku/core/util/communication.py` & `renku-2.6.0rc1/renku/core/util/communication.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/contexts.py` & `renku-2.6.0rc1/renku/core/util/contexts.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/datetime8601.py` & `renku-2.6.0rc1/renku/core/util/datetime8601.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/doi.py` & `renku-2.6.0rc1/renku/core/util/doi.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/git.py` & `renku-2.6.0rc1/renku/core/util/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/jwt.py` & `renku-2.6.0rc1/renku/core/util/jwt.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/metadata.py` & `renku-2.6.0rc1/renku/core/util/metadata.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/os.py` & `renku-2.6.0rc1/renku/core/util/os.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/requests.py` & `renku-2.6.0rc1/renku/core/util/requests.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/shacl.py` & `renku-2.6.0rc1/renku/core/util/shacl.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/ssh.py` & `renku-2.6.0rc1/renku/core/util/ssh.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/tabulate.py` & `renku-2.6.0rc1/renku/core/util/tabulate.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/urls.py` & `renku-2.6.0rc1/renku/core/util/urls.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/util.py` & `renku-2.6.0rc1/renku/core/util/util.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/util/yaml.py` & `renku-2.6.0rc1/renku/core/util/yaml.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/__init__.py` & `renku-2.6.0rc1/renku/core/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/__pycache__/activity.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/__pycache__/activity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 22713 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 b958 0000  a........w.d.X..
+00000000: 610d 0d0a 0000 0000 195e 9464 b958 0000  a........^.d.X..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 4402 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/__pycache__/execute.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/__pycache__/execute.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 18756 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 4449 0000  a........w.dDI..
+00000000: 610d 0d0a 0000 0000 195e 9464 4449 0000  a........^.dDI..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 8402 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/__pycache__/plan.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/__pycache__/plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 34209 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 a185 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 a185 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0016 0000 0040 0000 0073 2406 0000 6400  .....@...s$...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d03 5a03 6d04 5a04  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c05 6d06 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/__pycache__/plan_factory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 33046 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 1681 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 1681 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ee01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/__pycache__/run.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 13562 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,630 +1,642 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 fa34 0000  a........w.d.4..
+00000000: 610d 0d0a 0000 0000 195e 9464 3038 0000  a........^.d08..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 e201 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 ee01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
-00000080: 6d0f 5a0f 6d10 5a10 0100 6401 6402 6c11  m.Z.m.Z...d.d.l.
-00000090: 5a11 6401 6407 6c12 6d13 5a13 0100 6401  Z.d.d.l.m.Z...d.
+00000070: 0100 6401 6407 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
+00000080: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
+00000090: 6d12 5a12 0100 6401 6402 6c13 5a13 6401  m.Z...d.d.l.Z.d.
 000000a0: 6408 6c14 6d15 5a15 0100 6401 6409 6c16  d.l.m.Z...d.d.l.
 000000b0: 6d17 5a17 0100 6401 640a 6c18 6d19 5a19  m.Z...d.d.l.m.Z.
 000000c0: 0100 6401 640b 6c1a 6d1b 5a1b 0100 6401  ..d.d.l.m.Z...d.
 000000d0: 640c 6c1c 6d1d 5a1d 0100 6401 640d 6c1e  d.l.m.Z...d.d.l.
 000000e0: 6d1f 5a1f 0100 6401 640e 6c20 6d21 5a21  m.Z...d.d.l m!Z!
-000000f0: 0100 6401 640f 6c22 6d23 5a23 6d24 5a24  ..d.d.l"m#Z#m$Z$
-00000100: 0100 6401 6410 6c25 6d26 5a26 0100 6401  ..d.d.l%m&Z&..d.
+000000f0: 0100 6401 640f 6c22 6d23 5a23 0100 6401  ..d.d.l"m#Z#..d.
+00000100: 6410 6c24 6d25 5a25 6d26 5a26 0100 6401  d.l$m%Z%m&Z&..d.
 00000110: 6411 6c27 6d28 5a28 0100 6401 6412 6c29  d.l'm(Z(..d.d.l)
-00000120: 6d2a 5a2a 6d2b 5a2b 0100 6401 6413 6c2c  m*Z*m+Z+..d.d.l,
+00000120: 6d2a 5a2a 0100 6401 6413 6c2b 6d2c 5a2c  m*Z*..d.d.l+m,Z,
 00000130: 6d2d 5a2d 0100 6401 6414 6c2e 6d2f 5a2f  m-Z-..d.d.l.m/Z/
-00000140: 6d30 5a30 6d31 5a31 0100 6401 6415 6c32  m0Z0m1Z1..d.d.l2
+00000140: 0100 6401 6415 6c30 6d31 5a31 6d32 5a32  ..d.d.l0m1Z1m2Z2
 00000150: 6d33 5a33 0100 6401 6416 6c34 6d35 5a35  m3Z3..d.d.l4m5Z5
 00000160: 0100 6401 6417 6c36 6d37 5a37 0100 6401  ..d.d.l6m7Z7..d.
-00000170: 6418 6c38 6d39 5a39 0100 4700 6419 641a  d.l8m9Z9..G.d.d.
-00000180: 8400 641a 650c 8303 5a3a 6513 653b 641b  ..d.e...Z:e.e;d.
-00000190: 641c 8d01 641d 8d01 642c 650d 650b 650f  d...d...d,e.e.e.
-000001a0: 6506 653c 6602 1900 1900 1900 653d 653a  e.e<f.......e=e:
-000001b0: 641f 9c03 6420 6421 8405 8301 5a3e 653c  d...d d!....Z>e<
-000001c0: 653c 6422 9c02 6423 6424 8404 5a3f 653c  e<d"..d#d$..Z?e<
-000001d0: 653c 6422 9c02 6425 6426 8404 5a40 6515  e<d"..d%d&..Z@e.
-000001e0: a041 6427 6428 a102 6513 653b 641b 641c  .Ad'd(..e.e;d.d.
-000001f0: 8d01 641d 8d01 651f 6521 6517 6429 9c03  ..d...e.e!e.d)..
-00000200: 642a 642b 8404 8301 8301 5a42 6402 5300  d*d+......ZBd.S.
-00000210: 292d 7a18 5275 6e6e 696e 6720 776f 726b  )-z.Running work
-00000220: 666c 6f77 7320 6c6f 6769 632e e900 0000  flows logic.....
-00000230: 004e 2901 da0b 6465 6661 756c 7464 6963  .N)...defaultdic
-00000240: 7429 01da 0450 6174 6829 01da 0463 616c  t)...Path)...cal
-00000250: 6c29 07da 0444 6963 74da 044c 6973 74da  l)...Dict..List.
-00000260: 0a4e 616d 6564 5475 706c 65da 084f 7074  .NamedTuple..Opt
-00000270: 696f 6e61 6cda 0353 6574 da05 556e 696f  ional..Set..Unio
-00000280: 6eda 0463 6173 7429 01da 1276 616c 6964  n..cast)...valid
-00000290: 6174 655f 6172 6775 6d65 6e74 7329 01da  ate_arguments)..
-000002a0: 0669 6e6a 6563 7429 01da 0d50 6c61 6e56  .inject)...PlanV
-000002b0: 6965 774d 6f64 656c 2901 da06 6572 726f  iewModel)...erro
-000002c0: 7273 2901 da09 6765 745f 7661 6c75 6529  rs)...get_value)
-000002d0: 01da 1667 6574 5f6d 6170 7065 645f 7374  ...get_mapped_st
-000002e0: 645f 7374 7265 616d 7329 01da 1049 4163  d_streams)...IAc
-000002f0: 7469 7669 7479 4761 7465 7761 7929 01da  tivityGateway)..
-00000300: 0c49 506c 616e 4761 7465 7761 7929 02da  .IPlanGateway)..
-00000310: 1663 6865 636b 5f65 7874 6572 6e61 6c5f  .check_external_
-00000320: 7374 6f72 6167 65da 1770 756c 6c5f 7061  storage..pull_pa
-00000330: 7468 735f 6672 6f6d 5f73 746f 7261 6765  ths_from_storage
-00000340: 2901 da09 6c6f 6361 6c5f 6e6f 7729 01da  )...local_now)..
-00000350: 0c67 6574 5f67 6974 5f75 7365 7229 02da  .get_git_user)..
-00000360: 1867 6574 5f72 656c 6174 6976 655f 7061  .get_relative_pa
-00000370: 7468 5f74 6f5f 6377 64da 1267 6574 5f72  th_to_cwd..get_r
-00000380: 656c 6174 6976 655f 7061 7468 73a9 01da  elative_paths...
-00000390: 0867 6574 5f73 6c75 6729 03da 3467 6574  .get_slug)..4get
-000003a0: 5f61 6c6c 5f6d 6f64 6966 6965 645f 616e  _all_modified_an
-000003b0: 645f 6465 6c65 7465 645f 6163 7469 7669  d_deleted_activi
-000003c0: 7469 6573 5f61 6e64 5f65 6e74 6974 6965  ties_and_entitie
-000003d0: 73da 2467 6574 5f64 6f77 6e73 7472 6561  s.$get_downstrea
-000003e0: 6d5f 6765 6e65 7261 7469 6e67 5f61 6374  m_generating_act
-000003f0: 6976 6974 6965 73da 1169 735f 6163 7469  ivities..is_acti
-00000400: 7669 7479 5f76 616c 6964 2901 da0b 506c  vity_valid)...Pl
-00000410: 616e 4661 6374 6f72 7929 01da 0f70 726f  anFactory)...pro
-00000420: 6a65 6374 5f63 6f6e 7465 7874 2901 da08  ject_context)...
-00000430: 4163 7469 7669 7479 2901 da06 5065 7273  Activity)...Pers
-00000440: 6f6e 6300 0000 0000 0000 0000 0000 0000  onc.............
-00000450: 0000 0004 0000 0040 0000 0073 6600 0000  .......@...sf...
-00000460: 6500 5a01 6400 5a02 5500 6401 5a03 6504  e.Z.d.Z.U.d.Z.e.
-00000470: 6505 6506 6505 1900 6602 1900 6507 6402  e.e.e...f...e.d.
-00000480: 3c00 6504 6505 6506 6505 1900 6602 1900  <.e.e.e.e...f...
-00000490: 6507 6403 3c00 6506 6505 1900 6507 6404  e.d.<.e.e...e.d.
-000004a0: 3c00 6506 6505 1900 6507 6405 3c00 6504  <.e.e...e.d.<.e.
-000004b0: 6505 6506 6505 1900 6602 1900 6507 6406  e.e.e...f...e.d.
-000004c0: 3c00 6407 5300 2908 da0c 5374 6174 7573  <.d.S.)...Status
-000004d0: 5265 7375 6c74 6134 0100 0052 6570 7265  Resulta4...Repre
-000004e0: 7365 6e74 2073 7461 7475 7320 6f66 2061  sent status of a
-000004f0: 2070 726f 6a65 6374 2e0a 0a20 2020 2041   project...    A
-00000500: 2071 7569 6e74 7570 6c65 2063 6f6e 7461   quintuple conta
-00000510: 696e 696e 6720 6120 6d61 7070 696e 6720  ining a mapping 
-00000520: 6f66 2073 7461 6c65 206f 7574 7075 7473  of stale outputs
-00000530: 2074 6f20 6d6f 6469 6669 6564 2075 7361   to modified usa
-00000540: 6765 732c 2061 206d 6170 7069 6e67 206f  ges, a mapping o
-00000550: 6620 7374 616c 6520 6163 7469 7669 7469  f stale activiti
-00000560: 6573 2074 6861 7420 6861 7665 206e 6f0a  es that have no.
-00000570: 2020 2020 6765 6e65 7261 7469 6f6e 2074      generation t
-00000580: 6f20 6d6f 6469 6669 6564 2075 7361 6765  o modified usage
-00000590: 732c 2061 2073 6574 206f 6620 6d6f 6469  s, a set of modi
-000005a0: 6669 6564 2075 7361 6765 732c 2061 2073  fied usages, a s
-000005b0: 6574 206f 6620 6465 6c65 7465 6420 7573  et of deleted us
-000005c0: 6167 6573 2c20 616e 6420 6120 6d61 7020  ages, and a map 
-000005d0: 6f66 206d 6f64 6966 6965 6420 6869 6464  of modified hidd
-000005e0: 656e 0a20 2020 2069 6e70 7574 7320 746f  en.    inputs to
-000005f0: 2070 6174 6873 2074 6861 7420 7468 6579   paths that they
-00000600: 2067 656e 6572 6174 652e 0a20 2020 20da   generate..    .
-00000610: 106f 7574 6461 7465 645f 6f75 7470 7574  .outdated_output
-00000620: 73da 136f 7574 6461 7465 645f 6163 7469  s..outdated_acti
-00000630: 7669 7469 6573 da0f 6d6f 6469 6669 6564  vities..modified
-00000640: 5f69 6e70 7574 73da 0e64 656c 6574 6564  _inputs..deleted
-00000650: 5f69 6e70 7574 73da 166d 6f64 6966 6965  _inputs..modifie
-00000660: 645f 6869 6464 656e 5f69 6e70 7574 734e  d_hidden_inputsN
-00000670: 2908 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000680: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000690: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
-000006a0: 0500 0000 da03 7374 7272 0900 0000 da0f  ......strr......
-000006b0: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fa9  __annotations__.
-000006c0: 0072 2f00 0000 722f 0000 00fa 462f 686f  .r/...r/....F/ho
-000006d0: 6d65 2f72 756e 6e65 722f 776f 726b 2f72  me/runner/work/r
-000006e0: 656e 6b75 2d70 7974 686f 6e2f 7265 6e6b  enku-python/renk
-000006f0: 752d 7079 7468 6f6e 2f72 656e 6b75 2f63  u-python/renku/c
-00000700: 6f72 652f 776f 726b 666c 6f77 2f72 756e  ore/workflow/run
-00000710: 2e70 7972 2300 0000 3400 0000 730c 0000  .pyr#...4...s...
-00000720: 000a 0104 0714 0114 010c 010c 0172 2300  .............r#.
-00000730: 0000 5429 01da 1761 7262 6974 7261 7279  ..T)...arbitrary
-00000740: 5f74 7970 6573 5f61 6c6c 6f77 6564 2901  _types_allowed).
-00000750: da06 636f 6e66 6967 4629 03da 0570 6174  ..configF)...pat
-00000760: 6873 da0e 6967 6e6f 7265 5f64 656c 6574  hs..ignore_delet
-00000770: 6564 da06 7265 7475 726e 6302 0000 0000  ed..returnc.....
-00000780: 0000 0000 0000 0012 0000 0007 0000 0003  ................
-00000790: 0000 0073 d201 0000 6401 6402 8400 7d02  ...s....d.d...}.
-000007a0: 8700 6601 6403 6404 8408 7d03 7c01 7020  ..f.d.d...}.|.p 
-000007b0: 7400 6405 6406 8302 7d01 7401 7402 6a03  t.d.d...}.t.t.j.
-000007c0: 6407 6408 8d02 5c03 7d04 7d05 7d06 6409  d.d...\.}.}.}.d.
-000007d0: 640a 8400 7c04 4400 8301 7d04 640b 640a  d...|.D...}.d.d.
-000007e0: 8400 7c05 4400 8301 7d05 640c 640a 8400  ..|.D...}.d.d...
-000007f0: 7c06 4400 8301 7d06 7c04 7380 7c05 7380  |.D...}.|.s.|.s.
-00000800: 7c06 7380 7404 6900 6900 7405 8300 7405  |.s.t.i.i.t...t.
-00000810: 8300 6900 8305 5300 8800 7086 6700 8900  ..i...S...p.g...
-00000820: 7406 7402 6a07 640d 640e 8400 8800 4400  t.t.j.d.d.....D.
-00000830: 8301 640f 8d02 8900 7405 8300 7d07 7408  ..d.....t...}.t.
-00000840: 7405 8301 7d08 7408 7405 8301 7d09 7408  t...}.t.t...}.t.
-00000850: 7405 8301 7d0a 7c04 4400 5d7e 5c02 7d0b  t...}.|.D.]~\.}.
-00000860: 7d0c 7c03 7c0b 7c0c 7c01 6410 8d03 7d0d  }.|.|.|.|.d...}.
-00000870: 7c0d 72c2 7409 7402 6a07 7c0c 6a07 1b00  |.r.t.t.j.|.j...
-00000880: 8301 7d0e 7c07 a00a 7c0e a101 0100 7c0d  ..}.|...|.....|.
-00000890: 4400 5d44 7d0f 740b 7c0f 6a0c 8301 6411  D.]D}.t.|.j...d.
-000008a0: 6b02 9001 7220 7c09 7c0f 6a0d 1900 a00a  k...r |.|.j.....
-000008b0: 7c0e a101 0100 71fa 7c02 7c0f 8301 4400  |.....q.|.|...D.
-000008c0: 5d14 7d10 7c08 7c10 1900 a00a 7c0e a101  ].}.|.|.....|...
-000008d0: 0100 9001 7128 71fa 71c2 6412 640a 8400  ....q(q.q.d.d...
-000008e0: 7c05 4400 8301 7d11 8700 6601 6413 640a  |.D...}...f.d.d.
-000008f0: 8408 7c11 4400 8301 7d11 7c06 4400 5d58  ..|.D...}.|.D.]X
-00000900: 5c02 7d0b 7d0c 7c03 7c0b 7c0c 6407 6410  \.}.}.|.|.|.d.d.
-00000910: 8d03 7d0d 7c0d 9001 7266 7409 7402 6a07  ..}.|...rft.t.j.
-00000920: 7c0c 6a07 1b00 8301 7d0e 7c0d 4400 5d24  |.j.....}.|.D.]$
-00000930: 7d0f 7c02 7c0f 8301 4400 5d14 7d10 7c0a  }.|.|...D.].}.|.
-00000940: 7c0e 1900 a00a 7c10 a101 0100 9001 71a2  |.....|.......q.
-00000950: 9001 7196 9001 7166 7404 7c08 7c09 7c07  ..q...qft.|.|.|.
-00000960: 7c11 7c0a 6414 8d05 5300 2915 6134 0100  |.|.d...S.).a4..
-00000970: 0052 6574 7572 6e20 7374 6174 7573 206f  .Return status o
-00000980: 6620 6120 7072 6f6a 6563 742e 0a0a 2020  f a project...  
-00000990: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000009a0: 7061 7468 7328 4f70 7469 6f6e 616c 5b4c  paths(Optional[L
-000009b0: 6973 745b 556e 696f 6e5b 5061 7468 2c20  ist[Union[Path, 
-000009c0: 7374 725d 5d5d 293a 204c 696d 6974 2074  str]]]): Limit t
-000009d0: 6865 2073 7461 7475 7320 746f 2074 6869  he status to thi
-000009e0: 7320 6c69 7374 206f 6620 7061 7468 7320  s list of paths 
-000009f0: 2844 6566 6175 6c74 2076 616c 7565 203d  (Default value =
-00000a00: 204e 6f6e 6529 2e0a 2020 2020 2020 2020   None)..        
-00000a10: 6967 6e6f 7265 5f64 656c 6574 6564 2862  ignore_deleted(b
-00000a20: 6f6f 6c29 3a20 5768 6574 6865 7220 746f  ool): Whether to
-00000a30: 2069 676e 6f72 6520 6465 6c65 7465 6420   ignore deleted 
-00000a40: 6765 6e65 7261 7469 6f6e 7320 2844 6566  generations (Def
-00000a50: 6175 6c74 2076 616c 7565 203d 2046 616c  ault value = Fal
-00000a60: 7365 292e 0a0a 2020 2020 5265 7475 726e  se)...    Return
-00000a70: 733a 0a20 2020 2020 2020 2053 7461 7475  s:.        Statu
-00000a80: 7352 6573 756c 743a 2053 7461 7475 7320  sResult: Status 
-00000a90: 6f66 2074 6865 2070 726f 6a65 6374 2e0a  of the project..
-00000aa0: 0a20 2020 2063 0100 0000 0000 0000 0000  .    c..........
-00000ab0: 0000 0100 0000 0200 0000 5300 0000 7310  ..........S...s.
-00000ac0: 0000 0064 0164 0284 007c 006a 0044 0083  ...d.d...|.j.D..
-00000ad0: 0153 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
-00000ae0: 0000 0002 0000 0004 0000 0073 0000 0073  ...........s...s
-00000af0: 2000 0000 7c00 5d18 7d01 7400 7401 6a02   ...|.].}.t.t.j.
-00000b00: 7c01 6a03 6a02 1b00 8301 5600 0100 7102  |.j.j.....V...q.
-00000b10: 6400 5300 a901 4e29 0472 1800 0000 7220  d.S...N).r....r 
-00000b20: 0000 00da 0470 6174 68da 0665 6e74 6974  .....path..entit
-00000b30: 7929 02da 022e 30da 0a67 656e 6572 6174  y)....0..generat
-00000b40: 696f 6e72 2f00 0000 722f 0000 0072 3000  ionr/...r/...r0.
-00000b50: 0000 da09 3c67 656e 6578 7072 3e51 0000  ....<genexpr>Q..
-00000b60: 0073 0400 0000 0402 02ff 7a3a 6765 745f  .s........z:get_
-00000b70: 7374 6174 7573 2e3c 6c6f 6361 6c73 3e2e  status.<locals>.
-00000b80: 6765 745f 616c 6c5f 6765 6e65 7261 7469  get_all_generati
-00000b90: 6f6e 732e 3c6c 6f63 616c 733e 2e3c 6765  ons.<locals>.<ge
-00000ba0: 6e65 7870 723e 2901 da0b 6765 6e65 7261  nexpr>)...genera
-00000bb0: 7469 6f6e 7329 01da 0861 6374 6976 6974  tions)...activit
-00000bc0: 7972 2f00 0000 722f 0000 0072 3000 0000  yr/...r/...r0...
-00000bd0: da13 6765 745f 616c 6c5f 6765 6e65 7261  ..get_all_genera
-00000be0: 7469 6f6e 7350 0000 0073 0600 0000 0001  tionsP...s......
-00000bf0: 0602 04fe 7a27 6765 745f 7374 6174 7573  ....z'get_status
-00000c00: 2e3c 6c6f 6361 6c73 3e2e 6765 745f 616c  .<locals>.get_al
-00000c10: 6c5f 6765 6e65 7261 7469 6f6e 7363 0300  l_generationsc..
-00000c20: 0000 0000 0000 0000 0000 0400 0000 0600  ................
-00000c30: 0000 1300 0000 732a 0000 0088 0072 0e7c  ......s*.....r.|
-00000c40: 016a 0088 0076 0072 1267 006e 0288 007d  .j...v.r.g.n...}
-00000c50: 0374 017c 0068 017c 037c 0274 026a 0064  .t.|.h.|.|.t.j.d
-00000c60: 018d 0453 0029 024e 2904 5a13 7374 6172  ...S.).N).Z.star
-00000c70: 7469 6e67 5f61 6374 6976 6974 6965 7372  ting_activitiesr
-00000c80: 3300 0000 7234 0000 00da 0c70 726f 6a65  3...r4.....proje
-00000c90: 6374 5f70 6174 6829 0372 3700 0000 721d  ct_path).r7...r.
-00000ca0: 0000 0072 2000 0000 2904 da0e 7374 6172  ...r ...)...star
-00000cb0: 745f 6163 7469 7669 7479 7238 0000 0072  t_activityr8...r
-00000cc0: 3400 0000 da10 6765 6e65 7261 7469 6f6e  4.....generation
-00000cd0: 5f70 6174 6873 a901 7233 0000 0072 2f00  _paths..r3...r/.
-00000ce0: 0000 7230 0000 00da 1967 6574 5f64 6f77  ..r0.....get_dow
-00000cf0: 6e73 7472 6561 6d5f 6163 7469 7669 7469  nstream_activiti
-00000d00: 6573 5600 0000 730e 0000 0000 0316 0202  esV...s.........
-00000d10: 0104 0102 0102 0104 fc7a 2d67 6574 5f73  .........z-get_s
-00000d20: 7461 7475 732e 3c6c 6f63 616c 733e 2e67  tatus.<locals>.g
-00000d30: 6574 5f64 6f77 6e73 7472 6561 6d5f 6163  et_downstream_ac
-00000d40: 7469 7669 7469 6573 da05 7265 6e6b 755a  tivities..renkuZ
-00000d50: 1475 7064 6174 655f 6967 6e6f 7265 5f64  .update_ignore_d
-00000d60: 656c 6574 6554 2902 da0a 7265 706f 7369  eleteT)...reposi
-00000d70: 746f 7279 5a19 6368 6563 6b5f 6869 6464  toryZ.check_hidd
-00000d80: 656e 5f64 6570 656e 6465 6e63 6965 7363  en_dependenciesc
-00000d90: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000da0: 0400 0000 5300 0000 7320 0000 0068 007c  ....S...s ...h.|
-00000db0: 005d 185c 027d 017d 0274 007c 0183 0172  .].\.}.}.t.|...r
-00000dc0: 047c 017c 0266 0292 0271 0453 0072 2f00  .|.|.f...q.S.r/.
-00000dd0: 0000 a901 721e 0000 00a9 0372 3900 0000  ....r......r9...
-00000de0: da01 61da 0165 722f 0000 0072 2f00 0000  ..a..er/...r/...
-00000df0: 7230 0000 00da 093c 7365 7463 6f6d 703e  r0.....<setcomp>
-00000e00: 6800 0000 f300 0000 007a 1d67 6574 5f73  h........z.get_s
-00000e10: 7461 7475 732e 3c6c 6f63 616c 733e 2e3c  tatus.<locals>.<
-00000e20: 7365 7463 6f6d 703e 6301 0000 0000 0000  setcomp>c.......
-00000e30: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
-00000e40: 0073 2000 0000 6800 7c00 5d18 5c02 7d01  .s ...h.|.].\.}.
-00000e50: 7d02 7400 7c01 8301 7204 7c01 7c02 6602  }.t.|...r.|.|.f.
-00000e60: 9202 7104 5300 722f 0000 0072 4600 0000  ..q.S.r/...rF...
-00000e70: 7247 0000 0072 2f00 0000 722f 0000 0072  rG...r/...r/...r
-00000e80: 3000 0000 724a 0000 0069 0000 0072 4b00  0...rJ...i...rK.
-00000e90: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
-00000ea0: 0000 0004 0000 0053 0000 0073 2000 0000  .......S...s ...
-00000eb0: 6800 7c00 5d18 5c02 7d01 7d02 7400 7c01  h.|.].\.}.}.t.|.
-00000ec0: 8301 7204 7c01 7c02 6602 9202 7104 5300  ..r.|.|.f...q.S.
-00000ed0: 722f 0000 0072 4600 0000 7247 0000 0072  r/...rF...rG...r
-00000ee0: 2f00 0000 722f 0000 0072 3000 0000 724a  /...r/...r0...rJ
-00000ef0: 0000 006a 0000 0072 4b00 0000 6301 0000  ...j...rK...c...
-00000f00: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000f10: 0053 0000 0073 1800 0000 6700 7c00 5d10  .S...s....g.|.].
-00000f20: 7d01 7400 a001 a100 7c01 1b00 9102 7104  }.t.....|.....q.
-00000f30: 5300 722f 0000 0029 0272 0300 0000 da03  S.r/...).r......
-00000f40: 6377 6429 0272 3900 0000 da01 7072 2f00  cwd).r9.....pr/.
-00000f50: 0000 722f 0000 0072 3000 0000 da0a 3c6c  ..r/...r0.....<l
-00000f60: 6973 7463 6f6d 703e 7000 0000 724b 0000  istcomp>p...rK..
-00000f70: 007a 1e67 6574 5f73 7461 7475 732e 3c6c  .z.get_status.<l
-00000f80: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000f90: 3e29 02da 0462 6173 6572 3300 0000 2903  >)...baser3...).
-00000fa0: 7240 0000 0072 3800 0000 7234 0000 0072  r@...r8...r4...r
-00000fb0: 0100 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00000fc0: 0003 0000 0004 0000 0053 0000 0073 1600  .........S...s..
-00000fd0: 0000 6800 7c00 5d0e 5c02 7d01 7d02 7c02  ..h.|.].\.}.}.|.
-00000fe0: 6a00 9202 7104 5300 722f 0000 0029 0172  j...q.S.r/...).r
-00000ff0: 3700 0000 2903 7239 0000 00da 015f 7249  7...).r9....._rI
-00001000: 0000 0072 2f00 0000 722f 0000 0072 3000  ...r/...r/...r0.
-00001010: 0000 724a 0000 0086 0000 0072 4b00 0000  ..rJ.......rK...
-00001020: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001030: 0005 0000 0013 0000 0073 2600 0000 6800  .........s&...h.
-00001040: 7c00 5d1e 7d01 8800 7214 7c01 8800 7600  |.].}...r.|...v.
-00001050: 7204 7400 7401 6a02 7c01 1b00 8301 9202  r.t.t.j.|.......
-00001060: 7104 5300 722f 0000 0029 0372 1800 0000  q.S.r/...).r....
-00001070: 7220 0000 0072 3700 0000 2902 7239 0000  r ...r7...).r9..
-00001080: 00da 0164 7242 0000 0072 2f00 0000 7230  ...drB...r/...r0
-00001090: 0000 0072 4a00 0000 8700 0000 7302 0000  ...rJ.......s...
-000010a0: 0006 0129 0572 2400 0000 7225 0000 0072  ...).r$...r%...r
-000010b0: 2600 0000 7227 0000 0072 2800 0000 290e  &...r'...r(...).
-000010c0: 7210 0000 0072 1c00 0000 7220 0000 0072  r....r....r ...r
-000010d0: 4500 0000 7223 0000 00da 0373 6574 7219  E...r#.....setr.
-000010e0: 0000 0072 3700 0000 7202 0000 0072 1800  ...r7...r....r..
-000010f0: 0000 da03 6164 64da 036c 656e 723c 0000  ....add..lenr<..
-00001100: 00da 0269 6429 1272 3300 0000 7234 0000  ...id).r3...r4..
-00001110: 0072 3e00 0000 7243 0000 00da 086d 6f64  .r>...rC.....mod
-00001120: 6966 6965 64da 0764 656c 6574 6564 5a0f  ified..deletedZ.
-00001130: 6869 6464 656e 5f6d 6f64 6966 6965 6472  hidden_modifiedr
-00001140: 2600 0000 5a0d 7374 616c 655f 6f75 7470  &...Z.stale_outp
-00001150: 7574 735a 1073 7461 6c65 5f61 6374 6976  utsZ.stale_activ
-00001160: 6974 6965 7372 2800 0000 7240 0000 0072  itiesr(...r@...r
-00001170: 3800 0000 da0a 6163 7469 7669 7469 6573  8.....activities
-00001180: 5a0a 7573 6167 655f 7061 7468 723d 0000  Z.usage_pathr=..
-00001190: 005a 0f67 656e 6572 6174 696f 6e5f 7061  .Z.generation_pa
-000011a0: 7468 da0d 6465 6c65 7465 645f 7061 7468  th..deleted_path
-000011b0: 7372 2f00 0000 7242 0000 0072 3000 0000  sr/...rB...r0...
-000011c0: da0a 6765 745f 7374 6174 7573 4300 0000  ..get_statusC...
-000011d0: 735e 0000 0000 0d08 060c 0c0e 0202 0106  s^..............
-000011e0: ff0c 040e 010e 010e 020c 0114 0208 0118  ................
-000011f0: 0206 0108 0108 0108 020c 0102 0106 ff06  ................
-00001200: 0304 0110 010a 0208 0110 0112 020c 0116  ................
-00001210: 020e 010a 0102 ff06 040c 010e 0106 0110  ................
-00001220: 0108 010c 011a 0202 0102 0102 0102 0102  ................
-00001230: 0102 fb72 5a00 0000 2902 da04 6e61 6d65  ...rZ...)...name
-00001240: 7235 0000 0063 0100 0000 0000 0000 0000  r5...c..........
-00001250: 0000 0100 0000 0500 0000 4300 0000 7310  ..........C...s.
-00001260: 0000 0074 007c 0064 0167 0164 0264 038d  ...t.|.d.g.d.d..
-00001270: 0353 0029 047a 3252 6574 7572 6e20 6120  .S.).z2Return a 
-00001280: 7661 6c69 6420 706c 616e 206e 616d 6520  valid plan name 
-00001290: 6261 7365 6420 6f6e 2074 6865 2070 6173  based on the pas
-000012a0: 7365 6420 6e61 6d65 2eda 012e 4629 02da  sed name....F)..
-000012b0: 0d69 6e76 616c 6964 5f63 6861 7273 da09  .invalid_chars..
-000012c0: 6c6f 7765 7263 6173 6572 1a00 0000 a901  lowercaser......
-000012d0: 725b 0000 0072 2f00 0000 722f 0000 0072  r[...r/...r/...r
-000012e0: 3000 0000 da13 6765 745f 7661 6c69 645f  0.....get_valid_
-000012f0: 706c 616e 5f6e 616d 659c 0000 0073 0200  plan_name....s..
-00001300: 0000 0002 7260 0000 0063 0100 0000 0000  ....r`...c......
-00001310: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00001320: 0000 7308 0000 0074 007c 0083 0153 0029  ..s....t.|...S.)
-00001330: 017a 3752 6574 7572 6e20 6120 7661 6c69  .z7Return a vali
-00001340: 6420 7061 7261 6d65 7465 7220 6e61 6d65  d parameter name
-00001350: 2062 6173 6564 206f 6e20 7468 6520 7061   based on the pa
-00001360: 7373 6564 206e 616d 652e 2901 7260 0000  ssed name.).r`..
-00001370: 0072 5f00 0000 722f 0000 0072 2f00 0000  .r_...r/...r/...
-00001380: 7230 0000 00da 1867 6574 5f76 616c 6964  r0.....get_valid
-00001390: 5f70 6172 616d 6574 6572 5f6e 616d 65a1  _parameter_name.
-000013a0: 0000 0073 0200 0000 0002 7261 0000 00da  ...s......ra....
-000013b0: 1061 6374 6976 6974 795f 6761 7465 7761  .activity_gatewa
-000013c0: 79da 0c70 6c61 6e5f 6761 7465 7761 7929  y..plan_gateway)
-000013d0: 0372 6200 0000 7263 0000 0072 3500 0000  .rb...rc...r5...
-000013e0: 630e 0000 0000 0000 0000 0000 0025 0000  c............%..
-000013f0: 000c 0000 0003 0000 0073 3604 0000 7c00  .........s6...|.
-00001400: 724e 7400 7c00 8301 7d0e 7c00 7c0e 6b03  rNt.|...}.|.|.k.
-00001410: 722c 7401 a002 6401 7c00 9b00 6402 7c0e  r,t...d.|...d.|.
-00001420: 9b00 6403 9d05 a101 8201 7c0d a003 a100  ..d.......|.....
-00001430: 7d0f 7c00 7c0f 7600 724e 7401 a004 6404  }.|.|.v.rNt...d.
-00001440: 7c00 9b00 6405 9d03 a101 8201 7c08 7256  |...d.......|.rV
-00001450: 7c04 6e06 7405 6a06 6a07 7d10 7408 7c10  |.n.t.j.j.}.t.|.
-00001460: 6406 6407 8d02 7d11 7c07 7272 7c03 6e06  d.d...}.|.rr|.n.
-00001470: 7405 6a06 6a07 7d10 7408 7c10 6408 6407  t.j.j.}.t.|.d.d.
-00001480: 8d02 7d12 7c11 a009 7c12 a101 0100 7408  ..}.|...|.....t.
-00001490: 7c03 6406 6407 8d02 7d13 7c13 72c6 7401  |.d.d...}.|.r.t.
-000014a0: a00a 6409 740b 6a0c 640a a00d 7c13 a00e  ..d.t.j.d...|...
-000014b0: a100 a101 640b 640c 8d02 1700 640d 1700  ....d.d.....d...
-000014c0: a101 8201 7408 7c04 6408 6407 8d02 7d13  ....t.|.d.d...}.
-000014d0: 7c13 72fc 7401 a00a 640e 740b 6a0c 640a  |.r.t...d.t.j.d.
-000014e0: a00d 7c13 a00e a100 a101 640b 640c 8d02  ..|.......d.d...
-000014f0: 1700 640d 1700 a101 8201 640f 7d14 640f  ..d.......d.}.d.
-00001500: 7d15 7a34 740f 6410 6411 8302 8f14 0100  }.z4t.d.d.......
-00001510: 6412 7d16 5700 640f 0400 0400 8303 0100  d.}.W.d.........
-00001520: 6e12 3100 9001 732c 3000 0100 0100 0100  n.1...s,0.......
-00001530: 5900 0100 5700 6e18 0400 7410 9001 7950  Y...W.n...t...yP
-00001540: 0100 0100 0100 6413 7d16 5900 6e02 3000  ......d.}.Y.n.0.
-00001550: 9002 7aa2 6414 7c11 7600 7d17 6415 7c11  ..z.d.|.v.}.d.|.
-00001560: 7600 7d18 7c16 9001 72a4 7c17 9001 7288  v.}.|...r.|...r.
-00001570: 740f 6410 6411 8302 7d14 7411 6a12 7d19  t.d.d...}.t.j.}.
-00001580: 7c14 7411 5f12 7c18 9001 72a4 740f 6410  |.t._.|...r.t.d.
-00001590: 6411 8302 7d15 7411 6a13 7d1a 7c15 7411  d...}.t.j.}.|.t.
-000015a0: 5f13 7414 7405 6a15 8301 8900 6416 6417  _.t.t.j.....d.d.
-000015b0: 8400 7d1b 7c1b 7c03 6418 8302 7d03 7c1b  ..}.|.|.d...}.|.
-000015c0: 7c04 6419 8302 7d04 7c1b 7c05 641a 8302  |.d...}.|.|.d...
-000015d0: 7d05 7416 6600 7c0a 7c03 7c04 7c05 7417  }.t.f.|.|.|.|.t.
-000015e0: a018 a100 8800 7c07 7c08 7c09 641b 9c09  ......|.|.|.d...
-000015f0: 8700 6601 641c 641d 8408 7c11 a019 a100  ..f.d.d...|.....
-00001600: 4400 8301 a401 8e01 7d1c 7c1c 6a1a 7c06  D.......}.|.j.|.
-00001610: 641e 8d01 9001 8f1c 7d1d 741b 8300 9002  d.......}.t.....
-00001620: 724c 641f 6420 8400 7c1d a01c 7405 6a15  rLd.d ..|...t.j.
-00001630: a101 4400 8301 7d1e 741d 7405 6a06 6701  ..D...}.t.t.j.g.
-00001640: 7c1e a201 5200 8e00 0100 7c16 9002 726a  |...R.....|...rj
-00001650: 7c17 9002 725e 7c19 7411 5f12 7c18 9002  |...r^|.t._.|...
-00001660: 726a 7c1a 7411 5f13 741e 8300 7d1f 7a2c  rj|.t._.t...}.z,
-00001670: 741f 7c1c 6a20 6601 6421 7417 a018 a100  t.|.j f.d!t.....
-00001680: 6901 6422 641d 8400 7c11 a021 a100 4400  i.d"d...|..!..D.
-00001690: 8301 a401 8e01 7d20 5700 6e32 0400 7422  ......} W.n2..t"
-000016a0: 9002 79ce 0100 0100 0100 6423 a00d 7c1c  ..y.......d#..|.
-000016b0: 6a23 a101 7d21 7401 a002 6424 7c21 9b00  j#..}!t...d$|!..
-000016c0: 6425 9d03 a101 8201 5900 6e02 3000 741e  d%......Y.n.0.t.
-000016d0: 8300 7d22 7411 6a12 a024 a100 0100 7411  ..}"t.j..$....t.
-000016e0: 6a13 a024 a100 0100 7c16 9003 7208 7c17  j..$....|...r.|.
-000016f0: 9002 72fc 7c14 7411 5f12 7c18 9003 7208  ..r.|.t._.|...r.
-00001700: 7c15 7411 5f13 7c20 7c09 9003 7014 6426  |.t._.| |...p.d&
-00001710: 6801 7601 9003 7228 7401 6a25 7c20 7c09  h.v...r(t.j%| |.
-00001720: 6427 8d02 8201 5700 640f 0400 0400 8303  d'....W.d.......
-00001730: 0100 6e12 3100 9003 733e 3000 0100 0100  ..n.1...s>0.....
-00001740: 0100 5900 0100 7c0b 9003 7360 7426 7427  ..Y...|...s`t&t'
-00001750: 7428 7405 6a06 8301 8302 6701 7d0b 7c1d  t(t.j.....g.}.|.
-00001760: 6a29 7c00 7c01 7c02 7c0b 7c1f 6428 8d05  j)|.|.|.|.|.d(..
-00001770: 7d23 742a 6a2b 7c23 7405 6a06 7c1f 7c22  }#t*j+|#t.j.|.|"
-00001780: 7c1d 6a2c 6429 8d05 7d24 7c0c a02d 7c24  |.j,d)..}$|..-|$
-00001790: a101 0100 742e a02b 7c23 a101 5700 7c14  ....t..+|#..W.|.
-000017a0: 9003 72bc 7c14 a024 a100 0100 7c19 7411  ..r.|..$....|.t.
-000017b0: 5f12 7c14 a02f a100 0100 7c15 9003 72d8  _.|../....|...r.
-000017c0: 7c15 a024 a100 0100 7c1a 7411 5f13 7c15  |..$....|.t._.|.
-000017d0: a02f a100 0100 5300 7c15 9004 7232 7c15  ./....S.|...r2|.
-000017e0: a024 a100 0100 7c1a 7411 5f13 7c15 a02f  .$....|.t._.|../
-000017f0: a100 0100 6e3a 7c14 9004 7214 7c14 a024  ....n:|...r.|..$
-00001800: a100 0100 7c19 7411 5f12 7c14 a02f a100  ....|.t._.|../..
-00001810: 0100 7c15 9004 7230 7c15 a024 a100 0100  ..|...r0|..$....
-00001820: 7c1a 7411 5f13 7c15 a02f a100 0100 3000  |.t._.|../....0.
-00001830: 640f 5300 292a 7a1b 5275 6e20 636f 6d6d  d.S.)*z.Run comm
-00001840: 616e 6420 6c69 6e65 2061 7267 756d 656e  and line argumen
-00001850: 7473 2e7a 0f49 6e76 616c 6964 206e 616d  ts.z.Invalid nam
-00001860: 653a 2027 7a0a 2720 2848 696e 743a 2027  e: 'z.' (Hint: '
-00001870: 7a0c 2720 6973 2076 616c 6964 292e 7a23  z.' is valid).z#
-00001880: 4475 706c 6963 6174 6520 776f 726b 666c  Duplicate workfl
-00001890: 6f77 206e 616d 653a 2057 6f72 6b66 6c6f  ow name: Workflo
-000018a0: 7720 277a 1127 2061 6c72 6561 6479 2065  w 'z.' already e
-000018b0: 7869 7374 732e 2902 da06 7374 646f 7574  xists.)...stdout
-000018c0: da06 7374 6465 7272 2901 da07 7374 7265  ..stderr)...stre
-000018d0: 616d 7329 01da 0573 7464 696e 7a36 4578  ams)...stdinz6Ex
-000018e0: 706c 6963 6974 2069 6e70 7574 2066 696c  plicit input fil
-000018f0: 6520 6361 6e6e 6f74 2062 6520 7573 6564  e cannot be used
-00001900: 2061 7320 7374 646f 7574 2f73 7464 6572   as stdout/stder
-00001910: 723a 0a09 7a02 0a09 da06 7965 6c6c 6f77  r:..z.....yellow
-00001920: 2901 da02 6667 da01 0a7a 2f45 7870 6c69  )...fg...z/Expli
-00001930: 6369 7420 6f75 7470 7574 2066 696c 6520  cit output file 
-00001940: 6361 6e6e 6f74 2062 6520 7573 6564 2061  cannot be used a
-00001950: 7320 7374 6469 6e3a 0a09 4e7a 082f 6465  s stdin:..Nz./de
-00001960: 762f 7474 79da 0177 5446 7264 0000 0072  v/tty..wTFrd...r
-00001970: 6500 0000 6302 0000 0000 0000 0000 0000  e...c...........
-00001980: 0005 0000 0005 0000 0053 0000 0073 8400  .........S...s..
-00001990: 0000 6401 6402 8400 7c00 4400 8301 7d02  ..d.d...|.D...}.
-000019a0: 7c02 7316 7c02 5300 7400 7c02 8e00 5c02  |.s.|.S.t.|...\.
-000019b0: 7d03 7d04 7401 7c03 8301 7401 7402 7c03  }.}.t.|...t.t.|.
-000019c0: 8301 8301 6b03 7248 7403 a004 6403 7c01  ....k.rHt...d.|.
-000019d0: 9b00 6404 9d03 a101 8201 6405 6402 8400  ..d.......d.d...
-000019e0: 7c04 4400 8301 7d04 7c04 7280 7401 7c04  |.D...}.|.r.t.|.
-000019f0: 8301 7401 7402 7c04 8301 8301 6b03 7280  ..t.t.|.....k.r.
-00001a00: 7403 a004 6403 7c01 9b00 6406 9d03 a101  t...d.|...d.....
-00001a10: 8201 7c02 5300 2907 4e63 0100 0000 0000  ..|.S.).Nc......
-00001a20: 0000 0000 0000 0200 0000 0700 0000 5300  ..............S.
-00001a30: 0000 7338 0000 0067 007c 005d 307d 0164  ..s8...g.|.]0}.d
-00001a40: 007c 0176 0072 2c74 007c 016a 0164 0064  .|.v.r,t.|.j.d.d
-00001a50: 0164 028d 0264 0364 0364 0485 0319 0083  .d...d.d.d......
-00001a60: 016e 067c 0164 0366 0291 0271 0453 0029  .n.|.d.f...q.S.)
-00001a70: 05da 013d e901 0000 0029 01da 086d 6178  ...=.....)...max
-00001a80: 7370 6c69 744e e9ff ffff ff29 02da 0574  splitN.....)...t
-00001a90: 7570 6c65 da05 7370 6c69 7429 0272 3900  uple..split).r9.
-00001aa0: 0000 7249 0000 0072 2f00 0000 722f 0000  ..rI...r/...r/..
-00001ab0: 0072 3000 0000 724e 0000 00f7 0000 0072  .r0...rN.......r
-00001ac0: 4b00 0000 7a47 7275 6e5f 636f 6d6d 616e  K...zGrun_comman
-00001ad0: 645f 6c69 6e65 2e3c 6c6f 6361 6c73 3e2e  d_line.<locals>.
-00001ae0: 7061 7273 655f 6578 706c 6963 6974 5f64  parse_explicit_d
-00001af0: 6566 696e 6974 696f 6e2e 3c6c 6f63 616c  efinition.<local
-00001b00: 733e 2e3c 6c69 7374 636f 6d70 3e7a 2143  s>.<listcomp>z!C
-00001b10: 616e 6e6f 7420 7370 6563 6966 7920 7468  annot specify th
-00001b20: 6520 7361 6d65 2065 7870 6c69 6369 7420  e same explicit 
-00001b30: 7a0d 2076 616c 7565 2074 7769 6365 2e63  z. value twice.c
-00001b40: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001b50: 0300 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00001b60: 005d 0c7d 017c 0172 047c 0191 0271 0453  .].}.|.r.|...q.S
-00001b70: 0072 2f00 0000 722f 0000 0029 0272 3900  .r/...r/...).r9.
-00001b80: 0000 da01 6e72 2f00 0000 722f 0000 0072  ....nr/...r/...r
-00001b90: 3000 0000 724e 0000 0001 0100 0072 4b00  0...rN.......rK.
-00001ba0: 0000 7a0c 206e 616d 6520 7477 6963 652e  ..z. name twice.
-00001bb0: 2905 da03 7a69 7072 5400 0000 7252 0000  )...ziprT...rR..
-00001bc0: 0072 0f00 0000 da0a 5573 6167 6545 7272  .r......UsageErr
-00001bd0: 6f72 2905 da07 656e 7472 6965 73da 0474  or)...entries..t
-00001be0: 7970 65da 0672 6573 756c 74da 0676 616c  ype..result..val
-00001bf0: 7565 73da 056e 616d 6573 722f 0000 0072  ues..namesr/...r
-00001c00: 2f00 0000 7230 0000 00da 1970 6172 7365  /...r0.....parse
-00001c10: 5f65 7870 6c69 6369 745f 6465 6669 6e69  _explicit_defini
-00001c20: 7469 6f6e f600 0000 7314 0000 0000 010e  tion....s.......
-00001c30: 0204 0104 020c 0214 0112 020e 0218 0112  ................
-00001c40: 027a 3372 756e 5f63 6f6d 6d61 6e64 5f6c  .z3run_command_l
-00001c50: 696e 652e 3c6c 6f63 616c 733e 2e70 6172  ine.<locals>.par
-00001c60: 7365 5f65 7870 6c69 6369 745f 6465 6669  se_explicit_defi
-00001c70: 6e69 7469 6f6e da05 696e 7075 74da 066f  nition..input..o
-00001c80: 7574 7075 74da 0570 6172 616d 2909 da0c  utput..param)...
-00001c90: 636f 6d6d 616e 645f 6c69 6e65 da0f 6578  command_line..ex
-00001ca0: 706c 6963 6974 5f69 6e70 7574 73da 1065  plicit_inputs..e
-00001cb0: 7870 6c69 6369 745f 6f75 7470 7574 73da  xplicit_outputs.
-00001cc0: 1365 7870 6c69 6369 745f 7061 7261 6d65  .explicit_parame
-00001cd0: 7465 7273 da09 6469 7265 6374 6f72 79da  ters..directory.
-00001ce0: 0b77 6f72 6b69 6e67 5f64 6972 da12 6e6f  .working_dir..no
-00001cf0: 5f69 6e70 7574 5f64 6574 6563 7469 6f6e  _input_detection
-00001d00: da13 6e6f 5f6f 7574 7075 745f 6465 7465  ..no_output_dete
-00001d10: 6374 696f 6eda 0d73 7563 6365 7373 5f63  ction..success_c
-00001d20: 6f64 6573 6301 0000 0000 0000 0000 0000  odesc...........
-00001d30: 0003 0000 0007 0000 0013 0000 0073 2000  .............s .
-00001d40: 0000 6900 7c00 5d18 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
-00001d50: 7400 6a01 a002 7c02 8800 a102 9302 7104  t.j...|.......q.
-00001d60: 5300 722f 0000 0029 03da 026f 7372 3700  S.r/...)...osr7.
-00001d70: 0000 da07 7265 6c70 6174 6829 0372 3900  ....relpath).r9.
-00001d80: 0000 725b 0000 0072 3700 0000 a901 7283  ..r[...r7.....r.
-00001d90: 0000 0072 2f00 0000 7230 0000 00da 0a3c  ...r/...r0.....<
-00001da0: 6469 6374 636f 6d70 3e16 0100 0072 4b00  dictcomp>....rK.
-00001db0: 0000 7a24 7275 6e5f 636f 6d6d 616e 645f  ..z$run_command_
-00001dc0: 6c69 6e65 2e3c 6c6f 6361 6c73 3e2e 3c64  line.<locals>.<d
-00001dd0: 6963 7463 6f6d 703e 2901 da09 6e6f 5f6f  ictcomp>)...no_o
-00001de0: 7574 7075 7463 0100 0000 0000 0000 0000  utputc..........
-00001df0: 0000 0300 0000 0300 0000 7300 0000 7316  ..........s...s.
-00001e00: 0000 007c 005d 0e5c 027d 017d 027c 0256  ...|.].\.}.}.|.V
-00001e10: 0001 0071 0264 0053 0072 3600 0000 722f  ...q.d.S.r6...r/
-00001e20: 0000 0029 0372 3900 0000 7250 0000 0072  ...).r9...rP...r
-00001e30: 3700 0000 722f 0000 0072 2f00 0000 7230  7...r/...r/...r0
-00001e40: 0000 0072 3b00 0000 1c01 0000 724b 0000  ...r;.......rK..
-00001e50: 007a 2372 756e 5f63 6f6d 6d61 6e64 5f6c  .z#run_command_l
-00001e60: 696e 652e 3c6c 6f63 616c 733e 2e3c 6765  ine.<locals>.<ge
-00001e70: 6e65 7870 723e 724c 0000 0063 0100 0000  nexpr>rL...c....
-00001e80: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00001e90: 5300 0000 7318 0000 0069 007c 005d 107d  S...s....i.|.].}
-00001ea0: 017c 0174 0074 017c 0183 0293 0271 0453  .|.t.t.|.....q.S
-00001eb0: 0072 2f00 0000 2902 da07 6765 7461 7474  .r/...)...getatt
-00001ec0: 72da 0373 7973 2902 7239 0000 00da 036b  r..sys).r9.....k
-00001ed0: 6579 722f 0000 0072 2f00 0000 7230 0000  eyr/...r/...r0..
-00001ee0: 0072 8a00 0000 2a01 0000 724b 0000 00da  .r....*...rK....
-00001ef0: 0120 7a18 4361 6e6e 6f74 2065 7865 6375  . z.Cannot execu
-00001f00: 7465 2063 6f6d 6d61 6e64 2027 7a58 273a  te command 'zX':
-00001f10: 2054 6869 7320 6973 206c 696b 656c 7920   This is likely 
-00001f20: 6265 6361 7573 6520 7468 6520 6578 6563  because the exec
-00001f30: 7574 6162 6c65 2064 6f65 736e 2774 2065  utable doesn't e
-00001f40: 7869 7374 206f 7220 6861 7320 7468 6520  xist or has the 
-00001f50: 7772 6f6e 6720 7065 726d 6973 7369 6f6e  wrong permission
-00001f60: 7320 7365 742e 7201 0000 0029 0172 8600  s set.r....).r..
-00001f70: 0000 2905 725b 0000 00da 0b64 6573 6372  ..).r[.....descr
-00001f80: 6970 7469 6f6e da08 6b65 7977 6f72 6473  iption..keywords
-00001f90: da08 6372 6561 746f 7273 da0c 6461 7465  ..creators..date
-00001fa0: 5f63 7265 6174 6564 2905 da04 706c 616e  _created)...plan
-00001fb0: 7245 0000 00da 0f73 7461 7274 6564 5f61  rE.....started_a
-00001fc0: 745f 7469 6d65 da0d 656e 6465 645f 6174  t_time..ended_at
-00001fd0: 5f74 696d 65da 0b61 6e6e 6f74 6174 696f  _time..annotatio
-00001fe0: 6e73 2930 7260 0000 0072 0f00 0000 da0e  ns)0r`...r......
-00001ff0: 5061 7261 6d65 7465 7245 7272 6f72 da19  ParameterError..
-00002000: 6765 745f 6e65 7765 7374 5f70 6c61 6e73  get_newest_plans
-00002010: 5f62 795f 6e61 6d65 73da 1a44 7570 6c69  _by_names..Dupli
-00002020: 6361 7465 576f 726b 666c 6f77 4e61 6d65  cateWorkflowName
-00002030: 4572 726f 7272 2000 0000 7245 0000 00da  Errorr ...rE....
-00002040: 0961 6c6c 5f66 696c 6573 7211 0000 00da  .all_filesr.....
-00002050: 0675 7064 6174 6572 7400 0000 da05 636c  .updatert.....cl
-00002060: 6963 6bda 0573 7479 6c65 da04 6a6f 696e  ick..style..join
-00002070: 7278 0000 00da 046f 7065 6eda 074f 5345  rx.....open..OSE
-00002080: 7272 6f72 728d 0000 0072 6400 0000 7265  rrorr....rd...re
-00002090: 0000 0072 2d00 0000 7237 0000 0072 1f00  ...r-...r7...r..
-000020a0: 0000 7287 0000 00da 0667 6574 6377 64da  ..r......getcwd.
-000020b0: 0569 7465 6d73 5a05 7761 7463 6872 1400  .itemsZ.watchr..
-000020c0: 0000 5a10 6974 6572 5f69 6e70 7574 5f66  ..Z.iter_input_f
-000020d0: 696c 6573 7215 0000 0072 1600 0000 7204  ilesr....r....r.
-000020e0: 0000 0072 7e00 0000 da04 6b65 7973 da11  ...r~.....keys..
-000020f0: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
-00002100: 72da 0c62 6173 655f 636f 6d6d 616e 64da  r..base_command.
-00002110: 0566 6c75 7368 da12 496e 7661 6c69 6453  .flush..InvalidS
-00002120: 7563 6365 7373 436f 6465 720b 0000 0072  uccessCoder....r
-00002130: 2200 0000 7217 0000 00da 0774 6f5f 706c  "...r......to_pl
-00002140: 616e 7221 0000 00da 0966 726f 6d5f 706c  anr!.....from_pl
-00002150: 616e 7297 0000 0072 5300 0000 720e 0000  anr....rS...r...
-00002160: 00da 0563 6c6f 7365 2925 725b 0000 0072  ...close)%r[...r
-00002170: 9000 0000 da07 6b65 7977 6f72 6472 7f00  ......keywordr..
-00002180: 0000 7280 0000 0072 8100 0000 728b 0000  ..r....r....r...
-00002190: 0072 8400 0000 7285 0000 0072 8600 0000  .r....r....r....
-000021a0: 727e 0000 0072 9200 0000 7262 0000 0072  r~...r....rb...r
-000021b0: 6300 0000 da0a 7661 6c69 645f 6e61 6d65  c.....valid_name
-000021c0: da09 776f 726b 666c 6f77 7372 3300 0000  ..workflowsr3...
-000021d0: 5a0a 6d61 7070 6564 5f73 7464 5a0d 6d61  Z.mapped_stdZ.ma
-000021e0: 7070 6564 5f73 7464 5f69 6eda 0769 6e76  pped_std_in..inv
-000021f0: 616c 6964 5a0d 7379 7374 656d 5f73 7464  alidZ.system_std
-00002200: 6f75 745a 0d73 7973 7465 6d5f 7374 6465  outZ.system_stde
-00002210: 7272 5a0a 7474 795f 6578 6973 7473 5a11  rrZ.tty_existsZ.
-00002220: 7374 646f 7574 5f72 6564 6972 6563 7465  stdout_redirecte
-00002230: 645a 1173 7464 6572 725f 7265 6469 7265  dZ.stderr_redire
-00002240: 6374 6564 5a0a 6f6c 645f 7374 646f 7574  ctedZ.old_stdout
-00002250: 5a0a 6f6c 645f 7374 6465 7272 727a 0000  Z.old_stderrrz..
-00002260: 00da 0766 6163 746f 7279 da04 746f 6f6c  ...factory..tool
-00002270: 5a06 7061 7468 735f 7295 0000 00da 0b72  Z.paths_r......r
-00002280: 6574 7572 6e5f 636f 6465 da07 636f 6d6d  eturn_code..comm
-00002290: 616e 6472 9600 0000 7294 0000 0072 3d00  andr....r....r=.
-000022a0: 0000 722f 0000 0072 8900 0000 7230 0000  ..r/...r....r0..
-000022b0: 00da 1072 756e 5f63 6f6d 6d61 6e64 5f6c  ...run_command_l
-000022c0: 696e 65a6 0000 0073 1601 0000 0014 0401  ine....s........
-000022d0: 0801 0801 1802 0801 0801 1202 1001 0c02  ................
-000022e0: 1001 0c01 0a02 0c01 0401 0401 0201 16ff  ................
-000022f0: 0201 02ff 02ff 0405 0c01 0401 0401 0201  ................
-00002300: 16ff 0201 02ff 02ff 0405 0401 0404 0201  ................
-00002310: 0c01 2801 0e01 0a02 0401 0801 0802 0603  ..(.............
-00002320: 0601 0a01 0601 0602 0601 0a01 0601 0602  ................
-00002330: 0a02 0812 0a01 0a01 0a02 0401 0201 0201  ................
-00002340: 0201 0201 0601 0201 0201 0201 02f7 040a  ................
-00002350: 14f6 060c 1002 0802 1601 1202 0602 0601  ................
-00002360: 0601 0601 0602 0602 0201 0201 04ff 0401  ................
-00002370: 06ff 0201 10ff 0a03 0e01 0c01 0401 0aff  ................
-00002380: 0a05 0602 0a01 0a02 0602 0601 0601 0601  ................
-00002390: 0602 1201 2e02 0601 1202 0401 0aff 0603  ................
-000023a0: 0401 0201 0401 0201 0201 04fb 0607 0a02  ................
-000023b0: 0a03 0601 0801 0601 0801 0601 0801 0601  ................
-000023c0: 08f6 0203 0001 0001 0001 0001 0601 0801  ................
-000023d0: 0601 0af9 0601 0801 0601 0801 0601 0801  ................
-000023e0: 0601 72b4 0000 0029 024e 4629 4372 2c00  ..r....).NF)Cr,.
-000023f0: 0000 7287 0000 0072 8d00 0000 da0b 636f  ..r....r......co
-00002400: 6c6c 6563 7469 6f6e 7372 0200 0000 da07  llectionsr......
-00002410: 7061 7468 6c69 6272 0300 0000 da0a 7375  pathlibr......su
-00002420: 6270 726f 6365 7373 7204 0000 00da 0674  bprocessr......t
-00002430: 7970 696e 6772 0500 0000 7206 0000 0072  ypingr....r....r
-00002440: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
-00002450: 0000 0072 0b00 0000 729d 0000 00da 0870  ...r....r......p
-00002460: 7964 616e 7469 6372 0c00 0000 da1d 7265  ydanticr......re
-00002470: 6e6b 752e 636f 6d6d 616e 642e 636f 6d6d  nku.command.comm
-00002480: 616e 645f 6275 696c 6465 7272 0d00 0000  and_builderr....
-00002490: da1d 7265 6e6b 752e 636f 6d6d 616e 642e  ..renku.command.
-000024a0: 7669 6577 5f6d 6f64 656c 2e70 6c61 6e72  view_model.planr
-000024b0: 0e00 0000 da0a 7265 6e6b 752e 636f 7265  ......renku.core
-000024c0: 720f 0000 00da 1172 656e 6b75 2e63 6f72  r......renku.cor
-000024d0: 652e 636f 6e66 6967 7210 0000 005a 0e72  e.configr....Z.r
-000024e0: 656e 6b75 2e63 6f72 652e 6769 7472 1100  enku.core.gitr..
-000024f0: 0000 da25 7265 6e6b 752e 636f 7265 2e69  ...%renku.core.i
-00002500: 6e74 6572 6661 6365 2e61 6374 6976 6974  nterface.activit
-00002510: 795f 6761 7465 7761 7972 1200 0000 da21  y_gatewayr.....!
-00002520: 7265 6e6b 752e 636f 7265 2e69 6e74 6572  renku.core.inter
-00002530: 6661 6365 2e70 6c61 6e5f 6761 7465 7761  face.plan_gatewa
-00002540: 7972 1300 0000 da12 7265 6e6b 752e 636f  yr......renku.co
-00002550: 7265 2e73 746f 7261 6765 7214 0000 0072  re.storager....r
-00002560: 1500 0000 da1c 7265 6e6b 752e 636f 7265  ......renku.core
-00002570: 2e75 7469 6c2e 6461 7465 7469 6d65 3836  .util.datetime86
-00002580: 3031 7216 0000 00da 1372 656e 6b75 2e63  01r......renku.c
-00002590: 6f72 652e 7574 696c 2e67 6974 7217 0000  ore.util.gitr...
-000025a0: 00da 1272 656e 6b75 2e63 6f72 652e 7574  ...renku.core.ut
-000025b0: 696c 2e6f 7372 1800 0000 7219 0000 00da  il.osr....r.....
-000025c0: 1472 656e 6b75 2e63 6f72 652e 7574 696c  .renku.core.util
-000025d0: 2e75 726c 7372 1b00 0000 da1c 7265 6e6b  .urlsr......renk
-000025e0: 752e 636f 7265 2e77 6f72 6b66 6c6f 772e  u.core.workflow.
-000025f0: 6163 7469 7669 7479 721c 0000 0072 1d00  activityr....r..
-00002600: 0000 721e 0000 005a 2072 656e 6b75 2e63  ..r....Z renku.c
-00002610: 6f72 652e 776f 726b 666c 6f77 2e70 6c61  ore.workflow.pla
-00002620: 6e5f 6661 6374 6f72 7972 1f00 0000 da22  n_factoryr....."
-00002630: 7265 6e6b 752e 646f 6d61 696e 5f6d 6f64  renku.domain_mod
-00002640: 656c 2e70 726f 6a65 6374 5f63 6f6e 7465  el.project_conte
-00002650: 7874 7220 0000 00da 2672 656e 6b75 2e64  xtr ....&renku.d
-00002660: 6f6d 6169 6e5f 6d6f 6465 6c2e 7072 6f76  omain_model.prov
-00002670: 656e 616e 6365 2e61 6374 6976 6974 7972  enance.activityr
-00002680: 2100 0000 da23 7265 6e6b 752e 646f 6d61  !....#renku.doma
-00002690: 696e 5f6d 6f64 656c 2e70 726f 7665 6e61  in_model.provena
-000026a0: 6e63 652e 6167 656e 7472 2200 0000 7223  nce.agentr"...r#
-000026b0: 0000 00da 0464 6963 7472 2d00 0000 da04  .....dictr-.....
-000026c0: 626f 6f6c 725a 0000 0072 6000 0000 7261  boolrZ...r`...ra
-000026d0: 0000 00da 0a61 7574 6f70 6172 616d 7372  .....autoparamsr
-000026e0: b400 0000 722f 0000 0072 2f00 0000 722f  ....r/...r/...r/
-000026f0: 0000 0072 3000 0000 da08 3c6d 6f64 756c  ...r0.....<modul
-00002700: 653e 1100 0000 7348 0000 0004 0208 0108  e>....sH........
-00002710: 010c 010c 010c 0124 0208 010c 020c 010c  .......$........
-00002720: 010c 010c 010c 010c 010c 0110 010c 010c  ................
-00002730: 0110 010c 0114 050c 010c 010c 010c 0310  ................
-00002740: 0f0e 0126 5810 0510 050a 010e 0e02 0102  ...&X...........
-00002750: 0102 f1                                  ...
+00000170: 6418 6c38 6d39 5a39 0100 6401 6419 6c3a  d.l8m9Z9..d.d.l:
+00000180: 6d3b 5a3b 0100 4700 641a 641b 8400 641b  m;Z;..G.d.d...d.
+00000190: 650e 8303 5a3c 6515 653d 641c 641d 8d01  e...Z<e.e=d.d...
+000001a0: 641e 8d01 642d 650f 650d 6511 6508 653e  d...d-e.e.e.e.e>
+000001b0: 6602 1900 1900 1900 653f 653c 6420 9c03  f.......e?e<d ..
+000001c0: 6421 6422 8405 8301 5a40 653e 653e 6423  d!d"....Z@e>e>d#
+000001d0: 9c02 6424 6425 8404 5a41 653e 653e 6423  ..d$d%..ZAe>e>d#
+000001e0: 9c02 6426 6427 8404 5a42 6517 a043 6428  ..d&d'..ZBe..Cd(
+000001f0: 6429 a102 6515 653d 641c 641d 8d01 641e  d)..e.e=d.d...d.
+00000200: 8d01 6521 6523 6519 642a 9c03 642b 642c  ..e!e#e.d*..d+d,
+00000210: 8404 8301 8301 5a44 6402 5300 292e 7a18  ......ZDd.S.).z.
+00000220: 5275 6e6e 696e 6720 776f 726b 666c 6f77  Running workflow
+00000230: 7320 6c6f 6769 632e e900 0000 004e 2901  s logic......N).
+00000240: da0b 6465 6661 756c 7464 6963 7429 01da  ..defaultdict)..
+00000250: 1455 6e73 7570 706f 7274 6564 4f70 6572  .UnsupportedOper
+00000260: 6174 696f 6e29 01da 0450 6174 6829 01da  ation)...Path)..
+00000270: 0463 616c 6c29 07da 0444 6963 74da 044c  .call)...Dict..L
+00000280: 6973 74da 0a4e 616d 6564 5475 706c 65da  ist..NamedTuple.
+00000290: 084f 7074 696f 6e61 6cda 0353 6574 da05  .Optional..Set..
+000002a0: 556e 696f 6eda 0463 6173 7429 01da 1276  Union..cast)...v
+000002b0: 616c 6964 6174 655f 6172 6775 6d65 6e74  alidate_argument
+000002c0: 7329 01da 0669 6e6a 6563 7429 01da 0d50  s)...inject)...P
+000002d0: 6c61 6e56 6965 774d 6f64 656c 2901 da06  lanViewModel)...
+000002e0: 6572 726f 7273 2901 da09 6765 745f 7661  errors)...get_va
+000002f0: 6c75 6529 01da 1667 6574 5f6d 6170 7065  lue)...get_mappe
+00000300: 645f 7374 645f 7374 7265 616d 7329 01da  d_std_streams)..
+00000310: 1049 4163 7469 7669 7479 4761 7465 7761  .IActivityGatewa
+00000320: 7929 01da 0c49 506c 616e 4761 7465 7761  y)...IPlanGatewa
+00000330: 7929 02da 1663 6865 636b 5f65 7874 6572  y)...check_exter
+00000340: 6e61 6c5f 7374 6f72 6167 65da 1770 756c  nal_storage..pul
+00000350: 6c5f 7061 7468 735f 6672 6f6d 5f73 746f  l_paths_from_sto
+00000360: 7261 6765 2901 da09 6c6f 6361 6c5f 6e6f  rage)...local_no
+00000370: 7729 01da 0c67 6574 5f67 6974 5f75 7365  w)...get_git_use
+00000380: 7229 02da 1867 6574 5f72 656c 6174 6976  r)...get_relativ
+00000390: 655f 7061 7468 5f74 6f5f 6377 64da 1267  e_path_to_cwd..g
+000003a0: 6574 5f72 656c 6174 6976 655f 7061 7468  et_relative_path
+000003b0: 73a9 01da 0867 6574 5f73 6c75 6729 03da  s....get_slug)..
+000003c0: 3467 6574 5f61 6c6c 5f6d 6f64 6966 6965  4get_all_modifie
+000003d0: 645f 616e 645f 6465 6c65 7465 645f 6163  d_and_deleted_ac
+000003e0: 7469 7669 7469 6573 5f61 6e64 5f65 6e74  tivities_and_ent
+000003f0: 6974 6965 73da 2467 6574 5f64 6f77 6e73  ities.$get_downs
+00000400: 7472 6561 6d5f 6765 6e65 7261 7469 6e67  tream_generating
+00000410: 5f61 6374 6976 6974 6965 73da 1169 735f  _activities..is_
+00000420: 6163 7469 7669 7479 5f76 616c 6964 2901  activity_valid).
+00000430: da0b 506c 616e 4661 6374 6f72 7929 01da  ..PlanFactory)..
+00000440: 0f70 726f 6a65 6374 5f63 6f6e 7465 7874  .project_context
+00000450: 2901 da08 4163 7469 7669 7479 2901 da06  )...Activity)...
+00000460: 5065 7273 6f6e 6300 0000 0000 0000 0000  Personc.........
+00000470: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
+00000480: 6600 0000 6500 5a01 6400 5a02 5500 6401  f...e.Z.d.Z.U.d.
+00000490: 5a03 6504 6505 6506 6505 1900 6602 1900  Z.e.e.e.e...f...
+000004a0: 6507 6402 3c00 6504 6505 6506 6505 1900  e.d.<.e.e.e.e...
+000004b0: 6602 1900 6507 6403 3c00 6506 6505 1900  f...e.d.<.e.e...
+000004c0: 6507 6404 3c00 6506 6505 1900 6507 6405  e.d.<.e.e...e.d.
+000004d0: 3c00 6504 6505 6506 6505 1900 6602 1900  <.e.e.e.e...f...
+000004e0: 6507 6406 3c00 6407 5300 2908 da0c 5374  e.d.<.d.S.)...St
+000004f0: 6174 7573 5265 7375 6c74 6134 0100 0052  atusResulta4...R
+00000500: 6570 7265 7365 6e74 2073 7461 7475 7320  epresent status 
+00000510: 6f66 2061 2070 726f 6a65 6374 2e0a 0a20  of a project... 
+00000520: 2020 2041 2071 7569 6e74 7570 6c65 2063     A quintuple c
+00000530: 6f6e 7461 696e 696e 6720 6120 6d61 7070  ontaining a mapp
+00000540: 696e 6720 6f66 2073 7461 6c65 206f 7574  ing of stale out
+00000550: 7075 7473 2074 6f20 6d6f 6469 6669 6564  puts to modified
+00000560: 2075 7361 6765 732c 2061 206d 6170 7069   usages, a mappi
+00000570: 6e67 206f 6620 7374 616c 6520 6163 7469  ng of stale acti
+00000580: 7669 7469 6573 2074 6861 7420 6861 7665  vities that have
+00000590: 206e 6f0a 2020 2020 6765 6e65 7261 7469   no.    generati
+000005a0: 6f6e 2074 6f20 6d6f 6469 6669 6564 2075  on to modified u
+000005b0: 7361 6765 732c 2061 2073 6574 206f 6620  sages, a set of 
+000005c0: 6d6f 6469 6669 6564 2075 7361 6765 732c  modified usages,
+000005d0: 2061 2073 6574 206f 6620 6465 6c65 7465   a set of delete
+000005e0: 6420 7573 6167 6573 2c20 616e 6420 6120  d usages, and a 
+000005f0: 6d61 7020 6f66 206d 6f64 6966 6965 6420  map of modified 
+00000600: 6869 6464 656e 0a20 2020 2069 6e70 7574  hidden.    input
+00000610: 7320 746f 2070 6174 6873 2074 6861 7420  s to paths that 
+00000620: 7468 6579 2067 656e 6572 6174 652e 0a20  they generate.. 
+00000630: 2020 20da 106f 7574 6461 7465 645f 6f75     ..outdated_ou
+00000640: 7470 7574 73da 136f 7574 6461 7465 645f  tputs..outdated_
+00000650: 6163 7469 7669 7469 6573 da0f 6d6f 6469  activities..modi
+00000660: 6669 6564 5f69 6e70 7574 73da 0e64 656c  fied_inputs..del
+00000670: 6574 6564 5f69 6e70 7574 73da 166d 6f64  eted_inputs..mod
+00000680: 6966 6965 645f 6869 6464 656e 5f69 6e70  ified_hidden_inp
+00000690: 7574 734e 2908 da08 5f5f 6e61 6d65 5f5f  utsN)...__name__
+000006a0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000006b0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+000006c0: 635f 5f72 0600 0000 da03 7374 7272 0a00  c__r......strr..
+000006d0: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
+000006e0: 735f 5fa9 0072 3000 0000 7230 0000 00fa  s__..r0...r0....
+000006f0: 462f 686f 6d65 2f72 756e 6e65 722f 776f  F/home/runner/wo
+00000700: 726b 2f72 656e 6b75 2d70 7974 686f 6e2f  rk/renku-python/
+00000710: 7265 6e6b 752d 7079 7468 6f6e 2f72 656e  renku-python/ren
+00000720: 6b75 2f63 6f72 652f 776f 726b 666c 6f77  ku/core/workflow
+00000730: 2f72 756e 2e70 7972 2400 0000 3500 0000  /run.pyr$...5...
+00000740: 730c 0000 000a 0104 0714 0114 010c 010c  s...............
+00000750: 0172 2400 0000 5429 01da 1761 7262 6974  .r$...T)...arbit
+00000760: 7261 7279 5f74 7970 6573 5f61 6c6c 6f77  rary_types_allow
+00000770: 6564 2901 da06 636f 6e66 6967 4629 03da  ed)...configF)..
+00000780: 0570 6174 6873 da0e 6967 6e6f 7265 5f64  .paths..ignore_d
+00000790: 656c 6574 6564 da06 7265 7475 726e 6302  eleted..returnc.
+000007a0: 0000 0000 0000 0000 0000 0012 0000 0007  ................
+000007b0: 0000 0003 0000 0073 d201 0000 6401 6402  .......s....d.d.
+000007c0: 8400 7d02 8700 6601 6403 6404 8408 7d03  ..}...f.d.d...}.
+000007d0: 7c01 7020 7400 6405 6406 8302 7d01 7401  |.p t.d.d...}.t.
+000007e0: 7402 6a03 6407 6408 8d02 5c03 7d04 7d05  t.j.d.d...\.}.}.
+000007f0: 7d06 6409 640a 8400 7c04 4400 8301 7d04  }.d.d...|.D...}.
+00000800: 640b 640a 8400 7c05 4400 8301 7d05 640c  d.d...|.D...}.d.
+00000810: 640a 8400 7c06 4400 8301 7d06 7c04 7380  d...|.D...}.|.s.
+00000820: 7c05 7380 7c06 7380 7404 6900 6900 7405  |.s.|.s.t.i.i.t.
+00000830: 8300 7405 8300 6900 8305 5300 8800 7086  ..t...i...S...p.
+00000840: 6700 8900 7406 7402 6a07 640d 640e 8400  g...t.t.j.d.d...
+00000850: 8800 4400 8301 640f 8d02 8900 7405 8300  ..D...d.....t...
+00000860: 7d07 7408 7405 8301 7d08 7408 7405 8301  }.t.t...}.t.t...
+00000870: 7d09 7408 7405 8301 7d0a 7c04 4400 5d7e  }.t.t...}.|.D.]~
+00000880: 5c02 7d0b 7d0c 7c03 7c0b 7c0c 7c01 6410  \.}.}.|.|.|.|.d.
+00000890: 8d03 7d0d 7c0d 72c2 7409 7402 6a07 7c0c  ..}.|.r.t.t.j.|.
+000008a0: 6a07 1b00 8301 7d0e 7c07 a00a 7c0e a101  j.....}.|...|...
+000008b0: 0100 7c0d 4400 5d44 7d0f 740b 7c0f 6a0c  ..|.D.]D}.t.|.j.
+000008c0: 8301 6411 6b02 9001 7220 7c09 7c0f 6a0d  ..d.k...r |.|.j.
+000008d0: 1900 a00a 7c0e a101 0100 71fa 7c02 7c0f  ....|.....q.|.|.
+000008e0: 8301 4400 5d14 7d10 7c08 7c10 1900 a00a  ..D.].}.|.|.....
+000008f0: 7c0e a101 0100 9001 7128 71fa 71c2 6412  |.......q(q.q.d.
+00000900: 640a 8400 7c05 4400 8301 7d11 8700 6601  d...|.D...}...f.
+00000910: 6413 640a 8408 7c11 4400 8301 7d11 7c06  d.d...|.D...}.|.
+00000920: 4400 5d58 5c02 7d0b 7d0c 7c03 7c0b 7c0c  D.]X\.}.}.|.|.|.
+00000930: 6407 6410 8d03 7d0d 7c0d 9001 7266 7409  d.d...}.|...rft.
+00000940: 7402 6a07 7c0c 6a07 1b00 8301 7d0e 7c0d  t.j.|.j.....}.|.
+00000950: 4400 5d24 7d0f 7c02 7c0f 8301 4400 5d14  D.]$}.|.|...D.].
+00000960: 7d10 7c0a 7c0e 1900 a00a 7c10 a101 0100  }.|.|.....|.....
+00000970: 9001 71a2 9001 7196 9001 7166 7404 7c08  ..q...q...qft.|.
+00000980: 7c09 7c07 7c11 7c0a 6414 8d05 5300 2915  |.|.|.|.d...S.).
+00000990: 6134 0100 0052 6574 7572 6e20 7374 6174  a4...Return stat
+000009a0: 7573 206f 6620 6120 7072 6f6a 6563 742e  us of a project.
+000009b0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000009c0: 2020 2020 7061 7468 7328 4f70 7469 6f6e      paths(Option
+000009d0: 616c 5b4c 6973 745b 556e 696f 6e5b 5061  al[List[Union[Pa
+000009e0: 7468 2c20 7374 725d 5d5d 293a 204c 696d  th, str]]]): Lim
+000009f0: 6974 2074 6865 2073 7461 7475 7320 746f  it the status to
+00000a00: 2074 6869 7320 6c69 7374 206f 6620 7061   this list of pa
+00000a10: 7468 7320 2844 6566 6175 6c74 2076 616c  ths (Default val
+00000a20: 7565 203d 204e 6f6e 6529 2e0a 2020 2020  ue = None)..    
+00000a30: 2020 2020 6967 6e6f 7265 5f64 656c 6574      ignore_delet
+00000a40: 6564 2862 6f6f 6c29 3a20 5768 6574 6865  ed(bool): Whethe
+00000a50: 7220 746f 2069 676e 6f72 6520 6465 6c65  r to ignore dele
+00000a60: 7465 6420 6765 6e65 7261 7469 6f6e 7320  ted generations 
+00000a70: 2844 6566 6175 6c74 2076 616c 7565 203d  (Default value =
+00000a80: 2046 616c 7365 292e 0a0a 2020 2020 5265   False)...    Re
+00000a90: 7475 726e 733a 0a20 2020 2020 2020 2053  turns:.        S
+00000aa0: 7461 7475 7352 6573 756c 743a 2053 7461  tatusResult: Sta
+00000ab0: 7475 7320 6f66 2074 6865 2070 726f 6a65  tus of the proje
+00000ac0: 6374 2e0a 0a20 2020 2063 0100 0000 0000  ct...    c......
+00000ad0: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
+00000ae0: 0000 7310 0000 0064 0164 0284 007c 006a  ..s....d.d...|.j
+00000af0: 0044 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
+00000b00: 0000 0000 0000 0002 0000 0004 0000 0073  ...............s
+00000b10: 0000 0073 2000 0000 7c00 5d18 7d01 7400  ...s ...|.].}.t.
+00000b20: 7401 6a02 7c01 6a03 6a02 1b00 8301 5600  t.j.|.j.j.....V.
+00000b30: 0100 7102 6400 5300 a901 4e29 0472 1900  ..q.d.S...N).r..
+00000b40: 0000 7221 0000 00da 0470 6174 68da 0665  ..r!.....path..e
+00000b50: 6e74 6974 7929 02da 022e 30da 0a67 656e  ntity)....0..gen
+00000b60: 6572 6174 696f 6e72 3000 0000 7230 0000  erationr0...r0..
+00000b70: 0072 3100 0000 da09 3c67 656e 6578 7072  .r1.....<genexpr
+00000b80: 3e52 0000 0073 0400 0000 0402 02ff 7a3a  >R...s........z:
+00000b90: 6765 745f 7374 6174 7573 2e3c 6c6f 6361  get_status.<loca
+00000ba0: 6c73 3e2e 6765 745f 616c 6c5f 6765 6e65  ls>.get_all_gene
+00000bb0: 7261 7469 6f6e 732e 3c6c 6f63 616c 733e  rations.<locals>
+00000bc0: 2e3c 6765 6e65 7870 723e 2901 da0b 6765  .<genexpr>)...ge
+00000bd0: 6e65 7261 7469 6f6e 7329 01da 0861 6374  nerations)...act
+00000be0: 6976 6974 7972 3000 0000 7230 0000 0072  ivityr0...r0...r
+00000bf0: 3100 0000 da13 6765 745f 616c 6c5f 6765  1.....get_all_ge
+00000c00: 6e65 7261 7469 6f6e 7351 0000 0073 0600  nerationsQ...s..
+00000c10: 0000 0001 0602 04fe 7a27 6765 745f 7374  ........z'get_st
+00000c20: 6174 7573 2e3c 6c6f 6361 6c73 3e2e 6765  atus.<locals>.ge
+00000c30: 745f 616c 6c5f 6765 6e65 7261 7469 6f6e  t_all_generation
+00000c40: 7363 0300 0000 0000 0000 0000 0000 0400  sc..............
+00000c50: 0000 0600 0000 1300 0000 732a 0000 0088  ..........s*....
+00000c60: 0072 0e7c 016a 0088 0076 0072 1267 006e  .r.|.j...v.r.g.n
+00000c70: 0288 007d 0374 017c 0068 017c 037c 0274  ...}.t.|.h.|.|.t
+00000c80: 026a 0064 018d 0453 0029 024e 2904 5a13  .j.d...S.).N).Z.
+00000c90: 7374 6172 7469 6e67 5f61 6374 6976 6974  starting_activit
+00000ca0: 6965 7372 3400 0000 7235 0000 00da 0c70  iesr4...r5.....p
+00000cb0: 726f 6a65 6374 5f70 6174 6829 0372 3800  roject_path).r8.
+00000cc0: 0000 721e 0000 0072 2100 0000 2904 da0e  ..r....r!...)...
+00000cd0: 7374 6172 745f 6163 7469 7669 7479 7239  start_activityr9
+00000ce0: 0000 0072 3500 0000 da10 6765 6e65 7261  ...r5.....genera
+00000cf0: 7469 6f6e 5f70 6174 6873 a901 7234 0000  tion_paths..r4..
+00000d00: 0072 3000 0000 7231 0000 00da 1967 6574  .r0...r1.....get
+00000d10: 5f64 6f77 6e73 7472 6561 6d5f 6163 7469  _downstream_acti
+00000d20: 7669 7469 6573 5700 0000 730e 0000 0000  vitiesW...s.....
+00000d30: 0316 0202 0104 0102 0102 0104 fc7a 2d67  .............z-g
+00000d40: 6574 5f73 7461 7475 732e 3c6c 6f63 616c  et_status.<local
+00000d50: 733e 2e67 6574 5f64 6f77 6e73 7472 6561  s>.get_downstrea
+00000d60: 6d5f 6163 7469 7669 7469 6573 da05 7265  m_activities..re
+00000d70: 6e6b 755a 1475 7064 6174 655f 6967 6e6f  nkuZ.update_igno
+00000d80: 7265 5f64 656c 6574 6554 2902 da0a 7265  re_deleteT)...re
+00000d90: 706f 7369 746f 7279 5a19 6368 6563 6b5f  positoryZ.check_
+00000da0: 6869 6464 656e 5f64 6570 656e 6465 6e63  hidden_dependenc
+00000db0: 6965 7363 0100 0000 0000 0000 0000 0000  iesc............
+00000dc0: 0300 0000 0400 0000 5300 0000 7320 0000  ........S...s ..
+00000dd0: 0068 007c 005d 185c 027d 017d 0274 007c  .h.|.].\.}.}.t.|
+00000de0: 0183 0172 047c 017c 0266 0292 0271 0453  ...r.|.|.f...q.S
+00000df0: 0072 3000 0000 a901 721f 0000 00a9 0372  .r0.....r......r
+00000e00: 3a00 0000 da01 61da 0165 7230 0000 0072  :.....a..er0...r
+00000e10: 3000 0000 7231 0000 00da 093c 7365 7463  0...r1.....<setc
+00000e20: 6f6d 703e 6900 0000 f300 0000 007a 1d67  omp>i........z.g
+00000e30: 6574 5f73 7461 7475 732e 3c6c 6f63 616c  et_status.<local
+00000e40: 733e 2e3c 7365 7463 6f6d 703e 6301 0000  s>.<setcomp>c...
+00000e50: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00000e60: 0053 0000 0073 2000 0000 6800 7c00 5d18  .S...s ...h.|.].
+00000e70: 5c02 7d01 7d02 7400 7c01 8301 7204 7c01  \.}.}.t.|...r.|.
+00000e80: 7c02 6602 9202 7104 5300 7230 0000 0072  |.f...q.S.r0...r
+00000e90: 4700 0000 7248 0000 0072 3000 0000 7230  G...rH...r0...r0
+00000ea0: 0000 0072 3100 0000 724b 0000 006a 0000  ...r1...rK...j..
+00000eb0: 0072 4c00 0000 6301 0000 0000 0000 0000  .rL...c.........
+00000ec0: 0000 0003 0000 0004 0000 0053 0000 0073  ...........S...s
+00000ed0: 2000 0000 6800 7c00 5d18 5c02 7d01 7d02   ...h.|.].\.}.}.
+00000ee0: 7400 7c01 8301 7204 7c01 7c02 6602 9202  t.|...r.|.|.f...
+00000ef0: 7104 5300 7230 0000 0072 4700 0000 7248  q.S.r0...rG...rH
+00000f00: 0000 0072 3000 0000 7230 0000 0072 3100  ...r0...r0...r1.
+00000f10: 0000 724b 0000 006b 0000 0072 4c00 0000  ..rK...k...rL...
+00000f20: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000f30: 0004 0000 0053 0000 0073 1800 0000 6700  .....S...s....g.
+00000f40: 7c00 5d10 7d01 7400 a001 a100 7c01 1b00  |.].}.t.....|...
+00000f50: 9102 7104 5300 7230 0000 0029 0272 0400  ..q.S.r0...).r..
+00000f60: 0000 da03 6377 6429 0272 3a00 0000 da01  ....cwd).r:.....
+00000f70: 7072 3000 0000 7230 0000 0072 3100 0000  pr0...r0...r1...
+00000f80: da0a 3c6c 6973 7463 6f6d 703e 7100 0000  ..<listcomp>q...
+00000f90: 724c 0000 007a 1e67 6574 5f73 7461 7475  rL...z.get_statu
+00000fa0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+00000fb0: 636f 6d70 3e29 02da 0462 6173 6572 3400  comp>)...baser4.
+00000fc0: 0000 2903 7241 0000 0072 3900 0000 7235  ..).rA...r9...r5
+00000fd0: 0000 0072 0100 0000 6301 0000 0000 0000  ...r....c.......
+00000fe0: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
+00000ff0: 0073 1600 0000 6800 7c00 5d0e 5c02 7d01  .s....h.|.].\.}.
+00001000: 7d02 7c02 6a00 9202 7104 5300 7230 0000  }.|.j...q.S.r0..
+00001010: 0029 0172 3800 0000 2903 723a 0000 00da  .).r8...).r:....
+00001020: 015f 724a 0000 0072 3000 0000 7230 0000  ._rJ...r0...r0..
+00001030: 0072 3100 0000 724b 0000 0087 0000 0072  .r1...rK.......r
+00001040: 4c00 0000 6301 0000 0000 0000 0000 0000  L...c...........
+00001050: 0002 0000 0005 0000 0013 0000 0073 2600  .............s&.
+00001060: 0000 6800 7c00 5d1e 7d01 8800 7214 7c01  ..h.|.].}...r.|.
+00001070: 8800 7600 7204 7400 7401 6a02 7c01 1b00  ..v.r.t.t.j.|...
+00001080: 8301 9202 7104 5300 7230 0000 0029 0372  ....q.S.r0...).r
+00001090: 1900 0000 7221 0000 0072 3800 0000 2902  ....r!...r8...).
+000010a0: 723a 0000 00da 0164 7243 0000 0072 3000  r:.....drC...r0.
+000010b0: 0000 7231 0000 0072 4b00 0000 8800 0000  ..r1...rK.......
+000010c0: 7302 0000 0006 0129 0572 2500 0000 7226  s......).r%...r&
+000010d0: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
+000010e0: 0000 290e 7211 0000 0072 1d00 0000 7221  ..).r....r....r!
+000010f0: 0000 0072 4600 0000 7224 0000 00da 0373  ...rF...r$.....s
+00001100: 6574 721a 0000 0072 3800 0000 7202 0000  etr....r8...r...
+00001110: 0072 1900 0000 da03 6164 64da 036c 656e  .r......add..len
+00001120: 723d 0000 00da 0269 6429 1272 3400 0000  r=.....id).r4...
+00001130: 7235 0000 0072 3f00 0000 7244 0000 00da  r5...r?...rD....
+00001140: 086d 6f64 6966 6965 64da 0764 656c 6574  .modified..delet
+00001150: 6564 5a0f 6869 6464 656e 5f6d 6f64 6966  edZ.hidden_modif
+00001160: 6965 6472 2700 0000 5a0d 7374 616c 655f  iedr'...Z.stale_
+00001170: 6f75 7470 7574 735a 1073 7461 6c65 5f61  outputsZ.stale_a
+00001180: 6374 6976 6974 6965 7372 2900 0000 7241  ctivitiesr)...rA
+00001190: 0000 0072 3900 0000 da0a 6163 7469 7669  ...r9.....activi
+000011a0: 7469 6573 5a0a 7573 6167 655f 7061 7468  tiesZ.usage_path
+000011b0: 723e 0000 005a 0f67 656e 6572 6174 696f  r>...Z.generatio
+000011c0: 6e5f 7061 7468 da0d 6465 6c65 7465 645f  n_path..deleted_
+000011d0: 7061 7468 7372 3000 0000 7243 0000 0072  pathsr0...rC...r
+000011e0: 3100 0000 da0a 6765 745f 7374 6174 7573  1.....get_status
+000011f0: 4400 0000 735e 0000 0000 0d08 060c 0c0e  D...s^..........
+00001200: 0202 0106 ff0c 040e 010e 010e 020c 0114  ................
+00001210: 0208 0118 0206 0108 0108 0108 020c 0102  ................
+00001220: 0106 ff06 0304 0110 010a 0208 0110 0112  ................
+00001230: 020c 0116 020e 010a 0102 ff06 040c 010e  ................
+00001240: 0106 0110 0108 010c 011a 0202 0102 0102  ................
+00001250: 0102 0102 0102 fb72 5b00 0000 2902 da04  .......r[...)...
+00001260: 6e61 6d65 7236 0000 0063 0100 0000 0000  namer6...c......
+00001270: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+00001280: 0000 7310 0000 0074 007c 0064 0167 0164  ..s....t.|.d.g.d
+00001290: 0264 038d 0353 0029 047a 3252 6574 7572  .d...S.).z2Retur
+000012a0: 6e20 6120 7661 6c69 6420 706c 616e 206e  n a valid plan n
+000012b0: 616d 6520 6261 7365 6420 6f6e 2074 6865  ame based on the
+000012c0: 2070 6173 7365 6420 6e61 6d65 2eda 012e   passed name....
+000012d0: 4629 02da 0d69 6e76 616c 6964 5f63 6861  F)...invalid_cha
+000012e0: 7273 da09 6c6f 7765 7263 6173 6572 1b00  rs..lowercaser..
+000012f0: 0000 a901 725c 0000 0072 3000 0000 7230  ....r\...r0...r0
+00001300: 0000 0072 3100 0000 da13 6765 745f 7661  ...r1.....get_va
+00001310: 6c69 645f 706c 616e 5f6e 616d 659d 0000  lid_plan_name...
+00001320: 0073 0200 0000 0002 7261 0000 0063 0100  .s......ra...c..
+00001330: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001340: 0000 4300 0000 7308 0000 0074 007c 0083  ..C...s....t.|..
+00001350: 0153 0029 017a 3752 6574 7572 6e20 6120  .S.).z7Return a 
+00001360: 7661 6c69 6420 7061 7261 6d65 7465 7220  valid parameter 
+00001370: 6e61 6d65 2062 6173 6564 206f 6e20 7468  name based on th
+00001380: 6520 7061 7373 6564 206e 616d 652e 2901  e passed name.).
+00001390: 7261 0000 0072 6000 0000 7230 0000 0072  ra...r`...r0...r
+000013a0: 3000 0000 7231 0000 00da 1867 6574 5f76  0...r1.....get_v
+000013b0: 616c 6964 5f70 6172 616d 6574 6572 5f6e  alid_parameter_n
+000013c0: 616d 65a2 0000 0073 0200 0000 0002 7262  ame....s......rb
+000013d0: 0000 00da 1061 6374 6976 6974 795f 6761  .....activity_ga
+000013e0: 7465 7761 79da 0c70 6c61 6e5f 6761 7465  teway..plan_gate
+000013f0: 7761 7929 0372 6300 0000 7264 0000 0072  way).rc...rd...r
+00001400: 3600 0000 630e 0000 0000 0000 0000 0000  6...c...........
+00001410: 0025 0000 000c 0000 0003 0000 0073 a604  .%...........s..
+00001420: 0000 7c00 724e 7400 7c00 8301 7d0e 7c00  ..|.rNt.|...}.|.
+00001430: 7c0e 6b03 722c 7401 a002 6401 7c00 9b00  |.k.r,t...d.|...
+00001440: 6402 7c0e 9b00 6403 9d05 a101 8201 7c0d  d.|...d.......|.
+00001450: a003 a100 7d0f 7c00 7c0f 7600 724e 7401  ....}.|.|.v.rNt.
+00001460: a004 6404 7c00 9b00 6405 9d03 a101 8201  ..d.|...d.......
+00001470: 7c08 7256 7c04 6e06 7405 6a06 6a07 7d10  |.rV|.n.t.j.j.}.
+00001480: 7408 7c10 6406 6407 8d02 7d11 7c07 7272  t.|.d.d...}.|.rr
+00001490: 7c03 6e06 7405 6a06 6a07 7d10 7408 7c10  |.n.t.j.j.}.t.|.
+000014a0: 6408 6407 8d02 7d12 7c11 a009 7c12 a101  d.d...}.|...|...
+000014b0: 0100 7408 7c03 6406 6407 8d02 7d13 7c13  ..t.|.d.d...}.|.
+000014c0: 72c6 7401 a00a 6409 740b 6a0c 640a a00d  r.t...d.t.j.d...
+000014d0: 7c13 a00e a100 a101 640b 640c 8d02 1700  |.......d.d.....
+000014e0: 640d 1700 a101 8201 7408 7c04 6408 6407  d.......t.|.d.d.
+000014f0: 8d02 7d13 7c13 72fc 7401 a00a 640e 740b  ..}.|.r.t...d.t.
+00001500: 6a0c 640a a00d 7c13 a00e a100 a101 640b  j.d...|.......d.
+00001510: 640c 8d02 1700 640d 1700 a101 8201 640f  d.....d.......d.
+00001520: 7d14 640f 7d15 7a34 740f 6410 6411 8302  }.d.}.z4t.d.d...
+00001530: 8f14 0100 6412 7d16 5700 640f 0400 0400  ....d.}.W.d.....
+00001540: 8303 0100 6e12 3100 9001 732c 3000 0100  ....n.1...s,0...
+00001550: 0100 0100 5900 0100 5700 6e18 0400 7410  ....Y...W.n...t.
+00001560: 9001 7950 0100 0100 0100 6413 7d16 5900  ..yP......d.}.Y.
+00001570: 6e02 3000 9003 7a12 6414 7c11 7600 7d17  n.0...z.d.|.v.}.
+00001580: 6415 7c11 7600 7d18 7c16 9001 72a4 7c17  d.|.v.}.|...r.|.
+00001590: 9001 7288 740f 6410 6411 8302 7d14 7411  ..r.t.d.d...}.t.
+000015a0: 6a12 7d19 7c14 7411 5f12 7c18 9001 72a4  j.}.|.t._.|...r.
+000015b0: 740f 6410 6411 8302 7d15 7411 6a13 7d1a  t.d.d...}.t.j.}.
+000015c0: 7c15 7411 5f13 7414 7405 6a15 8301 8900  |.t._.t.t.j.....
+000015d0: 6416 6417 8400 7d1b 7c1b 7c03 6418 8302  d.d...}.|.|.d...
+000015e0: 7d03 7c1b 7c04 6419 8302 7d04 7c1b 7c05  }.|.|.d...}.|.|.
+000015f0: 641a 8302 7d05 7416 6600 7c0a 7c03 7c04  d...}.t.f.|.|.|.
+00001600: 7c05 7417 a018 a100 8800 7c07 7c08 7c09  |.t.......|.|.|.
+00001610: 641b 9c09 8700 6601 641c 641d 8408 7c11  d.....f.d.d...|.
+00001620: a019 a100 4400 8301 a401 8e01 7d1c 7c1c  ....D.......}.|.
+00001630: 6a1a 7c06 641e 8d01 9001 8f8c 7d1d 741b  j.|.d.......}.t.
+00001640: 8300 9002 724c 641f 6420 8400 7c1d a01c  ....rLd.d ..|...
+00001650: 7405 6a15 a101 4400 8301 7d1e 741d 7405  t.j...D...}.t.t.
+00001660: 6a06 6701 7c1e a201 5200 8e00 0100 7c16  j.g.|...R.....|.
+00001670: 9002 72da 7c17 9002 725e 7c19 7411 5f12  ..r.|...r^|.t._.
+00001680: 7c18 9002 726a 7c1a 7411 5f13 6414 7c11  |...rj|.t._.d.|.
+00001690: 7601 9002 72a2 7a0e 7411 6a12 a01e a100  v...r.z.t.j.....
+000016a0: 0100 5700 6e14 0400 741f 9002 7996 0100  ..W.n...t...y...
+000016b0: 0100 0100 5900 6e0c 3000 7411 6a12 7c11  ....Y.n.0.t.j.|.
+000016c0: 6414 3c00 6415 7c11 7601 9002 72da 7a0e  d.<.d.|.v...r.z.
+000016d0: 7411 6a13 a01e a100 0100 5700 6e14 0400  t.j.......W.n...
+000016e0: 741f 9002 79ce 0100 0100 0100 5900 6e0c  t...y.......Y.n.
+000016f0: 3000 7411 6a13 7c11 6415 3c00 7420 8300  0.t.j.|.d.<.t ..
+00001700: 7d1f 7a2c 7421 7c1c 6a22 6601 6421 7417  }.z,t!|.j"f.d!t.
+00001710: a018 a100 6901 6422 641d 8400 7c11 a023  ....i.d"d...|..#
+00001720: a100 4400 8301 a401 8e01 7d20 5700 6e32  ..D.......} W.n2
+00001730: 0400 7424 9003 793e 0100 0100 0100 6423  ..t$..y>......d#
+00001740: a00d 7c1c 6a25 a101 7d21 7401 a002 6424  ..|.j%..}!t...d$
+00001750: 7c21 9b00 6425 9d03 a101 8201 5900 6e02  |!..d%......Y.n.
+00001760: 3000 7420 8300 7d22 7411 6a12 a026 a100  0.t ..}"t.j..&..
+00001770: 0100 7411 6a13 a026 a100 0100 7c16 9003  ..t.j..&....|...
+00001780: 7278 7c17 9003 726c 7c14 7411 5f12 7c18  rx|...rl|.t._.|.
+00001790: 9003 7278 7c15 7411 5f13 7c20 7c09 9003  ..rx|.t._.| |...
+000017a0: 7084 6426 6801 7601 9003 7298 7401 6a27  p.d&h.v...r.t.j'
+000017b0: 7c20 7c09 6427 8d02 8201 5700 640f 0400  | |.d'....W.d...
+000017c0: 0400 8303 0100 6e12 3100 9003 73ae 3000  ......n.1...s.0.
+000017d0: 0100 0100 0100 5900 0100 7c0b 9003 73d0  ......Y...|...s.
+000017e0: 7428 7429 742a 7405 6a06 8301 8302 6701  t(t)t*t.j.....g.
+000017f0: 7d0b 7c1d 6a2b 7c00 7c01 7c02 7c0b 7c1f  }.|.j+|.|.|.|.|.
+00001800: 6428 8d05 7d23 742c 6a2d 7c23 7405 6a06  d(..}#t,j-|#t.j.
+00001810: 7c1f 7c22 7c1d 6a2e 6429 8d05 7d24 7c0c  |.|"|.j.d)..}$|.
+00001820: a02f 7c24 a101 0100 7430 a02d 7c23 a101  ./|$....t0.-|#..
+00001830: 5700 7c14 9004 722c 7c14 a026 a100 0100  W.|...r,|..&....
+00001840: 7c19 7411 5f12 7c14 a031 a100 0100 7c15  |.t._.|..1....|.
+00001850: 9004 7248 7c15 a026 a100 0100 7c1a 7411  ..rH|..&....|.t.
+00001860: 5f13 7c15 a031 a100 0100 5300 7c15 9004  _.|..1....S.|...
+00001870: 72a2 7c15 a026 a100 0100 7c1a 7411 5f13  r.|..&....|.t._.
+00001880: 7c15 a031 a100 0100 6e3a 7c14 9004 7284  |..1....n:|...r.
+00001890: 7c14 a026 a100 0100 7c19 7411 5f12 7c14  |..&....|.t._.|.
+000018a0: a031 a100 0100 7c15 9004 72a0 7c15 a026  .1....|...r.|..&
+000018b0: a100 0100 7c1a 7411 5f13 7c15 a031 a100  ....|.t._.|..1..
+000018c0: 0100 3000 640f 5300 292a 7a1b 5275 6e20  ..0.d.S.)*z.Run 
+000018d0: 636f 6d6d 616e 6420 6c69 6e65 2061 7267  command line arg
+000018e0: 756d 656e 7473 2e7a 0f49 6e76 616c 6964  uments.z.Invalid
+000018f0: 206e 616d 653a 2027 7a0a 2720 2848 696e   name: 'z.' (Hin
+00001900: 743a 2027 7a0c 2720 6973 2076 616c 6964  t: 'z.' is valid
+00001910: 292e 7a23 4475 706c 6963 6174 6520 776f  ).z#Duplicate wo
+00001920: 726b 666c 6f77 206e 616d 653a 2057 6f72  rkflow name: Wor
+00001930: 6b66 6c6f 7720 277a 1127 2061 6c72 6561  kflow 'z.' alrea
+00001940: 6479 2065 7869 7374 732e 2902 da06 7374  dy exists.)...st
+00001950: 646f 7574 da06 7374 6465 7272 2901 da07  dout..stderr)...
+00001960: 7374 7265 616d 7329 01da 0573 7464 696e  streams)...stdin
+00001970: 7a36 4578 706c 6963 6974 2069 6e70 7574  z6Explicit input
+00001980: 2066 696c 6520 6361 6e6e 6f74 2062 6520   file cannot be 
+00001990: 7573 6564 2061 7320 7374 646f 7574 2f73  used as stdout/s
+000019a0: 7464 6572 723a 0a09 7a02 0a09 da06 7965  tderr:..z.....ye
+000019b0: 6c6c 6f77 2901 da02 6667 da01 0a7a 2f45  llow)...fg...z/E
+000019c0: 7870 6c69 6369 7420 6f75 7470 7574 2066  xplicit output f
+000019d0: 696c 6520 6361 6e6e 6f74 2062 6520 7573  ile cannot be us
+000019e0: 6564 2061 7320 7374 6469 6e3a 0a09 4e7a  ed as stdin:..Nz
+000019f0: 082f 6465 762f 7474 79da 0177 5446 7265  ./dev/tty..wTFre
+00001a00: 0000 0072 6600 0000 6302 0000 0000 0000  ...rf...c.......
+00001a10: 0000 0000 0005 0000 0005 0000 0053 0000  .............S..
+00001a20: 0073 8400 0000 6401 6402 8400 7c00 4400  .s....d.d...|.D.
+00001a30: 8301 7d02 7c02 7316 7c02 5300 7400 7c02  ..}.|.s.|.S.t.|.
+00001a40: 8e00 5c02 7d03 7d04 7401 7c03 8301 7401  ..\.}.}.t.|...t.
+00001a50: 7402 7c03 8301 8301 6b03 7248 7403 a004  t.|.....k.rHt...
+00001a60: 6403 7c01 9b00 6404 9d03 a101 8201 6405  d.|...d.......d.
+00001a70: 6402 8400 7c04 4400 8301 7d04 7c04 7280  d...|.D...}.|.r.
+00001a80: 7401 7c04 8301 7401 7402 7c04 8301 8301  t.|...t.t.|.....
+00001a90: 6b03 7280 7403 a004 6403 7c01 9b00 6406  k.r.t...d.|...d.
+00001aa0: 9d03 a101 8201 7c02 5300 2907 4e63 0100  ......|.S.).Nc..
+00001ab0: 0000 0000 0000 0000 0000 0200 0000 0700  ................
+00001ac0: 0000 5300 0000 7338 0000 0067 007c 005d  ..S...s8...g.|.]
+00001ad0: 307d 0164 007c 0176 0072 2c74 007c 016a  0}.d.|.v.r,t.|.j
+00001ae0: 0164 0064 0164 028d 0264 0364 0364 0485  .d.d.d...d.d.d..
+00001af0: 0319 0083 016e 067c 0164 0366 0291 0271  .....n.|.d.f...q
+00001b00: 0453 0029 05da 013d e901 0000 0029 01da  .S.)...=.....)..
+00001b10: 086d 6178 7370 6c69 744e e9ff ffff ff29  .maxsplitN.....)
+00001b20: 02da 0574 7570 6c65 da05 7370 6c69 7429  ...tuple..split)
+00001b30: 0272 3a00 0000 724a 0000 0072 3000 0000  .r:...rJ...r0...
+00001b40: 7230 0000 0072 3100 0000 724f 0000 00f8  r0...r1...rO....
+00001b50: 0000 0072 4c00 0000 7a47 7275 6e5f 636f  ...rL...zGrun_co
+00001b60: 6d6d 616e 645f 6c69 6e65 2e3c 6c6f 6361  mmand_line.<loca
+00001b70: 6c73 3e2e 7061 7273 655f 6578 706c 6963  ls>.parse_explic
+00001b80: 6974 5f64 6566 696e 6974 696f 6e2e 3c6c  it_definition.<l
+00001b90: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00001ba0: 3e7a 2143 616e 6e6f 7420 7370 6563 6966  >z!Cannot specif
+00001bb0: 7920 7468 6520 7361 6d65 2065 7870 6c69  y the same expli
+00001bc0: 6369 7420 7a0d 2076 616c 7565 2074 7769  cit z. value twi
+00001bd0: 6365 2e63 0100 0000 0000 0000 0000 0000  ce.c............
+00001be0: 0200 0000 0300 0000 5300 0000 7314 0000  ........S...s...
+00001bf0: 0067 007c 005d 0c7d 017c 0172 047c 0191  .g.|.].}.|.r.|..
+00001c00: 0271 0453 0072 3000 0000 7230 0000 0029  .q.S.r0...r0...)
+00001c10: 0272 3a00 0000 da01 6e72 3000 0000 7230  .r:.....nr0...r0
+00001c20: 0000 0072 3100 0000 724f 0000 0002 0100  ...r1...rO......
+00001c30: 0072 4c00 0000 7a0c 206e 616d 6520 7477  .rL...z. name tw
+00001c40: 6963 652e 2905 da03 7a69 7072 5500 0000  ice.)...ziprU...
+00001c50: 7253 0000 0072 1000 0000 da0a 5573 6167  rS...r......Usag
+00001c60: 6545 7272 6f72 2905 da07 656e 7472 6965  eError)...entrie
+00001c70: 73da 0474 7970 65da 0672 6573 756c 74da  s..type..result.
+00001c80: 0676 616c 7565 73da 056e 616d 6573 7230  .values..namesr0
+00001c90: 0000 0072 3000 0000 7231 0000 00da 1970  ...r0...r1.....p
+00001ca0: 6172 7365 5f65 7870 6c69 6369 745f 6465  arse_explicit_de
+00001cb0: 6669 6e69 7469 6f6e f700 0000 7314 0000  finition....s...
+00001cc0: 0000 010e 0204 0104 020c 0214 0112 020e  ................
+00001cd0: 0218 0112 027a 3372 756e 5f63 6f6d 6d61  .....z3run_comma
+00001ce0: 6e64 5f6c 696e 652e 3c6c 6f63 616c 733e  nd_line.<locals>
+00001cf0: 2e70 6172 7365 5f65 7870 6c69 6369 745f  .parse_explicit_
+00001d00: 6465 6669 6e69 7469 6f6e da05 696e 7075  definition..inpu
+00001d10: 74da 066f 7574 7075 74da 0570 6172 616d  t..output..param
+00001d20: 2909 da0c 636f 6d6d 616e 645f 6c69 6e65  )...command_line
+00001d30: da0f 6578 706c 6963 6974 5f69 6e70 7574  ..explicit_input
+00001d40: 73da 1065 7870 6c69 6369 745f 6f75 7470  s..explicit_outp
+00001d50: 7574 73da 1365 7870 6c69 6369 745f 7061  uts..explicit_pa
+00001d60: 7261 6d65 7465 7273 da09 6469 7265 6374  rameters..direct
+00001d70: 6f72 79da 0b77 6f72 6b69 6e67 5f64 6972  ory..working_dir
+00001d80: da12 6e6f 5f69 6e70 7574 5f64 6574 6563  ..no_input_detec
+00001d90: 7469 6f6e da13 6e6f 5f6f 7574 7075 745f  tion..no_output_
+00001da0: 6465 7465 6374 696f 6eda 0d73 7563 6365  detection..succe
+00001db0: 7373 5f63 6f64 6573 6301 0000 0000 0000  ss_codesc.......
+00001dc0: 0000 0000 0003 0000 0007 0000 0013 0000  ................
+00001dd0: 0073 2000 0000 6900 7c00 5d18 5c02 7d01  .s ...i.|.].\.}.
+00001de0: 7d02 7c01 7400 6a01 a002 7c02 8800 a102  }.|.t.j...|.....
+00001df0: 9302 7104 5300 7230 0000 0029 03da 026f  ..q.S.r0...)...o
+00001e00: 7372 3800 0000 da07 7265 6c70 6174 6829  sr8.....relpath)
+00001e10: 0372 3a00 0000 725c 0000 0072 3800 0000  .r:...r\...r8...
+00001e20: a901 7284 0000 0072 3000 0000 7231 0000  ..r....r0...r1..
+00001e30: 00da 0a3c 6469 6374 636f 6d70 3e17 0100  ...<dictcomp>...
+00001e40: 0072 4c00 0000 7a24 7275 6e5f 636f 6d6d  .rL...z$run_comm
+00001e50: 616e 645f 6c69 6e65 2e3c 6c6f 6361 6c73  and_line.<locals
+00001e60: 3e2e 3c64 6963 7463 6f6d 703e 2901 da09  >.<dictcomp>)...
+00001e70: 6e6f 5f6f 7574 7075 7463 0100 0000 0000  no_outputc......
+00001e80: 0000 0000 0000 0300 0000 0300 0000 7300  ..............s.
+00001e90: 0000 7316 0000 007c 005d 0e5c 027d 017d  ..s....|.].\.}.}
+00001ea0: 027c 0256 0001 0071 0264 0053 0072 3700  .|.V...q.d.S.r7.
+00001eb0: 0000 7230 0000 0029 0372 3a00 0000 7251  ..r0...).r:...rQ
+00001ec0: 0000 0072 3800 0000 7230 0000 0072 3000  ...r8...r0...r0.
+00001ed0: 0000 7231 0000 0072 3c00 0000 1d01 0000  ..r1...r<.......
+00001ee0: 724c 0000 007a 2372 756e 5f63 6f6d 6d61  rL...z#run_comma
+00001ef0: 6e64 5f6c 696e 652e 3c6c 6f63 616c 733e  nd_line.<locals>
+00001f00: 2e3c 6765 6e65 7870 723e 724d 0000 0063  .<genexpr>rM...c
+00001f10: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001f20: 0600 0000 5300 0000 7318 0000 0069 007c  ....S...s....i.|
+00001f30: 005d 107d 017c 0174 0074 017c 0183 0293  .].}.|.t.t.|....
+00001f40: 0271 0453 0072 3000 0000 2902 da07 6765  .q.S.r0...)...ge
+00001f50: 7461 7474 72da 0373 7973 2902 723a 0000  tattr..sys).r:..
+00001f60: 00da 036b 6579 7230 0000 0072 3000 0000  ...keyr0...r0...
+00001f70: 7231 0000 0072 8b00 0000 3d01 0000 724c  r1...r....=...rL
+00001f80: 0000 00da 0120 7a18 4361 6e6e 6f74 2065  ..... z.Cannot e
+00001f90: 7865 6375 7465 2063 6f6d 6d61 6e64 2027  xecute command '
+00001fa0: 7a58 273a 2054 6869 7320 6973 206c 696b  zX': This is lik
+00001fb0: 656c 7920 6265 6361 7573 6520 7468 6520  ely because the 
+00001fc0: 6578 6563 7574 6162 6c65 2064 6f65 736e  executable doesn
+00001fd0: 2774 2065 7869 7374 206f 7220 6861 7320  't exist or has 
+00001fe0: 7468 6520 7772 6f6e 6720 7065 726d 6973  the wrong permis
+00001ff0: 7369 6f6e 7320 7365 742e 7201 0000 0029  sions set.r....)
+00002000: 0172 8700 0000 2905 725c 0000 00da 0b64  .r....).r\.....d
+00002010: 6573 6372 6970 7469 6f6e da08 6b65 7977  escription..keyw
+00002020: 6f72 6473 da08 6372 6561 746f 7273 da0c  ords..creators..
+00002030: 6461 7465 5f63 7265 6174 6564 2905 da04  date_created)...
+00002040: 706c 616e 7246 0000 00da 0f73 7461 7274  planrF.....start
+00002050: 6564 5f61 745f 7469 6d65 da0d 656e 6465  ed_at_time..ende
+00002060: 645f 6174 5f74 696d 65da 0b61 6e6e 6f74  d_at_time..annot
+00002070: 6174 696f 6e73 2932 7261 0000 0072 1000  ations)2ra...r..
+00002080: 0000 da0e 5061 7261 6d65 7465 7245 7272  ....ParameterErr
+00002090: 6f72 da19 6765 745f 6e65 7765 7374 5f70  or..get_newest_p
+000020a0: 6c61 6e73 5f62 795f 6e61 6d65 73da 1a44  lans_by_names..D
+000020b0: 7570 6c69 6361 7465 576f 726b 666c 6f77  uplicateWorkflow
+000020c0: 4e61 6d65 4572 726f 7272 2100 0000 7246  NameErrorr!...rF
+000020d0: 0000 00da 0961 6c6c 5f66 696c 6573 7212  .....all_filesr.
+000020e0: 0000 00da 0675 7064 6174 6572 7500 0000  .....updateru...
+000020f0: da05 636c 6963 6bda 0573 7479 6c65 da04  ..click..style..
+00002100: 6a6f 696e 7279 0000 00da 046f 7065 6eda  joinry.....open.
+00002110: 074f 5345 7272 6f72 728e 0000 0072 6500  .OSErrorr....re.
+00002120: 0000 7266 0000 0072 2e00 0000 7238 0000  ..rf...r....r8..
+00002130: 0072 2000 0000 7288 0000 00da 0667 6574  .r ...r......get
+00002140: 6377 64da 0569 7465 6d73 5a05 7761 7463  cwd..itemsZ.watc
+00002150: 6872 1500 0000 5a10 6974 6572 5f69 6e70  hr....Z.iter_inp
+00002160: 7574 5f66 696c 6573 7216 0000 00da 0666  ut_filesr......f
+00002170: 696c 656e 6f72 0300 0000 7217 0000 0072  ilenor....r....r
+00002180: 0500 0000 727f 0000 00da 046b 6579 73da  ....r......keys.
+00002190: 1146 696c 654e 6f74 466f 756e 6445 7272  .FileNotFoundErr
+000021a0: 6f72 da0c 6261 7365 5f63 6f6d 6d61 6e64  or..base_command
+000021b0: da05 666c 7573 68da 1249 6e76 616c 6964  ..flush..Invalid
+000021c0: 5375 6363 6573 7343 6f64 6572 0c00 0000  SuccessCoder....
+000021d0: 7223 0000 0072 1800 0000 da07 746f 5f70  r#...r......to_p
+000021e0: 6c61 6e72 2200 0000 da09 6672 6f6d 5f70  lanr".....from_p
+000021f0: 6c61 6e72 9800 0000 7254 0000 0072 0f00  lanr....rT...r..
+00002200: 0000 da05 636c 6f73 6529 2572 5c00 0000  ....close)%r\...
+00002210: 7291 0000 00da 076b 6579 776f 7264 7280  r......keywordr.
+00002220: 0000 0072 8100 0000 7282 0000 0072 8c00  ...r....r....r..
+00002230: 0000 7285 0000 0072 8600 0000 7287 0000  ..r....r....r...
+00002240: 0072 7f00 0000 7293 0000 0072 6300 0000  .r....r....rc...
+00002250: 7264 0000 00da 0a76 616c 6964 5f6e 616d  rd.....valid_nam
+00002260: 65da 0977 6f72 6b66 6c6f 7773 7234 0000  e..workflowsr4..
+00002270: 005a 0a6d 6170 7065 645f 7374 645a 0d6d  .Z.mapped_stdZ.m
+00002280: 6170 7065 645f 7374 645f 696e da07 696e  apped_std_in..in
+00002290: 7661 6c69 645a 0d73 7973 7465 6d5f 7374  validZ.system_st
+000022a0: 646f 7574 5a0d 7379 7374 656d 5f73 7464  doutZ.system_std
+000022b0: 6572 725a 0a74 7479 5f65 7869 7374 735a  errZ.tty_existsZ
+000022c0: 1173 7464 6f75 745f 7265 6469 7265 6374  .stdout_redirect
+000022d0: 6564 5a11 7374 6465 7272 5f72 6564 6972  edZ.stderr_redir
+000022e0: 6563 7465 645a 0a6f 6c64 5f73 7464 6f75  ectedZ.old_stdou
+000022f0: 745a 0a6f 6c64 5f73 7464 6572 7272 7b00  tZ.old_stderrr{.
+00002300: 0000 da07 6661 6374 6f72 79da 0474 6f6f  ....factory..too
+00002310: 6c5a 0670 6174 6873 5f72 9600 0000 da0b  lZ.paths_r......
+00002320: 7265 7475 726e 5f63 6f64 65da 0763 6f6d  return_code..com
+00002330: 6d61 6e64 7297 0000 0072 9500 0000 723e  mandr....r....r>
+00002340: 0000 0072 3000 0000 728a 0000 0072 3100  ...r0...r....r1.
+00002350: 0000 da10 7275 6e5f 636f 6d6d 616e 645f  ....run_command_
+00002360: 6c69 6e65 a700 0000 732e 0100 0000 1404  line....s.......
+00002370: 0108 0108 0118 0208 0108 0112 0210 010c  ................
+00002380: 0210 010c 010a 020c 0104 0104 0102 0116  ................
+00002390: ff02 0102 ff02 ff04 050c 0104 0104 0102  ................
+000023a0: 0116 ff02 0102 ff02 ff04 0504 0104 0402  ................
+000023b0: 010c 0128 010e 010a 0204 0108 0108 0206  ...(............
+000023c0: 0306 010a 0106 0106 0206 010a 0106 0106  ................
+000023d0: 020a 0208 120a 010a 010a 0204 0102 0102  ................
+000023e0: 0102 0102 0106 0102 0102 0102 0102 f704  ................
+000023f0: 0a14 f606 0c10 0208 0216 0112 0206 0206  ................
+00002400: 0106 0106 0106 020a 0102 010e 010e 0206  ................
+00002410: 020a 020a 0102 010e 010e 0206 020a 0206  ................
+00002420: 0202 0102 0104 ff04 0106 ff02 0110 ff0a  ................
+00002430: 030e 010c 0104 010a ff0a 0506 020a 010a  ................
+00002440: 0206 0206 0106 0106 0106 0212 012e 0206  ................
+00002450: 0112 0204 010a ff06 0304 0102 0104 0102  ................
+00002460: 0102 0104 fb06 070a 020a 0306 0108 0106  ................
+00002470: 0108 0106 0108 0106 0108 f602 0300 0100  ................
+00002480: 0100 0100 0106 0108 0106 010a f906 0108  ................
+00002490: 0106 0108 0106 0108 0106 0172 b600 0000  ...........r....
+000024a0: 2902 4e46 2945 722d 0000 0072 8800 0000  ).NF)Er-...r....
+000024b0: 728e 0000 00da 0b63 6f6c 6c65 6374 696f  r......collectio
+000024c0: 6e73 7202 0000 00da 0269 6f72 0300 0000  nsr......ior....
+000024d0: da07 7061 7468 6c69 6272 0400 0000 da0a  ..pathlibr......
+000024e0: 7375 6270 726f 6365 7373 7205 0000 00da  subprocessr.....
+000024f0: 0674 7970 696e 6772 0600 0000 7207 0000  .typingr....r...
+00002500: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00002510: 720b 0000 0072 0c00 0000 729e 0000 00da  r....r....r.....
+00002520: 0870 7964 616e 7469 6372 0d00 0000 da1d  .pydanticr......
+00002530: 7265 6e6b 752e 636f 6d6d 616e 642e 636f  renku.command.co
+00002540: 6d6d 616e 645f 6275 696c 6465 7272 0e00  mmand_builderr..
+00002550: 0000 da1d 7265 6e6b 752e 636f 6d6d 616e  ....renku.comman
+00002560: 642e 7669 6577 5f6d 6f64 656c 2e70 6c61  d.view_model.pla
+00002570: 6e72 0f00 0000 da0a 7265 6e6b 752e 636f  nr......renku.co
+00002580: 7265 7210 0000 00da 1172 656e 6b75 2e63  rer......renku.c
+00002590: 6f72 652e 636f 6e66 6967 7211 0000 005a  ore.configr....Z
+000025a0: 0e72 656e 6b75 2e63 6f72 652e 6769 7472  .renku.core.gitr
+000025b0: 1200 0000 da25 7265 6e6b 752e 636f 7265  .....%renku.core
+000025c0: 2e69 6e74 6572 6661 6365 2e61 6374 6976  .interface.activ
+000025d0: 6974 795f 6761 7465 7761 7972 1300 0000  ity_gatewayr....
+000025e0: da21 7265 6e6b 752e 636f 7265 2e69 6e74  .!renku.core.int
+000025f0: 6572 6661 6365 2e70 6c61 6e5f 6761 7465  erface.plan_gate
+00002600: 7761 7972 1400 0000 da12 7265 6e6b 752e  wayr......renku.
+00002610: 636f 7265 2e73 746f 7261 6765 7215 0000  core.storager...
+00002620: 0072 1600 0000 da1c 7265 6e6b 752e 636f  .r......renku.co
+00002630: 7265 2e75 7469 6c2e 6461 7465 7469 6d65  re.util.datetime
+00002640: 3836 3031 7217 0000 00da 1372 656e 6b75  8601r......renku
+00002650: 2e63 6f72 652e 7574 696c 2e67 6974 7218  .core.util.gitr.
+00002660: 0000 00da 1272 656e 6b75 2e63 6f72 652e  .....renku.core.
+00002670: 7574 696c 2e6f 7372 1900 0000 721a 0000  util.osr....r...
+00002680: 00da 1472 656e 6b75 2e63 6f72 652e 7574  ...renku.core.ut
+00002690: 696c 2e75 726c 7372 1c00 0000 da1c 7265  il.urlsr......re
+000026a0: 6e6b 752e 636f 7265 2e77 6f72 6b66 6c6f  nku.core.workflo
+000026b0: 772e 6163 7469 7669 7479 721d 0000 0072  w.activityr....r
+000026c0: 1e00 0000 721f 0000 005a 2072 656e 6b75  ....r....Z renku
+000026d0: 2e63 6f72 652e 776f 726b 666c 6f77 2e70  .core.workflow.p
+000026e0: 6c61 6e5f 6661 6374 6f72 7972 2000 0000  lan_factoryr ...
+000026f0: da22 7265 6e6b 752e 646f 6d61 696e 5f6d  ."renku.domain_m
+00002700: 6f64 656c 2e70 726f 6a65 6374 5f63 6f6e  odel.project_con
+00002710: 7465 7874 7221 0000 00da 2672 656e 6b75  textr!....&renku
+00002720: 2e64 6f6d 6169 6e5f 6d6f 6465 6c2e 7072  .domain_model.pr
+00002730: 6f76 656e 616e 6365 2e61 6374 6976 6974  ovenance.activit
+00002740: 7972 2200 0000 da23 7265 6e6b 752e 646f  yr"....#renku.do
+00002750: 6d61 696e 5f6d 6f64 656c 2e70 726f 7665  main_model.prove
+00002760: 6e61 6e63 652e 6167 656e 7472 2300 0000  nance.agentr#...
+00002770: 7224 0000 00da 0464 6963 7472 2e00 0000  r$.....dictr....
+00002780: da04 626f 6f6c 725b 0000 0072 6100 0000  ..boolr[...ra...
+00002790: 7262 0000 00da 0a61 7574 6f70 6172 616d  rb.....autoparam
+000027a0: 7372 b600 0000 7230 0000 0072 3000 0000  sr....r0...r0...
+000027b0: 7230 0000 0072 3100 0000 da08 3c6d 6f64  r0...r1.....<mod
+000027c0: 756c 653e 1100 0000 734a 0000 0004 0208  ule>....sJ......
+000027d0: 0108 010c 010c 010c 010c 0124 0208 010c  ...........$....
+000027e0: 020c 010c 010c 010c 010c 010c 010c 0110  ................
+000027f0: 010c 010c 0110 010c 0114 050c 010c 010c  ................
+00002800: 010c 0310 0f0e 0126 5810 0510 050a 010e  .......&X.......
+00002810: 0e02 0102 0102 f1                        .......
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/__pycache__/types.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/__pycache__/types.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1681 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9106 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 9106 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 4700 6405 6406  m.Z.m.Z...G.d.d.
 00000060: 8400 6406 8302 5a08 4700 6407 6408 8400  ..d...Z.G.d.d...
 00000070: 6408 6508 8303 5a09 4700 6409 640a 8400  d.e...Z.G.d.d...
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/__pycache__/value_resolution.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 8335 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8f20 0000  a........w.d. ..
+00000000: 610d 0d0a 0000 0000 195e 9464 8f20 0000  a........^.d. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/__pycache__/workflow_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5089 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 e113 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 e113 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0173 3401 0000 6400  .....@...s4...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6403 6c0a 5a0b 6401  m.Z...d.d.l.Z.d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 6401 6407 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/activity.py` & `renku-2.6.0rc1/renku/core/workflow/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/converters/__init__.py` & `renku-2.6.0rc1/renku/core/workflow/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/cwl.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 17937 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 1146 0000  a........w.d.F..
+00000000: 610d 0d0a 0000 0000 195e 9464 1146 0000  a........^.d.F..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6405 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/converters/__pycache__/renku.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5142 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 1614 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 1614 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/converters/cwl.py` & `renku-2.6.0rc1/renku/core/workflow/converters/cwl.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/converters/renku.py` & `renku-2.6.0rc1/renku/core/workflow/converters/renku.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/execute.py` & `renku-2.6.0rc1/renku/core/workflow/execute.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/model/__init__.py` & `renku-2.6.0rc1/renku/core/workflow/model/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/model/__pycache__/concrete_execution_graph.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8219 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 8219 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6405 6c0a 5a0b 6401 6406 6c0c  ..d.d.l.Z.d.d.l.
 00000070: 6d0d 5a0d 0100 6401 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/model/__pycache__/workflow_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 37866 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 ea93 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 ea93 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 1802 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6404 6c04 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c05 6d06 5a06 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/model/concrete_execution_graph.py` & `renku-2.6.0rc1/renku/core/workflow/model/concrete_execution_graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/model/workflow_file.py` & `renku-2.6.0rc1/renku/core/workflow/model/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/parser/__init__.py` & `renku-2.6.0rc1/renku/core/workflow/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/parser/__pycache__/renku.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 10631 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8729 0000  a........w.d.)..
+00000000: 610d 0d0a 0000 0000 195e 9464 8729 0000  a........^.d.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 3e01 0000 6400  .....@...s>...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6405 6c0e 6d0f 5a0f 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/parser/renku.py` & `renku-2.6.0rc1/renku/core/workflow/parser/renku.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/plan.py` & `renku-2.6.0rc1/renku/core/workflow/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/plan_factory.py` & `renku-2.6.0rc1/renku/core/workflow/plan_factory.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/providers/__init__.py` & `renku-2.6.0rc1/renku/core/workflow/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/cwltool.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5999 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6f17 0000  a........w.do...
+00000000: 610d 0d0a 0000 0000 195e 9464 6f17 0000  a........^.do...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 6401  d.l.m.Z.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6401 6406 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/local.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 af10 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 af10 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc` & `renku-2.6.0rc1/renku/core/workflow/providers/__pycache__/toil.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 13372 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 3c34 0000  a........w.d<4..
+00000000: 610d 0d0a 0000 0000 195e 9464 3c34 0000  a........^.d<4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 0a02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/providers/cwltool.py` & `renku-2.6.0rc1/renku/core/workflow/providers/cwltool.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/providers/local.py` & `renku-2.6.0rc1/renku/core/workflow/providers/local.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/providers/toil.py` & `renku-2.6.0rc1/renku/core/workflow/providers/toil.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/run.py` & `renku-2.6.0rc1/renku/core/workflow/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Running workflows logic."""
 
 import os
 import sys
 from collections import defaultdict
+from io import UnsupportedOperation
 from pathlib import Path
 from subprocess import call
 from typing import Dict, List, NamedTuple, Optional, Set, Union, cast
 
 import click
 from pydantic import validate_arguments
 
@@ -287,14 +288,32 @@
             if tty_exists:
                 # apply original output redirection
                 if stdout_redirected:
                     sys.stdout = old_stdout
                 if stderr_redirected:
                     sys.stderr = old_stderr
 
+                if "stdout" not in mapped_std:
+                    try:
+                        sys.stdout.fileno()
+                    except UnsupportedOperation:
+                        # Pytest capsys creates a pseudo device that doesn't have fileno and would fail if passed
+                        pass
+                    else:
+                        mapped_std["stdout"] = sys.stdout
+
+                if "stderr" not in mapped_std:
+                    try:
+                        sys.stderr.fileno()
+                    except UnsupportedOperation:
+                        # Pytest capsys creates a pseudo device that doesn't have fileno and would fail if passed
+                        pass
+                    else:
+                        mapped_std["stderr"] = sys.stderr
+
             started_at_time = local_now()
 
             try:
                 return_code = call(
                     factory.command_line, cwd=os.getcwd(), **{key: getattr(sys, key) for key in mapped_std.keys()}
                 )
             except FileNotFoundError:
```

### Comparing `renku-2.5.0rc3/renku/core/workflow/types.py` & `renku-2.6.0rc1/renku/core/workflow/types.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/update.py` & `renku-2.6.0rc1/renku/core/workflow/update.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/value_resolution.py` & `renku-2.6.0rc1/renku/core/workflow/value_resolution.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/core/workflow/workflow_file.py` & `renku-2.6.0rc1/renku/core/workflow/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/data/__init__.py` & `renku-2.6.0rc1/renku/data/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/data/gitignore.default` & `renku-2.6.0rc1/renku/data/gitignore.default`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/data/pre-commit.sh` & `renku-2.6.0rc1/renku/data/pre-commit.sh`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/data/shacl_shape.json` & `renku-2.6.0rc1/renku/data/shacl_shape.json`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/__init__.py` & `renku-2.6.0rc1/renku/domain_model/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 29611 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 ab73 0000  a........w.d.s..
+00000000: 610d 0d0a 0000 0000 195e 9464 ab73 0000  a........^.d.s..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4e02 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/__pycache__/dataset_provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1267 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 f304 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 f304 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6503 722c 6401  m.Z.m.Z...e.r,d.
 00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6501 6a07 8303 5a08 6402 5300  ..d.e.j...Z.d.S.
 00000070: 2907 7a12 4461 7461 7365 7420 7072 6f76  ).z.Dataset prov
```

### Comparing `renku-2.5.0rc3/renku/domain_model/__pycache__/datastructures.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/__pycache__/datastructures.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 c20a 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 c20a 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
 00000070: 650a 8303 5a0b 6402 5300 2908 7a32 4261  e...Z.d.S.).z2Ba
```

### Comparing `renku-2.5.0rc3/renku/domain_model/__pycache__/entity.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/__pycache__/entity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2499 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 c309 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 c309 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c0a 6d0b 5a0b 0100 6401 6406 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/__pycache__/enums.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/__pycache__/enums.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 cb03 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 cb03 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 4700  Z.d.d.l.m.Z...G.
 00000040: 6403 6404 8400 6404 6502 8303 5a03 6405  d.d...d.e...Z.d.
 00000050: 5300 2906 7a14 456e 756d 7320 7573 6564  S.).z.Enums used
 00000060: 2069 6e20 7265 6e6b 752e e900 0000 0029   in renku......)
 00000070: 01da 0445 6e75 6d63 0000 0000 0000 0000  ...Enumc........
```

### Comparing `renku-2.5.0rc3/renku/domain_model/__pycache__/project.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/__pycache__/project.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 8329 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8920 0000  a........w.d. ..
+00000000: 610d 0d0a 0000 0000 195e 9464 8920 0000  a........^.d. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0c 5a0c 6401 6407 6c0d  ..d.d.l.Z.d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/__pycache__/project_context.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/__pycache__/project_context.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 11817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 292e 0000  a........w.d)...
+00000000: 610d 0d0a 0000 0000 195e 9464 292e 0000  a........^.d)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1601 0000 5500  .....@...s....U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6402 6c03 5a03 6401 6403  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 6d05 5a05 0100 6401 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 0100 6401 6405 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000070: 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  Z.m.Z.m.Z.m.Z.m.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/__pycache__/session.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6871 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 d71a 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 d71a 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 b800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6401 6406 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/constant.py` & `renku-2.6.0rc1/renku/domain_model/constant.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/dataset.py` & `renku-2.6.0rc1/renku/domain_model/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/dataset_provider.py` & `renku-2.6.0rc1/renku/domain_model/dataset_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/datastructures.py` & `renku-2.6.0rc1/renku/domain_model/datastructures.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/entity.py` & `renku-2.6.0rc1/renku/domain_model/entity.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/enums.py` & `renku-2.6.0rc1/renku/domain_model/enums.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/git.py` & `renku-2.6.0rc1/renku/domain_model/git.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/project.py` & `renku-2.6.0rc1/renku/domain_model/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/project_context.py` & `renku-2.6.0rc1/renku/domain_model/project_context.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/provenance/__init__.py` & `renku-2.6.0rc1/renku/domain_model/provenance/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/activity.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 13200 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9033 0000  a........w.d.3..
+00000000: 610d 0d0a 0000 0000 195e 9464 9033 0000  a........^.d.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6401 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6406 6c0c 5a0c 6401 6407 6c0d  ..d.d.l.Z.d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/agent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5155 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 2314 0000  a........w.d#...
+00000000: 610d 0d0a 0000 0000 195e 9464 2314 0000  a........^.d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6401 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/annotation.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1268 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 f404 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 f404 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 8302 5a04 6402 5300 2906 7a27 5265 7072  ..Z.d.S.).z'Repr
 00000060: 6573 656e 7420 616e 2061 6e6e 6f74 6174  esent an annotat
 00000070: 696f 6e20 666f 7220 6120 776f 726b 666c  ion for a workfl
```

### Comparing `renku-2.5.0rc3/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/provenance/__pycache__/parameter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 fa05 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 fa05 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 8302 5a07 6407 5300 2908 7a34 436c 6173  ..Z.d.S.).z4Clas
 00000070: 7365 7320 666f 7220 7472 6163 6b69 6e67  ses for tracking
```

### Comparing `renku-2.5.0rc3/renku/domain_model/provenance/activity.py` & `renku-2.6.0rc1/renku/domain_model/provenance/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/provenance/agent.py` & `renku-2.6.0rc1/renku/domain_model/provenance/agent.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/provenance/annotation.py` & `renku-2.6.0rc1/renku/domain_model/provenance/annotation.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/provenance/parameter.py` & `renku-2.6.0rc1/renku/domain_model/provenance/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/session.py` & `renku-2.6.0rc1/renku/domain_model/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/sort.py` & `renku-2.6.0rc1/renku/domain_model/sort.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/template.py` & `renku-2.6.0rc1/renku/domain_model/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/__init__.py` & `renku-2.6.0rc1/renku/domain_model/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/composite_plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 15917 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 2d3e 0000  a........w.d->..
+00000000: 610d 0d0a 0000 0000 195e 9464 2d3e 0000  a........^.d->..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6406 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/parameter.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 18124 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 cc46 0000  a........w.d.F..
+00000000: 610d 0d0a 0000 0000 195e 9464 cc46 0000  a........^.d.F..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6401 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6401  m.Z.m.Z.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/plan.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 16602 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 da40 0000  a........w.d.@..
+00000000: 610d 0d0a 0000 0000 195e 9464 da40 0000  a........^.d.@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3201 0000 6400  .....@...s2...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1639 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6706 0000  a........w.dg...
+00000000: 610d 0d0a 0000 0000 195e 9464 6706 0000  a........^.dg...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6509 7250 6401 6406 6c0d 5a0e 4700  ..e.rPd.d.l.Z.G.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/workflow/__pycache__/workflow_file.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4660 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 3412 0000  a........w.d4...
+00000000: 610d 0d0a 0000 0000 195e 9464 3412 0000  a........^.d4...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6401 6407 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/composite_plan.py` & `renku-2.6.0rc1/renku/domain_model/workflow/composite_plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/converters/__init__.py` & `renku-2.6.0rc1/renku/domain_model/workflow/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc` & `renku-2.6.0rc1/renku/domain_model/workflow/converters/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1531 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 fb05 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 fb05 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 6d05 5a05 0100 6401  d.l.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0c 6d0d 5a0d 0100 4700 6407 6408  d.l.m.Z...G.d.d.
```

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/parameter.py` & `renku-2.6.0rc1/renku/domain_model/workflow/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/plan.py` & `renku-2.6.0rc1/renku/domain_model/workflow/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/provider.py` & `renku-2.6.0rc1/renku/domain_model/workflow/provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/domain_model/workflow/workflow_file.py` & `renku-2.6.0rc1/renku/domain_model/workflow/workflow_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/__init__.py` & `renku-2.6.0rc1/renku/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/__pycache__/database.cpython-39.pyc` & `renku-2.6.0rc1/renku/infrastructure/__pycache__/database.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 41333 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 75a1 0000  a........w.du...
+00000000: 610d 0d0a 0000 0000 195e 9464 75a1 0000  a........^.du...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2602 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/infrastructure/__pycache__/immutable.cpython-39.pyc` & `renku-2.6.0rc1/renku/infrastructure/__pycache__/immutable.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4969 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6913 0000  a........w.di...
+00000000: 610d 0d0a 0000 0000 195e 9464 6913 0000  a........^.di...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 8302 5a06  ..G.d.d...d...Z.
 00000060: 4700 6406 6407 8400 6407 6506 8303 5a07  G.d.d...d.e...Z.
 00000070: 4700 6408 6409 8400 6409 8302 5a08 6402  G.d.d...d...Z.d.
```

### Comparing `renku-2.5.0rc3/renku/infrastructure/__pycache__/persistent.cpython-39.pyc` & `renku-2.6.0rc1/renku/infrastructure/__pycache__/persistent.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 5a09 0000  a........w.dZ...
+00000000: 610d 0d0a 0000 0000 195e 9464 5a09 0000  a........^.dZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 5a00 6401 6402 6c01 5a01 4700 6403 6404  Z.d.d.l.Z.G.d.d.
 00000040: 8400 6404 6501 6a02 8303 5a02 6402 5300  ..d.e.j...Z.d.S.
 00000050: 2905 7a1c 4261 7365 2052 656e 6b75 2070  ).z.Base Renku p
 00000060: 6572 7369 7374 656e 7420 636c 6173 732e  ersistent class.
 00000070: e900 0000 004e 6300 0000 0000 0000 0000  .....Nc.........
```

### Comparing `renku-2.5.0rc3/renku/infrastructure/__pycache__/repository.cpython-39.pyc` & `renku-2.6.0rc1/renku/infrastructure/__pycache__/repository.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 72047 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6f19 0100  a........w.do...
+00000000: 610d 0d0a 0000 0000 195e 9464 6f19 0100  a........^.do...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 fc02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6402 6c07 5a07 6401 6403 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 6d09 5a09 0100 6401 6404 6c0a 6d0a 5a0a  m.Z...d.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/infrastructure/database.py` & `renku-2.6.0rc1/renku/infrastructure/database.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/gateway/__init__.py` & `renku-2.6.0rc1/renku/infrastructure/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-39.pyc` & `renku-2.6.0rc1/renku/infrastructure/gateway/__pycache__/dataset_gateway.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3743 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9f0e 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 9f0e 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a04 6401 6404 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 0100 4700  ..d.d.l.m.Z...G.
```

### Comparing `renku-2.5.0rc3/renku/infrastructure/gateway/activity_gateway.py` & `renku-2.6.0rc1/renku/infrastructure/gateway/activity_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/gateway/database_gateway.py` & `renku-2.6.0rc1/renku/infrastructure/gateway/database_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/gateway/dataset_gateway.py` & `renku-2.6.0rc1/renku/infrastructure/gateway/dataset_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/gateway/plan_gateway.py` & `renku-2.6.0rc1/renku/infrastructure/gateway/plan_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/gateway/project_gateway.py` & `renku-2.6.0rc1/renku/infrastructure/gateway/project_gateway.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/git_merger.py` & `renku-2.6.0rc1/renku/infrastructure/git_merger.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/immutable.py` & `renku-2.6.0rc1/renku/infrastructure/immutable.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/persistent.py` & `renku-2.6.0rc1/renku/infrastructure/persistent.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/repository.py` & `renku-2.6.0rc1/renku/infrastructure/repository.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/storage/__init__.py` & `renku-2.6.0rc1/renku/infrastructure/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc` & `renku-2.6.0rc1/renku/infrastructure/storage/__pycache__/factory.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1989 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 c507 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 c507 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6502 7238 6401 6404 6c07 6d08 5a08  ..e.r8d.d.l.m.Z.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6506 8303 5a0a 6407 5300 2908 7a1f 5374  e...Z.d.S.).z.St
```

### Comparing `renku-2.5.0rc3/renku/infrastructure/storage/factory.py` & `renku-2.6.0rc1/renku/infrastructure/storage/factory.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/infrastructure/storage/rclone.py` & `renku-2.6.0rc1/renku/infrastructure/storage/rclone.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md` & `renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/.github/ISSUE_TEMPLATE/config.yml` & `renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md` & `renku-2.6.0rc1/renku/templates/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/.github/dependabot.yml` & `renku-2.6.0rc1/renku/templates/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/.gitignore` & `renku-2.6.0rc1/renku/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/R-minimal/.gitignore` & `renku-2.6.0rc1/renku/templates/R-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/R-minimal/.renkulfsignore` & `renku-2.6.0rc1/renku/templates/R-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/R-minimal/Dockerfile` & `renku-2.6.0rc1/renku/templates/R-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/R-minimal/README.md` & `renku-2.6.0rc1/renku/templates/R-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/R-minimal/workflows/my-workflow.yaml` & `renku-2.6.0rc1/renku/templates/R-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/R-minimal.png` & `renku-2.6.0rc1/renku/templates/R-minimal.png`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/README.md` & `renku-2.6.0rc1/renku/templates/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/bioc-minimal/.gitignore` & `renku-2.6.0rc1/renku/templates/bioc-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/bioc-minimal/.renkulfsignore` & `renku-2.6.0rc1/renku/templates/bioc-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/bioc-minimal/Dockerfile` & `renku-2.6.0rc1/renku/templates/bioc-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/bioc-minimal/README.md` & `renku-2.6.0rc1/renku/templates/bioc-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/bioc-minimal/workflows/my-workflow.yaml` & `renku-2.6.0rc1/renku/templates/bioc-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/bioconductor.png` & `renku-2.6.0rc1/renku/templates/bioconductor.png`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/julia-minimal/.gitignore` & `renku-2.6.0rc1/renku/templates/julia-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/julia-minimal/.renkulfsignore` & `renku-2.6.0rc1/renku/templates/julia-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/julia-minimal/Dockerfile` & `renku-2.6.0rc1/renku/templates/julia-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/julia-minimal/README.md` & `renku-2.6.0rc1/renku/templates/julia-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/julia-minimal/workflows/my-workflow.yaml` & `renku-2.6.0rc1/renku/templates/julia-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/julialang.png` & `renku-2.6.0rc1/renku/templates/julialang.png`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/manifest.yaml` & `renku-2.6.0rc1/renku/templates/manifest.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/minimal/.renkulfsignore` & `renku-2.6.0rc1/renku/templates/minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/minimal/Dockerfile` & `renku-2.6.0rc1/renku/templates/minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/minimal/workflows/my-workflow.yaml` & `renku-2.6.0rc1/renku/templates/minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/python-minimal/.gitignore` & `renku-2.6.0rc1/renku/templates/python-minimal/.gitignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/python-minimal/.renkulfsignore` & `renku-2.6.0rc1/renku/templates/python-minimal/.renkulfsignore`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/python-minimal/Dockerfile` & `renku-2.6.0rc1/renku/templates/python-minimal/Dockerfile`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/python-minimal/README.md` & `renku-2.6.0rc1/renku/templates/python-minimal/README.md`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/python-minimal/workflows/my-workflow.yaml` & `renku-2.6.0rc1/renku/templates/python-minimal/workflows/my-workflow.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/templates/python-minimal.png` & `renku-2.6.0rc1/renku/templates/python-minimal.png`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/__init__.py` & `renku-2.6.0rc1/renku/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/__init__.py` & `renku-2.6.0rc1/renku/ui/api/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/graph/__init__.py` & `renku-2.6.0rc1/renku/ui/api/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/graph/rdf.py` & `renku-2.6.0rc1/renku/ui/api/graph/rdf.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/models/__init__.py` & `renku-2.6.0rc1/renku/ui/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/models/activity.py` & `renku-2.6.0rc1/renku/ui/api/models/activity.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/models/dataset.py` & `renku-2.6.0rc1/renku/ui/api/models/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/models/parameter.py` & `renku-2.6.0rc1/renku/ui/api/models/parameter.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/models/plan.py` & `renku-2.6.0rc1/renku/ui/api/models/plan.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/models/project.py` & `renku-2.6.0rc1/renku/ui/api/models/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/api/util.py` & `renku-2.6.0rc1/renku/ui/api/util.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/__init__.py` & `renku-2.6.0rc1/renku/ui/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/__main__.py` & `renku-2.6.0rc1/renku/ui/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/__init__.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 9319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6724 0000  a........w.dg$..
+00000000: 610d 0d0a 0000 0000 195e 9464 6724 0000  a........^.dg$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 5404 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6402 6c06 5a06 6401  m.Z...d.d.l.Z.d.
 00000060: 6402 6c07 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6405 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/clone.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/clone.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2594 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 220a 0000  a........w.d"...
+00000000: 610d 0d0a 0000 0000 195e 9464 220a 0000  a........^.d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6501 a007 a100 6501  ..m.Z...e.....e.
 00000060: 6a08 6403 6404 6405 6406 6407 8d04 6501  j.d.d.d.d.d...e.
 00000070: a009 6408 a101 6501 6a09 6409 6406 6402  ..d...e.j.d.d.d.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/config.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 7953 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 111f 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 111f 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 a009 a100 6404 6405 8400  Z...e.....d.d...
 00000070: 8301 5a0a 650a a00b a100 6501 6a0c 6406  ..Z.e.....e.j.d.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/dataset.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/dataset.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 42787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 23a7 0000  a........w.d#...
+00000000: 610d 0d0a 0000 0000 195e 9464 23a7 0000  a........^.d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0015 0000 0040 0000 0073 fc07 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6402 6c09 5a09 6401 6405 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6402 6c0c 6d0d 0200  m.Z...d.d.l.m...
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/doctor.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/doctor.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2333 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 1d09 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 1d09 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6502  Z.d.d.l.m.Z...e.
 00000050: a005 a100 6502 6a06 6502 6a07 6404 6405  ....e.j.e.j.d.d.
 00000060: 6406 6407 8d03 6502 6a07 6408 6409 6405  d.d...e.j.d.d.d.
 00000070: 640a 6407 8d04 640b 640c 8400 8301 8301  d.d...d.d.......
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/env.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/env.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1587 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 3306 0000  a........w.d3...
+00000000: 610d 0d0a 0000 0000 195e 9464 3306 0000  a........^.d3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 a100  Z.d.d.l.Z.e.....
 00000040: 6501 6a03 6403 6404 6405 6406 6407 8d04  e.j.d.d.d.d.d...
 00000050: 6501 6a04 6408 6409 8400 8301 8301 8301  e.j.d.d.........
 00000060: 5a05 6402 5300 290a 7a23 5265 6e6b 7520  Z.d.S.).z#Renku 
 00000070: 656e 7669 726f 6e6d 656e 7420 7265 6c61  environment rela
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/exception_handler.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 7931 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 fb1e 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 fb1e 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6403 6c07 6d08 5a08 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6402 6c09 5a09 6401 6402 6c0a 6d0b 0200  d.l.Z.d.d.l.m...
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/gc.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/gc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1139 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 7304 0000  a........w.ds...
+00000000: 610d 0d0a 0000 0000 195e 9464 7304 0000  a........^.ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6501 a002 a100  Z.d.d.l.Z.e.....
 00000040: 6403 6404 8400 8301 5a03 6402 5300 2905  d.d.....Z.d.S.).
 00000050: 7adf 4672 6565 2075 7020 6469 736b 2073  z.Free up disk s
 00000060: 7061 6365 2062 7920 7265 6d6f 7669 6e67  pace by removing
 00000070: 2074 656d 706f 7261 7279 2066 696c 6573   temporary files
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/githooks.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/githooks.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2538 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 ea09 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 ea09 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6402 6c05 6d06 0200 0100 6d07 0200 0100  d.l.m.....m.....
 00000060: 6d08 0200 0100 6d09 5a09 0100 6504 a00a  m.....m.Z...e...
 00000070: a100 6404 6405 8400 8301 5a0b 650b a00c  ..d.d.....Z.e...
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/graph.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/graph.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4950 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 5613 0000  a........w.dV...
+00000000: 610d 0d0a 0000 0000 195e 9464 5613 0000  a........^.dV...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6404 6404 6405 6406 6407  m.Z...d.d.d.d.d.
 00000050: 6408 6409 640a 9c07 5a04 6501 a005 a100  d.d.d...Z.e.....
 00000060: 640b 640c 8400 8301 5a06 6506 a007 a100  d.d.....Z.e.....
 00000070: 6501 6a08 640d 6503 6509 6504 a00a a100  e.j.d.e.e.e.....
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/init.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/init.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 11113 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 692b 0000  a........w.di+..
+00000000: 610d 0d0a 0000 0000 195e 9464 692b 0000  a........^.di+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0013 0000 0040 0000 0073 a001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6405 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6700 6407 a201  d.l.m.Z...g.d...
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/log.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/log.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 8581 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8521 0000  a........w.d.!..
+00000000: 610d 0d0a 0000 0000 195e 9464 8521 0000  a........^.d.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 2e01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0c 0100 6401 6404 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/login.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/login.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4845 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 ed12 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 ed12 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 a009 a100 6501 6a0a 6404  Z...e.....e.j.d.
 00000070: 6405 6402 6406 8d03 6501 6a0b 6407 6408  d.d.d...e.j.d.d.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/mergetool.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2499 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 c309 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 c309 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 a004 a100 6404 6405  m.Z...e.....d.d.
 00000050: 8400 8301 5a05 6505 6a06 6406 6407 8d01  ....Z.e.j.d.d...
 00000060: 6501 6a07 6408 6501 6a08 6406 6409 8d01  e.j.d.e.j.d.d...
 00000070: 640a 8d02 6501 6a07 640b 6501 6a08 6406  d...e.j.d.e.j.d.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/migrate.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/migrate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5894 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 0617 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 0617 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 2a01 0000 6400  .....@...s*...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a05 6401 6402 6c06 6d07 0200  d.l.Z.d.d.l.m...
 00000060: 0100 6d08 0200 0100 6d09 0200 0100 6d0a  ..m.....m.....m.
 00000070: 5a0a 0100 6401 6404 6c0b 6d0c 5a0c 6d0d  Z...d.d.l.m.Z.m.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/move.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/move.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2881 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 410b 0000  a........w.dA...
+00000000: 610d 0d0a 0000 0000 195e 9464 410b 0000  a........^.dA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 6a04 6404 6405 8d01  m.Z...e.j.d.d...
 00000050: 6501 6a05 6406 6501 6a06 6407 6408 8d01  e.j.d.e.j.d.d...
 00000060: 6409 640a 8d03 6501 6a05 640b 6501 a006  d.d...e.j.d.e...
 00000070: a100 640c 640a 8d03 6501 6a07 640d 640e  ..d.d...e.j.d.d.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/project.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/project.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8816 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 8816 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6402 6c05 6d06 0200 0100 6d07 0200 0100  d.l.m.....m.....
 00000060: 6d08 0200 0100 6d09 5a09 0100 6401 6404  m.....m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6401 6405 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/remove.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/remove.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 da06 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 da06 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 6a04 6404 6405 8d01  m.Z...e.j.d.d...
 00000050: 6501 6a05 6406 6501 6a06 6407 6408 8d01  e.j.d.e.j.d.d...
 00000060: 6409 6407 640a 8d04 640b 640c 8400 8301  d.d.d...d.d.....
 00000070: 8301 5a07 6402 5300 290d 6121 0200 0052  ..Z.d.S.).a!...R
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/rerun.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/rerun.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 4227 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 8310 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 8310 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6501 a00a a100  d.l.m.Z...e.....
 00000070: 6501 6a0b 6407 6408 6409 640a 640b 640c  e.j.d.d.d.d.d.d.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/rollback.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/rollback.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3249 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 b10c 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 b10c 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6501 a004 a100 6501 6a05  m.Z...e.....e.j.
 00000050: 6404 6405 8400 8301 8301 5a06 6402 5300  d.d.......Z.d.S.
 00000060: 2906 75f8 0700 0052 6f6c 6c62 6163 6b20  ).u....Rollback 
 00000070: 7072 6f6a 6563 7420 746f 2061 2070 7265  project to a pre
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/run.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/run.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 26417 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 3167 0000  a........w.d1g..
+00000000: 610d 0d0a 0000 0000 195e 9464 3167 0000  a........^.d1g..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0019 0000 0040 0000 0073 0e02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0b 6d0c 5a0c 0100 6401  ..d.d.l.m.Z...d.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/save.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/save.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 3510 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 b60d 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 b60d 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 6a09 6404 6405 8d01 6501  Z...e.j.d.d...e.
 00000070: 6a0a 6406 6407 6402 6408 6409 8d04 6501  j.d.d.d.d.d...e.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/service.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/service.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 11927 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 972e 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 972e 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 8002 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6401 6403 6c07 6d07 5a07 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6404 6c08 6d09 5a09 0100 6401 6402 6c0a  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/session.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/session.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 14738 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 9239 0000  a........w.d.9..
+00000000: 610d 0d0a 0000 0000 195e 9464 9239 0000  a........^.d.9..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 d602 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/status.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/status.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5489 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 7115 0000  a........w.dq...
+00000000: 610d 0d0a 0000 0000 195e 9464 7115 0000  a........^.dq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 0200 0100 6d04 0200 0100 6d05 0200  m.....m.....m...
 00000050: 0100 6d06 5a06 0100 6401 6403 6c07 6d08  ..m.Z...d.d.l.m.
 00000060: 5a08 0100 6501 a009 a100 6501 6a0a 6501  Z...e.....e.j.e.
 00000070: 6a0b 6404 6405 6406 6407 6408 8d04 6501  j.d.d.d.d.d...e.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/storage.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/storage.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5604 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 e415 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 e415 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 4801 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 6d04 0200 0100 6d05  Z.d.d.l.m.....m.
 00000050: 0200 0100 6d06 0200 0100 6d07 5a07 0100  ....m.....m.Z...
 00000060: 6401 6403 6c08 6d09 5a09 0100 6401 6404  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6502 a00c a100 6405  l.m.Z...e.....d.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/template.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/template.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 13434 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 7a34 0000  a........w.dz4..
+00000000: 610d 0d0a 0000 0000 195e 9464 7a34 0000  a........^.dz4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 7402 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6401 6402 6c08  m.Z.m.Z...d.d.l.
 00000060: 5a08 6401 6402 6c09 6d0a 0200 0100 6d0b  Z.d.d.l.m.....m.
 00000070: 0200 0100 6d0c 0200 0100 6d0d 5a0d 0100  ....m.....m.Z...
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/update.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/update.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 6723 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 431a 0000  a........w.dC...
+00000000: 610d 0d0a 0000 0000 195e 9464 431a 0000  a........^.dC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6401 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6501 a00c a100 6501 6a0d  m.Z...e.....e.j.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/__pycache__/workflow.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/__pycache__/workflow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 47787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 abba 0000  a........w.d....
+00000000: 610d 0d0a 0000 0000 195e 9464 abba 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0016 0000 0040 0000 0073 6607 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6402 6c07 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6401 6402 6c0a 6d0b 0200 0100 6d0c  ..d.d.l.m.....m.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/clone.py` & `renku-2.6.0rc1/renku/ui/cli/clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/config.py` & `renku-2.6.0rc1/renku/ui/cli/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/dataset.py` & `renku-2.6.0rc1/renku/ui/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/doctor.py` & `renku-2.6.0rc1/renku/ui/cli/doctor.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/env.py` & `renku-2.6.0rc1/renku/ui/cli/env.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/exception_handler.py` & `renku-2.6.0rc1/renku/ui/cli/exception_handler.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/gc.py` & `renku-2.6.0rc1/renku/ui/cli/gc.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/githooks.py` & `renku-2.6.0rc1/renku/ui/cli/githooks.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/graph.py` & `renku-2.6.0rc1/renku/ui/cli/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/init.py` & `renku-2.6.0rc1/renku/ui/cli/init.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/log.py` & `renku-2.6.0rc1/renku/ui/cli/log.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/login.py` & `renku-2.6.0rc1/renku/ui/cli/login.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/mergetool.py` & `renku-2.6.0rc1/renku/ui/cli/mergetool.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/migrate.py` & `renku-2.6.0rc1/renku/ui/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/move.py` & `renku-2.6.0rc1/renku/ui/cli/move.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/project.py` & `renku-2.6.0rc1/renku/ui/cli/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/remove.py` & `renku-2.6.0rc1/renku/ui/cli/remove.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/rerun.py` & `renku-2.6.0rc1/renku/ui/cli/rerun.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/rollback.py` & `renku-2.6.0rc1/renku/ui/cli/rollback.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/run.py` & `renku-2.6.0rc1/renku/ui/cli/run.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/save.py` & `renku-2.6.0rc1/renku/ui/cli/save.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/service.py` & `renku-2.6.0rc1/renku/ui/cli/service.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/session.py` & `renku-2.6.0rc1/renku/ui/cli/session.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/status.py` & `renku-2.6.0rc1/renku/ui/cli/status.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/storage.py` & `renku-2.6.0rc1/renku/ui/cli/storage.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/template.py` & `renku-2.6.0rc1/renku/ui/cli/template.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/update.py` & `renku-2.6.0rc1/renku/ui/cli/update.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/__init__.py` & `renku-2.6.0rc1/renku/ui/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/callback.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5409 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 2115 0000  a........w.d!...
+00000000: 610d 0d0a 0000 0000 195e 9464 2115 0000  a........^.d!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6402 6c04 5a04 6401  m.Z...d.d.l.Z.d.
 00000050: 6404 6c05 6d05 5a05 0100 6401 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d06 5a06 0100 6401 6402 6c07 6d08 0200  m.Z...d.d.l.m...
 00000070: 0100 6d09 0200 0100 6d0a 0200 0100 6d0b  ..m.....m.....m.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/click.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 5473 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 6115 0000  a........w.da...
+00000000: 610d 0d0a 0000 0000 195e 9464 6115 0000  a........^.da...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 aa00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a04 6502 722c 6401  ..d.d.l.Z.e.r,d.
 00000050: 6404 6c05 6d06 5a06 0100 6503 6507 1900  d.l.m.Z...e.e...
 00000060: 6405 9c01 6406 6407 8404 5a08 6503 6507  d...d.d...Z.e.e.
 00000070: 1900 6405 9c01 6408 6409 8404 5a09 6503  ..d...d.d...Z.e.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/plugins.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 1375 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 5f05 0000  a........w.d_...
+00000000: 610d 0d0a 0000 0000 195e 9464 5f05 0000  a........^.d_...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 5a00 6401 6402 8400 5a01 6403 6404 8400  Z.d.d...Z.d.d...
 00000040: 5a02 6405 6406 8400 5a03 6407 5300 2908  Z.d.d...Z.d.S.).
 00000050: 7a1e 5574 696c 6974 7920 6675 6e63 7469  z.Utility functi
 00000060: 6f6e 7320 666f 7220 706c 7567 696e 732e  ons for plugins.
 00000070: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/cli/utils/__pycache__/terminal.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 9917 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 bd26 0000  a........w.d.&..
+00000000: 610d 0d0a 0000 0000 195e 9464 bd26 0000  a........^.d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6e01 0000 6400  .....@...sn...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6402 6c07 5a07 6401 6404 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
 00000070: 0100 6506 7270 6401 6405 6c0a 6d0b 5a0b  ..e.rpd.d.l.m.Z.
```

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/callback.py` & `renku-2.6.0rc1/renku/ui/cli/utils/callback.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/click.py` & `renku-2.6.0rc1/renku/ui/cli/utils/click.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/color.py` & `renku-2.6.0rc1/renku/ui/cli/utils/color.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/curses.py` & `renku-2.6.0rc1/renku/ui/cli/utils/curses.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/plugins.py` & `renku-2.6.0rc1/renku/ui/cli/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/utils/terminal.py` & `renku-2.6.0rc1/renku/ui/cli/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/cli/workflow.py` & `renku-2.6.0rc1/renku/ui/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/.env-example` & `renku-2.6.0rc1/renku/ui/service/.env-example`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/__init__.py` & `renku-2.6.0rc1/renku/ui/service/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/__pycache__/config.cpython-39.pyc` & `renku-2.6.0rc1/renku/ui/service/__pycache__/config.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Jun 14 08:18:31 2023 UTC, .py size: 2931 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 d777 8964 730b 0000  a........w.ds...
+00000000: 610d 0d0a 0000 0000 195e 9464 130c 0000  a........^.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 be01 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0073 ca01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 7a0c  Z.d.d.l.m.Z...z.
 00000050: 6401 6402 6c05 5a05 5700 6e1e 0400 6506  d.d.l.Z.W.n...e.
 00000060: 794a 0100 0100 0100 6401 6402 6c07 6d08  yJ......d.d.l.m.
 00000070: 5a05 0100 5900 6e02 3000 6401 5a09 6404  Z...Y.n.0.d.Z.d.
 00000080: 5a0a 6405 5a0b 6406 5a0c 6407 5a0d 6408  Z.d.Z.d.Z.d.Z.d.
 00000090: 5a0e 6409 5a0f 640a 5a10 640b 5a11 640c  Z.d.Z.d.Z.d.Z.d.
@@ -24,103 +24,109 @@
 00000170: a102 5a29 6505 a02a 6421 a101 6422 1b00  ..Z)e..*d!..d"..
 00000180: 5a2b 6505 a02c 652b a101 8f14 5a19 6519  Z+e..,e+....Z.e.
 00000190: 5a2d 5700 6402 0400 0400 8303 0100 6e12  Z-W.d.........n.
 000001a0: 3100 9001 737a 3000 0100 0100 0100 5900  1...sz0.......Y.
 000001b0: 0100 6501 6a2e a02f 6423 6424 a102 6425  ..e.j../d#d$..d%
 000001c0: 1700 5a30 6501 a015 6426 6427 a102 a031  ..Z0e...d&d'...1
 000001d0: a100 6428 6b02 5a32 6533 6501 a015 6429  ..d(k.Z2e3e...d)
-000001e0: 642a a102 8301 5a34 6402 5300 292b 7a15  d*....Z4d.S.)+z.
-000001f0: 5265 6e6b 7520 7365 7276 6963 6520 636f  Renku service co
-00000200: 6e66 6967 2ee9 0000 0000 4e29 01da 0450  nfig......N)...P
-00000210: 6174 6869 e803 0000 69d0 0700 0069 b80b  athi....i....i..
-00000220: 0000 7a2e 6874 7470 733a 2f2f 7265 6e6b  ..z.https://renk
-00000230: 752d 7079 7468 6f6e 2e72 6561 6474 6865  u-python.readthe
-00000240: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00000250: 742f 7a2c 7365 7276 6963 655f 6572 726f  t/z,service_erro
-00000260: 7273 2e68 746d 6c23 7265 6e6b 752e 7569  rs.html#renku.ui
-00000270: 2e73 6572 7669 6365 2e65 7272 6f72 732e  .service.errors.
-00000280: da07 556e 6b6e 6f77 6e7a 0d52 656e 6b75  ..Unknownz.Renku
-00000290: 2053 6572 7669 6365 7a05 332e 302e 33da   Servicez.3.0.3.
-000002a0: 0276 31e9 ffff ffff da1b 5052 4f4a 4543  .v1.......PROJEC
-000002b0: 545f 434c 4f4e 455f 4445 5054 485f 4445  T_CLONE_DEPTH_DE
-000002c0: 4641 554c 54e9 0100 0000 da1c 5445 4d50  FAULT.......TEMP
-000002d0: 4c41 5445 5f43 4c4f 4e45 5f44 4550 5448  LATE_CLONE_DEPTH
-000002e0: 5f44 4546 4155 4c54 da12 4d41 585f 434f  _DEFAULT..MAX_CO
-000002f0: 4e54 454e 545f 4c45 4e47 5448 6900 0000  NTENT_LENGTHi...
-00000300: 40da 0943 4143 4845 5f44 4952 5a07 7570  @..CACHE_DIRZ.up
-00000310: 6c6f 6164 7354 2902 da07 7061 7265 6e74  loadsT)...parent
-00000320: 73da 0865 7869 7374 5f6f 6bda 0870 726f  s..exist_ok..pro
-00000330: 6a65 6374 737a 1161 7070 6c69 6361 7469  jectsz.applicati
-00000340: 6f6e 2f78 2d74 6172 7a0f 6170 706c 6963  on/x-tarz.applic
-00000350: 6174 696f 6e2f 7a69 707a 1261 7070 6c69  ation/zipz.appli
-00000360: 6361 7469 6f6e 2f78 2d67 7a69 705a 1343  cation/x-gzipZ.C
-00000370: 4f52 455f 5345 5256 4943 455f 5052 4546  ORE_SERVICE_PREF
-00000380: 4958 da01 2f5a 1a43 4f52 455f 5345 5256  IX../Z.CORE_SERV
-00000390: 4943 455f 4150 495f 4241 5345 5f50 4154  ICE_API_BASE_PAT
-000003a0: 487a 0a2f 7370 6563 2e6a 736f 6eda 084f  Hz./spec.json..O
-000003b0: 4944 435f 5552 4c7a 332f 6175 7468 2f72  IDC_URLz3/auth/r
-000003c0: 6561 6c6d 732f 5265 6e6b 752f 2e77 656c  ealms/Renku/.wel
-000003d0: 6c2d 6b6e 6f77 6e2f 6f70 656e 6964 2d63  l-known/openid-c
-000003e0: 6f6e 6669 6775 7261 7469 6f6e 7a10 7265  onfigurationz.re
-000003f0: 6e6b 752e 7569 2e73 6572 7669 6365 7a0c  nku.ui.servicez.
-00000400: 6c6f 6767 696e 672e 7961 6d6c da0c 5245  logging.yaml..RE
-00000410: 4e4b 555f 444f 4d41 494e da07 7365 7276  NKU_DOMAIN..serv
-00000420: 6963 65da 013a da0e 5345 4e54 5259 5f45  ice..:..SENTRY_E
-00000430: 4e41 424c 4544 da05 6661 6c73 65da 0474  NABLED..false..t
-00000440: 7275 655a 1253 454e 5452 595f 5341 4d50  rueZ.SENTRY_SAMP
-00000450: 4c45 5f52 4154 4567 9a99 9999 9999 c93f  LE_RATEg.......?
-00000460: 2935 da07 5f5f 646f 635f 5fda 026f 73da  )5..__doc__..os.
-00000470: 0874 656d 7066 696c 65da 0770 6174 686c  .tempfile..pathl
-00000480: 6962 7202 0000 00da 1369 6d70 6f72 746c  ibr......importl
-00000490: 6962 5f72 6573 6f75 7263 6573 da0b 496d  ib_resources..Im
-000004a0: 706f 7274 4572 726f 72da 1369 6d70 6f72  portError..impor
-000004b0: 746c 6962 2e72 6573 6f75 7263 6573 da09  tlib.resources..
-000004c0: 7265 736f 7572 6365 735a 1153 5643 5f45  resourcesZ.SVC_E
-000004d0: 5252 4f52 5f47 454e 4552 4943 5a0e 5356  RROR_GENERICZ.SV
-000004e0: 435f 4552 524f 525f 5553 4552 5a15 5356  C_ERROR_USERZ.SV
-000004f0: 435f 4552 524f 525f 5052 4f47 5241 4d4d  C_ERROR_PROGRAMM
-00000500: 494e 475a 1653 5643 5f45 5252 4f52 5f49  INGZ.SVC_ERROR_I
-00000510: 4e54 4552 4d49 5454 454e 545a 0d44 4f43  NTERMITTENTZ.DOC
-00000520: 535f 5552 4c5f 4241 5345 5a0f 444f 4353  S_URL_BASEZ.DOCS
-00000530: 5f55 524c 5f45 5252 4f52 535a 1345 5252  _URL_ERRORSZ.ERR
-00000540: 4f52 5f4e 4f54 5f41 5641 494c 4142 4c45  OR_NOT_AVAILABLE
-00000550: 5a0c 5345 5256 4943 455f 4e41 4d45 5a0f  Z.SERVICE_NAMEZ.
-00000560: 4f50 454e 4150 495f 5645 5253 494f 4e5a  OPENAPI_VERSIONZ
-00000570: 0b41 5049 5f56 4552 5349 4f4e 5a16 5052  .API_VERSIONZ.PR
-00000580: 4f4a 4543 545f 434c 4f4e 455f 4e4f 5f44  OJECT_CLONE_NO_D
-00000590: 4550 5448 da03 696e 74da 0667 6574 656e  EPTH..int..geten
-000005a0: 7672 0600 0000 7208 0000 0072 0900 0000  vr....r....r....
-000005b0: da04 7061 7468 da08 7265 616c 7061 7468  ..path..realpath
-000005c0: da12 5465 6d70 6f72 6172 7944 6972 6563  ..TemporaryDirec
-000005d0: 746f 7279 da04 6e61 6d65 720a 0000 005a  tory..namer....Z
-000005e0: 1243 4143 4845 5f55 504c 4f41 4453 5f50  .CACHE_UPLOADS_P
-000005f0: 4154 48da 056d 6b64 6972 5a13 4341 4348  ATH..mkdirZ.CACH
-00000600: 455f 5052 4f4a 4543 5453 5f50 4154 485a  E_PROJECTS_PATHZ
-00000610: 1854 4152 5f41 5243 4849 5645 5f43 4f4e  .TAR_ARCHIVE_CON
-00000620: 5445 4e54 5f54 5950 455a 185a 4950 5f41  TENT_TYPEZ.ZIP_A
-00000630: 5243 4849 5645 5f43 4f4e 5445 4e54 5f54  RCHIVE_CONTENT_T
-00000640: 5950 455a 1747 5a5f 4152 4348 4956 455f  YPEZ.GZ_ARCHIVE_
-00000650: 434f 4e54 454e 545f 5459 5045 5a12 5355  CONTENT_TYPEZ.SU
-00000660: 5050 4f52 5445 445f 4152 4348 4956 4553  PPORTED_ARCHIVES
-00000670: 5a0e 5345 5256 4943 455f 5052 4546 4958  Z.SERVICE_PREFIX
-00000680: 5a15 5345 5256 4943 455f 4150 495f 4241  Z.SERVICE_API_BA
-00000690: 5345 5f50 4154 48da 066c 7374 7269 705a  SE_PATH..lstripZ
-000006a0: 0c41 5049 5f53 5045 435f 5552 4c72 0f00  .API_SPEC_URLr..
-000006b0: 0000 da05 6669 6c65 73da 0372 6566 da07  ....files..ref..
-000006c0: 6173 5f66 696c 655a 124c 4f47 4745 525f  as_fileZ.LOGGER_
-000006d0: 434f 4e46 4947 5f46 494c 45da 0765 6e76  CONFIG_FILE..env
-000006e0: 6972 6f6e da03 6765 745a 0e4d 4553 5341  iron..getZ.MESSA
-000006f0: 4745 5f50 5245 4649 58da 056c 6f77 6572  GE_PREFIX..lower
-00000700: 7213 0000 00da 0566 6c6f 6174 da11 5345  r......float..SE
-00000710: 4e54 5259 5f53 414d 504c 4552 4154 45a9  NTRY_SAMPLERATE.
-00000720: 0072 2e00 0000 722e 0000 00fa 462f 686f  .r....r.....F/ho
-00000730: 6d65 2f72 756e 6e65 722f 776f 726b 2f72  me/runner/work/r
-00000740: 656e 6b75 2d70 7974 686f 6e2f 7265 6e6b  enku-python/renk
-00000750: 752d 7079 7468 6f6e 2f72 656e 6b75 2f75  u-python/renku/u
-00000760: 692f 7365 7276 6963 652f 636f 6e66 6967  i/service/config
-00000770: 2e70 79da 083c 6d6f 6475 6c65 3e11 0000  .py..<module>...
-00000780: 0073 5600 0000 0401 0801 0801 0c02 0201  .sV.............
-00000790: 0c01 0c01 1202 0401 0401 0401 0402 0401  ................
-000007a0: 0401 0402 0401 0401 0402 0401 1001 1003  ................
-000007b0: 1002 1a01 1001 0e02 1001 0e02 0401 0401  ................
-000007c0: 0403 0201 0201 02fd 0407 0c02 0c02 0e02  ................
-000007d0: 0c02 0e01 0c01 2401 1203 1401            ......$.....
+000001e0: 642a a102 8301 5a34 6501 a015 642b 642c  d*....Z4e...d+d,
+000001f0: a102 5a35 6402 5300 292d 7a15 5265 6e6b  ..Z5d.S.)-z.Renk
+00000200: 7520 7365 7276 6963 6520 636f 6e66 6967  u service config
+00000210: 2ee9 0000 0000 4e29 01da 0450 6174 6869  ......N)...Pathi
+00000220: e803 0000 69d0 0700 0069 b80b 0000 7a2e  ....i....i....z.
+00000230: 6874 7470 733a 2f2f 7265 6e6b 752d 7079  https://renku-py
+00000240: 7468 6f6e 2e72 6561 6474 6865 646f 6373  thon.readthedocs
+00000250: 2e69 6f2f 656e 2f6c 6174 6573 742f 7a2c  .io/en/latest/z,
+00000260: 7365 7276 6963 655f 6572 726f 7273 2e68  service_errors.h
+00000270: 746d 6c23 7265 6e6b 752e 7569 2e73 6572  tml#renku.ui.ser
+00000280: 7669 6365 2e65 7272 6f72 732e da07 556e  vice.errors...Un
+00000290: 6b6e 6f77 6e7a 0d52 656e 6b75 2053 6572  knownz.Renku Ser
+000002a0: 7669 6365 7a05 332e 302e 33da 0276 31e9  vicez.3.0.3..v1.
+000002b0: ffff ffff da1b 5052 4f4a 4543 545f 434c  ......PROJECT_CL
+000002c0: 4f4e 455f 4445 5054 485f 4445 4641 554c  ONE_DEPTH_DEFAUL
+000002d0: 54e9 0100 0000 da1c 5445 4d50 4c41 5445  T.......TEMPLATE
+000002e0: 5f43 4c4f 4e45 5f44 4550 5448 5f44 4546  _CLONE_DEPTH_DEF
+000002f0: 4155 4c54 da12 4d41 585f 434f 4e54 454e  AULT..MAX_CONTEN
+00000300: 545f 4c45 4e47 5448 6900 0000 40da 0943  T_LENGTHi...@..C
+00000310: 4143 4845 5f44 4952 5a07 7570 6c6f 6164  ACHE_DIRZ.upload
+00000320: 7354 2902 da07 7061 7265 6e74 73da 0865  sT)...parents..e
+00000330: 7869 7374 5f6f 6bda 0870 726f 6a65 6374  xist_ok..project
+00000340: 737a 1161 7070 6c69 6361 7469 6f6e 2f78  sz.application/x
+00000350: 2d74 6172 7a0f 6170 706c 6963 6174 696f  -tarz.applicatio
+00000360: 6e2f 7a69 707a 1261 7070 6c69 6361 7469  n/zipz.applicati
+00000370: 6f6e 2f78 2d67 7a69 705a 1343 4f52 455f  on/x-gzipZ.CORE_
+00000380: 5345 5256 4943 455f 5052 4546 4958 da01  SERVICE_PREFIX..
+00000390: 2f5a 1a43 4f52 455f 5345 5256 4943 455f  /Z.CORE_SERVICE_
+000003a0: 4150 495f 4241 5345 5f50 4154 487a 0a2f  API_BASE_PATHz./
+000003b0: 7370 6563 2e6a 736f 6eda 084f 4944 435f  spec.json..OIDC_
+000003c0: 5552 4c7a 332f 6175 7468 2f72 6561 6c6d  URLz3/auth/realm
+000003d0: 732f 5265 6e6b 752f 2e77 656c 6c2d 6b6e  s/Renku/.well-kn
+000003e0: 6f77 6e2f 6f70 656e 6964 2d63 6f6e 6669  own/openid-confi
+000003f0: 6775 7261 7469 6f6e 7a10 7265 6e6b 752e  gurationz.renku.
+00000400: 7569 2e73 6572 7669 6365 7a0c 6c6f 6767  ui.servicez.logg
+00000410: 696e 672e 7961 6d6c da0c 5245 4e4b 555f  ing.yaml..RENKU_
+00000420: 444f 4d41 494e da07 7365 7276 6963 65da  DOMAIN..service.
+00000430: 013a da0e 5345 4e54 5259 5f45 4e41 424c  .:..SENTRY_ENABL
+00000440: 4544 da05 6661 6c73 65da 0474 7275 655a  ED..false..trueZ
+00000450: 1253 454e 5452 595f 5341 4d50 4c45 5f52  .SENTRY_SAMPLE_R
+00000460: 4154 4567 9a99 9999 9999 c93f da16 4d45  ATEg.......?..ME
+00000470: 5441 4441 5441 5f56 4552 5349 4f4e 535f  TADATA_VERSIONS_
+00000480: 4c49 5354 7a34 2f73 7663 2f63 6f6e 6669  LISTz4/svc/confi
+00000490: 672f 6d65 7461 6461 7461 2d76 6572 7369  g/metadata-versi
+000004a0: 6f6e 732f 6d65 7461 6461 7461 2d76 6572  ons/metadata-ver
+000004b0: 7369 6f6e 732e 6a73 6f6e 2936 da07 5f5f  sions.json)6..__
+000004c0: 646f 635f 5fda 026f 73da 0874 656d 7066  doc__..os..tempf
+000004d0: 696c 65da 0770 6174 686c 6962 7202 0000  ile..pathlibr...
+000004e0: 00da 1369 6d70 6f72 746c 6962 5f72 6573  ...importlib_res
+000004f0: 6f75 7263 6573 da0b 496d 706f 7274 4572  ources..ImportEr
+00000500: 726f 72da 1369 6d70 6f72 746c 6962 2e72  ror..importlib.r
+00000510: 6573 6f75 7263 6573 da09 7265 736f 7572  esources..resour
+00000520: 6365 735a 1153 5643 5f45 5252 4f52 5f47  cesZ.SVC_ERROR_G
+00000530: 454e 4552 4943 5a0e 5356 435f 4552 524f  ENERICZ.SVC_ERRO
+00000540: 525f 5553 4552 5a15 5356 435f 4552 524f  R_USERZ.SVC_ERRO
+00000550: 525f 5052 4f47 5241 4d4d 494e 475a 1653  R_PROGRAMMINGZ.S
+00000560: 5643 5f45 5252 4f52 5f49 4e54 4552 4d49  VC_ERROR_INTERMI
+00000570: 5454 454e 545a 0d44 4f43 535f 5552 4c5f  TTENTZ.DOCS_URL_
+00000580: 4241 5345 5a0f 444f 4353 5f55 524c 5f45  BASEZ.DOCS_URL_E
+00000590: 5252 4f52 535a 1345 5252 4f52 5f4e 4f54  RRORSZ.ERROR_NOT
+000005a0: 5f41 5641 494c 4142 4c45 5a0c 5345 5256  _AVAILABLEZ.SERV
+000005b0: 4943 455f 4e41 4d45 5a0f 4f50 454e 4150  ICE_NAMEZ.OPENAP
+000005c0: 495f 5645 5253 494f 4e5a 0b41 5049 5f56  I_VERSIONZ.API_V
+000005d0: 4552 5349 4f4e 5a16 5052 4f4a 4543 545f  ERSIONZ.PROJECT_
+000005e0: 434c 4f4e 455f 4e4f 5f44 4550 5448 da03  CLONE_NO_DEPTH..
+000005f0: 696e 74da 0667 6574 656e 7672 0600 0000  int..getenvr....
+00000600: 7208 0000 0072 0900 0000 da04 7061 7468  r....r......path
+00000610: da08 7265 616c 7061 7468 da12 5465 6d70  ..realpath..Temp
+00000620: 6f72 6172 7944 6972 6563 746f 7279 da04  oraryDirectory..
+00000630: 6e61 6d65 720a 0000 005a 1243 4143 4845  namer....Z.CACHE
+00000640: 5f55 504c 4f41 4453 5f50 4154 48da 056d  _UPLOADS_PATH..m
+00000650: 6b64 6972 5a13 4341 4348 455f 5052 4f4a  kdirZ.CACHE_PROJ
+00000660: 4543 5453 5f50 4154 485a 1854 4152 5f41  ECTS_PATHZ.TAR_A
+00000670: 5243 4849 5645 5f43 4f4e 5445 4e54 5f54  RCHIVE_CONTENT_T
+00000680: 5950 455a 185a 4950 5f41 5243 4849 5645  YPEZ.ZIP_ARCHIVE
+00000690: 5f43 4f4e 5445 4e54 5f54 5950 455a 1747  _CONTENT_TYPEZ.G
+000006a0: 5a5f 4152 4348 4956 455f 434f 4e54 454e  Z_ARCHIVE_CONTEN
+000006b0: 545f 5459 5045 5a12 5355 5050 4f52 5445  T_TYPEZ.SUPPORTE
+000006c0: 445f 4152 4348 4956 4553 5a0e 5345 5256  D_ARCHIVESZ.SERV
+000006d0: 4943 455f 5052 4546 4958 5a15 5345 5256  ICE_PREFIXZ.SERV
+000006e0: 4943 455f 4150 495f 4241 5345 5f50 4154  ICE_API_BASE_PAT
+000006f0: 48da 066c 7374 7269 705a 0c41 5049 5f53  H..lstripZ.API_S
+00000700: 5045 435f 5552 4c72 0f00 0000 da05 6669  PEC_URLr......fi
+00000710: 6c65 73da 0372 6566 da07 6173 5f66 696c  les..ref..as_fil
+00000720: 655a 124c 4f47 4745 525f 434f 4e46 4947  eZ.LOGGER_CONFIG
+00000730: 5f46 494c 45da 0765 6e76 6972 6f6e da03  _FILE..environ..
+00000740: 6765 745a 0e4d 4553 5341 4745 5f50 5245  getZ.MESSAGE_PRE
+00000750: 4649 58da 056c 6f77 6572 7213 0000 00da  FIX..lowerr.....
+00000760: 0566 6c6f 6174 da11 5345 4e54 5259 5f53  .float..SENTRY_S
+00000770: 414d 504c 4552 4154 4572 1600 0000 a900  AMPLERATEr......
+00000780: 722f 0000 0072 2f00 0000 fa46 2f68 6f6d  r/...r/....F/hom
+00000790: 652f 7275 6e6e 6572 2f77 6f72 6b2f 7265  e/runner/work/re
+000007a0: 6e6b 752d 7079 7468 6f6e 2f72 656e 6b75  nku-python/renku
+000007b0: 2d70 7974 686f 6e2f 7265 6e6b 752f 7569  -python/renku/ui
+000007c0: 2f73 6572 7669 6365 2f63 6f6e 6669 672e  /service/config.
+000007d0: 7079 da08 3c6d 6f64 756c 653e 1100 0000  py..<module>....
+000007e0: 7358 0000 0004 0108 0108 010c 0202 010c  sX..............
+000007f0: 010c 0112 0204 0104 0104 0104 0204 0104  ................
+00000800: 0104 0204 0104 0104 0204 0110 0110 0310  ................
+00000810: 021a 0110 010e 0210 010e 0204 0104 0104  ................
+00000820: 0302 0102 0102 fd04 070c 020c 020e 020c  ................
+00000830: 020e 010c 0124 0112 0314 0110 03         .....$.......
```

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/__init__.py` & `renku-2.6.0rc1/renku/ui/service/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/base.py` & `renku-2.6.0rc1/renku/ui/service/cache/base.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/config.py` & `renku-2.6.0rc1/renku/ui/service/cache/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/files.py` & `renku-2.6.0rc1/renku/ui/service/cache/files.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/jobs.py` & `renku-2.6.0rc1/renku/ui/service/cache/jobs.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/models/__init__.py` & `renku-2.6.0rc1/renku/ui/service/cache/models/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/models/file.py` & `renku-2.6.0rc1/renku/ui/service/cache/models/file.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/models/job.py` & `renku-2.6.0rc1/renku/ui/service/cache/models/job.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/models/project.py` & `renku-2.6.0rc1/renku/ui/service/cache/models/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/models/user.py` & `renku-2.6.0rc1/renku/ui/service/cache/models/user.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/projects.py` & `renku-2.6.0rc1/renku/ui/service/cache/projects.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/serializers/__init__.py` & `renku-2.6.0rc1/renku/ui/service/cache/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/serializers/file.py` & `renku-2.6.0rc1/renku/ui/service/cache/serializers/file.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/serializers/job.py` & `renku-2.6.0rc1/renku/ui/service/cache/serializers/job.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/serializers/project.py` & `renku-2.6.0rc1/renku/ui/service/cache/serializers/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/serializers/user.py` & `renku-2.6.0rc1/renku/ui/service/cache/serializers/user.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/cache/users.py` & `renku-2.6.0rc1/renku/ui/service/cache/users.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/config.py` & `renku-2.6.0rc1/renku/ui/service/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020 - Swiss Data Science Center (SDSC)
+# Copyright 2022 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -74,7 +74,10 @@
 with importlib_resources.as_file(ref) as path:
     LOGGER_CONFIG_FILE = path
 MESSAGE_PREFIX = os.environ.get("RENKU_DOMAIN", "service") + ":"
 
 # Sentry configuration
 SENTRY_ENABLED = os.getenv("SENTRY_ENABLED", "false").lower() == "true"
 SENTRY_SAMPLERATE = float(os.getenv("SENTRY_SAMPLE_RATE", 0.2))
+
+# List of all available metadata versions
+METADATA_VERSIONS_LIST = os.getenv("METADATA_VERSIONS_LIST", "/svc/config/metadata-versions/metadata-versions.json")
```

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/__init__.py` & `renku-2.6.0rc1/renku/ui/service/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/api/__init__.py` & `renku-2.6.0rc1/renku/ui/service/controllers/api/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/api/abstract.py` & `renku-2.6.0rc1/renku/ui/service/controllers/api/abstract.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/api/mixins.py` & `renku-2.6.0rc1/renku/ui/service/controllers/api/mixins.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/cache_files_delete_chunks.py` & `renku-2.6.0rc1/renku/ui/service/controllers/cache_files_delete_chunks.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/cache_files_upload.py` & `renku-2.6.0rc1/renku/ui/service/controllers/cache_files_upload.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/cache_list_projects.py` & `renku-2.6.0rc1/renku/ui/service/controllers/cache_list_projects.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/cache_list_uploaded.py` & `renku-2.6.0rc1/renku/ui/service/controllers/cache_list_uploaded.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/cache_migrate_project.py` & `renku-2.6.0rc1/renku/ui/service/controllers/cache_migrate_project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/cache_migrations_check.py` & `renku-2.6.0rc1/renku/ui/service/controllers/cache_migrations_check.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/cache_project_clone.py` & `renku-2.6.0rc1/renku/ui/service/controllers/cache_project_clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/config_set.py` & `renku-2.6.0rc1/renku/ui/service/controllers/config_set.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/config_show.py` & `renku-2.6.0rc1/renku/ui/service/controllers/config_show.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/datasets_add_file.py` & `renku-2.6.0rc1/renku/ui/service/controllers/datasets_add_file.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/datasets_create.py` & `renku-2.6.0rc1/renku/ui/service/controllers/datasets_create.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/datasets_edit.py` & `renku-2.6.0rc1/renku/ui/service/controllers/datasets_edit.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/datasets_files_list.py` & `renku-2.6.0rc1/renku/ui/service/controllers/datasets_files_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/datasets_import.py` & `renku-2.6.0rc1/renku/ui/service/controllers/datasets_import.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/datasets_list.py` & `renku-2.6.0rc1/renku/ui/service/controllers/datasets_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/datasets_remove.py` & `renku-2.6.0rc1/renku/ui/service/controllers/datasets_remove.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/datasets_unlink.py` & `renku-2.6.0rc1/renku/ui/service/controllers/datasets_unlink.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/graph_export.py` & `renku-2.6.0rc1/renku/ui/service/controllers/graph_export.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/project_edit.py` & `renku-2.6.0rc1/renku/ui/service/controllers/project_edit.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/project_lock_status.py` & `renku-2.6.0rc1/renku/ui/service/controllers/project_lock_status.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/project_show.py` & `renku-2.6.0rc1/renku/ui/service/controllers/project_show.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/templates_create_project.py` & `renku-2.6.0rc1/renku/ui/service/controllers/templates_create_project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/templates_read_manifest.py` & `renku-2.6.0rc1/renku/ui/service/controllers/templates_read_manifest.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/utils/__init__.py` & `renku-2.6.0rc1/renku/ui/service/controllers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/utils/datasets.py` & `renku-2.6.0rc1/renku/ui/service/controllers/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/utils/project_clone.py` & `renku-2.6.0rc1/renku/ui/service/controllers/utils/project_clone.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/utils/remote_project.py` & `renku-2.6.0rc1/renku/ui/service/controllers/utils/remote_project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/version.py` & `renku-2.6.0rc1/renku/ui/service/controllers/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/workflow_plans_export.py` & `renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_export.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/workflow_plans_list.py` & `renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_list.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/controllers/workflow_plans_show.py` & `renku-2.6.0rc1/renku/ui/service/controllers/workflow_plans_show.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/entrypoint.py` & `renku-2.6.0rc1/renku/ui/service/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020 - Swiss Data Science Center (SDSC)
+# Copyright 2022 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -46,14 +46,15 @@
 from renku.ui.service.views.config import config_blueprint
 from renku.ui.service.views.datasets import dataset_blueprint
 from renku.ui.service.views.graph import graph_blueprint
 from renku.ui.service.views.jobs import jobs_blueprint
 from renku.ui.service.views.project import project_blueprint
 from renku.ui.service.views.templates import templates_blueprint
 from renku.ui.service.views.version import version_blueprint
+from renku.ui.service.views.versions_list import versions_list_blueprint
 from renku.ui.service.views.workflow_plans import workflow_plans_blueprint
 
 logging.basicConfig(level=os.getenv("SERVICE_LOG_LEVEL", "WARNING"))
 
 if SENTRY_ENABLED:
     sentry_sdk.init(
         dsn=os.getenv("SENTRY_DSN"),
@@ -150,14 +151,15 @@
     app.register_blueprint(dataset_blueprint)
     app.register_blueprint(graph_blueprint)
     app.register_blueprint(jobs_blueprint)
     app.register_blueprint(project_blueprint)
     app.register_blueprint(templates_blueprint)
     app.register_blueprint(version_blueprint)
     app.register_blueprint(apispec_blueprint)
+    app.register_blueprint(versions_list_blueprint)
 
 
 app = create_app()
 
 
 @app.after_request
 def after_request(response):
```

### Comparing `renku-2.5.0rc3/renku/ui/service/errors.py` & `renku-2.6.0rc1/renku/ui/service/errors.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/gateways/__init__.py` & `renku-2.6.0rc1/renku/ui/service/gateways/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/gateways/gitlab_api_provider.py` & `renku-2.6.0rc1/renku/ui/service/gateways/gitlab_api_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/interfaces/__init__.py` & `renku-2.6.0rc1/renku/ui/service/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/interfaces/git_api_provider.py` & `renku-2.6.0rc1/renku/ui/service/interfaces/git_api_provider.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/jobs/__init__.py` & `renku-2.6.0rc1/renku/ui/service/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/jobs/cleanup.py` & `renku-2.6.0rc1/renku/ui/service/jobs/cleanup.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/jobs/constants.py` & `renku-2.6.0rc1/renku/ui/service/jobs/constants.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/jobs/contexts.py` & `renku-2.6.0rc1/renku/ui/service/jobs/contexts.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/jobs/datasets.py` & `renku-2.6.0rc1/renku/ui/service/jobs/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Dataset jobs."""
+import os
 import urllib
 
 from urllib3.exceptions import HTTPError
 
 from renku.command.dataset import add_to_dataset_command, import_dataset_command
 from renku.core import errors
 from renku.core.util.contexts import renku_project_context
@@ -83,15 +84,15 @@
         # Reraise exception, so we see trace in job metadata
         # and in metrics as failed job.
         raise exp
 
 
 def _is_safe_to_pass_gitlab_token(project_git_url, dataset_uri):
     """Passing token is safe if project and dataset belong to the same deployment."""
-    project_host = GitURL.parse(project_git_url).hostname
+    project_host = os.environ.get("RENKU_DOMAIN") or GitURL.parse(project_git_url).hostname
     dataset_host = urllib.parse.urlparse(dataset_uri).netloc
 
     # NOTE: URLs changed from domain/gitlab to gitlab.domain when moving to cloud native gitlab
     if project_host.startswith("gitlab.") and not dataset_host.startswith("gitlab."):
         project_host = project_host.replace("gitlab.", "", 1)
 
     return project_host == dataset_host
```

### Comparing `renku-2.5.0rc3/renku/ui/service/jobs/delayed_ctrl.py` & `renku-2.6.0rc1/renku/ui/service/jobs/delayed_ctrl.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/jobs/queues.py` & `renku-2.6.0rc1/renku/ui/service/jobs/queues.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/logger.py` & `renku-2.6.0rc1/renku/ui/service/logger.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/logging.yaml` & `renku-2.6.0rc1/renku/ui/service/logging.yaml`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/scheduler.py` & `renku-2.6.0rc1/renku/ui/service/scheduler.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/__init__.py` & `renku-2.6.0rc1/renku/ui/service/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/cache.py` & `renku-2.6.0rc1/renku/ui/service/serializers/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/common.py` & `renku-2.6.0rc1/renku/ui/service/serializers/common.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/config.py` & `renku-2.6.0rc1/renku/ui/service/serializers/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/datasets.py` & `renku-2.6.0rc1/renku/ui/service/serializers/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/graph.py` & `renku-2.6.0rc1/renku/ui/service/serializers/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/headers.py` & `renku-2.6.0rc1/renku/ui/service/serializers/headers.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/jobs.py` & `renku-2.6.0rc1/renku/ui/service/serializers/jobs.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/project.py` & `renku-2.6.0rc1/renku/ui/service/serializers/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/rpc.py` & `renku-2.6.0rc1/renku/ui/service/serializers/rpc.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/templates.py` & `renku-2.6.0rc1/renku/ui/service/serializers/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/v1/__init__.py` & `renku-2.6.0rc1/renku/ui/service/serializers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/v1/cache.py` & `renku-2.6.0rc1/renku/ui/service/serializers/v1/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/v1/templates.py` & `renku-2.6.0rc1/renku/ui/service/serializers/v1/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/version.py` & `renku-2.6.0rc1/renku/ui/service/serializers/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright 2020 - Swiss Data Science Center (SDSC)
+# Copyright 2022 - Swiss Data Science Center (SDSC)
 # A partnership between École Polytechnique Fédérale de Lausanne (EPFL) and
 # Eidgenössische Technische Hochschule Zürich (ETHZ).
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Renku service version controller."""
+"""Renku service version serializers."""
 from marshmallow import Schema, fields
 
 
 class VersionResponse(Schema):
     """Version response schema."""
 
     latest_version = fields.String()
```

### Comparing `renku-2.5.0rc3/renku/ui/service/serializers/workflows.py` & `renku-2.6.0rc1/renku/ui/service/serializers/workflows.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/utils/__init__.py` & `renku-2.6.0rc1/renku/ui/service/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/utils/callback.py` & `renku-2.6.0rc1/renku/ui/service/utils/callback.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/utils/json_encoder.py` & `renku-2.6.0rc1/renku/ui/service/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/utils/squash.py` & `renku-2.6.0rc1/renku/ui/service/utils/squash.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/utils/timeout.py` & `renku-2.6.0rc1/renku/ui/service/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/__init__.py` & `renku-2.6.0rc1/renku/ui/service/views/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/api_versions.py` & `renku-2.6.0rc1/renku/ui/service/views/api_versions.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/apispec.py` & `renku-2.6.0rc1/renku/ui/service/views/apispec.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/cache.py` & `renku-2.6.0rc1/renku/ui/service/views/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/config.py` & `renku-2.6.0rc1/renku/ui/service/views/config.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/datasets.py` & `renku-2.6.0rc1/renku/ui/service/views/datasets.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/decorators.py` & `renku-2.6.0rc1/renku/ui/service/views/decorators.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/error_handlers.py` & `renku-2.6.0rc1/renku/ui/service/views/error_handlers.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/graph.py` & `renku-2.6.0rc1/renku/ui/service/views/graph.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/jobs.py` & `renku-2.6.0rc1/renku/ui/service/views/jobs.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/project.py` & `renku-2.6.0rc1/renku/ui/service/views/project.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/templates.py` & `renku-2.6.0rc1/renku/ui/service/views/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/v1/__init__.py` & `renku-2.6.0rc1/renku/ui/service/views/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/v1/cache.py` & `renku-2.6.0rc1/renku/ui/service/views/v1/cache.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/v1/templates.py` & `renku-2.6.0rc1/renku/ui/service/views/v1/templates.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/version.py` & `renku-2.6.0rc1/renku/ui/service/views/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/views/workflow_plans.py` & `renku-2.6.0rc1/renku/ui/service/views/workflow_plans.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/ui/service/worker.py` & `renku-2.6.0rc1/renku/ui/service/worker.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/renku/version.py` & `renku-2.6.0rc1/renku/version.py`

 * *Files identical despite different names*

### Comparing `renku-2.5.0rc3/PKG-INFO` & `renku-2.6.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renku
-Version: 2.5.0rc3
+Version: 2.6.0rc1
 Summary: Python SDK and CLI for the Renku platform.
 Home-page: https://github.com/swissdatasciencecenter/renku-python
 License: Apache-2.0
 Keywords: Renku,CLI
 Author: Swiss Data Science Center
 Author-email: contact@datascience.ch
 Requires-Python: >=3.8.1,<3.12
@@ -31,15 +31,15 @@
 Requires-Dist: bashlex (>=0.16,<0.17)
 Requires-Dist: calamus (>=0.3.13,<0.5)
 Requires-Dist: circus (==0.18.0) ; extra == "service"
 Requires-Dist: click (>=8.0,<8.1.4)
 Requires-Dist: click-option-group (>=0.5.2,<0.6.0)
 Requires-Dist: click-plugins (==1.1.1)
 Requires-Dist: coverage[toml] (>=4.5.3,<6.5)
-Requires-Dist: cryptography (>=38.0.0,<41.0.0)
+Requires-Dist: cryptography (>=38.0.0,<42.0.0)
 Requires-Dist: cwl-utils (>=0.27,<0.28)
 Requires-Dist: cwltool (==3.1.20230425144158)
 Requires-Dist: deal (>=4.24.0,<5.0.0)
 Requires-Dist: deepdiff (>=5.8,<7.0)
 Requires-Dist: deepmerge (==1.0.1)
 Requires-Dist: docker (>=3.7.2,<6)
 Requires-Dist: filelock (>=3.3.0,<3.12.1)
@@ -72,21 +72,21 @@
 Requires-Dist: python-editor (==1.0.4)
 Requires-Dist: python-gitlab (>=2.10.1,<3.8.2)
 Requires-Dist: pyyaml (>=5.4,<6.1.0)
 Requires-Dist: rdflib (>=6.0.0,<7.0)
 Requires-Dist: redis (>=3.5.3,<4.6.0) ; extra == "service"
 Requires-Dist: requests (>=2.23.0,<2.31.1)
 Requires-Dist: rich (>=9.3.0,<13.4.0)
-Requires-Dist: rq (==1.14.1) ; extra == "service"
+Requires-Dist: rq (==1.15.0) ; extra == "service"
 Requires-Dist: rq-scheduler (==0.13.1) ; extra == "service"
-Requires-Dist: sentry-sdk[flask] (>=1.5.11,<1.24.0) ; extra == "service"
+Requires-Dist: sentry-sdk[flask] (>=1.5.11,<1.26.0) ; extra == "service"
 Requires-Dist: shellingham (==1.5.0.post1)
 Requires-Dist: tabulate (>=0.7.7,<0.9.1)
 Requires-Dist: toil (==5.10.0)
-Requires-Dist: tqdm (>=4.48.1,<4.62.4)
+Requires-Dist: tqdm (>=4.48.1,<4.65.1)
 Requires-Dist: walrus (>=0.8.2,<0.10.0) ; extra == "service"
 Requires-Dist: werkzeug (>=1.0.0,<2.2.4)
 Requires-Dist: yagup (>=0.1.1)
 Requires-Dist: yaspin (==2.1.0)
 Requires-Dist: zc.relation (>=1.1,<2.1)
 Requires-Dist: zodb (==5.8.0)
 Requires-Dist: zstandard (>=0.16.0,<0.22.0)
```

