# Comparing `tmp/pybritive-1.4.0rc3.tar.gz` & `tmp/pybritive-1.4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybritive-1.4.0rc3.tar", last modified: Tue May 16 13:10:55 2023, max compression
+gzip compressed data, was "pybritive-1.4.0rc4.tar", last modified: Thu Jun 22 18:08:59 2023, max compression
```

## Comparing `pybritive-1.4.0rc3.tar` & `pybritive-1.4.0rc4.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.249538 pybritive-1.4.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-16 13:10:55.249538 pybritive-1.4.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 13:10:55.253538 pybritive-1.4.0rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.233538 pybritive-1.4.0rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.233538 pybritive-1.4.0rc3/src/pybritive/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43430 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/britive_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.237538 pybritive-1.4.0rc3/src/pybritive/choices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/cli_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.237538 pybritive-1.4.0rc3/src/pybritive/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.237538 pybritive-1.4.0rc3/src/pybritive/completers/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/api_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/bash_gte_42.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/powershell_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.241538 pybritive-1.4.0rc3/src/pybritive/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/api_method_argument_dectorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/aws_credential_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/build_britive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/cloud_credential_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/profile_argument_dectorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.249538 pybritive-1.4.0rc3/src/pybritive/options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/aws_console_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/aws_credentials_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/blocktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/britive_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/checked_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/configure_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/configure_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/configure_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/configure_tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/federation_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/force_renew.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/gcloud_key_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/justification.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/maxpolltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/passphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/silent.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_push_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_username.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.237538 pybritive-1.4.0rc3/src/pybritive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.249538 pybritive-1.4.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0100_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0200_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0300_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0400_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0450_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0500_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0600_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0700_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0800_checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0850_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0900_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_1000_logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.355534 pybritive-1.4.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-22 18:08:59.355534 pybritive-1.4.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-22 18:08:59.355534 pybritive-1.4.0rc4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.335532 pybritive-1.4.0rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.339532 pybritive-1.4.0rc4/src/pybritive/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/britive_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.339532 pybritive-1.4.0rc4/src/pybritive/choices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/ssh_push_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/cli_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.343533 pybritive-1.4.0rc4/src/pybritive/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.343533 pybritive-1.4.0rc4/src/pybritive/completers/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/api_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/bash_gte_42.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/powershell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.347533 pybritive-1.4.0rc4/src/pybritive/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/api_method_argument_dectorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/aws_credential_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/build_britive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/cloud_credential_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/profile_argument_dectorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.351534 pybritive-1.4.0rc4/src/pybritive/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/aws_console_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/aws_credentials_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/blocktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/britive_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/checked_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/configure_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/configure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/configure_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/configure_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/federation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/force_renew.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/gcloud_key_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/justification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/maxpolltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/passphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/silent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_push_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.339532 pybritive-1.4.0rc4/src/pybritive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.355534 pybritive-1.4.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0100_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0200_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0300_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0400_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0450_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0500_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0600_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0700_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0800_checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0850_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0900_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_1000_logout.py
```

### Comparing `pybritive-1.4.0rc3/LICENSE` & `pybritive-1.4.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/PKG-INFO` & `pybritive-1.4.0rc4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.4.0rc3
+Version: 1.4.0rc4
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybritive-1.4.0rc3/README.md` & `pybritive-1.4.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/setup.cfg` & `pybritive-1.4.0rc4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybritive
-version = 1.4.0rc3
+version = 1.4.0rc4
 author = Britive Inc.
 author_email = support@britive.com
 description = A pure Python CLI for Britive
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.britive.com
 classifiers = 
@@ -15,22 +15,22 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	click
-	requests
+	requests>=2.31.0
 	PyYAML
 	merge_args
 	tabulate
 	toml
-	cryptography~=39.0.1
+	cryptography>=41.0.0
 	python-dateutil
-	britive>=2.19.0
+	britive>=2.20.0
 	jmespath
 	pyjwt
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
```

### Comparing `pybritive-1.4.0rc3/src/pybritive/britive_cli.py` & `pybritive-1.4.0rc4/src/pybritive/britive_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from tabulate import tabulate
 import yaml
 from .helpers import cloud_credential_printer as printer
 from .helpers.cache import Cache
 from britive import exceptions
 from pathlib import Path
 from datetime import datetime
