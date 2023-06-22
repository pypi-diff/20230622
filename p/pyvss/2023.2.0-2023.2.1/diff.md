# Comparing `tmp/pyvss-2023.2.0.tar.gz` & `tmp/pyvss-2023.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvss-2023.2.0.tar", last modified: Thu Feb 16 16:04:46 2023, max compression
+gzip compressed data, was "pyvss-2023.2.1.tar", last modified: Fri Feb 24 20:58:59 2023, max compression
```

## Comparing `pyvss-2023.2.0.tar` & `pyvss-2023.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 16:04:46.469240 pyvss-2023.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-02-16 02:15:19.000000 pyvss-2023.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-02-16 02:15:19.000000 pyvss-2023.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7784 2023-02-16 16:04:46.469240 pyvss-2023.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6477 2023-02-16 02:15:19.000000 pyvss-2023.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-02-16 02:15:19.000000 pyvss-2023.2.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 16:04:46.469240 pyvss-2023.2.0/pyvss/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-16 02:15:19.000000 pyvss-2023.2.0/pyvss/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6751 2023-02-16 15:59:06.000000 pyvss-2023.2.0/pyvss/const.py
--rw-rw-rw-   0 root         (0) root         (0)     1409 2023-02-16 02:15:19.000000 pyvss-2023.2.0/pyvss/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2023-02-16 02:15:19.000000 pyvss-2023.2.0/pyvss/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-02-16 02:15:19.000000 pyvss-2023.2.0/pyvss/helper.py
--rw-rw-rw-   0 root         (0) root         (0)   277248 2023-02-16 02:15:19.000000 pyvss-2023.2.0/pyvss/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 16:04:46.469240 pyvss-2023.2.0/pyvss.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7784 2023-02-16 16:04:46.000000 pyvss-2023.2.0/pyvss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      325 2023-02-16 16:04:46.000000 pyvss-2023.2.0/pyvss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 16:04:46.000000 pyvss-2023.2.0/pyvss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      288 2023-02-16 16:04:46.000000 pyvss-2023.2.0/pyvss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-16 16:04:46.000000 pyvss-2023.2.0/pyvss.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-02-16 02:25:25.000000 pyvss-2023.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-02-16 16:04:46.469240 pyvss-2023.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3322 2023-02-16 02:15:19.000000 pyvss-2023.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 20:58:59.994942 pyvss-2023.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-02-16 02:15:19.000000 pyvss-2023.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-02-16 02:15:19.000000 pyvss-2023.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7784 2023-02-24 20:58:59.994942 pyvss-2023.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6477 2023-02-16 02:15:19.000000 pyvss-2023.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-02-16 02:15:19.000000 pyvss-2023.2.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 20:58:59.990942 pyvss-2023.2.1/pyvss/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-16 02:15:19.000000 pyvss-2023.2.1/pyvss/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6751 2023-02-24 20:55:34.000000 pyvss-2023.2.1/pyvss/const.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-02-16 02:15:19.000000 pyvss-2023.2.1/pyvss/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2023-02-16 02:15:19.000000 pyvss-2023.2.1/pyvss/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-02-16 02:15:19.000000 pyvss-2023.2.1/pyvss/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)   278930 2023-02-24 20:47:00.000000 pyvss-2023.2.1/pyvss/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 20:58:59.994942 pyvss-2023.2.1/pyvss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7784 2023-02-24 20:58:59.000000 pyvss-2023.2.1/pyvss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      325 2023-02-24 20:58:59.000000 pyvss-2023.2.1/pyvss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 20:58:59.000000 pyvss-2023.2.1/pyvss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      288 2023-02-24 20:58:59.000000 pyvss-2023.2.1/pyvss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-02-24 20:58:59.000000 pyvss-2023.2.1/pyvss.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-02-16 02:25:25.000000 pyvss-2023.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-02-24 20:58:59.994942 pyvss-2023.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3322 2023-02-16 02:15:19.000000 pyvss-2023.2.1/setup.py
```

### Comparing `pyvss-2023.2.0/LICENSE` & `pyvss-2023.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvss-2023.2.0/PKG-INFO` & `pyvss-2023.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyvss
-Version: 2023.2.0
+Version: 2023.2.1
 Summary: ITS Private Cloud Python Client
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/py-vss
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/py-vss/archive/2023.2.0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/py-vss/archive/2023.2.1.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/py-vss/issues
 Project-URL: Documentation, https://eis.utorotno.ca/~vss/py-vss/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/py-vss
