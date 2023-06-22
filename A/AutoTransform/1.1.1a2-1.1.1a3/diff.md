# Comparing `tmp/AutoTransform-1.1.1a2.tar.gz` & `tmp/AutoTransform-1.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoTransform-1.1.1a2.tar", last modified: Mon Apr 10 12:23:29 2023, max compression
+gzip compressed data, was "AutoTransform-1.1.1a3.tar", last modified: Thu Jun 22 09:11:39 2023, max compression
```

## Comparing `AutoTransform-1.1.1a2.tar` & `AutoTransform-1.1.1a3.tar`

### file list

```diff
@@ -1,178 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.781783 AutoTransform-1.1.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/BEST_PRACTICES.md
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/COMPONENTS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/CUSTOM_DEPLOYMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/MANAGE_CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-10 12:23:29.781783 AutoTransform-1.1.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/SCHEDULED_RUNS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/examples/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/docker/docker_autotransform.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/manager.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/scheduler.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/examples/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/schemas/black_format.json
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/schemas/schema_map.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/examples/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/workflows/autotransform.manage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/workflows/autotransform.run.yml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/workflows/autotransform.schedule.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/workflows/autotransform.update.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:23:29.781783 AutoTransform-1.1.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.761783 AutoTransform-1.1.1a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.761783 AutoTransform-1.1.1a2/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/src/python/autotransform/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/batcher/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/codeowners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/extradata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/change/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/change/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/change/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/change/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/command/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/command/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/command/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/event/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/logginglevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/remoterun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/schedulerun.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/codeowners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/key_hash_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/shard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/input/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/gitgrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/inline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/item/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/item/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/item/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/repo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/repo/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/repo/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/schema/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/schema/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/step/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/step/action/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/created.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/conditional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/jscodeshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/libcst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/util/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/cachedfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18520 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/schema_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/validator/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/validator/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.577221 AutoTransform-1.1.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/BEST_PRACTICES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/COMPONENTS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/CUSTOM_DEPLOYMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/MANAGE_CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-22 09:11:39.577221 AutoTransform-1.1.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/SCHEDULED_RUNS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.557221 AutoTransform-1.1.1a3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.561221 AutoTransform-1.1.1a3/examples/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/docker/docker_autotransform.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/scheduler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.561221 AutoTransform-1.1.1a3/examples/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/schemas/black_format.json
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/schemas/schema_map.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.561221 AutoTransform-1.1.1a3/examples/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/workflows/autotransform.manage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/workflows/autotransform.run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/workflows/autotransform.schedule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/examples/workflows/autotransform.update.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:11:39.577221 AutoTransform-1.1.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.557221 AutoTransform-1.1.1a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.557221 AutoTransform-1.1.1a3/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.561221 AutoTransform-1.1.1a3/src/python/AutoTransform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-22 09:11:39.000000 AutoTransform-1.1.1a3/src/python/AutoTransform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-22 09:11:39.000000 AutoTransform-1.1.1a3/src/python/AutoTransform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:11:39.000000 AutoTransform-1.1.1a3/src/python/AutoTransform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-22 09:11:39.000000 AutoTransform-1.1.1a3/src/python/AutoTransform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 09:11:39.000000 AutoTransform-1.1.1a3/src/python/AutoTransform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 09:11:39.000000 AutoTransform-1.1.1a3/src/python/AutoTransform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.561221 AutoTransform-1.1.1a3/src/python/autotransform/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.561221 AutoTransform-1.1.1a3/src/python/autotransform/batcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/batcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/batcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/batcher/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/batcher/codeowners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/batcher/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/batcher/extradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/batcher/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/batcher/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.561221 AutoTransform-1.1.1a3/src/python/autotransform/change/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/change/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/change/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/change/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.561221 AutoTransform-1.1.1a3/src/python/autotransform/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/command/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.565221 AutoTransform-1.1.1a3/src/python/autotransform/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/config/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.565221 AutoTransform-1.1.1a3/src/python/autotransform/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/logginglevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/remoterun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/schedulerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/event/warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.565221 AutoTransform-1.1.1a3/src/python/autotransform/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/filter/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/filter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/filter/codeowners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/filter/key_hash_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/filter/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/filter/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/filter/shard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.569221 AutoTransform-1.1.1a3/src/python/autotransform/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/input/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/input/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/input/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/input/gitgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/input/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/input/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.569221 AutoTransform-1.1.1a3/src/python/autotransform/item/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/item/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/item/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.569221 AutoTransform-1.1.1a3/src/python/autotransform/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/repo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/repo/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/repo/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.569221 AutoTransform-1.1.1a3/src/python/autotransform/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/runner/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/runner/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/runner/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.569221 AutoTransform-1.1.1a3/src/python/autotransform/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/schema/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/schema/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.569221 AutoTransform-1.1.1a3/src/python/autotransform/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.569221 AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.573221 AutoTransform-1.1.1a3/src/python/autotransform/scripts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/migrations/p1_0_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/migrations/p1_0_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/scripts/migrations/p1_0_5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.573221 AutoTransform-1.1.1a3/src/python/autotransform/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.573221 AutoTransform-1.1.1a3/src/python/autotransform/step/action/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/action/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/action/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/action/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/action/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/action/reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/action/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.573221 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/condition/updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/step/conditional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.573221 AutoTransform-1.1.1a3/src/python/autotransform/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/transformer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/transformer/jscodeshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/transformer/libcst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/transformer/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/transformer/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/transformer/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.577221 AutoTransform-1.1.1a3/src/python/autotransform/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/cachedfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18520 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/util/schema_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:39.577221 AutoTransform-1.1.1a3/src/python/autotransform/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-06-22 09:10:40.000000 AutoTransform-1.1.1a3/src/python/autotransform/validator/script.py
```

### Comparing `AutoTransform-1.1.1a2/BEST_PRACTICES.md` & `AutoTransform-1.1.1a3/BEST_PRACTICES.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/COMPONENTS.md` & `AutoTransform-1.1.1a3/COMPONENTS.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/CONTRIBUTING.md` & `AutoTransform-1.1.1a3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/CUSTOM_DEPLOYMENT.md` & `AutoTransform-1.1.1a3/CUSTOM_DEPLOYMENT.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/LICENSE` & `AutoTransform-1.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/MANAGE_CHANGES.md` & `AutoTransform-1.1.1a3/MANAGE_CHANGES.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/PKG-INFO` & `AutoTransform-1.1.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoTransform
-Version: 1.1.1a2
+Version: 1.1.1a3
 Summary: A component based framework for designing automated code modification
 Home-page: https://github.com/nathro/AutoTransform
 Author: Nathan Rockenbach
 Author-email: nathro.software@gmail.com
 Project-URL: Source, https://github.com/nathro/AutoTransform/
 Project-URL: Bug Tracker, https://github.com/nathro/AutoTransform/issues
 Keywords: codemod,automation,code change,codeshift,transformation,maintain
