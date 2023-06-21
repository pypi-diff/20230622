# Comparing `tmp/awsebcli-3.9.0.tar.gz` & `tmp/awsebcli-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awsebcli-3.9.0.tar", last modified: Thu Dec 22 23:47:51 2016, max compression
+gzip compressed data, was "dist/awsebcli-3.9.1.tar", last modified: Thu Feb  9 01:15:32 2017, max compression
```

## Comparing `awsebcli-3.9.0.tar` & `awsebcli-3.9.1.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/awsebcli.egg-info/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        1 2016-12-22 23:47:50.000000 awsebcli-3.9.0/awsebcli.egg-info/dependency_links.txt
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)       47 2016-12-22 23:47:50.000000 awsebcli-3.9.0/awsebcli.egg-info/entry_points.txt
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    22683 2016-12-22 23:47:50.000000 awsebcli-3.9.0/awsebcli.egg-info/PKG-INFO
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      296 2016-12-22 23:47:50.000000 awsebcli-3.9.0/awsebcli.egg-info/requires.txt
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5593 2016-12-22 23:47:51.000000 awsebcli-3.9.0/awsebcli.egg-info/SOURCES.txt
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)       10 2016-12-22 23:47:50.000000 awsebcli-3.9.0/awsebcli.egg-info/top_level.txt
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/bin/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      562 2016-12-22 21:13:20.000000 awsebcli-3.9.0/bin/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      710 2016-12-22 21:13:20.000000 awsebcli-3.9.0/bin/eb
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      280 2016-12-22 21:13:20.000000 awsebcli-3.9.0/bin/eb_completion.bash
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3776 2016-12-22 21:13:20.000000 awsebcli-3.9.0/bin/install-ebcli.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    10318 2016-12-22 21:13:20.000000 awsebcli-3.9.0/CHANGES.rst
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)       27 2016-12-22 21:13:20.000000 awsebcli-3.9.0/dev_requirements.txt
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      615 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/__init__.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/bundled/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/__init__.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/bundled/_compose/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      110 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/__init__.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      821 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/colors.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4822 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/command.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1124 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/docker_client.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1556 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/docopt_command.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1920 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/errors.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      392 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/formatter.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2642 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/log_printer.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    17455 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/main.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1017 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/multiplexer.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3319 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/utils.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1691 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/cli/verbose_proxy.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    12416 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/config.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5274 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/container.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2322 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/progress_stream.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     9650 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/project.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    22719 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/bundled/_compose/service.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/containers/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      561 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5053 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/abstractcontainer.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     8658 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/commands.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3484 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/compat.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5212 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/compose.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2716 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/container_viewmodel.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/containers/containerfiles/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1541 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/containerfiles/container_config.json
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)       64 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/containerfiles/glassfish-runtime-4.0-jdk7
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)       64 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/containerfiles/glassfish-runtime-4.1-jdk8
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)       52 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/containerfiles/golang-runtime-1.3
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)       52 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/containerfiles/golang-runtime-1.4
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)       58 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/containerfiles/python3-runtime
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3921 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/containerops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5120 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/dockerrun.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2311 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/envvarcollector.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4711 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/factory.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5390 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/fshandler.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1347 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/generic_container.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3544 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/log.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2306 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/multicontainer.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1622 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/pathconfig.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3031 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/containers/preconfigured_container.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/controllers/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      562 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1913 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/abort.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2295 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/appversion.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5396 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/clone.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2208 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/codesource.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5249 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/config.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1081 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/console.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    18430 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/create.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     7976 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/deploy.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1304 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/events.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1641 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/health.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    25703 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/initialize.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1599 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/lifecycle.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1592 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/list.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5359 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/local.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5439 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/logs.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1050 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/open.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4619 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/platform.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1089 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/printenv.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1776 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/restore.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2113 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/scale.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1900 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/setenv.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4292 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/ssh.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1108 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/status.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2189 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/swap.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3270 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/terminate.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1584 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/upgrade.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2715 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/controllers/use.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/core/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      562 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5752 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/abstractcontroller.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2266 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/arghandler.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3143 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/base.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4699 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/completer.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     6687 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/ebcore.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      586 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/ebglobals.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2275 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/ebrun.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    28676 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/fileoperations.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1950 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/hooks.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    10216 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/core/io.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/display/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      562 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    13033 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/appversion.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    11867 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/data_poller.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    10409 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/environments.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2793 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/help.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    17907 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/screen.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3210 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/specialtables.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     9158 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/table.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     9411 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/term.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4101 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/display/traditional.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/labs/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      562 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3593 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/cleanupversions.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/labs/cloudwatchfiles/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2311 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/cloudwatchfiles/cwl-activity-logs-v1.config
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5315 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/cloudwatchfiles/cwl-setup-v1.config
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1516 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/cloudwatchfiles/eb-logs-v1.config
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2480 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/cloudwatchsetup.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2409 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/controller.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4058 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/convertdockerrun.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3170 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/download.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4179 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/quicklink.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     6703 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/labs/setupssl.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/lib/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      562 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    11166 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/aws.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/codebuild/
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/codebuild/2016-10-06/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    17131 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/codebuild/2016-10-06/service-2.json
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/elasticbeanstalk/
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/elasticbeanstalk/2010-12-01/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      187 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/elasticbeanstalk/2010-12-01/paginators-1.json
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)   100657 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/elasticbeanstalk/2010-12-01/service-2.json
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/elbv2/
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/elbv2/2015-12-01/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)   115731 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/botocoredata/elbv2/2015-12-01/service-2.json
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2637 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/botopatch.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      948 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/cloudformation.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2233 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/cloudwatch.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3737 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/codebuild.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5070 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/codecommit.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3903 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/ec2.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    23312 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/elasticbeanstalk.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1447 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/elb.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2545 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/elbv2.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3481 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/heuristics.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3696 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/iam.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     9702 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/s3.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     9493 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/lib/utils.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/objects/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      562 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      992 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/application.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1052 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/buildconfiguration.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1869 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/conversionconfiguration.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1514 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/environment.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     6751 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/environmentsettings.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      949 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/event.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3574 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/exceptions.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3507 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/lifecycleconfiguration.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1602 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/region.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    11059 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/requests.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2985 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/solutionstack.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    16728 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/sourcecontrol.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2564 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/objects/tier.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/operations/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      562 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1027 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/abortops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4129 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/appversionops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5225 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/buildspecops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2573 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/cloneops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    41749 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/commonops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1778 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/composeops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2362 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/configops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1529 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/consoleops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    11568 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/createops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3616 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/deployops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1971 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/envvarops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1626 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/eventsops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5705 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/gitops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4810 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/healthops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3521 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/initializeops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3287 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/lifecycleops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1770 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/listops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4551 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/localops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    15652 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/logsops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1237 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/openops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      822 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/platformops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3952 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/restoreops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     6876 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/saved_configs.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2296 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/scaleops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5654 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/sshops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     4907 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/statusops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      855 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/swapops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3690 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/terminateops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     3792 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/upgradeops.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     1312 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/operations/useops.py
-drwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)        0 2016-12-22 23:47:51.000000 awsebcli-3.9.0/ebcli/resources/
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      562 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/resources/__init__.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     2799 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/resources/statics.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    37388 2016-12-22 21:13:20.000000 awsebcli-3.9.0/ebcli/resources/strings.py
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     9489 2016-12-22 21:13:20.000000 awsebcli-3.9.0/LICENSE.txt
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)      115 2016-12-22 21:13:20.000000 awsebcli-3.9.0/MANIFEST.in
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)    22683 2016-12-22 23:47:51.000000 awsebcli-3.9.0/PKG-INFO
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     7067 2016-12-22 21:13:20.000000 awsebcli-3.9.0/README.rst
--rw-r--r--   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)       59 2016-12-22 23:47:51.000000 awsebcli-3.9.0/setup.cfg
--rwxr-xr-x   0 yueyanm  (2112670236) ANT\Domain Users (1896053708)     5241 2016-12-22 21:13:20.000000 awsebcli-3.9.0/setup.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/awsebcli.egg-info/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        1 2017-02-09 01:15:32.000000 awsebcli-3.9.1/awsebcli.egg-info/dependency_links.txt
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)       47 2017-02-09 01:15:32.000000 awsebcli-3.9.1/awsebcli.egg-info/entry_points.txt
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    23252 2017-02-09 01:15:32.000000 awsebcli-3.9.1/awsebcli.egg-info/PKG-INFO
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      296 2017-02-09 01:15:32.000000 awsebcli-3.9.1/awsebcli.egg-info/requires.txt
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5593 2017-02-09 01:15:32.000000 awsebcli-3.9.1/awsebcli.egg-info/SOURCES.txt
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)       10 2017-02-09 01:15:32.000000 awsebcli-3.9.1/awsebcli.egg-info/top_level.txt
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/bin/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      562 2017-01-24 01:36:29.000000 awsebcli-3.9.1/bin/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      710 2016-07-28 15:48:38.000000 awsebcli-3.9.1/bin/eb
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      280 2016-05-18 18:32:54.000000 awsebcli-3.9.1/bin/eb_completion.bash
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3776 2017-01-04 04:27:33.000000 awsebcli-3.9.1/bin/install-ebcli.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    10757 2017-02-07 00:30:04.000000 awsebcli-3.9.1/CHANGES.rst
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)       27 2017-01-24 01:36:58.000000 awsebcli-3.9.1/dev_requirements.txt
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      615 2017-01-24 01:36:29.000000 awsebcli-3.9.1/ebcli/__init__.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/bundled/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/__init__.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/bundled/_compose/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      110 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/__init__.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      821 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/colors.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4822 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/command.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1124 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/docker_client.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1556 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/docopt_command.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1920 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/errors.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      392 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/formatter.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2642 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/log_printer.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    17455 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/main.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1017 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/multiplexer.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3319 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/utils.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1691 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/cli/verbose_proxy.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    12416 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/config.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5274 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/container.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2322 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/progress_stream.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     9650 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/project.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    22719 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/bundled/_compose/service.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/containers/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      561 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5053 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/abstractcontainer.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     8658 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/commands.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3484 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/compat.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5212 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/compose.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2716 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/container_viewmodel.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/containers/containerfiles/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1541 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/containerfiles/container_config.json
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)       64 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/containerfiles/glassfish-runtime-4.0-jdk7
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)       64 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/containerfiles/glassfish-runtime-4.1-jdk8
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)       52 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/containerfiles/golang-runtime-1.3
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)       52 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/containerfiles/golang-runtime-1.4
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)       58 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/containerfiles/python3-runtime
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3921 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/containerops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5120 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/dockerrun.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2311 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/envvarcollector.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4711 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/factory.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5390 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/fshandler.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1347 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/generic_container.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3544 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/log.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2306 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/multicontainer.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1622 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/pathconfig.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3031 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/containers/preconfigured_container.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/controllers/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      562 2016-09-07 22:04:24.000000 awsebcli-3.9.1/ebcli/controllers/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1913 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/abort.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2295 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/controllers/appversion.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5396 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/clone.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2208 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/codesource.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5249 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/config.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1081 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/console.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    18595 2017-02-06 22:53:47.000000 awsebcli-3.9.1/ebcli/controllers/create.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     8151 2017-02-06 21:24:17.000000 awsebcli-3.9.1/ebcli/controllers/deploy.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1304 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/events.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1641 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/health.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    25326 2017-01-24 01:36:29.000000 awsebcli-3.9.1/ebcli/controllers/initialize.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1599 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/controllers/lifecycle.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1592 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/list.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5359 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/local.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5439 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/controllers/logs.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1050 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/open.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4619 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/platform.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1089 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/printenv.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1776 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/controllers/restore.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2113 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/scale.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1900 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/setenv.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4292 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/ssh.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1108 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/status.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2189 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/swap.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3270 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/terminate.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1584 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/upgrade.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2715 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/controllers/use.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/core/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      562 2016-09-07 22:04:24.000000 awsebcli-3.9.1/ebcli/core/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5752 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/core/abstractcontroller.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2266 2016-09-07 22:04:24.000000 awsebcli-3.9.1/ebcli/core/arghandler.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3143 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/core/base.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4699 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/core/completer.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     6717 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/core/ebcore.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      586 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/core/ebglobals.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2275 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/core/ebrun.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    28887 2017-01-24 01:36:29.000000 awsebcli-3.9.1/ebcli/core/fileoperations.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1950 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/core/hooks.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    10216 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/core/io.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/display/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      562 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    13033 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/appversion.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    11867 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/data_poller.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    10409 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/environments.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2793 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/help.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    17907 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/screen.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3210 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/specialtables.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     9158 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/table.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     9411 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/term.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4101 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/display/traditional.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/labs/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      562 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/labs/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3593 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/labs/cleanupversions.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/labs/cloudwatchfiles/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2311 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/labs/cloudwatchfiles/cwl-activity-logs-v1.config
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5315 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/labs/cloudwatchfiles/cwl-setup-v1.config
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1516 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/labs/cloudwatchfiles/eb-logs-v1.config
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2480 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/labs/cloudwatchsetup.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2409 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/labs/controller.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4058 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/labs/convertdockerrun.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3170 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/labs/download.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4179 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/labs/quicklink.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     6703 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/labs/setupssl.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/lib/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      562 2016-09-07 22:04:24.000000 awsebcli-3.9.1/ebcli/lib/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    11166 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/aws.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/codebuild/
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/codebuild/2016-10-06/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    17131 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/codebuild/2016-10-06/service-2.json
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/elasticbeanstalk/
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/elasticbeanstalk/2010-12-01/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      187 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/elasticbeanstalk/2010-12-01/paginators-1.json
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)   100657 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/elasticbeanstalk/2010-12-01/service-2.json
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/elbv2/
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/elbv2/2015-12-01/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)   115731 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/botocoredata/elbv2/2015-12-01/service-2.json
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2637 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/botopatch.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      948 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/cloudformation.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2233 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/lib/cloudwatch.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3734 2017-01-24 01:36:29.000000 awsebcli-3.9.1/ebcli/lib/codebuild.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5070 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/codecommit.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3903 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/ec2.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    23458 2017-01-07 00:10:14.000000 awsebcli-3.9.1/ebcli/lib/elasticbeanstalk.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1447 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/elb.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2545 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/elbv2.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3481 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/heuristics.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3696 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/lib/iam.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     9702 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/lib/s3.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     9660 2017-01-24 01:36:29.000000 awsebcli-3.9.1/ebcli/lib/utils.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/objects/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      562 2016-09-07 22:04:24.000000 awsebcli-3.9.1/ebcli/objects/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      992 2016-09-07 22:04:24.000000 awsebcli-3.9.1/ebcli/objects/application.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1052 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/objects/buildconfiguration.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1869 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/objects/conversionconfiguration.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1514 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/objects/environment.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     6751 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/objects/environmentsettings.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      949 2016-10-13 18:42:06.000000 awsebcli-3.9.1/ebcli/objects/event.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3574 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/objects/exceptions.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3507 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/objects/lifecycleconfiguration.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1602 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/objects/region.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    11059 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/objects/requests.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2985 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/objects/solutionstack.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    16665 2017-01-24 01:36:29.000000 awsebcli-3.9.1/ebcli/objects/sourcecontrol.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2564 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/objects/tier.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/operations/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      562 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1027 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/abortops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4129 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/operations/appversionops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5225 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/buildspecops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2573 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/cloneops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    41749 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/operations/commonops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1778 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/composeops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2362 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/operations/configops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1529 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/consoleops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    11568 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/createops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3616 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/operations/deployops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1971 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/envvarops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1626 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/eventsops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5705 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/gitops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4810 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/operations/healthops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3521 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/initializeops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3287 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/operations/lifecycleops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1770 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/listops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4551 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/localops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    15582 2017-01-24 01:36:29.000000 awsebcli-3.9.1/ebcli/operations/logsops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1237 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/openops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      822 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/platformops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3952 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/operations/restoreops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     7332 2017-02-03 22:17:43.000000 awsebcli-3.9.1/ebcli/operations/saved_configs.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2296 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/scaleops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5654 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/sshops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     4907 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/statusops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      855 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/swapops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3690 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/operations/terminateops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     3792 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/upgradeops.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     1312 2017-01-04 04:27:33.000000 awsebcli-3.9.1/ebcli/operations/useops.py
+drwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)        0 2017-02-09 01:15:32.000000 awsebcli-3.9.1/ebcli/resources/
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      562 2016-09-07 22:04:24.000000 awsebcli-3.9.1/ebcli/resources/__init__.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     2799 2017-01-04 04:29:46.000000 awsebcli-3.9.1/ebcli/resources/statics.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    38718 2017-02-06 21:12:17.000000 awsebcli-3.9.1/ebcli/resources/strings.py
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     9489 2016-05-18 18:32:54.000000 awsebcli-3.9.1/LICENSE.txt
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)      115 2017-01-04 04:29:46.000000 awsebcli-3.9.1/MANIFEST.in
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)    23252 2017-02-09 01:15:32.000000 awsebcli-3.9.1/PKG-INFO
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     7067 2017-01-04 04:27:33.000000 awsebcli-3.9.1/README.rst
+-rw-r--r--   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)       59 2017-02-09 01:15:32.000000 awsebcli-3.9.1/setup.cfg
+-rwxr-xr-x   0 nbbalas  (2025313535) ANT\Domain Users (1896053708)     5302 2017-01-24 01:36:29.000000 awsebcli-3.9.1/setup.py
```

### Comparing `awsebcli-3.9.0/awsebcli.egg-info/PKG-INFO` & `awsebcli-3.9.1/awsebcli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: awsebcli
-Version: 3.9.0
+Version: 3.9.1
 Summary: Command Line Interface for AWS EB.
 Home-page: http://aws.amazon.com/elasticbeanstalk/
 Author: AWS Elastic Beanstalk
 Author-email: aws-eb-cli@amazon.com
 License: Apache License 2.0
 Description: ======
         EB-CLI
