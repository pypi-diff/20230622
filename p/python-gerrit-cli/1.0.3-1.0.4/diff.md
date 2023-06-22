# Comparing `tmp/python-gerrit-cli-1.0.3.tar.gz` & `tmp/python-gerrit-cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/devspace/python-gerrit-cli/dist/.tmp-p7f094yu/python-gerrit-cli-1.0.3.tar", last modified: Sun May  7 13:24:33 2023, max compression
+gzip compressed data, was "/devspace/python-gerrit-cli/dist/.tmp-j_ooo6ko/python-gerrit-cli-1.0.4.tar", last modified: Thu Jun 22 10:39:07 2023, max compression
```

## Comparing `python-gerrit-cli-1.0.3.tar` & `python-gerrit-cli-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-05-07 13:24:33.699368 python-gerrit-cli-1.0.3/
--rw-rw-r--   0 pk        (1000) pk        (1000)     1113 2023-05-07 07:31:21.000000 python-gerrit-cli-1.0.3/LICENSE
--rw-rw-r--   0 pk        (1000) pk        (1000)     2244 2023-05-07 13:24:33.687368 python-gerrit-cli-1.0.3/PKG-INFO
--rw-rw-r--   0 pk        (1000) pk        (1000)       33 2023-05-07 07:23:12.000000 python-gerrit-cli-1.0.3/README.md
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-05-07 13:24:33.635368 python-gerrit-cli-1.0.3/gerritcli/
--rw-rw-r--   0 pk        (1000) pk        (1000)     6573 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.3/gerritcli/__init__.py
--rwxrwxr-x   0 pk        (1000) pk        (1000)     1203 2023-05-07 12:34:46.000000 python-gerrit-cli-1.0.3/gerritcli/__main__.py
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-05-07 13:24:33.663368 python-gerrit-cli-1.0.3/gerritcli/command/
--rw-rw-r--   0 pk        (1000) pk        (1000)      288 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.3/gerritcli/command/__init__.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     6090 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.3/gerritcli/command/account_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     5652 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.3/gerritcli/command/change_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     5557 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.3/gerritcli/command/group_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     4281 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.3/gerritcli/command/project_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     2112 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.3/gerritcli/command/server_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)      497 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.3/gerritcli/command/version_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     4031 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.3/gerritcli/utils.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     6021 2023-05-07 13:23:16.000000 python-gerrit-cli-1.0.3/pyproject.toml
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-05-07 13:24:33.683368 python-gerrit-cli-1.0.3/python_gerrit_cli.egg-info/
--rw-rw-r--   0 pk        (1000) pk        (1000)     2244 2023-05-07 13:24:33.000000 python-gerrit-cli-1.0.3/python_gerrit_cli.egg-info/PKG-INFO
--rw-rw-r--   0 pk        (1000) pk        (1000)      591 2023-05-07 13:24:33.000000 python-gerrit-cli-1.0.3/python_gerrit_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)        1 2023-05-07 13:24:33.000000 python-gerrit-cli-1.0.3/python_gerrit_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       54 2023-05-07 13:24:33.000000 python-gerrit-cli-1.0.3/python_gerrit_cli.egg-info/entry_points.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       39 2023-05-07 13:24:33.000000 python-gerrit-cli-1.0.3/python_gerrit_cli.egg-info/requires.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       10 2023-05-07 13:24:33.000000 python-gerrit-cli-1.0.3/python_gerrit_cli.egg-info/top_level.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       38 2023-05-07 13:24:33.699368 python-gerrit-cli-1.0.3/setup.cfg
+drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-06-22 10:39:07.658120 python-gerrit-cli-1.0.4/
+-rw-rw-r--   0 pk        (1000) pk        (1000)     1113 2023-05-07 07:31:21.000000 python-gerrit-cli-1.0.4/LICENSE
+-rw-rw-r--   0 pk        (1000) pk        (1000)     2244 2023-06-22 10:39:07.654120 python-gerrit-cli-1.0.4/PKG-INFO
+-rw-rw-r--   0 pk        (1000) pk        (1000)       33 2023-05-07 07:23:12.000000 python-gerrit-cli-1.0.4/README.md
+drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-06-22 10:39:07.554120 python-gerrit-cli-1.0.4/gerritcli/
+-rw-rw-r--   0 pk        (1000) pk        (1000)     6573 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/__init__.py
+-rwxrwxr-x   0 pk        (1000) pk        (1000)     1203 2023-05-07 12:34:46.000000 python-gerrit-cli-1.0.4/gerritcli/__main__.py
+drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-06-22 10:39:07.594120 python-gerrit-cli-1.0.4/gerritcli/command/
+-rw-rw-r--   0 pk        (1000) pk        (1000)      327 2023-06-22 03:56:56.000000 python-gerrit-cli-1.0.4/gerritcli/command/__init__.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)     6090 2023-06-22 09:21:24.000000 python-gerrit-cli-1.0.4/gerritcli/command/account_command.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)     5698 2023-06-22 09:21:57.000000 python-gerrit-cli-1.0.4/gerritcli/command/change_command.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)     5557 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/command/group_command.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)     1740 2023-06-22 09:32:38.000000 python-gerrit-cli-1.0.4/gerritcli/command/patch_command.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)     4281 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/command/project_command.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)     2112 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/command/server_command.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)      497 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/command/version_command.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)     4031 2023-06-22 09:21:14.000000 python-gerrit-cli-1.0.4/gerritcli/utils.py
+-rw-rw-r--   0 pk        (1000) pk        (1000)     6021 2023-06-22 10:37:31.000000 python-gerrit-cli-1.0.4/pyproject.toml
+drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-06-22 10:39:07.650120 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/
+-rw-rw-r--   0 pk        (1000) pk        (1000)     2244 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 pk        (1000) pk        (1000)      626 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 pk        (1000) pk        (1000)        1 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 pk        (1000) pk        (1000)       54 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 pk        (1000) pk        (1000)       39 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/requires.txt
+-rw-rw-r--   0 pk        (1000) pk        (1000)       10 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/top_level.txt
+-rw-rw-r--   0 pk        (1000) pk        (1000)       38 2023-06-22 10:39:07.658120 python-gerrit-cli-1.0.4/setup.cfg
```

### Comparing `python-gerrit-cli-1.0.3/LICENSE` & `python-gerrit-cli-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.3/PKG-INFO` & `python-gerrit-cli-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Gerrit Command Line Interface
 Author-email: Kai Peng <pkemb@outlook.com>
 Maintainer-email: Kai Peng <pkemb@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kai Peng, https://pkemb.com <pkemb@outlook.com>
