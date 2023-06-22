# Comparing `tmp/routeros-check-0.9.1.tar.gz` & `tmp/routeros-check-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routeros-check-0.9.1.tar", last modified: Wed Jun  7 10:54:09 2023, max compression
+gzip compressed data, was "routeros-check-0.9.2.tar", last modified: Thu Jun 22 13:12:31 2023, max compression
```

## Comparing `routeros-check-0.9.1.tar` & `routeros-check-0.9.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.801489 routeros-check-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.793490 routeros-check-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.793490 routeros-check-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/icinga.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-07 10:53:53.000000 routeros-check-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 10:53:53.000000 routeros-check-0.9.1/CHANGELOG.md.license
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-07 10:53:53.000000 routeros-check-0.9.1/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-07 10:53:53.000000 routeros-check-0.9.1/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-06-07 10:53:53.000000 routeros-check-0.9.1/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-07 10:53:53.000000 routeros-check-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-07 10:54:09.801489 routeros-check-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-07 10:53:53.000000 routeros-check-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 10:53:53.000000 routeros-check-0.9.1/README.md.license
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-07 10:53:53.000000 routeros-check-0.9.1/check_routeros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/config/
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-06-07 10:53:53.000000 routeros-check-0.9.1/config/check_routeros.icinga2.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/cli.md.license
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-07 10:53:53.000000 routeros-check-0.9.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-07 10:53:53.000000 routeros-check-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-07 10:53:53.000000 routeros-check-0.9.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/routeros_check/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check/_scm_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.801489 routeros-check-0.9.1/routeros_check/check/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/interface_gre.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/interface_vrrp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/routing_bgp_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/routing_ospf_neighbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_fan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_ntp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_psu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_uptime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/tool_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/exeption.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/routeros_check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:54:09.801489 routeros-check-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 10:53:53.000000 routeros-check-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.801489 routeros-check-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:53:53.000000 routeros-check-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-07 10:53:53.000000 routeros-check-0.9.1/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-07 10:53:53.000000 routeros-check-0.9.1/tests/helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 10:53:53.000000 routeros-check-0.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.094795 routeros-check-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-22 13:12:09.000000 routeros-check-0.9.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.082794 routeros-check-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.086794 routeros-check-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-22 13:12:09.000000 routeros-check-0.9.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-22 13:12:09.000000 routeros-check-0.9.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-22 13:12:09.000000 routeros-check-0.9.2/.github/workflows/icinga.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-22 13:12:09.000000 routeros-check-0.9.2/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-22 13:12:09.000000 routeros-check-0.9.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-22 13:12:09.000000 routeros-check-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-22 13:12:09.000000 routeros-check-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-22 13:12:09.000000 routeros-check-0.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 13:12:09.000000 routeros-check-0.9.2/CHANGELOG.md.license
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-22 13:12:09.000000 routeros-check-0.9.2/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.086794 routeros-check-0.9.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-22 13:12:09.000000 routeros-check-0.9.2/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-06-22 13:12:09.000000 routeros-check-0.9.2/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-22 13:12:09.000000 routeros-check-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-22 13:12:31.094795 routeros-check-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-22 13:12:09.000000 routeros-check-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 13:12:09.000000 routeros-check-0.9.2/README.md.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-22 13:12:09.000000 routeros-check-0.9.2/check_routeros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.086794 routeros-check-0.9.2/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-06-22 13:12:09.000000 routeros-check-0.9.2/config/check_routeros.icinga2.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.086794 routeros-check-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-22 13:12:09.000000 routeros-check-0.9.2/docs/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 13:12:09.000000 routeros-check-0.9.2/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 13:12:09.000000 routeros-check-0.9.2/docs/cli.md.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-22 13:12:09.000000 routeros-check-0.9.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 13:12:09.000000 routeros-check-0.9.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-22 13:12:09.000000 routeros-check-0.9.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-22 13:12:09.000000 routeros-check-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-22 13:12:09.000000 routeros-check-0.9.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.086794 routeros-check-0.9.2/routeros_check/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 13:12:30.000000 routeros-check-0.9.2/routeros_check/_scm_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.090795 routeros-check-0.9.2/routeros_check/check/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/interface_gre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/interface_vrrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/routing_bgp_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/routing_ospf_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_fan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_ntp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_psu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/system_uptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/check/tool_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/exeption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-22 13:12:09.000000 routeros-check-0.9.2/routeros_check/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.090795 routeros-check-0.9.2/routeros_check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-22 13:12:31.000000 routeros-check-0.9.2/routeros_check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-22 13:12:31.000000 routeros-check-0.9.2/routeros_check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:12:31.000000 routeros-check-0.9.2/routeros_check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 13:12:31.000000 routeros-check-0.9.2/routeros_check.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 13:12:31.000000 routeros-check-0.9.2/routeros_check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 13:12:31.000000 routeros-check-0.9.2/routeros_check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:12:31.094795 routeros-check-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-22 13:12:09.000000 routeros-check-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:31.094795 routeros-check-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:09.000000 routeros-check-0.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-22 13:12:09.000000 routeros-check-0.9.2/tests/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-22 13:12:09.000000 routeros-check-0.9.2/tests/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-22 13:12:09.000000 routeros-check-0.9.2/tox.ini
```

### Comparing `routeros-check-0.9.1/.github/workflows/ci.yml` & `routeros-check-0.9.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/.github/workflows/docs.yml` & `routeros-check-0.9.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/.github/workflows/icinga.yml` & `routeros-check-0.9.2/.github/workflows/icinga.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/.github/workflows/pages.yml` & `routeros-check-0.9.2/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/.github/workflows/pypi.yml` & `routeros-check-0.9.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/.gitignore` & `routeros-check-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/.pre-commit-config.yaml` & `routeros-check-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/CHANGELOG.md` & `routeros-check-0.9.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.9.2 - 2023-06-22
+------------------
+
+- Fix checks
+  - system.ntp.client - Fix issue with offset on RouterOS 7.x
+
 0.9.1 - 2023-06-07
 ------------------
 
 - Fix checks
   - interface - Fix l2mtu issue on CHR devices
 - Update icinga2 example config