@@ -243,14 +243,24 @@
         Now whenever you switch to a new branch, your default environment will also switch.
         
         
         =========
         Changelog
         =========
         ------------------
+        3.9.1 (2017-02-08)
+        ------------------
+        - Changed Beanstalk CodeBuild integration to be optional by not specifying the header in buildspec
+        - Fixed 'eb config put' to update DateModified field
+        - Fixed 'eb config put' full path failure
+        - Fixed exit codes to return correctly
+        - Removed CodeCommit failed prompt in eb init to avoid confusion
+        - Added 'process' flag for eb create/deploy for preprocessing application versions
+        
+        ------------------
         3.9.0 (2016-12-22)
         ------------------
         - Added native support in 'eb logs' for log streaming.
         - Added '--log-group' and '--cloudwatch-logs' flags in 'eb logs'
         - Added 'appversion' command to managed application versions
         - Added 'appversion lifecycle' sub command to manage application lifecycle configurations
         
@@ -585,7 +595,8 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
```

### Comparing `awsebcli-3.9.0/awsebcli.egg-info/SOURCES.txt` & `awsebcli-3.9.1/awsebcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/bin/__init__.py` & `awsebcli-3.9.1/ebcli/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/bin/eb` & `awsebcli-3.9.1/bin/eb`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/bin/install-ebcli.py` & `awsebcli-3.9.1/bin/install-ebcli.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/CHANGES.rst` & `awsebcli-3.9.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
 Changelog
 =========
 ------------------
+3.9.1 (2017-02-08)
+------------------
+- Changed Beanstalk CodeBuild integration to be optional by not specifying the header in buildspec
+- Fixed 'eb config put' to update DateModified field
+- Fixed 'eb config put' full path failure
+- Fixed exit codes to return correctly
+- Removed CodeCommit failed prompt in eb init to avoid confusion
+- Added 'process' flag for eb create/deploy for preprocessing application versions
+
+------------------
 3.9.0 (2016-12-22)
 ------------------
 - Added native support in 'eb logs' for log streaming.
 - Added '--log-group' and '--cloudwatch-logs' flags in 'eb logs'
 - Added 'appversion' command to managed application versions
 - Added 'appversion lifecycle' sub command to manage application lifecycle configurations
```