```

### Comparing `AutoTransform-1.1.1a2/README.md` & `AutoTransform-1.1.1a3/README.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/SCHEDULED_RUNS.md` & `AutoTransform-1.1.1a3/SCHEDULED_RUNS.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/examples/docker/docker_autotransform.sh` & `AutoTransform-1.1.1a3/examples/docker/docker_autotransform.sh`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/examples/docker/entrypoint.sh` & `AutoTransform-1.1.1a3/examples/docker/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/examples/manager.json` & `AutoTransform-1.1.1a3/examples/manager.json`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/examples/schemas/black_format.json` & `AutoTransform-1.1.1a3/examples/schemas/black_format.json`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/examples/workflows/autotransform.manage.yml` & `AutoTransform-1.1.1a3/examples/workflows/autotransform.manage.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/examples/workflows/autotransform.run.yml` & `AutoTransform-1.1.1a3/examples/workflows/autotransform.run.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/examples/workflows/autotransform.schedule.yml` & `AutoTransform-1.1.1a3/examples/workflows/autotransform.schedule.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/examples/workflows/autotransform.update.yml` & `AutoTransform-1.1.1a3/examples/workflows/autotransform.update.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/setup.py` & `AutoTransform-1.1.1a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         data_files.append((f"autotransform-{path}", [os.path.join(path, file) for file in files]))
 
     return data_files
 
 
 setuptools.setup(
     name="AutoTransform",
-    version="1.1.1a2",
+    version="1.1.1a3",
     author="Nathan Rockenbach",
     author_email="nathro.software@gmail.com",
     description="A component based framework for designing automated code modification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nathro/AutoTransform",
     project_urls={
```

