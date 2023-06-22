# Comparing `tmp/ccstorage-1.1.tar.gz` & `tmp/ccstorage-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccstorage-1.1.tar", last modified: Fri Aug  5 07:51:34 2022, max compression
+gzip compressed data, was "ccstorage-1.2.tar", last modified: Thu Jun 22 12:58:41 2023, max compression
```

## Comparing `ccstorage-1.1.tar` & `ccstorage-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 openthread   (502) staff       (20)        0 2022-08-05 07:51:34.551051 ccstorage-1.1/
--rw-r--r--   0 openthread   (502) staff       (20)     1402 2022-08-05 07:51:34.550935 ccstorage-1.1/PKG-INFO
--rw-r--r--   0 openthread   (502) staff       (20)      848 2022-08-05 07:50:35.000000 ccstorage-1.1/README.md
-drwxr-xr-x   0 openthread   (502) staff       (20)        0 2022-08-05 07:51:34.550296 ccstorage-1.1/ccstorage/
--rw-r--r--   0 openthread   (502) staff       (20)     2223 2022-08-05 07:35:09.000000 ccstorage-1.1/ccstorage/__init__.py
-drwxr-xr-x   0 openthread   (502) staff       (20)        0 2022-08-05 07:51:34.550780 ccstorage-1.1/ccstorage.egg-info/
--rw-r--r--   0 openthread   (502) staff       (20)     1402 2022-08-05 07:51:34.000000 ccstorage-1.1/ccstorage.egg-info/PKG-INFO
--rw-r--r--   0 openthread   (502) staff       (20)      204 2022-08-05 07:51:34.000000 ccstorage-1.1/ccstorage.egg-info/SOURCES.txt
--rw-r--r--   0 openthread   (502) staff       (20)        1 2022-08-05 07:51:34.000000 ccstorage-1.1/ccstorage.egg-info/dependency_links.txt
--rw-r--r--   0 openthread   (502) staff       (20)        1 2022-08-05 07:51:29.000000 ccstorage-1.1/ccstorage.egg-info/not-zip-safe
--rw-r--r--   0 openthread   (502) staff       (20)       10 2022-08-05 07:51:34.000000 ccstorage-1.1/ccstorage.egg-info/top_level.txt
--rw-r--r--   0 openthread   (502) staff       (20)       38 2022-08-05 07:51:34.551089 ccstorage-1.1/setup.cfg
--rw-r--r--   0 openthread   (502) staff       (20)      700 2022-08-05 07:51:09.000000 ccstorage-1.1/setup.py
+drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-06-22 12:58:41.199245 ccstorage-1.2/
+-rw-r--r--   0 openthread   (501) staff       (20)     1127 2023-06-22 12:58:41.199143 ccstorage-1.2/PKG-INFO
+-rw-r--r--   0 openthread   (501) staff       (20)      848 2023-06-22 12:43:06.000000 ccstorage-1.2/README.md
+drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-06-22 12:58:41.198366 ccstorage-1.2/ccstorage/
+-rw-r--r--   0 openthread   (501) staff       (20)     2413 2023-06-22 12:43:22.000000 ccstorage-1.2/ccstorage/__init__.py
+drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-06-22 12:58:41.199007 ccstorage-1.2/ccstorage.egg-info/
+-rw-r--r--   0 openthread   (501) staff       (20)     1127 2023-06-22 12:58:41.000000 ccstorage-1.2/ccstorage.egg-info/PKG-INFO
+-rw-r--r--   0 openthread   (501) staff       (20)      204 2023-06-22 12:58:41.000000 ccstorage-1.2/ccstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 openthread   (501) staff       (20)        1 2023-06-22 12:58:41.000000 ccstorage-1.2/ccstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 openthread   (501) staff       (20)        1 2023-06-22 12:58:41.000000 ccstorage-1.2/ccstorage.egg-info/not-zip-safe
+-rw-r--r--   0 openthread   (501) staff       (20)       10 2023-06-22 12:58:41.000000 ccstorage-1.2/ccstorage.egg-info/top_level.txt
+-rw-r--r--   0 openthread   (501) staff       (20)       38 2023-06-22 12:58:41.199275 ccstorage-1.2/setup.cfg
+-rw-r--r--   0 openthread   (501) staff       (20)      700 2023-06-22 12:43:41.000000 ccstorage-1.2/setup.py
```

### Comparing `ccstorage-1.1/README.md` & `ccstorage-1.2/README.md`

 * *Files identical despite different names*

### Comparing `ccstorage-1.1/ccstorage/__init__.py` & `ccstorage-1.2/ccstorage/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,18 @@
                 if isinstance(result, dict):
                     self.__storage_dict = result
                     return True
             except Exception as e:
                 print('ccstorage read exception: ', e)
         return False
 
+    def resort(self, key: str, reverse: bool):
+        sorted_data = sorted(self.__storage_dict.items(), key=lambda x: x[1][key], reverse=reverse)
+        self.__storage_dict = sorted_data
+
     def __setitem__(self, key: str, value: Union[str, float, dict, list, None]) -> None:
         if self.force_reload_at_data_access is True:
             self.read()
         if value is None:
             self.__storage_dict.pop(key, None)
         else:
             self.__storage_dict[key] = value
```

### Comparing `ccstorage-1.1/setup.py` & `ccstorage-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                 lst = f.read()
                 return lst
         else:
             return None
 
 
 setup(name='ccstorage',
-      version='1.1',
+      version='1.2',
       description='Local storage: CCStorage, and simple local file string read/write: CCIO',
       long_description=READMarkDown.read_string(),
       long_description_content_type='text/markdown',
       url='',
       author='OpenFibers',
       author_email='openfibers@gmail.com',
       license='MIT',
```

