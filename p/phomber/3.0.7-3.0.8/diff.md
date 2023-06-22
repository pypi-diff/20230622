# Comparing `tmp/phomber-3.0.7-py3.9.egg` & `tmp/phomber-3.0.8-py3.9.egg`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 28459 bytes, number of entries: 11
--rw-r--r--  2.0 unx     5411 b- defN 23-Jun-23 00:58 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      245 b- defN 23-Jun-23 00:58 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 00:58 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       50 b- defN 23-Jun-23 00:58 EGG-INFO/entry_points.txt
--rw-r--r--  2.0 unx       90 b- defN 23-Jun-23 00:58 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-23 00:58 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 00:58 EGG-INFO/zip-safe
+Zip file size: 28389 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     5291 b- defN 23-Jun-23 01:04 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      245 b- defN 23-Jun-23 01:04 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 01:04 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-23 01:04 EGG-INFO/entry_points.txt
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-23 01:04 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-23 01:04 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 01:04 EGG-INFO/zip-safe
 -rw-r--r--  2.0 unx        0 b- defN 23-May-21 17:02 phomber/__init__.py
--rw-r--r--  2.0 unx    70448 b- defN 23-Jun-23 00:53 phomber/phomber.py
--rw-r--r--  2.0 unx      139 b- defN 23-Jun-23 00:58 phomber/__pycache__/__init__.cpython-39.pyc
--rw-r--r--  2.0 unx    41676 b- defN 23-Jun-23 00:58 phomber/__pycache__/phomber.cpython-39.pyc
-11 files, 118069 bytes uncompressed, 27055 bytes compressed:  77.1%
+-rw-r--r--  2.0 unx    70448 b- defN 23-Jun-23 01:03 phomber/phomber.py
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-23 01:04 phomber/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx    41676 b- defN 23-Jun-23 01:04 phomber/__pycache__/phomber.cpython-39.pyc
+11 files, 117949 bytes uncompressed, 26985 bytes compressed:  77.1%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomber
-Version: 3.0.7
+Version: 3.0.8
 Summary: `PH0MBER` a simple yet powerful osint framework for reconnaissance and information gathering
 Home-page: https://github.com/s41r4j/phomber
 Author: s41r4j
 License: UNKNOWN
 Description: <p align=center>
                  <img src='.images/phomber_logo.png'>
         </p>
@@ -117,10 +117,8 @@
         - `PH0MBER` is back with all new features and user interface
         - `v3` has osint tools with no _api key_ requirement
         - Currently this `v3.0-beta` is for testing, try using & report bugs
         ```
         
 Keywords: python,hacking,pentesting,phomber,reverse lookup,osint,framework,s41r4j
 Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phomber Version: 3.0.7 Summary: `PH0MBER` a simple
+Metadata-Version: 2.1 Name: phomber Version: 3.0.8 Summary: `PH0MBER` a simple
 yet powerful osint framework for reconnaissance and information gathering Home-
 page: https://github.com/s41r4j/phomber Author: s41r4j License: UNKNOWN
 Description:
                           [.images/phomber_logo.png]
 ``` An open source infomation grathering & reconnaissance framework! ```
   [https://img.shields.io/badge/Etical_Hacking-OSINT-yellow.svg?logo=sharp]
 [https://img.shields.io/badge/Version-v3.0-orange.svg?logo=vectorworks] [https:
@@ -43,10 +43,8 @@
 silent mode by using `-s`/`--silent` flag - You can also use `Ctrl+C` to exit -
 Descriptions ending with `*` needs internet connection
 
 ### NOTES: ``` - `PH0MBER` is back with all new features and user interface -
 `v3` has osint tools with no _api key_ requirement - Currently this `v3.0-beta`
 is for testing, try using & report bugs ``` Keywords:
 python,hacking,pentesting,phomber,reverse lookup,osint,framework,s41r4j
-Platform: UNKNOWN Classifier: Programming Language :: Python Classifier:
-License :: OSI Approved :: GNU General Public License v3 (GPLv3) Description-
-Content-Type: text/markdown
+Platform: UNKNOWN Description-Content-Type: text/markdown
```