### Comparing `awsebcli-3.9.0/ebcli/__init__.py` & `awsebcli-3.9.1/ebcli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
-__version__ = '3.9.0'
+__version__ = '3.9.1'
```

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/colors.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/colors.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/command.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/command.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/docker_client.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/docker_client.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/docopt_command.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/docopt_command.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/errors.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/errors.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/log_printer.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/log_printer.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/main.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/main.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/multiplexer.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/multiplexer.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/utils.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/utils.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/cli/verbose_proxy.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/cli/verbose_proxy.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/config.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/config.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/container.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/container.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/progress_stream.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/progress_stream.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/project.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/project.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/bundled/_compose/service.py` & `awsebcli-3.9.1/ebcli/bundled/_compose/service.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/__init__.py` & `awsebcli-3.9.1/ebcli/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/abstractcontainer.py` & `awsebcli-3.9.1/ebcli/containers/abstractcontainer.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/commands.py` & `awsebcli-3.9.1/ebcli/containers/commands.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/compat.py` & `awsebcli-3.9.1/ebcli/containers/compat.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/compose.py` & `awsebcli-3.9.1/ebcli/containers/compose.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/container_viewmodel.py` & `awsebcli-3.9.1/ebcli/containers/container_viewmodel.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/containerfiles/container_config.json` & `awsebcli-3.9.1/ebcli/containers/containerfiles/container_config.json`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/containerops.py` & `awsebcli-3.9.1/ebcli/containers/containerops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/dockerrun.py` & `awsebcli-3.9.1/ebcli/containers/dockerrun.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/envvarcollector.py` & `awsebcli-3.9.1/ebcli/containers/envvarcollector.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/factory.py` & `awsebcli-3.9.1/ebcli/containers/factory.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/fshandler.py` & `awsebcli-3.9.1/ebcli/containers/fshandler.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/generic_container.py` & `awsebcli-3.9.1/ebcli/containers/generic_container.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/log.py` & `awsebcli-3.9.1/ebcli/containers/log.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/multicontainer.py` & `awsebcli-3.9.1/ebcli/containers/multicontainer.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/pathconfig.py` & `awsebcli-3.9.1/ebcli/containers/pathconfig.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/containers/preconfigured_container.py` & `awsebcli-3.9.1/ebcli/containers/preconfigured_container.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/__init__.py` & `awsebcli-3.9.1/ebcli/core/__init__.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/abort.py` & `awsebcli-3.9.1/ebcli/controllers/abort.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/appversion.py` & `awsebcli-3.9.1/ebcli/controllers/appversion.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/clone.py` & `awsebcli-3.9.1/ebcli/controllers/clone.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/codesource.py` & `awsebcli-3.9.1/ebcli/controllers/codesource.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/config.py` & `awsebcli-3.9.1/ebcli/controllers/config.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/console.py` & `awsebcli-3.9.1/ebcli/controllers/console.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/create.py` & `awsebcli-3.9.1/ebcli/controllers/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,16 @@
             (['--vpc.publicip'], dict(
                 action='store_true', dest='vpc_publicip',
                 help=argparse.SUPPRESS)),
             (['--vpc.securitygroups'], dict(
                 dest='vpc_securitygroups', help=argparse.SUPPRESS)),
             (['--vpc.dbsubnets'], dict(
                 dest='vpc_dbsubnets', help=argparse.SUPPRESS)),
-
+            (['-pr', '--process'], dict(
+                action='store_true', help=flag_text['create.process'])),
         ]
 
     def do_command(self):
         # save command line args
         env_name = self.app.pargs.environment_name
         modules = self.app.pargs.modules
         if modules and len(modules) > 0:
@@ -121,14 +122,15 @@
         tags = self.app.pargs.tags
         envvars = self.app.pargs.envvars
         scale = self.app.pargs.scale
         timeout = self.app.pargs.timeout
         cfg = self.app.pargs.cfg
         elb_type = self.app.pargs.elb_type
         source = self.app.pargs.source
+        process = self.app.pargs.process
         interactive = False if env_name else True
 
         provided_env_name = env_name is not None
 
         if sample and label:
             raise InvalidOptionsError(strings['create.sampleandlabel'])
 
@@ -238,15 +240,15 @@
             scale=scale,
             database=database,
             vpc=vpc,
             elb_type=elb_type)
 
         env_request.option_settings += envvars
 
-        process_app_version = fileoperations.env_yaml_exists()
+        process_app_version = fileoperations.env_yaml_exists() or process
         createops.make_new_env(env_request,
                                branch_default=branch_default,
                                process_app_version=process_app_version,
                                nohang=nohang,
                                interactive=interactive,
                                timeout=timeout,
                                source=source)
