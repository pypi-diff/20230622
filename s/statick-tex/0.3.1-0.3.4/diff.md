# Comparing `tmp/statick-tex-0.3.1.tar.gz` & `tmp/statick-tex-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statick-tex-0.3.1.tar", last modified: Mon Oct 10 21:08:12 2022, max compression
+gzip compressed data, was "statick-tex-0.3.4.tar", last modified: Thu Jun 22 01:14:02 2023, max compression
```

## Comparing `statick-tex-0.3.1.tar` & `statick-tex-0.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:08:12.732541 statick-tex-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (116)     6401 2022-10-10 21:08:04.000000 statick-tex-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5061 2022-10-10 21:08:12.732541 statick-tex-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4299 2022-10-10 21:08:04.000000 statick-tex-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:08:12.732541 statick-tex-0.3.1/rsc/
--rw-r--r--   0 runner    (1001) docker     (116)      299 2022-10-10 21:08:04.000000 statick-tex-0.3.1/rsc/tex-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       25 2022-10-10 21:08:04.000000 statick-tex-0.3.1/rsc/tex-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-10 21:08:12.732541 statick-tex-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1665 2022-10-10 21:08:04.000000 statick-tex-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:08:12.732541 statick-tex-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:08:12.732541 statick-tex-0.3.1/src/statick_tex/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:08:12.732541 statick-tex-0.3.1/src/statick_tex/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:08:12.732541 statick-tex-0.3.1/src/statick_tex/plugins/discovery/
--rw-r--r--   0 runner    (1001) docker     (116)       33 2022-10-10 21:08:04.000000 statick-tex-0.3.1/src/statick_tex/plugins/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1755 2022-10-10 21:08:04.000000 statick-tex-0.3.1/src/statick_tex/plugins/discovery/tex_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       65 2022-10-10 21:08:04.000000 statick-tex-0.3.1/src/statick_tex/plugins/discovery/tex_discovery_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:08:12.732541 statick-tex-0.3.1/src/statick_tex/plugins/tool/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-10-10 21:08:04.000000 statick-tex-0.3.1/src/statick_tex/plugins/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3292 2022-10-10 21:08:04.000000 statick-tex-0.3.1/src/statick_tex/plugins/tool/chktex_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       61 2022-10-10 21:08:04.000000 statick-tex-0.3.1/src/statick_tex/plugins/tool/chktex_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     2990 2022-10-10 21:08:04.000000 statick-tex-0.3.1/src/statick_tex/plugins/tool/lacheck_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       63 2022-10-10 21:08:04.000000 statick-tex-0.3.1/src/statick_tex/plugins/tool/lacheck_tool_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:08:12.732541 statick-tex-0.3.1/statick_tex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5061 2022-10-10 21:08:12.000000 statick-tex-0.3.1/statick_tex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      684 2022-10-10 21:08:12.000000 statick-tex-0.3.1/statick_tex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-10 21:08:12.000000 statick-tex-0.3.1/statick_tex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2022-10-10 21:08:12.000000 statick-tex-0.3.1/statick_tex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2022-10-10 21:08:12.000000 statick-tex-0.3.1/statick_tex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.412473 statick-tex-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-22 01:13:57.000000 statick-tex-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-22 01:14:02.412473 statick-tex-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-22 01:13:57.000000 statick-tex-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.408473 statick-tex-0.3.4/rsc/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-22 01:13:57.000000 statick-tex-0.3.4/rsc/tex-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 01:13:57.000000 statick-tex-0.3.4/rsc/tex-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:14:02.412473 statick-tex-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-22 01:13:57.000000 statick-tex-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.408473 statick-tex-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.408473 statick-tex-0.3.4/src/statick_tex/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.408473 statick-tex-0.3.4/src/statick_tex/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.412473 statick-tex-0.3.4/src/statick_tex/plugins/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/discovery/tex_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/discovery/tex_discovery_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.412473 statick-tex-0.3.4/src/statick_tex/plugins/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/chktex_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/chktex_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/lacheck_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 01:13:57.000000 statick-tex-0.3.4/src/statick_tex/plugins/tool/lacheck_tool_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:14:02.412473 statick-tex-0.3.4/statick_tex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 01:14:02.000000 statick-tex-0.3.4/statick_tex.egg-info/top_level.txt
```

### Comparing `statick-tex-0.3.1/LICENSE` & `statick-tex-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `statick-tex-0.3.1/PKG-INFO` & `statick-tex-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: statick-tex
-Version: 0.3.1
+Version: 0.3.4
 Summary: Statick analysis plugins for TeX/LaTeX files and projects.
 Home-page: https://github.com/tdenewiler/statick-tex
 Author: Thomas Denewiler
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `statick-tex-0.3.1/README.md` & `statick-tex-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `statick-tex-0.3.1/setup.py` & `statick-tex-0.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 with open("README.md", encoding="utf-8") as fid:
     long_description = fid.read()  # pylint: disable=invalid-name
 
 TEST_DEPS = [
     "mock",
     "pre-commit",
-    "pytest",
+    "pytest==7.1",
 ]
 
 EXTRAS = {
     "test": TEST_DEPS,
 }
 
 setup(
     author="Thomas Denewiler",
     name="statick-tex",
     description="Statick analysis plugins for TeX/LaTeX files and projects.",
-    version="0.3.1",
+    version="0.3.4",
     packages=[
         "statick_tool",
         "statick_tool.plugins.discovery",
         "statick_tool.plugins.tool",
     ],
     package_dir={
         "statick_tool": ".",
@@ -40,17 +40,17 @@
     long_description_content_type="text/markdown",
     install_requires=["statick"],
     tests_require=TEST_DEPS,
     extras_require=EXTRAS,
     url="https://github.com/tdenewiler/statick-tex",
     classifiers=[
         "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
         "Topic :: Text Processing :: Markup :: LaTeX",
         "Typing :: Typed",
     ],
 )
```

