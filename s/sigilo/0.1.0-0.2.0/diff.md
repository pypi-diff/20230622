# Comparing `tmp/sigilo-0.1.0.tar.gz` & `tmp/sigilo-0.2.0.tar.gz`

## Comparing `sigilo-0.1.0.tar` & `sigilo-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 sigilo-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 sigilo-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 sigilo-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sigilo-0.1.0/docs/api.rst
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 sigilo-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 sigilo-0.1.0/docs/contributing.rst
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 sigilo-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 sigilo-0.1.0/sigilo/__init__.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sigilo-0.1.0/sigilo/ciphers/__init__.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 sigilo-0.1.0/sigilo/ciphers/fernet.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sigilo-0.1.0/sigilo/ciphers/plain.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sigilo-0.1.0/sigilo/stores/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 sigilo-0.1.0/sigilo/stores/memory.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 sigilo-0.1.0/sigilo/stores/redis.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 sigilo-0.1.0/tests/test_cipher_fernet.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 sigilo-0.1.0/tests/test_sigilo.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 sigilo-0.1.0/tests/test_store_redis.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 sigilo-0.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sigilo-0.1.0/LICENSE
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 sigilo-0.1.0/README.md
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sigilo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 sigilo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 sigilo-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 sigilo-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 sigilo-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sigilo-0.2.0/docs/api.rst
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 sigilo-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 sigilo-0.2.0/docs/contributing.rst
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 sigilo-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 sigilo-0.2.0/sigilo/__init__.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sigilo-0.2.0/sigilo/ciphers/__init__.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 sigilo-0.2.0/sigilo/ciphers/fernet.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sigilo-0.2.0/sigilo/ciphers/plain.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sigilo-0.2.0/sigilo/stores/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 sigilo-0.2.0/sigilo/stores/memcache.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 sigilo-0.2.0/sigilo/stores/memory.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 sigilo-0.2.0/sigilo/stores/redis.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 sigilo-0.2.0/tests/test_cipher_fernet.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 sigilo-0.2.0/tests/test_sigilo.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sigilo-0.2.0/tests/test_store_memcache.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 sigilo-0.2.0/tests/test_store_redis.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 sigilo-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sigilo-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 sigilo-0.2.0/README.md
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 sigilo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 sigilo-0.2.0/PKG-INFO
```

### Comparing `sigilo-0.1.0/.github/workflows/test.yml` & `sigilo-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sigilo-0.1.0/docs/api.rst` & `sigilo-0.2.0/docs/api.rst`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 
 .. autoclass:: MemoryStore
 
 .. module:: sigilo.stores.redis
 
 .. autoclass:: RedisStore
 
+.. module:: sigilo.stores.memcache
+
+.. autoclass:: MemcacheStore
+
 Ciphers
 ------
 
 .. module:: sigilo.ciphers
 
 .. autoclass:: Cipher
```

### Comparing `sigilo-0.1.0/docs/conf.py` & `sigilo-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sigilo-0.1.0/docs/contributing.rst` & `sigilo-0.2.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sigilo-0.1.0/docs/index.rst` & `sigilo-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sigilo-0.1.0/sigilo/__init__.py` & `sigilo-0.2.0/sigilo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 from .ciphers import Cipher
 from .stores import Store
 
 
 class Sigilo:
     """Teste"""
```

### Comparing `sigilo-0.1.0/tests/test_sigilo.py` & `sigilo-0.2.0/tests/test_sigilo.py`

 * *Files identical despite different names*

### Comparing `sigilo-0.1.0/LICENSE` & `sigilo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sigilo-0.1.0/README.md` & `sigilo-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Sigilo 🤫
 
 [![Documentation](https://readthedocs.org/projects/sigilo/badge/)](https://sigilo.readthedocs.io/en/latest/)
+[![PyPI](https://img.shields.io/pypi/v/sigilo)](https://pypi.org/project/sigilo/)
 ![GitHub](https://img.shields.io/github/license/ecarrara/sigilo)
 
 Sigilo provides a secure way to store and retrieve sensitive information like
 passwords, OAuth access tokens, credit card numbers, etc.
 
 For example, to store a secret on [redis](https://redis.io/) using
 sigilo.Sigilo:
```

### Comparing `sigilo-0.1.0/pyproject.toml` & `sigilo-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,42 +21,47 @@
 [project.optional-dependencies]
 redis = [
   "redis"
 ]
 cryptography = [
   "cryptography"
 ]
+pymemcache = [
+  "pymemcache"
+]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 path = "sigilo/__init__.py"
 
 [tool.hatch.envs.test]
 dependencies = [
   "pytest",
   "pytest-cov",
   "redis",
-  "cryptography"
+  "cryptography",
+  "pymemcache"
 ]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.11", "3.10", "3.9", "3.8"]
 
 [tool.hatch.envs.test.scripts]
 cov = "pytest --cov=sigilo {args:tests}"
 
 [tool.hatch.envs.default]
 dependencies = [
   "black>=23.3",
   "pyright>=1.1",
   "ruff>=0.0.274",
   "redis",
+  "pymemcache",
   "cryptography",
   "pytest",
   "sphinx"
 ]
 
 [tool.hatch.envs.default.scripts]
 typing = "pyright {args:sigilo tests}"
```

### Comparing `sigilo-0.1.0/PKG-INFO` & `sigilo-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: sigilo
-Version: 0.1.0
+Version: 0.2.0
 Project-URL: Source, https://github.com/ecarrara/sigilo
 Project-URL: Issues, https://github.com/ecarrara/sigilo/issues
 Author-email: Erle Carrara <carrara.erle@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Provides-Extra: cryptography
 Requires-Dist: cryptography; extra == 'cryptography'
+Provides-Extra: pymemcache
+Requires-Dist: pymemcache; extra == 'pymemcache'
 Provides-Extra: redis
 Requires-Dist: redis; extra == 'redis'
 Description-Content-Type: text/markdown
 
 # Sigilo 🤫
 
 [![Documentation](https://readthedocs.org/projects/sigilo/badge/)](https://sigilo.readthedocs.io/en/latest/)
+[![PyPI](https://img.shields.io/pypi/v/sigilo)](https://pypi.org/project/sigilo/)
 ![GitHub](https://img.shields.io/github/license/ecarrara/sigilo)
 
 Sigilo provides a secure way to store and retrieve sensitive information like
 passwords, OAuth access tokens, credit card numbers, etc.
 
 For example, to store a secret on [redis](https://redis.io/) using
 sigilo.Sigilo:
```

