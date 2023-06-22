# Comparing `tmp/otherworlds-0.9.0b1.tar.gz` & `tmp/otherworlds-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otherworlds-0.9.0b1.tar", max compression
+gzip compressed data, was "otherworlds-0.9.1.tar", max compression
```

## Comparing `otherworlds-0.9.0b1.tar` & `otherworlds-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2022-10-01 05:58:49.357727 otherworlds-0.9.0b1/LICENSE
--rw-r--r--   0        0        0      471 2022-10-02 19:07:05.089120 otherworlds-0.9.0b1/README.md
--rw-r--r--   0        0        0        0 2022-10-02 19:07:05.089120 otherworlds-0.9.0b1/otherworlds/__init__.py
--rw-r--r--   0        0        0     2236 2022-10-02 19:07:05.089120 otherworlds-0.9.0b1/otherworlds/exoplanets.py
--rw-r--r--   0        0        0      365 2022-10-02 19:07:05.089120 otherworlds-0.9.0b1/otherworlds/klingon.py
--rw-r--r--   0        0        0     1832 2022-10-02 19:07:05.089120 otherworlds-0.9.0b1/otherworlds/main.py
--rw-r--r--   0        0        0      195 2022-10-02 19:07:05.089120 otherworlds-0.9.0b1/otherworlds/utils.py
--rw-r--r--   0        0        0      727 2022-10-02 19:11:33.974434 otherworlds-0.9.0b1/pyproject.toml
--rw-r--r--   0        0        0     1148 2022-10-02 19:11:44.471431 otherworlds-0.9.0b1/setup.py
--rw-r--r--   0        0        0     1174 2022-10-02 19:11:44.471617 otherworlds-0.9.0b1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-01 05:58:49.357727 otherworlds-0.9.1/LICENSE
+drwxr-xr-x   0        0        0        0 2023-05-31 23:01:25.215392 otherworlds-0.9.1/LICENSES/
+-rw-r--r--   0        0        0     1238 2023-05-31 23:25:48.888198 otherworlds-0.9.1/README.md
+-rw-r--r--   0        0        0       95 2023-05-31 23:01:25.219392 otherworlds-0.9.1/otherworlds/__init__.py
+-rw-r--r--   0        0        0     2325 2023-05-31 23:01:25.219392 otherworlds-0.9.1/otherworlds/exoplanets.py
+-rw-r--r--   0        0        0      461 2023-05-31 23:01:25.219392 otherworlds-0.9.1/otherworlds/klingon.py
+-rw-r--r--   0        0        0     1922 2023-05-31 23:01:25.219392 otherworlds-0.9.1/otherworlds/main.py
+-rw-r--r--   0        0        0      291 2023-05-31 23:01:25.219392 otherworlds-0.9.1/otherworlds/utils.py
+-rw-r--r--   0        0        0     1014 2023-05-31 23:25:48.888198 otherworlds-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 otherworlds-0.9.1/PKG-INFO
```

### Comparing `otherworlds-0.9.0b1/LICENSE` & `otherworlds-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `otherworlds-0.9.0b1/otherworlds/exoplanets.py` & `otherworlds-0.9.1/otherworlds/exoplanets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+# SPDX-FileCopyrightText: 2023 Civic Hacker, LLC
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+
 import argparse
-import os
 import uuid
 import random
 import csv
 
 PREFIX_TYPES = [
     "mathematical",
     "empty"
@@ -29,15 +32,15 @@
     'Rho',
     'Delta',
     'Omega',
     'Epsilon',
     'Theta'
 ]
 
-NUMERICAL = random.sample(range(1,10), 1)
+NUMERICAL = random.sample(range(1, 10), 1)
 
 FEMALE_KLINGON = [
     "Azetbur",
     "B'Etor",
     "Ba'el",
     "Ch'Rega",
     "Ezri",
@@ -80,16 +83,16 @@
         reader = csv.DictReader(f)
         for line in reader:
             EXOPLANETS.append(line.get("Name Exoplanet"))
             STARNAMES.append(line.get("Name Star"))
     UUID = str(uuid.uuid4())
     ending = UUID.split('-')[-1]
     starting = UUID.split('-')[0]
-    ending_ans = int(ending[0], base=16)+int(ending[1],base=16)
-    starting_ans = int(starting[0], base=16)+int(starting[1],base=16)
+    ending_ans = int(ending[0], base=16)+int(ending[1], base=16)
+    starting_ans = int(starting[0], base=16)+int(starting[1], base=16)
     suffix_source = SUFFIX_TYPES[ending_ans % len(SUFFIX_TYPES)]
     namefix = NAME_SOURCES[starting_ans % len(NAME_SOURCES)]
     suffix = ''
     if namefix == 'female_klingon':
         name = random.sample(FEMALE_KLINGON, 1)[0]
     elif namefix == 'male_klingon':
         name = random.sample(MALE_KLINGON, 1)[0]
```

