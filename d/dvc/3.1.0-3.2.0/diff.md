# Comparing `tmp/dvc-3.1.0.tar.gz` & `tmp/dvc-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-3.1.0.tar", last modified: Sun Jun 18 22:22:43 2023, max compression
+gzip compressed data, was "dvc-3.2.0.tar", last modified: Thu Jun 22 15:40:16 2023, max compression
```

## Comparing `dvc-3.1.0.tar` & `dvc-3.2.0.tar`

### file list

```diff
@@ -1,688 +1,665 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.142194 dvc-3.1.0/.dvc/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-18 22:22:24.000000 dvc-3.1.0/.dvc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-06-18 22:22:24.000000 dvc-3.1.0/.dvc/config
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-18 22:22:24.000000 dvc-3.1.0/.dvcignore
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-18 22:22:24.000000 dvc-3.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-18 22:22:24.000000 dvc-3.1.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-18 22:22:24.000000 dvc-3.1.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-18 22:22:24.000000 dvc-3.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.142194 dvc-3.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.142194 dvc-3.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/ISSUE_TEMPLATE/epic_story.md
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.142194 dvc-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/packages.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/plugin_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-18 22:22:24.000000 dvc-3.1.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-18 22:22:24.000000 dvc-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-06-18 22:22:24.000000 dvc-3.1.0/.mailmap
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-18 22:22:24.000000 dvc-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-18 22:22:24.000000 dvc-3.1.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-18 22:22:24.000000 dvc-3.1.0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-18 22:22:24.000000 dvc-3.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-18 22:22:24.000000 dvc-3.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-18 22:22:24.000000 dvc-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-18 22:22:43.214195 dvc-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-06-18 22:22:24.000000 dvc-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.146194 dvc-3.1.0/dvc/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-18 22:22:29.000000 dvc-3.1.0/dvc/_build.py
--rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-18 22:22:42.000000 dvc-3.1.0/dvc/_dvc_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.150194 dvc-3.1.0/dvc/api/
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9904 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    11924 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/api/show.py
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cachemgr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.150194 dvc-3.1.0/dvc/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     7614 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.154194 dvc-3.1.0/dvc/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.154194 dvc-3.1.0/dvc/commands/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/exec_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3481 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3672 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/install.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/ls/ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/params.py
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/commands/queue/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/kill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/start.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/queue/stop.py
--rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/repro.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/compare.py
--rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    11039 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dagascii.py
--rw-r--r--   0 runner    (1001) docker     (122)    11333 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/data_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5148 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dependency/param.py
--rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dependency/repo.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/env.py
--rw-r--r--   0 runner    (1001) docker     (122)     9622 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/fs/
--rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    13922 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/fs/git.py
--rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     4981 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/machine/
--rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/machine/backend/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/machine/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/machine/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/machine/backend/terraform.py
--rw-r--r--   0 runner    (1001) docker     (122)    45816 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)    13884 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/parsing/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/parsing/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/render/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.158194 dvc-3.1.0/dvc/render/converter/
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/converter/image.py
--rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/converter/vega.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/render/match.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.166194 dvc-3.1.0/dvc/repo/
--rw-r--r--   0 runner    (1001) docker     (122)    18691 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7017 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/brancher.py
--rw-r--r--   0 runner    (1001) docker     (122)     4248 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1934 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.166194 dvc-3.1.0/dvc/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/brancher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.166194 dvc-3.1.0/dvc/repo/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25373 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/executor/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7929 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/executor/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/executor/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/push.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24548 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    23073 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6834 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8879 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/queue/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/refs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     6759 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/stash.py
--rw-r--r--   0 runner    (1001) docker     (122)    24913 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/fetch.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/get.py
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)    23105 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/index.py
--rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/ls_url.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/repo/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/metrics/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/metrics/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     8230 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/open_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/repo/params/
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/params/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/params/show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)    17028 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/plots/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     7559 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/trie.py
--rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    13769 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/repo/worktree.py
--rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.170194 dvc-3.1.0/dvc/stage/
--rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9221 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     7462 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/params.py
--rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     7116 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/stage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4128 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/api_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_exp_show.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_help.py
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_push.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.174194 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/use_cases/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/benchmarks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/path_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/remote_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/tmp_dir.py
--rw-r--r--   0 runner    (1001) docker     (122)    12070 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/testing/workspace_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/dvc/ui/
--rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ui/_rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ui/pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/ui/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/dvc/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/dvc/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_py.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/serialize/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/utils/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-18 22:22:24.000000 dvc-3.1.0/dvc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.150194 dvc-3.1.0/dvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17145 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-18 22:22:43.000000 dvc-3.1.0/dvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8683 2023-06-18 22:22:24.000000 dvc-3.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/build-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/build.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      226 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/build_package.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.178194 dvc-3.1.0/scripts/fpm/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/after-install.sh
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/after-remove.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/notarize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/fpm/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.182194 dvc-3.1.0/scripts/innosetup/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/addSymLinkPermissions.ps1
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/addsymlink.iss
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/build.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/dvc.ico.dvc
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/dvc_left.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/dvc_up.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/modpath.iss
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/innosetup/setup.iss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.182194 dvc-3.1.0/scripts/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/build.py
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.182194 dvc-3.1.0/scripts/pyinstaller/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-asyncssh.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.system.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc_task.py
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-fsspec.py
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/hooks/hook-pydrive2.py
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-06-18 22:22:24.000000 dvc-3.1.0/scripts/pyinstaller/sign.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-18 22:22:43.214195 dvc-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.186195 dvc-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/dir_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8061 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/api/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/artifacts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/artifacts/test_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.190194 dvc-3.1.0/tests/func/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3425 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/data/db/test_index.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/executor/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    26286 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)    13387 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4928 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_save.py
--rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_set_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_stash_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/machine/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/machine/test_machine_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/machine/test_machine_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7730 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/metrics/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     9854 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/metrics/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/params/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8161 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/params/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/params/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7479 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    11227 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/test_foreach.py
--rw-r--r--   0 runner    (1001) docker     (122)     5484 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/test_interpolated_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/parsing/test_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.194195 dvc-3.1.0/tests/func/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/plots/test_modify.py
--rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/plots/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/func/repro/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/repro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    33140 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/repro/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/repro/test_repro_allow_missing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/repro/test_repro_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)    30138 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    23047 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     9505 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    16589 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_data_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    19044 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    12234 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     7976 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_external_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)    14156 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)    10535 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    21031 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     5090 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    17911 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_merge_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_move.py
--rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_odb.py
--rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     9915 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_root.py
--rw-r--r--   0 runner    (1001) docker     (122)    20611 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_run_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)    14963 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_stage_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      860 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)    14871 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_used_objs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/test_virtual_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/func/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/utils/test_hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/func/utils/test_strict_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/integration/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/plots/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    13823 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/plots/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/plots/test_repo_plots_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/integration/test_studio_live_experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/remotes/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.198195 dvc-3.1.0/tests/remotes/git-init/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/git_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/user.key
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes/user.key.pub
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/remotes_env.sample
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.202195 dvc-3.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.202195 dvc-3.1.0/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/cli/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/command/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/command/ls/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/ls/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/ls/test_ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2478 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_compat_flag.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)    11210 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    11627 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3862 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/command/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/data/db/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/dependency/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/dependency/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/fs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7345 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    19226 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_dvc_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/fs/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.206195 dvc-3.1.0/tests/unit/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/output/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/test_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/test_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/output/test_output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/remote/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/test_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/test_webdav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/remote/test_webhdfs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/render/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/test_image_converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/test_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/render/test_vega_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/queue/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/queue/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/test_executor_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/test_open_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/test_reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/repo/test_scm_context.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.210195 dvc-3.1.0/tests/unit/scm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/scm/test_scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/unit/stage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6074 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     9286 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_loader_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_serialize_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_serialize_pipeline_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/stage/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_hashinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     8740 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     4168 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_tabular_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/unit/ui/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/ui/test_console.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/ui/test_pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/ui/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/unit/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/serialize/test_python.py
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/serialize/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/serialize/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 22:22:43.214195 dvc-3.1.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-18 22:22:24.000000 dvc-3.1.0/tests/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.787374 dvc-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-22 15:39:57.000000 dvc-3.2.0/.dvcignore
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-22 15:39:57.000000 dvc-3.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-22 15:39:57.000000 dvc-3.2.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-22 15:39:57.000000 dvc-3.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-22 15:39:57.000000 dvc-3.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.719373 dvc-3.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.719373 dvc-3.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/ISSUE_TEMPLATE/epic_story.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.719373 dvc-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/workflows/packages.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/workflows/plugin_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-22 15:39:57.000000 dvc-3.2.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-22 15:39:57.000000 dvc-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-06-22 15:39:57.000000 dvc-3.2.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-22 15:39:57.000000 dvc-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-22 15:39:57.000000 dvc-3.2.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-22 15:39:57.000000 dvc-3.2.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-22 15:39:57.000000 dvc-3.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-22 15:39:57.000000 dvc-3.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-22 15:39:57.000000 dvc-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-22 15:40:16.787374 dvc-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-06-22 15:39:57.000000 dvc-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.723373 dvc-3.2.0/dvc/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-22 15:40:02.000000 dvc-3.2.0/dvc/_build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-22 15:40:16.000000 dvc-3.2.0/dvc/_dvc_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.723373 dvc-3.2.0/dvc/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9904 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/api/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/api/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/api/scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11924 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/api/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/cachemgr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.723373 dvc-3.2.0/dvc/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     7614 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.731373 dvc-3.2.0/dvc/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.731373 dvc-3.2.0/dvc/commands/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/exec_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3672 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/install.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.731373 dvc-3.2.0/dvc/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/ls/ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.731373 dvc-3.2.0/dvc/commands/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/queue/kill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/queue/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/queue/start.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/queue/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/queue/stop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11039 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/dagascii.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11333 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/data_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.731373 dvc-3.2.0/dvc/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)     2997 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5148 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/dependency/param.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/dependency/repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9622 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.731373 dvc-3.2.0/dvc/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/fs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/fs/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13922 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/fs/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/fs/git.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4981 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.735373 dvc-3.2.0/dvc/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.735373 dvc-3.2.0/dvc/machine/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/machine/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/machine/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/machine/backend/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46033 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.735373 dvc-3.2.0/dvc/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)    15488 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/parsing/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/parsing/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.735373 dvc-3.2.0/dvc/render/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/render/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.735373 dvc-3.2.0/dvc/render/converter/
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/render/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/render/converter/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/render/converter/vega.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/render/match.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.743373 dvc-3.2.0/dvc/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)    18691 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7017 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1934 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.743373 dvc-3.2.0/dvc/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.743373 dvc-3.2.0/dvc/repo/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25373 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/executor/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7929 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/executor/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/executor/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3541 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/push.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.747373 dvc-3.2.0/dvc/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24548 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/queue/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23073 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/queue/celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/queue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/queue/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6834 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/queue/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/queue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8879 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/queue/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/refs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6759 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/stash.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24913 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23105 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/ls_url.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.747373 dvc-3.2.0/dvc/repo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/metrics/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/metrics/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8230 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/open_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.747373 dvc-3.2.0/dvc/repo/params/
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/params/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/params/show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.747373 dvc-3.2.0/dvc/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)    17028 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/plots/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7559 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/trie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13768 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/repo/worktree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4310 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.747373 dvc-3.2.0/dvc/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9221 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7462 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7116 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/stage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.751373 dvc-3.2.0/dvc/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4128 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/api_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.751373 dvc-3.2.0/dvc/testing/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.751373 dvc-3.2.0/dvc/testing/benchmarks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.751373 dvc-3.2.0/dvc/testing/benchmarks/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.751373 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_exp_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.751373 dvc-3.2.0/dvc/testing/benchmarks/cli/stories/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.751373 dvc-3.2.0/dvc/testing/benchmarks/cli/stories/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/benchmarks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/path_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/remote_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/tmp_dir.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12070 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/testing/workspace_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.755373 dvc-3.2.0/dvc/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/ui/_rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/ui/pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/ui/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.755373 dvc-3.2.0/dvc/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.755373 dvc-3.2.0/dvc/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/serialize/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/serialize/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/serialize/_py.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/serialize/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/serialize/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/utils/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-22 15:39:57.000000 dvc-3.2.0/dvc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.723373 dvc-3.2.0/dvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-06-22 15:40:16.000000 dvc-3.2.0/dvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16599 2023-06-22 15:40:16.000000 dvc-3.2.0/dvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 15:40:16.000000 dvc-3.2.0/dvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-22 15:40:16.000000 dvc-3.2.0/dvc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-06-22 15:40:16.000000 dvc-3.2.0/dvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-22 15:40:16.000000 dvc-3.2.0/dvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8683 2023-06-22 15:39:57.000000 dvc-3.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.755373 dvc-3.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/build-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      226 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/build_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.755373 dvc-3.2.0/scripts/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/build.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.759374 dvc-3.2.0/scripts/pyinstaller/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-asyncssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-dvc.system.py
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-dvc_task.py
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-22 15:39:57.000000 dvc-3.2.0/scripts/pyinstaller/hooks/hook-pydrive2.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 15:40:16.787374 dvc-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.759374 dvc-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/dir_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.763373 dvc-3.2.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.767374 dvc-3.2.0/tests/func/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8061 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/api/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/api/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/api/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.767374 dvc-3.2.0/tests/func/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/artifacts/test_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.767374 dvc-3.2.0/tests/func/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.767374 dvc-3.2.0/tests/func/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3425 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/data/db/test_index.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.767374 dvc-3.2.0/tests/func/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.767374 dvc-3.2.0/tests/func/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/executor/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26341 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13854 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_set_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_stash_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.767374 dvc-3.2.0/tests/func/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/machine/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/machine/test_machine_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/machine/test_machine_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.767374 dvc-3.2.0/tests/func/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7730 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/metrics/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9854 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/metrics/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.767374 dvc-3.2.0/tests/func/params/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8161 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/params/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/params/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.771374 dvc-3.2.0/tests/func/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10114 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/parsing/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15835 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/parsing/test_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9670 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/parsing/test_interpolated_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/parsing/test_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.771374 dvc-3.2.0/tests/func/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/plots/test_modify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12989 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/plots/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.771374 dvc-3.2.0/tests/func/repro/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/repro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33460 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/repro/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/repro/test_repro_allow_missing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/repro/test_repro_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30224 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22833 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9598 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16589 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_data_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19044 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12234 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7976 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_external_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14156 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10535 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21031 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5648 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5090 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17911 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_merge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_odb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3470 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9915 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20611 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_run_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14963 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_stage_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14871 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_used_objs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/test_virtual_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.771374 dvc-3.2.0/tests/func/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/utils/test_hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/func/utils/test_strict_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.771374 dvc-3.2.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.771374 dvc-3.2.0/tests/integration/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/integration/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/integration/plots/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13823 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/integration/plots/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/integration/plots/test_repo_plots_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/integration/test_studio_live_experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.771374 dvc-3.2.0/tests/remotes/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/remotes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.771374 dvc-3.2.0/tests/remotes/git-init/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/remotes/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/remotes/git_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/remotes/user.key
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/remotes/user.key.pub
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/remotes_env.sample
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.775374 dvc-3.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.775374 dvc-3.2.0/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/cli/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.779374 dvc-3.2.0/tests/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.779374 dvc-3.2.0/tests/unit/command/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/ls/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/ls/test_ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_compat_flag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11250 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11272 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3882 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4841 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/command/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.779374 dvc-3.2.0/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.779374 dvc-3.2.0/tests/unit/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/data/db/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.779374 dvc-3.2.0/tests/unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/dependency/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/dependency/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.783374 dvc-3.2.0/tests/unit/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7345 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19226 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/test_dvc_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/fs/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.783374 dvc-3.2.0/tests/unit/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.783374 dvc-3.2.0/tests/unit/output/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/output/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/output/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/output/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/output/test_output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.783374 dvc-3.2.0/tests/unit/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/remote/test_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/remote/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/remote/test_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/remote/test_webhdfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.783374 dvc-3.2.0/tests/unit/render/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/render/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/render/test_image_converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/render/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/render/test_vega_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.783374 dvc-3.2.0/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.783374 dvc-3.2.0/tests/unit/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.783374 dvc-3.2.0/tests/unit/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/experiments/queue/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/experiments/queue/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/experiments/test_executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.783374 dvc-3.2.0/tests/unit/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/test_open_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1724 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/test_reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/repo/test_scm_context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.787374 dvc-3.2.0/tests/unit/scm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/scm/test_scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.787374 dvc-3.2.0/tests/unit/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6074 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/stage/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9286 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/stage/test_loader_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/stage/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/stage/test_serialize_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/stage/test_serialize_pipeline_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/stage/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/stage/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_hashinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8740 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4168 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_tabular_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.787374 dvc-3.2.0/tests/unit/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/ui/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/ui/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/ui/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.787374 dvc-3.2.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.787374 dvc-3.2.0/tests/unit/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/serialize/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/serialize/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/serialize/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/test_cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3522 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 15:40:16.787374 dvc-3.2.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-22 15:39:57.000000 dvc-3.2.0/tests/utils/plots.py
```

### Comparing `dvc-3.1.0/.git-blame-ignore-revs` & `dvc-3.2.0/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvc-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/.github/ISSUE_TEMPLATE/epic_story.md` & `dvc-3.2.0/.github/ISSUE_TEMPLATE/epic_story.md`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/.github/workflows/codeql.yml` & `dvc-3.2.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/.github/workflows/packages.yaml` & `dvc-3.2.0/.github/workflows/packages.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -7,74 +7,14 @@
     types: [released, prereleased]
   workflow_dispatch:
 
 permissions:  # added using https://github.com/step-security/secure-workflows
   contents: read
 
 jobs:
-  binary:
-    permissions:
-      contents: write  # for actions/upload-release-asset to upload release asset
-    strategy:
-      matrix:
-        include:
-         - {pkg: "deb",  os: "ubuntu-20.04", asset: "dvc_${{ github.event.release.tag_name }}_amd64.deb"}
-         - {pkg: "rpm", os: "ubuntu-20.04", asset: "dvc-${{ github.event.release.tag_name }}-1.x86_64.rpm"}
-         - {pkg: "osxpkg", os: "macos-11", asset: "dvc-${{ github.event.release.tag_name }}.pkg"}
-         - {pkg: "exe",  os: "windows-2019", asset: "dvc-${{ github.event.release.tag_name }}.exe"}
-
-    name: ${{ matrix.pkg }}
-    runs-on: ${{ matrix.os }}
-    steps:
-    - uses: actions/checkout@v3
-      with:
-          fetch-depth: 0
-
-    - name: Set up Python 3.10
-      uses: actions/setup-python@v4
-      with:
-        python-version: "3.10"
-        cache: pip
-        cache-dependency-path: |
-          pyproject.toml
-          scripts/build-requirements.txt
-
-    - name: Set up Ruby 2.6
-      uses: ruby/setup-ruby@v1
-      if: matrix.pkg != 'exe'
-      with:
-        ruby-version: '2.6'
-
-    - name: Install fpm
-      if: matrix.pkg != 'exe'
-      run: gem install --no-document fpm
-
-    - name: Install deps
-      run: |
-        pip install --upgrade pip wheel setuptools
-        pip install .[all]
-        pip install -r scripts/build-requirements.txt
-
-    - name: Pull images
-      run: dvc pull
-
-    - name: Build ${{ matrix.pkg }}
-      run: python scripts/build.py ${{ matrix.pkg }}
-
-    - name: Publish ${{ matrix.pkg }}
-      if: github.event_name == 'release'
-      uses: actions/upload-release-asset@v1.0.2
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-      with:
-        upload_url: ${{ github.event.release.upload_url }}
-        asset_path: scripts/${{ matrix.pkg == 'exe' && 'innosetup' || 'fpm' }}/${{ matrix.asset }}
-        asset_name: ${{ matrix.asset }}
-        asset_content_type: binary/octet-stream
-
   pip:
     runs-on: ubuntu-20.04
     permissions:
       id-token: write
     steps:
     - uses: actions/checkout@v3
       with:
```