+from datetime import timezone
+from datetime import timedelta
 import os
 import sys
 import jmespath
 
 
 default_table_format = 'fancy_grid'
 debug_enabled = os.getenv('PYBRITIVE_DEBUG')
@@ -835,21 +837,25 @@
         aws_region = None  # will drop to using standard aws boto3/cli region provider chain
         if len(helper) > 1:
             aws_profile = helper[1]
         if len(helper) > 2:
             aws_region = helper[2]
 
         if push_public_key:
-            self._ssh_aws_generate_key(
+            details = self._ssh_generate_key(
+                username=username,
+                hostname=hostname,
+                key_source=key_source
+            )
+            self._ssh_aws_push_key(
                 instance_id=instance_id,
                 aws_profile=aws_profile,
                 aws_region=aws_region,
                 username=username,
-                hostname=hostname,
-                key_source=key_source
+                key_pair=details['key_pair']
             )
 
         commands = [
             'aws',
             'ssm',
             'start-session',
             f'--parameters portNumber={port_number}',
@@ -860,40 +866,20 @@
         if aws_profile:
             commands.append(f'--profile {aws_profile}')
         if aws_region:
             commands.append(f'--region {aws_region}')
 
         self.print(' '.join(commands), ignore_silent=True)
 
-    def _ssh_aws_generate_key(self, instance_id, aws_profile, aws_region, username, hostname, key_source):
+    @staticmethod
+    def _ssh_generate_key_pair():
         # doing imports here as these packages are not a requirement to use pybritive in general
-
-        # cryptography is already a hard requirement so we know it will eixst
         from cryptography.hazmat.primitives.asymmetric import rsa
         from cryptography.hazmat.primitives import serialization
 
-        # these 3 ship with python3.x
-        import glob
-        import time
-        import subprocess
-
-        # this is the one that may not be available so be careful
-        try:
-            import boto3
-        except ImportError:
-            message = 'boto3 package is required. Please ensure the package is installed.'
-            raise click.ClickException(message)
-
-        # we know we will be pushing the key to the instance so establish the
-        # boto3 clients which are required to perform those actions
-        session = boto3.Session(profile_name=aws_profile, region_name=aws_region)
-        eic = session.client('ec2-instance-connect')
-        ec2 = session.client('ec2')
-
-        # now let's create the ephemeral private and public key pair
         private_key = rsa.generate_private_key(
             public_exponent=65537,
             key_size=2048
         )
 
         pem_private_key = private_key.private_bytes(
             encoding=serialization.Encoding.PEM,
@@ -902,18 +888,32 @@
         )
 
         pem_public_key = private_key.public_key().public_bytes(
             encoding=serialization.Encoding.OpenSSH,
             format=serialization.PublicFormat.OpenSSH
         )
 
+        return {
+            'private': pem_private_key,
+            'public': pem_public_key
+        }
+
+    def _ssh_generate_key(self, username, hostname, key_source):
+        # doing imports here as these packages are not a requirement to use pybritive in general
+
+        # these 3 ship with python3.x
+        import glob
+        import time
+        import subprocess
+
+        key_pair = self._ssh_generate_key_pair()
+
         # let's do the right thing and clean up old ephemeral keys
         ssh_dir = Path(self.config.path).parent.absolute() / 'ssh'
         ssh_dir.mkdir(exist_ok=True, parents=True)  # create the directory if it doesn't exist already
-        pem_file = None
         if key_source == 'ssh-agent':
             # cleanup any old ssh keys that were randomly generated
             now = int(time.time())
             for key in glob.glob(f'{str(ssh_dir)}/random-*'):
                 file = key.split('/')[-1].split('.')[0]
                 expiration = int(file.split('-')[2])
                 if expiration < now:
@@ -928,33 +928,52 @@
             raise ValueError(f'invalid --key-source value {key_source}')
 
         # we only need to persist the private key locally
         # as the public key is just pushed to the ec2 instance
         # as a string in the ec2 instance connect api call (no file
         # reference)
         with open(str(pem_file), 'w') as f:
-            f.write(pem_private_key.decode())
+            f.write(key_pair['private'].decode())
         os.chmod(pem_file, 0o400)
 
+        # and if we are using ssh-agent we need to add the private key via ssh-add
+        if key_source == 'ssh-agent':
+            subprocess.run(['ssh-add', str(pem_file), '-t', '60', '-q'])
+
+        return {
+            'private_key_filename': pem_file,
+            'key_pair': key_pair
+        }
+
+    @staticmethod
+    def _ssh_aws_push_key(aws_profile, aws_region, instance_id, username, key_pair):
+        try:
+            import boto3
+        except ImportError:
+            message = 'boto3 package is required. Please ensure the package is installed.'
+            raise click.ClickException(message)
+
+        # we know we will be pushing the key to the instance so establish the
+        # boto3 clients which are required to perform those actions
+        session = boto3.Session(profile_name=aws_profile, region_name=aws_region)
+        eic = session.client('ec2-instance-connect')
+        ec2 = session.client('ec2')
+
         # now push the key
         az = ec2.describe_instances(
             InstanceIds=[instance_id]
         )['Reservations'][0]['Instances'][0]['Placement']['AvailabilityZone']
 
         eic.send_ssh_public_key(
             InstanceId=instance_id,
             InstanceOSUser=username,
-            SSHPublicKey=pem_public_key.decode(),
+            SSHPublicKey=key_pair['public'].decode(),
             AvailabilityZone=az
         )
 
-        # and if we are using ssh-agent we need to add the private key via ssh-add
-        if key_source == 'ssh-agent':
-            subprocess.run(['ssh-add', str(pem_file), '-t', '60', '-q'])
-
     def ssh_aws_openssh_config(self, push_public_key, key_source):
         lines = ['Match host i-*,mi-*']
         if push_public_key:
             commands = [
                 '\tProxyCommand eval $(pybritive ssh aws ssm-proxy --hostname %h',
                 '--username %r --port-number %p --push-public-key',
                 f'--key-source {key_source})'
@@ -1051,7 +1070,144 @@
 
         # then we can try to split it into parts and clear that version of the
         # profile name as well - it will not hurt anything to try to clear
         # both versions
         parts = self._split_profile_into_parts(profile)
         Cache().clear_awscredentialprocess(profile_name=f"{parts['app']}/{parts['env']}/{parts['profile']}")
 
+    def ssh_gcp_identity_aware_proxy(self, username, hostname, push_public_key, port_number, key_source):
+        self.silent = True
+        helper = hostname.split('.')
+        instance_name = helper[1]
+        project = helper[2]
+
+        import subprocess
+        import shlex
+
+        command = f'gcloud compute instances list --format json --project {project}'
+        instances = json.loads(subprocess.check_output(shlex.split(command)).decode('utf-8'))
+
+        zone = None
+        metadata = None
+        for instance in instances:
+            if instance['name'] == instance_name:
+                zone = instance['zone'].split('/')[-1]
+                metadata = instance.get('metadata')
+
+        if not zone:
+            raise click.BadParameter(f'no zone found for instance {instance_name} in project {project}')
+
+        if push_public_key:
+            details = self._ssh_generate_key(
+                username=username,
+                hostname=hostname,
+                key_source=key_source
+            )
+
+            if push_public_key == 'os-login':  # this is pretty straightforward
+                public_key = details["key_pair"]["public"].decode('utf-8')
+                command = f'gcloud compute os-login ssh-keys add --key="{public_key}" ' \
+                          f'--project={project} --ttl=1m --no-user-output-enabled --quiet'
+                subprocess.check_output(shlex.split(command))
+            if push_public_key == 'instance-metadata':  # this is a bit more involved
+                now = datetime.now(timezone.utc).replace(microsecond=0)
+
+                if metadata:
+                    existing_keys_str = None
+                    for item in metadata.get('items', []):
+                        if item['key'] == 'ssh-keys':
+                            existing_keys_str = item['value']
+                            break
+                    future_keys = []
+                    if existing_keys_str:
+                        existing_keys = existing_keys_str.split('\n')
+
+                        for key in existing_keys:
+                            should_carry_forward = True
+
+                            if 'google-ssh' in key:  # non google-ssh keys should always carry forward
+                                key_details = json.loads(key.split('google-ssh')[1].strip())
+                                expires = key_details['expireOn']
+                                if now > datetime.fromisoformat(expires):
+                                    should_carry_forward = False
+                            if should_carry_forward:
+                                future_keys.append(key)
+
+                    command = 'gcloud auth list --filter=status:ACTIVE --format="value(account)" --quiet'
+                    active_gcloud_user = subprocess.check_output(shlex.split(command)).decode('utf-8').strip()
+
+                    # format is 2023-05-16T20:15:22+0000
+                    google_ssh_data = {
+                        'userName': active_gcloud_user,
+                        'expireOn': (now + timedelta(seconds=60)).strftime('%Y-%m-%dT%H:%M:%S+0000')
+                    }
+                    google_ssh_data = json.dumps(google_ssh_data, separators=(',', ':'))  # separators IMPORTANT
+                    public_key = details["key_pair"]["public"].decode('utf-8')
+                    new_key = f'{username}:{public_key} google-ssh {google_ssh_data}'
+                    future_keys.append(new_key)
+
+                    ssh_dir = Path(self.config.path).parent.absolute() / 'ssh'
+                    ssh_dir.mkdir(exist_ok=True, parents=True)  # create the directory if it doesn't exist already
+                    key_file = ssh_dir / uuid.uuid4().hex
+                    with open(str(key_file), 'w') as f:
+                        f.write('\n'.join(future_keys))
+
+                    commands = [
+                        'gcloud',
+                        'compute',
+                        'instances',
+                        'add-metadata',
+                        instance_name,
+                        '--project',
+                        project,
+                        '--metadata-from-file',
+                        f'ssh-keys={str(key_file)}',
+                        '--zone',
+                        zone,
+                        '--verbosity=error',
+                        '--no-user-output-enabled',
+                        '--quiet'
+                    ]
+                    subprocess.run(commands)
+                    key_file.unlink(missing_ok=True)
+
+        commands = [
+            'gcloud',
+            'compute',
+            'start-iap-tunnel',
+            instance_name,
+            port_number,
+            '--listen-on-stdin',
+            f'--project={project}',
+            f'--zone={zone}',
+            '--verbosity=error'
+        ]
+
+        self.print(' '.join(commands), ignore_silent=True)
+
+    def ssh_gcp_openssh_config(self, push_public_key, key_source):
+        lines = ['Match host gcp.*']
+        if push_public_key:
+            commands = [
+                '\tProxyCommand eval $(pybritive gcp identity-aware-proxy --hostname %h',
+                f'--username %r --port-number %p --push-public-key {push_public_key}',
+                f'--key-source {key_source})'
+            ]
+            lines.append(' '.join(commands))
+
+            if key_source == 'static':
+                ssh_dir = Path(self.config.path).parent.absolute() / 'ssh'
+                lines.append(f'\tIdentityFile {str(ssh_dir)}/%h.%r.pem')
+        else:
+            line = '\tProxyCommand eval $(pybritive ssh gcp identity-aware-proxy --hostname %h --username %r ' \
+                   '--port-number %p)'
+            lines.append(line)
+
+        self.print('Add the below Match directive to your SSH config file, after all Host directives.')
+        self.print('This file is generally located at ~/.ssh/config.')
+        self.print('Additional SSH config parameters can be added as required.')
+        self.print('The below directive is the minimum required configuration.')
+        self.print('')
+        self.print('')
+        self.print('\n'.join(lines))
+
+
```

### Comparing `pybritive-1.4.0rc3/src/pybritive/choices/mode.py` & `pybritive-1.4.0rc4/src/pybritive/choices/mode.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/choices/output_format.py` & `pybritive-1.4.0rc4/src/pybritive/choices/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/cli_interface.py` & `pybritive-1.4.0rc4/src/pybritive/cli_interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 def safe_cli():
     debug = os.getenv('PYBRITIVE_DEBUG')
     try:
         if not debug:
             sys.tracebacklimit = 0
         cli()
     except Exception as e:
+        part1 = '401 - e0000 - aws access token for subject'
+        part2 = 'not authorized by cognito'
+        if part1 in str(e).lower() and part2 in str(e).lower():
+            click.echo('You have logged out of Britive via the browser. Please run `pybritive logout` to clear your '
+                       'token and then re-run your command.')
+            return
         if debug:
             raise e
         else:
             raise e from None
 
 
 # this is the "main" app - it really does nothing but print the overview/help section
```

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/api.py` & `pybritive-1.4.0rc4/src/pybritive/commands/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/aws.py` & `pybritive-1.4.0rc4/src/pybritive/commands/aws.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/cache.py` & `pybritive-1.4.0rc4/src/pybritive/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/checkin.py` & `pybritive-1.4.0rc4/src/pybritive/commands/checkin.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/checkout.py` & `pybritive-1.4.0rc4/src/pybritive/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/clear.py` & `pybritive-1.4.0rc4/src/pybritive/commands/clear.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/configure.py` & `pybritive-1.4.0rc4/src/pybritive/commands/configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/login.py` & `pybritive-1.4.0rc4/src/pybritive/commands/login.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/ls.py` & `pybritive-1.4.0rc4/src/pybritive/commands/ls.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/request.py` & `pybritive-1.4.0rc4/src/pybritive/commands/request.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/secret.py` & `pybritive-1.4.0rc4/src/pybritive/commands/secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/commands/ssh.py` & `pybritive-1.4.0rc4/src/pybritive/commands/ssh.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,23 @@
     """Facilitates connecting, via SSH, to private AWS EC2 instances via Session Manager and EC2 Instance Connect.
 
     This command generally should be called from within an SSH config as opposed to being directly invoked.
     """
     pass
 
 
+@ssh.group()
+def gcp():
+    """Facilitates connecting, via SSH, to private GCP Compute Instances via Identity Aware Proxy and OS Login/SSH Metadata.
+
+    This command generally should be called from within an SSH config as opposed to being directly invoked.
+    """
+    pass
+
+
 @aws.command()
 @build_britive
 @britive_options(names='ssh_push_public_key,ssh_key_source')
 def config(ctx, push_public_key, key_source):
     """Prints the required Match directive to add to an OpenSSH config file (normally located at ~/.ssh/config.)"""
 
     ctx.obj.britive.ssh_aws_openssh_config(
@@ -32,14 +41,47 @@
 
 @aws.command()
 @build_britive
 @britive_options(names='ssh_username,ssh_hostname,ssh_push_public_key,ssh_port,ssh_key_source')
 def ssm_proxy(ctx, username, hostname, push_public_key, port_number, key_source):
     """Outputs AWS CLI command to be consumed by ProxyCommand to establish an OpenSSH proxy tunnel."""
 
+    if push_public_key == 'default':
+        push_public_key = True
+
     ctx.obj.britive.ssh_aws_ssm_proxy(
         username=username,
         hostname=hostname,
         push_public_key=push_public_key,
         port_number=port_number,
         key_source=key_source
     )
+
+
+@gcp.command()
+@build_britive
+@britive_options(names='ssh_push_public_key,ssh_key_source')
+def config(ctx, push_public_key, key_source):
+    """Prints the required Match directive to add to an OpenSSH config file (normally located at ~/.ssh/config.)"""
+
+    ctx.obj.britive.ssh_gcp_openssh_config(
+        push_public_key=push_public_key,
+        key_source=key_source
+    )
+
+
+@gcp.command()
+@build_britive
+@britive_options(names='ssh_username,ssh_hostname,ssh_push_public_key,ssh_port,ssh_key_source')
+def identity_aware_proxy(ctx, username, hostname, push_public_key, port_number, key_source):
+    """Outputs gcloud CLI command to be consumed by ProxyCommand to establish an OpenSSH proxy tunnel."""
+
+    if push_public_key == 'default':
+        push_public_key = 'os-login'
+
+    ctx.obj.britive.ssh_gcp_identity_aware_proxy(
+        username=username,
+        hostname=hostname,
+        push_public_key=push_public_key,
+        port_number=port_number,
+        key_source=key_source
+    )
```

### Comparing `pybritive-1.4.0rc3/src/pybritive/completers/api.py` & `pybritive-1.4.0rc4/src/pybritive/completers/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/completers/api_command.py` & `pybritive-1.4.0rc4/src/pybritive/completers/api_command.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/completers/bash_gte_42.py` & `pybritive-1.4.0rc4/src/pybritive/completers/bash_gte_42.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/completers/powershell_completion.py` & `pybritive-1.4.0rc4/src/pybritive/completers/powershell_completion.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/completers/profile.py` & `pybritive-1.4.0rc4/src/pybritive/completers/profile.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/helpers/aws_credential_process.py` & `pybritive-1.4.0rc4/src/pybritive/helpers/aws_credential_process.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/helpers/build_britive.py` & `pybritive-1.4.0rc4/src/pybritive/helpers/build_britive.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/helpers/cache.py` & `pybritive-1.4.0rc4/src/pybritive/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/helpers/cloud_credential_printer.py` & `pybritive-1.4.0rc4/src/pybritive/helpers/cloud_credential_printer.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/helpers/config.py` & `pybritive-1.4.0rc4/src/pybritive/helpers/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     'output_format',
     'credential_backend',
     'auto-refresh-profile-cache'
 ]
 
 tenant_fields = [
     'name',
-    'output_format'
+    'output_format',
+    'sso_idp'
 ]
 
 aws_fields = [
     'default_checkout_mode'
 ]
```

### Comparing `pybritive-1.4.0rc3/src/pybritive/helpers/credentials.py` & `pybritive-1.4.0rc4/src/pybritive/helpers/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,19 @@
             os.environ['REQUESTS_CA_BUNDLE'] = ""
             # disable the warning message
             import urllib3
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     def perform_interactive_login(self):
         self.cli.print(f'Performing interactive login against tenant {self.tenant}.')
-        url = f'{self.base_url}/login?token={self.auth_token}'
+        sso_idp = self.cli.config.get_tenant().get('sso_idp')
+        if sso_idp:
+            url = f'{self.base_url}/sso?idp={sso_idp}&token={self.auth_token}'
+        else:
+            url = f'{self.base_url}/login?token={self.auth_token}'
 
         # establish a requests session which will be used in retrieve_tokens()
         self._setup_requests_session()
 
         try:
             webbrowser.get()
             webbrowser.open(url)
```

### Comparing `pybritive-1.4.0rc3/src/pybritive/helpers/encryption.py` & `pybritive-1.4.0rc4/src/pybritive/helpers/encryption.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/helpers/split.py` & `pybritive-1.4.0rc4/src/pybritive/helpers/split.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/options/britive_options.py` & `pybritive-1.4.0rc4/src/pybritive/options/britive_options.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/options/browser.py` & `pybritive-1.4.0rc4/src/pybritive/options/browser.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/options/mode.py` & `pybritive-1.4.0rc4/src/pybritive/options/mode.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/options/output_format.py` & `pybritive-1.4.0rc4/src/pybritive/options/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive/options/version.py` & `pybritive-1.4.0rc4/src/pybritive/options/version.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/src/pybritive.egg-info/PKG-INFO` & `pybritive-1.4.0rc4/src/pybritive.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.4.0rc3
+Version: 1.4.0rc4
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybritive-1.4.0rc3/src/pybritive.egg-info/SOURCES.txt` & `pybritive-1.4.0rc4/src/pybritive.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/pybritive.egg-info/top_level.txt
 src/pybritive/choices/__init__.py
 src/pybritive/choices/backend.py
 src/pybritive/choices/browser.py
 src/pybritive/choices/mode.py
 src/pybritive/choices/output_format.py
 src/pybritive/choices/ssh_key_source.py
+src/pybritive/choices/ssh_push_public_key.py
 src/pybritive/commands/__init__.py
 src/pybritive/commands/api.py
 src/pybritive/commands/aws.py
 src/pybritive/commands/cache.py
 src/pybritive/commands/checkin.py
 src/pybritive/commands/checkout.py
 src/pybritive/commands/clear.py
```

### Comparing `pybritive-1.4.0rc3/tests/test_0100_version.py` & `pybritive-1.4.0rc4/tests/test_0100_version.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/tests/test_0200_configure.py` & `pybritive-1.4.0rc4/tests/test_0200_configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/tests/test_0400_ls.py` & `pybritive-1.4.0rc4/tests/test_0400_ls.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/tests/test_0500_secret.py` & `pybritive-1.4.0rc4/tests/test_0500_secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/tests/test_0700_checkout.py` & `pybritive-1.4.0rc4/tests/test_0700_checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/tests/test_0850_clear.py` & `pybritive-1.4.0rc4/tests/test_0850_clear.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc3/tests/test_0900_login.py` & `pybritive-1.4.0rc4/tests/test_0900_login.py`

 * *Files identical despite different names*