```

### Comparing `awsebcli-3.9.0/ebcli/controllers/deploy.py` & `awsebcli-3.9.1/ebcli/controllers/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,28 +40,31 @@
             (['-m', '--message'], dict(help=flag_text['deploy.message'])),
             (['-nh', '--nohang'], dict(
                 action='store_true', help=flag_text['deploy.nohang'])),
             (['--staged'], dict(
                 action='store_true', help=flag_text['deploy.staged'])),
             (['--timeout'], dict(type=int, help=flag_text['general.timeout'])),
             (['--source'], dict(type=utils.check_source, help=flag_text['deploy.source'])),
+            (['-p', '--process'], dict(
+                action='store_true', help=flag_text['deploy.process'])),
             ]
         usage = AbstractBaseController.Meta.usage.replace('{cmd}', label)
 
     def do_command(self):
         self.message = self.app.pargs.message
         self.staged = self.app.pargs.staged
         self.timeout = self.app.pargs.timeout
         self.nohang = self.app.pargs.nohang
         self.modules = self.app.pargs.modules
         self.source = self.app.pargs.source
         self.app_name = self.get_app_name()
         self.env_name = self.app.pargs.environment_name
         self.version = self.app.pargs.version
         self.label = self.app.pargs.label
+        self.process = self.app.pargs.process
         group_name = self.app.pargs.env_group_suffix
 
         if self.modules and len(self.modules) > 0:
             self.multiple_app_deploy()
             return
 
         if self.nohang:
@@ -80,15 +83,15 @@
             raise NoEnvironmentForBranchError()
 
         # ToDo add support for deploying to multiples?
         # for arg in self.app.pargs.environment_name:
         #     # deploy to every environment listed
         #     ## Right now you can only list one
 
-        process_app_versions = fileoperations.env_yaml_exists()
+        process_app_versions = fileoperations.env_yaml_exists() or self.process
 
         deployops.deploy(self.app_name, self.env_name, self.version, self.label,
                          self.message, group_name=group_name, process_app_versions=process_app_versions,
                          staged=self.staged, timeout=self.timeout, source=self.source)
 
     def complete_command(self, commands):
         # TODO: edit this if we ever support multiple env deploys
```

### Comparing `awsebcli-3.9.0/ebcli/controllers/events.py` & `awsebcli-3.9.1/ebcli/controllers/events.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/health.py` & `awsebcli-3.9.1/ebcli/controllers/health.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/initialize.py` & `awsebcli-3.9.1/ebcli/controllers/initialize.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # language governing permissions and limitations under the License.
 
 import sys
 import os.path
 
 from cement.utils.misc import minimal_logger
 
-from ..core import fileoperations, io
-from ..core.abstractcontroller import AbstractBaseController
-from ..lib import utils, elasticbeanstalk, codecommit, aws
-from ..objects.sourcecontrol import SourceControl
-from ..objects import solutionstack, region as regions
-from ..objects.exceptions import NotInitializedError, NoRegionError, \
+from ebcli.core import fileoperations, io
+from ebcli.core.abstractcontroller import AbstractBaseController
+from ebcli.lib import utils, elasticbeanstalk, codecommit, aws
+from ebcli.objects.sourcecontrol import SourceControl
+from ebcli.objects import solutionstack, region as regions
+from ebcli.objects.exceptions import NotInitializedError, NoRegionError, \
     InvalidProfileError, ServiceError, ValidationError, CommandError
-from ..operations import commonops, initializeops, sshops, gitops
-from ..resources.strings import strings, flag_text
+from ebcli.operations import commonops, initializeops, sshops, gitops
+from ebcli.resources.strings import strings, flag_text, prompts
 
 LOG = minimal_logger(__name__)
 
 class InitController(AbstractBaseController):
     class Meta:
         label = 'init'
         description = strings['init.info']
@@ -78,20 +78,20 @@
         else:
             self.region = self.get_region_from_inputs()
         aws.set_region(self.region)
 
         # Warn the customer if they picked a region that CodeCommit is not supported
         codecommit_region_supported = codecommit.region_supported(self.region)
         if self.source is not None and not codecommit_region_supported:
-            io.log_warning("AWS CodeCommit is not supported in this region. Continuing initialization without CodeCommit")
+            io.log_warning(strings['codecommit.badregion'])
 
         self.set_up_credentials()
 
         self.solution = self.get_solution_stack()
-        self.app_name, new_app = self.get_app_name()
+        self.app_name = self.get_app_name()
         if self.noverify:
             fileoperations.write_config_setting('global',
                                                 'no-verify-ssl', True)
 
         if not default_env and not self.interactive:
             # try to get default env from config file if exists
             try:
@@ -101,15 +101,15 @@
         elif self.interactive:
             default_env = None
 
         if self.force_non_interactive:
             default_env = '/ni'
 
         # Create application
-        sstack, key = commonops.create_app(self.app_name, default_env=default_env) if new_app \
+        sstack, key = commonops.create_app(self.app_name, default_env=default_env) if elasticbeanstalk.application_exist(self.app_name) \
             else commonops.pull_down_app_info(self.app_name, default_env=default_env)
 
         if not self.solution:
             self.solution = sstack
 
         platform_set = False
         if not self.solution or \
@@ -124,32 +124,32 @@
             if not platform_set:
                 result = commonops.prompt_for_solution_stack()
                 self.solution = result.version
 
         # Select CodeBuild image if BuildSpec is present do not prompt or show if we are non-interactive
         if fileoperations.build_spec_exists() and not self.force_non_interactive:
             build_spec = fileoperations.get_build_configuration()
-            if build_spec.image is None:
+            if build_spec is not None and build_spec.image is None:
                 LOG.debug("Buildspec file is present but image is does not exist. Attempting to fill best guess.")
                 platform_image = initializeops.get_codebuild_image_from_platform(self.solution)
 
                 # If the return is a dictionary then it must be a single image and we can use that automatically
                 if type(platform_image) is dict:
-                    io.echo("buildspec file is present but no image is specified. Using latest image for selected platform: {0}".format(self.solution))
+                    io.echo('codebuild.latestplatform'.replace('{platform}', self.solution))
                 else:
                     # Otherwise we have an array for images which we must prompt the customer to pick from
-                    io.echo("Could not determine best image for buildspec file please select from list.\n"
-                            "Current chosen platform: {0}".format(self.solution))
+                    io.echo(prompts['codebuild.getplatform'].replace('{platform}', self.solution))
                     selected = utils.prompt_for_index_in_list(map(lambda image: image['description'], platform_image))
                     platform_image = platform_image[selected]
+                    platform_image['name'] = utils.decode_bytes(platform_image['name'])
 
                 # Finally write the CodeBuild image back to the buildspec file
                 fileoperations.write_config_setting(fileoperations.buildspec_config_header,
                                                     'Image',
-                                                    platform_image['name'].encode('ascii', 'ignore'),
+                                                    platform_image['name'],
                                                     file=fileoperations.buildspec_name)
 
         # Setup code commit integration
         # Ensure that git is setup
         source_control = SourceControl.get_source_control()
         try:
             source_control_setup = source_control.is_setup()
@@ -170,43 +170,42 @@
                 or self.source is not None \
                 or default_branch_exists:
             prompt_codecommit = False
 
         # Prompt for interactive CodeCommit
         if prompt_codecommit:
             if not source_control_setup:
-                io.echo("Cannot setup CodeCommit because there is no Source Control setup, continuing with initialization")
+                io.echo(strings['codecommit.nosc'])
             else:
-                io.echo("Note:\n Elastic Beanstalk now supports AWS CodeCommit; a fully-managed source control service."
-                    " To learn more, see Docs: https://aws.amazon.com/codecommit/")
+                io.echo(strings['codecommit.ccwarning'])
                 try:
-                    io.validate_action("Do you wish to continue with CodeCommit? (y/n) (default is n)", "y")
+                    io.validate_action(prompts['codecommit.usecc'], "y")
 
                     # Setup git config settings for code commit credentials
                     source_control.setup_codecommit_cred_config()
 
                     # Get user specified repository
                     if repository is None:
                         repository = get_repository_interactive()
                     else:
                         try:
                             result = codecommit.get_repository(repository)
                             source_control.setup_codecommit_remote_repo(remote_url=result['repositoryMetadata']['cloneUrlHttp'])
                         except ServiceError as ex:
