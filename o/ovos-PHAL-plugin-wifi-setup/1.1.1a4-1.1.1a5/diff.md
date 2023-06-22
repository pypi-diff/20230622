# Comparing `tmp/ovos-PHAL-plugin-wifi-setup-1.1.1a4.tar.gz` & `tmp/ovos-PHAL-plugin-wifi-setup-1.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.1a4.tar", last modified: Wed Jun 21 23:28:22 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.1a5.tar", last modified: Wed Jun 21 23:45:06 2023, max compression
```

## Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a4.tar` & `ovos-PHAL-plugin-wifi-setup-1.1.1a5.tar`

### file list

```diff
@@ -1,17 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 23:28:11.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-21 23:28:11.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup/
--rw-r--r--   0 runner    (1001) docker     (123)    23664 2023-06-21 23:28:11.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 23:28:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-21 23:28:11.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:45:06.367205 ovos-PHAL-plugin-wifi-setup-1.1.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-06-21 23:45:06.367205 ovos-PHAL-plugin-wifi-setup-1.1.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:45:06.363205 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)    23664 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:45:06.363205 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/ModeChoose.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/WifiPluginClientLoader.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:45:06.363205 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/icons/check-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/icons/info-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/icons/ondisplay.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/icons/ongeneric.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/icons/onmobile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/icons/times-circle.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:45:06.363205 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/sounds/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/sounds/ui_sounds_clicked.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:45:06.367205 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ModeChoose_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ModeChoose_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ModeChoose_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ModeChoose_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ModeChoose_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ModeChoose_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ovos-PHAL-plugin-wifi-setup_de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ovos-PHAL-plugin-wifi-setup_es.qm
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ovos-PHAL-plugin-wifi-setup_fr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ovos-PHAL-plugin-wifi-setup_it.qm
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ovos-PHAL-plugin-wifi-setup_nl.qm
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/ui/translations/ovos-PHAL-plugin-wifi-setup_pt.qm
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:45:06.363205 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-06-21 23:45:06.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-21 23:45:06.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:45:06.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-21 23:45:06.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 23:45:06.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 23:45:06.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:45:06.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:45:06.367205 ovos-PHAL-plugin-wifi-setup-1.1.1a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3187 2023-06-21 23:45:01.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a5/setup.py
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a4/LICENSE` & `ovos-PHAL-plugin-wifi-setup-1.1.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a4/README.md` & `ovos-PHAL-plugin-wifi-setup-1.1.1a5/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup/__init__.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a5/ovos_PHAL_plugin_wifi_setup/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a4/setup.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a5/setup.py`

 * *Files 12% similar despite different names*

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
     version_file = os.path.join(BASEDIR, 'ovos_PHAL_plugin_wifi_setup', 'version.py')
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
 PLUGIN_ENTRY_POINT = 'ovos-PHAL-plugin-wifi-setup=ovos_PHAL_plugin_wifi_setup:WifiSetupPlugin'
 setup(
     name='ovos-PHAL-plugin-wifi-setup',
     version=get_version(),
     description='A plugin for OpenVoiceOS hardware abstraction layer',
+    long_description=get_description(),
+    long_description_content_type="text/markdown",
     url='https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wifi-setup',
     author='Aiix',
     author_email='aix.m@outlook.com',
     license='Apache-2.0',
     packages=['ovos_PHAL_plugin_wifi_setup'],
     package_data={'': package_files('ovos_PHAL_plugin_wifi_setup')},
     install_requires=required("requirements.txt"),
```