### Comparing `otherworlds-0.9.0b1/otherworlds/main.py` & `otherworlds-0.9.1/otherworlds/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import os
+# SPDX-FileCopyrightText: 2023 Civic Hacker, LLC
+#
+# SPDX-License-Identifier: GPL-3.0-or-later
+
 import uuid
 import random
 import csv
 
 from otherworlds.klingon import FEMALE_KLINGON, MALE_KLINGON
 
 DEFAULT_SEED = 270055
@@ -31,30 +34,31 @@
     'Rho',
     'Delta',
     'Omega',
     'Epsilon',
     'Theta'
 ]
 
-NUMERICAL = random.sample(range(1,10), 1)
+NUMERICAL = random.sample(range(1, 10), 1)
 
 EXOPLANETS = list()
 STARNAMES = list()
 
+
 def generate_name(include_klingon=False):
     with open('./data/NameExoWorlds.csv', 'r') as f:
         reader = csv.DictReader(f)
         for line in reader:
             EXOPLANETS.append(line.get("Name Exoplanet"))
             STARNAMES.append(line.get("Name Star"))
     UUID = str(uuid.uuid4())
     ending = UUID.split('-')[-1]
     starting = UUID.split('-')[0]
-    ending_ans = int(ending[0], base=16)+int(ending[1],base=16)
-    starting_ans = int(starting[0], base=16)+int(starting[1],base=16)
+    ending_ans = int(ending[0], base=16)+int(ending[1], base=16)
+    starting_ans = int(starting[0], base=16)+int(starting[1], base=16)
     suffix_source = SUFFIX_TYPES[ending_ans % len(SUFFIX_TYPES)]
     if include_klingon:
         NAME_SOURCES.append('female_klingon')
         NAME_SOURCES.append('male_klingon')
     namefix = NAME_SOURCES[starting_ans % len(NAME_SOURCES)]
     suffix = ''
     if namefix == 'female_klingon':
```

### Comparing `otherworlds-0.9.0b1/pyproject.toml` & `otherworlds-0.9.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 [tool.poetry]
 name = "otherworlds"
-version = "0.9.0-beta.1"
-description = "A name generator for new worlds"
+version = "0.9.1"
+description = "A name generator for nonsensitive things"
 authors = ["Jurnell Cockhren <jurnell@civichacker.com>"]
-license = "LGPL-3.0-or-later"
+license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
-    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 packages = [
     { include = "otherworlds" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 
+[tool.poetry.group.dev.dependencies]
+reuse = "^1.1.2"
+flake8 = { version = "^6.0.0", python = ">=3.8.1" }
+vulture = "^2.7"
+pytest = "^7.3.1"
+tox = "^4.5.2"
+pytest-cov = "^4.1.0"
+
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 otherworlds = 'console:run'
+
+[tool.vulture]
+ignore_names = ["run"]
+paths = ["otherworlds", "console"]
+min_confidence = 80
+sort_by_size = true
```