### Comparing `AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/PKG-INFO` & `AutoTransform-1.1.1a3/src/python/AutoTransform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoTransform
-Version: 1.1.1a2
+Version: 1.1.1a3
 Summary: A component based framework for designing automated code modification
 Home-page: https://github.com/nathro/AutoTransform
 Author: Nathan Rockenbach
 Author-email: nathro.software@gmail.com
 Project-URL: Source, https://github.com/nathro/AutoTransform/
 Project-URL: Bug Tracker, https://github.com/nathro/AutoTransform/issues
 Keywords: codemod,automation,code change,codeshift,transformation,maintain
```

### Comparing `AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/SOURCES.txt` & `AutoTransform-1.1.1a3/src/python/AutoTransform.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,21 +62,23 @@
 src/python/autotransform/event/warning.py
 src/python/autotransform/filter/__init__.py
 src/python/autotransform/filter/aggregate.py
 src/python/autotransform/filter/base.py
 src/python/autotransform/filter/codeowners.py
 src/python/autotransform/filter/key_hash_shard.py
 src/python/autotransform/filter/regex.py
+src/python/autotransform/filter/script.py
 src/python/autotransform/filter/shard.py
 src/python/autotransform/input/__init__.py
 src/python/autotransform/input/base.py
 src/python/autotransform/input/directory.py
 src/python/autotransform/input/empty.py
 src/python/autotransform/input/gitgrep.py
 src/python/autotransform/input/inline.py
+src/python/autotransform/input/script.py
 src/python/autotransform/item/__init__.py
 src/python/autotransform/item/base.py
 src/python/autotransform/item/file.py
 src/python/autotransform/repo/__init__.py
 src/python/autotransform/repo/base.py
 src/python/autotransform/repo/git.py
 src/python/autotransform/repo/github.py