### Comparing `dvc-3.1.0/.github/workflows/plugin_tests.yaml` & `dvc-3.2.0/.github/workflows/plugin_tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/.github/workflows/tests.yaml` & `dvc-3.2.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/.pre-commit-config.yaml` & `dvc-3.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/.pre-commit-hooks.yaml` & `dvc-3.2.0/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/CODE_OF_CONDUCT.md` & `dvc-3.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/LICENSE` & `dvc-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/PKG-INFO` & `dvc-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.1.0
+Version: 3.2.0
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.1.0/README.rst` & `dvc-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/_debug.py` & `dvc-3.2.0/dvc/_debug.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/analytics.py` & `dvc-3.2.0/dvc/analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/annotations.py` & `dvc-3.2.0/dvc/annotations.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/api/data.py` & `dvc-3.2.0/dvc/api/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/api/experiments.py` & `dvc-3.2.0/dvc/api/experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/api/scm.py` & `dvc-3.2.0/dvc/api/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/api/show.py` & `dvc-3.2.0/dvc/api/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/cachemgr.py` & `dvc-3.2.0/dvc/cachemgr.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/cli/__init__.py` & `dvc-3.2.0/dvc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/cli/command.py` & `dvc-3.2.0/dvc/cli/command.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/cli/completion.py` & `dvc-3.2.0/dvc/cli/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/cli/parser.py` & `dvc-3.2.0/dvc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/cli/utils.py` & `dvc-3.2.0/dvc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/add.py` & `dvc-3.2.0/dvc/commands/add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/cache.py` & `dvc-3.2.0/dvc/commands/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/check_ignore.py` & `dvc-3.2.0/dvc/commands/check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/checkout.py` & `dvc-3.2.0/dvc/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/commit.py` & `dvc-3.2.0/dvc/commands/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/completion.py` & `dvc-3.2.0/dvc/commands/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/config.py` & `dvc-3.2.0/dvc/commands/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/daemon.py` & `dvc-3.2.0/dvc/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/dag.py` & `dvc-3.2.0/dvc/commands/dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/data.py` & `dvc-3.2.0/dvc/commands/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/data_sync.py` & `dvc-3.2.0/dvc/commands/data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/destroy.py` & `dvc-3.2.0/dvc/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/diff.py` & `dvc-3.2.0/dvc/commands/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/__init__.py` & `dvc-3.2.0/dvc/commands/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/apply.py` & `dvc-3.2.0/dvc/commands/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/branch.py` & `dvc-3.2.0/dvc/commands/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/clean.py` & `dvc-3.2.0/dvc/commands/experiments/clean.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/diff.py` & `dvc-3.2.0/dvc/commands/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/exec_run.py` & `dvc-3.2.0/dvc/commands/experiments/exec_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/ls.py` & `dvc-3.2.0/dvc/commands/experiments/ls.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,22 @@
             rev=self.args.rev,
             num=self.args.num,
             git_remote=git_remote,
         )
 
         for baseline in exps:
             if not (name_only or sha_only):
-                ui.write(f"{baseline[:7]}:")
+                tag_base = "refs/tags/"
+                branch_base = "refs/heads/"
+                name = baseline[:7]
+                if baseline.startswith(tag_base):
+                    name = baseline[len(tag_base) :]
+                elif baseline.startswith(branch_base):
+                    name = baseline[len(branch_base) :]
+                ui.write(f"{name}:")
             for exp_name, rev in exps[baseline]:
                 if name_only:
                     ui.write(exp_name)
                 elif sha_only:
                     ui.write(rev)
                 elif rev:
                     ui.write(f"\t{rev[:7]} [{exp_name}]")
```

### Comparing `dvc-3.1.0/dvc/commands/experiments/pull.py` & `dvc-3.2.0/dvc/commands/experiments/pull.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 import argparse
 import logging
 
 from dvc.cli.command import CmdBase
 from dvc.cli.utils import append_doc_link
-from dvc.exceptions import InvalidArgumentError
 from dvc.ui import ui
 
 logger = logging.getLogger(__name__)
 
 
 class CmdExperimentsPull(CmdBase):
-    def raise_error_if_all_disabled(self):
-        if not any([self.args.experiment, self.args.all_commits, self.args.rev]):
-            raise InvalidArgumentError(
-                "Either provide an `experiment` argument, or use the "
-                "`--rev` or `--all-commits` flag."
-            )
-
     def run(self):