### Comparing `statick-tex-0.3.1/src/statick_tex/plugins/discovery/tex_discovery_plugin.py` & `statick-tex-0.3.4/src/statick_tex/plugins/discovery/tex_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-tex-0.3.1/src/statick_tex/plugins/tool/chktex_tool_plugin.py` & `statick-tex-0.3.4/src/statick_tex/plugins/tool/lacheck_tool_plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,90 @@
-"""Apply chktex tool and gather results.
-
-Chktex documentation at http://mirrors.rit.edu/CTAN/systems/doc/chktex/ChkTeX.pdf.
-"""
+"""Apply lacheck tool and gather results."""
 import logging
 import re
 import subprocess
 from typing import List, Match, Optional, Pattern
 
 from statick_tool.issue import Issue
 from statick_tool.package import Package
 from statick_tool.tool_plugin import ToolPlugin
 
 
-class ChktexToolPlugin(ToolPlugin):  # type: ignore
-    """Apply chktex tool and gather results."""
+class LacheckToolPlugin(ToolPlugin):  # type: ignore
+    """Apply lacheck tool and gather results."""
 
     def get_name(self) -> str:
         """Get name of tool."""
-        return "chktex"
+        return "lacheck"
 
-    def scan(self, package: Package, level: str) -> Optional[List[Issue]]:
+    def get_file_types(self) -> List[str]:
+        """Return a list of file types the plugin can scan."""
+        return ["tex"]
+
+    # pylint: disable=too-many-locals
+    def process_files(
+        self, package: Package, level: str, files: List[str], user_flags: List[str]
+    ) -> Optional[List[str]]:
         """Run tool and gather output."""
         flags: List[str] = []
-        user_flags: List[str] = self.get_user_flags(level)
         flags += user_flags
-        total_output: List[str] = []
 