```

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/__init__.py` & `AutoTransform-1.1.1a3/src/python/autotransform/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/batcher/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/batcher/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/batcher/chunk.py` & `AutoTransform-1.1.1a3/src/python/autotransform/batcher/chunk.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/batcher/codeowners.py` & `AutoTransform-1.1.1a3/src/python/autotransform/batcher/codeowners.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/batcher/directory.py` & `AutoTransform-1.1.1a3/src/python/autotransform/batcher/directory.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/batcher/extradata.py` & `AutoTransform-1.1.1a3/src/python/autotransform/batcher/extradata.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/batcher/regex.py` & `AutoTransform-1.1.1a3/src/python/autotransform/batcher/regex.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/batcher/single.py` & `AutoTransform-1.1.1a3/src/python/autotransform/batcher/single.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/change/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/change/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/change/github.py` & `AutoTransform-1.1.1a3/src/python/autotransform/change/github.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/command/__init__.py` & `AutoTransform-1.1.1a3/src/python/autotransform/command/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/command/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/command/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/command/script.py` & `AutoTransform-1.1.1a3/src/python/autotransform/command/script.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/config/__init__.py` & `AutoTransform-1.1.1a3/src/python/autotransform/config/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/config/config.py` & `AutoTransform-1.1.1a3/src/python/autotransform/config/config.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/config/default.py` & `AutoTransform-1.1.1a3/src/python/autotransform/config/default.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/config/environment.py` & `AutoTransform-1.1.1a3/src/python/autotransform/config/environment.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/config/fetcher.py` & `AutoTransform-1.1.1a3/src/python/autotransform/config/fetcher.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/__init__.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/action.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/action.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/debug.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/debug.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/handler.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/handler.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/logginglevel.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/logginglevel.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/remoterun.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/remoterun.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/run.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/run.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/schedulerun.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/schedulerun.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/type.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/type.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/update.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/update.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/verbose.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/verbose.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/event/warning.py` & `AutoTransform-1.1.1a3/src/python/autotransform/event/warning.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/filter/aggregate.py` & `AutoTransform-1.1.1a3/src/python/autotransform/filter/aggregate.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/filter/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/runner/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,89 +3,74 @@
 #
 # Licensed under the MIT License <http://opensource.org/licenses/MIT>
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2022-present Nathan Rockenbach <http://github.com/nathro>
 
 # @black_format
 
-"""The base class and associated classes for Filter components."""
+"""The base class and associated classes for Runner components."""
 
 from __future__ import annotations
 
 from abc import abstractmethod
 from enum import Enum
 from typing import ClassVar
 
-from autotransform.item.base import Item
+from autotransform.change.base import Change
+from autotransform.schema.schema import AutoTransformSchema
 from autotransform.util.component import ComponentFactory, ComponentImport, NamedComponent
 
 
-class FilterName(str, Enum):
+class RunnerName(str, Enum):
     """A simple enum for mapping."""
 
-    AGGREGATE = "aggregate"
-    CODEOWNERS = "codeowners"
-    REGEX = "regex"
-    REGEX_FILE_CONTENT = "regex_file_content"
-
-    # Shard Filters
-    KEY_HASH_SHARD = "key_hash_shard"
+    GITHUB = "github"
+    JENKINS_API = "jenkins_api"
+    JENKINS_FILE = "jenkins_file"
+    LOCAL = "local"
 
 
-class Filter(NamedComponent):
-    """The base for Filter components. Used by AutoTransform to determine if an Item from an Input
-    is eligible for transformation.
+class Runner(NamedComponent):
+    """The base for Runner components. Used by AutoTransform to run an AutoTransformSchema,
+    either locally on the machine or on remote infrastructure.
 
     Attributes:
-        inverted (bool, optional): Whether to invert the results of the filter. Defaults to False.
-        name (ClassVar[FilterName]): The name of the component.
+        name (ClassVar[RunnerName]): The name of the component.
     """
 
-    inverted: bool = False
+    name: ClassVar[RunnerName]
 
-    name: ClassVar[FilterName]
-
-    def is_valid(self, item: Item) -> bool:
-        """Check whether an Item is valid based on the Filter and handle inversion.
+    @abstractmethod
+    def run(self, schema: AutoTransformSchema) -> None:
+        """Triggers a full run of a Schema.
 
         Args:
-            item (Item): The Item to check.
-
-        Returns:
-            bool: Returns True if the Item is eligible for transformation.
+            schema (AutoTransformSchema): The schema that will be run.
         """
 
-        return self.inverted != self._is_valid(item)
-
     @abstractmethod
-    def _is_valid(self, item: Item) -> bool:
-        """Check whether an Item is valid based on the Filter. Does not handle inversion.
+    def update(self, change: Change) -> None:
+        """Triggers an update of the Change.
 
         Args:
-            item (Item): The Item to check.
-
-        Returns:
-            bool: Returns True if the Item is eligible for transformation.
+            change (Change): The Change to update.
         """
 
 
 FACTORY = ComponentFactory(
     {
-        FilterName.AGGREGATE: ComponentImport(
-            class_name="AggregateFilter", module="autotransform.filter.aggregate"
-        ),
-        FilterName.CODEOWNERS: ComponentImport(
-            class_name="CodeownersFilter", module="autotransform.filter.codeowners"
+        RunnerName.GITHUB: ComponentImport(
+            class_name="GithubRunner", module="autotransform.runner.github"
         ),
-        FilterName.REGEX: ComponentImport(
-            class_name="RegexFilter", module="autotransform.filter.regex"
+        RunnerName.JENKINS_API: ComponentImport(
+            class_name="JenkinsAPIRunner", module="autotransform.runner.jenkins"
         ),
-        FilterName.REGEX_FILE_CONTENT: ComponentImport(
-            class_name="RegexFileContentFilter", module="autotransform.filter.regex"
+        RunnerName.JENKINS_FILE: ComponentImport(
+            class_name="JenkinsFileRunner", module="autotransform.runner.jenkins"
         ),
-        FilterName.KEY_HASH_SHARD: ComponentImport(
-            class_name="KeyHashShardFilter", module="autotransform.filter.key_hash_shard"
+        RunnerName.LOCAL: ComponentImport(
+            class_name="LocalRunner", module="autotransform.runner.local"
         ),
     },
-    Filter,  # type: ignore [type-abstract]
-    "filter.json",
+    Runner,  # type: ignore [type-abstract]
+    "runner.json",
 )
```

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/filter/codeowners.py` & `AutoTransform-1.1.1a3/src/python/autotransform/filter/codeowners.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/filter/key_hash_shard.py` & `AutoTransform-1.1.1a3/src/python/autotransform/filter/key_hash_shard.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/filter/regex.py` & `AutoTransform-1.1.1a3/src/python/autotransform/filter/regex.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/filter/shard.py` & `AutoTransform-1.1.1a3/src/python/autotransform/filter/shard.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/input/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/input/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     DIRECTORY = "directory"
     EMPTY = "empty"
     GIT_GREP = "git_grep"
     INLINE = "inline"
     INLINE_FILE = "inline_file"
     INLINE_GENERIC = "inline_generic"