-        self.raise_error_if_all_disabled()
-
         pulled_exps = self.repo.experiments.pull(
             self.args.git_remote,
             self.args.experiment,
             all_commits=self.args.all_commits,
             rev=self.args.rev,
             num=self.args.num,
             force=self.args.force,
@@ -57,15 +47,15 @@
     experiments_pull_parser = experiments_subparsers.add_parser(
         "pull",
         parents=[parent_parser],
         description=append_doc_link(EXPERIMENTS_PULL_HELP, "exp/pull"),
         help=EXPERIMENTS_PULL_HELP,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
-    add_rev_selection_flags(experiments_pull_parser, "Pull", False)
+    add_rev_selection_flags(experiments_pull_parser, "Pull", True)
     experiments_pull_parser.add_argument(
         "-f",
         "--force",
         action="store_true",
         help="Replace local experiment if it already exists.",
     )
     experiments_pull_parser.add_argument(
```

### Comparing `dvc-3.1.0/dvc/commands/experiments/push.py` & `dvc-3.2.0/dvc/commands/experiments/push.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 import argparse
 import logging
 from typing import Any, Dict
 
 from dvc.cli import completion
 from dvc.cli.command import CmdBase
 from dvc.cli.utils import append_doc_link
-from dvc.exceptions import InvalidArgumentError
 from dvc.ui import ui
 
 logger = logging.getLogger(__name__)
 
 
 class CmdExperimentsPush(CmdBase):
-    def raise_error_if_all_disabled(self):
-        if not any([self.args.experiment, self.args.all_commits, self.args.rev]):
-            raise InvalidArgumentError(
-                "Either provide an `experiment` argument, or use the "
-                "`--rev` or `--all-commits` flag."
-            )
-
     @staticmethod
     def log_result(result: Dict[str, Any], remote: str):
         from dvc.utils import humanize
 
         def join_exps(exps):
             return humanize.join([f"[bold]{e}[/]" for e in exps])
 
@@ -55,16 +47,14 @@
             ui.rich_print(
                 "View your experiments at", project_url, style="yellow", soft_wrap=True
             )
 
     def run(self):
         from dvc.repo.experiments.push import UploadError
 
-        self.raise_error_if_all_disabled()
-
         try:
             result = self.repo.experiments.push(
                 self.args.git_remote,
                 self.args.experiment,
                 all_commits=self.args.all_commits,
                 rev=self.args.rev,
                 num=self.args.num,
@@ -98,15 +88,15 @@
     experiments_push_parser = experiments_subparsers.add_parser(
         "push",
         parents=[parent_parser],
         description=append_doc_link(EXPERIMENTS_PUSH_HELP, "exp/push"),
         help=EXPERIMENTS_PUSH_HELP,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
-    add_rev_selection_flags(experiments_push_parser, "Push", False)
+    add_rev_selection_flags(experiments_push_parser, "Push", True)
     experiments_push_parser.add_argument(
         "-f",
         "--force",
         action="store_true",
         help="Replace experiment in the Git remote if it already exists.",
     )
     experiments_push_parser.add_argument(
```

### Comparing `dvc-3.1.0/dvc/commands/experiments/queue_worker.py` & `dvc-3.2.0/dvc/commands/experiments/queue_worker.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/remove.py` & `dvc-3.2.0/dvc/commands/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/run.py` & `dvc-3.2.0/dvc/commands/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/save.py` & `dvc-3.2.0/dvc/commands/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/experiments/show.py` & `dvc-3.2.0/dvc/commands/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/freeze.py` & `dvc-3.2.0/dvc/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/gc.py` & `dvc-3.2.0/dvc/commands/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/get.py` & `dvc-3.2.0/dvc/commands/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/get_url.py` & `dvc-3.2.0/dvc/commands/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/git_hook.py` & `dvc-3.2.0/dvc/commands/git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/imp.py` & `dvc-3.2.0/dvc/commands/imp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/imp_url.py` & `dvc-3.2.0/dvc/commands/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/init.py` & `dvc-3.2.0/dvc/commands/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/install.py` & `dvc-3.2.0/dvc/commands/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/ls/__init__.py` & `dvc-3.2.0/dvc/commands/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/ls/ls_colors.py` & `dvc-3.2.0/dvc/commands/ls/ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/ls_url.py` & `dvc-3.2.0/dvc/commands/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/machine.py` & `dvc-3.2.0/dvc/commands/machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/metrics.py` & `dvc-3.2.0/dvc/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/move.py` & `dvc-3.2.0/dvc/commands/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/params.py` & `dvc-3.2.0/dvc/commands/params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/plots.py` & `dvc-3.2.0/dvc/commands/plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/queue/__init__.py` & `dvc-3.2.0/dvc/commands/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/queue/kill.py` & `dvc-3.2.0/dvc/commands/queue/kill.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/queue/logs.py` & `dvc-3.2.0/dvc/commands/queue/logs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/queue/remove.py` & `dvc-3.2.0/dvc/commands/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/queue/start.py` & `dvc-3.2.0/dvc/commands/queue/start.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/queue/status.py` & `dvc-3.2.0/dvc/commands/queue/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/queue/stop.py` & `dvc-3.2.0/dvc/commands/queue/stop.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/remote.py` & `dvc-3.2.0/dvc/commands/remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/remove.py` & `dvc-3.2.0/dvc/commands/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/repro.py` & `dvc-3.2.0/dvc/commands/repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/root.py` & `dvc-3.2.0/dvc/commands/root.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/stage.py` & `dvc-3.2.0/dvc/commands/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/status.py` & `dvc-3.2.0/dvc/commands/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/unprotect.py` & `dvc-3.2.0/dvc/commands/unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/update.py` & `dvc-3.2.0/dvc/commands/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/commands/version.py` & `dvc-3.2.0/dvc/commands/version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/compare.py` & `dvc-3.2.0/dvc/compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/config.py` & `dvc-3.2.0/dvc/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/config_schema.py` & `dvc-3.2.0/dvc/config_schema.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/daemon.py` & `dvc-3.2.0/dvc/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/dagascii.py` & `dvc-3.2.0/dvc/dagascii.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/data_cloud.py` & `dvc-3.2.0/dvc/data_cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/dependency/__init__.py` & `dvc-3.2.0/dvc/dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/dependency/base.py` & `dvc-3.2.0/dvc/dependency/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/dependency/param.py` & `dvc-3.2.0/dvc/dependency/param.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/dependency/repo.py` & `dvc-3.2.0/dvc/dependency/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/dirs.py` & `dvc-3.2.0/dvc/dirs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/dvcfile.py` & `dvc-3.2.0/dvc/dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/env.py` & `dvc-3.2.0/dvc/env.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/exceptions.py` & `dvc-3.2.0/dvc/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/fs/__init__.py` & `dvc-3.2.0/dvc/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/fs/callbacks.py` & `dvc-3.2.0/dvc/fs/callbacks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/fs/data.py` & `dvc-3.2.0/dvc/fs/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/fs/dvc.py` & `dvc-3.2.0/dvc/fs/dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/fs/git.py` & `dvc-3.2.0/dvc/fs/git.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/ignore.py` & `dvc-3.2.0/dvc/ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/info.py` & `dvc-3.2.0/dvc/info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/lock.py` & `dvc-3.2.0/dvc/lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/logger.py` & `dvc-3.2.0/dvc/logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/machine/__init__.py` & `dvc-3.2.0/dvc/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/machine/backend/base.py` & `dvc-3.2.0/dvc/machine/backend/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/machine/backend/terraform.py` & `dvc-3.2.0/dvc/machine/backend/terraform.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/output.py` & `dvc-3.2.0/dvc/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -688,16 +688,15 @@
             logger.warning("'%s' is empty.", self)
 
         self.ignore()
 
         if self.metric:
             self.verify_metric()
 
-        if self.hash_name == "md5-dos2unix":
-            self.hash_name = "md5"
+        self._update_legacy_hash_name()
         if self.use_cache:
             _, self.meta, self.obj = build(
                 self.cache,
                 self.fs_path,
                 self.fs,
                 self.hash_name,
                 ignore=self.dvcignore,
@@ -713,14 +712,18 @@
             )
             if not self.IS_DEPENDENCY:
                 logger.debug("Output '%s' doesn't use cache. Skipping saving.", self)
 
         self.hash_info = self.obj.hash_info
         self.files = None
 
+    def _update_legacy_hash_name(self):
+        if self.hash_name == "md5-dos2unix" and self.changed_checksum():
+            self.hash_name = "md5"
+
     def set_exec(self) -> None:
         if self.isfile() and self.meta.isexec:
             self.cache.set_exec(self.fs_path)
 
     def _checkout(self, *args, **kwargs) -> Optional[bool]:
         from dvc_data.hashfile.checkout import CheckoutError as _CheckoutError
         from dvc_data.hashfile.checkout import LinkError, PromptError
@@ -961,15 +964,18 @@
             if allow_missing:
                 return None
             raise
         self.set_exec()
         return added, False if added else modified
 
     def remove(self, ignore_remove=False):
-        self.fs.remove(self.fs_path, recursive=True)
+        try:
+            self.fs.remove(self.fs_path, recursive=True)
+        except FileNotFoundError:
+            pass
         if self.protocol != Schemes.LOCAL:
             return
 
         if ignore_remove:
             self.ignore_remove()
 
     def move(self, out):
@@ -1331,14 +1337,15 @@
         path = path or self.fs_path
         if self.hash_info and not self.is_dir_checksum and self.fs_path != path:
             raise DvcException(
                 f"Cannot modify '{self}' which is being tracked as a file"
             )
 
         assert self.repo
+        self._update_legacy_hash_name()
         cache = self.cache if self.use_cache else self.local_cache
         assert isinstance(cache, HashFileDB)
 
         new: "HashFile"
         try:
             assert self.hash_name
             staging, meta, obj = build(
```

### Comparing `dvc-3.1.0/dvc/parsing/__init__.py` & `dvc-3.2.0/dvc/parsing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,14 +228,26 @@
         self.wdir = self.resolver.wdir
         self.relpath = self.resolver.relpath
         self.context = context
         self.name = name
         self.definition = definition
         self.where = where
 
+    def _resolve_wdir(
+        self, context: Context, name: str, wdir: Optional[str] = None
+    ) -> str:
+        if not wdir:
+            return self.wdir
+
+        try:
+            wdir = to_str(context.resolve_str(wdir))
+        except (ContextError, ParseError) as exc:
+            format_and_raise(exc, f"'{self.where}.{name}.wdir'", self.relpath)
+        return self.resolver.fs.path.join(self.wdir, wdir)
+
     def resolve(self, **kwargs):
         try:
             return self.resolve_stage(**kwargs)
         except ContextError as exc:
             format_and_raise(exc, f"stage '{self.name}'", self.relpath)
 
     def resolve_stage(self, skip_checks: bool = False) -> "DictStrAny":
@@ -245,15 +257,41 @@
             # we can check for syntax errors as we go for interpolated entries,
             # but for foreach-generated ones, once is enough, which it does
             # that itself. See `ForeachDefinition.do_definition`.
             check_syntax_errors(self.definition, name, self.relpath)
 
         # we need to pop vars from generated/evaluated data
         definition = deepcopy(self.definition)
+
+        wdir = self._resolve_wdir(context, name, definition.get(WDIR_KWD))
+        vars_ = definition.pop(VARS_KWD, [])
+        # FIXME: Should `vars` be templatized?
+        check_interpolations(vars_, f"{self.where}.{name}.vars", self.relpath)
+        if vars_:
+            # Optimization: Lookahead if it has any vars, if it does not, we
+            # don't need to clone them.
+            context = Context.clone(context)
+
+        try:
+            fs = self.resolver.fs
+            context.load_from_vars(fs, vars_, wdir, stage_name=name)
+        except VarsAlreadyLoaded as exc:
+            format_and_raise(exc, f"'{self.where}.{name}.vars'", self.relpath)
+
+        logger.trace(  # type: ignore[attr-defined]
+            "Context during resolution of stage %s:\n%s", name, context
+        )
+
         with context.track() as tracked_data:
+            # NOTE: we do not pop "wdir", and resolve it again
+            # this does not affect anything and is done to try to
+            # track the source of `wdir` interpolation.
+            # This works because of the side-effect that we do not
+            # allow overwriting and/or str interpolating complex objects.
+            # Fix if/when those assumptions are no longer valid.
             resolved = {
                 key: self._resolve(context, value, key, skip_checks)
                 for key, value in definition.items()
             }
 
         self.resolver.track_vars(name, tracked_data)
         return {name: resolved}
```

### Comparing `dvc-3.1.0/dvc/parsing/context.py` & `dvc-3.2.0/dvc/parsing/context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/parsing/interpolate.py` & `dvc-3.2.0/dvc/parsing/interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/pathspec_math.py` & `dvc-3.2.0/dvc/pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/progress.py` & `dvc-3.2.0/dvc/progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/prompt.py` & `dvc-3.2.0/dvc/prompt.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/render/convert.py` & `dvc-3.2.0/dvc/render/convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/render/converter/__init__.py` & `dvc-3.2.0/dvc/render/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/render/converter/image.py` & `dvc-3.2.0/dvc/render/converter/image.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/render/converter/vega.py` & `dvc-3.2.0/dvc/render/converter/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/render/match.py` & `dvc-3.2.0/dvc/render/match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/__init__.py` & `dvc-3.2.0/dvc/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/add.py` & `dvc-3.2.0/dvc/repo/add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/artifacts.py` & `dvc-3.2.0/dvc/repo/artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/brancher.py` & `dvc-3.2.0/dvc/repo/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/checkout.py` & `dvc-3.2.0/dvc/repo/checkout.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 import logging
 import os
-from typing import Dict, List
+from typing import TYPE_CHECKING, Dict, List
 
-from dvc.exceptions import CheckoutError, CheckoutErrorSuggestGit, NoOutputOrStageError
+from dvc.exceptions import (
+    CheckoutError,
+    CheckoutErrorSuggestGit,
+    DvcException,
+    NoOutputOrStageError,
+)
 from dvc.utils import relpath
 
 from . import locked
 
+if TYPE_CHECKING:
+    from dvc_data.index import BaseDataIndex, DataIndexEntry
+    from dvc_objects.fs.base import FileSystem
+
 logger = logging.getLogger(__name__)
 
 
 def _fspath_dir(path):
     if not os.path.exists(str(path)):
         return str(path)
 
@@ -55,26 +64,52 @@
                 elif not out_changes.get(out_key):
                     out_changes[out_key] = MODIFY
                 break
 
     return out_changes
 
 
+def _check_can_delete(
+    entries: List["DataIndexEntry"],
+    index: "BaseDataIndex",
+    path: str,
+    fs: "FileSystem",
+):
+    entry_paths = []
+    for entry in entries:
+        try:
+            cache_fs, cache_path = index.storage_map.get_cache(entry)
+        except ValueError:
+            continue
+
+        if cache_fs.exists(cache_path):
+            continue
+
+        entry_paths.append(fs.path.join(path, *entry.key))
+
+    if not entry_paths:
+        return
+
+    raise DvcException(
+        "Can't remove the following unsaved files without confirmation. "
+        "Use `--force` to force.\n" + "\n".join(entry_paths)
+    )
+
+
 @locked
 def checkout(  # noqa: C901
     self,
     targets=None,
     with_deps=False,
     force=False,
     relink=False,
     recursive=False,
     allow_missing=False,
     **kwargs,
 ):
-    from dvc import prompt
     from dvc.fs.callbacks import Callback
     from dvc.repo.index import build_data_index
     from dvc.stage.exceptions import StageFileBadNameError, StageFileDoesNotExistError
     from dvc_data.index.checkout import ADD, DELETE, MODIFY, apply, compare
 
     stats: Dict[str, List[str]] = {
         "added": [],
@@ -119,44 +154,53 @@
 
     with Callback.as_tqdm_callback(
         desc="Comparing indexes",
         unit="entry",
     ) as cb:
         diff = compare(old, new, relink=relink, delete=True, callback=cb)
 
-    failed = []
+    if not force:
+        _check_can_delete(diff.files_delete, new, self.root_dir, self.fs)
+
+    failed = set()
+    out_paths = [out.fs_path for out in view.outs if out.use_cache and out.is_in_repo]
 
     def checkout_onerror(src_path, dest_path, _exc):
         logger.debug(
             "failed to create {%s} from {%s}", dest_path, src_path, exc_info=True
         )
-        failed.append(dest_path)
+
+        for out_path in out_paths:
+            if self.fs.path.isin_or_eq(dest_path, out_path):
+                failed.add(out_path)
 
     with Callback.as_tqdm_callback(
         unit="file",
         desc="Checkout",
     ) as cb:
-        changes = apply(
+        apply(
             diff,
             self.root_dir,
             self.fs,
             callback=cb,
-            prompt=prompt.confirm,
             update_meta=False,
-            force=force,
             onerror=checkout_onerror,
             state=self.state,
             **kwargs,
         )
 
-    out_changes = _build_out_changes(view, changes)
+    out_changes = _build_out_changes(view, diff.changes)
 
     typ_map = {ADD: "added", DELETE: "deleted", MODIFY: "modified"}
     for key, typ in out_changes.items():
         out_path = self.fs.path.join(self.root_dir, *key)
-        self.state.save_link(out_path, self.fs)
-        stats[typ_map[typ]].append(_fspath_dir(out_path))
+
+        if out_path in failed:
+            self.fs.remove(out_path, recursive=True)
+        else:
+            self.state.save_link(out_path, self.fs)
+            stats[typ_map[typ]].append(_fspath_dir(out_path))
 
     if failed and not allow_missing:
-        raise CheckoutError(failed, stats)
+        raise CheckoutError([relpath(out_path) for out_path in failed], stats)
 
     return stats
```

### Comparing `dvc-3.1.0/dvc/repo/collect.py` & `dvc-3.2.0/dvc/repo/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/commit.py` & `dvc-3.2.0/dvc/repo/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/data.py` & `dvc-3.2.0/dvc/repo/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/destroy.py` & `dvc-3.2.0/dvc/repo/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/diff.py` & `dvc-3.2.0/dvc/repo/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/__init__.py` & `dvc-3.2.0/dvc/repo/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/apply.py` & `dvc-3.2.0/dvc/repo/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/branch.py` & `dvc-3.2.0/dvc/repo/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/brancher.py` & `dvc-3.2.0/dvc/repo/experiments/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/cache.py` & `dvc-3.2.0/dvc/repo/experiments/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/collect.py` & `dvc-3.2.0/dvc/repo/experiments/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/diff.py` & `dvc-3.2.0/dvc/repo/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/exceptions.py` & `dvc-3.2.0/dvc/repo/experiments/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/executor/base.py` & `dvc-3.2.0/dvc/repo/experiments/executor/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/executor/local.py` & `dvc-3.2.0/dvc/repo/experiments/executor/local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/executor/ssh.py` & `dvc-3.2.0/dvc/repo/experiments/executor/ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/ls.py` & `dvc-3.2.0/dvc/repo/experiments/ls.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     base = "refs/heads"
     ref_heads = repo.scm.describe(remained, base=base)
 
     results = defaultdict(list)
     for baseline in ref_info_dict:
         name = baseline
         if tags[baseline] or ref_heads[baseline]:
-            name = tags[baseline] or ref_heads[baseline][len(base) + 1 :]
+            name = tags[baseline] or ref_heads[baseline]
         for info in ref_info_dict[baseline]:
             if git_remote:
                 exp_rev = None
             else:
                 exp_rev = repo.scm.get_ref(str(info))
             results[name].append((info.name, exp_rev))
```

### Comparing `dvc-3.1.0/dvc/repo/experiments/pull.py` & `dvc-3.2.0/dvc/repo/experiments/pull.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,49 +17,49 @@
 
 
 @locked
 @scm_context
 def pull(  # noqa: C901
     repo,
     git_remote: str,
-    exp_names: Union[Iterable[str], str],
+    exp_names: Optional[Union[Iterable[str], str]] = None,
     all_commits=False,
     rev: Optional[Union[List[str], str]] = None,
     num=1,
     force: bool = False,
     pull_cache: bool = False,
     **kwargs,
 ) -> Iterable[str]:
     exp_ref_set: Set["ExpRefInfo"] = set()
     if all_commits:
         exp_ref_set.update(exp_refs(repo.scm, git_remote))
+    elif exp_names:
+        if isinstance(exp_names, str):
+            exp_names = [exp_names]
+        exp_ref_dict = resolve_name(repo.scm, exp_names, git_remote)
+
+        unresolved_exp_names = []
+        for exp_name, exp_ref in exp_ref_dict.items():
+            if exp_ref is None:
+                unresolved_exp_names.append(exp_name)
+            else:
+                exp_ref_set.add(exp_ref)
+
+        if unresolved_exp_names:
+            raise UnresolvedExpNamesError(unresolved_exp_names)
+
     else:
-        if exp_names:
-            if isinstance(exp_names, str):
-                exp_names = [exp_names]
-            exp_ref_dict = resolve_name(repo.scm, exp_names, git_remote)
-
-            unresolved_exp_names = []
-            for exp_name, exp_ref in exp_ref_dict.items():
-                if exp_ref is None:
-                    unresolved_exp_names.append(exp_name)
-                else:
-                    exp_ref_set.add(exp_ref)
-
-            if unresolved_exp_names:
-                raise UnresolvedExpNamesError(unresolved_exp_names)
-
-        if rev:
-            if isinstance(rev, str):
-                rev = [rev]
-            rev_dict = iter_revs(repo.scm, rev, num)
-            rev_set = set(rev_dict.keys())
-            ref_info_dict = exp_refs_by_baseline(repo.scm, rev_set, git_remote)
-            for _, ref_info_list in ref_info_dict.items():
-                exp_ref_set.update(ref_info_list)
+        rev = rev or "HEAD"
+        if isinstance(rev, str):
+            rev = [rev]
+        rev_dict = iter_revs(repo.scm, rev, num)
+        rev_set = set(rev_dict.keys())
+        ref_info_dict = exp_refs_by_baseline(repo.scm, rev_set, git_remote)
+        for _, ref_info_list in ref_info_dict.items():
+            exp_ref_set.update(ref_info_list)
 
     pull_result = _pull(repo, git_remote, exp_ref_set, force)
 
     if pull_result[SyncStatus.DIVERGED]:
         diverged_refs = [ref.name for ref in pull_result[SyncStatus.DIVERGED]]
         ui.warn(
             f"Local experiment '{diverged_refs}' has diverged from remote "
```

### Comparing `dvc-3.1.0/dvc/repo/experiments/push.py` & `dvc-3.2.0/dvc/repo/experiments/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,29 +93,30 @@
 
 
 @locked
 @scm_context
 def push(
     repo: "Repo",
     git_remote: str,
-    exp_names: Union[List[str], str],
+    exp_names: Optional[Union[List[str], str]] = None,
     all_commits: bool = False,
     rev: Optional[Union[List[str], str]] = None,
     num: int = 1,
     force: bool = False,
     push_cache: bool = False,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     exp_ref_set: Set["ExpRefInfo"] = set()
     assert isinstance(repo.scm, Git)
     if all_commits:
         exp_ref_set.update(exp_refs(repo.scm))
     if exp_names:
         exp_ref_set.update(exp_refs_from_names(repo.scm, ensure_list(exp_names)))
-    if rev:
+    else:
+        rev = rev or "HEAD"
         if isinstance(rev, str):
             rev = [rev]
         exp_ref_set.update(exp_refs_from_rev(repo.scm, rev, num=num))
 
     push_result = _push(repo, git_remote, exp_ref_set, force)
 
     refs = {
```

### Comparing `dvc-3.1.0/dvc/repo/experiments/queue/base.py` & `dvc-3.2.0/dvc/repo/experiments/queue/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/queue/celery.py` & `dvc-3.2.0/dvc/repo/experiments/queue/celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/queue/remove.py` & `dvc-3.2.0/dvc/repo/experiments/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/queue/tasks.py` & `dvc-3.2.0/dvc/repo/experiments/queue/tasks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/queue/tempdir.py` & `dvc-3.2.0/dvc/repo/experiments/queue/tempdir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/queue/utils.py` & `dvc-3.2.0/dvc/repo/experiments/queue/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/queue/workspace.py` & `dvc-3.2.0/dvc/repo/experiments/queue/workspace.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/refs.py` & `dvc-3.2.0/dvc/repo/experiments/refs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/remove.py` & `dvc-3.2.0/dvc/repo/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/run.py` & `dvc-3.2.0/dvc/repo/experiments/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/save.py` & `dvc-3.2.0/dvc/repo/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/serialize.py` & `dvc-3.2.0/dvc/repo/experiments/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/show.py` & `dvc-3.2.0/dvc/repo/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/stash.py` & `dvc-3.2.0/dvc/repo/experiments/stash.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/experiments/utils.py` & `dvc-3.2.0/dvc/repo/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/fetch.py` & `dvc-3.2.0/dvc/repo/fetch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/gc.py` & `dvc-3.2.0/dvc/repo/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/get.py` & `dvc-3.2.0/dvc/repo/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/get_url.py` & `dvc-3.2.0/dvc/repo/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/graph.py` & `dvc-3.2.0/dvc/repo/graph.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/imp_url.py` & `dvc-3.2.0/dvc/repo/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/imports.py` & `dvc-3.2.0/dvc/repo/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/index.py` & `dvc-3.2.0/dvc/repo/index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/init.py` & `dvc-3.2.0/dvc/repo/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/install.py` & `dvc-3.2.0/dvc/repo/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/ls.py` & `dvc-3.2.0/dvc/repo/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/ls_url.py` & `dvc-3.2.0/dvc/repo/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/metrics/diff.py` & `dvc-3.2.0/dvc/repo/metrics/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/metrics/show.py` & `dvc-3.2.0/dvc/repo/metrics/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/move.py` & `dvc-3.2.0/dvc/repo/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/open_repo.py` & `dvc-3.2.0/dvc/repo/open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/params/diff.py` & `dvc-3.2.0/dvc/repo/params/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/params/show.py` & `dvc-3.2.0/dvc/repo/params/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/plots/__init__.py` & `dvc-3.2.0/dvc/repo/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/plots/diff.py` & `dvc-3.2.0/dvc/repo/plots/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/pull.py` & `dvc-3.2.0/dvc/repo/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/push.py` & `dvc-3.2.0/dvc/repo/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/remove.py` & `dvc-3.2.0/dvc/repo/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/reproduce.py` & `dvc-3.2.0/dvc/repo/reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/run.py` & `dvc-3.2.0/dvc/repo/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/scm_context.py` & `dvc-3.2.0/dvc/repo/scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/stage.py` & `dvc-3.2.0/dvc/repo/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/status.py` & `dvc-3.2.0/dvc/repo/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/trie.py` & `dvc-3.2.0/dvc/repo/trie.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/update.py` & `dvc-3.2.0/dvc/repo/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/repo/worktree.py` & `dvc-3.2.0/dvc/repo/worktree.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,23 +154,23 @@
         with Callback.as_tqdm_callback(
             unit="file",
             desc=f"Pushing to remote {remote_obj.name!r}",
             disable=total == 0,
         ) as cb:
             cb.set_size(total)
             try:
-                stats = apply(
+                apply(
                     diff,
                     remote_obj.path,
                     remote_obj.fs,
                     callback=cb,
                     latest_only=remote_obj.worktree,
                     jobs=jobs,
                 )
-                pushed += sum(len(changes) for changes in stats.values())
+                pushed += sum(len(changes) for changes in diff.changes.values())
             except VersioningNotSupported:
                 logger.exception("")
                 raise DvcException(
                     f"remote {remote_obj.name!r} does not support versioning"
                 ) from None
 
         if remote_obj.index is not None:
```

### Comparing `dvc-3.1.0/dvc/rwlock.py` & `dvc-3.2.0/dvc/rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/schema.py` & `dvc-3.2.0/dvc/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 }
 
 OUT_PSTAGE_DETAILED_SCHEMA = {
     str: {
         **ANNOTATION_SCHEMA,  # type: ignore[arg-type]
         Output.PARAM_CACHE: bool,
         Output.PARAM_PERSIST: bool,
+        "checkpoint": bool,
         Output.PARAM_REMOTE: str,
         Output.PARAM_PUSH: bool,
     }
 }
 
 PLOTS = "plots"
 PLOT_PROPS = {
@@ -69,20 +70,22 @@
     Output.PARAM_PLOT_HEADER: bool,
 }
 PLOT_PROPS_SCHEMA = {**OUT_PSTAGE_DETAILED_SCHEMA[str], **PLOT_PROPS}
 PLOT_PSTAGE_SCHEMA = {str: Any(PLOT_PROPS_SCHEMA, [PLOT_PROPS_SCHEMA])}
 
 PARAM_PSTAGE_NON_DEFAULT_SCHEMA = {str: [str]}
 
+VARS_SCHEMA = [str, dict]
 
 STAGE_DEFINITION = {
     Required(StageParams.PARAM_CMD): Any(str, list),
     Optional(StageParams.PARAM_WDIR): str,
     Optional(StageParams.PARAM_DEPS): [str],
     Optional(StageParams.PARAM_PARAMS): [Any(str, dict)],
+    Optional(VARS_KWD): VARS_SCHEMA,
     Optional(StageParams.PARAM_FROZEN): bool,
     Optional(StageParams.PARAM_META): object,
     Optional(StageParams.PARAM_DESC): str,
     Optional(StageParams.PARAM_ALWAYS_CHANGED): bool,
     Optional(StageParams.PARAM_OUTS): [Any(str, OUT_PSTAGE_DETAILED_SCHEMA)],
     Optional(StageParams.PARAM_METRICS): [Any(str, OUT_PSTAGE_DETAILED_SCHEMA)],
     Optional(StageParams.PARAM_PLOTS): [Any(str, PLOT_PSTAGE_SCHEMA)],
@@ -116,15 +119,15 @@
 }
 SINGLE_PIPELINE_STAGE_SCHEMA = {
     str: either_or(STAGE_DEFINITION, FOREACH_IN, [FOREACH_KWD, DO_KWD])
 }
 MULTI_STAGE_SCHEMA = {
     PLOTS: [Any(str, SINGLE_PLOT_SCHEMA)],
     STAGES: SINGLE_PIPELINE_STAGE_SCHEMA,
-    VARS_KWD: [str, dict],
+    VARS_KWD: VARS_SCHEMA,
     StageParams.PARAM_PARAMS: [str],
     StageParams.PARAM_METRICS: [str],
     ARTIFACTS: SINGLE_ARTIFACT_SCHEMA,
 }
 
 COMPILED_SINGLE_STAGE_SCHEMA = Schema(SINGLE_STAGE_SCHEMA)
 COMPILED_MULTI_STAGE_SCHEMA = Schema(MULTI_STAGE_SCHEMA)
```

### Comparing `dvc-3.1.0/dvc/scm.py` & `dvc-3.2.0/dvc/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/stage/__init__.py` & `dvc-3.2.0/dvc/stage/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/stage/cache.py` & `dvc-3.2.0/dvc/stage/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/stage/decorators.py` & `dvc-3.2.0/dvc/stage/decorators.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/stage/exceptions.py` & `dvc-3.2.0/dvc/stage/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/stage/imports.py` & `dvc-3.2.0/dvc/stage/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/stage/loader.py` & `dvc-3.2.0/dvc/stage/loader.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/stage/run.py` & `dvc-3.2.0/dvc/stage/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/stage/serialize.py` & `dvc-3.2.0/dvc/stage/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/stage/utils.py` & `dvc-3.2.0/dvc/stage/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/README.rst` & `dvc-3.2.0/dvc/testing/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/api_tests.py` & `dvc-3.2.0/dvc/testing/api_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_checkout.py` & `dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_data_status.py` & `dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/benchmarks/cli/commands/test_plots.py` & `dvc-3.2.0/dvc/testing/benchmarks/cli/commands/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py` & `dvc-3.2.0/dvc/testing/benchmarks/cli/stories/test_modify_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/benchmarks/fixtures.py` & `dvc-3.2.0/dvc/testing/benchmarks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/benchmarks/plugin.py` & `dvc-3.2.0/dvc/testing/benchmarks/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/cloud.py` & `dvc-3.2.0/dvc/testing/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/fixtures.py` & `dvc-3.2.0/dvc/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/path_info.py` & `dvc-3.2.0/dvc/testing/path_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/plugin.py` & `dvc-3.2.0/dvc/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/remote_tests.py` & `dvc-3.2.0/dvc/testing/remote_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/tmp_dir.py` & `dvc-3.2.0/dvc/testing/tmp_dir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/testing/workspace_tests.py` & `dvc-3.2.0/dvc/testing/workspace_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/ui/__init__.py` & `dvc-3.2.0/dvc/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/ui/_rich_progress.py` & `dvc-3.2.0/dvc/ui/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/ui/pager.py` & `dvc-3.2.0/dvc/ui/pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/ui/table.py` & `dvc-3.2.0/dvc/ui/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/updater.py` & `dvc-3.2.0/dvc/updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/__init__.py` & `dvc-3.2.0/dvc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/cli_parse.py` & `dvc-3.2.0/dvc/utils/cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/collections.py` & `dvc-3.2.0/dvc/utils/collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/diff.py` & `dvc-3.2.0/dvc/utils/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/fs.py` & `dvc-3.2.0/dvc/utils/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/humanize.py` & `dvc-3.2.0/dvc/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/hydra.py` & `dvc-3.2.0/dvc/utils/hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/serialize/__init__.py` & `dvc-3.2.0/dvc/utils/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/serialize/_common.py` & `dvc-3.2.0/dvc/utils/serialize/_common.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/serialize/_json.py` & `dvc-3.2.0/dvc/utils/serialize/_json.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/serialize/_py.py` & `dvc-3.2.0/dvc/utils/serialize/_py.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/serialize/_toml.py` & `dvc-3.2.0/dvc/utils/serialize/_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/serialize/_yaml.py` & `dvc-3.2.0/dvc/utils/serialize/_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/strictyaml.py` & `dvc-3.2.0/dvc/utils/strictyaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/studio.py` & `dvc-3.2.0/dvc/utils/studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/table.py` & `dvc-3.2.0/dvc/utils/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc/utils/threadpool.py` & `dvc-3.2.0/dvc/utils/threadpool.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/dvc.egg-info/PKG-INFO` & `dvc-3.2.0/dvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.1.0
+Version: 3.2.0
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.1.0/dvc.egg-info/SOURCES.txt` & `dvc-3.2.0/dvc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 .pre-commit-hooks.yaml
 .zenodo.json
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.rst
 pyproject.toml
-.dvc/.gitignore
-.dvc/config
 .github/PULL_REQUEST_TEMPLATE.md
 .github/codecov.yml
 .github/dependabot.yml
 .github/mergify.yml
 .github/release.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
@@ -311,35 +309,17 @@
 dvc/utils/serialize/__init__.py
 dvc/utils/serialize/_common.py
 dvc/utils/serialize/_json.py
 dvc/utils/serialize/_py.py
 dvc/utils/serialize/_toml.py
 dvc/utils/serialize/_yaml.py
 scripts/build-requirements.txt
-scripts/build.py
 scripts/build_package.sh
-scripts/fpm/.gitignore
-scripts/fpm/after-install.sh
-scripts/fpm/after-remove.sh
-scripts/fpm/build.py
-scripts/fpm/notarize.py
-scripts/fpm/sign.py
-scripts/innosetup/.gitignore
-scripts/innosetup/addSymLinkPermissions.ps1
-scripts/innosetup/addsymlink.iss
-scripts/innosetup/build.py
-scripts/innosetup/dvc.ico.dvc
-scripts/innosetup/dvc_left.bmp.dvc
-scripts/innosetup/dvc_up.bmp.dvc
-scripts/innosetup/modpath.iss
-scripts/innosetup/setup.iss
 scripts/pyinstaller/.gitignore
 scripts/pyinstaller/build.py
-scripts/pyinstaller/entitlements.plist
-scripts/pyinstaller/sign.py
 scripts/pyinstaller/hooks/hook-asyncssh.py
 scripts/pyinstaller/hooks/hook-celery.py
 scripts/pyinstaller/hooks/hook-dvc.py
 scripts/pyinstaller/hooks/hook-dvc.system.py
 scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
 scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
 scripts/pyinstaller/hooks/hook-dvc_task.py
```

### Comparing `dvc-3.1.0/dvc.egg-info/requires.txt` & `dvc-3.2.0/dvc.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 colorama>=0.3.9
 configobj>=5.0.6
 distro>=1.3
 dpath<3,>=2.1.0
-dvc-data<2.1.0,>=2.0.2
+dvc-data<2.4.0,>=2.3.0
 dvc-http>=2.29.0
 dvc-render<1,>=0.3.1
 dvc-studio-client<1,>=0.9.2
 dvc-task<1,>=0.3.0
 flatten_dict<1,>=0.4.1
 flufl.lock>=5
 funcy>=1.14
@@ -20,15 +20,15 @@
 psutil>=5.8
 pydot>=1.2.4
 pygtrie>=2.3.2
 pyparsing>=2.4.7
 requests>=2.22
 rich>=12
 ruamel.yaml>=0.17.11
-scmrepo<2,>=1.0.0
+scmrepo<2,>=1.0.4
 shortuuid>=0.5
 shtab<2,>=1.3.4
 tabulate>=0.8.7
 tomlkit>=0.11.1
 tqdm<5,>=4.63.1
 voluptuous>=0.11.7
 zc.lockfile>=1.2.1
```

### Comparing `dvc-3.1.0/pyproject.toml` & `dvc-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 dynamic = ["version"]
 dependencies = [
     "colorama>=0.3.9",
     "configobj>=5.0.6",
     "distro>=1.3",
     "dpath<3,>=2.1.0",
-    "dvc-data>=2.0.2,<2.1.0",
+    "dvc-data>=2.3.0,<2.4.0",
     "dvc-http>=2.29.0",
     "dvc-render>=0.3.1,<1",
     "dvc-studio-client>=0.9.2,<1",
     "dvc-task>=0.3.0,<1",
     "flatten_dict<1,>=0.4.1",
     "flufl.lock>=5",
     "funcy>=1.14",
@@ -52,15 +52,15 @@
     "psutil>=5.8",
     "pydot>=1.2.4",
     "pygtrie>=2.3.2",
     "pyparsing>=2.4.7",
     "requests>=2.22",
     "rich>=12",
     "ruamel.yaml>=0.17.11",
-    "scmrepo>=1.0.0,<2",
+    "scmrepo>=1.0.4,<2",
     "shortuuid>=0.5",
     "shtab<2,>=1.3.4",
     "tabulate>=0.8.7",
     "tomlkit>=0.11.1",
     "tqdm<5,>=4.63.1",
     "voluptuous>=0.11.7",
     "zc.lockfile>=1.2.1",
```

### Comparing `dvc-3.1.0/scripts/pyinstaller/build.py` & `dvc-3.2.0/scripts/pyinstaller/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/scripts/pyinstaller/hooks/hook-dvc.py` & `dvc-3.2.0/scripts/pyinstaller/hooks/hook-dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/conftest.py` & `dvc-3.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/dir_helpers.py` & `dvc-3.2.0/tests/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/api/test_data.py` & `dvc-3.2.0/tests/func/api/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/api/test_experiments.py` & `dvc-3.2.0/tests/func/api/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/api/test_scm.py` & `dvc-3.2.0/tests/func/api/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/api/test_show.py` & `dvc-3.2.0/tests/func/api/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/artifacts/test_artifacts.py` & `dvc-3.2.0/tests/func/artifacts/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/data/db/test_index.py` & `dvc-3.2.0/tests/func/data/db/test_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/conftest.py` & `dvc-3.2.0/tests/func/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/executor/test_ssh.py` & `dvc-3.2.0/tests/func/experiments/executor/test_ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/test_apply.py` & `dvc-3.2.0/tests/func/experiments/test_apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/test_diff.py` & `dvc-3.2.0/tests/func/experiments/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/test_experiments.py` & `dvc-3.2.0/tests/func/experiments/test_experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,38 +358,38 @@
     ref_info_b = first(exp_refs_by_rev(scm, exp_b))
 
     tmp_dir.scm_gen("new", "new", commit="new")
     results = dvc.experiments.run(exp_stage.addressing, params=["foo=4"])
     exp_c = first(results)
     ref_info_c = first(exp_refs_by_rev(scm, exp_c))
 
-    assert dvc.experiments.ls() == {"master": [(ref_info_c.name, exp_c)]}
+    assert dvc.experiments.ls() == {"refs/heads/master": [(ref_info_c.name, exp_c)]}
 
     exp_list = dvc.experiments.ls(rev=ref_info_a.baseline_sha)
     assert {key: set(val) for key, val in exp_list.items()} == {
         baseline_a: {(ref_info_a.name, exp_a), (ref_info_b.name, exp_b)}
     }
 
     exp_list = dvc.experiments.ls(rev=[baseline_a, scm.get_rev()])
     assert {key: set(val) for key, val in exp_list.items()} == {
         baseline_a: {(ref_info_a.name, exp_a), (ref_info_b.name, exp_b)},
-        "master": {(ref_info_c.name, exp_c)},
+        "refs/heads/master": {(ref_info_c.name, exp_c)},
     }
 
     exp_list = dvc.experiments.ls(all_commits=True)
     assert {key: set(val) for key, val in exp_list.items()} == {
         baseline_a: {(ref_info_a.name, exp_a), (ref_info_b.name, exp_b)},
-        "master": {(ref_info_c.name, exp_c)},
+        "refs/heads/master": {(ref_info_c.name, exp_c)},
     }
 
     scm.checkout("branch", True)
     exp_list = dvc.experiments.ls(all_commits=True)
     assert {key: set(val) for key, val in exp_list.items()} == {
         baseline_a: {(ref_info_a.name, exp_a), (ref_info_b.name, exp_b)},
-        "branch": {(ref_info_c.name, exp_c)},
+        "refs/heads/branch": {(ref_info_c.name, exp_c)},
     }
 
 
 def test_subdir(tmp_dir, scm, dvc, workspace):
     subdir = tmp_dir / "dir"
     subdir.gen("copy.py", COPY_SCRIPT)
     subdir.gen("params.yaml", "foo: 1")
@@ -672,15 +672,15 @@
     assert (tmp_dir / DVC_EXP_NAME).read_text().strip() == "foo"
 
 
 def test_experiment_unchanged(tmp_dir, scm, dvc, exp_stage):
     dvc.experiments.run(exp_stage.addressing)
     dvc.experiments.run(exp_stage.addressing)
 
-    assert len(dvc.experiments.ls()["master"]) == 2
+    assert len(dvc.experiments.ls()["refs/heads/master"]) == 2
 
 
 def test_experiment_run_dry(tmp_dir, scm, dvc, exp_stage):
     dvc.experiments.run(exp_stage.addressing, dry=True)
 
     assert len(dvc.experiments.ls()["master"]) == 0
```

### Comparing `dvc-3.1.0/tests/func/experiments/test_queue.py` & `dvc-3.2.0/tests/func/experiments/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/test_remote.py` & `dvc-3.2.0/tests/func/experiments/test_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
     git_upstream.tmp_dir.scm.remove_ref(str(ref_info1))
     assert git_upstream.tmp_dir.scm.get_ref(str(ref_info1)) is None
 
     dvc.experiments.push(remote, [ref_info1.name])
     assert git_upstream.tmp_dir.scm.get_ref(str(ref_info1)) == exp1
 
+    dvc.experiments.push(remote)
+    assert git_upstream.tmp_dir.scm.get_ref(str(ref_info3)) == exp3
+
 
 @pytest.mark.parametrize("all_,rev,result3", [(True, False, True), (False, True, None)])
 def test_push_args(tmp_dir, scm, dvc, git_upstream, exp_stage, all_, rev, result3):
     remote = git_upstream.url
     baseline = scm.get_rev()
 
     results = dvc.experiments.run(exp_stage.addressing, params=["foo=1"])
@@ -161,22 +164,27 @@
     assert {key: set(val) for key, val in exp_list.items()} == {
         baseline_a: {(ref_info_a.name, None), (ref_info_b.name, None)}
     }
 
     exp_list = downstream_exp.ls(all_commits=True, git_remote=remote)
     assert {key: set(val) for key, val in exp_list.items()} == {
         baseline_a: {(ref_info_a.name, None), (ref_info_b.name, None)},
-        "master": {(ref_info_c.name, None)},
+        "refs/heads/master": {(ref_info_c.name, None)},
     }
 
 
 @pytest.mark.parametrize("use_url", [True, False])
 def test_pull(tmp_dir, scm, dvc, git_downstream, exp_stage, use_url):
     from dvc.exceptions import InvalidArgumentError
 
+    # fetch and checkout to downstream so both repos start from same commit
+    downstream_repo = git_downstream.tmp_dir.scm.gitpython.repo
+    fetched = downstream_repo.remote(git_downstream.remote).fetch()
+    downstream_repo.git.checkout(fetched)
+
     remote = git_downstream.url if use_url else git_downstream.remote
     downstream_exp = git_downstream.tmp_dir.dvc.experiments
     with pytest.raises(InvalidArgumentError):
         downstream_exp.pull(remote, ["foo"])
 
     results = dvc.experiments.run(exp_stage.addressing, params=["foo=1"])
     exp1 = first(results)
@@ -196,14 +204,17 @@
     assert git_downstream.tmp_dir.scm.get_ref(str(ref_info3)) is None
 
     git_downstream.tmp_dir.scm.remove_ref(str(ref_info1))
 
     downstream_exp.pull(remote, [str(ref_info1)])
     assert git_downstream.tmp_dir.scm.get_ref(str(ref_info1)) == exp1
 
+    downstream_exp.pull(remote)
+    assert git_downstream.tmp_dir.scm.get_ref(str(ref_info3)) == exp3
+
 
 @pytest.mark.parametrize("all_,rev,result3", [(True, False, True), (False, True, None)])
 def test_pull_args(tmp_dir, scm, dvc, git_downstream, exp_stage, all_, rev, result3):
     baseline = scm.get_rev()
 
     results = dvc.experiments.run(exp_stage.addressing, params=["foo=1"])
     exp1 = first(results)
```

### Comparing `dvc-3.1.0/tests/func/experiments/test_remove.py` & `dvc-3.2.0/tests/func/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/test_save.py` & `dvc-3.2.0/tests/func/experiments/test_save.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     dvc.experiments.save(name="exp-1", force=True)
 
     tmp_dir.scm_gen({"new_file": "new_file"}, commit="new baseline")
     dvc.experiments.save(name="exp-2", force=True)
 
     all_exps = dvc.experiments.ls(all_commits=True)
     assert all_exps[baseline][0][0] == "exp-1"
-    assert all_exps["master"][0][0] == "exp-2"
+    assert all_exps["refs/heads/master"][0][0] == "exp-2"
 
 
 def test_exp_save_with_staged_changes(tmp_dir, dvc, scm):
     setup_stage(tmp_dir, dvc, scm)
     tmp_dir.gen({"deleted": "deleted", "modified": "modified"})
     scm.add_commit(["deleted", "modified"], "init")
```

### Comparing `dvc-3.1.0/tests/func/experiments/test_set_params.py` & `dvc-3.2.0/tests/func/experiments/test_set_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/test_show.py` & `dvc-3.2.0/tests/func/experiments/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/test_stash_exp.py` & `dvc-3.2.0/tests/func/experiments/test_stash_exp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/experiments/test_utils.py` & `dvc-3.2.0/tests/func/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/machine/conftest.py` & `dvc-3.2.0/tests/func/machine/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/machine/test_machine_config.py` & `dvc-3.2.0/tests/func/machine/test_machine_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/machine/test_machine_status.py` & `dvc-3.2.0/tests/func/machine/test_machine_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/metrics/test_diff.py` & `dvc-3.2.0/tests/func/metrics/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/metrics/test_show.py` & `dvc-3.2.0/tests/func/metrics/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/params/test_diff.py` & `dvc-3.2.0/tests/func/params/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/params/test_show.py` & `dvc-3.2.0/tests/func/params/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/parsing/__init__.py` & `dvc-3.2.0/tests/func/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/parsing/test_errors.py` & `dvc-3.2.0/tests/func/parsing/test_errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,26 +5,39 @@
 import re
 
 import pytest
 
 from dvc.parsing import ResolveError
 from dvc.parsing.context import Context
 from dvc.parsing.interpolate import embrace
+from dvc.utils.humanize import join
 
 from . import make_entry_definition, make_foreach_def
 
 
 def escape_ansi(line):
     ansi_escape = re.compile(r"(\x9B|\x1B\[)[0-?]*[ -\/]*[@-~]")
     return ansi_escape.sub("", line)
 
 
 # Tests for the interpolated entries
 
 
+@pytest.mark.parametrize("vars_", ["${file}_params.yaml", {"foo": "${foo}"}])
+def test_vars_interpolation_errors(tmp_dir, dvc, vars_):
+    definition = make_entry_definition(tmp_dir, "build", {"vars": [vars_]})
+    with pytest.raises(ResolveError) as exc_info:
+        definition.resolve()
+
+    assert (
+        str(exc_info.value) == "failed to parse 'stages.build.vars' in 'dvc.yaml': "
+        "interpolating is not allowed"
+    )
+
+
 def test_failed_to_interpolate(tmp_dir, dvc):
     context = Context(models={"foo": "bar"})
     definition = make_entry_definition(
         tmp_dir, "build", {"cmd": "echo ${models.foo.}"}, context
     )
 
     with pytest.raises(ResolveError) as exc_info:
@@ -37,14 +50,31 @@
         "            ^\n"
         "ParseException: Expected end of text, found '.'"
         "  (at char 12), (line:1, col:13)"
     )
     assert definition.context == {"models": {"foo": "bar"}}
 
 
+def test_local_vars_params_file_not_exist(tmp_dir, dvc):
+    definition = make_entry_definition(
+        tmp_dir,
+        "build",
+        {"vars": ["not_existing_params.yaml"], "cmd": "echo ${models.foo}"},
+    )
+
+    with pytest.raises(ResolveError) as exc_info:
+        definition.resolve()
+
+    assert (
+        str(exc_info.value) == "failed to parse stage 'build' in 'dvc.yaml': "
+        "'not_existing_params.yaml' does not exist"
+    )
+    assert not definition.context
+
+
 def test_specified_key_does_not_exist(tmp_dir, dvc):
     definition = make_entry_definition(
         tmp_dir,
         "build",
         {"cmd": "echo ${models.foobar}"},
         Context(models={"foo": "foo"}),
     )
@@ -115,14 +145,33 @@
 
     assert (
         str(exc_info.value) == "failed to parse 'stages.build.cmd' in 'dvc.yaml':\n"
         "Cannot interpolate nested iterable in 'list'"
     )
 
 
+def test_partial_vars_doesnot_exist(tmp_dir, dvc):
+    (tmp_dir / "test_params.yaml").dump({"sub1": "sub1", "sub2": "sub2"})
+
+    definition = make_entry_definition(
+        tmp_dir,
+        "build",
+        {"vars": ["test_params.yaml:sub3"], "cmd": "echo ${sub1} ${sub2}"},
+    )
+
+    with pytest.raises(ResolveError) as exc_info:
+        definition.resolve()
+
+    assert (
+        str(exc_info.value) == "failed to parse stage 'build' in 'dvc.yaml': "
+        "could not find 'sub3' in 'test_params.yaml'"
+    )
+    assert not definition.context
+
+
 # Tests foreach generated stages and their error messages
 
 
 def test_foreach_data_syntax_error(tmp_dir, dvc):
     definition = make_foreach_def(tmp_dir, "build", "${syntax.[error}", {})
     with pytest.raises(ResolveError) as exc_info:
         definition.resolve_all()
@@ -231,14 +280,55 @@
         == f"failed to parse '{loc}' in 'dvc.yaml': Could not find '{key}'"
     )
 
     # should have no `item` and `key` even though it failed to resolve.
     assert context == {"foo": "bar"}
 
 
+@pytest.mark.parametrize(
+    "redefine",
+    [
+        {"item": 5},
+        {"key": 5},
+        {"item": 5, "key": 10},
+        {"item": {"epochs": 10}},
+    ],
+)
+@pytest.mark.parametrize("from_file", [True, False])
+def test_item_key_in_generated_stage_vars(tmp_dir, dvc, redefine, from_file):
+    context = Context(foo="bar")
+    vars_ = [redefine]
+    if from_file:
+        (tmp_dir / "test_params.yaml").dump(redefine)
+        vars_ = ["test_params.yaml"]
+
+    definition = make_foreach_def(
+        tmp_dir,
+        "build",
+        {"model1": {"thresh": "10"}, "model2": {"thresh": 5}},
+        {"vars": vars_, "cmd": "${item}"},
+        context,
+    )
+
+    with pytest.raises(ResolveError) as exc_info:
+        definition.resolve_all()
+
+    message = str(exc_info.value)
+    assert (
+        "failed to parse stage 'build@model1' in 'dvc.yaml': "
+        "attempted to modify reserved" in message
+    )
+
+    key_or_keys = "keys" if len(redefine) > 1 else "key"
+    assert f"{key_or_keys} {join(redefine)}" in message
+    if from_file:
+        assert "in 'test_params.yaml'" in message
+    assert context == {"foo": "bar"}
+
+
 def test_foreach_wdir_key_does_not_exist(tmp_dir, dvc):
     definition = make_foreach_def(
         tmp_dir,
         "build",
         "${models}",
         {"wdir": "${ite}", "cmd": "echo ${item}"},
         Context(models=["foo", "bar"]),
```

### Comparing `dvc-3.1.0/tests/func/parsing/test_foreach.py` & `dvc-3.2.0/tests/func/parsing/test_foreach.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Testing happy paths for the foreach."""
+import os
 
 import pytest
 
-from dvc.parsing import DataResolver, ForeachDefinition
+from dvc.parsing import DEFAULT_PARAMS_FILE, DataResolver, ForeachDefinition
 from dvc.parsing.context import Context
 
 
 def test_with_simple_list_data(tmp_dir, dvc):
     """Testing a simple non-nested list as a foreach data"""
     resolver = DataResolver(dvc, tmp_dir.fs_path, {})
 
@@ -265,14 +266,142 @@
         "build@bar": {"wdir": "bar", "cmd": "echo hello"},
     }
 
     assert not resolver.context
     assert not any(item for item in resolver.tracked_vars.values())
 
 
+def test_foreach_with_local_vars(tmp_dir, dvc):
+    resolver = DataResolver(dvc, (tmp_dir / "data").fs_path, {})
+    foreach_data = ["foo", "bar"]
+    data = {
+        "foreach": foreach_data,
+        "do": {
+            "vars": [{"foobar": "foobar"}],
+            "cmd": "echo ${item} ${foobar}",
+        },
+    }
+    definition = ForeachDefinition(resolver, resolver.context, "build", data)
+
+    assert definition.resolve_all() == {
+        # note that the resolver generates `wdir` relative to file's wdir
+        # so, this is just `foo`, not `data/foo`.
+        # figuring out `wdir` is the responsibility of the `load_stage`/`Stage`
+        "build@foo": {"cmd": "echo foo foobar"},
+        "build@bar": {"cmd": "echo bar foobar"},
+    }
+    assert not resolver.context
+    assert not any(item for item in resolver.tracked_vars.values())
+
+
+@pytest.mark.parametrize(
+    "local_import",
+    [
+        "test_params.yaml",
+        "test_params.yaml:train",
+        "test_params.yaml:train,prepare",
+    ],
+)
+def test_foreach_with_imported_vars(tmp_dir, dvc, local_import):
+    (tmp_dir / "params.yaml").dump({"models": {"model1": {"thresh": "foo"}}})
+    (tmp_dir / "test_params.yaml").dump(
+        {"train": {"epochs": 10}, "prepare": {"nums": 25}}
+    )
+    resolver = DataResolver(dvc, tmp_dir.fs_path, {})
+    foreach_data = ["foo", "bar"]
+    data = {
+        "foreach": foreach_data,
+        "do": {"vars": [local_import], "cmd": "echo ${item} ${train.epochs}"},
+    }
+    definition = ForeachDefinition(resolver, resolver.context, "build", data)
+
+    assert definition.resolve_all() == {
+        # note that the resolver generates `wdir` relative to file's wdir
+        # so, this is just `foo`, not `data/foo`.
+        # figuring out `wdir` is the responsibility of the `load_stage`/`Stage`
+        "build@foo": {"cmd": "echo foo 10"},
+        "build@bar": {"cmd": "echo bar 10"},
+    }
+
+    assert resolver.context == {"models": {"model1": {"thresh": "foo"}}}
+    assert resolver.tracked_vars == {
+        "build@foo": {"test_params.yaml": {"train.epochs": 10}},
+        "build@bar": {"test_params.yaml": {"train.epochs": 10}},
+    }
+
+
+@pytest.mark.parametrize("local_import", ["params.yaml", "params.yaml:train,prepare"])
+def test_foreach_with_interpolated_wdir_and_local_vars(tmp_dir, dvc, local_import):
+    (tmp_dir / "params.yaml").dump({"models": {"model1": {"thresh": "foo"}}})
+
+    for i in range(5):
+        build_dir = tmp_dir / ("model-" + str(i))
+        build_dir.mkdir()
+        (build_dir / "params.yaml").dump(
+            {"train": {"epochs": 1 + i}, "prepare": {"nums": 10 * i}},
+        )
+
+    resolver = DataResolver(dvc, tmp_dir.fs_path, {})
+    data = {
+        "foreach": [0, 1, 2, 3, 4],
+        "do": {
+            "wdir": "model-${item}",
+            "vars": [local_import],
+            "cmd": "echo ${item} ${train.epochs} ${prepare.nums}",
+        },
+    }
+    definition = ForeachDefinition(resolver, resolver.context, "build", data)
+
+    assert definition.resolve_all() == {
+        # note that the resolver generates `wdir` relative to file's wdir
+        # so, this is just `foo`, not `data/foo`.
+        # figuring out `wdir` is the responsibility of the `load_stage`/`Stage`
+        "build@0": {"wdir": "model-0", "cmd": "echo 0 1 0"},
+        "build@1": {"wdir": "model-1", "cmd": "echo 1 2 10"},
+        "build@2": {"wdir": "model-2", "cmd": "echo 2 3 20"},
+        "build@3": {"wdir": "model-3", "cmd": "echo 3 4 30"},
+        "build@4": {"wdir": "model-4", "cmd": "echo 4 5 40"},
+    }
+
+    assert resolver.context == {"models": {"model1": {"thresh": "foo"}}}
+    assert resolver.tracked_vars == {
+        "build@0": {
+            os.path.join("model-0", "params.yaml"): {
+                "train.epochs": 1,
+                "prepare.nums": 0,
+            }
+        },
+        "build@1": {
+            os.path.join("model-1", "params.yaml"): {
+                "train.epochs": 2,
+                "prepare.nums": 10,
+            }
+        },
+        "build@2": {
+            os.path.join("model-2", "params.yaml"): {
+                "train.epochs": 3,
+                "prepare.nums": 20,
+            }
+        },
+        "build@3": {
+            os.path.join("model-3", "params.yaml"): {
+                "train.epochs": 4,
+                "prepare.nums": 30,
+            }
+        },
+        "build@4": {
+            os.path.join("model-4", "params.yaml"): {
+                "train.epochs": 5,
+                "prepare.nums": 40,
+            }
+        },
+    }
+    assert resolver.context.imports == {DEFAULT_PARAMS_FILE: None}
+
+
 def test_foreach_do_syntax_is_checked_once(tmp_dir, dvc, mocker):
     do_def = {"cmd": "python script.py --epochs ${item}"}
     data = {"foreach": [0, 1, 2, 3, 4], "do": do_def}
     definition = ForeachDefinition(
         DataResolver(dvc, tmp_dir.fs_path, {}), Context(), "build", data
     )
     mock = mocker.patch("dvc.parsing.check_syntax_errors", return_value=True)
```

### Comparing `dvc-3.1.0/tests/func/parsing/test_interpolated_entry.py` & `dvc-3.2.0/tests/func/parsing/test_resolver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,170 +1,187 @@
 from copy import deepcopy
 
 import pytest
 
-from dvc.dependency import _merge_params
-from dvc.parsing import DEFAULT_PARAMS_FILE, DataResolver
-from dvc.parsing.context import recurse_not_a_node
-from dvc.parsing.interpolate import escape_str
-
-from . import CONTEXT_DATA, RESOLVED_DVC_YAML_DATA, TEMPLATED_DVC_YAML_DATA, USED_VARS
-
-
-def assert_stage_equal(d1, d2):
-    """Keeps the params section in order, and then checks for equality."""
-    for d in [d1, d2]:
-        assert recurse_not_a_node(d)
-        for _, stage_d in d.get("stages", {}).items():
-            params = _merge_params(stage_d.get("params", []))
-            for k in params:
-                params[k] = sorted(params[k])
-            if params:
-                stage_d["params"] = params
-    assert d1 == d2
-
-
-def test_simple(tmp_dir, dvc):
-    (tmp_dir / DEFAULT_PARAMS_FILE).dump(CONTEXT_DATA)
-    resolver = DataResolver(dvc, tmp_dir.fs_path, deepcopy(TEMPLATED_DVC_YAML_DATA))
-    assert_stage_equal(resolver.resolve(), deepcopy(RESOLVED_DVC_YAML_DATA))
-    assert resolver.tracked_vars == {
-        "stage1": {DEFAULT_PARAMS_FILE: USED_VARS["stage1"]},
-        "stage2": {DEFAULT_PARAMS_FILE: USED_VARS["stage2"]},
-    }
-
-
-def test_vars_import(tmp_dir, dvc):
-    """
-    Test that different file can be loaded using `vars`
-    instead of default params.yaml.
-    """
-    (tmp_dir / "params2.yaml").dump(CONTEXT_DATA)
-    d = deepcopy(TEMPLATED_DVC_YAML_DATA)
-    d["vars"] = ["params2.yaml"]
-    resolver = DataResolver(dvc, tmp_dir.fs_path, d)
+from dvc.parsing import DEFAULT_PARAMS_FILE, DataResolver, ResolveError
+from dvc.parsing.context import Context
+from dvc.utils.serialize import dumps_yaml
+
+from . import CONTEXT_DATA, RESOLVED_DVC_YAML_DATA, TEMPLATED_DVC_YAML_DATA
+
+DATA = {"models": {"bar": "bar", "foo": "foo"}}
+
+
+def test_resolver(tmp_dir, dvc):
+    resolver = DataResolver(dvc, tmp_dir.fs_path, TEMPLATED_DVC_YAML_DATA)
+    resolver.context.merge_update(Context(CONTEXT_DATA))
+    assert resolver.resolve() == RESOLVED_DVC_YAML_DATA
+
 
-    resolved_data = deepcopy(RESOLVED_DVC_YAML_DATA)
-    assert_stage_equal(resolver.resolve(), resolved_data)
-    assert resolver.tracked_vars == {
-        "stage1": {"params2.yaml": USED_VARS["stage1"]},
-        "stage2": {"params2.yaml": USED_VARS["stage2"]},
-    }
-
-
-def test_vars_and_params_import(tmp_dir, dvc):
-    """
-    Test that vars and params are both merged together for interpolation,
-    whilst tracking the "used" variables from params.
-    """
-    d = {
-        "vars": [DEFAULT_PARAMS_FILE, {"dict": {"foo": "foobar"}}],
-        "stages": {"stage1": {"cmd": "echo ${dict.foo} ${dict.bar}"}},
-    }
-    (tmp_dir / DEFAULT_PARAMS_FILE).dump({"dict": {"bar": "bar"}})
+def test_default_params_file_not_exist(tmp_dir, dvc):
+    d = {"vars": [DATA["models"]]}
     resolver = DataResolver(dvc, tmp_dir.fs_path, d)
+    assert resolver.context == d["vars"][0]
+
+
+def test_no_params_yaml_and_vars(tmp_dir, dvc):
+    resolver = DataResolver(dvc, tmp_dir.fs_path, {})
+    assert not resolver.context
+
+
+def test_local_vars(tmp_dir, dvc):
+    resolver = DataResolver(
+        dvc, tmp_dir.fs_path, {"vars": [{"foo": "bar", "bar": "foo"}]}
+    )
+    assert resolver.context == {"foo": "bar", "bar": "foo"}
 
-    assert_stage_equal(
-        resolver.resolve(), {"stages": {"stage1": {"cmd": "echo foobar bar"}}}
+
+@pytest.mark.parametrize("vars_", ["${file}_params.yaml", {"foo": "${foo}"}])
+def test_vars_interpolation_errors(tmp_dir, dvc, vars_):
+    with pytest.raises(ResolveError) as exc_info:
+        DataResolver(dvc, tmp_dir.fs_path, {"vars": [vars_, {"bar": "foo"}]})
+    assert (
+        str(exc_info.value)
+        == "failed to parse 'vars' in 'dvc.yaml': interpolating is not allowed"
     )
-    assert resolver.tracked_vars == {
-        "stage1": {DEFAULT_PARAMS_FILE: {"dict.bar": "bar"}}
-    }
-
-
-def test_vars_relpath_overwrite(tmp_dir, dvc):
-    iterable = {"bar": "bar", "foo": "foo"}
-    (tmp_dir / "params.yaml").dump(iterable)
-    d = {
-        "vars": ["params.yaml"],
-        "stages": {
-            "build": {
-                "wdir": "data",
-                "cmd": "echo ${bar}",
-                "vars": ["../params.yaml"],
-            }
-        },
-    }
+
+
+@pytest.mark.parametrize("vars_", [{}, {"vars": []}, {"vars": [DEFAULT_PARAMS_FILE]}])
+def test_default_params_file(tmp_dir, dvc, vars_):
+    (tmp_dir / DEFAULT_PARAMS_FILE).dump(DATA)
+    resolver = DataResolver(dvc, tmp_dir.fs_path, vars_)
+    assert resolver.context == DATA
+
+
+def test_load_vars_from_file(tmp_dir, dvc):
+    (tmp_dir / DEFAULT_PARAMS_FILE).dump(DATA)
+
+    datasets = {"datasets": ["foo", "bar"]}
+    (tmp_dir / "params.json").dump(datasets)
+    d = {"vars": [DEFAULT_PARAMS_FILE, "params.json"]}
     resolver = DataResolver(dvc, tmp_dir.fs_path, d)
-    resolver.resolve()
-    assert resolver.context.imports == {"params.yaml": None}
+
+    expected = deepcopy(DATA)
+    expected.update(datasets)
+    assert resolver.context == expected
+
+
+def test_load_vars_with_relpath(tmp_dir, scm, dvc):
+    tmp_dir.scm_gen(DEFAULT_PARAMS_FILE, dumps_yaml(DATA), commit="add params")
+
+    revisions = ["HEAD", "workspace"]
+    for rev in dvc.brancher(revs=["HEAD"]):
+        assert rev == revisions.pop()
+        d = {
+            "vars": [f"../{DEFAULT_PARAMS_FILE}"],
+        }
+        resolver = DataResolver(dvc, "subdir", d)
+        assert resolver.context == deepcopy(DATA)
+
+
+def test_partial_vars_doesnot_exist(tmp_dir, dvc):
+    (tmp_dir / "test_params.yaml").dump({"sub1": "sub1"})
+
+    with pytest.raises(ResolveError) as exc_info:
+        DataResolver(dvc, tmp_dir.fs_path, {"vars": ["test_params.yaml:sub2"]})
+
+    assert (
+        str(exc_info.value) == "failed to parse 'vars' in 'dvc.yaml': "
+        "could not find 'sub2' in 'test_params.yaml'"
+    )
+
+
+def test_global_overwrite_error_on_imports(tmp_dir, dvc):
+    (tmp_dir / DEFAULT_PARAMS_FILE).dump(DATA)
+    (tmp_dir / "params.json").dump(DATA)
+
+    d = {"vars": [DEFAULT_PARAMS_FILE, "params.json"]}
+    with pytest.raises(ResolveError) as exc_info:
+        DataResolver(dvc, tmp_dir.fs_path, d)
+
+    assert (
+        str(exc_info.value) == "failed to parse 'vars' in 'dvc.yaml':\n"
+        "cannot redefine 'models.bar' from 'params.json' "
+        "as it already exists in 'params.yaml'"
+    )
+
+
+def test_global_overwrite_vars(tmp_dir, dvc):
+    (tmp_dir / DEFAULT_PARAMS_FILE).dump(DATA)
+    d = {"vars": [DATA]}
+
+    with pytest.raises(ResolveError) as exc_info:
+        DataResolver(dvc, tmp_dir.fs_path, d)
+
+    assert (
+        str(exc_info.value) == "failed to parse 'vars' in 'dvc.yaml':\n"
+        "cannot redefine 'models.bar' from 'vars[0]' "
+        "as it already exists in 'params.yaml'"
+    )
+
+
+def test_local_declared_vars_overwrite(tmp_dir, dvc):
+    (tmp_dir / DEFAULT_PARAMS_FILE).dump(DATA)
+
+    d = {"vars": [DATA["models"], DATA["models"]]}
+    with pytest.raises(ResolveError) as exc_info:
+        DataResolver(dvc, tmp_dir.fs_path, d)
+
+    assert (
+        str(exc_info.value) == "failed to parse 'vars' in 'dvc.yaml':\n"
+        "cannot redefine 'bar' from 'vars[1]' "
+        "as it already exists in 'vars[0]'"
+    )
 
 
+def test_specified_params_file_not_exist(tmp_dir, dvc):
+    d = {"vars": ["not_existing_params.yaml"]}
+    with pytest.raises(ResolveError) as exc_info:
+        DataResolver(dvc, tmp_dir.fs_path, d)
+
+    assert (
+        str(exc_info.value) == "failed to parse 'vars' in 'dvc.yaml': "
+        "'not_existing_params.yaml' does not exist"
+    )
+
+
+@pytest.mark.parametrize("local", [True, False])
 @pytest.mark.parametrize(
     "vars_",
     [
-        ["test_params.yaml:bar", "test_params.yaml:foo"],
-        ["test_params.yaml:foo,bar"],
-        ["test_params.yaml"],
-        ["test_params.yaml", "test_params.yaml"],
+        ["test_params.yaml", "test_params.yaml:sub1"],
+        ["test_params.yaml:sub1", "test_params.yaml"],
+        ["test_params.yaml:sub1", "test_params.yaml:sub1,sub2"],
     ],
 )
-def test_vars_load_partial(tmp_dir, dvc, vars_):
-    iterable = {"bar": "bar", "foo": "foo"}
-    (tmp_dir / "test_params.yaml").dump(iterable)
-    d = {"vars": vars_, "stages": {"build": {"cmd": "echo ${bar}"}}}
-    resolver = DataResolver(dvc, tmp_dir.fs_path, d)
-    resolver.resolve()
+def test_vars_already_loaded_message(tmp_dir, dvc, local, vars_):
+    d = {"stages": {"build": {"cmd": "echo ${sub1} ${sub2}"}}}
+    (tmp_dir / "test_params.yaml").dump({"sub1": "sub1", "sub2": "sub2"})
+    if not local:
+        d["vars"] = vars_
+    else:
+        d["stages"]["build"]["vars"] = vars_
+
+    with pytest.raises(ResolveError) as exc_info:  # noqa: PT012
+        resolver = DataResolver(dvc, tmp_dir.fs_path, d)
+        resolver.resolve()
+    assert "partially" in str(exc_info.value)
 
 
 @pytest.mark.parametrize(
-    "bool_config, list_config",
-    [(None, None), ("store_true", "nargs"), ("boolean_optional", "append")],
+    "vars_, loc", [(DATA, "build.vars[0]"), ("params.json", "params.json")]
 )
-def test_cmd_dict(tmp_dir, dvc, bool_config, list_config):
-    with dvc.config.edit() as conf:
-        if bool_config:
-            conf["parsing"]["bool"] = bool_config
-        if list_config:
-            conf["parsing"]["list"] = list_config
-
-    string = "spaced string"
-    mixed_quote_string = "quote\"'d"
-    data = {
-        "dict": {
-            "foo": "foo",
-            "bar": 2,
-            "string": string,
-            "mixed_quote_string": mixed_quote_string,
-            "bool": True,
-            "bool-false": False,
-            "list": [1, 2, "foo", mixed_quote_string],
-            "nested": {"foo": "foo"},
-        }
-    }
-    (tmp_dir / DEFAULT_PARAMS_FILE).dump(data)
-    resolver = DataResolver(
-        dvc,
-        tmp_dir.fs_path,
-        {"stages": {"stage1": {"cmd": "python script.py ${dict}"}}},
-    )
+def test_local_overwrite_error(tmp_dir, dvc, vars_, loc):
+    (tmp_dir / DEFAULT_PARAMS_FILE).dump(DATA)
+    (tmp_dir / "params.json").dump(DATA)
 
-    if bool_config is None or bool_config == "store_true":
-        bool_resolved = " --bool"
-    else:
-        bool_resolved = " --bool --no-bool-false"
+    d = {"stages": {"build": {"cmd": "echo ${models.foo}", "vars": [vars_]}}}
 
-    if list_config is None or list_config == "nargs":
-        list_resolved = f" --list 1 2 foo {escape_str(mixed_quote_string)}"
-    else:
-        list_resolved = " --list 1 --list 2 --list foo"
-        list_resolved += f" --list {escape_str(mixed_quote_string)}"
+    resolver = DataResolver(dvc, tmp_dir.fs_path, d)
+    with pytest.raises(ResolveError) as exc_info:
+        resolver.resolve()
 
-    assert_stage_equal(
-        resolver.resolve(),
-        {
-            "stages": {
-                "stage1": {
-                    "cmd": (
-                        "python script.py"
-                        " --foo foo --bar 2"
-                        f" --string {escape_str(string)}"
-                        " --mixed_quote_string"
-                        f" {escape_str(mixed_quote_string)}"
-                        f"{bool_resolved}"
-                        f"{list_resolved}"
-                        " --nested.foo foo"
-                    )
-                }
-            }
-        },
+    assert (
+        str(exc_info.value) == "failed to parse stage 'build' in 'dvc.yaml':\n"
+        f"cannot redefine 'models.bar' from '{loc}' "
+        "as it already exists in 'params.yaml'"
     )
```

### Comparing `dvc-3.1.0/tests/func/plots/test_diff.py` & `dvc-3.2.0/tests/func/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/plots/test_modify.py` & `dvc-3.2.0/tests/func/plots/test_modify.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/plots/test_show.py` & `dvc-3.2.0/tests/func/plots/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/repro/test_repro.py` & `dvc-3.2.0/tests/func/repro/test_repro.py`

 * *Files 1% similar despite different names*

```diff
@@ -1269,7 +1269,16 @@
         deps=["foo", "copy.py"],
         cmd="python copy.py foo file1",
         name="copy-foo-file1",
     )
 
     stages = dvc.reproduce(stage.addressing)
     assert len(stages) == 1
+
+
+def test_repro_rm_recursive(tmp_dir, dvc):
+    # check that dir output recursively removes files in the dir
+    tmp_dir.gen({"dir": {"foo": "foo"}})
+    dvc.stage.add(name="dir", cmd="mkdir dir", outs=["dir"])
+    dvc.reproduce()
+    assert (tmp_dir / "dir").exists()
+    assert not (tmp_dir / "dir" / "foo").exists()
```

### Comparing `dvc-3.1.0/tests/func/repro/test_repro_allow_missing.py` & `dvc-3.2.0/tests/func/repro/test_repro_allow_missing.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/repro/test_repro_pull.py` & `dvc-3.2.0/tests/func/repro/test_repro_pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_add.py` & `dvc-3.2.0/tests/func/test_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -780,14 +780,15 @@
           type: mytype
           labels:
           - label1
           - label2
           remote: testremote
           md5: acbd18db4cc2f85cedef654fccc4a4d8
           size: 3
+          hash: md5
         meta: some metadata
     """
     )
 
 
 # NOTE: unless long paths are enabled on Windows, PATH_MAX and NAME_MAX
 # are the same 260 chars, which makes the test unnecessarily complex
@@ -971,14 +972,15 @@
 def test_add_updates_to_cloud_versioning_dir(tmp_dir, dvc):
     data_dvc = tmp_dir / "data.dvc"
     data_dvc.dump(
         {
             "outs": [
                 {
                     "path": "data",
+                    "hash": "md5",
                     "files": [
                         {
                             "size": 3,
                             "version_id": "WYRG4BglP7pD.gEoJP6a4AqOhl.FRA.h",
                             "etag": "acbd18db4cc2f85cedef654fccc4a4d8",
                             "md5": "acbd18db4cc2f85cedef654fccc4a4d8",
                             "relpath": "bar",
@@ -1003,14 +1005,15 @@
 
     dvc.add("data")
 
     assert (tmp_dir / "data.dvc").parse() == {
         "outs": [
             {
                 "path": "data",
+                "hash": "md5",
                 "files": [
                     {
                         "size": 4,
                         "md5": "224e2539f52203eb33728acd228b4432",
                         "relpath": "bar",
                     },
                     {
```

### Comparing `dvc-3.1.0/tests/func/test_analytics.py` & `dvc-3.2.0/tests/func/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_check_ignore.py` & `dvc-3.2.0/tests/func/test_check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_checkout.py` & `dvc-3.2.0/tests/func/test_checkout.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,31 +80,27 @@
     ret = main(["checkout", "--force"])
     assert ret == 0
     assert not os.path.exists("file_in_a_branch")
 
 
 class TestCheckoutCleanWorkingDir:
     def test(self, mocker, tmp_dir, dvc):
-        mock_prompt = mocker.patch("dvc.prompt.confirm", return_value=True)
         (stage,) = tmp_dir.dvc_gen("data", {"foo": "foo"})
 
         # change working directory
         (tmp_dir / "data").gen("not_cached.txt", "not_cached")
-        assert main(["checkout", stage.relpath]) == 0
-        mock_prompt.assert_called()
+        assert main(["checkout", stage.relpath, "--force"]) == 0
         assert not (tmp_dir / "data" / "not_cached.txt").exists()
 
     def test_force(self, mocker, tmp_dir, dvc):
-        mock_prompt = mocker.patch("dvc.prompt.confirm", return_value=False)
         (stage,) = tmp_dir.dvc_gen("data", {"foo": "foo"})
 
         # change working directory
         (tmp_dir / "data").gen("not_cached.txt", "not_cached")
         assert main(["checkout", stage.relpath]) != 0
-        mock_prompt.assert_called()
         assert (tmp_dir / "data" / "not_cached.txt").exists()
 
 
 def test_checkout_selective_remove(tmp_dir, dvc):
     # Use copy to test for changes in the inodes
     dvc.cache.local.cache_types = ["copy"]
     tmp_dir.dvc_gen({"data": {"foo": "foo", "bar": "bar"}})
```

### Comparing `dvc-3.1.0/tests/func/test_cli.py` & `dvc-3.2.0/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_commit.py` & `dvc-3.2.0/tests/func/test_commit.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,13 +312,16 @@
         {
             "outs": [
                 {"path": "foo", "md5": "acbd18db4cc2f85cedef654fccc4a4d8", "size": 3},
             ]
         }
     )
     legacy_content = (tmp_dir / "foo.dvc").read_text()
+    assert "hash: md5" not in legacy_content
 
-    dvc.commit("foo.dvc")
+    dvc.commit("foo.dvc", force=True)
     assert (tmp_dir / "foo.dvc").read_text() == legacy_content
+
+    tmp_dir.gen("foo", "modified")
     dvc.commit("foo.dvc", force=True)
     content = (tmp_dir / "foo.dvc").read_text()
     assert "hash: md5" in content
```

### Comparing `dvc-3.1.0/tests/func/test_config.py` & `dvc-3.2.0/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_data_cloud.py` & `dvc-3.2.0/tests/func/test_data_cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_data_status.py` & `dvc-3.2.0/tests/func/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_diff.py` & `dvc-3.2.0/tests/func/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_dvcfile.py` & `dvc-3.2.0/tests/func/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_external_repo.py` & `dvc-3.2.0/tests/func/test_external_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_fs.py` & `dvc-3.2.0/tests/func/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_gc.py` & `dvc-3.2.0/tests/func/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_get.py` & `dvc-3.2.0/tests/func/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_get_url.py` & `dvc-3.2.0/tests/func/test_get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_ignore.py` & `dvc-3.2.0/tests/func/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_import.py` & `dvc-3.2.0/tests/func/test_import.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_import_url.py` & `dvc-3.2.0/tests/func/test_import_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_init.py` & `dvc-3.2.0/tests/func/test_init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_install.py` & `dvc-3.2.0/tests/func/test_install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_lock.py` & `dvc-3.2.0/tests/func/test_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_lockfile.py` & `dvc-3.2.0/tests/func/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_ls.py` & `dvc-3.2.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_merge_driver.py` & `dvc-3.2.0/tests/func/test_merge_driver.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_move.py` & `dvc-3.2.0/tests/func/test_move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_odb.py` & `dvc-3.2.0/tests/func/test_odb.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_remote.py` & `dvc-3.2.0/tests/func/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_remove.py` & `dvc-3.2.0/tests/func/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_repo.py` & `dvc-3.2.0/tests/func/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_repo_index.py` & `dvc-3.2.0/tests/func/test_repo_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_run.py` & `dvc-3.2.0/tests/func/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_run_cache.py` & `dvc-3.2.0/tests/func/test_run_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_scm.py` & `dvc-3.2.0/tests/func/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_scm_context.py` & `dvc-3.2.0/tests/func/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_stage.py` & `dvc-3.2.0/tests/func/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_stage_load.py` & `dvc-3.2.0/tests/func/test_stage_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_state.py` & `dvc-3.2.0/tests/func/test_state.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_status.py` & `dvc-3.2.0/tests/func/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_unprotect.py` & `dvc-3.2.0/tests/func/test_unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_update.py` & `dvc-3.2.0/tests/func/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_used_objs.py` & `dvc-3.2.0/tests/func/test_used_objs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_utils.py` & `dvc-3.2.0/tests/func/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_version.py` & `dvc-3.2.0/tests/func/test_version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/test_virtual_directory.py` & `dvc-3.2.0/tests/func/test_virtual_directory.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/utils/test_hydra.py` & `dvc-3.2.0/tests/func/utils/test_hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/func/utils/test_strict_yaml.py` & `dvc-3.2.0/tests/func/utils/test_strict_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/integration/plots/conftest.py` & `dvc-3.2.0/tests/integration/plots/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/integration/plots/test_plots.py` & `dvc-3.2.0/tests/integration/plots/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/integration/plots/test_repo_plots_api.py` & `dvc-3.2.0/tests/integration/plots/test_repo_plots_api.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/integration/test_studio_live_experiments.py` & `dvc-3.2.0/tests/integration/test_studio_live_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/remotes/git_server.py` & `dvc-3.2.0/tests/remotes/git_server.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/remotes/user.key` & `dvc-3.2.0/tests/remotes/user.key`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/remotes_env.sample` & `dvc-3.2.0/tests/remotes_env.sample`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/scripts.py` & `dvc-3.2.0/tests/scripts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/cli/test_main.py` & `dvc-3.2.0/tests/unit/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/ls/test_ls.py` & `dvc-3.2.0/tests/unit/command/ls/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/ls/test_ls_colors.py` & `dvc-3.2.0/tests/unit/command/ls/test_ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_add.py` & `dvc-3.2.0/tests/unit/command/test_add.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         remote=None,
         to_remote=False,
         remote_jobs=None,
         force=False,
     )
 
 
-def test_add_to_remote(mocker):
+def test_add_to_remote(mocker, dvc):
     cli_args = parse_args(
         [
             "add",
             "s3://bucket/foo",
             "--to-remote",
             "--out",
             "bar",
@@ -59,15 +59,15 @@
         remote="remote",
         to_remote=True,
         remote_jobs=None,
         force=False,
     )
 
 
-def test_add_to_remote_invalid_combinations(mocker, caplog):
+def test_add_to_remote_invalid_combinations(mocker, caplog, dvc):
     cli_args = parse_args(["add", "s3://bucket/foo", "s3://bucket/bar", "--to-remote"])
     assert cli_args.func == CmdAdd
 
     cmd = cli_args.func(cli_args)
     with caplog.at_level(logging.ERROR, logger="dvc"):
         assert cmd.run() == 1
         expected_msg = "multiple targets can't be used with --to-remote"
@@ -79,15 +79,15 @@
         cmd = cli_args.func(cli_args)
         with caplog.at_level(logging.ERROR, logger="dvc"):
             assert cmd.run() == 1
             expected_msg = f"{option} can't be used without --to-remote"
             assert expected_msg in caplog.text
 
 
-def test_add_to_cache_invalid_combinations(mocker, caplog):
+def test_add_to_cache_invalid_combinations(mocker, caplog, dvc):
     cli_args = parse_args(["add", "s3://bucket/foo", "s3://bucket/bar", "-o", "foo"])
     assert cli_args.func == CmdAdd
 
     cmd = cli_args.func(cli_args)
     with caplog.at_level(logging.ERROR, logger="dvc"):
         assert cmd.run() == 1
         expected_msg = "multiple targets can't be used with --out"
```

### Comparing `dvc-3.1.0/tests/unit/command/test_cache.py` & `dvc-3.2.0/tests/unit/command/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_checkout.py` & `dvc-3.2.0/tests/unit/command/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_compat_flag.py` & `dvc-3.2.0/tests/unit/command/test_compat_flag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_config.py` & `dvc-3.2.0/tests/unit/command/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_dag.py` & `dvc-3.2.0/tests/unit/command/test_dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_data_status.py` & `dvc-3.2.0/tests/unit/command/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_data_sync.py` & `dvc-3.2.0/tests/unit/command/test_data_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dvc.cli import parse_args
 from dvc.commands.data_sync import CmdDataFetch, CmdDataPull, CmdDataPush
 
 
-def test_fetch(mocker):
+def test_fetch(mocker, dvc):
     cli_args = parse_args(
         [
             "fetch",
             "target1",
             "target2",
             "--jobs",
             "2",
@@ -36,15 +36,15 @@
         all_commits=True,
         with_deps=True,
         recursive=True,
         run_cache=True,
     )
 
 
-def test_pull(mocker):
+def test_pull(mocker, dvc):
     cli_args = parse_args(
         [
             "pull",
             "target1",
             "target2",
             "--jobs",
             "2",
@@ -80,15 +80,15 @@
         recursive=True,
         run_cache=True,
         glob=True,
         allow_missing=True,
     )
 
 
-def test_push(mocker):
+def test_push(mocker, dvc):
     cli_args = parse_args(
         [
             "push",
             "target1",
             "target2",
             "--jobs",
             "2",
```

### Comparing `dvc-3.1.0/tests/unit/command/test_diff.py` & `dvc-3.2.0/tests/unit/command/test_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ],
     ids=["str", "dict"],
 )
 def test_digest(checksum, expected):
     assert expected == _digest(checksum)
 
 
-def test_default(mocker, capsys):
+def test_default(mocker, capsys, dvc):
     args = parse_args(["diff"])
     cmd = args.func(args)
     diff = {
         "added": [{"path": "file", "hash": "00000000"}],
         "deleted": [],
         "modified": [],
         "renamed": [
@@ -47,15 +47,15 @@
         "Renamed:\n"
         "    data{sep}file_old -> data{sep}file_new\n"
         "\n"
         "files summary: 1 added, 1 renamed"
     ).format(sep=os.path.sep) in capsys.readouterr()[0]
 
 
-def test_show_hash(mocker, capsys):
+def test_show_hash(mocker, capsys, dvc):
     args = parse_args(["diff", "--show-hash"])
     cmd = args.func(args)
     diff = {
         "added": [],
         "deleted": [
             {"path": os.path.join("data", ""), "hash": "XXXXXXXX.dir"},
             {"path": os.path.join("data", "foo"), "hash": "11111111"},
@@ -97,15 +97,15 @@
         "    CCCCCCCC..DDDDDDDD  file1\n"
         "    AAAAAAAA..BBBBBBBB  file2\n"
         "\n"
         "files summary: 2 deleted, 1 renamed, 2 modified"
     ) in out
 
 
-def test_show_json(mocker, capsys):
+def test_show_json(mocker, capsys, dvc):
     args = parse_args(["diff", "--json"])
     cmd = args.func(args)
     diff = {
         "added": [
             {"path": "file2", "hash": "22222222"},
             {"path": "file1", "hash": "11111111"},
         ],
@@ -119,15 +119,15 @@
     out, _ = capsys.readouterr()
     assert '"added": [{"path": "file1"}, {"path": "file2"}]' in out
     assert '"deleted": []' in out
     assert '"modified": []' in out
     assert '"not in cache": []' in out
 
 
-def test_show_json_and_hash(mocker, capsys):
+def test_show_json_and_hash(mocker, capsys, dvc):
     args = parse_args(["diff", "--json", "--show-hash"])
     cmd = args.func(args)
 
     diff = {
         "added": [
             # py35: maintain a consistent key order for tests purposes
             collections.OrderedDict([("path", "file2"), ("hash", "22222222")]),
@@ -156,15 +156,15 @@
     assert (
         '"renamed": [{"path": {"old": "file_old", '
         '"new": "file_new"}, "hash": "11111111"}]' in out
     )
     assert '"not in cache": []' in out
 
 
-def test_show_json_hide_missing(mocker, capsys):
+def test_show_json_hide_missing(mocker, capsys, dvc):
     args = parse_args(["diff", "--json", "--hide-missing"])
     cmd = args.func(args)
     diff = {
         "added": [
             {"path": "file2", "hash": "22222222"},
             {"path": "file1", "hash": "11111111"},
         ],
@@ -186,15 +186,15 @@
     assert '"deleted": []' in out
     assert '"renamed": [{"path": {"old": "file_old", "new": "file_new"}' in out
     assert '"modified": []' in out
     assert '"not in cache": []' not in out
 
 
 @pytest.mark.parametrize("show_hash", [None, True, False])
-def test_diff_show_markdown_and_hash(mocker, show_hash):
+def test_diff_show_markdown_and_hash(mocker, show_hash, dvc):
     options = ["diff", "--md"] + (["--show-hash"] if show_hash else [])
     args = parse_args(options)
     cmd = args.func(args)
 
     diff = {}
     show_hash = show_hash if show_hash else False
     mock_show_markdown = mocker.patch("dvc.commands.diff._show_markdown")
@@ -217,15 +217,15 @@
     "show, expected",
     (
         ([], ""),
         (["--json"], "{}"),
         (["--md"], "| Status   | Path   |\n|----------|--------|"),
     ),
 )
-def test_no_changes(mocker, capsys, opts, show, expected):
+def test_no_changes(mocker, capsys, opts, show, expected, dvc):
     args = parse_args(["diff", *opts, *show])
     cmd = args.func(args)
     mocker.patch("dvc.repo.Repo.diff", return_value={})
 
     assert cmd.run() == 0
     out, _ = capsys.readouterr()
     assert expected == out.strip()
@@ -326,15 +326,15 @@
         "| deleted  | data{sep}bar             |\n"
         "| renamed  | file_old -> file_new |\n"
         "| modified | file                 |\n"
         "\n"
     ).format(sep=os.path.sep)
 
 
-def test_hide_missing(mocker, capsys):
+def test_hide_missing(mocker, capsys, dvc):
     args = parse_args(["diff", "--hide-missing"])
     cmd = args.func(args)
     diff = {
         "added": [{"path": "file", "hash": "00000000"}],
         "deleted": [],
         "modified": [],
         "renamed": [
```

### Comparing `dvc-3.1.0/tests/unit/command/test_experiments.py` & `dvc-3.2.0/tests/unit/command/test_experiments.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     assert cmd.run() == 0
 
     m.assert_called_once_with(
         cmd.repo, a_rev="HEAD~10", b_rev="HEAD~1", all=True, param_deps=True
     )
 
 
-def test_experiments_diff_revs(mocker, capsys):
+def test_experiments_diff_revs(mocker, capsys, dvc, scm):
     mocker.patch(
         "dvc.repo.experiments.diff.diff",
         return_value={
             "params": {"params.yaml": {"foo": {"diff": 1, "old": 1, "new": 2}}},
             "metrics": {"metrics.yaml": {"foo": {"diff": 1, "old": 1, "new": 2}}},
         },
     )
@@ -190,19 +190,19 @@
     "args,expected",
     [
         ([], "main:\n\tsha-a [exp-a]\n"),
         (["--name-only"], "exp-a\n"),
         (["--sha-only"], "sha-a\n"),
     ],
 )
-def test_experiments_list_format(mocker, capsys, args, expected):
+def test_experiments_list_format(mocker, capsys, args, expected, dvc, scm):
     mocker.patch(
         "dvc.repo.experiments.ls.ls",
         return_value={
-            "main": [
+            "refs/heads/main": [
                 ("exp-a", "sha-a"),
             ]
         },
     )
     raw_args = ["experiments", "list", *args]
     cli_args = parse_args(raw_args)
 
@@ -210,15 +210,15 @@
 
     capsys.readouterr()
     assert cmd.run() == 0
     cap = capsys.readouterr()
     assert cap.out == expected
 
 
-def test_experiments_list_remote(mocker, capsys):
+def test_experiments_list_remote(mocker, capsys, dvc, scm):
     mocker.patch(
         "dvc.repo.experiments.ls.ls",
         return_value={
             "main": [
                 ("exp-a", None),
             ]
         },
@@ -290,20 +290,15 @@
             "experiments",
             "push",
             "origin",
         ]
     )
     cmd = cli_args.func(cli_args)
 
-    with pytest.raises(InvalidArgumentError) as exp_info:
-        cmd.run()
-    assert (
-        str(exp_info.value) == "Either provide an `experiment` argument"
-        ", or use the `--rev` or `--all-commits` flag."
-    )
+    assert cmd.run() == 0
 
 
 def test_experiments_pull(dvc, scm, mocker):
     cli_args = parse_args(
         [
             "experiments",
             "pull",
@@ -347,20 +342,15 @@
             "experiments",
             "pull",
             "origin",
         ]
     )
     cmd = cli_args.func(cli_args)
 
-    with pytest.raises(InvalidArgumentError) as exp_info:
-        cmd.run()
-    assert (
-        str(exp_info.value) == "Either provide an `experiment` argument"
-        ", or use the `--rev` or `--all-commits` flag."
-    )
+    assert cmd.run() == 0
 
 
 def test_experiments_remove_flag(dvc, scm, mocker, capsys, caplog):
     cli_args = parse_args(
         [
             "experiments",
             "remove",
```

### Comparing `dvc-3.1.0/tests/unit/command/test_gc.py` & `dvc-3.2.0/tests/unit/command/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_get.py` & `dvc-3.2.0/tests/unit/command/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_git_hook.py` & `dvc-3.2.0/tests/unit/command/test_git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_imp.py` & `dvc-3.2.0/tests/unit/command/test_imp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dvc.cli import parse_args
 from dvc.commands.imp import CmdImport
 
 
-def test_import(mocker):
+def test_import(mocker, dvc):
     cli_args = parse_args(
         [
             "import",
             "repo_url",
             "src",
             "--out",
             "out",
@@ -30,15 +30,15 @@
         rev="version",
         no_exec=False,
         no_download=False,
         jobs=3,
     )
 
 
-def test_import_no_exec(mocker):
+def test_import_no_exec(mocker, dvc):
     cli_args = parse_args(
         [
             "import",
             "repo_url",
             "src",
             "--out",
             "out",
@@ -60,15 +60,15 @@
         rev="version",
         no_exec=True,
         no_download=False,
         jobs=None,
     )
 
 
-def test_import_no_download(mocker):
+def test_import_no_download(mocker, dvc):
     cli_args = parse_args(
         [
             "import",
             "repo_url",
             "src",
             "--out",
             "out",
```

### Comparing `dvc-3.1.0/tests/unit/command/test_imp_url.py` & `dvc-3.2.0/tests/unit/command/test_imp_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 
 from dvc.cli import parse_args
 from dvc.commands.imp_url import CmdImportUrl
 from dvc.exceptions import DvcException
 
 
-def test_import_url(mocker):
+def test_import_url(mocker, dvc):
     cli_args = parse_args(
         [
             "import-url",
             "src",
             "out",
             "--jobs",
             "4",
@@ -33,15 +33,15 @@
         to_remote=False,
         jobs=4,
         force=False,
         version_aware=False,
     )
 
 
-def test_failed_import_url(mocker, caplog):
+def test_failed_import_url(mocker, caplog, dvc):
     cli_args = parse_args(["import-url", "http://somesite.com/file_name"])
     assert cli_args.func == CmdImportUrl
 
     cmd = cli_args.func(cli_args)
     mocker.patch.object(cmd.repo, "imp_url", side_effect=DvcException("error"))
     with caplog.at_level(logging.ERROR, logger="dvc"):
         assert cmd.run() == 1
@@ -56,15 +56,15 @@
 @pytest.mark.parametrize(
     "flag,expected",
     [
         ("--no-exec", {"no_exec": True, "no_download": False}),
         ("--no-download", {"no_download": True, "no_exec": False}),
     ],
 )
-def test_import_url_no_exec_download_flags(mocker, flag, expected):
+def test_import_url_no_exec_download_flags(mocker, flag, expected, dvc):
     cli_args = parse_args(
         [
             "import-url",
             flag,
             "src",
             "out",
         ]
@@ -83,15 +83,15 @@
         jobs=None,
         force=False,
         version_aware=False,
         **expected,
     )
 
 
-def test_import_url_to_remote(mocker):
+def test_import_url_to_remote(mocker, dvc):
     cli_args = parse_args(
         [
             "import-url",
             "s3://bucket/foo",
             "bar",
             "--to-remote",
             "--remote",
```

### Comparing `dvc-3.1.0/tests/unit/command/test_ls_url.py` & `dvc-3.2.0/tests/unit/command/test_ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_machine.py` & `dvc-3.2.0/tests/unit/command/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_metrics.py` & `dvc-3.2.0/tests/unit/command/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_params.py` & `dvc-3.2.0/tests/unit/command/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_plots.py` & `dvc-3.2.0/tests/unit/command/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_queue.py` & `dvc-3.2.0/tests/unit/command/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_repro.py` & `dvc-3.2.0/tests/unit/command/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_stage.py` & `dvc-3.2.0/tests/unit/command/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_status.py` & `dvc-3.2.0/tests/unit/command/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/command/test_update.py` & `dvc-3.2.0/tests/unit/command/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/data/db/test_local.py` & `dvc-3.2.0/tests/unit/data/db/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/dependency/test_params.py` & `dvc-3.2.0/tests/unit/dependency/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/fs/test_azure.py` & `dvc-3.2.0/tests/unit/fs/test_azure.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/fs/test_data.py` & `dvc-3.2.0/tests/unit/fs/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/fs/test_dvc.py` & `dvc-3.2.0/tests/unit/fs/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/fs/test_dvc_info.py` & `dvc-3.2.0/tests/unit/fs/test_dvc_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/fs/test_fs.py` & `dvc-3.2.0/tests/unit/fs/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/fs/test_path.py` & `dvc-3.2.0/tests/unit/fs/test_path.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/fs/test_s3.py` & `dvc-3.2.0/tests/unit/fs/test_s3.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/fs/test_tree.py` & `dvc-3.2.0/tests/unit/fs/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/machine/test_machine.py` & `dvc-3.2.0/tests/unit/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/output/test_load.py` & `dvc-3.2.0/tests/unit/output/test_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/output/test_local.py` & `dvc-3.2.0/tests/unit/output/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/output/test_output.py` & `dvc-3.2.0/tests/unit/output/test_output.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/remote/test_oss.py` & `dvc-3.2.0/tests/unit/remote/test_oss.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/remote/test_remote.py` & `dvc-3.2.0/tests/unit/remote/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/remote/test_webdav.py` & `dvc-3.2.0/tests/unit/remote/test_webdav.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/remote/test_webhdfs.py` & `dvc-3.2.0/tests/unit/remote/test_webhdfs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/render/test_convert.py` & `dvc-3.2.0/tests/unit/render/test_convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/render/test_image_converter.py` & `dvc-3.2.0/tests/unit/render/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/render/test_match.py` & `dvc-3.2.0/tests/unit/render/test_match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/render/test_vega_converter.py` & `dvc-3.2.0/tests/unit/render/test_vega_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/experiments/conftest.py` & `dvc-3.2.0/tests/unit/repo/experiments/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/experiments/queue/test_celery.py` & `dvc-3.2.0/tests/unit/repo/experiments/queue/test_celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/experiments/queue/test_remove.py` & `dvc-3.2.0/tests/unit/repo/experiments/queue/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/experiments/test_executor_status.py` & `dvc-3.2.0/tests/unit/repo/experiments/test_executor_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/experiments/test_remove.py` & `dvc-3.2.0/tests/unit/repo/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/experiments/test_utils.py` & `dvc-3.2.0/tests/unit/repo/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/plots/test_diff.py` & `dvc-3.2.0/tests/unit/repo/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/test_open_repo.py` & `dvc-3.2.0/tests/unit/repo/test_open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/test_repo.py` & `dvc-3.2.0/tests/unit/repo/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/test_reproduce.py` & `dvc-3.2.0/tests/unit/repo/test_reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/repo/test_scm_context.py` & `dvc-3.2.0/tests/unit/repo/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/scm/test_scm.py` & `dvc-3.2.0/tests/unit/scm/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/stage/test_cache.py` & `dvc-3.2.0/tests/unit/stage/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/stage/test_loader_pipeline_file.py` & `dvc-3.2.0/tests/unit/stage/test_loader_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/stage/test_run.py` & `dvc-3.2.0/tests/unit/stage/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/stage/test_serialize_pipeline_file.py` & `dvc-3.2.0/tests/unit/stage/test_serialize_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/stage/test_serialize_pipeline_lock.py` & `dvc-3.2.0/tests/unit/stage/test_serialize_pipeline_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/stage/test_stage.py` & `dvc-3.2.0/tests/unit/stage/test_stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/stage/test_utils.py` & `dvc-3.2.0/tests/unit/stage/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_analytics.py` & `dvc-3.2.0/tests/unit/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_collect.py` & `dvc-3.2.0/tests/unit/test_collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_compare.py` & `dvc-3.2.0/tests/unit/test_compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_config.py` & `dvc-3.2.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_context.py` & `dvc-3.2.0/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_daemon.py` & `dvc-3.2.0/tests/unit/test_daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_dvcfile.py` & `dvc-3.2.0/tests/unit/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_ignore.py` & `dvc-3.2.0/tests/unit/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_imports.py` & `dvc-3.2.0/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_info.py` & `dvc-3.2.0/tests/unit/test_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_interpolate.py` & `dvc-3.2.0/tests/unit/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_lockfile.py` & `dvc-3.2.0/tests/unit/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_logger.py` & `dvc-3.2.0/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_metrics.py` & `dvc-3.2.0/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_params.py` & `dvc-3.2.0/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_pathspec_math.py` & `dvc-3.2.0/tests/unit/test_pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_progress.py` & `dvc-3.2.0/tests/unit/test_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_rwlock.py` & `dvc-3.2.0/tests/unit/test_rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_tabular_data.py` & `dvc-3.2.0/tests/unit/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/test_updater.py` & `dvc-3.2.0/tests/unit/test_updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/ui/test_console.py` & `dvc-3.2.0/tests/unit/ui/test_console.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/ui/test_pager.py` & `dvc-3.2.0/tests/unit/ui/test_pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/ui/test_table.py` & `dvc-3.2.0/tests/unit/ui/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/serialize/test_python.py` & `dvc-3.2.0/tests/unit/utils/serialize/test_python.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/serialize/test_toml.py` & `dvc-3.2.0/tests/unit/utils/serialize/test_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/serialize/test_yaml.py` & `dvc-3.2.0/tests/unit/utils/serialize/test_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/test_cli_parse.py` & `dvc-3.2.0/tests/unit/utils/test_cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/test_collections.py` & `dvc-3.2.0/tests/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/test_executors.py` & `dvc-3.2.0/tests/unit/utils/test_executors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/test_fs.py` & `dvc-3.2.0/tests/unit/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/test_humanize.py` & `dvc-3.2.0/tests/unit/utils/test_humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/test_studio.py` & `dvc-3.2.0/tests/unit/utils/test_studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/unit/utils/test_utils.py` & `dvc-3.2.0/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/utils/__init__.py` & `dvc-3.2.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.1.0/tests/utils/asserts.py` & `dvc-3.2.0/tests/utils/asserts.py`

 * *Files identical despite different names*