```

### Comparing `pyvss-2023.2.0/README.md` & `pyvss-2023.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyvss-2023.2.0/pyvss/const.py` & `pyvss-2023.2.1/pyvss/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constants package for PyVSS."""
 PACKAGE_NAME = "pyvss"
 
-__version__ = '2023.2.0'
+__version__ = '2023.2.1'
 
 
 API_ENDPOINT_BASE = 'https://cloud-api.eis.utoronto.ca'
 
 VSS_S3_URL = 'https://vskey-stor.eis.utoronto.ca'
 VSS_S3_SVC_URL = '{s3_server}/s3/minio-svc/index.php'
 VSS_S3_STS_URL = '{s3_svc_url}?status=json'
```

### Comparing `pyvss-2023.2.0/pyvss/enums.py` & `pyvss-2023.2.1/pyvss/enums.py`

 * *Files identical despite different names*

### Comparing `pyvss-2023.2.0/pyvss/exceptions.py` & `pyvss-2023.2.1/pyvss/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvss-2023.2.0/pyvss/helper.py` & `pyvss-2023.2.1/pyvss/helper.py`

 * *Files identical despite different names*

### Comparing `pyvss-2023.2.0/pyvss/manager.py` & `pyvss-2023.2.1/pyvss/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -2860,32 +2860,37 @@
         :param vm_id: virtual machine moref or uuid
         :type vm_id: str
         :return: object
         """
         data = self.request(f'/vm/{vm_id}/storage-type')
         return data.get('data')
 
-    def update_vm_storage_type(self, vm_id, storage_type):
+    def update_vm_storage_type(self, vm_id, storage_type, **kwargs):
         """Update vm storage type.
 
         :param vm_id: virtual machine moref or uuid
         :type vm_id: str
         :param storage_type: new storage type
         :type storage_type: str
         :return:
+
+        .. note:: keyword arguments include schedule to process request
+          on a given date and time
         """
         current_st = self.get_vm_storage_type(vm_id)
         # check if current storage type is the same as requested
         if current_st['storage_type'] == storage_type.lower():
             raise VssError(f'Instance is already on {storage_type}')
         # validate storage type
         storage_type = self.validate_vm_storage_type(storage_type)
         # make the post
         rv = self.request(
-            f'/vm/{vm_id}/storage-type/{storage_type}', method=self.PUT
+            f'/vm/{vm_id}/storage-type/{storage_type}',
+            method=self.PUT,
+            payload=kwargs,
         )
         return rv.get('data')
 
     # Virtual Machine Configuration
     def get_vm_boot(self, vm_id):
         """Get given Virtual Machine boot configuration.
 
@@ -2894,14 +2899,15 @@
         :return: object
 
         Configuration includes:
 
         - enter_bios_setup
         - boot_retry_delayMs
         - boot_delay_ms
+        - secure_boot
 
         .. note:: more information about required attributes available in
           `Virtual Machine Attributes
           <https://vss-wiki.eis.utoronto.ca/x/5ACC>`__
 
         """
         json = self.request(f'/vm/{vm_id}/boot')
@@ -5774,14 +5780,61 @@
         :param vm_id: virtual machine moref or uuid
         :type vm_id: str
         :return: change request object
         """
         json = self.request(f'/vm/{vm_id}/cpu/config')
         return json.get('data')
 
+    def update_vm_secure_boot(self, vm_id, value, **kwargs):
+        """Update Virtual Machine secure boot configuration.
+
+        :param vm_id: virtual machine moref or uuid
+        :type vm_id: str
+        :param value: Enable or disable hot add
+        :type value: bool
+        :return: change request object
+
+        .. note:: keyword arguments include schedule to process request
+          on a given date and time
+        """
+        payload = {"value": bool(value)}
+        payload.update(kwargs)
+        rv = self.request(
+            f'/vm/{vm_id}/boot/secure',
+            payload=payload,
+            method=self.PUT,
+        )
+        return rv.get('data')
+
+    def enable_vm_secure_boot(self, vm_id, **kwargs):
+        """Enable vm secure boot.
+
+        :param vm_id: virtual machine moref or uuid
+        :type vm_id: str
+        :param kwargs:
+        :return: change request object
+
+        .. note:: keyword arguments include schedule to process request
+          on a given date and time
+        """
+        return self.update_vm_secure_boot(vm_id, True, **kwargs)
+
+    def disable_vm_secure_boot(self, vm_id, **kwargs):
+        """Enable vm secure boot.
+
+        :param vm_id: virtual machine moref or uuid
+        :type vm_id: str
+        :param kwargs:
+        :return: change request object
+
+        .. note:: keyword arguments include schedule to process request
+          on a given date and time
+        """
+        return self.update_vm_secure_boot(vm_id, False, **kwargs)
+
     def update_vm_cpu_hot_add(self, vm_id, hot_add, **kwargs):
         """Update Virtual Machine CPU hot add configuration.
 
         :param vm_id: virtual machine moref or uuid
         :type vm_id: str
         :param hot_add: Enable or disable hot add
         :type hot_add: bool
```

### Comparing `pyvss-2023.2.0/pyvss.egg-info/PKG-INFO` & `pyvss-2023.2.1/pyvss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyvss
-Version: 2023.2.0
+Version: 2023.2.1
 Summary: ITS Private Cloud Python Client
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/py-vss
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/py-vss/archive/2023.2.0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/py-vss/archive/2023.2.1.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/py-vss/issues
 Project-URL: Documentation, https://eis.utorotno.ca/~vss/py-vss/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/py-vss
```

### Comparing `pyvss-2023.2.0/setup.cfg` & `pyvss-2023.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyvss-2023.2.0/setup.py` & `pyvss-2023.2.1/setup.py`

 * *Files identical despite different names*

