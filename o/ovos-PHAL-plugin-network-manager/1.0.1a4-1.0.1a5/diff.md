# Comparing `tmp/ovos-PHAL-plugin-network-manager-1.0.1a4.tar.gz` & `tmp/ovos-PHAL-plugin-network-manager-1.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-network-manager-1.0.1a4.tar", last modified: Wed Jun 21 16:12:11 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-network-manager-1.0.1a5.tar", last modified: Wed Jun 21 19:37:14 2023, max compression
```

## Comparing `ovos-PHAL-plugin-network-manager-1.0.1a4.tar` & `ovos-PHAL-plugin-network-manager-1.0.1a5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:11.919216 ovos-PHAL-plugin-network-manager-1.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 16:12:01.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-21 16:12:11.919216 ovos-PHAL-plugin-network-manager-1.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-21 16:12:01.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:11.919216 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-06-21 16:12:01.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 16:12:04.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:12:11.919216 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-21 16:12:11.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 16:12:11.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:12:11.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-21 16:12:11.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 16:12:11.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 16:12:11.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:12:11.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 16:12:11.919216 ovos-PHAL-plugin-network-manager-1.0.1a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-06-21 16:12:01.000000 ovos-PHAL-plugin-network-manager-1.0.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:14.559043 ovos-PHAL-plugin-network-manager-1.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-21 19:37:14.559043 ovos-PHAL-plugin-network-manager-1.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:14.555043 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:14.559043 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:37:14.559043 ovos-PHAL-plugin-network-manager-1.0.1a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3241 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/setup.py
```

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a4/LICENSE` & `ovos-PHAL-plugin-network-manager-1.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a4/README.md` & `ovos-PHAL-plugin-network-manager-1.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a4/ovos_PHAL_plugin_network_manager/__init__.py` & `ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a4/setup.py` & `ovos-PHAL-plugin-network-manager-1.0.1a5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 import os
 from setuptools import setup
 
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
+
 def get_version():
     """ Find the version of the package"""
     version = None
     version_file = os.path.join(BASEDIR, 'ovos_PHAL_plugin_network_manager', 'version.py')
     major, minor, build, alpha = (None, None, None, None)
     with open(version_file) as f:
         for line in f:
@@ -24,36 +25,47 @@
                     '# END_VERSION_BLOCK' in line):
                 break
     version = f"{major}.{minor}.{build}"
     if alpha and int(alpha) > 0:
         version += f"a{alpha}"
     return version
 
+
 def required(requirements_file):
     """ Read requirements file and remove comments and empty lines. """
     with open(os.path.join(BASEDIR, requirements_file), 'r') as f:
         requirements = f.read().splitlines()
         if 'MYCROFT_LOOSE_REQUIREMENTS' in os.environ:
             print('USING LOOSE REQUIREMENTS!')
             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
+
 def package_files(directory):
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join('..', path, filename))
     return paths
 
+
+def get_description():
+    with open(os.path.join(BASEDIR, "README.md"), "r") as f:
+        long_description = f.read()
+    return long_description
+
+
 PLUGIN_ENTRY_POINT = 'ovos-PHAL-plugin-network-manager=ovos_PHAL_plugin_network_manager:NetworkManagerPlugin'
 setup(
     name='ovos-PHAL-plugin-network-manager',
     version=get_version(),
     description='Network Manager plugin for OpenVoiceOS hardware abstraction layer',
+    long_description=get_description(),
+    long_description_content_type="text/markdown",
     url='https://github.com/OpenVoiceOS/ovos-PHAL-plugin-network-manager',
     author='Aiix',
     author_email='aix.m@outlook.com',
     license='Apache-2.0',
     packages=['ovos_PHAL_plugin_network_manager'],
     package_data={'': package_files('ovos_PHAL_plugin_network_manager')},
     install_requires=required("requirements.txt"),
```

