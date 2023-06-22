# Comparing `tmp/tif-3.0.1.tar.gz` & `tmp/tif-3.1.0.tar.gz`

## Comparing `tif-3.0.1.tar` & `tif-3.1.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.0.1/tif/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.0.1/tif/bin/__init__.py
--rw-r--r--   0        0        0     9712 2020-02-02 00:00:00.000000 tif-3.0.1/tif/bin/magento.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.0.1/tif/cli/__init__.py
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 tif-3.0.1/tif/cli/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.0.1/tif/composer/__init__.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 tif-3.0.1/tif/composer/operations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.0.1/tif/docker/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 tif-3.0.1/tif/docker/magento.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 tif-3.0.1/tif/docker/service.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 tif-3.0.1/tif/fabric/Colors.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 tif-3.0.1/tif/fabric/CommandPrefix.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tif-3.0.1/tif/fabric/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 tif-3.0.1/tif/fabric/cli.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 tif-3.0.1/tif/fabric/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.0.1/tif/files/__init__.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 tif-3.0.1/tif/files/operations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.0.1/tif/git/__init__.py
--rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 tif-3.0.1/tif/git/operations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.0.1/tif/sql/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 tif-3.0.1/tif/sql/operations.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tif-3.0.1/LICENSE
--rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 tif-3.0.1/README.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tif-3.0.1/pyproject.toml
--rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 tif-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tif-3.1.0/tif/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.1.0/tif/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.1.0/tif/bin/__init__.py
+-rw-r--r--   0        0        0     9712 2020-02-02 00:00:00.000000 tif-3.1.0/tif/bin/magento.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.1.0/tif/cli/__init__.py
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 tif-3.1.0/tif/cli/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.1.0/tif/composer/__init__.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 tif-3.1.0/tif/composer/operations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.1.0/tif/docker/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 tif-3.1.0/tif/docker/magento.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 tif-3.1.0/tif/docker/service.py
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 tif-3.1.0/tif/docker/warden.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 tif-3.1.0/tif/fabric/Colors.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 tif-3.1.0/tif/fabric/CommandPrefix.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tif-3.1.0/tif/fabric/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 tif-3.1.0/tif/fabric/cli.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 tif-3.1.0/tif/fabric/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.1.0/tif/files/__init__.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 tif-3.1.0/tif/files/operations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.1.0/tif/git/__init__.py
+-rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 tif-3.1.0/tif/git/operations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tif-3.1.0/tif/sql/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 tif-3.1.0/tif/sql/operations.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tif-3.1.0/LICENSE
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 tif-3.1.0/README.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tif-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 tif-3.1.0/PKG-INFO
```

### Comparing `tif-3.0.1/tif/bin/magento.py` & `tif-3.1.0/tif/bin/magento.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/tif/cli/options.py` & `tif-3.1.0/tif/cli/options.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/tif/composer/operations.py` & `tif-3.1.0/tif/composer/operations.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/tif/docker/magento.py` & `tif-3.1.0/tif/docker/magento.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/tif/docker/service.py` & `tif-3.1.0/tif/docker/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,31 +44,47 @@
         """
         Returns formatted command to execute on a docker container
         """
         command = "docker exec {} {} bash -c \"{}\"".format(exec_options, container, command)
         Logger().log("Running command '{}'".format(command))
         return command
 
-    def composeExec(self, yml_location: string, container : string, command : string, exec_options = "-it") -> string:
+    def compose_exec(self, yml_location: string, container : string, command : string, exec_options = "-it") -> string:
         """
         Returns formatted command to execute on a docker container
         """
         command = "cd {} && docker-compose exec {} {} bash -c \"{}\"".format(yml_location, exec_options, container, command)
         Logger().log("Running command '{}'".format(command))
         return command
 
-    def containerBash(self, container : string):
+    def container_bash(self, container : string):
         """
         Logs into a container bash
         """
         docker_compose_command = "docker-compose exec {} bash".format(container)
         command = "cd {} && {}".format(self.docker_dir, docker_compose_command)
         Logger().log("Running command '{}'".format(docker_compose_command))
         run(command, pty=True)
     
     def restart_container(self, container : string):
         """
-        Restart a container
+        Restarts a container
         """
         command = "docker restart {}".format(container)
         Logger().log("Running command '{}'".format(command))
+        run(command, pty=True)
+
+    def stop_container(self, container : string):
+        """
+        Stops a container
+        """
+        command = "docker stop {}".format(container)
+        Logger().log("Running command '{}'".format(command))
+        run(command, pty=True)
+
+    def start_container(self, container : string):
+        """
+        Starts a container
+        """
+        command = "docker start {}".format(container)
+        Logger().log("Running command '{}'".format(command))
         run(command, pty=True)
```

### Comparing `tif-3.0.1/tif/fabric/Colors.py` & `tif-3.1.0/tif/fabric/Colors.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/tif/fabric/cli.py` & `tif-3.1.0/tif/fabric/cli.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/tif/fabric/logger.py` & `tif-3.1.0/tif/fabric/logger.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/tif/files/operations.py` & `tif-3.1.0/tif/files/operations.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/tif/git/operations.py` & `tif-3.1.0/tif/git/operations.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/tif/sql/operations.py` & `tif-3.1.0/tif/sql/operations.py`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/LICENSE` & `tif-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tif-3.0.1/pyproject.toml` & `tif-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tif"
-version = "3.0.1"
+version = "3.1.0"
 authors = [
   { name="Carlo Tasca", email="c.tasca.tif@gmail.com" },
 ]
 description = "TIF Python Package"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

