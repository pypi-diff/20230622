# Comparing `tmp/pybritive-1.4.0rc4.tar.gz` & `tmp/pybritive-1.4.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybritive-1.4.0rc4.tar", last modified: Thu Jun 22 18:08:59 2023, max compression
+gzip compressed data, was "pybritive-1.4.0rc5.tar", last modified: Thu Jun 22 18:25:16 2023, max compression
```

## Comparing `pybritive-1.4.0rc4.tar` & `pybritive-1.4.0rc5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.355534 pybritive-1.4.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-22 18:08:59.355534 pybritive-1.4.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-22 18:08:59.355534 pybritive-1.4.0rc4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.335532 pybritive-1.4.0rc4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.339532 pybritive-1.4.0rc4/src/pybritive/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/britive_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.339532 pybritive-1.4.0rc4/src/pybritive/choices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/choices/ssh_push_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/cli_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.343533 pybritive-1.4.0rc4/src/pybritive/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/commands/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.343533 pybritive-1.4.0rc4/src/pybritive/completers/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/api_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/bash_gte_42.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/powershell_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/completers/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.347533 pybritive-1.4.0rc4/src/pybritive/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/api_method_argument_dectorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/aws_credential_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/build_britive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/cloud_credential_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/profile_argument_dectorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/helpers/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.351534 pybritive-1.4.0rc4/src/pybritive/options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/aws_console_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/aws_credentials_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/blocktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/britive_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/checked_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/configure_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/configure_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/configure_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/configure_tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/federation_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/force_renew.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/gcloud_key_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/justification.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/maxpolltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/passphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/silent.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_push_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/ssh_username.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/src/pybritive/options/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.339532 pybritive-1.4.0rc4/src/pybritive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 18:08:59.000000 pybritive-1.4.0rc4/src/pybritive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:08:59.355534 pybritive-1.4.0rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0100_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0200_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0300_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0400_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0450_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0500_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0600_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0700_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0800_checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0850_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_0900_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-22 18:08:46.000000 pybritive-1.4.0rc4/tests/test_1000_logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.370029 pybritive-1.4.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-22 18:25:16.370029 pybritive-1.4.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-22 18:25:16.374029 pybritive-1.4.0rc5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.354029 pybritive-1.4.0rc5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.358029 pybritive-1.4.0rc5/src/pybritive/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49990 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/britive_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.358029 pybritive-1.4.0rc5/src/pybritive/choices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/choices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/choices/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/choices/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/choices/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/choices/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/choices/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/choices/ssh_push_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/cli_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.362028 pybritive-1.4.0rc5/src/pybritive/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/commands/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.362028 pybritive-1.4.0rc5/src/pybritive/completers/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/completers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/completers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/completers/api_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/completers/bash_gte_42.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/completers/powershell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/completers/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.366029 pybritive-1.4.0rc5/src/pybritive/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/api_method_argument_dectorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/aws_credential_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/build_britive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/cloud_credential_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/profile_argument_dectorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/helpers/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.370029 pybritive-1.4.0rc5/src/pybritive/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/aws_console_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/aws_credentials_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/blocktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/britive_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/checked_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/configure_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/configure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/configure_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/configure_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/federation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/force_renew.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/gcloud_key_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/justification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/maxpolltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/passphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/silent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/ssh_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/ssh_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/ssh_push_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/ssh_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/src/pybritive/options/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.358029 pybritive-1.4.0rc5/src/pybritive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-22 18:25:16.000000 pybritive-1.4.0rc5/src/pybritive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-22 18:25:16.000000 pybritive-1.4.0rc5/src/pybritive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:25:16.000000 pybritive-1.4.0rc5/src/pybritive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 18:25:16.000000 pybritive-1.4.0rc5/src/pybritive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 18:25:16.000000 pybritive-1.4.0rc5/src/pybritive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 18:25:16.000000 pybritive-1.4.0rc5/src/pybritive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:16.370029 pybritive-1.4.0rc5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0100_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0200_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0300_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0400_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0450_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0500_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0600_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0700_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0800_checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0850_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_0900_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-22 18:25:04.000000 pybritive-1.4.0rc5/tests/test_1000_logout.py
```

### Comparing `pybritive-1.4.0rc4/LICENSE` & `pybritive-1.4.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/PKG-INFO` & `pybritive-1.4.0rc5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.4.0rc4
+Version: 1.4.0rc5
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybritive-1.4.0rc4/README.md` & `pybritive-1.4.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/setup.cfg` & `pybritive-1.4.0rc5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybritive
-version = 1.4.0rc4
+version = 1.4.0rc5
 author = Britive Inc.
 author_email = support@britive.com
 description = A pure Python CLI for Britive
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.britive.com
 classifiers =