-                            io.log_error("Repository does not exist in CodeCommit.")
+                            io.log_error(strings['codecommit.norepo'])
                             raise ex
 
                     # Get user specified branch
                     if branch is None:
                         branch = get_branch_interactive(repository)
                     else:
                         try:
                             codecommit.get_branch(repository, branch)
                         except ServiceError as ex:
-                            io.log_error("Branch does not exist in CodeCommit.")
+                            io.log_error(strings['codecommit.nobranch'])
                             raise ex
                         source_control.setup_existing_codecommit_branch(branch)
 
                 except ValidationError:
                     LOG.debug("Denied option to use CodeCommit, continuing initialization")
 
         # Initialize the whole setup
@@ -257,15 +256,14 @@
         if not initializeops.credentials_are_valid():
             initializeops.setup_credentials()
         else:
             fileoperations.write_config_setting('global', 'profile',
                                                 profile)
 
     def get_app_name(self):
-        new_app = True
         # Get app name from command line arguments
         app_name = self.app.pargs.application_name
 
         # Get app name from config file, if exists
         if not app_name:
             try:
                 app_name = fileoperations.get_application_name(default=None)
@@ -275,24 +273,24 @@
         if not app_name and self.force_non_interactive:
             # Choose defaults
             app_name = fileoperations.get_current_directory_name()
 
         # Ask for app name
         if not app_name or \
                 (self.interactive and not self.app.pargs.application_name):
-            app_name, new_app = _get_application_name_interactive()
+            app_name = _get_application_name_interactive()
 
         if sys.version_info[0] < 3 and isinstance(app_name, unicode):
             try:
                 app_name.encode('utf8').encode('utf8')
                 app_name = app_name.encode('utf8')
             except UnicodeDecodeError:
                 pass
 
-        return app_name, new_app
+        return app_name
 
     def get_region_from_inputs(self):
         # Get region from command line arguments
         region = self.app.pargs.region
 
         # Get region from config file
         if not region:
@@ -497,15 +495,15 @@
 
     if len(app_list) == 0 or new_app:
         io.echo()
         io.echo('Enter Application Name')
         unique_name = utils.get_unique_name(file_name, app_list)
         app_name = io.prompt_for_unique_name(unique_name, app_list)
 
-    return app_name, new_app
+    return app_name
 
 
 # Code Commit repository setup methods
 def get_repository_interactive():
     source_control = SourceControl.get_source_control()
     # Give list of code commit repositories to use
     new_repo = False
```

### Comparing `awsebcli-3.9.0/ebcli/controllers/lifecycle.py` & `awsebcli-3.9.1/ebcli/controllers/lifecycle.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/list.py` & `awsebcli-3.9.1/ebcli/controllers/list.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/local.py` & `awsebcli-3.9.1/ebcli/controllers/local.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/logs.py` & `awsebcli-3.9.1/ebcli/controllers/logs.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/open.py` & `awsebcli-3.9.1/ebcli/controllers/open.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/platform.py` & `awsebcli-3.9.1/ebcli/controllers/platform.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/printenv.py` & `awsebcli-3.9.1/ebcli/controllers/printenv.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/restore.py` & `awsebcli-3.9.1/ebcli/controllers/restore.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/scale.py` & `awsebcli-3.9.1/ebcli/controllers/scale.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/setenv.py` & `awsebcli-3.9.1/ebcli/controllers/setenv.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/ssh.py` & `awsebcli-3.9.1/ebcli/controllers/ssh.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/status.py` & `awsebcli-3.9.1/ebcli/controllers/status.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/swap.py` & `awsebcli-3.9.1/ebcli/controllers/swap.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/terminate.py` & `awsebcli-3.9.1/ebcli/controllers/terminate.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/upgrade.py` & `awsebcli-3.9.1/ebcli/controllers/upgrade.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/controllers/use.py` & `awsebcli-3.9.1/ebcli/controllers/use.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/core/__init__.py` & `awsebcli-3.9.1/ebcli/labs/__init__.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/core/abstractcontroller.py` & `awsebcli-3.9.1/ebcli/core/abstractcontroller.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/core/arghandler.py` & `awsebcli-3.9.1/ebcli/core/arghandler.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/core/base.py` & `awsebcli-3.9.1/ebcli/core/base.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/core/completer.py` & `awsebcli-3.9.1/ebcli/core/completer.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/core/ebcore.py` & `awsebcli-3.9.1/ebcli/core/ebcore.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,21 +68,23 @@
 from ..resources.strings import strings, flag_text
 from ..labs.controller import LabsController
 from ..controllers.codesource import CodeSourceController
 from ..controllers.restore import RestoreController
 from ..controllers.appversion import AppVersionController
 from ..controllers.lifecycle import LifecycleController
 
+
 class EB(foundation.CementApp):
     class Meta:
         label = 'eb'
         base_controller = base.EbBaseController
         defaults = init_defaults('eb', 'log.logging')
         defaults['log.logging']['level'] = 'WARN'
         config_defaults = defaults
