# Comparing `tmp/mse_cli_core-0.1a5.tar.gz` & `tmp/mse_cli_core-0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_cli_core-0.1a5.tar", last modified: Tue Jun 20 16:40:42 2023, max compression
+gzip compressed data, was "mse_cli_core-0.1a6.tar", last modified: Thu Jun 22 08:32:31 2023, max compression
```

## Comparing `mse_cli_core-0.1a5.tar` & `mse_cli_core-0.1a6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.255714 mse_cli_core-0.1a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/src/mse_cli_core/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/clock_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/enclave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/src/mse_cli_core/test_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:40:42.000000 mse_cli_core-0.1a5/src/mse_cli_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:40:42.259714 mse_cli_core-0.1a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_boostrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-20 16:40:12.000000 mse_cli_core-0.1a5/tests/test_test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.286998 mse_cli_core-0.1a6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.286998 mse_cli_core-0.1a6/src/mse_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/clock_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/src/mse_cli_core/test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:32:31.000000 mse_cli_core-0.1a6/src/mse_cli_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:32:31.290998 mse_cli_core-0.1a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_boostrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-22 08:31:56.000000 mse_cli_core-0.1a6/tests/test_test_docker.py
```

### Comparing `mse_cli_core-0.1a5/PKG-INFO` & `mse_cli_core-0.1a6/src/mse_cli_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mse_cli_core
-Version: 0.1a5
+Name: mse-cli-core
+Version: 0.1a6
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a5/setup.cfg` & `mse_cli_core-0.1a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/setup.py` & `mse_cli_core-0.1a6/setup.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/base64.py` & `mse_cli_core-0.1a6/src/mse_cli_core/base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/bootstrap.py` & `mse_cli_core-0.1a6/src/mse_cli_core/bootstrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 def is_waiting_for_secrets(url: str, verify: Union[bool, str] = True) -> bool:
     """Check whether the configuration server is up."""
     try:
         response = requests.get(url=url, verify=verify, timeout=5)
 
         if response.status_code == 200 and "Mse-Status" in response.headers:
             return True
+    except requests.exceptions.Timeout:
+        return False
     except requests.exceptions.SSLError:
         return False
     except requests.exceptions.ConnectionError:
         return False
 
     return False
 
@@ -114,13 +116,15 @@
             url=f"{url}{healthcheck_endpoint}",
             verify=verify,
             timeout=5,
         )
 
         if response.status_code != 503 and "Mse-Status" not in response.headers:
             return True
+    except requests.exceptions.Timeout:
+        return False
     except requests.exceptions.SSLError:
         return False
     except requests.exceptions.ConnectionError:
         return False
 
     return False
```

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/clock_tick.py` & `mse_cli_core-0.1a6/src/mse_cli_core/clock_tick.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/enclave.py` & `mse_cli_core-0.1a6/src/mse_cli_core/enclave.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     """MR signer does not matched with the expected value."""
 
 
 def compute_mr_enclave(
     client: DockerClient,
     image: str,
     app_args: NoSgxDockerConfig,
-    code_tar_path: Path,
+    app_path: Path,
     docker_path_log: Path,
 ) -> str:
     """Compute the MR enclave."""
     container = client.containers.run(
         image,
         command=app_args.cmd(),
-        volumes=app_args.volumes(code_tar_path),
+        volumes=app_args.volumes(app_path),
         entrypoint=NoSgxDockerConfig.entrypoint,
         remove=True,
         detach=False,
         stdout=True,
         stderr=True,
     )
```

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/fs.py` & `mse_cli_core-0.1a6/src/mse_cli_core/fs.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/ignore_file.py` & `mse_cli_core-0.1a6/src/mse_cli_core/ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/no_sgx_docker.py` & `mse_cli_core-0.1a6/src/mse_cli_core/no_sgx_docker.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,60 +15,46 @@
     host: str
     expiration_date: Optional[int]
     app_cert: Optional[Path]
     size: int
     app_id: UUID
     application: str
 
-    code_mountpoint: ClassVar[str] = "/tmp/app.tar"
-    app_cert_mountpoint: ClassVar[str] = "/tmp/cert.pem"
+    app_mountpoint: ClassVar[str] = "/opt/input"
     entrypoint: ClassVar[str] = "mse-run"
 
     def cmd(self) -> List[str]:
         """Serialize the docker command args."""
         command = [
             "--size",
             f"{self.size}M",
-            "--code",
-            NoSgxDockerConfig.code_mountpoint,
             "--san",
             str(self.host),
             "--id",
             str(self.app_id),
             "--application",
             self.application,
             "--dry-run",
         ]
 