```

### Comparing `pybritive-1.4.0rc4/src/pybritive/britive_cli.py` & `pybritive-1.4.0rc5/src/pybritive/britive_cli.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/choices/mode.py` & `pybritive-1.4.0rc5/src/pybritive/choices/mode.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/choices/output_format.py` & `pybritive-1.4.0rc5/src/pybritive/choices/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/cli_interface.py` & `pybritive-1.4.0rc5/src/pybritive/cli_interface.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/api.py` & `pybritive-1.4.0rc5/src/pybritive/commands/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/aws.py` & `pybritive-1.4.0rc5/src/pybritive/commands/aws.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/cache.py` & `pybritive-1.4.0rc5/src/pybritive/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/checkin.py` & `pybritive-1.4.0rc5/src/pybritive/commands/checkin.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/checkout.py` & `pybritive-1.4.0rc5/src/pybritive/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/clear.py` & `pybritive-1.4.0rc5/src/pybritive/commands/clear.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/configure.py` & `pybritive-1.4.0rc5/src/pybritive/commands/configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/login.py` & `pybritive-1.4.0rc5/src/pybritive/commands/login.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/ls.py` & `pybritive-1.4.0rc5/src/pybritive/commands/ls.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/request.py` & `pybritive-1.4.0rc5/src/pybritive/commands/request.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/secret.py` & `pybritive-1.4.0rc5/src/pybritive/commands/secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/commands/ssh.py` & `pybritive-1.4.0rc5/src/pybritive/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/completers/api.py` & `pybritive-1.4.0rc5/src/pybritive/completers/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/completers/api_command.py` & `pybritive-1.4.0rc5/src/pybritive/completers/api_command.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/completers/bash_gte_42.py` & `pybritive-1.4.0rc5/src/pybritive/completers/bash_gte_42.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/completers/powershell_completion.py` & `pybritive-1.4.0rc5/src/pybritive/completers/powershell_completion.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/completers/profile.py` & `pybritive-1.4.0rc5/src/pybritive/completers/profile.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/helpers/aws_credential_process.py` & `pybritive-1.4.0rc5/src/pybritive/helpers/aws_credential_process.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/helpers/build_britive.py` & `pybritive-1.4.0rc5/src/pybritive/helpers/build_britive.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/helpers/cache.py` & `pybritive-1.4.0rc5/src/pybritive/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/helpers/cloud_credential_printer.py` & `pybritive-1.4.0rc5/src/pybritive/helpers/cloud_credential_printer.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/helpers/config.py` & `pybritive-1.4.0rc5/src/pybritive/helpers/config.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/helpers/credentials.py` & `pybritive-1.4.0rc5/src/pybritive/helpers/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
             import urllib3
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     def perform_interactive_login(self):
         self.cli.print(f'Performing interactive login against tenant {self.tenant}.')
         sso_idp = self.cli.config.get_tenant().get('sso_idp')
         if sso_idp:
+            sso_idp = sso_idp.replace('saml', 'SAML')  # ui is expecting it in caps
             url = f'{self.base_url}/sso?idp={sso_idp}&token={self.auth_token}'
         else:
             url = f'{self.base_url}/login?token={self.auth_token}'
 
         # establish a requests session which will be used in retrieve_tokens()
         self._setup_requests_session()
```

### Comparing `pybritive-1.4.0rc4/src/pybritive/helpers/encryption.py` & `pybritive-1.4.0rc5/src/pybritive/helpers/encryption.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/helpers/split.py` & `pybritive-1.4.0rc5/src/pybritive/helpers/split.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/options/britive_options.py` & `pybritive-1.4.0rc5/src/pybritive/options/britive_options.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/options/browser.py` & `pybritive-1.4.0rc5/src/pybritive/options/browser.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/options/mode.py` & `pybritive-1.4.0rc5/src/pybritive/options/mode.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/options/output_format.py` & `pybritive-1.4.0rc5/src/pybritive/options/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/options/ssh_push_public_key.py` & `pybritive-1.4.0rc5/src/pybritive/options/ssh_push_public_key.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive/options/version.py` & `pybritive-1.4.0rc5/src/pybritive/options/version.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/src/pybritive.egg-info/PKG-INFO` & `pybritive-1.4.0rc5/src/pybritive.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.4.0rc4
+Version: 1.4.0rc5
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybritive-1.4.0rc4/src/pybritive.egg-info/SOURCES.txt` & `pybritive-1.4.0rc5/src/pybritive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/tests/test_0100_version.py` & `pybritive-1.4.0rc5/tests/test_0100_version.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/tests/test_0200_configure.py` & `pybritive-1.4.0rc5/tests/test_0200_configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/tests/test_0400_ls.py` & `pybritive-1.4.0rc5/tests/test_0400_ls.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/tests/test_0500_secret.py` & `pybritive-1.4.0rc5/tests/test_0500_secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/tests/test_0700_checkout.py` & `pybritive-1.4.0rc5/tests/test_0700_checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/tests/test_0850_clear.py` & `pybritive-1.4.0rc5/tests/test_0850_clear.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc4/tests/test_0900_login.py` & `pybritive-1.4.0rc5/tests/test_0900_login.py`

 * *Files identical despite different names*