## phomber/phomber.py

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 
 #==============================================================================#
 #                                                                              #
 # [prog]   : PH0MBER                                                           #
-# [ver]    : 3.0.7 beta                                                        #
+# [ver]    : 3.0.8 beta                                                        #
 # [desc]   : An open source infomation grathering & reconnaissance framework!  #
 # [dev]    : @s41r4j                                                           #
 # [license]: GNU GPLv3                                                         #
 # [github] : https://github.com/s41r4j/phomber                                 #
 # [pypi]   : https://pypi.org/project/phomber/                                 #
 #                                                                              #
 #==============================================================================#
@@ -902,15 +902,15 @@
     os_name = '\33[1;49;96m'+str(os.uname().sysname)+'\033[0m'+' '*int(34-len(str(os.uname().sysname)))
     ram = '\33[1;49;96m'+str(psutil.virtual_memory().percent)+"%"+'\033[0m'+' '*int(33-len(str(psutil.virtual_memory().percent)))
     cpu = '\33[1;49;96m'+str(psutil.cpu_percent())+"%"+'\033[0m'+' '*int(32-len(str(psutil.cpu_percent())))
     disk = '\33[1;49;96m'+str(psutil.disk_usage('/').percent)+"%"+'\033[0m'+' '*int(33-len(str(psutil.disk_usage('/').percent)))
     sys_mac = '\33[1;49;96m'+str(':'.join(re.findall('..', '%012x' % uuid.getnode())))+'\033[0m'+' '*int(34-len(str(':'.join(re.findall('..', '%012x' % uuid.getnode())))))
     arch = '\33[1;49;96m'+str(os.uname().machine)+'\033[0m'+' '*int(34-len(str(os.uname().machine)))
 
-    ver = '\33[1;49;96m3.0.7 (beta)\033[0m'+' '*int(34-len(str(3.0)))
+    ver = '\33[1;49;96m3.0.8 (beta)\033[0m'+' '*int(34-len(str(3.0)))
 
     sysinfo = f'''
     ┌────────────────────────────────────────────────────┐
     | SYSTEM INFO   | DESCRIPTION                        |
     |----------------------------------------------------|
     | \33[1;49;97mUser\033[0m          | {user} |
     | \33[1;49;97mHostname\033[0m      | {hostname} |
```

## phomber/__pycache__/phomber.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Jun 22 19:23:34 2023 UTC, .py size: 70448 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b69f 9464 3013 0100  a..........d0...
+00000000: 610d 0d0a 0000 0000 1fa2 9464 3013 0100  a..........d0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 3001 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c08 5a08 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
@@ -1767,15 +1767,15 @@
 00006e60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00006e70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00006e80: e294 80e2 9480 e294 80e2 9480 e294 987a  ...............z
 00006e90: 0a1b 5b31 3b34 393b 3936 6d72 a400 0000  ..[1;49;96mr....
 00006ea0: 7236 0000 00e9 2200 0000 fa01 25e9 2100  r6....".....%.!.
 00006eb0: 0000 e920 0000 0072 3b00 0000 fa01 3a7a  ... ...r;.....:z
 00006ec0: 022e 2e7a 0525 3031 3278 7a1a 1b5b 313b  ...z.%012xz..[1;
-00006ed0: 3439 3b39 366d 332e 302e 3720 2862 6574  49;96m3.0.7 (bet
+00006ed0: 3439 3b39 366d 332e 302e 3820 2862 6574  49;96m3.0.8 (bet
 00006ee0: 6129 1b5b 306d 6700 0000 0000 0008 4075  a).[0mg.......@u
 00006ef0: 4201 0000 0a20 2020 20e2 948c e294 80e2  B....    .......
 00006f00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00006f10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00006f20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00006f30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00006f40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
```

