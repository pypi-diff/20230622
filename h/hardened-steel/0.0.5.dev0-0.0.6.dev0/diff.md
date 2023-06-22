# Comparing `tmp/hardened-steel-0.0.5.dev0.tar.gz` & `tmp/hardened-steel-0.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardened-steel-0.0.5.dev0.tar", last modified: Wed Jun 21 23:22:46 2023, max compression
+gzip compressed data, was "hardened-steel-0.0.6.dev0.tar", last modified: Thu Jun 22 11:58:35 2023, max compression
```

## Comparing `hardened-steel-0.0.5.dev0.tar` & `hardened-steel-0.0.6.dev0.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/hardened_steel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-21 23:22:46.000000 hardened-steel-0.0.5.dev0/hardened_steel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-21 23:22:46.000000 hardened-steel-0.0.5.dev0/hardened_steel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:22:46.000000 hardened-steel-0.0.5.dev0/hardened_steel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 23:22:46.000000 hardened-steel-0.0.5.dev0/hardened_steel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/steel/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/steel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/steel/facades/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/steel/facades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/steel/facades/texts/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/steel/facades/texts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/steel/facades/texts/characters/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/steel/facades/texts/characters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/steel/facades/texts/characters/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/steel/facades/texts/random_text_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/steel/globals/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/steel/globals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/steel/globals/singletons/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/steel/globals/singletons/SingletonSystenRandom.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/steel/globals/singletons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:22:46.549288 hardened-steel-0.0.5.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-21 23:22:35.000000 hardened-steel-0.0.5.dev0/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/booleans/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/booleans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/booleans/random_boolean_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/integers/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/integers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/integers/random_number_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.047432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/characters/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/characters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/characters/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/random_text_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/HardenedSteel/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/HardenedSteel/globals/singletons/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/singletons/SingletonSystenRandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/singletons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/HardenedSteel/globals/vars/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/vars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/HardenedSteel/globals/vars/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-22 11:58:35.000000 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-22 11:58:35.000000 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:58:35.000000 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 11:58:35.000000 hardened-steel-0.0.6.dev0/hardened_steel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:58:35.051432 hardened-steel-0.0.6.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-22 11:58:15.000000 hardened-steel-0.0.6.dev0/tests/test_singleton.py
```

### Comparing `hardened-steel-0.0.5.dev0/PKG-INFO` & `hardened-steel-0.0.6.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardened-steel
-Version: 0.0.5.dev0
+Version: 0.0.6.dev0
 Summary: Framework for helping to test projects with the generation of random data during TDD
 Author-email: IO Jægers <support@cloud.iojaegers.com>, Kent Madsen <kent.vejrup.madsen@outlook.com>
 Project-URL: Homepage, https://github.com/IO-Jaegers/Steel
 Project-URL: Issues, https://github.com/IO-Jaegers/Steel/issues
 Project-URL: Wiki, https://github.com/IO-Jaegers/Steel/wiki
 Project-URL: Releases, https://pypi.org/manage/project/hardened-steel/releases/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hardened-steel-0.0.5.dev0/hardened_steel.egg-info/PKG-INFO` & `hardened-steel-0.0.6.dev0/hardened_steel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardened-steel
-Version: 0.0.5.dev0
+Version: 0.0.6.dev0
 Summary: Framework for helping to test projects with the generation of random data during TDD
 Author-email: IO Jægers <support@cloud.iojaegers.com>, Kent Madsen <kent.vejrup.madsen@outlook.com>
 Project-URL: Homepage, https://github.com/IO-Jaegers/Steel
 Project-URL: Issues, https://github.com/IO-Jaegers/Steel/issues
 Project-URL: Wiki, https://github.com/IO-Jaegers/Steel/wiki
 Project-URL: Releases, https://pypi.org/manage/project/hardened-steel/releases/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hardened-steel-0.0.5.dev0/steel/facades/texts/characters/ranges.py` & `hardened-steel-0.0.6.dev0/HardenedSteel/facades/texts/characters/ranges.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from steel.facades.texts.characters \
-    import get_system_random
+from HardenedSteel.facades.texts.characters \
+    import                                  \
+    get_system_random,                      \
+    generate_random_boolean
 
 ascii_lowercase_begin:  int = ord('a')
 ascii_lowercase_end:    int = ord('z')
 
 ascii_uppercase_begin:  int = ord('A')
 ascii_uppercase_end:    int = ord('Z')
 
 
 def random_letter() -> chr:
-    random = get_system_random()
-
-    choose_uppercase: bool = bool(
-        random.getrandbits(1)
-    )
+    choose_uppercase: bool = generate_random_boolean()
 
     if choose_uppercase:
         return random_uppercase_letter()
     else:
         return random_lowercase_letter()
```

### Comparing `hardened-steel-0.0.5.dev0/steel/globals/singletons/SingletonSystenRandom.py` & `hardened-steel-0.0.6.dev0/HardenedSteel/globals/singletons/SingletonSystenRandom.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from random \
+from random                                             \
     import SystemRandom
 
 singleton_system_random: SystemRandom | None = None
 
 
 def get_system_random() -> SystemRandom:
     global singleton_system_random
```

