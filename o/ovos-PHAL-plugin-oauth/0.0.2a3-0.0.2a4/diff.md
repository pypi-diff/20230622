# Comparing `tmp/ovos-PHAL-plugin-oauth-0.0.2a3.tar.gz` & `tmp/ovos-PHAL-plugin-oauth-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-oauth-0.0.2a3.tar", last modified: Wed Jun 21 16:13:23 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-oauth-0.0.2a4.tar", last modified: Wed Jun 21 19:41:43 2023, max compression
```

## Comparing `ovos-PHAL-plugin-oauth-0.0.2a3.tar` & `ovos-PHAL-plugin-oauth-0.0.2a4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:13:23.126564 ovos-PHAL-plugin-oauth-0.0.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 16:13:23.126564 ovos-PHAL-plugin-oauth-0.0.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-21 16:13:12.000000 ovos-PHAL-plugin-oauth-0.0.2a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:13:23.122564 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth/
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-21 16:13:12.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 16:13:15.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:13:23.122564 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-21 16:13:23.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:13:22.000000 ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:13:23.126564 ovos-PHAL-plugin-oauth-0.0.2a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-21 16:13:12.000000 ovos-PHAL-plugin-oauth-0.0.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:43.951971 ovos-PHAL-plugin-oauth-0.0.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-21 19:41:43.951971 ovos-PHAL-plugin-oauth-0.0.2a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-21 19:41:40.000000 ovos-PHAL-plugin-oauth-0.0.2a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:43.951971 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-21 19:41:40.000000 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 19:41:40.000000 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:43.951971 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-21 19:41:43.000000 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-21 19:41:43.000000 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:43.000000 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 19:41:43.000000 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-21 19:41:43.000000 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 19:41:43.000000 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:43.000000 ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:41:43.951971 ovos-PHAL-plugin-oauth-0.0.2a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2998 2023-06-21 19:41:40.000000 ovos-PHAL-plugin-oauth-0.0.2a4/setup.py
```

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a3/README.md` & `ovos-PHAL-plugin-oauth-0.0.2a4/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a3/ovos_PHAL_plugin_oauth/__init__.py` & `ovos-PHAL-plugin-oauth-0.0.2a4/ovos_PHAL_plugin_oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-oauth-0.0.2a3/setup.py` & `ovos-PHAL-plugin-oauth-0.0.2a4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,30 +35,39 @@
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join('..', path, filename))
     return paths
 
 
+def get_description():
+    with open(os.path.join(BASEDIR, "README.md"), "r") as f:
+        long_description = f.read()
+    return long_description
+
+
 def required(requirements_file):
     """ Read requirements file and remove comments and empty lines. """
     with open(os.path.join(BASEDIR, requirements_file), 'r') as f:
         requirements = f.read().splitlines()
         if 'MYCROFT_LOOSE_REQUIREMENTS' in os.environ:
             print('USING LOOSE REQUIREMENTS!')
-            requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
+            requirements = [r.replace('==', '>=').replace('~=', '>=')
+                            for r in requirements]
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
 
 PLUGIN_ENTRY_POINT = 'ovos-PHAL-plugin-oauth=ovos_PHAL_plugin_oauth:OAuthPlugin'
 setup(
     name='ovos-PHAL-plugin-oauth',
     version=get_version(),
     description='A plugin for OpenVoiceOS hardware abstraction layer',
+    long_description=get_description(),
+    long_description_content_type="text/markdown",
     url='https://github.com/OpenVoiceOS/ovos-PHAL-plugin-oauth',
     author='JarbasAi',
     author_email='jarbasai@mailfence.com',
     license='Apache-2.0',
     packages=['ovos_PHAL_plugin_oauth'],
     package_data={'': package_files('ovos_PHAL_plugin_oauth')},
     install_requires=required("requirements.txt"),
```