-        tool_bin: str = "chktex"
-        for src in package["tex"]:
-            try:
-                subproc_args: List[str] = [tool_bin, src] + flags
-                output = subprocess.check_output(
-                    subproc_args, stderr=subprocess.STDOUT, universal_newlines=True
-                )
-
-            except subprocess.CalledProcessError as ex:
-                # Return code 1 means "found problems".
-                # Return code 2 provides correct output with test cases used so far.
-                if ex.returncode not in (1, 2):
-                    logging.warning("Problem %s", ex.returncode)
-                    logging.warning("%s exception: %s", self.get_name(), ex.output)
-                    return None
-                output = ex.output
+        total_output: List[str] = []
 
-            except OSError as ex:
-                logging.warning("Couldn't find %s! (%s)", tool_bin, ex)
+        tool_bin: str = "lacheck"
+        try:
+            subproc_args: List[str] = [tool_bin] + flags + files
+            output = subprocess.check_output(
+                subproc_args, stderr=subprocess.STDOUT, universal_newlines=True
+            )
+
+        except subprocess.CalledProcessError as ex:
+            # Return code 1 just means "found problems"
+            if ex.returncode != 1:
+                logging.warning("Problem %d", ex.returncode)
+                logging.warning("%s exception: %s", self.get_name(), ex.output)
                 return None
+            output = ex.output
 
-            logging.debug("%s", output)
+        except OSError as ex:
+            logging.warning("Couldn't find %s! (%s)", tool_bin, ex)
+            return None
 
-            total_output.append(output)
+        logging.debug("%s", output)
 
-        with open(self.get_name() + ".log", "w", encoding="utf-8") as fid:
-            for output in total_output:
-                fid.write(output)
+        total_output.append(output)
 
-        issues: List[Issue] = self.parse_output(total_output)
-        return issues
+        return total_output
 
-    def parse_output(self, total_output: List[str]) -> List[Issue]:
+    def parse_output(
+        self, total_output: List[str], package: Optional[Package] = None
+    ) -> List[Issue]:
         """Parse tool output and report issues."""
-        tool_re: str = r"(.+)\s(\d+)\s(.+)\s(.+)\s(.+)\s(\d+):\s(.+)"
+        tool_re: str = r"(.+)\s(.+)\s(\d+):\s(.+)"
         parse: Pattern[str] = re.compile(tool_re)
         issues: List[Issue] = []
         filename: str = ""
         line_number: str = "0"
         issue_type: str = ""
         message: str = ""
 
         for output in total_output:
             for line in output.splitlines():
                 match: Optional[Match[str]] = parse.match(line)
                 if match:
-                    if match.group(1) == "Warning":
-                        filename = match.group(4)
-                        issue_type = match.group(2)
-                        line_number = match.group(6)
-                        message = match.group(7)
-                        issues.append(
-                            Issue(
-                                filename,
-                                line_number,
-                                self.get_name(),
-                                issue_type,
-                                "3",
-                                message,
-                                None,
-                            )
+                    filename = match.group(1)[1:-2]
+                    issue_type = "lacheck"
+                    line_number = match.group(3)
+                    message = match.group(4)
+                    issues.append(
+                        Issue(
+                            filename,
+                            line_number,
+                            self.get_name(),
+                            issue_type,
+                            "3",
+                            message,
+                            None,
                         )
+                    )
 
         return issues
```

### Comparing `statick-tex-0.3.1/statick_tex.egg-info/PKG-INFO` & `statick-tex-0.3.4/statick_tex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: statick-tex
-Version: 0.3.1
+Version: 0.3.4
 Summary: Statick analysis plugins for TeX/LaTeX files and projects.
 Home-page: https://github.com/tdenewiler/statick-tex
 Author: Thomas Denewiler
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `statick-tex-0.3.1/statick_tex.egg-info/SOURCES.txt` & `statick-tex-0.3.4/statick_tex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

