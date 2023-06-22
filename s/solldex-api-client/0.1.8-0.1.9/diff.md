# Comparing `tmp/solldex-api-client-0.1.8.tar.gz` & `tmp/solldex-api-client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solldex-api-client-0.1.8.tar", last modified: Fri Jun 16 12:44:13 2023, max compression
+gzip compressed data, was "solldex-api-client-0.1.9.tar", last modified: Fri Jun 16 13:49:59 2023, max compression
```

## Comparing `solldex-api-client-0.1.8.tar` & `solldex-api-client-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 12:44:13.993919 solldex-api-client-0.1.8/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.8/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 12:44:13.993774 solldex-api-client-0.1.8/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     3926 2023-06-16 03:21:01.000000 solldex-api-client-0.1.8/README.md
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-16 12:44:13.993970 solldex-api-client-0.1.8/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-16 12:44:09.000000 solldex-api-client-0.1.8/setup.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 12:44:13.992663 solldex-api-client-0.1.8/solldex_api/
--rw-r--r--   0 filterfeed   (501) staff       (20)      282 2023-06-16 12:43:54.000000 solldex-api-client-0.1.8/solldex_api/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     5233 2023-06-16 03:41:39.000000 solldex-api-client-0.1.8/solldex_api/solldex_api.py
--rw-r--r--   0 filterfeed   (501) staff       (20)     1647 2023-06-16 02:37:39.000000 solldex-api-client-0.1.8/solldex_api/solldex_models.py
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 12:44:13.993520 solldex-api-client-0.1.8/solldex_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 12:44:13.000000 solldex-api-client-0.1.8/solldex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      316 2023-06-16 12:44:13.000000 solldex-api-client-0.1.8/solldex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-16 12:44:13.000000 solldex-api-client-0.1.8/solldex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-16 12:44:13.000000 solldex-api-client-0.1.8/solldex_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-16 12:44:13.000000 solldex-api-client-0.1.8/solldex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 13:49:59.095599 solldex-api-client-0.1.9/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1067 2023-06-15 16:36:24.000000 solldex-api-client-0.1.9/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 13:49:59.095423 solldex-api-client-0.1.9/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     3926 2023-06-16 03:21:01.000000 solldex-api-client-0.1.9/README.md
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-06-16 13:49:59.095694 solldex-api-client-0.1.9/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-06-16 13:49:29.000000 solldex-api-client-0.1.9/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 13:49:59.094312 solldex-api-client-0.1.9/solldex_api/
+-rw-r--r--   0 filterfeed   (501) staff       (20)      282 2023-06-16 12:43:54.000000 solldex-api-client-0.1.9/solldex_api/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5233 2023-06-16 03:41:39.000000 solldex-api-client-0.1.9/solldex_api/solldex_api.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1651 2023-06-16 13:44:43.000000 solldex-api-client-0.1.9/solldex_api/solldex_models.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-06-16 13:49:59.095161 solldex-api-client-0.1.9/solldex_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     5347 2023-06-16 13:49:59.000000 solldex-api-client-0.1.9/solldex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      316 2023-06-16 13:49:59.000000 solldex-api-client-0.1.9/solldex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-06-16 13:49:59.000000 solldex-api-client-0.1.9/solldex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       18 2023-06-16 13:49:59.000000 solldex-api-client-0.1.9/solldex_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       12 2023-06-16 13:49:59.000000 solldex-api-client-0.1.9/solldex_api_client.egg-info/top_level.txt
```

### Comparing `solldex-api-client-0.1.8/LICENSE` & `solldex-api-client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.8/PKG-INFO` & `solldex-api-client-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
```

### Comparing `solldex-api-client-0.1.8/README.md` & `solldex-api-client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.8/setup.py` & `solldex-api-client-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='solldex-api-client',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     url='https://github.com/filterfeed/solldex-api-client',
     author='Victor Figueredo',  # replace with your name
     author_email='cto@filterfeed.com.br',
     description='Python client for the Solldex API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

### Comparing `solldex-api-client-0.1.8/solldex_api/solldex_api.py` & `solldex-api-client-0.1.9/solldex_api/solldex_api.py`

 * *Files identical despite different names*

### Comparing `solldex-api-client-0.1.8/solldex_api/solldex_models.py` & `solldex-api-client-0.1.9/solldex_api/solldex_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     codigo_municipio: Optional[int] = None
     endereco: Optional[Endereco] = None
     inscricao_municipal: Optional[int] = None
 
 
 @dataclass
 class Servico:
-    aliquota: int
+    aliquota: float
     discriminacao: str
     iss_retido: bool
     item_lista_servico: int
     codigo_tributario_municipio: int
-    valor_servicos: int
+    valor_servicos: float
 
 
 @dataclass
 class RecepcionarLoteParams:
     data_emissao: str
     prestador: Prestador
     tomador: Tomador
```

### Comparing `solldex-api-client-0.1.8/solldex_api_client.egg-info/PKG-INFO` & `solldex-api-client-0.1.9/solldex_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solldex-api-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client for the Solldex API
 Home-page: https://github.com/filterfeed/solldex-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # SolldexAPI Python Client
```