```

### Comparing `routeros-check-0.9.1/LICENSE.md` & `routeros-check-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/LICENSES/CC0-1.0.txt` & `routeros-check-0.9.2/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/LICENSES/GPL-3.0-or-later.txt` & `routeros-check-0.9.2/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/PKG-INFO` & `routeros-check-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeros-check
-Version: 0.9.1
+Version: 0.9.2
 Summary: Monitoring plugin for MikroTik devices for Icinga-Nagios-... 
 Author: DinoTools
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `routeros-check-0.9.1/README.md` & `routeros-check-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/config/check_routeros.icinga2.conf` & `routeros-check-0.9.2/config/check_routeros.icinga2.conf`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/docs/LICENSE.md` & `routeros-check-0.9.2/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/docs/index.md` & `routeros-check-0.9.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/mkdocs.yml` & `routeros-check-0.9.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/pyproject.toml` & `routeros-check-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/interface.py` & `routeros-check-0.9.2/routeros_check/check/interface.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/interface_gre.py` & `routeros-check-0.9.2/routeros_check/check/interface_gre.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/interface_vrrp.py` & `routeros-check-0.9.2/routeros_check/check/interface_vrrp.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/routing_bgp_peer.py` & `routeros-check-0.9.2/routeros_check/check/routing_bgp_peer.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/routing_ospf_neighbor.py` & `routeros-check-0.9.2/routeros_check/check/routing_ospf_neighbor.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_clock.py` & `routeros-check-0.9.2/routeros_check/check/system_clock.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_cpu.py` & `routeros-check-0.9.2/routeros_check/check/system_cpu.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_fan.py` & `routeros-check-0.9.2/routeros_check/check/system_fan.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_license.py` & `routeros-check-0.9.2/routeros_check/check/system_license.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_memory.py` & `routeros-check-0.9.2/routeros_check/check/system_memory.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_ntp_client.py` & `routeros-check-0.9.2/routeros_check/check/system_ntp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                                 "Unable to get address of server (last-update-from)"
                             )
                         )
         else:
             self._routeros_metric_values += [
                 {"name": "freq-drift", "type": float},
                 {"name": "synced-stratum", "dst": "stratum", "type": int},
-                {"name": "system-offset", "dst": "offset", "type": float, "uom": "s"},
+                {"name": "system-offset", "dst": "offset", "type": lambda v: float(v) / 1000, "uom": "s"},
             ]
             self._check.add(
                 PerfdataScalarContext(
                     name="freq-drift",
                 ),
                 nagiosplugin.ScalarContext(
                     name="offset",
```

### Comparing `routeros-check-0.9.1/routeros_check/check/system_power.py` & `routeros-check-0.9.2/routeros_check/check/system_power.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_psu.py` & `routeros-check-0.9.2/routeros_check/check/system_psu.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_temperature.py` & `routeros-check-0.9.2/routeros_check/check/system_temperature.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_update.py` & `routeros-check-0.9.2/routeros_check/check/system_update.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/system_uptime.py` & `routeros-check-0.9.2/routeros_check/check/system_uptime.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/check/tool_ping.py` & `routeros-check-0.9.2/routeros_check/check/tool_ping.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/cli.py` & `routeros-check-0.9.2/routeros_check/cli.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/context.py` & `routeros-check-0.9.2/routeros_check/context.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/helper.py` & `routeros-check-0.9.2/routeros_check/helper.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check/resource.py` & `routeros-check-0.9.2/routeros_check/resource.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/routeros_check.egg-info/PKG-INFO` & `routeros-check-0.9.2/routeros_check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeros-check
-Version: 0.9.1
+Version: 0.9.2
 Summary: Monitoring plugin for MikroTik devices for Icinga-Nagios-... 
 Author: DinoTools
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `routeros-check-0.9.1/routeros_check.egg-info/SOURCES.txt` & `routeros-check-0.9.2/routeros_check.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/tests/base_test.py` & `routeros-check-0.9.2/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.1/tests/helpers_test.py` & `routeros-check-0.9.2/tests/helpers_test.py`

 * *Files identical despite different names*