+    SCRIPT = "script"
 
 
 class Input(NamedComponent):
     """The base for Input components. Used by AutoTransform to get Items that
     represent potentially transformable units for a Schema. Usually returns files but
     any Item can be returned as long as Schema components work with it.
 
@@ -67,11 +68,14 @@
         ),
         InputName.INLINE_FILE: ComponentImport(
             class_name="InlineFileInput", module="autotransform.input.inline"
         ),
         InputName.INLINE_GENERIC: ComponentImport(
             class_name="InlineGenericInput", module="autotransform.input.inline"
         ),
+        InputName.SCRIPT: ComponentImport(
+            class_name="ScriptInput", module="autotransform.input.script"
+        ),
     },
     Input,  # type: ignore [type-abstract]
     "input.json",
 )
```

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/input/directory.py` & `AutoTransform-1.1.1a3/src/python/autotransform/input/directory.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/input/empty.py` & `AutoTransform-1.1.1a3/src/python/autotransform/input/empty.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/input/gitgrep.py` & `AutoTransform-1.1.1a3/src/python/autotransform/input/gitgrep.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/input/inline.py` & `AutoTransform-1.1.1a3/src/python/autotransform/input/inline.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/item/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/item/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/item/file.py` & `AutoTransform-1.1.1a3/src/python/autotransform/item/file.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/repo/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/repo/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/repo/git.py` & `AutoTransform-1.1.1a3/src/python/autotransform/repo/git.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/repo/github.py` & `AutoTransform-1.1.1a3/src/python/autotransform/repo/github.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/runner/github.py` & `AutoTransform-1.1.1a3/src/python/autotransform/runner/github.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/runner/jenkins.py` & `AutoTransform-1.1.1a3/src/python/autotransform/runner/jenkins.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/runner/local.py` & `AutoTransform-1.1.1a3/src/python/autotransform/runner/local.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/schema/__init__.py` & `AutoTransform-1.1.1a3/src/python/autotransform/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/schema/builder.py` & `AutoTransform-1.1.1a3/src/python/autotransform/schema/builder.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/schema/config.py` & `AutoTransform-1.1.1a3/src/python/autotransform/schema/config.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/schema/schema.py` & `AutoTransform-1.1.1a3/src/python/autotransform/schema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from autotransform.change.base import Change
 from autotransform.command.base import FACTORY as command_factory
 from autotransform.command.base import Command
 from autotransform.event.debug import DebugEvent
 from autotransform.event.handler import EventHandler
 from autotransform.event.verbose import VerboseEvent
 from autotransform.filter.base import FACTORY as filter_factory
-from autotransform.filter.base import Filter
+from autotransform.filter.base import BulkFilter, Filter
 from autotransform.input.base import FACTORY as input_factory
 from autotransform.input.base import Input
 from autotransform.item.base import Item
 from autotransform.repo.base import FACTORY as repo_factory
 from autotransform.repo.base import Repo
 from autotransform.schema.config import SchemaConfig
 from autotransform.transformer.base import FACTORY as transformer_factory
@@ -89,14 +89,17 @@
         item_str = "\n".join([f"{item!r}," for item in all_items])
         event_handler.handle(VerboseEvent({"message": f"Num Items: {len(all_items)}"}))
         event_handler.handle(DebugEvent({"message": f"Items: [\n{item_str}\n]"}))
 
         # Filter Items
         event_handler.handle(VerboseEvent({"message": "Begin filters"}))
         valid_items: List[Item] = []
+        for filt in self.filters:
+            if isinstance(filt, BulkFilter):
+                filt.pre_process(all_items)
         for item in all_items:
             is_valid = True
             for cur_filter in self.filters:
                 if not cur_filter.is_valid(item):
                     is_valid = False
                     event = DebugEvent({"message": f"[{cur_filter}] Invalid Item: {item!r}"})
                     event_handler.handle(event)
```

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/initialize.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/initialize.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/manage.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/manage.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/run.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/run.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/schedule.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/schedule.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/settings.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/settings.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/update.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/commands/update.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/main.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/main.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_1.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/migrations/p1_0_1.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_3.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/migrations/p1_0_3.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_5.py` & `AutoTransform-1.1.1a3/src/python/autotransform/scripts/migrations/p1_0_5.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/action/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/action/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/action/comments.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/action/comments.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/action/labels.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/action/labels.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/action/request.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/action/request.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/action/reviewers.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/action/reviewers.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/action/source.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/action/source.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/aggregate.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/aggregate.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/comparison.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/comparison.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/created.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/created.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/labels.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/labels.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/request.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/request.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/reviewers.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/reviewers.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/schema.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/schema.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/state.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/state.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/updated.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/condition/updated.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/step/conditional.py` & `AutoTransform-1.1.1a3/src/python/autotransform/step/conditional.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/transformer/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/transformer/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/transformer/jscodeshift.py` & `AutoTransform-1.1.1a3/src/python/autotransform/transformer/jscodeshift.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/transformer/libcst.py` & `AutoTransform-1.1.1a3/src/python/autotransform/transformer/libcst.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/transformer/regex.py` & `AutoTransform-1.1.1a3/src/python/autotransform/transformer/regex.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/transformer/script.py` & `AutoTransform-1.1.1a3/src/python/autotransform/transformer/script.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/transformer/single.py` & `AutoTransform-1.1.1a3/src/python/autotransform/transformer/single.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/cachedfile.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/cachedfile.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/component.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/component.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/console.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/console.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/enums.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/enums.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/functions.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/functions.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/github.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/github.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/manager.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/manager.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/package.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/package.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/request.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/request.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/scheduler.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/util/schema_map.py` & `AutoTransform-1.1.1a3/src/python/autotransform/util/schema_map.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/validator/base.py` & `AutoTransform-1.1.1a3/src/python/autotransform/validator/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a2/src/python/autotransform/validator/script.py` & `AutoTransform-1.1.1a3/src/python/autotransform/validator/script.py`

 * *Files identical despite different names*