-        if self.app_cert:
-            command.append("--certificate")
-            command.append(NoSgxDockerConfig.app_cert_mountpoint)
-        else:
-            command.append("--ratls")
+        if not self.app_cert:
+            command.append("--expiration")
             command.append(str(self.expiration_date))
 
         return command
 
-    def volumes(self, code_tar_path: Path) -> Dict[str, Dict[str, str]]:
+    def volumes(self, app_path: Path) -> Dict[str, Dict[str, str]]:
         """Define the docker volumes."""
-        v = {
-            f"{code_tar_path.resolve()}": {
-                "bind": NoSgxDockerConfig.code_mountpoint,
+        return {
+            f"{app_path.resolve()}": {
+                "bind": NoSgxDockerConfig.app_mountpoint,
                 "mode": "rw",
             }
         }
 
-        if self.app_cert:
-            v[f"{self.app_cert.resolve()}"] = {
-                "bind": NoSgxDockerConfig.app_cert_mountpoint,
-                "mode": "rw",
-            }
-
-        return v
-
     @staticmethod
     def from_sgx(docker_config: SgxDockerConfig):
         """Load from a SgxDockerConfig object."""
         return NoSgxDockerConfig(
             host=docker_config.host,
             expiration_date=docker_config.expiration_date,
             size=docker_config.size,
```

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/sgx_docker.py` & `mse_cli_core-0.1a6/src/mse_cli_core/sgx_docker.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,38 +11,36 @@
     """Definition of an mse docker running on a SGX hardware."""
 
     size: int
     host: str
     port: int
     app_id: UUID
     expiration_date: int
-    code: Path
+    app_dir: Path
     application: str
     healthcheck: str
     signer_key: Path
 
     signer_key_mountpoint: ClassVar[str] = "/root/.config/gramine/enclave-key.pem"
-    code_mountpoint: ClassVar[str] = "/tmp/app.tar"
+    app_mountpoint: ClassVar[str] = "/opt/input"
     docker_label: ClassVar[str] = "mse-home"
     entrypoint: ClassVar[str] = "mse-run"
 
     def cmd(self) -> List[str]:
         """Serialize the docker command args."""
         return [
             "--size",
             f"{self.size}M",
-            "--code",
-            SgxDockerConfig.code_mountpoint,
             "--san",
             str(self.host),
             "--id",
             str(self.app_id),
             "--application",
             self.application,
-            "--ratls",
+            "--expiration",
             str(self.expiration_date),
         ]
 
     def ports(self) -> Dict[str, Tuple[str, str]]:
         """Define the docker ports."""
         return {"443/tcp": ("127.0.0.1", str(self.port))}
 
@@ -52,16 +50,16 @@
             SgxDockerConfig.docker_label: "1",
             "healthcheck_endpoint": self.healthcheck,
         }
 
     def volumes(self) -> Dict[str, Dict[str, str]]:
         """Define the docker volumes."""
         return {
-            f"{self.code.resolve()}": {
-                "bind": SgxDockerConfig.code_mountpoint,
+            f"{self.app_dir.resolve()}": {
+                "bind": SgxDockerConfig.app_mountpoint,
                 "mode": "rw",
             },
             "/var/run/aesmd": {"bind": "/var/run/aesmd", "mode": "rw"},
             f"{self.signer_key.resolve()}": {
                 "bind": SgxDockerConfig.signer_key_mountpoint,
                 "mode": "rw",
             },
@@ -87,17 +85,17 @@
         signer_key = next(
             filter(
                 lambda mount: mount["Destination"]
                 == SgxDockerConfig.signer_key_mountpoint,
                 docker_attrs["Mounts"],
             )
         )
-        code = next(
+        app = next(
             filter(
-                lambda mount: mount["Destination"] == SgxDockerConfig.code_mountpoint,
+                lambda mount: mount["Destination"] == SgxDockerConfig.app_mountpoint,
                 docker_attrs["Mounts"],
             )
         )
 
         i = 0
         while i < len(cmd):
             key = cmd[i][2:]
@@ -114,14 +112,14 @@
             dataMap[key] = cmd[i + 1]
             i += 2
 
         return SgxDockerConfig(
             size=int(dataMap["size"][:-1]),
             host=dataMap["san"],
             app_id=UUID(dataMap["id"]),
-            expiration_date=int(dataMap["ratls"]),
-            code=Path(code["Source"]),
+            expiration_date=int(dataMap["expiration"]),
+            app_dir=Path(app["Source"]),
             application=dataMap["application"],
             port=int(port["443/tcp"][0]["HostPort"]),
             healthcheck=docker_labels["healthcheck_endpoint"],
             signer_key=Path(signer_key["Source"]),
         )
```

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/spinner.py` & `mse_cli_core-0.1a6/src/mse_cli_core/spinner.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core/test_docker.py` & `mse_cli_core-0.1a6/src/mse_cli_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core.egg-info/PKG-INFO` & `mse_cli_core-0.1a6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mse-cli-core
-Version: 0.1a5
+Name: mse_cli_core
+Version: 0.1a6
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a5/src/mse_cli_core.egg-info/SOURCES.txt` & `mse_cli_core-0.1a6/src/mse_cli_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/tests/test_base64.py` & `mse_cli_core-0.1a6/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/tests/test_boostrap.py` & `mse_cli_core-0.1a6/tests/test_boostrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/tests/test_ignore_file.py` & `mse_cli_core-0.1a6/tests/test_ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a5/tests/test_no_sgx_docker.py` & `mse_cli_core-0.1a6/tests/test_no_sgx_docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     conf = NoSgxDockerConfig.from_sgx(
         SgxDockerConfig(
             size=4096,
             host="localhost",
             port=7788,
             app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
             expiration_date=1714058115,
-            code="/home/cosmian/workspace/sgx_operator/code.tar",
+            app_dir="/home/cosmian/workspace/sgx_operator/",
             application="app:app",
             healthcheck="/health",
             signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
         )
     )
 
     assert conf == ref_conf
@@ -39,38 +39,34 @@
         host="localhost",
         expiration_date=1714058115,
         size=4096,
         app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
         application="app:app",
     )
 
-    assert ref_conf.volumes(Path("/tmp/code.tar")) == {
-        "/tmp/code.tar": {
-            "bind": "/tmp/app.tar",
+    assert ref_conf.volumes(Path("/tmp/")) == {
+        "/tmp": {
+            "bind": "/opt/input",
             "mode": "rw",
         }
     }
 
     ref_conf = NoSgxDockerConfig(
         host="localhost",
         app_cert="/app/cert.pem",
         size=4096,
         app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
         application="app:app",
     )
 
-    assert ref_conf.volumes(Path("/tmp/code.tar")) == {
-        "/tmp/code.tar": {
-            "bind": "/tmp/app.tar",
+    assert ref_conf.volumes(Path("/tmp/")) == {
+        "/tmp": {
+            "bind": "/opt/input",
             "mode": "rw",
-        },
-        "/app/cert.pem": {
-            "bind": "/tmp/cert.pem",
-            "mode": "rw",
-        },
+        }
     }
 
 
 def test_cmd():
     """Test `cmd` function."""
     ref_conf = NoSgxDockerConfig(
         host="localhost",
@@ -79,43 +75,37 @@
         app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
         application="app:app",
     )
 
     assert ref_conf.cmd() == [
         "--size",
         "4096M",
-        "--code",
-        "/tmp/app.tar",
         "--san",
         "localhost",
         "--id",
         "63322f85-1ff8-4483-91ae-f18d7398d157",
         "--application",
         "app:app",
         "--dry-run",
-        "--ratls",
+        "--expiration",
         "1714058115",
     ]
 
     ref_conf = NoSgxDockerConfig(
         host="localhost",
         app_cert="cert.pem",
         size=4096,
         app_id="63322f85-1ff8-4483-91ae-f18d7398d157",
         application="app:app",
     )
 
     assert ref_conf.cmd() == [
         "--size",
         "4096M",
-        "--code",
-        "/tmp/app.tar",
         "--san",
         "localhost",
         "--id",
         "63322f85-1ff8-4483-91ae-f18d7398d157",
         "--application",
         "app:app",
         "--dry-run",
-        "--certificate",
-        "/tmp/cert.pem",
     ]
```

### Comparing `mse_cli_core-0.1a5/tests/test_sgx_docker.py` & `mse_cli_core-0.1a6/tests/test_sgx_docker.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Test `load` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
         host="myapp.fr",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
         expiration_date=1714639412,
-        code="/home/cosmian/workspace/sgx_operator/code.tar",
+        app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
     conf = SgxDockerConfig.load(
         docker_labels={"healthcheck_endpoint": "/health", "mse-home": "1"},
@@ -26,39 +26,37 @@
                     "443/tcp": [{"HostIp": "127.0.0.1", "HostPort": "7788"}]
                 },
             },
             "Config": {
                 "Cmd": [
                     "--size",
                     "4096M",
-                    "--code",
-                    "/tmp/app.tar",
                     "--san",
                     "myapp.fr",
                     "--id",
                     "4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
                     "--application",
                     "app:app",
-                    "--ratls",
+                    "--expiration",
                     "1714639412",
                 ],
             },
             "Mounts": [
                 {
                     "Type": "bind",
                     "Source": "/opt/cosmian-internal/cosmian-signer-key.pem",
                     "Destination": "/root/.config/gramine/enclave-key.pem",
                     "Mode": "rw",
                     "RW": True,
                     "Propagation": "rprivate",
                 },
                 {
                     "Type": "bind",
-                    "Source": "/home/cosmian/workspace/sgx_operator/code.tar",
-                    "Destination": "/tmp/app.tar",
+                    "Source": "/home/cosmian/workspace/sgx_operator/",
+                    "Destination": "/opt/input",
                     "Mode": "rw",
                     "RW": True,
                     "Propagation": "rprivate",
                 },
                 {
                     "Type": "bind",
                     "Source": "/var/run/aesmd",
@@ -78,15 +76,15 @@
     """Test `labels` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
         host="myapp.fr",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
         expiration_date=1714639412,
-        code="/home/cosmian/workspace/sgx_operator/code.tar",
+        app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
     assert ref_conf.labels() == {"mse-home": "1", "healthcheck_endpoint": "/health"}
 
@@ -95,15 +93,15 @@
     """Test `devices` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
         host="myapp.fr",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
         expiration_date=1714639412,
-        code="/home/cosmian/workspace/sgx_operator/code.tar",
+        app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
     assert ref_conf.devices() == [
         "/dev/sgx_enclave:/dev/sgx_enclave:rw",
@@ -117,15 +115,15 @@
     """Test `ports` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
         host="myapp.fr",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
         expiration_date=1714639412,
-        code="/home/cosmian/workspace/sgx_operator/code.tar",
+        app_dir="/home/cosmian/workspace/sgx_operator/code.tar",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
     assert ref_conf.ports() == {"443/tcp": ("127.0.0.1", "7788")}
 
@@ -134,27 +132,27 @@
     """Test `volumes` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
         host="myapp.fr",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
         expiration_date=1714639412,
-        code="/home/cosmian/workspace/sgx_operator/code.tar",
+        app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
     assert ref_conf.volumes() == {
         "/opt/cosmian-internal/cosmian-signer-key.pem": {
             "bind": "/root/.config/gramine/enclave-key.pem",
             "mode": "rw",
         },
-        "/home/cosmian/workspace/sgx_operator/code.tar": {
-            "bind": "/tmp/app.tar",
+        "/home/cosmian/workspace/sgx_operator": {
+            "bind": "/opt/input",
             "mode": "rw",
         },
         "/var/run/aesmd": {
             "bind": "/var/run/aesmd",
             "mode": "rw",
         },
     }
@@ -164,27 +162,25 @@
     """Test `cmd` function."""
     ref_conf = SgxDockerConfig(
         size=4096,
         host="myapp.fr",
         port=7788,
         app_id="4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
         expiration_date=1714639412,
-        code="/home/cosmian/workspace/sgx_operator/code.tar",
+        app_dir="/home/cosmian/workspace/sgx_operator/",
         application="app:app",
         healthcheck="/health",
         signer_key="/opt/cosmian-internal/cosmian-signer-key.pem",
     )
 
     assert ref_conf.cmd() == [
         "--size",
         "4096M",
-        "--code",
-        "/tmp/app.tar",
         "--san",
         "myapp.fr",
         "--id",
         "4141a3e6-1f2b-4ccf-8610-aa0891a1a210",
         "--application",
         "app:app",
-        "--ratls",
+        "--expiration",
         "1714639412",
     ]
```

### Comparing `mse_cli_core-0.1a5/tests/test_test_docker.py` & `mse_cli_core-0.1a6/tests/test_test_docker.py`

 * *Files identical despite different names*

