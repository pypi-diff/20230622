# Comparing `tmp/dbt_copilot_tools-0.1.3.tar.gz` & `tmp/dbt_copilot_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_tools-0.1.3.tar", max compression
+gzip compressed data, was "dbt_copilot_tools-0.1.4.tar", max compression
```

## Comparing `dbt_copilot_tools-0.1.3.tar` & `dbt_copilot_tools-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.3/LICENSE
--rw-r--r--   0        0        0     1593 2023-06-21 10:28:30.704825 dbt_copilot_tools-0.1.3/commands/README.md
--rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.3/commands/__init__.py
--rwxr-xr-x   0        0        0     9980 2023-06-21 10:25:13.933813 dbt_copilot_tools-0.1.3/commands/bootstrap_cli.py
--rwxr-xr-x   0        0        0     2560 2023-06-20 14:07:55.205282 dbt_copilot_tools-0.1.3/commands/check_cloudformation.py
--rwxr-xr-x   0        0        0    13488 2023-06-20 09:47:08.337250 dbt_copilot_tools-0.1.3/commands/codebuild_cli.py
--rwxr-xr-x   0        0        0     8582 2023-06-15 16:41:34.056908 dbt_copilot_tools-0.1.3/commands/copilot_cli.py
--rwxr-xr-x   0        0        0    20699 2023-06-20 09:47:08.337507 dbt_copilot_tools-0.1.3/commands/dns_cli.py
--rw-r--r--   0        0        0     5902 2023-06-16 11:05:25.989196 dbt_copilot_tools-0.1.3/commands/utils.py
--rwxr-xr-x   0        0        0      803 2023-06-20 14:07:55.205587 dbt_copilot_tools-0.1.3/copilot_helper.py
--rw-r--r--   0        0        0     1169 2023-06-21 10:25:23.727055 dbt_copilot_tools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.4/LICENSE
+-rw-r--r--   0        0        0    20712 2023-06-22 15:45:06.988416 dbt_copilot_tools-0.1.4/commands/COMMANDS.md
+-rw-r--r--   0        0        0     1679 2023-06-22 15:42:02.772921 dbt_copilot_tools-0.1.4/commands/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.4/commands/__init__.py
+-rwxr-xr-x   0        0        0     9980 2023-06-22 13:57:32.008663 dbt_copilot_tools-0.1.4/commands/bootstrap_cli.py
+-rwxr-xr-x   0        0        0     2560 2023-06-20 14:07:55.205282 dbt_copilot_tools-0.1.4/commands/check_cloudformation.py
+-rwxr-xr-x   0        0        0    13488 2023-06-20 09:47:08.337250 dbt_copilot_tools-0.1.4/commands/codebuild_cli.py
+-rwxr-xr-x   0        0        0     8582 2023-06-15 16:41:34.056908 dbt_copilot_tools-0.1.4/commands/copilot_cli.py
+-rwxr-xr-x   0        0        0    20699 2023-06-20 09:47:08.337507 dbt_copilot_tools-0.1.4/commands/dns_cli.py
+-rw-r--r--   0        0        0     5902 2023-06-16 11:05:25.989196 dbt_copilot_tools-0.1.4/commands/utils.py
+-rwxr-xr-x   0        0        0      880 2023-06-22 14:38:58.585299 dbt_copilot_tools-0.1.4/copilot_helper.py
+-rw-r--r--   0        0        0     1169 2023-06-22 15:46:26.732715 dbt_copilot_tools-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.4/PKG-INFO
```

### Comparing `dbt_copilot_tools-0.1.3/LICENSE` & `dbt_copilot_tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.3/commands/README.md` & `dbt_copilot_tools-0.1.4/commands/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -44,7 +44,9 @@
   --help  Show this message and exit.
 
 Commands:
   instructions     Show migration instructions.
   make-config      Generate copilot boilerplate code.
   migrate-secrets  Migrate secrets from your gov paas application to...
 ```
+
+See the [Commands Reference](./COMMANDS.md) for a list of all available subcommands.
```

### Comparing `dbt_copilot_tools-0.1.3/commands/bootstrap_cli.py` & `dbt_copilot_tools-0.1.4/commands/bootstrap_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.3/commands/check_cloudformation.py` & `dbt_copilot_tools-0.1.4/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.3/commands/codebuild_cli.py` & `dbt_copilot_tools-0.1.4/commands/codebuild_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.3/commands/copilot_cli.py` & `dbt_copilot_tools-0.1.4/commands/copilot_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.3/commands/dns_cli.py` & `dbt_copilot_tools-0.1.4/commands/dns_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.3/commands/utils.py` & `dbt_copilot_tools-0.1.4/commands/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.3/pyproject.toml` & `dbt_copilot_tools-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 119
 
 [tool.poetry]
 name = "dbt-copilot-tools"
-version = "0.1.3"
+version = "0.1.4"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "commands/README.md"
 packages = [
     { include = "commands" },
     { include = "copilot_helper.py" }
```

### Comparing `dbt_copilot_tools-0.1.3/PKG-INFO` & `dbt_copilot_tools-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-copilot-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -70,7 +70,9 @@
 
 Commands:
   instructions     Show migration instructions.
   make-config      Generate copilot boilerplate code.
   migrate-secrets  Migrate secrets from your gov paas application to...
 ```
 
+See the [Commands Reference](./COMMANDS.md) for a list of all available subcommands.
+
```