+        exit_on_close = True
 
     def setup(self):
         # Add hooks
         hook.register('post_argument_parsing', hooks.pre_run_hook)
 
         # Add controllers
         controllers = [
```

### Comparing `awsebcli-3.9.0/ebcli/core/ebglobals.py` & `awsebcli-3.9.1/ebcli/core/ebglobals.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/core/ebrun.py` & `awsebcli-3.9.1/ebcli/core/ebrun.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/core/fileoperations.py` & `awsebcli-3.9.1/ebcli/core/fileoperations.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 from yaml.scanner import ScannerError
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 
 from ebcli.core import io
-from ebcli.resources.strings import prompts
+from ebcli.resources.strings import prompts, strings
 from ebcli.objects.exceptions import NotInitializedError, InvalidSyntaxError, \
-    NotFoundError, ValidationError
+    NotFoundError
 
 LOG = minimal_logger(__name__)
 
 
 def get_aws_home():
     sep = os.path.sep
     p = '~' + sep + '.aws' + sep
@@ -247,16 +247,17 @@
     :param location: Full location of either a folder or a location
     """
     os.chmod(location, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)
 
 
 def get_current_directory_name():
     dirname, filename = os.path.split(os.getcwd())
-    if sys.version_info[0] < 3:
-        filename = filename.decode('utf8')
+
+    from ebcli.lib.utils import decode_bytes
+    filename = decode_bytes(filename)
 
     return filename
 
 
 def get_application_name(default=_marker):
     result = get_config_setting('global', 'application_name')
     if result is not None:
@@ -618,14 +619,15 @@
                                  'invalid syntax.')
 
     finally:
         os.chdir(cwd)
 
     return app
 
+
 def write_config_setting(section, key_name, value, dir_path=None, file=local_config_file):
     cwd = os.getcwd()  # save working directory
     if dir_path:
         os.chdir(dir_path)
     try:
         _traverse_to_project_root()
 
@@ -633,14 +635,16 @@
         if not config:
             config = {}
         # Value will be a dict when we are passing in branch config settings
         if type(value) is dict:
             for key in value.keys():
                 config.setdefault(section, {}).setdefault(key_name, {})[key] = value[key]
         else:
+            if config.get(section) is None:
+                config[section] = {}
             config.setdefault(section, {})[key_name] = value
 
         with codecs.open(file, 'w', encoding='utf8') as f:
             f.write(safe_dump(config, default_flow_style=False,
                               line_break=os.linesep))
 
     finally:
@@ -728,15 +732,14 @@
         _traverse_to_project_root()
         return os.path.isfile(buildspec_name)
     finally:
         os.chdir(cwd)
 
 
 def get_build_configuration():
-    # TODO: Verify this is correct.
     # Values expected in the eb config section in BuildSpec
     service_role_key = 'CodeBuildServiceRole'
     image_key = 'Image'
     compute_key = 'ComputeType'
     timeout_key = 'Timeout'
 
     # get setting from global if it exists
@@ -744,20 +747,26 @@
 
     try:
         _traverse_to_project_root()
 
         build_spec = _get_yaml_dict(buildspec_name)
 
         # Assert that special beanstalk section exists
-        if buildspec_config_header not in build_spec.keys():
+        if build_spec is None or buildspec_config_header not in build_spec.keys():
             LOG.debug("Buildspec Keys: {0}".format(build_spec.keys()))
-            raise ValidationError("Beanstalk configuration header '{0}' is missing from Buildspec file".format(buildspec_config_header))
+            io.log_warning(strings['codebuild.noheader'].replace('{header}', buildspec_config_header))
+            return None
 
         build_configuration = BuildConfiguration()
         beanstalk_build_configs = build_spec[buildspec_config_header]
+
+        if beanstalk_build_configs is None:
+            LOG.debug("No values for EB header in buildspec file")
+            return build_configuration
+
         LOG.debug("EB Config Keys: {0}".format(beanstalk_build_configs.keys()))
 
         if service_role_key in beanstalk_build_configs.keys():
             build_configuration.service_role = beanstalk_build_configs[service_role_key]
 
         if image_key in beanstalk_build_configs.keys():
             build_configuration.image = beanstalk_build_configs[image_key]
```

### Comparing `awsebcli-3.9.0/ebcli/core/hooks.py` & `awsebcli-3.9.1/ebcli/core/hooks.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/core/io.py` & `awsebcli-3.9.1/ebcli/core/io.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/__init__.py` & `awsebcli-3.9.1/ebcli/display/__init__.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/appversion.py` & `awsebcli-3.9.1/ebcli/display/appversion.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/data_poller.py` & `awsebcli-3.9.1/ebcli/display/data_poller.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/environments.py` & `awsebcli-3.9.1/ebcli/display/environments.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/help.py` & `awsebcli-3.9.1/ebcli/display/help.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/screen.py` & `awsebcli-3.9.1/ebcli/display/screen.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/specialtables.py` & `awsebcli-3.9.1/ebcli/display/specialtables.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/table.py` & `awsebcli-3.9.1/ebcli/display/table.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/term.py` & `awsebcli-3.9.1/ebcli/display/term.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/display/traditional.py` & `awsebcli-3.9.1/ebcli/display/traditional.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/__init__.py` & `awsebcli-3.9.1/ebcli/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/cleanupversions.py` & `awsebcli-3.9.1/ebcli/labs/cleanupversions.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/cloudwatchfiles/cwl-activity-logs-v1.config` & `awsebcli-3.9.1/ebcli/labs/cloudwatchfiles/cwl-activity-logs-v1.config`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/cloudwatchfiles/cwl-setup-v1.config` & `awsebcli-3.9.1/ebcli/labs/cloudwatchfiles/cwl-setup-v1.config`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/cloudwatchfiles/eb-logs-v1.config` & `awsebcli-3.9.1/ebcli/labs/cloudwatchfiles/eb-logs-v1.config`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/cloudwatchsetup.py` & `awsebcli-3.9.1/ebcli/labs/cloudwatchsetup.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/controller.py` & `awsebcli-3.9.1/ebcli/labs/controller.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/convertdockerrun.py` & `awsebcli-3.9.1/ebcli/labs/convertdockerrun.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/download.py` & `awsebcli-3.9.1/ebcli/labs/download.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/quicklink.py` & `awsebcli-3.9.1/ebcli/labs/quicklink.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/labs/setupssl.py` & `awsebcli-3.9.1/ebcli/labs/setupssl.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/__init__.py` & `awsebcli-3.9.1/ebcli/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/aws.py` & `awsebcli-3.9.1/ebcli/lib/aws.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/botocoredata/codebuild/2016-10-06/service-2.json` & `awsebcli-3.9.1/ebcli/lib/botocoredata/codebuild/2016-10-06/service-2.json`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/botocoredata/elasticbeanstalk/2010-12-01/service-2.json` & `awsebcli-3.9.1/ebcli/lib/botocoredata/elasticbeanstalk/2010-12-01/service-2.json`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/botocoredata/elbv2/2015-12-01/service-2.json` & `awsebcli-3.9.1/ebcli/lib/botocoredata/elbv2/2015-12-01/service-2.json`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/botopatch.py` & `awsebcli-3.9.1/ebcli/lib/botopatch.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/cloudformation.py` & `awsebcli-3.9.1/ebcli/lib/cloudformation.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/cloudwatch.py` & `awsebcli-3.9.1/ebcli/lib/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/codebuild.py` & `awsebcli-3.9.1/ebcli/lib/codebuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,19 @@
     regex_search_version = "AWS ElasticBeanstalk - (.*)v([0-9]+\.[0-9]+\.[0-9]+)"
     result = _make_api_call('list_curated_environment_images')
     beanstalk_images = []
     for platform in result['platforms']:
         for language in platform['languages']:
             languages_by_platform_version = {}
             for image in language['images']:
-                if 'ElasticBeanstalk' in image['description'].encode('ascii','ignore'):
+                if 'ElasticBeanstalk'.encode(errors='ignore') in image['description'].encode(errors='ignore'):
                     matches = re.search(regex_search_version, image['description'])
 
                     # Get the Platform version for the current image
-                    current_version = int(matches.group(2).encode('ascii', 'ignore').replace(".", ""))
+                    current_version = int(matches.group(2).replace(".", ""))
 
                     # Set the description to to something nicer than the full description from CodeBuild
                     image['description'] = matches.group(1)
 
                     # Append the image to the correct array with the Platform version as the key
                     if current_version in languages_by_platform_version.keys():
                         current_value = languages_by_platform_version[current_version]
```

### Comparing `awsebcli-3.9.0/ebcli/lib/codecommit.py` & `awsebcli-3.9.1/ebcli/lib/codecommit.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/ec2.py` & `awsebcli-3.9.1/ebcli/lib/ec2.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/elasticbeanstalk.py` & `awsebcli-3.9.1/ebcli/lib/elasticbeanstalk.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,22 @@
 
 def describe_applications():
     LOG.debug('Inside describe_applications api wrapper')
     result = _make_api_call('describe_applications')
     return result['Applications']
 
 
+def application_exist(app_name):
+    try:
+        describe_application(app_name)
+    except NotFoundError:
+        return False
+    return True
+
+
 def describe_configuration_settings(app_name, env_name):
     LOG.debug('Inside describe_configuration_settings api wrapper')
     result = _make_api_call('describe_configuration_settings',
                             ApplicationName=app_name,
                             EnvironmentName=env_name)
     return result['ConfigurationSettings'][0]
```

### Comparing `awsebcli-3.9.0/ebcli/lib/elb.py` & `awsebcli-3.9.1/ebcli/lib/elb.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/elbv2.py` & `awsebcli-3.9.1/ebcli/lib/elbv2.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/heuristics.py` & `awsebcli-3.9.1/ebcli/lib/heuristics.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/iam.py` & `awsebcli-3.9.1/ebcli/lib/iam.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/s3.py` & `awsebcli-3.9.1/ebcli/lib/s3.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/lib/utils.py` & `awsebcli-3.9.1/ebcli/lib/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 # language governing permissions and limitations under the License.
 import argparse
 import os
 import re
 import pkg_resources
 import sys
 from datetime import datetime
-import warnings
 
 from dateutil import tz
 
 from botocore.compat import six
 from cement.utils.misc import minimal_logger
 from subprocess import Popen, PIPE, STDOUT
 urllib = six.moves.urllib
 
-from ..objects.exceptions import CommandError, InvalidOptionsError
-from ..core import io, fileoperations
+from ebcli.objects.exceptions import CommandError, InvalidOptionsError
+from ebcli.core import io, fileoperations
 
 
 LOG = minimal_logger(__name__)
 
 
 def prompt_for_item_in_list(lst, default=1):
     ind = prompt_for_index_in_list(lst, default)
     return lst[ind]
 
 
 def prompt_for_index_in_list(lst, default=1):
+    lst = list(lst)
     for x in range(0, len(lst)):
         io.echo(str(x + 1) + ')', lst[x])
 
     while True:
         try:
             choice = int(io.prompt('default is ' + str(default),
                                    default=default))
@@ -348,8 +348,15 @@
         raise InvalidOptionsError("Source location '{0}' is not in the list of valid locations: {1}".format(source_location, valid_source_locations))
 
 
 def encode_to_ascii(unicode_value):
     empty_string = ""
     if unicode_value is None:
         return empty_string
-    return unicode_value.encode('ascii', 'ignore')
+    return unicode_value.encode('ascii', 'ignore')
+
+
+def decode_bytes(value):
+    if sys.version_info[0] >= 3:
+        if isinstance(value, bytes):
+            value = value.decode('utf8')
+    return value
```

### Comparing `awsebcli-3.9.0/ebcli/objects/__init__.py` & `awsebcli-3.9.1/ebcli/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/application.py` & `awsebcli-3.9.1/ebcli/objects/application.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/buildconfiguration.py` & `awsebcli-3.9.1/ebcli/objects/buildconfiguration.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/conversionconfiguration.py` & `awsebcli-3.9.1/ebcli/objects/conversionconfiguration.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/environment.py` & `awsebcli-3.9.1/ebcli/objects/environment.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/environmentsettings.py` & `awsebcli-3.9.1/ebcli/objects/environmentsettings.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/event.py` & `awsebcli-3.9.1/ebcli/objects/event.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/exceptions.py` & `awsebcli-3.9.1/ebcli/objects/exceptions.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/lifecycleconfiguration.py` & `awsebcli-3.9.1/ebcli/objects/lifecycleconfiguration.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/region.py` & `awsebcli-3.9.1/ebcli/objects/region.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/requests.py` & `awsebcli-3.9.1/ebcli/objects/requests.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/solutionstack.py` & `awsebcli-3.9.1/ebcli/objects/solutionstack.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/objects/sourcecontrol.py` & `awsebcli-3.9.1/ebcli/objects/sourcecontrol.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 import fileinput
 import os
 import sys
 
 from cement.utils.misc import minimal_logger
 from cement.utils.shell import exec_cmd
 
-from ..lib import codecommit, aws
-from ..core import fileoperations, io
-from ..objects.exceptions import NoSourceControlError, CommandError, \
+from ebcli.lib import codecommit, utils
+from ebcli.core import fileoperations, io
+from ebcli.objects.exceptions import NoSourceControlError, CommandError, \
     NotInitializedError
-from ..resources.strings import git_ignore, strings
+from ebcli.resources.strings import git_ignore, strings
 
 LOG = minimal_logger(__name__)
 
 
 class SourceControl():
     name = 'base'
 
@@ -414,19 +414,18 @@
         self._run_cmd(
             ['git', 'config', '--local', '--replace-all', 'credential.UseHttpPath', 'true'])
         self._run_cmd(
             ['git', 'config', '--local', '--replace-all', 'credential.helper', '!aws codecommit credential-helper $@'])
 
     def _run_cmd(self, cmd, handle_exitcode=True):
         stdout, stderr, exitcode = exec_cmd(cmd)
-        if sys.version_info[0] >= 3:
-            stdout = stdout.decode('utf8')
-            stderr = stderr.decode('utf8')
-        stdout = stdout.strip()
-        stderr = stderr.strip()
+
+        stdout = utils.decode_bytes(stdout).strip()
+        stderr = utils.decode_bytes(stderr).strip()
+
         if handle_exitcode:
             self._handle_exitcode(exitcode, stderr)
         return stdout, stderr, exitcode
 
     def get_url_from_remote_repo(self, remote):
         stdout, stderr, exitcode = self._run_cmd(['git', 'config', '--get', "remote.{0}.url".format(remote)], handle_exitcode=False)
         if exitcode != 0:
```

### Comparing `awsebcli-3.9.0/ebcli/objects/tier.py` & `awsebcli-3.9.1/ebcli/objects/tier.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/__init__.py` & `awsebcli-3.9.1/ebcli/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/abortops.py` & `awsebcli-3.9.1/ebcli/operations/abortops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/appversionops.py` & `awsebcli-3.9.1/ebcli/operations/appversionops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/buildspecops.py` & `awsebcli-3.9.1/ebcli/operations/buildspecops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/cloneops.py` & `awsebcli-3.9.1/ebcli/operations/cloneops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/commonops.py` & `awsebcli-3.9.1/ebcli/operations/commonops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/composeops.py` & `awsebcli-3.9.1/ebcli/operations/composeops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/configops.py` & `awsebcli-3.9.1/ebcli/operations/configops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/consoleops.py` & `awsebcli-3.9.1/ebcli/operations/consoleops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/createops.py` & `awsebcli-3.9.1/ebcli/operations/createops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/deployops.py` & `awsebcli-3.9.1/ebcli/operations/deployops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/envvarops.py` & `awsebcli-3.9.1/ebcli/operations/envvarops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/eventsops.py` & `awsebcli-3.9.1/ebcli/operations/eventsops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/gitops.py` & `awsebcli-3.9.1/ebcli/operations/gitops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/healthops.py` & `awsebcli-3.9.1/ebcli/operations/healthops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/initializeops.py` & `awsebcli-3.9.1/ebcli/operations/initializeops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/lifecycleops.py` & `awsebcli-3.9.1/ebcli/operations/lifecycleops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/listops.py` & `awsebcli-3.9.1/ebcli/operations/listops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/localops.py` & `awsebcli-3.9.1/ebcli/operations/localops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/logsops.py` & `awsebcli-3.9.1/ebcli/operations/logsops.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,17 +108,15 @@
 
     else:
         # print logs
         data = []
         for i_id, url in iteritems(log_list):
             data.append('============= ' + str(i_id) + ' ==============')
             log_result = utils.get_data_from_url(url)
-            if sys.version_info[0] >= 3:
-                log_result = log_result.decode()
-            data.append(log_result)
+            data.append(utils.decode_bytes(log_result))
         io.echo_with_pager(os.linesep.join(data))
 
 
 def stream_cloudwatch_logs(env_name, sleep_time=2, log_group=None, instance_id=None):
     """
         This function will stream logs to the terminal for the log group given, if multiple streams are found we will
         spawn multiple threads with each stream switch between them to stream all streams at the same time.
```

### Comparing `awsebcli-3.9.0/ebcli/operations/openops.py` & `awsebcli-3.9.1/ebcli/operations/openops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/platformops.py` & `awsebcli-3.9.1/ebcli/operations/platformops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/restoreops.py` & `awsebcli-3.9.1/ebcli/operations/restoreops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/saved_configs.py` & `awsebcli-3.9.1/ebcli/operations/saved_configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 import os
+import time
 
-from ..lib import elasticbeanstalk, s3, utils
-from ..resources.strings import strings, responses
-from ..core import io, fileoperations
-from ..objects.exceptions import NotFoundError
-from ..lib.aws import InvalidParameterValueError
-from . import commonops
+from ebcli.lib import elasticbeanstalk, s3
+from ebcli.resources.strings import strings, responses
+from ebcli.core import io, fileoperations
+from ebcli.objects.exceptions import NotFoundError
+from ebcli.lib.aws import InvalidParameterValueError
+from ebcli.operations import commonops
 
 SAVED_CONFIG_FOLDER_NAME = 'saved_configs' + os.path.sep
 
 
 def _get_s3_keyname_for_template(app_name, cfg_name):
     return 'resources/templates/' + app_name + '/' + cfg_name
 
@@ -73,14 +74,20 @@
 
 
 def update_config(app_name, cfg_name):
     config_location = resolve_config_location(cfg_name)
     if config_location is None:
         raise NotFoundError('No local version of ' + cfg_name + ' found.')
 
+    # Update modified date
+    fileoperations.write_config_setting('EnvironmentConfigurationMetadata',
+                                        'DateModified',
+                                        (('%f' % (time.time() * 1000)).split('.')[0]),
+                                        file=config_location)
+
     # Get just the name of the file
     filename = fileoperations.get_filename_without_extension(config_location)
 
     upload_config_file(app_name, filename, config_location)
 
 
 def upload_config_file(app_name, cfg_name, file_location):
@@ -163,16 +170,18 @@
 
 def get_configurations(app_name):
     app = elasticbeanstalk.describe_application(app_name)
     return app['ConfigurationTemplates']
 
 
 def validate_config_file(app_name, cfg_name, platform):
+    # Get just the name of the file
+    filename = fileoperations.get_filename_without_extension(cfg_name)
     try:
-        result = elasticbeanstalk.validate_template(app_name, cfg_name)
+        result = elasticbeanstalk.validate_template(app_name, filename)
     except InvalidParameterValueError as e:
         # Platform not in Saved config. Try again with default platform
         if e.message == responses['create.noplatform']:
            result = elasticbeanstalk.validate_template(app_name, cfg_name,
                                                        platform=platform)
         else:
             raise
```

### Comparing `awsebcli-3.9.0/ebcli/operations/scaleops.py` & `awsebcli-3.9.1/ebcli/operations/scaleops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/sshops.py` & `awsebcli-3.9.1/ebcli/operations/sshops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/statusops.py` & `awsebcli-3.9.1/ebcli/operations/statusops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/swapops.py` & `awsebcli-3.9.1/ebcli/operations/swapops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/terminateops.py` & `awsebcli-3.9.1/ebcli/operations/terminateops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/upgradeops.py` & `awsebcli-3.9.1/ebcli/operations/upgradeops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/operations/useops.py` & `awsebcli-3.9.1/ebcli/operations/useops.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/resources/__init__.py` & `awsebcli-3.9.1/bin/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+# Copyright 2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"). You
 # may not use this file except in compliance with the License. A copy of
 # the License is located at
 #
 # http://aws.amazon.com/apache2.0/
 #
```

### Comparing `awsebcli-3.9.0/ebcli/resources/statics.py` & `awsebcli-3.9.1/ebcli/resources/statics.py`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/ebcli/resources/strings.py` & `awsebcli-3.9.1/ebcli/resources/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,26 @@
                                ' The lifecycle configuration will not be updated',
 
     # appversion
     'appversion.info': 'Listing and managing application versions',
     'appversion.delete.notfound': 'Application {} does not have Application Version {}.',
     'appversion.delete.deployed': 'Cannot delete Application version {} as it is deployed to Environments: {}',
     'appversion.delete.none': 'You must specify an Application version label to delete an Application version',
+
+    # CodeCommit
+    'codecommit.nosc': 'Cannot setup CodeCommit because there is no Source Control setup, continuing with initialization',
+    'codecommit.ccwarning': 'Note: Elastic Beanstalk now supports AWS CodeCommit; a fully-managed source control service.'
+                    ' To learn more, see Docs: https://aws.amazon.com/codecommit/',
+    'codecommit.norepo': 'Repository does not exist in CodeCommit',
+    'codecommit.nobranch': 'Branch does not exist in CodeCommit',
+    'codecommit.badregion': 'AWS CodeCommit is not supported in this region; continuing initialization without CodeCommit',
+
+    # CodeBuild
+    'codebuild.noheader': 'Beanstalk configuration header \'{header}\' is missing from Buildspec file; will not use Beanstalk Code Build integration',
+    'codebuild.latestplatform': 'Buildspec file is present but no image is specified; using latest image for selected platform: {platform}',
 }
 
 prompts = {
     'events.hanging': 'Streaming new events. Use CTRL+C to exit.',
     'platform.validate': 'It appears you are using {platform}. Is this correct?',
     'platform.prompt': 'Select a platform.',
     'platform.prompt.withmodule': 'Select a platform for module: {module_name}.',
@@ -335,14 +347,20 @@
     # appversion
     'appversion.redeploy.validate': 'Do you want to deploy a previous or different version? (y/n)',
     'appversion.redeploy.prompt': 'Select a version # to deploy (1 to {}).',
     'appversion.redeploy.inprogress': 'Deploying version {}.',
 
     'appversion.delete.validate': 'Do you want to delete the application version with label: {}? (y/n)',
     'appversion.delete.prompt': 'Select a version # to delete (1 to {}).',
+
+    # CodeCommit
+    'codecommit.usecc': 'Do you wish to continue with CodeCommit? (y/N) (default is n)',
+
+    # CodeBuild
+    'codebuild.getplatform': 'Could not determine best image for buildspec file please select from list.\n Current chosen platform: {platform}',
 }
 
 alerts = {
     'platform.old': 'There is a newer version of the platform used by your environment. You can upgrade your environment to the most recent platform version by typing "eb upgrade".'
 }
 
 flag_text = {
@@ -389,25 +407,27 @@
     'create.database': 'create a database',
     'create.vpc': 'create environment inside a VPC',
     'create.config': 'saved configuration name',
     'create.group': 'group suffix',
     'create.modules': 'a list of modules',
     'create.elb_type': 'load balancer type',
     'create.source': 'source of code to create from directly; example source_location/repo/branch',
+    'create.process': 'enable preprocessing of the application version',
 
     # Deploy
     'deploy.env': 'environment name',
     'deploy.modules': 'modules to deploy',
     'deploy.version': 'existing version label to deploy',
     'deploy.label': 'label name which version will be given',
     'deploy.message': 'description for version',
     'deploy.nohang': 'return immediately, do not wait for deploy to be completed',
     'deploy.staged': 'deploy files staged in git rather than the HEAD commit',
     'deploy.group_suffix': 'group suffix',
     'deploy.source': 'source of code to deploy directly; example source_location/repo/branch',
+    'deploy.process': 'enable preprocessing of the application version',
 
     # Events
     'events.follow': 'wait and continue to print events as they come',
 
     # Init
     'init.name': 'application name',
     'init.platform': 'default Platform',
```

### Comparing `awsebcli-3.9.0/LICENSE.txt` & `awsebcli-3.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/PKG-INFO` & `awsebcli-3.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: awsebcli
-Version: 3.9.0
+Version: 3.9.1
 Summary: Command Line Interface for AWS EB.
 Home-page: http://aws.amazon.com/elasticbeanstalk/
 Author: AWS Elastic Beanstalk
 Author-email: aws-eb-cli@amazon.com
 License: Apache License 2.0
 Description: ======
         EB-CLI
@@ -243,14 +243,24 @@
         Now whenever you switch to a new branch, your default environment will also switch.
         
         
         =========
         Changelog
         =========
         ------------------
+        3.9.1 (2017-02-08)
+        ------------------
+        - Changed Beanstalk CodeBuild integration to be optional by not specifying the header in buildspec
+        - Fixed 'eb config put' to update DateModified field
+        - Fixed 'eb config put' full path failure
+        - Fixed exit codes to return correctly
+        - Removed CodeCommit failed prompt in eb init to avoid confusion
+        - Added 'process' flag for eb create/deploy for preprocessing application versions
+        
+        ------------------
         3.9.0 (2016-12-22)
         ------------------
         - Added native support in 'eb logs' for log streaming.
         - Added '--log-group' and '--cloudwatch-logs' flags in 'eb logs'
         - Added 'appversion' command to managed application versions
         - Added 'appversion lifecycle' sub command to manage application lifecycle configurations
         
@@ -585,7 +595,8 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
```

### Comparing `awsebcli-3.9.0/README.rst` & `awsebcli-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `awsebcli-3.9.0/setup.py` & `awsebcli-3.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
            ]
 
 testing_requires = ['pytest>=3.03',
                     'mock>=2.0.0',
                     'nose>=1.3.7']
 
 if not sys.platform.startswith('win'):
-    requires.append('blessed==1.9.5')
+    requires.append('blessed>=1.9.5')
 
 try:
     with open('/etc/bash_completion.d/eb_completion.extra', 'w') as eo:
         eo.write('')
         data_files = [
             ('/etc/bash_completion.d/', ['bin/eb_completion.bash'])
         ]
@@ -44,15 +44,15 @@
     description='Command Line Interface for AWS EB.',
     long_description=open('README.rst').read() + open('CHANGES.rst').read(),
     scripts=['bin/eb', 'bin/eb_completion.bash'],
     data_files=data_files,
     author='AWS Elastic Beanstalk',
     author_email='aws-eb-cli@amazon.com',
     url='http://aws.amazon.com/elasticbeanstalk/',
-    packages=find_packages('.', exclude=['tests*', 'docs*', 'sampleApps*']),
+    packages=find_packages('.', exclude=['tests*', 'docs*', 'sampleApps*', 'scripts*']),
     package_dir={'ebcli': 'ebcli'},
     package_data={
         'ebcli.lib': ['botocoredata/*/*/*.json'],
         'ebcli.containers': ['containerfiles/*'],
         'ebcli.labs': ['cloudwatchfiles/*.config']},
     install_requires=requires,
     license="Apache License 2.0",
@@ -62,14 +62,15 @@
         'Intended Audience :: System Administrators',
         'Natural Language :: English',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
     ),
     entry_points={
         'console_scripts': [
             'eb=ebcli.core.ebcore:main'
         ]
     },
 )
```