```

### Comparing `python-gerrit-cli-1.0.3/gerritcli/__init__.py` & `python-gerrit-cli-1.0.4/gerritcli/__init__.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.3/gerritcli/__main__.py` & `python-gerrit-cli-1.0.4/gerritcli/__main__.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.3/gerritcli/command/account_command.py` & `python-gerrit-cli-1.0.4/gerritcli/command/account_command.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.3/gerritcli/command/change_command.py` & `python-gerrit-cli-1.0.4/gerritcli/command/change_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 }
 
 class gerrit_change_info(gerritcli.utils.gerrit_info):
     """
     Documentation/rest-api-changes.html#change-info
     """
     def __init__(self, change, **kwargs):
+        self.content = deepcopy(self.content)
         # 无需转换的内容的key
         keylist = ['project', 'branch', 'change_id', 'subject', \
                    'status', 'topic', 'id', 'insertions', 'deletions' \
                    'meta_rev_id']
         for key in keylist:
             self.content[key] = change.get(key, empty_change[key])
```

### Comparing `python-gerrit-cli-1.0.3/gerritcli/command/group_command.py` & `python-gerrit-cli-1.0.4/gerritcli/command/group_command.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.3/gerritcli/command/project_command.py` & `python-gerrit-cli-1.0.4/gerritcli/command/project_command.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.3/gerritcli/command/server_command.py` & `python-gerrit-cli-1.0.4/gerritcli/command/server_command.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.3/gerritcli/utils.py` & `python-gerrit-cli-1.0.4/gerritcli/utils.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.3/pyproject.toml` & `python-gerrit-cli-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "python-gerrit-cli"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.3"  # Required
+version = "1.0.4"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Gerrit Command Line Interface"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `python-gerrit-cli-1.0.3/python_gerrit_cli.egg-info/PKG-INFO` & `python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Gerrit Command Line Interface
 Author-email: Kai Peng <pkemb@outlook.com>
 Maintainer-email: Kai Peng <pkemb@outlook.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Kai Peng, https://pkemb.com <pkemb@outlook.com>
```

### Comparing `python-gerrit-cli-1.0.3/python_gerrit_cli.egg-info/SOURCES.txt` & `python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 gerritcli/__init__.py
 gerritcli/__main__.py
 gerritcli/utils.py
 gerritcli/command/__init__.py
 gerritcli/command/account_command.py
 gerritcli/command/change_command.py
 gerritcli/command/group_command.py
+gerritcli/command/patch_command.py
 gerritcli/command/project_command.py
 gerritcli/command/server_command.py
 gerritcli/command/version_command.py
 python_gerrit_cli.egg-info/PKG-INFO
 python_gerrit_cli.egg-info/SOURCES.txt
 python_gerrit_cli.egg-info/dependency_links.txt
 python_gerrit_cli.egg-info/entry_points.txt
```

