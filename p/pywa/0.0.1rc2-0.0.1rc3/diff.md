# Comparing `tmp/pywa-0.0.1rc2.linux-x86_64.tar.gz` & `tmp/pywa-0.0.1rc3.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywa-0.0.1rc2.linux-x86_64.tar", last modified: Wed Jun 21 08:44:24 2023, max compression
+gzip compressed data, was "pywa-0.0.1rc3.linux-x86_64.tar", last modified: Thu Jun 22 16:52:53 2023, max compression
```

## Comparing `pywa-0.0.1rc2.linux-x86_64.tar` & `pywa-0.0.1rc3.linux-x86_64.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/
--rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-21 08:44:14.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.873170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/
--rw-rw-r--   0 david     (1000) david     (1000)      388 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    10312 2023-06-21 08:44:24.869170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/api.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    24827 2023-06-21 08:44:24.873170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/client.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     1849 2023-06-21 08:44:24.869170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/errors.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    27626 2023-06-21 08:44:24.869170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/filters.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     3401 2023-06-21 08:44:24.869170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/handlers.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    39766 2023-06-21 08:44:24.865170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/types.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     2153 2023-06-21 08:44:24.861170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     6136 2023-06-21 08:44:24.865170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/webhook.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     7598 2023-06-20 20:53:37.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py
--rw-rw-r--   0 david     (1000) david     (1000)    22338 2023-06-20 20:45:27.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/pywa/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/pywa/venv/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/pywa/venv/lib/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.951557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.931556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/
+-rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-22 16:50:59.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.939556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/
+-rw-rw-r--   0 david     (1000) david     (1000)      388 2023-06-22 16:52:53.931556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    10696 2023-06-22 16:52:53.935557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/api.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    26453 2023-06-22 16:52:53.939556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/client.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     1849 2023-06-22 16:52:53.935557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/errors.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    26796 2023-06-22 16:52:53.939556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/filters.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     3401 2023-06-22 16:52:53.939556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/handlers.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    41016 2023-06-22 16:52:53.935557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/types.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     2153 2023-06-22 16:52:53.931556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     6136 2023-06-22 16:52:53.931556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/webhook.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     7965 2023-06-22 15:59:56.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    23766 2023-06-22 15:59:56.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py
 -rw-rw-r--   0 david     (1000) david     (1000)      989 2023-06-19 21:14:34.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/errors.py
--rw-rw-r--   0 david     (1000) david     (1000)    12393 2023-06-20 20:14:12.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11023 2023-06-22 14:58:38.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py
 -rw-rw-r--   0 david     (1000) david     (1000)     1656 2023-06-20 09:34:04.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py
--rw-rw-r--   0 david     (1000) david     (1000)    24771 2023-06-20 20:21:31.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py
+-rw-rw-r--   0 david     (1000) david     (1000)    25776 2023-06-22 15:59:56.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py
 -rw-rw-r--   0 david     (1000) david     (1000)      991 2023-06-20 16:58:34.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/utils.py
 -rw-rw-r--   0 david     (1000) david     (1000)     4141 2023-06-20 09:37:01.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/webhook.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     4573 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      293 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       51 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        5 2023-06-21 08:44:24.877170 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc2-py3.11.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.951557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)    10028 2023-06-22 16:52:53.947557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      301 2023-06-22 16:52:53.951557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-22 16:52:53.947557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       51 2023-06-22 16:52:53.947557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        5 2023-06-22 16:52:53.947557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/top_level.txt
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Python wrapper for the WhatsApp Cloud API. https://github.com/david-lev/pywa"""
 
-__version__ = "0.0.1rc2"
+__version__ = "0.0.1rc3"
 
 from pywa.client import WhatsApp
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,35 +1,35 @@
 magic:    0xa70d0d0a
-moddate:  0x5eb89264 (Wed Jun 21 08:44:14 2023 UTC)
+moddate:  0xf37b9464 (Thu Jun 22 16:50:59 2023 UTC)
 files sz: 143
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x970064005a0064015a01640264036c026d035a03010064045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Python wrapper for the WhatsApp Cloud API. https://github.com/david-lev/pywa')
                  4 STORE_NAME               0 (__doc__)
    
-     3           6 LOAD_CONST               1 ('0.0.1rc2')
+     3           6 LOAD_CONST               1 ('0.0.1rc3')
                  8 STORE_NAME               1 (__version__)
    
      5          10 LOAD_CONST               2 (0)
                 12 LOAD_CONST               3 (('WhatsApp',))
                 14 IMPORT_NAME              2 (pywa.client)
                 16 IMPORT_FROM              3 (WhatsApp)
                 18 STORE_NAME               3 (WhatsApp)
                 20 POP_TOP
                 22 LOAD_CONST               4 (None)
                 24 RETURN_VALUE
    consts
       'Python wrapper for the WhatsApp Cloud API. https://github.com/david-lev/pywa'
-      '0.0.1rc2'
+      '0.0.1rc3'
       0
       ('WhatsApp',)
       None
    names      ('__doc__', '__version__', 'pywa.client', 'WhatsApp')
    varnames   ()
    freevars   ()
    cellvars   ()
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/api.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xd1119264 (Tue Jun 20 20:53:37 2023 UTC)
-files sz: 7598
+moddate:  0xfc6f9464 (Thu Jun 22 15:59:56 2023 UTC)
+files sz: 7965
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064016c035a
@@ -68,27 +68,27 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 15
          flags     : 0
          code
             0x970065005a0164005a0264015a036402650464036504640465056a0600
             000000000000006405650464066507660a640784045a0864086504640965
-            04640a6509650a7a0700006606640b84045a0b09000900642a640e650465
+            04640a6509650a7a0700006606640b84045a0b09000900642b640e650465
             0c7a070000640f65046410650d64116504640d7a070000640a6504660a64
             1284055a0e64136504650f7a07000064146504640d7a070000640a650466
-            06641584045a100900642b640e6504650c7a070000641665046417650464
+            06641584045a100900642c640e6504650c7a070000641665046417650464
             116504640d7a0700006608641884055a11640e6504650c7a070000641965
-            04641a65046606641b84045a1209000900642c640e6504650c7a07000064
+            04641a65046606641b84045a1209000900642d640e6504650c7a07000064
             1c6507641d6507641e6504640d7a070000641f6504640d7a070000660a64
-            2084055a1364216509640a65096604642284045a14090009000900642d64
+            2084055a1364216509640a65096604642284045a14090009000900642e64
             0e6504650c7a0700006423650a65151900000000000000000065167a0700
             006424650464256509640d7a07000064266504640d7a0700006411650464
-            0d7a070000640a6504660e642784055a170900642b640e6504650c7a0700
+            0d7a070000640a6504660e642784055a170900642c640e6504650c7a0700
             006428651865191900000000000000000064116504640d7a070000640a65
-            046608642984055a1a640d5300
+            046608642984055a1a641a6504640a650d6604642a84045a1b640d5300
            8           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('WhatsAppCloudApi')
                        8 STORE_NAME               2 (__qualname__)
          
            9          10 LOAD_CONST               1 ('Internal methods for the WhatsApp client.')
@@ -139,15 +139,15 @@
                       74 MAKE_FUNCTION            4 (annotations)
                       76 STORE_NAME              11 (_make_request)
          
           46          78 NOP
          
           47          80 NOP
          
-          42          82 LOAD_CONST              42 ((False, None))
+          42          82 LOAD_CONST              43 ((False, None))
                       84 LOAD_CONST              14 ('to')
          
           44          86 LOAD_NAME                4 (str)
                       88 LOAD_NAME               12 (int)
                       90 BINARY_OP                7 (|)
          
           42          94 LOAD_CONST              15 ('text')
@@ -192,15 +192,15 @@
           67         148 BUILD_TUPLE              6
                      150 LOAD_CONST              21 (<code object upload_media, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py", line 67>)
                      152 MAKE_FUNCTION            4 (annotations)
                      154 STORE_NAME              16 (upload_media)
          
          118         156 NOP
          
-         113         158 LOAD_CONST              43 ((None,))
+         113         158 LOAD_CONST              44 ((None,))
                      160 LOAD_CONST              14 ('to')
          
          115         162 LOAD_NAME                4 (str)
                      164 LOAD_NAME               12 (int)
                      166 BINARY_OP                7 (|)
          
          113         170 LOAD_CONST              22 ('media_id_or_url')
@@ -241,15 +241,15 @@
                      218 MAKE_FUNCTION            4 (annotations)
                      220 STORE_NAME              18 (send_reaction)
          
          163         222 NOP
          
          164         224 NOP
          
-         158         226 LOAD_CONST              44 ((None, None))
+         158         226 LOAD_CONST              45 ((None, None))
                      228 LOAD_CONST              14 ('to')
          
          160         230 LOAD_NAME                4 (str)
                      232 LOAD_NAME               12 (int)
                      234 BINARY_OP                7 (|)
          
          158         238 LOAD_CONST              28 ('latitude')
@@ -292,15 +292,15 @@
          
          199         290 NOP
          
          200         292 NOP
          
          201         294 NOP
          
-         194         296 LOAD_CONST              45 ((None, None, None))
+         194         296 LOAD_CONST              46 ((None, None, None))
                      298 LOAD_CONST              14 ('to')
          
          196         300 LOAD_NAME                4 (str)
                      302 LOAD_NAME               12 (int)
                      304 BINARY_OP                7 (|)
          
          194         308 LOAD_CONST              35 ('keyboard')
@@ -340,15 +340,15 @@
          194         368 BUILD_TUPLE             14
                      370 LOAD_CONST              39 (<code object send_interactive_message, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py", line 194>)
                      372 MAKE_FUNCTION            5 (defaults, annotations)
                      374 STORE_NAME              23 (send_interactive_message)
          
          236         376 NOP
          
-         232         378 LOAD_CONST              43 ((None,))
+         232         378 LOAD_CONST              44 ((None,))
                      380 LOAD_CONST              14 ('to')
          
          234         382 LOAD_NAME                4 (str)
                      384 LOAD_NAME               12 (int)
                      386 BINARY_OP                7 (|)
          
          232         390 LOAD_CONST              40 ('contacts')
@@ -367,16 +367,29 @@
          
          237         418 LOAD_NAME                4 (str)
          
          232         420 BUILD_TUPLE              8
                      422 LOAD_CONST              41 (<code object send_contacts, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py", line 232>)
                      424 MAKE_FUNCTION            5 (defaults, annotations)
                      426 STORE_NAME              26 (send_contacts)
-                     428 LOAD_CONST              13 (None)
-                     430 RETURN_VALUE
+         
+         252         428 LOAD_CONST              26 ('message_id')
+         
+         254         430 LOAD_NAME                4 (str)
+         
+         252         432 LOAD_CONST              10 ('return')
+         
+         255         434 LOAD_NAME               13 (bool)
+         
+         252         436 BUILD_TUPLE              4
+                     438 LOAD_CONST              42 (<code object mark_message_as_read, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py", line 252>)
+                     440 MAKE_FUNCTION            4 (annotations)
+                     442 STORE_NAME              27 (mark_message_as_read)
+                     444 LOAD_CONST              13 (None)
+                     446 RETURN_VALUE
          consts
             'WhatsAppCloudApi'
             'Internal methods for the WhatsApp client.'
             'phone_id'
             'token'
             'session'
             'base_url'
@@ -1570,33 +1583,86 @@
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py'
                name       'send_contacts'
                firstlineno 232
                lnotab
                   0x020602010cff02021c01020116fc080604010e0118010201020102fd10
                   0402fc0a0402fc0a0402fc
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 8
+               flags     : 3
+               code
+                  0x97007c00a0000000000000000000000000000000000000000000640164
+                  02640364047c0164059c03ac06a6030000ab030000000000000000640719
+                  0000000000000000005300
+               252           0 RESUME                   0
+               
+               256           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (_make_request)
+               
+               257          26 LOAD_CONST               1 ('POST')
+               
+               258          28 LOAD_CONST               2 ('/messages')
+               
+               260          30 LOAD_CONST               3 ('whatsapp')
+               
+               261          32 LOAD_CONST               4 ('read')
+               
+               262          34 LOAD_FAST                1 (message_id)
+               
+               259          36 LOAD_CONST               5 (('messaging_product', 'status', 'message_id'))
+                            38 BUILD_CONST_KEY_MAP      3
+               
+               256          40 KW_NAMES                 6
+                            42 PRECALL                  3
+                            46 CALL                     3
+               
+               264          56 LOAD_CONST               7 ('success')
+               
+               256          58 BINARY_SUBSCR
+                            68 RETURN_VALUE
+               consts
+                  None
+                  'POST'
+                  '/messages'
+                  'whatsapp'
+                  'read'
+                  ('messaging_product', 'status', 'message_id')
+                  ('method', 'endpoint', 'json')
+                  'success'
+               names      ('_make_request',)
+               varnames   ('self', 'message_id')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py'
+               name       'mark_message_as_read'
+               firstlineno 252
+               lnotab 0x02041801020102020201020102fd04fd100802f8
             (False, None)
             (None,)
             (None, None)
             (None, None, None)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', 'requests', 'Session', 'float', '__init__', 'dict', 'list', '_make_request', 'int', 'bool', 'send_text_message', 'bytes', 'upload_media', 'send_media', 'send_reaction', 'send_location', 'send_raw_json', 'InlineButton', 'SectionList', 'send_interactive_message', 'Iterable', 'Contact', 'send_contacts')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', 'requests', 'Session', 'float', '__init__', 'dict', 'list', '_make_request', 'int', 'bool', 'send_text_message', 'bytes', 'upload_media', 'send_media', 'send_reaction', 'send_location', 'send_raw_json', 'InlineButton', 'SectionList', 'send_interactive_message', 'Iterable', 'Contact', 'send_contacts', 'mark_message_as_read')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py'
          name       'WhatsAppCloudApi'
          firstlineno 8
          lnotab
             0x0a010402020202fe020302fd02040cfc020502fb020602fa0814020202
             fe020302fd020508fb080f020102fb040208fe020302fd020402fc020508
             fb020602fa0819020208fe020308fd020402fc083302fb040208fe020302
             fd020402fc020508fb0819020208fe020302fd020402fc0819020102fa04
             0208fe020302fd020402fc020508fb020608fa081a020202fe020302fd08
             0f0201020102f9040208fe020314fd020402fc020508fb020608fa020708
-            f9020802f8082a02fc040208fe02030efd020408fc020502fb
+            f9020802f8082a02fc040208fe02030efd020408fc020502fb0814020202
+            fe020302fd
       'WhatsAppCloudApi'
    names      ('mimetypes', 'typing', 'Iterable', 'requests', 'pywa.errors', 'WhatsAppApiError', 'pywa.types', 'InlineButton', 'SectionList', 'Contact', 'WhatsAppCloudApi')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py'
    name       '<module>'
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/client.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe70f9264 (Tue Jun 20 20:45:27 2023 UTC)
-files sz: 22338
+moddate:  0xfc6f9464 (Thu Jun 22 15:59:56 2023 UTC)
+files sz: 23766
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a036d
@@ -106,51 +106,52 @@
       ('webhook',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 18
          flags     : 0
          code
-            0x970065005a0164005a0209000900090009000900090064396405650365
+            0x970065005a0164005a02090009000900090009000900643b6405650365
             047a070000640665036407650564017a070000640865036409650364017a
             070000640a6503640b6506640c65076a08000000000000000064017a0700
-            006610640d84055a09640e650a6602640f84045a0b0900643a6410650c65
+            006610640d84055a09640e650a6602640f84045a0b0900643c6410650c65
             0d6400650e6702650f660219000000000000000000190000000000000000
             00650d6400650e6702650f6602190000000000000000007a070000660264
-            1184055a100900643a6410650c650d640065116702650f66021900000000
+            1184055a100900643c6410650c650d640065116702650f66021900000000
             000000000019000000000000000000650d640065116702650f6602190000
-            000000000000007a0700006602641284055a120900643a6410650c650d64
+            000000000000007a0700006602641284055a120900643c6410650c650d64
             0065136702650f6602190000000000000000001900000000000000000065
             0d640065136702650f6602190000000000000000007a0700006602641384
-            055a140900643a6410650c650d640065156702650f660219000000000000
+            055a140900643c6410650c650d640065156702650f660219000000000000
             00000019000000000000000000650d640065156702650f66021900000000
-            00000000007a0700006602641484055a160900643a6410650c650d640065
+            00000000007a0700006602641484055a160900643c6410650c650d640065
             176702650f66021900000000000000000019000000000000000000650d64
             0065176702650f6602190000000000000000007a0700006602641584055a
-            1809000900090009000900643b64176503641865036419650f641a650364
+            1809000900090009000900643d64176503641865036419650f641a650364
             017a070000641b6519651a19000000000000000000651b7a07000064017a
             070000641c650364017a070000641d650364017a070000641e6503661064
-            1f84055a1c09000900090009000900643c6417650364206503651d7a0700
+            1f84055a1c09000900090009000900643e6417650364206503651d7a0700
             006421650364017a070000641a650364017a07000064226519651a190000
             0000000000000064017a0700006423650364017a070000641d650364017a
-            070000641e65036610642484055a1e09000900090009000900643c641765
+            070000641e65036610642484055a1e09000900090009000900643e641765
             0364256503651d7a0700006421650364017a070000641a650364017a0700
             0064226519651a1900000000000000000064017a0700006423650364017a
             070000641d650364017a070000641e65036610642684055a1f0900090009
-            00090009000900643d6417650364276503651d7a0700006428650364017a
+            00090009000900643f6417650364276503651d7a0700006428650364017a
             0700006421650364017a070000641a650364017a07000064226519651a19
             00000000000000000064017a0700006423650364017a070000641d650364
-            017a0700006610642984055a200900643a64176503642a6503651d7a0700
-            00641a650364017a070000641e65036608642b84055a2109000900643e64
+            017a0700006610642984055a200900643c64176503642a6503651d7a0700
+            00641a650364017a070000641e65036608642b84055a2109000900644064
             176503642c6503651d7a070000642d650f641a650364017a070000641e65
             03660a642e84055a2264176503642f650364306503641e65036608643184
-            045a2309000900643f6417650364326506643365066434650364017a0700
-            006435650364017a070000641e6503660c643684055a240900643a641765
-            0364376525650c6525190000000000000000007a070000641a650364017a
-            070000641e65036608643884055a2664015300
+            045a236417650364306503641e65036606643284045a2409000900644164
+            17650364336506643465066435650364017a0700006436650364017a0700
+            00641e6503660c643784055a250900643c6417650364386526650c652619
+            0000000000000000007a070000641a650364017a070000641e6503660864
+            3984055a2764306503641e650f6604643a84045a2864015300
           11           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('WhatsApp')
                        8 STORE_NAME               2 (__qualname__)
          
           16          10 NOP
@@ -161,15 +162,15 @@
          
           19          16 NOP
          
           20          18 NOP
          
           21          20 NOP
          
-          12          22 LOAD_CONST              57 ((None, '/pywa', None, 'https://graph.facebook.com', 17.0, None))
+          12          22 LOAD_CONST              59 ((None, '/pywa', None, 'https://graph.facebook.com', 17.0, None))
                       24 LOAD_CONST               5 ('phone_id')
          
           14          26 LOAD_NAME                3 (str)
                       28 LOAD_NAME                4 (int)
                       30 BINARY_OP                7 (|)
          
           12          34 LOAD_CONST               6 ('token')
@@ -217,15 +218,15 @@
                      102 BUILD_TUPLE              2
                      104 LOAD_CONST              15 (<code object add_handler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 60>)
                      106 MAKE_FUNCTION            4 (annotations)
                      108 STORE_NAME              11 (add_handler)
          
           67         110 NOP
          
-          65         112 LOAD_CONST              58 ((None,))
+          65         112 LOAD_CONST              60 ((None,))
                      114 LOAD_CONST              16 ('filters')
          
           67         116 LOAD_NAME               12 (Iterable)
                      118 LOAD_NAME               13 (Callable)
                      120 LOAD_CONST               0 ('WhatsApp')
                      122 LOAD_NAME               14 (dict)
                      124 BUILD_LIST               2
@@ -245,15 +246,15 @@
           65         176 BUILD_TUPLE              2
                      178 LOAD_CONST              17 (<code object on_raw_update, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 65>)
                      180 MAKE_FUNCTION            5 (defaults, annotations)
                      182 STORE_NAME              16 (on_raw_update)
          
           90         184 NOP
          
-          87         186 LOAD_CONST              58 ((None,))
+          87         186 LOAD_CONST              60 ((None,))
                      188 LOAD_CONST              16 ('filters')
          
           89         190 LOAD_NAME               12 (Iterable)
                      192 LOAD_NAME               13 (Callable)
                      194 LOAD_CONST               0 ('WhatsApp')
                      196 LOAD_NAME               17 (Message)
                      198 BUILD_LIST               2
@@ -275,15 +276,15 @@
           87         250 BUILD_TUPLE              2
                      252 LOAD_CONST              18 (<code object on_message, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 87>)
                      254 MAKE_FUNCTION            5 (defaults, annotations)
                      256 STORE_NAME              18 (on_message)
          
          114         258 NOP
          
-         111         260 LOAD_CONST              58 ((None,))
+         111         260 LOAD_CONST              60 ((None,))
                      262 LOAD_CONST              16 ('filters')
          
          113         264 LOAD_NAME               12 (Iterable)
                      266 LOAD_NAME               13 (Callable)
                      268 LOAD_CONST               0 ('WhatsApp')
                      270 LOAD_NAME               19 (CallbackButton)
                      272 BUILD_LIST               2
@@ -305,15 +306,15 @@
          111         324 BUILD_TUPLE              2
                      326 LOAD_CONST              19 (<code object on_callback_button, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 111>)
                      328 MAKE_FUNCTION            5 (defaults, annotations)
                      330 STORE_NAME              20 (on_callback_button)
          
          137         332 NOP
          
-         134         334 LOAD_CONST              58 ((None,))
+         134         334 LOAD_CONST              60 ((None,))
                      336 LOAD_CONST              16 ('filters')
          
          136         338 LOAD_NAME               12 (Iterable)
                      340 LOAD_NAME               13 (Callable)
                      342 LOAD_CONST               0 ('WhatsApp')
                      344 LOAD_NAME               21 (CallbackSelection)
                      346 BUILD_LIST               2
@@ -335,15 +336,15 @@
          134         398 BUILD_TUPLE              2
                      400 LOAD_CONST              20 (<code object on_callback_selection, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 134>)
                      402 MAKE_FUNCTION            5 (defaults, annotations)
                      404 STORE_NAME              22 (on_callback_selection)
          
          160         406 NOP
          
-         157         408 LOAD_CONST              58 ((None,))
+         157         408 LOAD_CONST              60 ((None,))
                      410 LOAD_CONST              16 ('filters')
          
          159         412 LOAD_NAME               12 (Iterable)
                      414 LOAD_NAME               13 (Callable)
                      416 LOAD_CONST               0 ('WhatsApp')
                      418 LOAD_NAME               23 (MessageStatus)
                      420 BUILD_LIST               2
@@ -373,15 +374,15 @@
          
          186         484 NOP
          
          187         486 NOP
          
          188         488 NOP
          
-         180         490 LOAD_CONST              59 ((False, None, None, None, None))
+         180         490 LOAD_CONST              61 ((False, None, None, None, None))
                      492 LOAD_CONST              23 ('to')
          
          182         494 LOAD_NAME                3 (str)
          
          180         496 LOAD_CONST              24 ('text')
          
          183         498 LOAD_NAME                3 (str)
@@ -433,15 +434,15 @@
          
          290         578 NOP
          
          291         580 NOP
          
          292         582 NOP
          
-         284         584 LOAD_CONST              60 ((None, None, None, None, None))
+         284         584 LOAD_CONST              62 ((None, None, None, None, None))
                      586 LOAD_CONST              23 ('to')
          
          286         588 LOAD_NAME                3 (str)
          
          284         590 LOAD_CONST              32 ('image')
          
          287         592 LOAD_NAME                3 (str)
@@ -495,15 +496,15 @@
          
          347         678 NOP
          
          348         680 NOP
          
          349         682 NOP
          
-         341         684 LOAD_CONST              60 ((None, None, None, None, None))
+         341         684 LOAD_CONST              62 ((None, None, None, None, None))
                      686 LOAD_CONST              23 ('to')
          
          343         688 LOAD_NAME                3 (str)
          
          341         690 LOAD_CONST              37 ('video')
          
          344         692 LOAD_NAME                3 (str)
@@ -559,15 +560,15 @@
          
          405         780 NOP
          
          406         782 NOP
          
          407         784 NOP
          
-         398         786 LOAD_CONST              61 ((None, None, None, None, None, None))
+         398         786 LOAD_CONST              63 ((None, None, None, None, None, None))
                      788 LOAD_CONST              23 ('to')
          
          400         790 LOAD_NAME                3 (str)
          
          398         792 LOAD_CONST              39 ('document')
          
          401         794 LOAD_NAME                3 (str)
@@ -615,15 +616,15 @@
          398         874 BUILD_TUPLE             16
                      876 LOAD_CONST              41 (<code object send_document, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 398>)
                      878 MAKE_FUNCTION            5 (defaults, annotations)
                      880 STORE_NAME              32 (send_document)
          
          465         882 NOP
          
-         461         884 LOAD_CONST              58 ((None,))
+         461         884 LOAD_CONST              60 ((None,))
                      886 LOAD_CONST              23 ('to')
          
          463         888 LOAD_NAME                3 (str)
          
          461         890 LOAD_CONST              42 ('audio')
          
          464         892 LOAD_NAME                3 (str)
@@ -645,15 +646,15 @@
                      918 MAKE_FUNCTION            5 (defaults, annotations)
                      920 STORE_NAME              33 (send_audio)
          
          496         922 NOP
          
          497         924 NOP
          
-         492         926 LOAD_CONST              62 ((False, None))
+         492         926 LOAD_CONST              64 ((False, None))
                      928 LOAD_CONST              23 ('to')
          
          494         930 LOAD_NAME                3 (str)
          
          492         932 LOAD_CONST              44 ('sticker')
          
          495         934 LOAD_NAME                3 (str)
@@ -675,104 +676,134 @@
          498         958 LOAD_NAME                3 (str)
          
          492         960 BUILD_TUPLE             10
                      962 LOAD_CONST              46 (<code object send_sticker, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 492>)
                      964 MAKE_FUNCTION            5 (defaults, annotations)
                      966 STORE_NAME              34 (send_sticker)
          
-         526         968 LOAD_CONST              23 ('to')
+         528         968 LOAD_CONST              23 ('to')
          
-         528         970 LOAD_NAME                3 (str)
+         530         970 LOAD_NAME                3 (str)
          
-         526         972 LOAD_CONST              47 ('emoji')
+         528         972 LOAD_CONST              47 ('emoji')
          
-         529         974 LOAD_NAME                3 (str)
+         531         974 LOAD_NAME                3 (str)
          
-         526         976 LOAD_CONST              48 ('message_id')
+         528         976 LOAD_CONST              48 ('message_id')
          
-         530         978 LOAD_NAME                3 (str)
+         532         978 LOAD_NAME                3 (str)
          
-         526         980 LOAD_CONST              30 ('return')
+         528         980 LOAD_CONST              30 ('return')
          
-         531         982 LOAD_NAME                3 (str)
+         533         982 LOAD_NAME                3 (str)
          
-         526         984 BUILD_TUPLE              8
-                     986 LOAD_CONST              49 (<code object send_reaction, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 526>)
+         528         984 BUILD_TUPLE              8
+                     986 LOAD_CONST              49 (<code object send_reaction, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 528>)
                      988 MAKE_FUNCTION            4 (annotations)
                      990 STORE_NAME              35 (send_reaction)
          
-         562         992 NOP
+         559         992 LOAD_CONST              23 ('to')
          
-         563         994 NOP
+         561         994 LOAD_NAME                3 (str)
          
-         557         996 LOAD_CONST              63 ((None, None))
-                     998 LOAD_CONST              23 ('to')
+         559         996 LOAD_CONST              48 ('message_id')
          
-         559        1000 LOAD_NAME                3 (str)
+         562         998 LOAD_NAME                3 (str)
          
-         557        1002 LOAD_CONST              50 ('latitude')
+         559        1000 LOAD_CONST              30 ('return')
          
-         560        1004 LOAD_NAME                6 (float)
+         563        1002 LOAD_NAME                3 (str)
          
-         557        1006 LOAD_CONST              51 ('longitude')
+         559        1004 BUILD_TUPLE              6
+                    1006 LOAD_CONST              50 (<code object remove_reaction, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 559>)
+                    1008 MAKE_FUNCTION            4 (annotations)
+                    1010 STORE_NAME              36 (remove_reaction)
          
-         561        1008 LOAD_NAME                6 (float)
+         585        1012 NOP
          
-         557        1010 LOAD_CONST              52 ('name')
+         586        1014 NOP
          
-         562        1012 LOAD_NAME                3 (str)
-                    1014 LOAD_CONST               1 (None)
-                    1016 BINARY_OP                7 (|)
+         580        1016 LOAD_CONST              65 ((None, None))
+                    1018 LOAD_CONST              23 ('to')
          
-         557        1020 LOAD_CONST              53 ('address')
+         582        1020 LOAD_NAME                3 (str)
          
-         563        1022 LOAD_NAME                3 (str)
-                    1024 LOAD_CONST               1 (None)
-                    1026 BINARY_OP                7 (|)
+         580        1022 LOAD_CONST              51 ('latitude')
          
-         557        1030 LOAD_CONST              30 ('return')
+         583        1024 LOAD_NAME                6 (float)
          
-         564        1032 LOAD_NAME                3 (str)
+         580        1026 LOAD_CONST              52 ('longitude')
          
-         557        1034 BUILD_TUPLE             12
-                    1036 LOAD_CONST              54 (<code object send_location, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 557>)
-                    1038 MAKE_FUNCTION            5 (defaults, annotations)
-                    1040 STORE_NAME              36 (send_location)
+         584        1028 LOAD_NAME                6 (float)
          
-         597        1042 NOP
+         580        1030 LOAD_CONST              53 ('name')
          
-         593        1044 LOAD_CONST              58 ((None,))
-                    1046 LOAD_CONST              23 ('to')
+         585        1032 LOAD_NAME                3 (str)
+                    1034 LOAD_CONST               1 (None)
+                    1036 BINARY_OP                7 (|)
          
-         595        1048 LOAD_NAME                3 (str)
+         580        1040 LOAD_CONST              54 ('address')
          
-         593        1050 LOAD_CONST              55 ('contact')
+         586        1042 LOAD_NAME                3 (str)
+                    1044 LOAD_CONST               1 (None)
+                    1046 BINARY_OP                7 (|)
          
-         596        1052 LOAD_NAME               37 (Contact)
-                    1054 LOAD_NAME               12 (Iterable)
-                    1056 LOAD_NAME               37 (Contact)
-                    1058 BINARY_SUBSCR
-                    1068 BINARY_OP                7 (|)
+         580        1050 LOAD_CONST              30 ('return')
          
-         593        1072 LOAD_CONST              26 ('reply_to_message_id')
+         587        1052 LOAD_NAME                3 (str)
          
-         597        1074 LOAD_NAME                3 (str)
-                    1076 LOAD_CONST               1 (None)
-                    1078 BINARY_OP                7 (|)
+         580        1054 BUILD_TUPLE             12
+                    1056 LOAD_CONST              55 (<code object send_location, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 580>)
+                    1058 MAKE_FUNCTION            5 (defaults, annotations)
+                    1060 STORE_NAME              37 (send_location)
          
-         593        1082 LOAD_CONST              30 ('return')
+         620        1062 NOP
          
-         598        1084 LOAD_NAME                3 (str)
+         616        1064 LOAD_CONST              60 ((None,))
+                    1066 LOAD_CONST              23 ('to')
          
-         593        1086 BUILD_TUPLE              8
-                    1088 LOAD_CONST              56 (<code object send_contact, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 593>)
-                    1090 MAKE_FUNCTION            5 (defaults, annotations)
-                    1092 STORE_NAME              38 (send_contact)
-                    1094 LOAD_CONST               1 (None)
-                    1096 RETURN_VALUE
+         618        1068 LOAD_NAME                3 (str)
+         
+         616        1070 LOAD_CONST              56 ('contact')
+         
+         619        1072 LOAD_NAME               38 (Contact)
+                    1074 LOAD_NAME               12 (Iterable)
+                    1076 LOAD_NAME               38 (Contact)
+                    1078 BINARY_SUBSCR
+                    1088 BINARY_OP                7 (|)
+         
+         616        1092 LOAD_CONST              26 ('reply_to_message_id')
+         
+         620        1094 LOAD_NAME                3 (str)
+                    1096 LOAD_CONST               1 (None)
+                    1098 BINARY_OP                7 (|)
+         
+         616        1102 LOAD_CONST              30 ('return')
+         
+         621        1104 LOAD_NAME                3 (str)
+         
+         616        1106 BUILD_TUPLE              8
+                    1108 LOAD_CONST              57 (<code object send_contact, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 616>)
+                    1110 MAKE_FUNCTION            5 (defaults, annotations)
+                    1112 STORE_NAME              39 (send_contact)
+         
+         652        1114 LOAD_CONST              48 ('message_id')
+         
+         654        1116 LOAD_NAME                3 (str)
+         
+         652        1118 LOAD_CONST              30 ('return')
+         
+         655        1120 LOAD_NAME               15 (bool)
+         
+         652        1122 BUILD_TUPLE              4
+                    1124 LOAD_CONST              58 (<code object mark_message_as_read, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 652>)
+                    1126 MAKE_FUNCTION            4 (annotations)
+                    1128 STORE_NAME              40 (mark_message_as_read)
+                    1130 LOAD_CONST               1 (None)
+                    1132 RETURN_VALUE
          consts
             'WhatsApp'
             None
             '/pywa'
             'https://graph.facebook.com'
             17.0
             'phone_id'
@@ -1417,15 +1448,15 @@
                281         122 LOAD_FAST                7 (footer)
                
                273         124 KW_NAMES                 5
                            126 PRECALL                  5
                            130 CALL                     5
                            140 RETURN_VALUE
                consts
-                  '\n        Send a message to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_message(\n            ...     to="1234567890",\n            ...     text="Hello from PyWa! (https://github.com/david-lev/pywa)",\n            ...     preview_url=True,\n            ... )\n\n        Example with keyboard buttons:\n\n            >>> wa.send_message(\n            ...     to="1234567890",\n            ...     header="Hello from PyWa!",\n            ...     text="What can I help you with?",\n            ...     keyboard=[\n            ...         InlineButton("Help", data="help"),\n            ...         InlineButton("About", data="about"),\n            ...     ],\n            ...     footer="Powered by PyWa",\n            ... )\n\n        Example with a section list:\n\n            >>> wa.send_message(\n            ...     to="1234567890",\n            ...     header="Hello from PyWa!",\n            ...     text="What can I help you with?",\n            ...     keyboard=SectionList(\n            ...         button_title="Choose an option",\n            ...         sections=[\n            ...             Section(\n            ...                 title="Help",\n            ...                 rows=[\n            ...                     SectionRow(\n            ...                         title="Help",\n            ...                         callback_data="help",\n            ...                         description="Get help with PyWa",\n            ...                     ),\n            ...                     SectionRow(\n            ...                         title="About",\n            ...                         callback_data="about",\n            ...                         description="Learn more about PyWa",\n            ...                     ),\n            ...                 ],\n            ...             ),\n            ...            Section(\n            ...                 title="Other",\n            ...                 rows=[\n            ...                     SectionRow(\n            ...                         title="GitHub",\n            ...                         callback_data="github",\n            ...                         description="View the PyWa GitHub repository",\n            ...                     ),\n            ...                 ],\n            ...             ),\n            ...         ],\n            ...     ),\n            ...     footer="Powered by PyWa",\n            ... )\n\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            text: The text to send.\n            preview_url: Whether to show a preview of the URL in the message (if any).\n            reply_to_message_id: The message ID to reply to (optional).\n            keyboard: The keyboard to send with the message (optional).\n            header: The header of the message (if keyboard is provided, optional).\n            footer: The footer of the message (if keyboard is provided, optional).\n\n        Returns:\n            The message ID of the sent message.\n        '
+                  '\n        Send a message to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_message(\n            ...     to="1234567890",\n            ...     text="Hello from PyWa! (https://github.com/david-lev/pywa)",\n            ...     preview_url=True,\n            ... )\n\n        Example with keyboard buttons:\n\n            >>> wa.send_message(\n            ...     to="1234567890",\n            ...     header="Hello from PyWa!",\n            ...     text="What can I help you with?",\n            ...     keyboard=[\n            ...         InlineButton("Help", data="help"),\n            ...         InlineButton("About", data="about"),\n            ...     ],\n            ...     footer="Powered by PyWa",\n            ... )\n\n        Example with a section list:\n\n            >>> wa.send_message(\n            ...     to="1234567890",\n            ...     header="Hello from PyWa!",\n            ...     text="What can I help you with?",\n            ...     keyboard=SectionList(\n            ...         button_title="Choose an option",\n            ...         sections=[\n            ...             Section(\n            ...                 title="Help",\n            ...                 rows=[\n            ...                     SectionRow(\n            ...                         title="Help",\n            ...                         callback_data="help",\n            ...                         description="Get help with PyWa",\n            ...                     ),\n            ...                     SectionRow(\n            ...                         title="About",\n            ...                         callback_data="about",\n            ...                         description="Learn more about PyWa",\n            ...                     ),\n            ...                 ],\n            ...             ),\n            ...            Section(\n            ...                 title="Other",\n            ...                 rows=[\n            ...                     SectionRow(\n            ...                         title="GitHub",\n            ...                         callback_data="github",\n            ...                         description="View the PyWa GitHub repository",\n            ...                     ),\n            ...                 ],\n            ...             ),\n            ...         ],\n            ...     ),\n            ...     footer="Powered by PyWa",\n            ... )\n\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            text: The text to send (markdown allowed, max 4096 characters).\n            preview_url: Whether to show a preview of the URL in the message (if any).\n            reply_to_message_id: The message ID to reply to (optional).\n            keyboard: The keyboard to send with the message (optional).\n            header: The header of the message (if keyboard is provided, optional, up to 60 characters, no markdown allowed).\n            footer: The footer of the message (if keyboard is provided, optional, up to 60 characters, markdown has no effect).\n\n        Returns:\n            The message ID of the sent message.\n        '
                   ('to', 'text', 'preview_url', 'reply_to_message_id')
                   'text'
                   ('type', 'text')
                   None
                   ('to', 'keyboard', 'header', 'body', 'footer')
                names      ('api', 'send_text_message', 'send_interactive_message')
                varnames   ('self', 'to', 'text', 'preview_url', 'reply_to_message_id', 'keyboard', 'header', 'footer')
@@ -1525,15 +1556,15 @@
                338         210 LOAD_FAST                4 (reply_to_message_id)
                
                327         212 KW_NAMES                 8
                            214 PRECALL                  6
                            218 CALL                     6
                            228 RETURN_VALUE
                consts
-                  '\n        Send an image to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_image(\n            ...     to="1234567890",\n            ...     image="https://example.com/image.png",\n            ...     caption="This is an image!",\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            image: The image to send (either a URL or a file ID).\n            caption: The caption of the image (optional).\n            reply_to_message_id: The message ID to reply to (optional).\n            buttons: The buttons to send with the image (optional).\n            body: The body of the message (if buttons are provided, optional).\n            footer: The footer of the message (if buttons are provided, optional).\n\n        Returns:\n            The message ID of the sent image.\n        '
+                  '\n        Send an image to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_image(\n            ...     to="1234567890",\n            ...     image="https://example.com/image.png",\n            ...     caption="This is an image!",\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            image: The image to send (either a URL or a file ID).\n            caption: The caption of the image (optional, markdown allowed).\n            reply_to_message_id: The message ID to reply to (optional).\n            buttons: The buttons to send with the image (optional).\n            body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).\n            footer: The footer of the message (if buttons is provided, optional, markdown has no effect).\n\n        Returns:\n            The message ID of the sent image.\n        '
                   'image'
                   ('to', 'media_id_or_url', 'media_type', 'reply_to_message_id', 'caption')
                   'Either body or caption must be provided when sending an image with buttons.'
                   ('https://', 'http://')
                   'link'
                   'id'
                   ('type', 'image')
@@ -1633,15 +1664,15 @@
                395         210 LOAD_FAST                4 (reply_to_message_id)
                
                384         212 KW_NAMES                 8
                            214 PRECALL                  6
                            218 CALL                     6
                            228 RETURN_VALUE
                consts
-                  '\n        Send a video to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_video(\n            ...     to="1234567890",\n            ...     video="https://example.com/video.mp4",\n            ...     caption="This is a video",\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            video: The video to send (either a URL or a file ID).\n            caption: The caption of the video (optional).\n            reply_to_message_id: The message ID to reply to (optional).\n            buttons: The buttons to send with the video (optional).\n            body: The body of the message (if buttons are provided, optional).\n            footer: The footer of the message (if buttons are provided, optional).\n\n        Returns:\n            The message ID of the sent message.\n        '
+                  '\n        Send a video to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_video(\n            ...     to="1234567890",\n            ...     video="https://example.com/video.mp4",\n            ...     caption="This is a video",\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            video: The video to send (either a URL or a file ID).\n            caption: The caption of the video (optional, markdown allowed).\n            reply_to_message_id: The message ID to reply to (optional).\n            buttons: The buttons to send with the video (optional).\n            body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).\n            footer: The footer of the message (if buttons is provided, optional, markdown has no effect).\n\n        Returns:\n            The message ID of the sent message.\n        '
                   'video'
                   ('to', 'media_id_or_url', 'media_type', 'reply_to_message_id', 'caption')
                   'Either body or caption must be provided when sending a video with buttons.'
                   ('https://', 'http://')
                   'link'
                   'id'
                   ('type', 'video')
@@ -1747,15 +1778,15 @@
                458         216 LOAD_FAST                5 (reply_to_message_id)
                
                446         218 KW_NAMES                 9
                            220 PRECALL                  6
                            224 CALL                     6
                            234 RETURN_VALUE
                consts
-                  '\n        Send a document to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_document(\n            ...     to="1234567890",\n            ...     document="https://example.com/example_123.pdf",\n            ...     filename="Example PDF",\n            ...     caption="Example PDF"\n            ... )\n\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            document: The document to send (either a URL or a file ID).\n            filename: The filename of the document (optional).\n            caption: The caption of the document (optional).\n            reply_to_message_id: The message ID to reply to (optional).\n            buttons: The buttons to send with the document (optional).\n            body: The body of the message (if buttons are provided, optional).\n            footer: The footer of the message (if buttons are provided, optional).\n\n        Returns:\n            The message ID of the sent message.\n        '
+                  '\n        Send a document to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_document(\n            ...     to="1234567890",\n            ...     document="https://example.com/example_123.pdf",\n            ...     filename="Example PDF",\n            ...     caption="Example PDF"\n            ... )\n\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            document: The document to send (either a URL or a file ID).\n            filename: The filename of the document (optional, The extension of the filename will specify what format the document is displayed as in WhatsApp).\n            caption: The caption of the document (optional).\n            reply_to_message_id: The message ID to reply to (optional).\n            buttons: The buttons to send with the document (optional).\n            body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).\n            footer: The footer of the message (if buttons is provided, optional, markdown has no effect).\n\n        Returns:\n            The message ID of the sent message.\n        '
                   'document'
                   ('to', 'media_id_or_url', 'media_type', 'reply_to_message_id', 'filename', 'caption')
                   'Either body or caption must be provided when sending a document with buttons.'
                   ('https://', 'http://')
                   'link'
                   'id'
                   'filename'
@@ -1820,181 +1851,247 @@
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c0264017c047c03ac02a6050000ab050000000000
                   0000005300
                492           0 RESUME                   0
                
-               518           2 LOAD_FAST                0 (self)
+               520           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_media)
                
-               519          36 LOAD_FAST                1 (to)
+               521          36 LOAD_FAST                1 (to)
                
-               520          38 LOAD_FAST                2 (sticker)
+               522          38 LOAD_FAST                2 (sticker)
                
-               521          40 LOAD_CONST               1 ('sticker')
+               523          40 LOAD_CONST               1 ('sticker')
                
-               522          42 LOAD_FAST                4 (reply_to_message_id)
+               524          42 LOAD_FAST                4 (reply_to_message_id)
                
-               523          44 LOAD_FAST                3 (animated)
+               525          44 LOAD_FAST                3 (animated)
                
-               518          46 KW_NAMES                 2
+               520          46 KW_NAMES                 2
                             48 PRECALL                  5
                             52 CALL                     5
                             62 RETURN_VALUE
                consts
-                  "\n        Send a sticker to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_sticker(\n            ...     to='1234567890',\n            ...     sticker='https://example.com/sticker.webp',\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            sticker: The sticker to send (either a URL or a file ID).\n            animated: Whether the sticker is animated (optional).\n            reply_to_message_id: The message ID to reply to (optional).\n\n        Returns:\n            The message ID of the sent message.\n        "
+                  "\n        Send a sticker to a WhatsApp user.\n            - A static sticker needs to be 512x512 pixels and cannot exceed 100 KB.\n            - An animated sticker must be 512x512 pixels and cannot exceed 500 KB.\n\n        Example:\n\n            >>> wa.send_sticker(\n            ...     to='1234567890',\n            ...     sticker='https://example.com/sticker.webp',\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            sticker: The sticker to send (either a URL or a file ID).\n            animated: Whether the sticker is animated (optional).\n            reply_to_message_id: The message ID to reply to (optional).\n\n        Returns:\n            The message ID of the sent message.\n        "
                   'sticker'
                   ('to', 'media_id_or_url', 'media_type', 'reply_to_message_id', 'animated')
                names      ('api', 'send_media')
                varnames   ('self', 'to', 'sticker', 'animated', 'reply_to_message_id')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_sticker'
                firstlineno 492
-               lnotab 0x021a2201020102010201020102fb
+               lnotab 0x021c2201020102010201020102fb
             'emoji'
             'message_id'
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c027c03ac01a6030000ab03000000000000000053
                   00
-               526           0 RESUME                   0
+               528           0 RESUME                   0
                
-               551           2 LOAD_FAST                0 (self)
+               553           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_reaction)
                
-               552          36 LOAD_FAST                1 (to)
+               554          36 LOAD_FAST                1 (to)
                
-               553          38 LOAD_FAST                2 (emoji)
+               555          38 LOAD_FAST                2 (emoji)
                
-               554          40 LOAD_FAST                3 (message_id)
+               556          40 LOAD_FAST                3 (message_id)
                
-               551          42 KW_NAMES                 1
+               553          42 KW_NAMES                 1
                             44 PRECALL                  3
                             48 CALL                     3
                             58 RETURN_VALUE
                consts
                   "\n        React to a message with an emoji.\n\n        Example:\n\n            >>> wa.send_reaction(\n            ...     to='1234567890',\n            ...     emoji='👍',\n            ...     message_id='wamid.XXX='\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            emoji: The emoji to react with.\n            message_id: The message ID to react to.\n\n        Returns:\n            The message ID of the reaction.\n        "
                   ('to', 'emoji', 'message_id')
                names      ('api', 'send_reaction')
                varnames   ('self', 'to', 'emoji', 'message_id')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_reaction'
-               firstlineno 526
+               firstlineno 528
                lnotab 0x021922010201020102fd
+            code
+               argcount  : 3
+               nlocals   : 3
+               stacksize : 5
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000007c017c026401ac02a6030000ab03000000000000000053
+                  00
+               559           0 RESUME                   0
+               
+               574           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (api)
+                            14 LOAD_METHOD              1 (send_reaction)
+               
+               575          36 LOAD_FAST                1 (to)
+               
+               576          38 LOAD_FAST                2 (message_id)
+               
+               577          40 LOAD_CONST               1 ('')
+               
+               574          42 KW_NAMES                 2
+                            44 PRECALL                  3
+                            48 CALL                     3
+                            58 RETURN_VALUE
+               consts
+                  "\n        Remove a reaction from a message.\n\n        Example:\n\n            >>> wa.remove_reaction(\n            ...     to='1234567890',\n            ...     message_id='wamid.XXX='\n            ... )\n        "
+                  ''
+                  ('to', 'message_id', 'emoji')
+               names      ('api', 'send_reaction')
+               varnames   ('self', 'to', 'message_id')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
+               name       'remove_reaction'
+               firstlineno 559
+               lnotab 0x020f22010201020102fd
             'latitude'
             'longitude'
             'name'
             'address'
             code
                argcount  : 6
                nlocals   : 6
                stacksize : 7
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c027c037c047c05ac01a6050000ab050000000000
                   0000005300
-               557           0 RESUME                   0
+               580           0 RESUME                   0
                
-               585           2 LOAD_FAST                0 (self)
+               608           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_location)
                
-               586          36 LOAD_FAST                1 (to)
+               609          36 LOAD_FAST                1 (to)
                
-               587          38 LOAD_FAST                2 (latitude)
+               610          38 LOAD_FAST                2 (latitude)
                
-               588          40 LOAD_FAST                3 (longitude)
+               611          40 LOAD_FAST                3 (longitude)
                
-               589          42 LOAD_FAST                4 (name)
+               612          42 LOAD_FAST                4 (name)
                
-               590          44 LOAD_FAST                5 (address)
+               613          44 LOAD_FAST                5 (address)
                
-               585          46 KW_NAMES                 1
+               608          46 KW_NAMES                 1
                             48 PRECALL                  5
                             52 CALL                     5
                             62 RETURN_VALUE
                consts
                   "\n        Send a location to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_location(\n            ...     to='1234567890',\n            ...     latitude=37.4847483695049,\n            ...     longitude=--122.1473373086664,\n            ...     name='WhatsApp HQ',\n            ...     address='Menlo Park, 1601 Willow Rd, United States',\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            latitude: The latitude of the location.\n            longitude: The longitude of the location.\n            name: The name of the location (optional).\n            address: The address of the location (optional).\n        "
                   ('to', 'latitude', 'longitude', 'name', 'address')
                names      ('api', 'send_location')
                varnames   ('self', 'to', 'latitude', 'longitude', 'name', 'address')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_location'
-               firstlineno 557
+               firstlineno 580
                lnotab 0x021c2201020102010201020102fb
             'contact'
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 7
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017405000000000000000000007c0274060000000000
                   0000000000a6020000ab02000000000000000072027c026e027c0267017c
                   03ac01a6030000ab0300000000000000005300
-               593           0 RESUME                   0
+               616           0 RESUME                   0
                
-               623           2 LOAD_FAST                0 (self)
+               646           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_contacts)
                
-               624          36 LOAD_FAST                1 (to)
+               647          36 LOAD_FAST                1 (to)
                
-               625          38 LOAD_GLOBAL              5 (NULL + isinstance)
+               648          38 LOAD_GLOBAL              5 (NULL + isinstance)
                             50 LOAD_FAST                2 (contact)
                             52 LOAD_GLOBAL              6 (Iterable)
                             64 PRECALL                  2
                             68 CALL                     2
                             78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
                             80 LOAD_FAST                2 (contact)
                             82 JUMP_FORWARD             2 (to 88)
                        >>   84 LOAD_FAST                2 (contact)
                             86 BUILD_LIST               1
                
-               626     >>   88 LOAD_FAST                3 (reply_to_message_id)
+               649     >>   88 LOAD_FAST                3 (reply_to_message_id)
                
-               623          90 KW_NAMES                 1
+               646          90 KW_NAMES                 1
                             92 PRECALL                  3
                             96 CALL                     3
                            106 RETURN_VALUE
                consts
                   "\n        Send a contact to a WhatsApp user.\n\n        Example:\n\n            >>> from pywa.types import Contact\n            >>> wa.send_contact(\n            ...     to='1234567890',\n            ...     contact=Contact(\n            ...         name=Contact.Name(formatted_name='David Lev', first_name='David'),\n            ...         phones=[Contact.Phone(phone='1234567890', wa_id='1234567890', type='MOBILE')],\n            ...         emails=[Contact.Email(email='test@test.com', type='WORK')],\n            ...         urls=[Contact.Url(url='https://exmaple.com', type='HOME')],\n            ...      )\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            contact: The contact/s to send.\n            reply_to_message_id: The message ID to reply to (optional).\n\n        Returns:\n            The message ID of the sent message.\n        "
                   ('to', 'contacts', 'reply_to_message_id')
                names      ('api', 'send_contacts', 'isinstance', 'Iterable')
                varnames   ('self', 'to', 'contact', 'reply_to_message_id')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_contact'
-               firstlineno 593
+               firstlineno 616
                lnotab 0x021e22010201320102fd
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000007c01ac01a6010000ab0100000000000000005300
+               652           0 RESUME                   0
+               
+               665           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (api)
+                            14 LOAD_METHOD              1 (mark_message_as_read)
+                            36 LOAD_FAST                1 (message_id)
+                            38 KW_NAMES                 1
+                            40 PRECALL                  1
+                            44 CALL                     1
+                            54 RETURN_VALUE
+               consts
+                  '\n        Mark a message as read.\n\n        Args:\n            message_id: The message ID to mark as read.\n\n        Returns:\n            Whether the message was marked as read.\n        '
+                  ('message_id',)
+               names      ('api', 'mark_message_as_read')
+               varnames   ('self', 'message_id')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
+               name       'mark_message_as_read'
+               firstlineno 652
+               lnotab 0x020d
             (None, '/pywa', None, 'https://graph.facebook.com', 17.0, None)
             (None,)
             (False, None, None, None, None)
             (None, None, None, None, None)
             (None, None, None, None, None, None)
             (False, None)
             (None, None)
-         names      ('__name__', '__module__', '__qualname__', 'str', 'int', 'Any', 'float', 'requests', 'Session', '__init__', 'Handler', 'add_handler', 'Iterable', 'Callable', 'dict', 'bool', 'on_raw_update', 'Message', 'on_message', 'CallbackButton', 'on_callback_button', 'CallbackSelection', 'on_callback_selection', 'MessageStatus', 'on_message_status_change', 'list', 'InlineButton', 'SectionList', 'send_message', 'bytes', 'send_image', 'send_video', 'send_document', 'send_audio', 'send_sticker', 'send_reaction', 'send_location', 'Contact', 'send_contact')
+         names      ('__name__', '__module__', '__qualname__', 'str', 'int', 'Any', 'float', 'requests', 'Session', '__init__', 'Handler', 'add_handler', 'Iterable', 'Callable', 'dict', 'bool', 'on_raw_update', 'Message', 'on_message', 'CallbackButton', 'on_callback_button', 'CallbackSelection', 'on_callback_selection', 'MessageStatus', 'on_message_status_change', 'list', 'InlineButton', 'SectionList', 'send_message', 'bytes', 'send_image', 'send_video', 'send_document', 'send_audio', 'send_sticker', 'send_reaction', 'remove_reaction', 'send_location', 'Contact', 'send_contact', 'mark_message_as_read')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
          name       'WhatsApp'
          firstlineno 11
          lnotab
@@ -2005,17 +2102,18 @@
             fe020302fd020402fc020508fb02061afa020708f9020808f8020902f708
             6c020102010201020102f8040202fe020308fd020408fc020508fb020614
             fa020708f9020808f8020902f7083d020102010201020102f8040202fe02
             0308fd020408fc020508fb020614fa020708f9020808f8020902f7083d02
             01020102010201020102f7040202fe020308fd020408fc020508fb020608
             fa020714f9020808f8020908f7084302fc040202fe020308fd020408fc02
             0502fb0823020102fb040202fe020308fd020402fc020508fb020602fa08
-            22020202fe020302fd020402fc020502fb0824020102fa040202fe020302
-            fd020402fc020508fb020608fa020702f9082802fc040202fe020314fd02
-            0408fc020502fb
+            24020202fe020302fd020402fc020502fb081f020202fe020302fd020402
+            fc081a020102fa040202fe020302fd020402fc020508fb020608fa020702
+            f9082802fc040202fe020314fd020408fc020502fb0824020202fe020302
+            fd
       'WhatsApp'
    names      ('collections', 'requests', 'typing', 'Callable', 'Any', 'Iterable', 'pywa.api', 'WhatsAppCloudApi', 'pywa.handlers', 'Handler', 'MessageHandler', 'ButtonCallbackHandler', 'SelectionCallbackHandler', 'RawUpdateHandler', 'MessageStatusHandler', 'pywa.types', 'InlineButton', 'SectionList', 'Message', 'CallbackButton', 'CallbackSelection', 'MessageStatus', 'Contact', 'pywa', 'webhook', 'WhatsApp')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
    name       '<module>'
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/filters.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,31 +1,32 @@
 magic:    0xa70d0d0a
-moddate:  0x94089264 (Tue Jun 20 20:14:12 2023 UTC)
-files sz: 12393
+moddate:  0x9e619464 (Thu Jun 22 14:58:38 2023 UTC)
+files sz: 11023
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 16777216
    code
       0x970064005a00640164026c016d025a020100640164036c035a03640164
-      046c046d055a056d065a066d075a070100640164056c086d095a0a6d0b5a
-      0c6d0d5a0e6d0f5a106d115a116d125a120100640164066c136d145a1401
-      0065067206640164076c136d155a16010002004700640884006409a60200
-      00ab0200000000000000005a1702004700640a8400640ba6020000ab0200
-      000000000000005a1802004700640c8400640da6020000ab020000000000
-      0000005a1902004700640e8400640fa6020000ab0200000000000000005a
-      1a02004700641084006411a6020000ab0200000000000000005a1b020047
-      00641284006413a6020000ab0200000000000000005a1c02004700641484
-      006415a6020000ab0200000000000000005a1d02004700641684006417a6
-      020000ab0200000000000000005a1e02004700641884006419a6020000ab
-      0200000000000000005a1f02004700641a8400641ba6020000ab02000000
-      00000000005a2002004700641c8400641da6020000ab0200000000000000
-      005a2102004700641e8400641fa6020000ab0200000000000000005a2264
-      035300
+      046c046d055a056d065a066d075a070100640164056c086d095a09010064
+      0164066c0a6d0b5a0c6d0d5a0e6d0f5a106d115a126d135a136d145a1401
+      0065067206640164076c086d155a16010064085a17020065036a18000000
+      00000000006409a6010000ab0100000000000000005a1902004700640a84
+      00640ba6020000ab0200000000000000005a1a02004700640c8400640da6
+      020000ab0200000000000000005a1b02004700640e8400640fa6020000ab
+      0200000000000000005a1c02004700641084006411a6020000ab02000000
+      00000000005a1d02004700641284006413a6020000ab0200000000000000
+      005a1e02004700641484006415a6020000ab0200000000000000005a1f02
+      004700641684006417a6020000ab0200000000000000005a200200470064
+      1884006419a6020000ab0200000000000000005a2102004700641a840064
+      1ba6020000ab0200000000000000005a2202004700641c8400641da60200
+      00ab0200000000000000005a2302004700641e8400641fa6020000ab0200
+      000000000000005a2402004700642084006421a6020000ab020000000000
+      0000005a2564035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Usefully filters to use in your handlers.')
                  4 STORE_NAME               0 (__doc__)
    
      2           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('annotations',))
@@ -47,656 +48,604 @@
                 36 IMPORT_FROM              6 (TYPE_CHECKING)
                 38 STORE_NAME               6 (TYPE_CHECKING)
                 40 IMPORT_FROM              7 (Iterable)
                 42 STORE_NAME               7 (Iterable)
                 44 POP_TOP
    
      6          46 LOAD_CONST               1 (0)
-                48 LOAD_CONST               5 (('MessageType', 'Message', 'MessageStatus', 'MessageStatusType', 'CallbackButton', 'CallbackSelection'))
-                50 IMPORT_NAME              8 (pywa.types)
-                52 IMPORT_FROM              9 (MessageType)
-                54 STORE_NAME              10 (Mt)
-                56 IMPORT_FROM             11 (Message)
-                58 STORE_NAME              12 (Msg)
-                60 IMPORT_FROM             13 (MessageStatus)
-                62 STORE_NAME              14 (Ms)
-                64 IMPORT_FROM             15 (MessageStatusType)
-                66 STORE_NAME              16 (Mst)
-                68 IMPORT_FROM             17 (CallbackButton)
-                70 STORE_NAME              17 (CallbackButton)
-                72 IMPORT_FROM             18 (CallbackSelection)
-                74 STORE_NAME              18 (CallbackSelection)
-                76 POP_TOP
+                48 LOAD_CONST               5 (('utils',))
+                50 IMPORT_NAME              8 (pywa)
+                52 IMPORT_FROM              9 (utils)
+                54 STORE_NAME               9 (utils)
+                56 POP_TOP
    
-     8          78 LOAD_CONST               1 (0)
-                80 LOAD_CONST               6 (('utils',))
-                82 IMPORT_NAME             19 (pywa)
-                84 IMPORT_FROM             20 (utils)
-                86 STORE_NAME              20 (utils)
+     7          58 LOAD_CONST               1 (0)
+                60 LOAD_CONST               6 (('MessageType', 'Message', 'MessageStatus', 'MessageStatusType', 'CallbackButton', 'CallbackSelection'))
+                62 IMPORT_NAME             10 (pywa.types)
+                64 IMPORT_FROM             11 (MessageType)
+                66 STORE_NAME              12 (Mt)
+                68 IMPORT_FROM             13 (Message)
+                70 STORE_NAME              14 (Msg)
+                72 IMPORT_FROM             15 (MessageStatus)
+                74 STORE_NAME              16 (Ms)
+                76 IMPORT_FROM             17 (MessageStatusType)
+                78 STORE_NAME              18 (Mst)
+                80 IMPORT_FROM             19 (CallbackButton)
+                82 STORE_NAME              19 (CallbackButton)
+                84 IMPORT_FROM             20 (CallbackSelection)
+                86 STORE_NAME              20 (CallbackSelection)
                 88 POP_TOP
    
     10          90 LOAD_NAME                6 (TYPE_CHECKING)
                 92 POP_JUMP_FORWARD_IF_FALSE     6 (to 106)
    
     11          94 LOAD_CONST               1 (0)
                 96 LOAD_CONST               7 (('WhatsApp',))
-                98 IMPORT_NAME             19 (pywa)
+                98 IMPORT_NAME              8 (pywa)
                100 IMPORT_FROM             21 (WhatsApp)
                102 STORE_NAME              22 (Wa)
                104 POP_TOP
    
-    14     >>  106 PUSH_NULL
-               108 LOAD_BUILD_CLASS
-               110 LOAD_CONST               8 (<code object TextFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 14>)
-               112 MAKE_FUNCTION            0
-               114 LOAD_CONST               9 ('TextFilter')
-               116 PRECALL                  2
-               120 CALL                     2
-               130 STORE_NAME              23 (TextFilter)
+    13     >>  106 LOAD_CONST               8 (('TextFilter', 'ImageFilter', 'VideoFilter', 'AudioFilter', 'DocumentFilter', 'StickerFilter', 'ReactionFilter', 'UnsupportedMsgFilter', 'LocationFilter', 'ContactsFilter', 'CallbackFilter'))
+               108 STORE_NAME              23 (__all__)
    
-    77         132 PUSH_NULL
-               134 LOAD_BUILD_CLASS
-               136 LOAD_CONST              10 (<code object ImageFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 77>)
-               138 MAKE_FUNCTION            0
-               140 LOAD_CONST              11 ('ImageFilter')
-               142 PRECALL                  2
-               146 CALL                     2
-               156 STORE_NAME              24 (ImageFilter)
+    27         110 PUSH_NULL
+               112 LOAD_NAME                3 (re)
+               114 LOAD_ATTR               24 (compile)
+               124 LOAD_CONST               9 ('\\D')
+               126 PRECALL                  1
+               130 CALL                     1
+               140 STORE_NAME              25 (_ONLY_NUMS_RE)
    
-    97         158 PUSH_NULL
-               160 LOAD_BUILD_CLASS
-               162 LOAD_CONST              12 (<code object VideoFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 97>)
-               164 MAKE_FUNCTION            0
-               166 LOAD_CONST              13 ('VideoFilter')
-               168 PRECALL                  2
-               172 CALL                     2
-               182 STORE_NAME              25 (VideoFilter)
+    30         142 PUSH_NULL
+               144 LOAD_BUILD_CLASS
+               146 LOAD_CONST              10 (<code object TextFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 30>)
+               148 MAKE_FUNCTION            0
+               150 LOAD_CONST              11 ('TextFilter')
+               152 PRECALL                  2
+               156 CALL                     2
+               166 STORE_NAME              26 (TextFilter)
    
-   114         184 PUSH_NULL
-               186 LOAD_BUILD_CLASS
-               188 LOAD_CONST              14 (<code object AudioFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 114>)
-               190 MAKE_FUNCTION            0
-               192 LOAD_CONST              15 ('AudioFilter')
-               194 PRECALL                  2
-               198 CALL                     2
-               208 STORE_NAME              26 (AudioFilter)
+    86         168 PUSH_NULL
+               170 LOAD_BUILD_CLASS
+               172 LOAD_CONST              12 (<code object ImageFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 86>)
+               174 MAKE_FUNCTION            0
+               176 LOAD_CONST              13 ('ImageFilter')
+               178 PRECALL                  2
+               182 CALL                     2
+               192 STORE_NAME              27 (ImageFilter)
    
-   137         210 PUSH_NULL
-               212 LOAD_BUILD_CLASS
-               214 LOAD_CONST              16 (<code object DocumentFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 137>)
-               216 MAKE_FUNCTION            0
-               218 LOAD_CONST              17 ('DocumentFilter')
-               220 PRECALL                  2
-               224 CALL                     2
-               234 STORE_NAME              27 (DocumentFilter)
+   106         194 PUSH_NULL
+               196 LOAD_BUILD_CLASS
+               198 LOAD_CONST              14 (<code object VideoFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 106>)
+               200 MAKE_FUNCTION            0
+               202 LOAD_CONST              15 ('VideoFilter')
+               204 PRECALL                  2
+               208 CALL                     2
+               218 STORE_NAME              28 (VideoFilter)
    
-   154         236 PUSH_NULL
-               238 LOAD_BUILD_CLASS
-               240 LOAD_CONST              18 (<code object StickerFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 154>)
-               242 MAKE_FUNCTION            0
-               244 LOAD_CONST              19 ('StickerFilter')
-               246 PRECALL                  2
-               250 CALL                     2
-               260 STORE_NAME              28 (StickerFilter)
+   121         220 PUSH_NULL
+               222 LOAD_BUILD_CLASS
+               224 LOAD_CONST              16 (<code object AudioFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 121>)
+               226 MAKE_FUNCTION            0
+               228 LOAD_CONST              17 ('AudioFilter')
+               230 PRECALL                  2
+               234 CALL                     2
+               244 STORE_NAME              29 (AudioFilter)
    
-   164         262 PUSH_NULL
-               264 LOAD_BUILD_CLASS
-               266 LOAD_CONST              20 (<code object LocationFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 164>)
-               268 MAKE_FUNCTION            0
-               270 LOAD_CONST              21 ('LocationFilter')
-               272 PRECALL                  2
-               276 CALL                     2
-               286 STORE_NAME              29 (LocationFilter)
+   142         246 PUSH_NULL
+               248 LOAD_BUILD_CLASS
+               250 LOAD_CONST              18 (<code object DocumentFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 142>)
+               252 MAKE_FUNCTION            0
+               254 LOAD_CONST              19 ('DocumentFilter')
+               256 PRECALL                  2
+               260 CALL                     2
+               270 STORE_NAME              30 (DocumentFilter)
    
-   192         288 PUSH_NULL
-               290 LOAD_BUILD_CLASS
-               292 LOAD_CONST              22 (<code object ReactionFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 192>)
-               294 MAKE_FUNCTION            0
-               296 LOAD_CONST              23 ('ReactionFilter')
-               298 PRECALL                  2
-               302 CALL                     2
-               312 STORE_NAME              30 (ReactionFilter)
+   157         272 PUSH_NULL
+               274 LOAD_BUILD_CLASS
+               276 LOAD_CONST              20 (<code object StickerFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 157>)
+               278 MAKE_FUNCTION            0
+               280 LOAD_CONST              21 ('StickerFilter')
+               282 PRECALL                  2
+               286 CALL                     2
+               296 STORE_NAME              31 (StickerFilter)
    
-   203         314 PUSH_NULL
-               316 LOAD_BUILD_CLASS
-               318 LOAD_CONST              24 (<code object ContactsFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 203>)
-               320 MAKE_FUNCTION            0
-               322 LOAD_CONST              25 ('ContactsFilter')
-               324 PRECALL                  2
-               328 CALL                     2
-               338 STORE_NAME              31 (ContactsFilter)
+   169         298 PUSH_NULL
+               300 LOAD_BUILD_CLASS
+               302 LOAD_CONST              22 (<code object LocationFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 169>)
+               304 MAKE_FUNCTION            0
+               306 LOAD_CONST              23 ('LocationFilter')
+               308 PRECALL                  2
+               312 CALL                     2
+               322 STORE_NAME              32 (LocationFilter)
    
-   230         340 PUSH_NULL
-               342 LOAD_BUILD_CLASS
-               344 LOAD_CONST              26 (<code object UnsupportedFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 230>)
-               346 MAKE_FUNCTION            0
-               348 LOAD_CONST              27 ('UnsupportedFilter')
-               350 PRECALL                  2
-               354 CALL                     2
-               364 STORE_NAME              32 (UnsupportedFilter)
+   197         324 PUSH_NULL
+               326 LOAD_BUILD_CLASS
+               328 LOAD_CONST              24 (<code object ReactionFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 197>)
+               330 MAKE_FUNCTION            0
+               332 LOAD_CONST              25 ('ReactionFilter')
+               334 PRECALL                  2
+               338 CALL                     2
+               348 STORE_NAME              33 (ReactionFilter)
    
-   237         366 PUSH_NULL
-               368 LOAD_BUILD_CLASS
-               370 LOAD_CONST              28 (<code object CallbackFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 237>)
-               372 MAKE_FUNCTION            0
-               374 LOAD_CONST              29 ('CallbackFilter')
-               376 PRECALL                  2
-               380 CALL                     2
-               390 STORE_NAME              33 (CallbackFilter)
+   211         350 PUSH_NULL
+               352 LOAD_BUILD_CLASS
+               354 LOAD_CONST              26 (<code object ContactsFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 211>)
+               356 MAKE_FUNCTION            0
+               358 LOAD_CONST              27 ('ContactsFilter')
+               360 PRECALL                  2
+               364 CALL                     2
+               374 STORE_NAME              34 (ContactsFilter)
    
-   266         392 PUSH_NULL
-               394 LOAD_BUILD_CLASS
-               396 LOAD_CONST              30 (<code object MessageStatusFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 266>)
-               398 MAKE_FUNCTION            0
-               400 LOAD_CONST              31 ('MessageStatusFilter')
-               402 PRECALL                  2
-               406 CALL                     2
-               416 STORE_NAME              34 (MessageStatusFilter)
-               418 LOAD_CONST               3 (None)
-               420 RETURN_VALUE
+   238         376 PUSH_NULL
+               378 LOAD_BUILD_CLASS
+               380 LOAD_CONST              28 (<code object UnsupportedMsgFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 238>)
+               382 MAKE_FUNCTION            0
+               384 LOAD_CONST              29 ('UnsupportedMsgFilter')
+               386 PRECALL                  2
+               390 CALL                     2
+               400 STORE_NAME              35 (UnsupportedMsgFilter)
+   
+   245         402 PUSH_NULL
+               404 LOAD_BUILD_CLASS
+               406 LOAD_CONST              30 (<code object CallbackFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 245>)
+               408 MAKE_FUNCTION            0
+               410 LOAD_CONST              31 ('CallbackFilter')
+               412 PRECALL                  2
+               416 CALL                     2
+               426 STORE_NAME              36 (CallbackFilter)
+   
+   277         428 PUSH_NULL
+               430 LOAD_BUILD_CLASS
+               432 LOAD_CONST              32 (<code object MessageStatusFilter, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 277>)
+               434 MAKE_FUNCTION            0
+               436 LOAD_CONST              33 ('MessageStatusFilter')
+               438 PRECALL                  2
+               442 CALL                     2
+               452 STORE_NAME              37 (MessageStatusFilter)
+               454 LOAD_CONST               3 (None)
+               456 RETURN_VALUE
    consts
       'Usefully filters to use in your handlers.'
       0
       ('annotations',)
       None
       ('Callable', 'TYPE_CHECKING', 'Iterable')
-      ('MessageType', 'Message', 'MessageStatus', 'MessageStatusType', 'CallbackButton', 'CallbackSelection')
       ('utils',)
+      ('MessageType', 'Message', 'MessageStatus', 'MessageStatusType', 'CallbackButton', 'CallbackSelection')
       ('WhatsApp',)
+      ('TextFilter', 'ImageFilter', 'VideoFilter', 'AudioFilter', 'DocumentFilter', 'StickerFilter', 'ReactionFilter', 'UnsupportedMsgFilter', 'LocationFilter', 'ContactsFilter', 'CallbackFilter')
+      '\\D'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
-            0000000900640584005a066406650564073c0000000900640884005a0764
-            06650564093c0000000900640a84005a0864066505640b3c000000090064
-            0c84005a0964066505640d3c0000000900640e84005a0a640f650564103c
-            0000000900641184005a0b6412650564133c0000000900650c641c641d64
-            1a8405a6000000ab0000000000000000005a0d641b5300
-          14           0 RESUME                   0
+            00000009006506641d64088404a6000000ab0000000000000000005a0765
+            06641d64098404a6000000ab0000000000000000005a086506641d640a84
+            04a6000000ab0000000000000000005a096506641d640b8404a6000000ab
+            0000000000000000005a0a6506640c640d9c01641e64128406a6000000ab
+            0000000000000000005a0b6506641f64158404a6000000ab000000000000
+            0000005a0c6506641664179c016420641b8406a6000000ab000000000000
+            0000005a0d641c5300
+          30           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('TextFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          15          12 LOAD_CONST               1 ('Useful filters for text messages.')
+          31          12 LOAD_CONST               1 ('Useful filters for text messages.')
                       14 STORE_NAME               3 (__doc__)
          
-          17          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 17>)
+          33          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 33>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-          18          32 NOP
+          34          32 NOP
          
-          21          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 21>)
-                      36 MAKE_FUNCTION            0
+          36          34 LOAD_NAME                6 (staticmethod)
          
-          20          38 STORE_NAME               6 (EQUALS)
-                      40 LOAD_CONST               6 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      42 LOAD_NAME                5 (__annotations__)
-                      44 LOAD_CONST               7 ('EQUALS')
-                      46 STORE_SUBSCR
+          37          36 LOAD_CONST              29 (('matches', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                      38 LOAD_CONST               8 (<code object equals, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 36>)
+                      40 MAKE_FUNCTION            4 (annotations)
          
-          25          50 NOP
+          36          42 PRECALL                  0
+                      46 CALL                     0
          
-          28          52 LOAD_CONST               8 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 28>)
-                      54 MAKE_FUNCTION            0
+          37          56 STORE_NAME               7 (equals)
          
-          27          56 STORE_NAME               7 (CONTAINS)
-                      58 LOAD_CONST               6 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      60 LOAD_NAME                5 (__annotations__)
-                      62 LOAD_CONST               9 ('CONTAINS')
-                      64 STORE_SUBSCR
+          41          58 LOAD_NAME                6 (staticmethod)
+         
+          42          60 LOAD_CONST              29 (('matches', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                      62 LOAD_CONST               9 (<code object contains, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 41>)
+                      64 MAKE_FUNCTION            4 (annotations)
+         
+          41          66 PRECALL                  0
+                      70 CALL                     0
+         
+          42          80 STORE_NAME               8 (contains)
+         
+          46          82 LOAD_NAME                6 (staticmethod)
          
-          32          68 NOP
+          47          84 LOAD_CONST              29 (('matches', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                      86 LOAD_CONST              10 (<code object startswith, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 46>)
+                      88 MAKE_FUNCTION            4 (annotations)
          
-          35          70 LOAD_CONST              10 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 35>)
-                      72 MAKE_FUNCTION            0
+          46          90 PRECALL                  0
+                      94 CALL                     0
          
-          34          74 STORE_NAME               8 (STARTS_WITH)
-                      76 LOAD_CONST               6 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      78 LOAD_NAME                5 (__annotations__)
-                      80 LOAD_CONST              11 ('STARTS_WITH')
-                      82 STORE_SUBSCR
+          47         104 STORE_NAME               9 (startswith)
          
-          39          86 NOP
+          51         106 LOAD_NAME                6 (staticmethod)
          
-          42          88 LOAD_CONST              12 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 42>)
-                      90 MAKE_FUNCTION            0
+          52         108 LOAD_CONST              29 (('matches', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                     110 LOAD_CONST              11 (<code object endswith, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 51>)
+                     112 MAKE_FUNCTION            4 (annotations)
          
-          41          92 STORE_NAME               9 (ENDS_WITH)
-                      94 LOAD_CONST               6 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      96 LOAD_NAME                5 (__annotations__)
-                      98 LOAD_CONST              13 ('ENDS_WITH')
-                     100 STORE_SUBSCR
+          51         114 PRECALL                  0
+                     118 CALL                     0
          
-          46         104 NOP
+          52         128 STORE_NAME              10 (endswith)
          
-          49         106 LOAD_CONST              14 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 49>)
-                     108 MAKE_FUNCTION            0
+          56         130 LOAD_NAME                6 (staticmethod)
          
-          48         110 STORE_NAME              10 (REGEX)
-                     112 LOAD_CONST              15 ('Callable[[str | Iterable[str] | re.Pattern | Iterable[re.Pattern]], Callable[[Wa, Msg], bool]]')
-                     114 LOAD_NAME                5 (__annotations__)
-                     116 LOAD_CONST              16 ('REGEX')
-                     118 STORE_SUBSCR
+          57         132 LOAD_CONST              12 (0)
+                     134 LOAD_CONST              13 (('flags',))
+                     136 BUILD_CONST_KEY_MAP      1
+                     138 LOAD_CONST              30 (('patterns', 'str | re.Pattern', 'flags', 'int', 'return', 'Callable[[Wa, Msg], bool]'))
+                     140 LOAD_CONST              18 (<code object regex, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 56>)
+                     142 MAKE_FUNCTION            6 (kwdefaults, annotations)
          
-          53         122 NOP
+          56         144 PRECALL                  0
+                     148 CALL                     0
          
-          56         124 LOAD_CONST              17 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 56>)
-                     126 MAKE_FUNCTION            0
+          57         158 STORE_NAME              11 (regex)
          
-          55         128 STORE_NAME              11 (LEN_BETWEEN)
-                     130 LOAD_CONST              18 ('Callable[[tuple[int, int] | Iterable[tuple[int, int]]], Callable[[Wa, Msg], bool]]')
-                     132 LOAD_NAME                5 (__annotations__)
-                     134 LOAD_CONST              19 ('LEN_BETWEEN')
-                     136 STORE_SUBSCR
+          64         160 LOAD_NAME                6 (staticmethod)
          
-          60         140 NOP
+          65         162 LOAD_CONST              31 (('lengths', 'tuple[int, int]', 'return', 'Callable[[Wa, Msg], bool]'))
+                     164 LOAD_CONST              21 (<code object length, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 64>)
+                     166 MAKE_FUNCTION            4 (annotations)
          
-          62         142 LOAD_NAME               12 (staticmethod)
+          64         168 PRECALL                  0
+                     172 CALL                     0
          
-          63         144 LOAD_CONST              28 (('/',))
-                     146 LOAD_CONST              29 (('cmd', 'str | Iterable[str]', 'prefix', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
-                     148 LOAD_CONST              26 (<code object COMMAND, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 62>)
-                     150 MAKE_FUNCTION            5 (defaults, annotations)
+          65         182 STORE_NAME              12 (length)
          
-          62         152 PRECALL                  0
-                     156 CALL                     0
+          74         184 LOAD_NAME                6 (staticmethod)
          
-          63         166 STORE_NAME              13 (COMMAND)
-                     168 LOAD_CONST              27 (None)
-                     170 RETURN_VALUE
+          75         186 LOAD_CONST              22 ('!')
+                     188 LOAD_CONST              23 (('prefixes',))
+                     190 BUILD_CONST_KEY_MAP      1
+                     192 LOAD_CONST              32 (('cmds', 'str', 'prefixes', 'str | Iterable[str]', 'return', 'Callable[[Wa, Msg], bool]'))
+                     194 LOAD_CONST              27 (<code object command, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 74>)
+                     196 MAKE_FUNCTION            6 (kwdefaults, annotations)
+         
+          74         198 PRECALL                  0
+                     202 CALL                     0
+         
+          75         212 STORE_NAME              13 (command)
+                     214 LOAD_CONST              28 (None)
+                     216 RETURN_VALUE
          consts
             'TextFilter'
             'Useful filters for text messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-                17           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+                33           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (TEXT)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'TEXT')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 17
+               firstlineno 33
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
+            'matches'
+            'str'
+            'return'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (text)
+                             0 MAKE_CELL                0 (matches)
+               
+                36           2 RESUME                   0
                
-                21           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (text)
+                39           4 LOAD_CLOSURE             0 (matches)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 21>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 39>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  'Filter for text messages that equal the given text/s.'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f4f7407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        0b890289016a0500000000000000006b0200000000702f74070000000000
-                        00000000008902740c00000000000000000000a6020000ab020000000000
-                        0000006f1a740f00000000000000000000880166016401840889024400a6
-                        000000ab000000000000000000a6010000ab0100000000000000005300
+                        006a0200000000000000006b02000000006f1a7407000000000000000000
+                        00880166016401840889024400a6000000ab000000000000000000a60100
+                        00ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                      21           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                      39           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (TEXT)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP    79 (to 206)
-                     
-                      22          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (text)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE    11 (to 112)
-                                  90 LOAD_DEREF               2 (text)
-                                  92 LOAD_DEREF               1 (data)
-                                  94 LOAD_ATTR                5 (text)
-                                 104 COMPARE_OP               2 (==)
-                                 110 JUMP_IF_TRUE_OR_POP     47 (to 206)
-                     
-                      23     >>  112 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 124 LOAD_DEREF               2 (text)
-                                 126 LOAD_GLOBAL             12 (Iterable)
-                                 138 PRECALL                  2
-                                 142 CALL                     2
-                                 152 JUMP_IF_FALSE_OR_POP    26 (to 206)
-                     
-                      24         154 LOAD_GLOBAL             15 (NULL + any)
-                                 166 LOAD_CLOSURE             1 (data)
-                                 168 BUILD_TUPLE              1
-                                 170 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 24>)
-                                 172 MAKE_FUNCTION            8 (closure)
-                                 174 LOAD_DEREF               2 (text)
-                                 176 GET_ITER
-                                 178 PRECALL                  0
-                                 182 CALL                     0
-                                 192 PRECALL                  1
-                                 196 CALL                     1
-                     
-                      21     >>  206 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    26 (to 100)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 BUILD_TUPLE              1
+                                  64 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 39>)
+                                  66 MAKE_FUNCTION            8 (closure)
+                                  68 LOAD_DEREF               2 (matches)
+                                  70 GET_ITER
+                                  72 PRECALL                  0
+                                  76 CALL                     0
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                             >>  100 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 3
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d0f7d017c0189026a0000000000000000006b
                               02000000005600970101008c1064005300
                                          0 COPY_FREE_VARS           1
                            
-                            24           2 RETURN_GENERATOR
+                            39           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                15 (to 42)
                                         12 STORE_FAST               1 (t)
                                         14 LOAD_FAST                1 (t)
-                                        16 LOAD_DEREF               2 (data)
+                                        16 LOAD_DEREF               2 (m)
                                         18 LOAD_ATTR                0 (text)
                                         28 COMPARE_OP               2 (==)
                                         34 YIELD_VALUE
                                         36 RESUME                   1
                                         38 POP_TOP
                                         40 JUMP_BACKWARD           16 (to 10)
                                    >>   42 LOAD_CONST               0 (None)
                                         44 RETURN_VALUE
                            consts
                               None
                            names      ('text',)
                            varnames   ('.0', 't')
-                           freevars   ('data',)
+                           freevars   ('m',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 24
+                           firstlineno 39
                            lnotab 0x
-                     names      ('type', 'Mt', 'TEXT', 'isinstance', 'str', 'text', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('text',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'TEXT', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('matches',)
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 21
-                     lnotab 0x300140012a0134fd
+                     firstlineno 39
+                     lnotab 0x
                names      ()
-               varnames   ('text',)
+               varnames   ('matches',)
                freevars   ()
-               cellvars   ('text',)
+               cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 21
-               lnotab 0x
-            'Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]'
-            'EQUALS'
+               name       'equals'
+               firstlineno 36
+               lnotab 0x0403
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (text)
+                             0 MAKE_CELL                0 (matches)
+               
+                41           2 RESUME                   0
                
-                28           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (text)
+                44           4 LOAD_CLOSURE             0 (matches)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 28>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 44>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  'Filter for text messages that contain the given text/s.'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f4d7407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        09890289016a0500000000000000007600702f7407000000000000000000
-                        008902740c00000000000000000000a6020000ab0200000000000000006f
-                        1a740f00000000000000000000880166016401840889024400a6000000ab
-                        000000000000000000a6010000ab0100000000000000005300
+                        006a0200000000000000006b02000000006f1a7407000000000000000000
+                        00880166016401840889024400a6000000ab000000000000000000a60100
+                        00ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                      28           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                      44           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (TEXT)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP    77 (to 202)
-                     
-                      29          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (text)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE     9 (to 108)
-                                  90 LOAD_DEREF               2 (text)
-                                  92 LOAD_DEREF               1 (data)
-                                  94 LOAD_ATTR                5 (text)
-                                 104 CONTAINS_OP              0
-                                 106 JUMP_IF_TRUE_OR_POP     47 (to 202)
-                     
-                      30     >>  108 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 120 LOAD_DEREF               2 (text)
-                                 122 LOAD_GLOBAL             12 (Iterable)
-                                 134 PRECALL                  2
-                                 138 CALL                     2
-                                 148 JUMP_IF_FALSE_OR_POP    26 (to 202)
-                     
-                      31         150 LOAD_GLOBAL             15 (NULL + any)
-                                 162 LOAD_CLOSURE             1 (data)
-                                 164 BUILD_TUPLE              1
-                                 166 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 31>)
-                                 168 MAKE_FUNCTION            8 (closure)
-                                 170 LOAD_DEREF               2 (text)
-                                 172 GET_ITER
-                                 174 PRECALL                  0
-                                 178 CALL                     0
-                                 188 PRECALL                  1
-                                 192 CALL                     1
-                     
-                      28     >>  202 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    26 (to 100)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 BUILD_TUPLE              1
+                                  64 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 44>)
+                                  66 MAKE_FUNCTION            8 (closure)
+                                  68 LOAD_DEREF               2 (matches)
+                                  70 GET_ITER
+                                  72 PRECALL                  0
+                                  76 CALL                     0
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                             >>  100 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 3
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d0d7d017c0189026a00000000000000000076
                               005600970101008c0e64005300
                                          0 COPY_FREE_VARS           1
                            
-                            31           2 RETURN_GENERATOR
+                            44           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                13 (to 38)
                                         12 STORE_FAST               1 (t)
                                         14 LOAD_FAST                1 (t)
-                                        16 LOAD_DEREF               2 (data)
+                                        16 LOAD_DEREF               2 (m)
                                         18 LOAD_ATTR                0 (text)
                                         28 CONTAINS_OP              0
                                         30 YIELD_VALUE
                                         32 RESUME                   1
                                         34 POP_TOP
                                         36 JUMP_BACKWARD           14 (to 10)
                                    >>   38 LOAD_CONST               0 (None)
                                         40 RETURN_VALUE
                            consts
                               None
                            names      ('text',)
                            varnames   ('.0', 't')
-                           freevars   ('data',)
+                           freevars   ('m',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 31
+                           firstlineno 44
                            lnotab 0x
-                     names      ('type', 'Mt', 'TEXT', 'isinstance', 'str', 'text', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('text',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'TEXT', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('matches',)
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 28
-                     lnotab 0x30013c012a0134fd
+                     firstlineno 44
+                     lnotab 0x
                names      ()
-               varnames   ('text',)
+               varnames   ('matches',)
                freevars   ()
-               cellvars   ('text',)
+               cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 28
-               lnotab 0x
-            'CONTAINS'
+               name       'contains'
+               firstlineno 41
+               lnotab 0x0403
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (text)
+                             0 MAKE_CELL                0 (matches)
+               
+                46           2 RESUME                   0
                
-                35           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (text)
+                49           4 LOAD_CLOSURE             0 (matches)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 35>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 49>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  'Filter for text messages that start with the given text/s.'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f5e7407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        1a89016a050000000000000000a006000000000000000000000000000000
-                        00000000008902a6010000ab010000000000000000702f74070000000000
-                        00000000008902740e00000000000000000000a6020000ab020000000000
-                        0000006f1a741100000000000000000000880166016401840889024400a6
-                        000000ab000000000000000000a6010000ab0100000000000000005300
+                        006a0200000000000000006b02000000006f1a7407000000000000000000
+                        00880166016401840889024400a6000000ab000000000000000000a60100
+                        00ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                      35           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                      49           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (TEXT)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP    94 (to 236)
-                     
-                      36          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (text)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE    26 (to 142)
-                                  90 LOAD_DEREF               1 (data)
-                                  92 LOAD_ATTR                5 (text)
-                                 102 LOAD_METHOD              6 (startswith)
-                                 124 LOAD_DEREF               2 (text)
-                                 126 PRECALL                  1
-                                 130 CALL                     1
-                                 140 JUMP_IF_TRUE_OR_POP     47 (to 236)
-                     
-                      37     >>  142 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 154 LOAD_DEREF               2 (text)
-                                 156 LOAD_GLOBAL             14 (Iterable)
-                                 168 PRECALL                  2
-                                 172 CALL                     2
-                                 182 JUMP_IF_FALSE_OR_POP    26 (to 236)
-                     
-                      38         184 LOAD_GLOBAL             17 (NULL + any)
-                                 196 LOAD_CLOSURE             1 (data)
-                                 198 BUILD_TUPLE              1
-                                 200 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 38>)
-                                 202 MAKE_FUNCTION            8 (closure)
-                                 204 LOAD_DEREF               2 (text)
-                                 206 GET_ITER
-                                 208 PRECALL                  0
-                                 212 CALL                     0
-                                 222 PRECALL                  1
-                                 226 CALL                     1
-                     
-                      35     >>  236 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    26 (to 100)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 BUILD_TUPLE              1
+                                  64 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 49>)
+                                  66 MAKE_FUNCTION            8 (closure)
+                                  68 LOAD_DEREF               2 (matches)
+                                  70 GET_ITER
+                                  72 PRECALL                  0
+                                  76 CALL                     0
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                             >>  100 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 4
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d1e7d0189026a000000000000000000a00100
                               000000000000000000000000000000000000007c01a6010000ab01000000
                               00000000005600970101008c1f64005300
                                          0 COPY_FREE_VARS           1
                            
-                            38           2 RETURN_GENERATOR
+                            49           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                30 (to 72)
                                         12 STORE_FAST               1 (t)
-                                        14 LOAD_DEREF               2 (data)
+                                        14 LOAD_DEREF               2 (m)
                                         16 LOAD_ATTR                0 (text)
                                         26 LOAD_METHOD              1 (startswith)
                                         48 LOAD_FAST                1 (t)
                                         50 PRECALL                  1
                                         54 CALL                     1
                                         64 YIELD_VALUE
                                         66 RESUME                   1
@@ -704,132 +653,105 @@
                                         70 JUMP_BACKWARD           31 (to 10)
                                    >>   72 LOAD_CONST               0 (None)
                                         74 RETURN_VALUE
                            consts
                               None
                            names      ('text', 'startswith')
                            varnames   ('.0', 't')
-                           freevars   ('data',)
+                           freevars   ('m',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 38
+                           firstlineno 49
                            lnotab 0x
-                     names      ('type', 'Mt', 'TEXT', 'isinstance', 'str', 'text', 'startswith', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('text',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'TEXT', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('matches',)
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 35
-                     lnotab 0x30015e012a0134fd
+                     firstlineno 49
+                     lnotab 0x
                names      ()
-               varnames   ('text',)
+               varnames   ('matches',)
                freevars   ()
-               cellvars   ('text',)
+               cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 35
-               lnotab 0x
-            'STARTS_WITH'
+               name       'startswith'
+               firstlineno 46
+               lnotab 0x0403
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (text)
+                             0 MAKE_CELL                0 (matches)
                
-                42           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (text)
+                51           2 RESUME                   0
+               
+                54           4 LOAD_CLOSURE             0 (matches)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 42>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 54>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  'Filter for text messages that end with the given text/s.'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f5e7407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        1a89016a050000000000000000a006000000000000000000000000000000
-                        00000000008902a6010000ab010000000000000000702f74070000000000
-                        00000000008902740e00000000000000000000a6020000ab020000000000
-                        0000006f1a741100000000000000000000880166016401840889024400a6
-                        000000ab000000000000000000a6010000ab0100000000000000005300
+                        006a0200000000000000006b02000000006f1a7407000000000000000000
+                        00880166016401840889024400a6000000ab000000000000000000a60100
+                        00ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                      42           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                      54           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (TEXT)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP    94 (to 236)
-                     
-                      43          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (text)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE    26 (to 142)
-                                  90 LOAD_DEREF               1 (data)
-                                  92 LOAD_ATTR                5 (text)
-                                 102 LOAD_METHOD              6 (endswith)
-                                 124 LOAD_DEREF               2 (text)
-                                 126 PRECALL                  1
-                                 130 CALL                     1
-                                 140 JUMP_IF_TRUE_OR_POP     47 (to 236)
-                     
-                      44     >>  142 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 154 LOAD_DEREF               2 (text)
-                                 156 LOAD_GLOBAL             14 (Iterable)
-                                 168 PRECALL                  2
-                                 172 CALL                     2
-                                 182 JUMP_IF_FALSE_OR_POP    26 (to 236)
-                     
-                      45         184 LOAD_GLOBAL             17 (NULL + any)
-                                 196 LOAD_CLOSURE             1 (data)
-                                 198 BUILD_TUPLE              1
-                                 200 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 45>)
-                                 202 MAKE_FUNCTION            8 (closure)
-                                 204 LOAD_DEREF               2 (text)
-                                 206 GET_ITER
-                                 208 PRECALL                  0
-                                 212 CALL                     0
-                                 222 PRECALL                  1
-                                 226 CALL                     1
-                     
-                      42     >>  236 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    26 (to 100)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 BUILD_TUPLE              1
+                                  64 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 54>)
+                                  66 MAKE_FUNCTION            8 (closure)
+                                  68 LOAD_DEREF               2 (matches)
+                                  70 GET_ITER
+                                  72 PRECALL                  0
+                                  76 CALL                     0
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                             >>  100 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 4
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d1e7d0189026a000000000000000000a00100
                               000000000000000000000000000000000000007c01a6010000ab01000000
                               00000000005600970101008c1f64005300
                                          0 COPY_FREE_VARS           1
                            
-                            45           2 RETURN_GENERATOR
+                            54           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                30 (to 72)
                                         12 STORE_FAST               1 (t)
-                                        14 LOAD_DEREF               2 (data)
+                                        14 LOAD_DEREF               2 (m)
                                         16 LOAD_ATTR                0 (text)
                                         26 LOAD_METHOD              1 (endswith)
                                         48 LOAD_FAST                1 (t)
                                         50 PRECALL                  1
                                         54 CALL                     1
                                         64 YIELD_VALUE
                                         66 RESUME                   1
@@ -837,302 +759,237 @@
                                         70 JUMP_BACKWARD           31 (to 10)
                                    >>   72 LOAD_CONST               0 (None)
                                         74 RETURN_VALUE
                            consts
                               None
                            names      ('text', 'endswith')
                            varnames   ('.0', 't')
-                           freevars   ('data',)
+                           freevars   ('m',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 45
+                           firstlineno 54
                            lnotab 0x
-                     names      ('type', 'Mt', 'TEXT', 'isinstance', 'str', 'text', 'endswith', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('text',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'TEXT', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('matches',)
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 42
-                     lnotab 0x30015e012a0134fd
+                     firstlineno 54
+                     lnotab 0x
                names      ()
-               varnames   ('text',)
+               varnames   ('matches',)
                freevars   ()
-               cellvars   ('text',)
+               cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 42
-               lnotab 0x
-            'ENDS_WITH'
+               name       'endswith'
+               firstlineno 51
+               lnotab 0x0403
+            0
+            ('flags',)
+            'patterns'
+            'str | re.Pattern'
+            'flags'
+            'int'
             code
-               argcount  : 1
-               nlocals   : 1
+               argcount  : 0
+               nlocals   : 2
                stacksize : 2
-               flags     : 16777219
-               code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (reg)
+               flags     : 16777223
+               code 0x870087019700880088016602640184085300
+                             0 MAKE_CELL                0 (flags)
+                             2 MAKE_CELL                1 (patterns)
                
-                49           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (reg)
-                             6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 49>)
-                            10 MAKE_FUNCTION            8 (closure)
-                            12 RETURN_VALUE
+                56           4 RESUME                   0
+               
+                62           6 LOAD_CLOSURE             0 (flags)
+                             8 LOAD_CLOSURE             1 (patterns)
+                            10 BUILD_TUPLE              2
+                            12 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 62>)
+                            14 MAKE_FUNCTION            8 (closure)
+                            16 RETURN_VALUE
                consts
-                  None
+                  "\n        Filter for text messages that match the given regex/regexes.\n            * It's recommended to pass compiled regexes to save time (``re.compile(your_pattern)``)\n        "
                   code
                      argcount  : 2
                      nlocals   : 2
-                     stacksize : 5
+                     stacksize : 4
                      flags     : 16777235
                      code
-                        0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f6a7407000000000000000000
-                        008902740800000000000000000000740a000000000000000000006a0600
-                        000000000000006602a6020000ab020000000000000000721a740b000000
-                        000000000000006a070000000000000000890289016a0800000000000000
-                        00a6020000ab020000000000000000702f74070000000000000000000089
-                        02741200000000000000000000a6020000ab0200000000000000006f1a74
-                        1500000000000000000000880166016401840889024400a6000000ab0000
-                        00000000000000a6010000ab0100000000000000005300
-                                   0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                        0x95028701970089016a0000000000000000007402000000000000000000
+                        006a0200000000000000006b02000000006f1b7407000000000000000000
+                        008802880166026401840889034400a6000000ab000000000000000000a6
+                        010000ab0100000000000000005300
+                                   0 COPY_FREE_VARS           2
+                                   2 MAKE_CELL                1 (m)
                      
-                      49           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                      62           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (TEXT)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP   106 (to 260)
-                     
-                      50          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (reg)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 LOAD_GLOBAL             10 (re)
-                                  86 LOAD_ATTR                6 (Pattern)
-                                  96 BUILD_TUPLE              2
-                                  98 PRECALL                  2
-                                 102 CALL                     2
-                                 112 POP_JUMP_FORWARD_IF_FALSE    26 (to 166)
-                                 114 LOAD_GLOBAL             11 (NULL + re)
-                                 126 LOAD_ATTR                7 (match)
-                                 136 LOAD_DEREF               2 (reg)
-                                 138 LOAD_DEREF               1 (data)
-                                 140 LOAD_ATTR                8 (text)
-                                 150 PRECALL                  2
-                                 154 CALL                     2
-                                 164 JUMP_IF_TRUE_OR_POP     47 (to 260)
-                     
-                      51     >>  166 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 178 LOAD_DEREF               2 (reg)
-                                 180 LOAD_GLOBAL             18 (Iterable)
-                                 192 PRECALL                  2
-                                 196 CALL                     2
-                                 206 JUMP_IF_FALSE_OR_POP    26 (to 260)
-                     
-                      52         208 LOAD_GLOBAL             21 (NULL + any)
-                                 220 LOAD_CLOSURE             1 (data)
-                                 222 BUILD_TUPLE              1
-                                 224 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 52>)
-                                 226 MAKE_FUNCTION            8 (closure)
-                                 228 LOAD_DEREF               2 (reg)
-                                 230 GET_ITER
-                                 232 PRECALL                  0
-                                 236 CALL                     0
-                                 246 PRECALL                  1
-                                 250 CALL                     1
-                     
-                      49     >>  260 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    27 (to 102)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             2 (flags)
+                                  62 LOAD_CLOSURE             1 (m)
+                                  64 BUILD_TUPLE              2
+                                  66 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 62>)
+                                  68 MAKE_FUNCTION            8 (closure)
+                                  70 LOAD_DEREF               3 (patterns)
+                                  72 GET_ITER
+                                  74 PRECALL                  0
+                                  78 CALL                     0
+                                  88 PRECALL                  1
+                                  92 CALL                     1
+                             >>  102 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
-                           stacksize : 5
+                           stacksize : 6
                            flags     : 16777267
                            code
-                              0x95014b00010097007c005d1e7d017401000000000000000000006a0100
-                              000000000000007c0189026a020000000000000000a6020000ab02000000
-                              00000000005600970101008c1f64005300
-                                         0 COPY_FREE_VARS           1
+                              0x95024b00010097007c005d1f7d017401000000000000000000006a0100
+                              000000000000007c0189036a0200000000000000008902a6030000ab0300
+                              000000000000005600970101008c2064005300
+                                         0 COPY_FREE_VARS           2
                            
-                            52           2 RETURN_GENERATOR
+                            62           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
-                                   >>   10 FOR_ITER                30 (to 72)
-                                        12 STORE_FAST               1 (t)
+                                   >>   10 FOR_ITER                31 (to 74)
+                                        12 STORE_FAST               1 (p)
                                         14 LOAD_GLOBAL              1 (NULL + re)
                                         26 LOAD_ATTR                1 (match)
-                                        36 LOAD_FAST                1 (t)
-                                        38 LOAD_DEREF               2 (data)
+                                        36 LOAD_FAST                1 (p)
+                                        38 LOAD_DEREF               3 (m)
                                         40 LOAD_ATTR                2 (text)
-                                        50 PRECALL                  2
-                                        54 CALL                     2
-                                        64 YIELD_VALUE
-                                        66 RESUME                   1
-                                        68 POP_TOP
-                                        70 JUMP_BACKWARD           31 (to 10)
-                                   >>   72 LOAD_CONST               0 (None)
-                                        74 RETURN_VALUE
+                                        50 LOAD_DEREF               2 (flags)
+                                        52 PRECALL                  3
+                                        56 CALL                     3
+                                        66 YIELD_VALUE
+                                        68 RESUME                   1
+                                        70 POP_TOP
+                                        72 JUMP_BACKWARD           32 (to 10)
+                                   >>   74 LOAD_CONST               0 (None)
+                                        76 RETURN_VALUE
                            consts
                               None
                            names      ('re', 'match', 'text')
-                           varnames   ('.0', 't')
-                           freevars   ('data',)
+                           varnames   ('.0', 'p')
+                           freevars   ('flags', 'm')
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 52
+                           firstlineno 62
                            lnotab 0x
-                     names      ('type', 'Mt', 'TEXT', 'isinstance', 'str', 're', 'Pattern', 'match', 'text', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('reg',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'TEXT', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('flags', 'patterns')
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 49
-                     lnotab 0x300176012a0134fd
+                     firstlineno 62
+                     lnotab 0x
                names      ()
-               varnames   ('reg',)
+               varnames   ('flags', 'patterns')
                freevars   ()
-               cellvars   ('reg',)
+               cellvars   ('flags', 'patterns')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 49
-               lnotab 0x
-            'Callable[[str | Iterable[str] | re.Pattern | Iterable[re.Pattern]], Callable[[Wa, Msg], bool]]'
-            'REGEX'
+               name       'regex'
+               firstlineno 56
+               lnotab 0x0606
+            'lengths'
+            'tuple[int, int]'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (length)
+                             0 MAKE_CELL                0 (lengths)
+               
+                64           2 RESUME                   0
                
-                56           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (length)
+                72           4 LOAD_CLOSURE             0 (lengths)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 56>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 72>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  '\n        Filter for text messages that have a length between the given range/s.\n\n        Args:\n            lengths: The length range/s to filter for (e.g. (1, 10), (50, 100)).\n        '
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f727407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        2e8902640119000000000000000000740b0000000000000000000089016a
-                        060000000000000000a6010000ab010000000000000000630278026b0100
-                        0000006f0b89026402190000000000000000006b01000000006e02630201
-                        00702f7407000000000000000000008902740e00000000000000000000a6
-                        020000ab0200000000000000006f1a741100000000000000000000880166
-                        016403840889024400a6000000ab000000000000000000a6010000ab0100
-                        000000000000005300
+                        006a0200000000000000006b02000000006f1a7407000000000000000000
+                        00880166016401840889024400a6000000ab000000000000000000a60100
+                        00ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                      56           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                      72           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (TEXT)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP   114 (to 276)
-                     
-                      57          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (length)
-                                  62 LOAD_GLOBAL              8 (tuple)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE    46 (to 182)
-                                  90 LOAD_DEREF               2 (length)
-                                  92 LOAD_CONST               1 (0)
-                                  94 BINARY_SUBSCR
-                                 104 LOAD_GLOBAL             11 (NULL + len)
-                                 116 LOAD_DEREF               1 (data)
-                                 118 LOAD_ATTR                6 (text)
-                                 128 PRECALL                  1
-                                 132 CALL                     1
-                                 142 SWAP                     2
-                                 144 COPY                     2
-                                 146 COMPARE_OP               1 (<=)
-                                 152 JUMP_IF_FALSE_OR_POP    11 (to 176)
-                                 154 LOAD_DEREF               2 (length)
-                                 156 LOAD_CONST               2 (1)
-                                 158 BINARY_SUBSCR
-                                 168 COMPARE_OP               1 (<=)
-                                 174 JUMP_FORWARD             2 (to 180)
-                             >>  176 SWAP                     2
-                                 178 POP_TOP
-                             >>  180 JUMP_IF_TRUE_OR_POP     47 (to 276)
-                     
-                      58     >>  182 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 194 LOAD_DEREF               2 (length)
-                                 196 LOAD_GLOBAL             14 (Iterable)
-                                 208 PRECALL                  2
-                                 212 CALL                     2
-                                 222 JUMP_IF_FALSE_OR_POP    26 (to 276)
-                     
-                      59         224 LOAD_GLOBAL             17 (NULL + any)
-                                 236 LOAD_CLOSURE             1 (data)
-                                 238 BUILD_TUPLE              1
-                                 240 LOAD_CONST               3 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 59>)
-                                 242 MAKE_FUNCTION            8 (closure)
-                                 244 LOAD_DEREF               2 (length)
-                                 246 GET_ITER
-                                 248 PRECALL                  0
-                                 252 CALL                     0
-                                 262 PRECALL                  1
-                                 266 CALL                     1
-                     
-                      56     >>  276 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    26 (to 100)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 BUILD_TUPLE              1
+                                  64 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 72>)
+                                  66 MAKE_FUNCTION            8 (closure)
+                                  68 LOAD_DEREF               2 (lengths)
+                                  70 GET_ITER
+                                  72 PRECALL                  0
+                                  76 CALL                     0
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                             >>  100 RETURN_VALUE
                      consts
                         None
-                        0
-                        1
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 5
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d327d017c0164001900000000000000000074
                               010000000000000000000089026a010000000000000000a6010000ab0100
                               00000000000000630278026b01000000006f0b7c01640119000000000000
                               0000006b01000000006e02630201005600970101008c3364025300
                                          0 COPY_FREE_VARS           1
                            
-                            59           2 RETURN_GENERATOR
+                            72           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                50 (to 112)
-                                        12 STORE_FAST               1 (l)
-                                        14 LOAD_FAST                1 (l)
+                                        12 STORE_FAST               1 (i)
+                                        14 LOAD_FAST                1 (i)
                                         16 LOAD_CONST               0 (0)
                                         18 BINARY_SUBSCR
                                         28 LOAD_GLOBAL              1 (NULL + len)
-                                        40 LOAD_DEREF               2 (data)
+                                        40 LOAD_DEREF               2 (m)
                                         42 LOAD_ATTR                1 (text)
                                         52 PRECALL                  1
                                         56 CALL                     1
                                         66 SWAP                     2
                                         68 COPY                     2
                                         70 COMPARE_OP               1 (<=)
                                         76 JUMP_IF_FALSE_OR_POP    11 (to 100)
-                                        78 LOAD_FAST                1 (l)
+                                        78 LOAD_FAST                1 (i)
                                         80 LOAD_CONST               1 (1)
                                         82 BINARY_SUBSCR
                                         92 COMPARE_OP               1 (<=)
                                         98 JUMP_FORWARD             2 (to 104)
                                    >>  100 SWAP                     2
                                        102 POP_TOP
                                    >>  104 YIELD_VALUE
@@ -1142,1346 +999,1293 @@
                                    >>  112 LOAD_CONST               2 (None)
                                        114 RETURN_VALUE
                            consts
                               0
                               1
                               None
                            names      ('len', 'text')
-                           varnames   ('.0', 'l')
-                           freevars   ('data',)
+                           varnames   ('.0', 'i')
+                           freevars   ('m',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 59
+                           firstlineno 72
                            lnotab 0x
-                     names      ('type', 'Mt', 'TEXT', 'isinstance', 'tuple', 'len', 'text', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('length',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'TEXT', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('lengths',)
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 56
-                     lnotab 0x300186012a0134fd
+                     firstlineno 72
+                     lnotab 0x
                names      ()
-               varnames   ('length',)
+               varnames   ('lengths',)
                freevars   ()
-               cellvars   ('length',)
+               cellvars   ('lengths',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 56
-               lnotab 0x
-            'Callable[[tuple[int, int] | Iterable[tuple[int, int]]], Callable[[Wa, Msg], bool]]'
-            'LEN_BETWEEN'
-            '/'
-            'cmd'
+               name       'length'
+               firstlineno 64
+               lnotab 0x0408
+            '!'
+            ('prefixes',)
+            'cmds'
+            'prefixes'
             'str | Iterable[str]'
-            'prefix'
-            'str'
-            'return'
             code
-               argcount  : 2
+               argcount  : 0
                nlocals   : 2
                stacksize : 2
-               flags     : 16777219
-               code 0x870087019700880088016602640184085300
-                             0 MAKE_CELL                0 (cmd)
-                             2 MAKE_CELL                1 (prefix)
+               flags     : 16777223
+               code 0x870087019700880188006602640184085300
+                             0 MAKE_CELL                0 (prefixes)
+                             2 MAKE_CELL                1 (cmds)
                
-                62           4 RESUME                   0
+                74           4 RESUME                   0
                
-                71           6 LOAD_CLOSURE             0 (cmd)
-                             8 LOAD_CLOSURE             1 (prefix)
+                83           6 LOAD_CLOSURE             1 (cmds)
+                             8 LOAD_CLOSURE             0 (prefixes)
                             10 BUILD_TUPLE              2
-                            12 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 71>)
+                            12 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 83>)
                             14 MAKE_FUNCTION            8 (closure)
                             16 RETURN_VALUE
                consts
-                  '\n        Filter for text messages that are commands.\n\n        Args:\n            cmd: The command/s to filter for.\n            prefix: The prefix to filter for (default: "/").\n        '
+                  '\n        Filter for text messages that are commands.\n\n        Args:\n            cmds: The command/s to filter for (e.g. "start", "hello").\n            prefixes: The prefix/s to filter for (default: "!", i.e. "!start").\n        '
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95028701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f627407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        1d89016a050000000000000000a006000000000000000000000000000000
-                        0000000000890389027a000000a6010000ab010000000000000000703074
-                        07000000000000000000008902740e00000000000000000000a6020000ab
-                        0200000000000000006f1b74110000000000000000000088018803660264
-                        01840889024400a6000000ab000000000000000000a6010000ab01000000
-                        00000000005300
+                        006a0200000000000000006b02000000006f1b7407000000000000000000
+                        008801880366026401840889024400a6000000ab000000000000000000a6
+                        010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           2
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                      71           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                      83           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (TEXT)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP    98 (to 244)
-                     
-                      72          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (cmd)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE    29 (to 148)
-                                  90 LOAD_DEREF               1 (data)
-                                  92 LOAD_ATTR                5 (text)
-                                 102 LOAD_METHOD              6 (startswith)
-                                 124 LOAD_DEREF               3 (prefix)
-                                 126 LOAD_DEREF               2 (cmd)
-                                 128 BINARY_OP                0 (+)
-                                 132 PRECALL                  1
-                                 136 CALL                     1
-                                 146 JUMP_IF_TRUE_OR_POP     48 (to 244)
-                     
-                      73     >>  148 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 160 LOAD_DEREF               2 (cmd)
-                                 162 LOAD_GLOBAL             14 (Iterable)
-                                 174 PRECALL                  2
-                                 178 CALL                     2
-                                 188 JUMP_IF_FALSE_OR_POP    27 (to 244)
-                     
-                      74         190 LOAD_GLOBAL             17 (NULL + any)
-                                 202 LOAD_CLOSURE             1 (data)
-                                 204 LOAD_CLOSURE             3 (prefix)
-                                 206 BUILD_TUPLE              2
-                                 208 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 74>)
-                                 210 MAKE_FUNCTION            8 (closure)
-                                 212 LOAD_DEREF               2 (cmd)
-                                 214 GET_ITER
-                                 216 PRECALL                  0
-                                 220 CALL                     0
-                                 230 PRECALL                  1
-                                 234 CALL                     1
-                     
-                      71     >>  244 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    27 (to 102)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 LOAD_CLOSURE             3 (prefixes)
+                                  64 BUILD_TUPLE              2
+                                  66 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 83>)
+                                  68 MAKE_FUNCTION            8 (closure)
+                                  70 LOAD_DEREF               2 (cmds)
+                                  72 GET_ITER
+                                  74 PRECALL                  0
+                                  78 CALL                     0
+                                  88 PRECALL                  1
+                                  92 CALL                     1
+                             >>  102 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
-                           stacksize : 5
+                           stacksize : 4
                            flags     : 16777267
                            code
-                              0x95024b00010097007c005d217d0189026a000000000000000000a00100
-                              0000000000000000000000000000000000000089037c017a000000a60100
-                              00ab0100000000000000005600970101008c2264005300
+                              0x95024b00010097007c005d357d0189026a000000000000000000640019
+                              000000000000000000890376006f2189026a000000000000000000640164
+                              02850219000000000000000000a001000000000000000000000000000000
+                              00000000007c01a6010000ab0100000000000000005600970101008c3664
+                              025300
                                          0 COPY_FREE_VARS           2
                            
-                            74           2 RETURN_GENERATOR
+                            83           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
-                                   >>   10 FOR_ITER                33 (to 78)
+                                   >>   10 FOR_ITER                53 (to 118)
                                         12 STORE_FAST               1 (c)
-                                        14 LOAD_DEREF               2 (data)
+                                        14 LOAD_DEREF               2 (m)
                                         16 LOAD_ATTR                0 (text)
-                                        26 LOAD_METHOD              1 (startswith)
-                                        48 LOAD_DEREF               3 (prefix)
-                                        50 LOAD_FAST                1 (c)
-                                        52 BINARY_OP                0 (+)
-                                        56 PRECALL                  1
-                                        60 CALL                     1
-                                        70 YIELD_VALUE
-                                        72 RESUME                   1
-                                        74 POP_TOP
-                                        76 JUMP_BACKWARD           34 (to 10)
-                                   >>   78 LOAD_CONST               0 (None)
-                                        80 RETURN_VALUE
+                                        26 LOAD_CONST               0 (0)
+                                        28 BINARY_SUBSCR
+                                        38 LOAD_DEREF               3 (prefixes)
+                                        40 CONTAINS_OP              0
+                                        42 JUMP_IF_FALSE_OR_POP    33 (to 110)
+                                        44 LOAD_DEREF               2 (m)
+                                        46 LOAD_ATTR                0 (text)
+                                        56 LOAD_CONST               1 (1)
+                                        58 LOAD_CONST               2 (None)
+                                        60 BUILD_SLICE              2
+                                        62 BINARY_SUBSCR
+                                        72 LOAD_METHOD              1 (startswith)
+                                        94 LOAD_FAST                1 (c)
+                                        96 PRECALL                  1
+                                       100 CALL                     1
+                                   >>  110 YIELD_VALUE
+                                       112 RESUME                   1
+                                       114 POP_TOP
+                                       116 JUMP_BACKWARD           54 (to 10)
+                                   >>  118 LOAD_CONST               2 (None)
+                                       120 RETURN_VALUE
                            consts
+                              0
+                              1
                               None
                            names      ('text', 'startswith')
                            varnames   ('.0', 'c')
-                           freevars   ('data', 'prefix')
+                           freevars   ('m', 'prefixes')
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 74
+                           firstlineno 83
                            lnotab 0x
-                     names      ('type', 'Mt', 'TEXT', 'isinstance', 'str', 'text', 'startswith', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('cmd', 'prefix')
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'TEXT', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('cmds', 'prefixes')
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 71
-                     lnotab 0x300164012a0136fd
+                     firstlineno 83
+                     lnotab 0x
                names      ()
-               varnames   ('cmd', 'prefix')
+               varnames   ('prefixes', 'cmds')
                freevars   ()
-               cellvars   ('cmd', 'prefix')
+               cellvars   ('prefixes', 'cmds')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       'COMMAND'
-               firstlineno 62
+               name       'command'
+               firstlineno 74
                lnotab 0x0609
             None
-            ('/',)
-            ('cmd', 'str | Iterable[str]', 'prefix', 'str', 'return', 'Callable[[Wa, Msg], bool]')
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'EQUALS', 'CONTAINS', 'STARTS_WITH', 'ENDS_WITH', 'REGEX', 'LEN_BETWEEN', 'staticmethod', 'COMMAND')
+            ('matches', 'str', 'return', 'Callable[[Wa, Msg], bool]')
+            ('patterns', 'str | re.Pattern', 'flags', 'int', 'return', 'Callable[[Wa, Msg], bool]')
+            ('lengths', 'tuple[int, int]', 'return', 'Callable[[Wa, Msg], bool]')
+            ('cmds', 'str', 'prefixes', 'str | Iterable[str]', 'return', 'Callable[[Wa, Msg], bool]')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'staticmethod', 'equals', 'contains', 'startswith', 'endswith', 'regex', 'length', 'command')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'TextFilter'
-         firstlineno 14
+         firstlineno 30
          lnotab
-            0x0c0104021001020304ff0c05020304ff0c05020304ff0c05020304ff0c
-            05020304ff0c05020304ff0c050202020108ff0e01
+            0x0c01040210010202020106ff0e010204020106ff0e010204020106ff0e
+            010204020106ff0e01020402010cff0e010207020106ff0e01020902010c
+            ff0e01
       'TextFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
-            0000000900640584005a066403650564063c0000000900640784005a0764
-            08650564093c000000640a5300
-          77           0 RESUME                   0
+            000000090065066410640b8404a6000000ab0000000000000000005a0765
+            066411640e8404a6000000ab0000000000000000005a08640f5300
+          86           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ImageFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          78          12 LOAD_CONST               1 ('Useful filters for image messages.')
+          87          12 LOAD_CONST               1 ('Useful filters for image messages.')
                       14 STORE_NAME               3 (__doc__)
          
-          80          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 80>)
+          89          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 89>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-          81          32 NOP
+          90          32 NOP
          
-          83          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 83>)
-                      36 MAKE_FUNCTION            0
-                      38 STORE_NAME               6 (HAS_CAPTION)
-                      40 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
-                      42 LOAD_NAME                5 (__annotations__)
-                      44 LOAD_CONST               6 ('HAS_CAPTION')
-                      46 STORE_SUBSCR
+          92          34 LOAD_NAME                6 (staticmethod)
          
-          84          50 NOP
+          93          36 LOAD_CONST              16 (('wa', 'Wa', 'm', 'Msg', 'return', 'bool'))
+                      38 LOAD_CONST              11 (<code object has_caption, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 92>)
+                      40 MAKE_FUNCTION            4 (annotations)
          
-          87          52 LOAD_CONST               7 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 87>)
-                      54 MAKE_FUNCTION            0
+          92          42 PRECALL                  0
+                      46 CALL                     0
          
-          86          56 STORE_NAME               7 (MIME_TYPE)
-                      58 LOAD_CONST               8 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      60 LOAD_NAME                5 (__annotations__)
-                      62 LOAD_CONST               9 ('MIME_TYPE')
-                      64 STORE_SUBSCR
+          93          56 STORE_NAME               7 (has_caption)
          
-          91          68 LOAD_CONST              10 (None)
-                      70 RETURN_VALUE
+          97          58 LOAD_NAME                6 (staticmethod)
+         
+          98          60 LOAD_CONST              17 (('mime_types', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                      62 LOAD_CONST              14 (<code object mimetype, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 97>)
+                      64 MAKE_FUNCTION            4 (annotations)
+         
+          97          66 PRECALL                  0
+                      70 CALL                     0
+         
+          98          80 STORE_NAME               8 (mimetype)
+                      82 LOAD_CONST              15 (None)
+                      84 RETURN_VALUE
          consts
             'ImageFilter'
             'Useful filters for image messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-                80           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+                89           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (IMAGE)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'IMAGE')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 80
+               firstlineno 89
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
+            'wa'
+            'Wa'
+            'm'
+            'Msg'
+            'return'
+            'bool'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000006f0d7c016a0300000000000000006a0400
-                  00000000000000640075015300
-                83           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+                  00000000000000640175015300
+                92           0 RESUME                   0
+               
+                95           2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (IMAGE)
                             36 COMPARE_OP               2 (==)
                             42 JUMP_IF_FALSE_OR_POP    13 (to 70)
-                            44 LOAD_FAST                1 (data)
+                            44 LOAD_FAST                1 (m)
                             46 LOAD_ATTR                3 (image)
                             56 LOAD_ATTR                4 (caption)
-                            66 LOAD_CONST               0 (None)
+                            66 LOAD_CONST               1 (None)
                             68 IS_OP                    1
                        >>   70 RETURN_VALUE
                consts
+                  'Filter for image messages that have a caption.'
                   None
                names      ('type', 'Mt', 'IMAGE', 'image', 'caption')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 83
-               lnotab 0x
-            'HAS_CAPTION'
+               name       'has_caption'
+               firstlineno 92
+               lnotab 0x0203
+            'mime_types'
+            'str'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (mime)
+                             0 MAKE_CELL                0 (mime_types)
+               
+                97           2 RESUME                   0
                
-                87           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (mime)
+               103           4 LOAD_CLOSURE             0 (mime_types)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 87>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 103>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  '\n        Filter for image messages that have the given mime type/s.\n        See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types\n        '
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f547407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        1089016a0500000000000000006a06000000000000000089026b02000000
-                        00702f7407000000000000000000008902740e00000000000000000000a6
-                        020000ab0200000000000000006f1a741100000000000000000000880166
-                        016401840889024400a6000000ab000000000000000000a6010000ab0100
-                        000000000000005300
+                        006a0200000000000000006b02000000006f1a7407000000000000000000
+                        00880166016401840889024400a6000000ab000000000000000000a60100
+                        00ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                      87           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                     103           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (IMAGE)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP    84 (to 216)
-                     
-                      88          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (mime)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE    16 (to 122)
-                                  90 LOAD_DEREF               1 (data)
-                                  92 LOAD_ATTR                5 (image)
-                                 102 LOAD_ATTR                6 (mime_type)
-                                 112 LOAD_DEREF               2 (mime)
-                                 114 COMPARE_OP               2 (==)
-                                 120 JUMP_IF_TRUE_OR_POP     47 (to 216)
-                     
-                      89     >>  122 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 134 LOAD_DEREF               2 (mime)
-                                 136 LOAD_GLOBAL             14 (Iterable)
-                                 148 PRECALL                  2
-                                 152 CALL                     2
-                                 162 JUMP_IF_FALSE_OR_POP    26 (to 216)
-                     
-                      90         164 LOAD_GLOBAL             17 (NULL + any)
-                                 176 LOAD_CLOSURE             1 (data)
-                                 178 BUILD_TUPLE              1
-                                 180 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 90>)
-                                 182 MAKE_FUNCTION            8 (closure)
-                                 184 LOAD_DEREF               2 (mime)
-                                 186 GET_ITER
-                                 188 PRECALL                  0
-                                 192 CALL                     0
-                                 202 PRECALL                  1
-                                 206 CALL                     1
-                     
-                      87     >>  216 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    26 (to 100)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 BUILD_TUPLE              1
+                                  64 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 103>)
+                                  66 MAKE_FUNCTION            8 (closure)
+                                  68 LOAD_DEREF               2 (mime_types)
+                                  70 GET_ITER
+                                  72 PRECALL                  0
+                                  76 CALL                     0
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                             >>  100 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 3
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d147d017c0189026a0000000000000000006a
                               0100000000000000006b02000000005600970101008c1564005300
                                          0 COPY_FREE_VARS           1
                            
-                            90           2 RETURN_GENERATOR
+                           103           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                20 (to 52)
                                         12 STORE_FAST               1 (t)
                                         14 LOAD_FAST                1 (t)
-                                        16 LOAD_DEREF               2 (data)
+                                        16 LOAD_DEREF               2 (m)
                                         18 LOAD_ATTR                0 (image)
                                         28 LOAD_ATTR                1 (mime_type)
                                         38 COMPARE_OP               2 (==)
                                         44 YIELD_VALUE
                                         46 RESUME                   1
                                         48 POP_TOP
                                         50 JUMP_BACKWARD           21 (to 10)
                                    >>   52 LOAD_CONST               0 (None)
                                         54 RETURN_VALUE
                            consts
                               None
                            names      ('image', 'mime_type')
                            varnames   ('.0', 't')
-                           freevars   ('data',)
+                           freevars   ('m',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 90
+                           firstlineno 103
                            lnotab 0x
-                     names      ('type', 'Mt', 'IMAGE', 'isinstance', 'str', 'image', 'mime_type', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('mime',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'IMAGE', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('mime_types',)
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 87
-                     lnotab 0x30014a012a0134fd
+                     firstlineno 103
+                     lnotab 0x
                names      ()
-               varnames   ('mime',)
+               varnames   ('mime_types',)
                freevars   ()
-               cellvars   ('mime',)
+               cellvars   ('mime_types',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 87
-               lnotab 0x
-            'Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]'
-            'MIME_TYPE'
+               name       'mimetype'
+               firstlineno 97
+               lnotab 0x0406
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'HAS_CAPTION', 'MIME_TYPE')
+            ('wa', 'Wa', 'm', 'Msg', 'return', 'bool')
+            ('mime_types', 'str', 'return', 'Callable[[Wa, Msg], bool]')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'staticmethod', 'has_caption', 'mimetype')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'ImageFilter'
-         firstlineno 77
-         lnotab 0x0c010402100102021001020304ff0c05
+         firstlineno 86
+         lnotab 0x0c01040210010202020106ff0e010204020106ff0e01
       'ImageFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
-            0000000900640584005a066406650564073c00000064085300
-          97           0 RESUME                   0
+            00000009006506640a64088404a6000000ab0000000000000000005a0764
+            095300
+         106           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('VideoFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          98          12 LOAD_CONST               1 ('Useful filters for video messages.')
+         107          12 LOAD_CONST               1 ('Useful filters for video messages.')
                       14 STORE_NAME               3 (__doc__)
          
-         100          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 100>)
+         109          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 109>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-         101          32 NOP
+         110          32 NOP
          
-         104          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 104>)
-                      36 MAKE_FUNCTION            0
+         112          34 LOAD_NAME                6 (staticmethod)
          
-         103          38 STORE_NAME               6 (MIME_TYPE)
-                      40 LOAD_CONST               6 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      42 LOAD_NAME                5 (__annotations__)
-                      44 LOAD_CONST               7 ('MIME_TYPE')
-                      46 STORE_SUBSCR
+         113          36 LOAD_CONST              10 (('mime_types', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                      38 LOAD_CONST               8 (<code object mimetype, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 112>)
+                      40 MAKE_FUNCTION            4 (annotations)
+         
+         112          42 PRECALL                  0
+                      46 CALL                     0
          
-         108          50 LOAD_CONST               8 (None)
-                      52 RETURN_VALUE
+         113          56 STORE_NAME               7 (mimetype)
+                      58 LOAD_CONST               9 (None)
+                      60 RETURN_VALUE
          consts
             'VideoFilter'
             'Useful filters for video messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               100           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               109           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (VIDEO)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'VIDEO')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 100
+               firstlineno 109
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
+            'mime_types'
+            'str'
+            'return'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (mime)
+                             0 MAKE_CELL                0 (mime_types)
+               
+               112           2 RESUME                   0
                
-               104           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (mime)
+               118           4 LOAD_CLOSURE             0 (mime_types)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 104>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 118>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  '\n        Filter for video messages that have the given mime type/s.\n        See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types\n        '
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f547407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        1089016a0500000000000000006a06000000000000000089026b02000000
-                        00702f7407000000000000000000008902740e00000000000000000000a6
-                        020000ab0200000000000000006f1a741100000000000000000000880166
-                        016401840889024400a6000000ab000000000000000000a6010000ab0100
-                        000000000000005300
+                        006a0200000000000000006b02000000006f1a7407000000000000000000
+                        00880166016401840889024400a6000000ab000000000000000000a60100
+                        00ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                     104           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                     118           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (VIDEO)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP    84 (to 216)
-                     
-                     105          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (mime)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE    16 (to 122)
-                                  90 LOAD_DEREF               1 (data)
-                                  92 LOAD_ATTR                5 (video)
-                                 102 LOAD_ATTR                6 (mime_type)
-                                 112 LOAD_DEREF               2 (mime)
-                                 114 COMPARE_OP               2 (==)
-                                 120 JUMP_IF_TRUE_OR_POP     47 (to 216)
-                     
-                     106     >>  122 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 134 LOAD_DEREF               2 (mime)
-                                 136 LOAD_GLOBAL             14 (Iterable)
-                                 148 PRECALL                  2
-                                 152 CALL                     2
-                                 162 JUMP_IF_FALSE_OR_POP    26 (to 216)
-                     
-                     107         164 LOAD_GLOBAL             17 (NULL + any)
-                                 176 LOAD_CLOSURE             1 (data)
-                                 178 BUILD_TUPLE              1
-                                 180 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 107>)
-                                 182 MAKE_FUNCTION            8 (closure)
-                                 184 LOAD_DEREF               2 (mime)
-                                 186 GET_ITER
-                                 188 PRECALL                  0
-                                 192 CALL                     0
-                                 202 PRECALL                  1
-                                 206 CALL                     1
-                     
-                     104     >>  216 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    26 (to 100)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 BUILD_TUPLE              1
+                                  64 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 118>)
+                                  66 MAKE_FUNCTION            8 (closure)
+                                  68 LOAD_DEREF               2 (mime_types)
+                                  70 GET_ITER
+                                  72 PRECALL                  0
+                                  76 CALL                     0
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                             >>  100 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 3
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d147d017c0189026a0000000000000000006a
                               0100000000000000006b02000000005600970101008c1564005300
                                          0 COPY_FREE_VARS           1
                            
-                           107           2 RETURN_GENERATOR
+                           118           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                20 (to 52)
                                         12 STORE_FAST               1 (t)
                                         14 LOAD_FAST                1 (t)
-                                        16 LOAD_DEREF               2 (data)
+                                        16 LOAD_DEREF               2 (m)
                                         18 LOAD_ATTR                0 (video)
                                         28 LOAD_ATTR                1 (mime_type)
                                         38 COMPARE_OP               2 (==)
                                         44 YIELD_VALUE
                                         46 RESUME                   1
                                         48 POP_TOP
                                         50 JUMP_BACKWARD           21 (to 10)
                                    >>   52 LOAD_CONST               0 (None)
                                         54 RETURN_VALUE
                            consts
                               None
                            names      ('video', 'mime_type')
                            varnames   ('.0', 't')
-                           freevars   ('data',)
+                           freevars   ('m',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 107
+                           firstlineno 118
                            lnotab 0x
-                     names      ('type', 'Mt', 'VIDEO', 'isinstance', 'str', 'video', 'mime_type', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('mime',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'VIDEO', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('mime_types',)
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 104
-                     lnotab 0x30014a012a0134fd
+                     firstlineno 118
+                     lnotab 0x
                names      ()
-               varnames   ('mime',)
+               varnames   ('mime_types',)
                freevars   ()
-               cellvars   ('mime',)
+               cellvars   ('mime_types',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 104
-               lnotab 0x
-            'Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]'
-            'MIME_TYPE'
+               name       'mimetype'
+               firstlineno 112
+               lnotab 0x0406
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'MIME_TYPE')
+            ('mime_types', 'str', 'return', 'Callable[[Wa, Msg], bool]')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'staticmethod', 'mimetype')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'VideoFilter'
-         firstlineno 97
-         lnotab 0x0c0104021001020304ff0c05
+         firstlineno 106
+         lnotab 0x0c01040210010202020106ff0e01
       'VideoFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
             0000000900640584005a066403650564063c0000000900640784005a0764
-            03650564083c0000000900640984005a08640a6505640b3c000000640c53
-            00
-         114           0 RESUME                   0
+            03650564083c00000009006508640e640c8404a6000000ab000000000000
+            0000005a09640d5300
+         121           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AudioFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         115          12 LOAD_CONST               1 ('Useful filters for audio messages.')
+         122          12 LOAD_CONST               1 ('Useful filters for audio messages.')
                       14 STORE_NAME               3 (__doc__)
          
-         117          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 117>)
+         124          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 124>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-         118          32 NOP
+         125          32 NOP
          
-         120          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 120>)
+         127          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 127>)
                       36 MAKE_FUNCTION            0
-                      38 STORE_NAME               6 (IS_VOICE)
+                      38 STORE_NAME               6 (VOICE)
                       40 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       42 LOAD_NAME                5 (__annotations__)
-                      44 LOAD_CONST               6 ('IS_VOICE')
+                      44 LOAD_CONST               6 ('VOICE')
                       46 STORE_SUBSCR
          
-         121          50 NOP
+         128          50 NOP
          
-         123          52 LOAD_CONST               7 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 123>)
+         130          52 LOAD_CONST               7 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 130>)
                       54 MAKE_FUNCTION            0
-                      56 STORE_NAME               7 (IS_AUDIO)
+                      56 STORE_NAME               7 (AUDIO)
                       58 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       60 LOAD_NAME                5 (__annotations__)
-                      62 LOAD_CONST               8 ('IS_AUDIO')
+                      62 LOAD_CONST               8 ('AUDIO')
                       64 STORE_SUBSCR
          
-         124          68 NOP
+         131          68 NOP
+         
+         133          70 LOAD_NAME                8 (staticmethod)
          
-         127          70 LOAD_CONST               9 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 127>)
-                      72 MAKE_FUNCTION            0
+         134          72 LOAD_CONST              14 (('mime_types', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                      74 LOAD_CONST              12 (<code object mimetype, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 133>)
+                      76 MAKE_FUNCTION            4 (annotations)
          
-         126          74 STORE_NAME               8 (MIME_TYPE)
-                      76 LOAD_CONST              10 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      78 LOAD_NAME                5 (__annotations__)
-                      80 LOAD_CONST              11 ('MIME_TYPE')
-                      82 STORE_SUBSCR
+         133          78 PRECALL                  0
+                      82 CALL                     0
          
-         131          86 LOAD_CONST              12 (None)
-                      88 RETURN_VALUE
+         134          92 STORE_NAME               9 (mimetype)
+                      94 LOAD_CONST              13 (None)
+                      96 RETURN_VALUE
          consts
             'AudioFilter'
             'Useful filters for audio messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               117           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               124           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (AUDIO)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'AUDIO')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 117
+               firstlineno 124
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000006f0b7c016a0300000000000000006a0400
                   000000000000005300
-               120           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               127           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (AUDIO)
                             36 COMPARE_OP               2 (==)
                             42 JUMP_IF_FALSE_OR_POP    11 (to 66)
-                            44 LOAD_FAST                1 (data)
+                            44 LOAD_FAST                1 (m)
                             46 LOAD_ATTR                3 (audio)
                             56 LOAD_ATTR                4 (voice)
                        >>   66 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'AUDIO', 'audio', 'voice')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 120
+               firstlineno 127
                lnotab 0x
-            'IS_VOICE'
+            'VOICE'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000006f0c7c016a0300000000000000006a0400
                   000000000000000c005300
-               123           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               130           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (AUDIO)
                             36 COMPARE_OP               2 (==)
                             42 JUMP_IF_FALSE_OR_POP    12 (to 68)
-                            44 LOAD_FAST                1 (data)
+                            44 LOAD_FAST                1 (m)
                             46 LOAD_ATTR                3 (audio)
                             56 LOAD_ATTR                4 (voice)
                             66 UNARY_NOT
                        >>   68 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'AUDIO', 'audio', 'voice')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 123
+               firstlineno 130
                lnotab 0x
-            'IS_AUDIO'
+            'AUDIO'
+            'mime_types'
+            'str'
+            'return'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (mime)
+                             0 MAKE_CELL                0 (mime_types)
                
-               127           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (mime)
+               133           2 RESUME                   0
+               
+               139           4 LOAD_CLOSURE             0 (mime_types)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 127>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 139>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  '\n        Filter for audio messages that have the given mime type/s.\n        See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types\n        '
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f547407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        1089016a0500000000000000006a06000000000000000089026b02000000
-                        00702f7407000000000000000000008902740e00000000000000000000a6
-                        020000ab0200000000000000006f1a741100000000000000000000880166
-                        016401840889024400a6000000ab000000000000000000a6010000ab0100
-                        000000000000005300
+                        006a0200000000000000006b02000000006f1a7407000000000000000000
+                        00880166016401840889024400a6000000ab000000000000000000a60100
+                        00ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                     127           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                     139           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (AUDIO)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP    84 (to 216)
-                     
-                     128          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (mime)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE    16 (to 122)
-                                  90 LOAD_DEREF               1 (data)
-                                  92 LOAD_ATTR                5 (audio)
-                                 102 LOAD_ATTR                6 (mime_type)
-                                 112 LOAD_DEREF               2 (mime)
-                                 114 COMPARE_OP               2 (==)
-                                 120 JUMP_IF_TRUE_OR_POP     47 (to 216)
-                     
-                     129     >>  122 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 134 LOAD_DEREF               2 (mime)
-                                 136 LOAD_GLOBAL             14 (Iterable)
-                                 148 PRECALL                  2
-                                 152 CALL                     2
-                                 162 JUMP_IF_FALSE_OR_POP    26 (to 216)
-                     
-                     130         164 LOAD_GLOBAL             17 (NULL + any)
-                                 176 LOAD_CLOSURE             1 (data)
-                                 178 BUILD_TUPLE              1
-                                 180 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 130>)
-                                 182 MAKE_FUNCTION            8 (closure)
-                                 184 LOAD_DEREF               2 (mime)
-                                 186 GET_ITER
-                                 188 PRECALL                  0
-                                 192 CALL                     0
-                                 202 PRECALL                  1
-                                 206 CALL                     1
-                     
-                     127     >>  216 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    26 (to 100)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 BUILD_TUPLE              1
+                                  64 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 139>)
+                                  66 MAKE_FUNCTION            8 (closure)
+                                  68 LOAD_DEREF               2 (mime_types)
+                                  70 GET_ITER
+                                  72 PRECALL                  0
+                                  76 CALL                     0
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                             >>  100 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 3
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d147d017c0189026a0000000000000000006a
                               0100000000000000006b02000000005600970101008c1564005300
                                          0 COPY_FREE_VARS           1
                            
-                           130           2 RETURN_GENERATOR
+                           139           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                20 (to 52)
                                         12 STORE_FAST               1 (t)
                                         14 LOAD_FAST                1 (t)
-                                        16 LOAD_DEREF               2 (data)
+                                        16 LOAD_DEREF               2 (m)
                                         18 LOAD_ATTR                0 (audio)
                                         28 LOAD_ATTR                1 (mime_type)
                                         38 COMPARE_OP               2 (==)
                                         44 YIELD_VALUE
                                         46 RESUME                   1
                                         48 POP_TOP
                                         50 JUMP_BACKWARD           21 (to 10)
                                    >>   52 LOAD_CONST               0 (None)
                                         54 RETURN_VALUE
                            consts
                               None
                            names      ('audio', 'mime_type')
                            varnames   ('.0', 't')
-                           freevars   ('data',)
+                           freevars   ('m',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 130
+                           firstlineno 139
                            lnotab 0x
-                     names      ('type', 'Mt', 'AUDIO', 'isinstance', 'str', 'audio', 'mime_type', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('mime',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'AUDIO', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('mime_types',)
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 127
-                     lnotab 0x30014a012a0134fd
+                     firstlineno 139
+                     lnotab 0x
                names      ()
-               varnames   ('mime',)
+               varnames   ('mime_types',)
                freevars   ()
-               cellvars   ('mime',)
+               cellvars   ('mime_types',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 127
-               lnotab 0x
-            'Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]'
-            'MIME_TYPE'
+               name       'mimetype'
+               firstlineno 133
+               lnotab 0x0406
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'IS_VOICE', 'IS_AUDIO', 'MIME_TYPE')
+            ('mime_types', 'str', 'return', 'Callable[[Wa, Msg], bool]')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'VOICE', 'AUDIO', 'staticmethod', 'mimetype')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'AudioFilter'
-         firstlineno 114
-         lnotab 0x0c01040210010202100102021001020304ff0c05
+         firstlineno 121
+         lnotab 0x0c010402100102021001020210010202020106ff0e01
       'AudioFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
-            0000000900640584005a066406650564073c00000064085300
-         137           0 RESUME                   0
+            00000009006506640a64088404a6000000ab0000000000000000005a0764
+            095300
+         142           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DocumentFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         138          12 LOAD_CONST               1 ('Useful filters for document messages.')
+         143          12 LOAD_CONST               1 ('Useful filters for document messages.')
                       14 STORE_NAME               3 (__doc__)
          
-         140          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 140>)
+         145          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 145>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-         141          32 NOP
+         146          32 NOP
          
-         144          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 144>)
-                      36 MAKE_FUNCTION            0
+         148          34 LOAD_NAME                6 (staticmethod)
          
-         143          38 STORE_NAME               6 (MIME_TYPE)
-                      40 LOAD_CONST               6 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      42 LOAD_NAME                5 (__annotations__)
-                      44 LOAD_CONST               7 ('MIME_TYPE')
-                      46 STORE_SUBSCR
+         149          36 LOAD_CONST              10 (('mime_types', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                      38 LOAD_CONST               8 (<code object mimetype, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 148>)
+                      40 MAKE_FUNCTION            4 (annotations)
          
-         148          50 LOAD_CONST               8 (None)
-                      52 RETURN_VALUE
+         148          42 PRECALL                  0
+                      46 CALL                     0
+         
+         149          56 STORE_NAME               7 (mimetype)
+                      58 LOAD_CONST               9 (None)
+                      60 RETURN_VALUE
          consts
             'DocumentFilter'
             'Useful filters for document messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               140           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               145           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (DOCUMENT)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'DOCUMENT')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 140
+               firstlineno 145
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
+            'mime_types'
+            'str'
+            'return'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (mime)
+                             0 MAKE_CELL                0 (mime_types)
                
-               144           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (mime)
+               148           2 RESUME                   0
+               
+               154           4 LOAD_CLOSURE             0 (mime_types)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 144>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 154>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  '\n        Filter for document messages that have the given mime type/s.\n        See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types\n        '
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x95018701970089016a0000000000000000007402000000000000000000
-                        006a0200000000000000006b02000000006f547407000000000000000000
-                        008902740800000000000000000000a6020000ab02000000000000000072
-                        1089016a0500000000000000006a06000000000000000089026b02000000
-                        00702f7407000000000000000000008902740e00000000000000000000a6
-                        020000ab0200000000000000006f1a741100000000000000000000880166
-                        016401840889024400a6000000ab000000000000000000a6010000ab0100
-                        000000000000005300
+                        006a0200000000000000006b02000000006f1a7407000000000000000000
+                        00880166016401840889024400a6000000ab000000000000000000a60100
+                        00ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data)
+                                   2 MAKE_CELL                1 (m)
                      
-                     144           4 RESUME                   0
-                                   6 LOAD_DEREF               1 (data)
+                     154           4 RESUME                   0
+                                   6 LOAD_DEREF               1 (m)
                                    8 LOAD_ATTR                0 (type)
                                   18 LOAD_GLOBAL              2 (Mt)
                                   30 LOAD_ATTR                2 (DOCUMENT)
                                   40 COMPARE_OP               2 (==)
-                                  46 JUMP_IF_FALSE_OR_POP    84 (to 216)
-                     
-                     145          48 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  60 LOAD_DEREF               2 (mime)
-                                  62 LOAD_GLOBAL              8 (str)
-                                  74 PRECALL                  2
-                                  78 CALL                     2
-                                  88 POP_JUMP_FORWARD_IF_FALSE    16 (to 122)
-                                  90 LOAD_DEREF               1 (data)
-                                  92 LOAD_ATTR                5 (document)
-                                 102 LOAD_ATTR                6 (mime_type)
-                                 112 LOAD_DEREF               2 (mime)
-                                 114 COMPARE_OP               2 (==)
-                                 120 JUMP_IF_TRUE_OR_POP     47 (to 216)
-                     
-                     146     >>  122 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 134 LOAD_DEREF               2 (mime)
-                                 136 LOAD_GLOBAL             14 (Iterable)
-                                 148 PRECALL                  2
-                                 152 CALL                     2
-                                 162 JUMP_IF_FALSE_OR_POP    26 (to 216)
-                     
-                     147         164 LOAD_GLOBAL             17 (NULL + any)
-                                 176 LOAD_CLOSURE             1 (data)
-                                 178 BUILD_TUPLE              1
-                                 180 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 147>)
-                                 182 MAKE_FUNCTION            8 (closure)
-                                 184 LOAD_DEREF               2 (mime)
-                                 186 GET_ITER
-                                 188 PRECALL                  0
-                                 192 CALL                     0
-                                 202 PRECALL                  1
-                                 206 CALL                     1
-                     
-                     144     >>  216 RETURN_VALUE
+                                  46 JUMP_IF_FALSE_OR_POP    26 (to 100)
+                                  48 LOAD_GLOBAL              7 (NULL + any)
+                                  60 LOAD_CLOSURE             1 (m)
+                                  62 BUILD_TUPLE              1
+                                  64 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 154>)
+                                  66 MAKE_FUNCTION            8 (closure)
+                                  68 LOAD_DEREF               2 (mime_types)
+                                  70 GET_ITER
+                                  72 PRECALL                  0
+                                  76 CALL                     0
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                             >>  100 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 3
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d147d017c0189026a0000000000000000006a
                               0100000000000000006b02000000005600970101008c1564005300
                                          0 COPY_FREE_VARS           1
                            
-                           147           2 RETURN_GENERATOR
+                           154           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                20 (to 52)
                                         12 STORE_FAST               1 (t)
                                         14 LOAD_FAST                1 (t)
-                                        16 LOAD_DEREF               2 (data)
+                                        16 LOAD_DEREF               2 (m)
                                         18 LOAD_ATTR                0 (document)
                                         28 LOAD_ATTR                1 (mime_type)
                                         38 COMPARE_OP               2 (==)
                                         44 YIELD_VALUE
                                         46 RESUME                   1
                                         48 POP_TOP
                                         50 JUMP_BACKWARD           21 (to 10)
                                    >>   52 LOAD_CONST               0 (None)
                                         54 RETURN_VALUE
                            consts
                               None
                            names      ('document', 'mime_type')
                            varnames   ('.0', 't')
-                           freevars   ('data',)
+                           freevars   ('m',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 147
+                           firstlineno 154
                            lnotab 0x
-                     names      ('type', 'Mt', 'DOCUMENT', 'isinstance', 'str', 'document', 'mime_type', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('mime',)
-                     cellvars   ('data',)
+                     names      ('type', 'Mt', 'DOCUMENT', 'any')
+                     varnames   ('wa', 'm')
+                     freevars   ('mime_types',)
+                     cellvars   ('m',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 144
-                     lnotab 0x30014a012a0134fd
+                     firstlineno 154
+                     lnotab 0x
                names      ()
-               varnames   ('mime',)
+               varnames   ('mime_types',)
                freevars   ()
-               cellvars   ('mime',)
+               cellvars   ('mime_types',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 144
-               lnotab 0x
-            'Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]'
-            'MIME_TYPE'
+               name       'mimetype'
+               firstlineno 148
+               lnotab 0x0406
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'MIME_TYPE')
+            ('mime_types', 'str', 'return', 'Callable[[Wa, Msg], bool]')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'staticmethod', 'mimetype')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'DocumentFilter'
-         firstlineno 137
-         lnotab 0x0c0104021001020304ff0c05
+         firstlineno 142
+         lnotab 0x0c01040210010202020106ff0e01
       'DocumentFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
-            0000000900640584005a066403650564063c00000064075300
-         154           0 RESUME                   0
+            0000000900640584005a066403650564063c0000000900640784005a0764
+            03650564083c00000064095300
+         157           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('StickerFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         155          12 LOAD_CONST               1 ('Useful filters for sticker messages.')
+         158          12 LOAD_CONST               1 ('Useful filters for sticker messages.')
                       14 STORE_NAME               3 (__doc__)
          
-         157          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 157>)
+         160          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 160>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-         158          32 NOP
+         161          32 NOP
          
-         160          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 160>)
+         163          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 163>)
                       36 MAKE_FUNCTION            0
-                      38 STORE_NAME               6 (IS_ANIMATED)
+                      38 STORE_NAME               6 (ANIMATED)
                       40 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       42 LOAD_NAME                5 (__annotations__)
-                      44 LOAD_CONST               6 ('IS_ANIMATED')
+                      44 LOAD_CONST               6 ('ANIMATED')
                       46 STORE_SUBSCR
          
-         161          50 LOAD_CONST               7 (None)
-                      52 RETURN_VALUE
+         164          50 NOP
+         
+         166          52 LOAD_CONST               7 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 166>)
+                      54 MAKE_FUNCTION            0
+                      56 STORE_NAME               7 (STATIC)
+                      58 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
+                      60 LOAD_NAME                5 (__annotations__)
+                      62 LOAD_CONST               8 ('STATIC')
+                      64 STORE_SUBSCR
+                      68 LOAD_CONST               9 (None)
+                      70 RETURN_VALUE
          consts
             'StickerFilter'
             'Useful filters for sticker messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               157           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               160           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (STICKER)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'STICKER')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 157
+               firstlineno 160
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000006f0b7c016a0300000000000000006a0400
                   000000000000005300
-               160           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               163           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (STICKER)
                             36 COMPARE_OP               2 (==)
                             42 JUMP_IF_FALSE_OR_POP    11 (to 66)
-                            44 LOAD_FAST                1 (data)
+                            44 LOAD_FAST                1 (m)
                             46 LOAD_ATTR                3 (sticker)
                             56 LOAD_ATTR                4 (animated)
                        >>   66 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'STICKER', 'sticker', 'animated')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 160
+               firstlineno 163
+               lnotab 0x
+            'ANIMATED'
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 2
+               flags     : 16777219
+               code
+                  0x97007c016a0000000000000000007402000000000000000000006a0200
+                  000000000000006b02000000006f0c7c016a0300000000000000006a0400
+                  000000000000000c005300
+               166           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
+                             4 LOAD_ATTR                0 (type)
+                            14 LOAD_GLOBAL              2 (Mt)
+                            26 LOAD_ATTR                2 (STICKER)
+                            36 COMPARE_OP               2 (==)
+                            42 JUMP_IF_FALSE_OR_POP    12 (to 68)
+                            44 LOAD_FAST                1 (m)
+                            46 LOAD_ATTR                3 (sticker)
+                            56 LOAD_ATTR                4 (animated)
+                            66 UNARY_NOT
+                       >>   68 RETURN_VALUE
+               consts
+                  None
+               names      ('type', 'Mt', 'STICKER', 'sticker', 'animated')
+               varnames   ('wa', 'm')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
+               name       '<lambda>'
+               firstlineno 166
                lnotab 0x
-            'IS_ANIMATED'
+            'STATIC'
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'IS_ANIMATED')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'ANIMATED', 'STATIC')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'StickerFilter'
-         firstlineno 154
-         lnotab 0x0c010402100102021001
+         firstlineno 157
+         lnotab 0x0c0104021001020210010202
       'StickerFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
             00000009006506640d640b8404a6000000ab0000000000000000005a0764
             0c5300
-         164           0 RESUME                   0
+         169           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LocationFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         165          12 LOAD_CONST               1 ('Useful filters for location messages.')
+         170          12 LOAD_CONST               1 ('Useful filters for location messages.')
                       14 STORE_NAME               3 (__doc__)
          
-         167          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 167>)
+         172          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 172>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-         168          32 NOP
+         173          32 NOP
          
-         170          34 LOAD_NAME                6 (staticmethod)
+         175          34 LOAD_NAME                6 (staticmethod)
          
-         171          36 LOAD_CONST              13 (('lat', 'float', 'lon', 'float', 'radius', 'float | int', 'return', 'Callable[[Wa, Msg], bool]'))
-                      38 LOAD_CONST              11 (<code object IN_RADIUS, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 170>)
+         176          36 LOAD_CONST              13 (('lat', 'float', 'lon', 'float', 'radius', 'float | int', 'return', 'Callable[[Wa, Msg], bool]'))
+                      38 LOAD_CONST              11 (<code object in_radius, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 175>)
                       40 MAKE_FUNCTION            4 (annotations)
          
-         170          42 PRECALL                  0
+         175          42 PRECALL                  0
                       46 CALL                     0
          
-         171          56 STORE_NAME               7 (IN_RADIUS)
+         176          56 STORE_NAME               7 (in_radius)
                       58 LOAD_CONST              12 (None)
                       60 RETURN_VALUE
          consts
             'LocationFilter'
             'Useful filters for location messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               167           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               172           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (LOCATION)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'LOCATION')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 167
+               firstlineno 172
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
             'lat'
             'float'
             'lon'
             'radius'
@@ -2493,29 +2297,29 @@
                stacksize : 4
                flags     : 16777219
                code 0x8700870187029700640888008801880266036407840c7d037c035300
                              0 MAKE_CELL                0 (lat)
                              2 MAKE_CELL                1 (lon)
                              4 MAKE_CELL                2 (radius)
                
-               170           6 RESUME                   0
+               175           6 RESUME                   0
                
-               183           8 LOAD_CONST               8 (('_', 'Wa', 'msg', 'Msg', 'return', 'bool'))
+               188           8 LOAD_CONST               8 (('_', 'Wa', 'msg', 'Msg', 'return', 'bool'))
                             10 LOAD_CLOSURE             0 (lat)
                             12 LOAD_CLOSURE             1 (lon)
                             14 LOAD_CLOSURE             2 (radius)
                             16 BUILD_TUPLE              3
-                            18 LOAD_CONST               7 (<code object _in_radius, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 183>)
+                            18 LOAD_CONST               7 (<code object _in_radius, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 188>)
                             20 MAKE_FUNCTION           12 (annotations, closure)
                             22 STORE_FAST               3 (_in_radius)
                
-               189          24 LOAD_FAST                3 (_in_radius)
+               194          24 LOAD_FAST                3 (_in_radius)
                             26 RETURN_VALUE
                consts
-                  '\n        Filter for location messages that are in a given radius.\n\n        >>> LocationFilter.IN_RADIUS(lat=37.48508108998884, lon=-122.14744733542707, radius=1)\n\n        Args:\n            lat (float): Latitude of the center of the radius.\n            lon (float): Longitude of the center of the radius.\n            radius (float | int): Radius in kilometers.\n        '
+                  '\n        Filter for location messages that are in a given radius.\n\n        >>> LocationFilter.in_radius(lat=37.48508108998884, lon=-122.14744733542707, radius=1)\n\n        Args:\n            lat: Latitude of the center of the radius.\n            lon: Longitude of the center of the radius.\n            radius: Radius in kilometers.\n        '
                   '_'
                   'Wa'
                   'msg'
                   'Msg'
                   'return'
                   'bool'
                   code
@@ -2527,1570 +2331,1439 @@
                         0x950397007c016a0000000000000000007402000000000000000000006a
                         0200000000000000006b02000000006f2f7407000000000000000000006a
                         040000000000000000890289037c016a0500000000000000006a06000000
                         00000000007c016a0500000000000000006a070000000000000000ac01a6
                         040000ab04000000000000000089046b01000000005300
                                    0 COPY_FREE_VARS           3
                      
-                     183           2 RESUME                   0
+                     188           2 RESUME                   0
                      
-                     184           4 LOAD_FAST                1 (msg)
+                     189           4 LOAD_FAST                1 (msg)
                                    6 LOAD_ATTR                0 (type)
                                   16 LOAD_GLOBAL              2 (Mt)
                                   28 LOAD_ATTR                2 (LOCATION)
                                   38 COMPARE_OP               2 (==)
                                   44 JUMP_IF_FALSE_OR_POP    47 (to 140)
                      
-                     185          46 LOAD_GLOBAL              7 (NULL + utils)
+                     190          46 LOAD_GLOBAL              7 (NULL + utils)
                                   58 LOAD_ATTR                4 (get_distance)
                      
-                     186          68 LOAD_DEREF               2 (lat)
+                     191          68 LOAD_DEREF               2 (lat)
                                   70 LOAD_DEREF               3 (lon)
                                   72 LOAD_FAST                1 (msg)
                                   74 LOAD_ATTR                5 (location)
                                   84 LOAD_ATTR                6 (latitude)
                                   94 LOAD_FAST                1 (msg)
                                   96 LOAD_ATTR                5 (location)
                                  106 LOAD_ATTR                7 (longitude)
                      
-                     185         116 KW_NAMES                 1
+                     190         116 KW_NAMES                 1
                                  118 PRECALL                  4
                                  122 CALL                     4
                      
-                     187         132 LOAD_DEREF               4 (radius)
+                     192         132 LOAD_DEREF               4 (radius)
                      
-                     185         134 COMPARE_OP               1 (<=)
+                     190         134 COMPARE_OP               1 (<=)
                      
-                     184     >>  140 RETURN_VALUE
+                     189     >>  140 RETURN_VALUE
                      consts
                         None
                         ('lat1', 'lon1', 'lat2', 'lon2')
                      names      ('type', 'Mt', 'LOCATION', 'utils', 'get_distance', 'location', 'latitude', 'longitude')
                      varnames   ('_', 'msg')
                      freevars   ('lat', 'lon', 'radius')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '_in_radius'
-                     firstlineno 183
+                     firstlineno 188
                      lnotab 0x04012a01160130ff100202fe06ff
                   ('_', 'Wa', 'msg', 'Msg', 'return', 'bool')
                names      ()
                varnames   ('lat', 'lon', 'radius', '_in_radius')
                freevars   ()
                cellvars   ('lat', 'lon', 'radius')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       'IN_RADIUS'
-               firstlineno 170
+               name       'in_radius'
+               firstlineno 175
                lnotab 0x080d1006
             None
             ('lat', 'float', 'lon', 'float', 'radius', 'float | int', 'return', 'Callable[[Wa, Msg], bool]')
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'staticmethod', 'IN_RADIUS')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'staticmethod', 'in_radius')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'LocationFilter'
-         firstlineno 164
+         firstlineno 169
          lnotab 0x0c01040210010202020106ff0e01
       'LocationFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
-            0000000900640584005a066406650564073c00000064085300
-         192           0 RESUME                   0
+            00000009006506640a64088404a6000000ab0000000000000000005a0764
+            095300
+         197           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ReactionFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         193          12 LOAD_CONST               1 ('Useful filters for reaction messages.')
+         198          12 LOAD_CONST               1 ('Useful filters for reaction messages.')
                       14 STORE_NAME               3 (__doc__)
          
-         195          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 195>)
+         200          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 200>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-         196          32 NOP
+         201          32 NOP
          
-         199          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 199>)
-                      36 MAKE_FUNCTION            0
+         203          34 LOAD_NAME                6 (staticmethod)
          
-         198          38 STORE_NAME               6 (EMOJI)
-                      40 LOAD_CONST               6 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      42 LOAD_NAME                5 (__annotations__)
-                      44 LOAD_CONST               7 ('EMOJI')
-                      46 STORE_SUBSCR
+         204          36 LOAD_CONST              10 (('emojis', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                      38 LOAD_CONST               8 (<code object emoji, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 203>)
+                      40 MAKE_FUNCTION            4 (annotations)
+         
+         203          42 PRECALL                  0
+                      46 CALL                     0
          
-         200          50 LOAD_CONST               8 (None)
-                      52 RETURN_VALUE
+         204          56 STORE_NAME               7 (emoji)
+                      58 LOAD_CONST               9 (None)
+                      60 RETURN_VALUE
          consts
             'ReactionFilter'
             'Useful filters for reaction messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               195           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               200           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (REACTION)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'REACTION')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 195
+               firstlineno 200
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
+            'emojis'
+            'str'
+            'return'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (reaction)
+                             0 MAKE_CELL                0 (emojis)
+               
+               203           2 RESUME                   0
                
-               199           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (reaction)
+               208           4 LOAD_CLOSURE             0 (emojis)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 199>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 208>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  '\n        Filter for custom reaction messages. pass emojis as strings.\n        '
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 2
                      flags     : 16777235
                      code
                         0x950197007c016a0000000000000000007402000000000000000000006a
                         0200000000000000006b02000000006f0d7c016a0300000000000000006a
                         040000000000000000890276005300
                                    0 COPY_FREE_VARS           1
                      
-                     199           2 RESUME                   0
-                                   4 LOAD_FAST                1 (data)
+                     208           2 RESUME                   0
+                                   4 LOAD_FAST                1 (m)
                                    6 LOAD_ATTR                0 (type)
                                   16 LOAD_GLOBAL              2 (Mt)
                                   28 LOAD_ATTR                2 (REACTION)
                                   38 COMPARE_OP               2 (==)
                                   44 JUMP_IF_FALSE_OR_POP    13 (to 72)
-                                  46 LOAD_FAST                1 (data)
+                                  46 LOAD_FAST                1 (m)
                                   48 LOAD_ATTR                3 (reaction)
                                   58 LOAD_ATTR                4 (emoji)
-                                  68 LOAD_DEREF               2 (reaction)
+                                  68 LOAD_DEREF               2 (emojis)
                                   70 CONTAINS_OP              0
                              >>   72 RETURN_VALUE
                      consts
                         None
                      names      ('type', 'Mt', 'REACTION', 'reaction', 'emoji')
-                     varnames   ('wa', 'data')
-                     freevars   ('reaction',)
+                     varnames   ('wa', 'm')
+                     freevars   ('emojis',)
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 199
+                     firstlineno 208
                      lnotab 0x
                names      ()
-               varnames   ('reaction',)
+               varnames   ('emojis',)
                freevars   ()
-               cellvars   ('reaction',)
+               cellvars   ('emojis',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 199
-               lnotab 0x
-            'Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]'
-            'EMOJI'
+               name       'emoji'
+               firstlineno 203
+               lnotab 0x0405
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'EMOJI')
+            ('emojis', 'str', 'return', 'Callable[[Wa, Msg], bool]')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'staticmethod', 'emoji')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'ReactionFilter'
-         firstlineno 192
-         lnotab 0x0c0104021001020304ff0c02
+         firstlineno 197
+         lnotab 0x0c01040210010202020106ff0e01
       'ReactionFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
-            0000000900640584005a066406650564073c0000000900640884005a0764
-            096505640a3c0000000900640b84005a0864036505640c3c000000640d53
-            00
-         203           0 RESUME                   0
+            0000000900640584005a066403650564063c000000090065076410640b84
+            04a6000000ab0000000000000000005a0865076411640e8404a6000000ab
+            0000000000000000005a09640f5300
+         211           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ContactsFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         204          12 LOAD_CONST               1 ('Useful filters for contact messages.')
+         212          12 LOAD_CONST               1 ('Useful filters for contact messages.')
                       14 STORE_NAME               3 (__doc__)
          
-         206          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 206>)
+         214          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 214>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-         207          32 NOP
+         215          32 NOP
          
-         210          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 210>)
+         217          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 217>)
                       36 MAKE_FUNCTION            0
-         
-         209          38 STORE_NAME               6 (COUNT_BETWEEN)
-                      40 LOAD_CONST               6 ('Callable[[int, int], Callable[[Wa, Msg], bool]]')
+                      38 STORE_NAME               6 (HAS_WA)
+                      40 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       42 LOAD_NAME                5 (__annotations__)
-                      44 LOAD_CONST               7 ('COUNT_BETWEEN')
+                      44 LOAD_CONST               6 ('HAS_WA')
                       46 STORE_SUBSCR
          
-         212          50 NOP
+         220          50 NOP
          
-         215          52 LOAD_CONST               8 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 215>)
-                      54 MAKE_FUNCTION            0
+         222          52 LOAD_NAME                7 (staticmethod)
          
-         214          56 STORE_NAME               7 (PHONE_NUMBER)
-                      58 LOAD_CONST               9 ('Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]')
-                      60 LOAD_NAME                5 (__annotations__)
-                      62 LOAD_CONST              10 ('PHONE_NUMBER')
-                      64 STORE_SUBSCR
+         223          54 LOAD_CONST              16 (('min_count', 'int', 'max_count', 'int', 'return', 'Callable[[Wa, Msg], bool]'))
+                      56 LOAD_CONST              11 (<code object count, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 222>)
+                      58 MAKE_FUNCTION            4 (annotations)
+         
+         222          60 PRECALL                  0
+                      64 CALL                     0
+         
+         223          74 STORE_NAME               8 (count)
          
-         221          68 NOP
+         227          76 LOAD_NAME                7 (staticmethod)
          
-         223          70 LOAD_CONST              11 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 223>)
-                      72 MAKE_FUNCTION            0
-                      74 STORE_NAME               8 (HAS_WA)
-                      76 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
-                      78 LOAD_NAME                5 (__annotations__)
-                      80 LOAD_CONST              12 ('HAS_WA')
-                      82 STORE_SUBSCR
+         228          78 LOAD_CONST              17 (('phones', 'str', 'return', 'Callable[[Wa, Msg], bool]'))
+                      80 LOAD_CONST              14 (<code object phone, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 227>)
+                      82 MAKE_FUNCTION            4 (annotations)
          
-         227          86 LOAD_CONST              13 (None)
-                      88 RETURN_VALUE
+         227          84 PRECALL                  0
+                      88 CALL                     0
+         
+         228          98 STORE_NAME               9 (phone)
+                     100 LOAD_CONST              15 (None)
+                     102 RETURN_VALUE
          consts
             'ContactsFilter'
             'Useful filters for contact messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               206           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               214           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (CONTACTS)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'CONTACTS')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 206
+               firstlineno 214
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
             code
                argcount  : 2
                nlocals   : 2
+               stacksize : 5
+               flags     : 16777219
+               code
+                  0x97007c016a0000000000000000007402000000000000000000006a0200
+                  000000000000006b02000000006f27740700000000000000000000640184
+                  00640284007c016a0400000000000000004400a6000000ab000000000000
+                  0000004400a6000000ab000000000000000000a6010000ab010000000000
+                  0000005300
+               217           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
+                             4 LOAD_ATTR                0 (type)
+                            14 LOAD_GLOBAL              2 (Mt)
+                            26 LOAD_ATTR                2 (CONTACTS)
+                            36 COMPARE_OP               2 (==)
+                            42 JUMP_IF_FALSE_OR_POP    39 (to 122)
+               
+               218          44 LOAD_GLOBAL              7 (NULL + any)
+                            56 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 218>)
+                            58 MAKE_FUNCTION            0
+                            60 LOAD_CONST               2 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 218>)
+                            62 MAKE_FUNCTION            0
+                            64 LOAD_FAST                1 (m)
+                            66 LOAD_ATTR                4 (contacts)
+                            76 GET_ITER
+                            78 PRECALL                  0
+                            82 CALL                     0
+                            92 GET_ITER
+                            94 PRECALL                  0
+                            98 CALL                     0
+                           108 PRECALL                  1
+                           112 CALL                     1
+               
+               217     >>  122 RETURN_VALUE
+               consts
+                  None
+                  code
+                     argcount  : 1
+                     nlocals   : 2
+                     stacksize : 2
+                     flags     : 16777267
+                     code
+                        0x4b00010097007c005d0b7d017c016a0000000000000000005600970101
+                        008c0c64005300
+                     218           0 RETURN_GENERATOR
+                                   2 POP_TOP
+                                   4 RESUME                   0
+                                   6 LOAD_FAST                0 (.0)
+                             >>    8 FOR_ITER                11 (to 32)
+                                  10 STORE_FAST               1 (p)
+                                  12 LOAD_FAST                1 (p)
+                                  14 LOAD_ATTR                0 (wa_id)
+                                  24 YIELD_VALUE
+                                  26 RESUME                   1
+                                  28 POP_TOP
+                                  30 JUMP_BACKWARD           12 (to 8)
+                             >>   32 LOAD_CONST               0 (None)
+                                  34 RETURN_VALUE
+                     consts
+                        None
+                     names      ('wa_id',)
+                     varnames   ('.0', 'p')
+                     freevars   ()
+                     cellvars   ()
+                     filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
+                     name       '<genexpr>'
+                     firstlineno 218
+                     lnotab 0x
+                  code
+                     argcount  : 1
+                     nlocals   : 3
+                     stacksize : 3
+                     flags     : 16777267
+                     code
+                        0x4b00010097007c005d107d017c016a00000000000000000044005d067d
+                        027c025600970101008c078c1164005300
+                     218           0 RETURN_GENERATOR
+                                   2 POP_TOP
+                                   4 RESUME                   0
+                                   6 LOAD_FAST                0 (.0)
+                             >>    8 FOR_ITER                16 (to 42)
+                                  10 STORE_FAST               1 (contact)
+                                  12 LOAD_FAST                1 (contact)
+                                  14 LOAD_ATTR                0 (phones)
+                                  24 GET_ITER
+                             >>   26 FOR_ITER                 6 (to 40)
+                                  28 STORE_FAST               2 (phone)
+                                  30 LOAD_FAST                2 (phone)
+                                  32 YIELD_VALUE
+                                  34 RESUME                   1
+                                  36 POP_TOP
+                                  38 JUMP_BACKWARD            7 (to 26)
+                             >>   40 JUMP_BACKWARD           17 (to 8)
+                             >>   42 LOAD_CONST               0 (None)
+                                  44 RETURN_VALUE
+                     consts
+                        None
+                     names      ('phones',)
+                     varnames   ('.0', 'contact', 'phone')
+                     freevars   ()
+                     cellvars   ()
+                     filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
+                     name       '<genexpr>'
+                     firstlineno 218
+                     lnotab 0x
+               names      ('type', 'Mt', 'CONTACTS', 'any', 'contacts')
+               varnames   ('wa', 'm')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
+               name       '<lambda>'
+               firstlineno 217
+               lnotab 0x2c014eff
+            'HAS_WA'
+            'min_count'
+            'int'
+            'max_count'
+            'return'
+            code
+               argcount  : 2
+               nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code 0x870087019700880188006602640184085300
                              0 MAKE_CELL                0 (min_count)
                              2 MAKE_CELL                1 (max_count)
                
-               210           4 RESUME                   0
-                             6 LOAD_CLOSURE             1 (max_count)
+               222           4 RESUME                   0
+               
+               225           6 LOAD_CLOSURE             1 (max_count)
                              8 LOAD_CLOSURE             0 (min_count)
                             10 BUILD_TUPLE              2
-                            12 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 210>)
+                            12 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 225>)
                             14 MAKE_FUNCTION            8 (closure)
                             16 RETURN_VALUE
                consts
-                  None
+                  'Filter for contacts messages that have a number of contacts between min_count and max_count.'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x950297007c016a0000000000000000007402000000000000000000006a
                         0200000000000000006b02000000006f2189037407000000000000000000
                         007c016a040000000000000000a6010000ab010000000000000000630278
                         026b01000000006f0589026b01000000006e02630201005300
                                    0 COPY_FREE_VARS           2
                      
-                     210           2 RESUME                   0
-                     
-                     211           4 LOAD_FAST                1 (data)
+                     225           2 RESUME                   0
+                                   4 LOAD_FAST                1 (m)
                                    6 LOAD_ATTR                0 (type)
                                   16 LOAD_GLOBAL              2 (Mt)
                                   28 LOAD_ATTR                2 (CONTACTS)
                                   38 COMPARE_OP               2 (==)
                                   44 JUMP_IF_FALSE_OR_POP    33 (to 112)
                                   46 LOAD_DEREF               3 (min_count)
                                   48 LOAD_GLOBAL              7 (NULL + len)
-                                  60 LOAD_FAST                1 (data)
+                                  60 LOAD_FAST                1 (m)
                                   62 LOAD_ATTR                4 (contacts)
                                   72 PRECALL                  1
                                   76 CALL                     1
                                   86 SWAP                     2
                                   88 COPY                     2
                                   90 COMPARE_OP               1 (<=)
                                   96 JUMP_IF_FALSE_OR_POP     5 (to 108)
                                   98 LOAD_DEREF               2 (max_count)
                                  100 COMPARE_OP               1 (<=)
                                  106 JUMP_FORWARD             2 (to 112)
                              >>  108 SWAP                     2
                                  110 POP_TOP
-                     
-                     210     >>  112 RETURN_VALUE
+                             >>  112 RETURN_VALUE
                      consts
                         None
                      names      ('type', 'Mt', 'CONTACTS', 'len', 'contacts')
-                     varnames   ('wa', 'data')
+                     varnames   ('wa', 'm')
                      freevars   ('max_count', 'min_count')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 210
-                     lnotab 0x04016cff
+                     firstlineno 225
+                     lnotab 0x
                names      ()
                varnames   ('min_count', 'max_count')
                freevars   ()
                cellvars   ('min_count', 'max_count')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 210
-               lnotab 0x
-            'Callable[[int, int], Callable[[Wa, Msg], bool]]'
-            'COUNT_BETWEEN'
+               name       'count'
+               firstlineno 222
+               lnotab 0x0603
+            'phones'
+            'str'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (phone_number)
+                             0 MAKE_CELL                0 (phones)
                
-               215           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (phone_number)
+               227           2 RESUME                   0
+               
+               233           4 LOAD_CLOSURE             0 (phones)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 215>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 233>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  '\n        Filter for contacts messages that have the given phone number/s.\n            * Pass only the numbers, without plus sign, spaces, etc.\n        '
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
                         0x950197007c016a0000000000000000007402000000000000000000006a
-                        0200000000000000006b02000000006f5c74070000000000000000000089
-                        02740800000000000000000000a6020000ab020000000000000000721389
-                        02640184007c016a0500000000000000004400a6000000ab000000000000
-                        000000760070347407000000000000000000008902740c00000000000000
-                        000000a6020000ab0200000000000000006f1f740f000000000000000000
-                        0088026601640284087c016a0500000000000000004400a6000000ab0000
-                        00000000000000a6010000ab0100000000000000005300
+                        0200000000000000006b02000000006f1f74070000000000000000000088
+                        026601640184087c016a0400000000000000004400a6000000ab00000000
+                        0000000000a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     215           2 RESUME                   0
-                                   4 LOAD_FAST                1 (data)
+                     233           2 RESUME                   0
+                                   4 LOAD_FAST                1 (m)
                                    6 LOAD_ATTR                0 (type)
                                   16 LOAD_GLOBAL              2 (Mt)
                                   28 LOAD_ATTR                2 (CONTACTS)
                                   38 COMPARE_OP               2 (==)
-                                  44 JUMP_IF_FALSE_OR_POP    92 (to 230)
-                     
-                     216          46 LOAD_GLOBAL              7 (NULL + isinstance)
-                                  58 LOAD_DEREF               2 (phone_number)
-                                  60 LOAD_GLOBAL              8 (str)
-                                  72 PRECALL                  2
-                                  76 CALL                     2
-                                  86 POP_JUMP_FORWARD_IF_FALSE    19 (to 126)
-                                  88 LOAD_DEREF               2 (phone_number)
-                     
-                     217          90 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 217>)
-                                  92 MAKE_FUNCTION            0
-                                  94 LOAD_FAST                1 (data)
-                                  96 LOAD_ATTR                5 (contacts)
-                                 106 GET_ITER
-                                 108 PRECALL                  0
-                                 112 CALL                     0
-                     
-                     216         122 CONTAINS_OP              0
-                                 124 JUMP_IF_TRUE_OR_POP     52 (to 230)
+                                  44 JUMP_IF_FALSE_OR_POP    31 (to 108)
                      
-                     218     >>  126 LOAD_GLOBAL              7 (NULL + isinstance)
-                                 138 LOAD_DEREF               2 (phone_number)
-                                 140 LOAD_GLOBAL             12 (Iterable)
-                                 152 PRECALL                  2
-                                 156 CALL                     2
-                                 166 JUMP_IF_FALSE_OR_POP    31 (to 230)
+                     234          46 LOAD_GLOBAL              7 (NULL + any)
+                                  58 LOAD_CLOSURE             2 (phones)
+                                  60 BUILD_TUPLE              1
+                                  62 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 234>)
+                                  64 MAKE_FUNCTION            8 (closure)
+                                  66 LOAD_FAST                1 (m)
+                                  68 LOAD_ATTR                4 (contacts)
+                                  78 GET_ITER
+                                  80 PRECALL                  0
+                                  84 CALL                     0
+                                  94 PRECALL                  1
+                                  98 CALL                     1
                      
-                     219         168 LOAD_GLOBAL             15 (NULL + any)
-                                 180 LOAD_CLOSURE             2 (phone_number)
-                                 182 BUILD_TUPLE              1
-                                 184 LOAD_CONST               2 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 219>)
-                                 186 MAKE_FUNCTION            8 (closure)
-                                 188 LOAD_FAST                1 (data)
-                                 190 LOAD_ATTR                5 (contacts)
-                                 200 GET_ITER
-                                 202 PRECALL                  0
-                                 206 CALL                     0
-                                 216 PRECALL                  1
-                                 220 CALL                     1
-                     
-                     215     >>  230 RETURN_VALUE
+                     233     >>  108 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 3
-                           stacksize : 3
-                           flags     : 16777267
-                           code
-                              0x4b00010097007c005d157d017c016a00000000000000000044005d0b7d
-                              027c026a0100000000000000005600970101008c0c8c1664005300
-                           217           0 RETURN_GENERATOR
-                                         2 POP_TOP
-                                         4 RESUME                   0
-                                         6 LOAD_FAST                0 (.0)
-                                   >>    8 FOR_ITER                21 (to 52)
-                                        10 STORE_FAST               1 (contact)
-                                        12 LOAD_FAST                1 (contact)
-                                        14 LOAD_ATTR                0 (phones)
-                                        24 GET_ITER
-                                   >>   26 FOR_ITER                11 (to 50)
-                                        28 STORE_FAST               2 (p)
-                                        30 LOAD_FAST                2 (p)
-                                        32 LOAD_ATTR                1 (phone)
-                                        42 YIELD_VALUE
-                                        44 RESUME                   1
-                                        46 POP_TOP
-                                        48 JUMP_BACKWARD           12 (to 26)
-                                   >>   50 JUMP_BACKWARD           22 (to 8)
-                                   >>   52 LOAD_CONST               0 (None)
-                                        54 RETURN_VALUE
-                           consts
-                              None
-                           names      ('phones', 'phone')
-                           varnames   ('.0', 'contact', 'p')
-                           freevars   ()
-                           cellvars   ()
-                           filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-                           name       '<genexpr>'
-                           firstlineno 217
-                           lnotab 0x
-                        code
-                           argcount  : 1
-                           nlocals   : 3
-                           stacksize : 4
+                           stacksize : 7
                            flags     : 16777267
                            code
-                              0x95014b00010097007c005d177d017c016a00000000000000000044005d
-                              0d7d027c026a010000000000000000890376005600970101008c0e8c1864
-                              005300
+                              0x95014b00010097007c005d307d017c016a00000000000000000044005d
+                              267d027403000000000000000000006a0200000000000000007406000000
+                              0000000000000064007c026a040000000000000000a6030000ab03000000
+                              0000000000890376005600970101008c278c3164015300
                                          0 COPY_FREE_VARS           1
                            
-                           219           2 RETURN_GENERATOR
+                           234           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
-                                   >>   10 FOR_ITER                23 (to 58)
+                                   >>   10 FOR_ITER                48 (to 108)
                                         12 STORE_FAST               1 (contact)
                                         14 LOAD_FAST                1 (contact)
                                         16 LOAD_ATTR                0 (phones)
                                         26 GET_ITER
-                                   >>   28 FOR_ITER                13 (to 56)
+                                   >>   28 FOR_ITER                38 (to 106)
                                         30 STORE_FAST               2 (p)
-                                        32 LOAD_FAST                2 (p)
-                                        34 LOAD_ATTR                1 (phone)
-                                        44 LOAD_DEREF               3 (phone_number)
-                                        46 CONTAINS_OP              0
-                                        48 YIELD_VALUE
-                                        50 RESUME                   1
-                                        52 POP_TOP
-                                        54 JUMP_BACKWARD           14 (to 28)
-                                   >>   56 JUMP_BACKWARD           24 (to 10)
-                                   >>   58 LOAD_CONST               0 (None)
-                                        60 RETURN_VALUE
+                                        32 LOAD_GLOBAL              3 (NULL + re)
+                                        44 LOAD_ATTR                2 (sub)
+                                        54 LOAD_GLOBAL              6 (_ONLY_NUMS_RE)
+                                        66 LOAD_CONST               0 ('')
+                                        68 LOAD_FAST                2 (p)
+                                        70 LOAD_ATTR                4 (phone)
+                                        80 PRECALL                  3
+                                        84 CALL                     3
+                                        94 LOAD_DEREF               3 (phones)
+                                        96 CONTAINS_OP              0
+                                        98 YIELD_VALUE
+                                       100 RESUME                   1
+                                       102 POP_TOP
+                                       104 JUMP_BACKWARD           39 (to 28)
+                                   >>  106 JUMP_BACKWARD           49 (to 10)
+                                   >>  108 LOAD_CONST               1 (None)
+                                       110 RETURN_VALUE
                            consts
+                              ''
                               None
-                           names      ('phones', 'phone')
+                           names      ('phones', 're', 'sub', '_ONLY_NUMS_RE', 'phone')
                            varnames   ('.0', 'contact', 'p')
-                           freevars   ('phone_number',)
+                           freevars   ('phones',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 219
+                           firstlineno 234
                            lnotab 0x
-                     names      ('type', 'Mt', 'CONTACTS', 'isinstance', 'str', 'contacts', 'Iterable', 'any')
-                     varnames   ('wa', 'data')
-                     freevars   ('phone_number',)
+                     names      ('type', 'Mt', 'CONTACTS', 'any', 'contacts')
+                     varnames   ('wa', 'm')
+                     freevars   ('phones',)
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 215
-                     lnotab 0x2e012c0120ff04022a013efc
+                     firstlineno 233
+                     lnotab 0x2e013eff
                names      ()
-               varnames   ('phone_number',)
+               varnames   ('phones',)
                freevars   ()
-               cellvars   ('phone_number',)
+               cellvars   ('phones',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 215
-               lnotab 0x
-            'Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]]'
-            'PHONE_NUMBER'
-            code
-               argcount  : 2
-               nlocals   : 2
-               stacksize : 5
-               flags     : 16777219
-               code
-                  0x97007c016a0000000000000000007402000000000000000000006a0200
-                  000000000000006b02000000006f27740700000000000000000000640184
-                  00640284007c016a0400000000000000004400a6000000ab000000000000
-                  0000004400a6000000ab000000000000000000a6010000ab010000000000
-                  0000005300
-               223           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
-                             4 LOAD_ATTR                0 (type)
-                            14 LOAD_GLOBAL              2 (Mt)
-                            26 LOAD_ATTR                2 (CONTACTS)
-                            36 COMPARE_OP               2 (==)
-                            42 JUMP_IF_FALSE_OR_POP    39 (to 122)
-               
-               224          44 LOAD_GLOBAL              7 (NULL + any)
-                            56 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 224>)
-                            58 MAKE_FUNCTION            0
-               
-               225          60 LOAD_CONST               2 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 225>)
-                            62 MAKE_FUNCTION            0
-                            64 LOAD_FAST                1 (data)
-                            66 LOAD_ATTR                4 (contacts)
-                            76 GET_ITER
-                            78 PRECALL                  0
-                            82 CALL                     0
-               
-               224          92 GET_ITER
-                            94 PRECALL                  0
-                            98 CALL                     0
-                           108 PRECALL                  1
-                           112 CALL                     1
-               
-               223     >>  122 RETURN_VALUE
-               consts
-                  None
-                  code
-                     argcount  : 1
-                     nlocals   : 2
-                     stacksize : 2
-                     flags     : 16777267
-                     code
-                        0x4b00010097007c005d0b7d017c016a0000000000000000005600970101
-                        008c0c64005300
-                     224           0 RETURN_GENERATOR
-                                   2 POP_TOP
-                                   4 RESUME                   0
-                                   6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                11 (to 32)
-                                  10 STORE_FAST               1 (p)
-                                  12 LOAD_FAST                1 (p)
-                                  14 LOAD_ATTR                0 (wa_id)
-                                  24 YIELD_VALUE
-                                  26 RESUME                   1
-                                  28 POP_TOP
-                                  30 JUMP_BACKWARD           12 (to 8)
-                             >>   32 LOAD_CONST               0 (None)
-                                  34 RETURN_VALUE
-                     consts
-                        None
-                     names      ('wa_id',)
-                     varnames   ('.0', 'p')
-                     freevars   ()
-                     cellvars   ()
-                     filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-                     name       '<genexpr>'
-                     firstlineno 224
-                     lnotab 0x
-                  code
-                     argcount  : 1
-                     nlocals   : 3
-                     stacksize : 3
-                     flags     : 16777267
-                     code
-                        0x4b00010097007c005d107d017c016a00000000000000000044005d067d
-                        027c025600970101008c078c1164005300
-                     225           0 RETURN_GENERATOR
-                                   2 POP_TOP
-                                   4 RESUME                   0
-                                   6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                16 (to 42)
-                                  10 STORE_FAST               1 (contact)
-                     
-                     226          12 LOAD_FAST                1 (contact)
-                                  14 LOAD_ATTR                0 (phones)
-                     
-                     225          24 GET_ITER
-                             >>   26 FOR_ITER                 6 (to 40)
-                                  28 STORE_FAST               2 (phone)
-                                  30 LOAD_FAST                2 (phone)
-                                  32 YIELD_VALUE
-                                  34 RESUME                   1
-                                  36 POP_TOP
-                                  38 JUMP_BACKWARD            7 (to 26)
-                             >>   40 JUMP_BACKWARD           17 (to 8)
-                             >>   42 LOAD_CONST               0 (None)
-                                  44 RETURN_VALUE
-                     consts
-                        None
-                     names      ('phones',)
-                     varnames   ('.0', 'contact', 'phone')
-                     freevars   ()
-                     cellvars   ()
-                     filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-                     name       '<genexpr>'
-                     firstlineno 225
-                     lnotab 0x0c010cff
-               names      ('type', 'Mt', 'CONTACTS', 'any', 'contacts')
-               varnames   ('wa', 'data')
-               freevars   ()
-               cellvars   ()
-               filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 223
-               lnotab 0x2c01100120ff1eff
-            'HAS_WA'
+               name       'phone'
+               firstlineno 227
+               lnotab 0x0406
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'COUNT_BETWEEN', 'PHONE_NUMBER', 'HAS_WA')
+            ('min_count', 'int', 'max_count', 'int', 'return', 'Callable[[Wa, Msg], bool]')
+            ('phones', 'str', 'return', 'Callable[[Wa, Msg], bool]')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__', 'HAS_WA', 'staticmethod', 'count', 'phone')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'ContactsFilter'
-         firstlineno 203
-         lnotab 0x0c0104021001020304ff0c03020304ff0c0702021004
+         firstlineno 211
+         lnotab 0x0c0104021001020210030202020106ff0e010204020106ff0e01
       'ContactsFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
             00000064055300
-         230           0 RESUME                   0
+         238           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('UnsupportedFilter')
+                       6 LOAD_CONST               0 ('UnsupportedMsgFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         231          12 LOAD_CONST               1 ('Useful filters for unsupported messages.')
+         239          12 LOAD_CONST               1 ('Useful filters for unsupported messages.')
                       14 STORE_NAME               3 (__doc__)
          
-         233          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 233>)
+         241          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 241>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (ANY)
                       22 LOAD_CONST               3 ('Callable[[Wa, Msg], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('ANY')
                       28 STORE_SUBSCR
          
-         234          32 LOAD_CONST               5 (None)
+         242          32 LOAD_CONST               5 (None)
                       34 RETURN_VALUE
          consts
-            'UnsupportedFilter'
+            'UnsupportedMsgFilter'
             'Useful filters for unsupported messages.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               233           0 RESUME                   0
-                             2 LOAD_FAST                1 (data)
+               241           0 RESUME                   0
+                             2 LOAD_FAST                1 (m)
                              4 LOAD_ATTR                0 (type)
                             14 LOAD_GLOBAL              2 (Mt)
                             26 LOAD_ATTR                2 (UNSUPPORTED)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('type', 'Mt', 'UNSUPPORTED')
-               varnames   ('wa', 'data')
+               varnames   ('wa', 'm')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 233
+               firstlineno 241
                lnotab 0x
             'Callable[[Wa, Msg], bool]'
             'ANY'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'ANY', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-         name       'UnsupportedFilter'
-         firstlineno 230
+         name       'UnsupportedMsgFilter'
+         firstlineno 238
          lnotab 0x0c0104021001
-      'UnsupportedFilter'
+      'UnsupportedMsgFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
-            0x970065005a0164005a02550064015a03640284005a046403650564043c
-            0000000900640584005a066403650564063c0000000900640784005a0764
-            03650564083c0000000900640984005a0864036505640a3c000000090064
-            0b84005a0964036505640c3c000000640d5300
-         237           0 RESUME                   0
+            0x970065005a0164005a0264015a036504640e64068404a6000000ab0000
+            000000000000005a056504640e64078404a6000000ab0000000000000000
+            005a066504640e64088404a6000000ab0000000000000000005a07650464
+            0e64098404a6000000ab0000000000000000005a086504640f640c8404a6
+            000000ab0000000000000000005a09640d5300
+         245           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CallbackFilter')
                        8 STORE_NAME               2 (__qualname__)
-                      10 SETUP_ANNOTATIONS
          
-         238          12 LOAD_CONST               1 ('Useful filters for callback queries.')
-                      14 STORE_NAME               3 (__doc__)
+         246          10 LOAD_CONST               1 ('Useful filters for callback queries.')
+                      12 STORE_NAME               3 (__doc__)
          
-         241          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 241>)
-                      18 MAKE_FUNCTION            0
+         248          14 LOAD_NAME                4 (staticmethod)
          
-         240          20 STORE_NAME               4 (DATA_EQUALS)
-                      22 LOAD_CONST               3 ('Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]]')
-                      24 LOAD_NAME                5 (__annotations__)
-                      26 LOAD_CONST               4 ('DATA_EQUALS')
-                      28 STORE_SUBSCR
+         249          16 LOAD_CONST              14 (('matches', 'str', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]'))
+                      18 LOAD_CONST               6 (<code object data_equals, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 248>)
+                      20 MAKE_FUNCTION            4 (annotations)
          
-         243          32 NOP
+         248          22 PRECALL                  0
+                      26 CALL                     0
          
-         246          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 246>)
-                      36 MAKE_FUNCTION            0
+         249          36 STORE_NAME               5 (data_equals)
          
-         245          38 STORE_NAME               6 (DATA_STARTS_WITH)
-                      40 LOAD_CONST               3 ('Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]]')
-                      42 LOAD_NAME                5 (__annotations__)
-                      44 LOAD_CONST               6 ('DATA_STARTS_WITH')
-                      46 STORE_SUBSCR
+         253          38 LOAD_NAME                4 (staticmethod)
          
-         248          50 NOP
+         254          40 LOAD_CONST              14 (('matches', 'str', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]'))
+                      42 LOAD_CONST               7 (<code object data_starts_with, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 253>)
+                      44 MAKE_FUNCTION            4 (annotations)
          
-         251          52 LOAD_CONST               7 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 251>)
-                      54 MAKE_FUNCTION            0
+         253          46 PRECALL                  0
+                      50 CALL                     0
          
-         250          56 STORE_NAME               7 (DATA_ENDS_WITH)
-                      58 LOAD_CONST               3 ('Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]]')
-                      60 LOAD_NAME                5 (__annotations__)
-                      62 LOAD_CONST               8 ('DATA_ENDS_WITH')
-                      64 STORE_SUBSCR
+         254          60 STORE_NAME               6 (data_starts_with)
+         
+         258          62 LOAD_NAME                4 (staticmethod)
+         
+         259          64 LOAD_CONST              14 (('matches', 'str', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]'))
+                      66 LOAD_CONST               8 (<code object data_ends_with, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 258>)
+                      68 MAKE_FUNCTION            4 (annotations)
+         
+         258          70 PRECALL                  0
+                      74 CALL                     0
+         
+         259          84 STORE_NAME               7 (data_ends_with)
+         
+         263          86 LOAD_NAME                4 (staticmethod)
+         
+         264          88 LOAD_CONST              14 (('matches', 'str', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]'))
+                      90 LOAD_CONST               9 (<code object data_contains, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 263>)
+                      92 MAKE_FUNCTION            4 (annotations)
+         
+         263          94 PRECALL                  0
+                      98 CALL                     0
          
-         253          68 NOP
+         264         108 STORE_NAME               8 (data_contains)
          
-         256          70 LOAD_CONST               9 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 256>)
-                      72 MAKE_FUNCTION            0
+         268         110 LOAD_NAME                4 (staticmethod)
          
-         255          74 STORE_NAME               8 (DATA_CONTAINS)
-                      76 LOAD_CONST               3 ('Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]]')
-                      78 LOAD_NAME                5 (__annotations__)
-                      80 LOAD_CONST              10 ('DATA_CONTAINS')
-                      82 STORE_SUBSCR
-         
-         258          86 NOP
-         
-         261          88 LOAD_CONST              11 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 261>)
-                      90 MAKE_FUNCTION            0
-         
-         260          92 STORE_NAME               9 (DATA_REGEX)
-                      94 LOAD_CONST               3 ('Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]]')
-                      96 LOAD_NAME                5 (__annotations__)
-                      98 LOAD_CONST              12 ('DATA_REGEX')
-                     100 STORE_SUBSCR
+         269         112 LOAD_CONST              15 (('patterns', 'str | re.Pattern', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]'))
+                     114 LOAD_CONST              12 (<code object data_regex, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 268>)
+                     116 MAKE_FUNCTION            4 (annotations)
          
-         263         104 LOAD_CONST              13 (None)
-                     106 RETURN_VALUE
+         268         118 PRECALL                  0
+                     122 CALL                     0
+         
+         269         132 STORE_NAME               9 (data_regex)
+                     134 LOAD_CONST              13 (None)
+                     136 RETURN_VALUE
          consts
             'CallbackFilter'
             'Useful filters for callback queries.'
+            'matches'
+            'str'
+            'return'
+            'Callable[[Wa, CallbackButton | CallbackSelection], bool]'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (data)
+                             0 MAKE_CELL                0 (matches)
+               
+               248           2 RESUME                   0
                
-               241           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (data)
+               251           4 LOAD_CLOSURE             0 (matches)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 241>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 251>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  'Filter for callbacks their data equals the given string/s.'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
-                        0x9501870197007401000000000000000000008902740200000000000000
-                        000000a6020000ab020000000000000000720b89016a0200000000000000
-                        0089026b02000000006e1a74070000000000000000000088016601640184
-                        0889024400a6000000ab000000000000000000a6010000ab010000000000
-                        0000005300
+                        0x9501870197007401000000000000000000008801660164018408890244
+                        00a6000000ab000000000000000000a6010000ab01000000000000000053
+                        00
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data_)
-                     
-                     241           4 RESUME                   0
-                                   6 LOAD_GLOBAL              1 (NULL + isinstance)
-                                  18 LOAD_DEREF               2 (data)
-                                  20 LOAD_GLOBAL              2 (str)
-                                  32 PRECALL                  2
-                                  36 CALL                     2
-                                  46 POP_JUMP_FORWARD_IF_FALSE    11 (to 70)
-                                  48 LOAD_DEREF               1 (data_)
-                                  50 LOAD_ATTR                2 (data)
-                                  60 LOAD_DEREF               2 (data)
-                                  62 COMPARE_OP               2 (==)
-                                  68 JUMP_FORWARD            26 (to 122)
-                             >>   70 LOAD_GLOBAL              7 (NULL + any)
+                                   2 MAKE_CELL                1 (c)
                      
-                     242          82 LOAD_CLOSURE             1 (data_)
-                                  84 BUILD_TUPLE              1
-                                  86 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 242>)
-                                  88 MAKE_FUNCTION            8 (closure)
-                                  90 LOAD_DEREF               2 (data)
-                                  92 GET_ITER
-                                  94 PRECALL                  0
-                                  98 CALL                     0
-                     
-                     241         108 PRECALL                  1
-                                 112 CALL                     1
-                             >>  122 RETURN_VALUE
+                     251           4 RESUME                   0
+                                   6 LOAD_GLOBAL              1 (NULL + any)
+                                  18 LOAD_CLOSURE             1 (c)
+                                  20 BUILD_TUPLE              1
+                                  22 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 251>)
+                                  24 MAKE_FUNCTION            8 (closure)
+                                  26 LOAD_DEREF               2 (matches)
+                                  28 GET_ITER
+                                  30 PRECALL                  0
+                                  34 CALL                     0
+                                  44 PRECALL                  1
+                                  48 CALL                     1
+                                  58 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 3
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d0f7d0189026a0000000000000000007c016b
                               02000000005600970101008c1064005300
                                          0 COPY_FREE_VARS           1
                            
-                           242           2 RETURN_GENERATOR
+                           251           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                15 (to 42)
-                                        12 STORE_FAST               1 (d)
-                                        14 LOAD_DEREF               2 (data_)
+                                        12 STORE_FAST               1 (m)
+                                        14 LOAD_DEREF               2 (c)
                                         16 LOAD_ATTR                0 (data)
-                                        26 LOAD_FAST                1 (d)
+                                        26 LOAD_FAST                1 (m)
                                         28 COMPARE_OP               2 (==)
                                         34 YIELD_VALUE
                                         36 RESUME                   1
                                         38 POP_TOP
                                         40 JUMP_BACKWARD           16 (to 10)
                                    >>   42 LOAD_CONST               0 (None)
                                         44 RETURN_VALUE
                            consts
                               None
                            names      ('data',)
-                           varnames   ('.0', 'd')
-                           freevars   ('data_',)
+                           varnames   ('.0', 'm')
+                           freevars   ('c',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 242
+                           firstlineno 251
                            lnotab 0x
-                     names      ('isinstance', 'str', 'data', 'any')
-                     varnames   ('wa', 'data_')
-                     freevars   ('data',)
-                     cellvars   ('data_',)
+                     names      ('any',)
+                     varnames   ('wa', 'c')
+                     freevars   ('matches',)
+                     cellvars   ('c',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 241
-                     lnotab 0x52011aff
+                     firstlineno 251
+                     lnotab 0x
                names      ()
-               varnames   ('data',)
+               varnames   ('matches',)
                freevars   ()
-               cellvars   ('data',)
+               cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 241
-               lnotab 0x
-            'Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]]'
-            'DATA_EQUALS'
+               name       'data_equals'
+               firstlineno 248
+               lnotab 0x0403
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (data)
+                             0 MAKE_CELL                0 (matches)
                
-               246           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (data)
+               253           2 RESUME                   0
+               
+               256           4 LOAD_CLOSURE             0 (matches)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 246>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 256>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  'Filter for callbacks their data starts with the given string/s.'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
-                        0x9501870197007401000000000000000000008902740200000000000000
-                        000000a6020000ab020000000000000000721a89016a0200000000000000
-                        00a00300000000000000000000000000000000000000008902a6010000ab
-                        0100000000000000006e1a74090000000000000000000088016601640184
-                        0889024400a6000000ab000000000000000000a6010000ab010000000000
-                        0000005300
+                        0x9501870197007401000000000000000000008801660164018408890244
+                        00a6000000ab000000000000000000a6010000ab01000000000000000053
+                        00
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data_)
-                     
-                     246           4 RESUME                   0
-                                   6 LOAD_GLOBAL              1 (NULL + isinstance)
-                                  18 LOAD_DEREF               2 (data)
-                                  20 LOAD_GLOBAL              2 (str)
-                                  32 PRECALL                  2
-                                  36 CALL                     2
-                                  46 POP_JUMP_FORWARD_IF_FALSE    26 (to 100)
-                                  48 LOAD_DEREF               1 (data_)
-                                  50 LOAD_ATTR                2 (data)
-                                  60 LOAD_METHOD              3 (startswith)
-                                  82 LOAD_DEREF               2 (data)
-                                  84 PRECALL                  1
-                                  88 CALL                     1
-                                  98 JUMP_FORWARD            26 (to 152)
-                             >>  100 LOAD_GLOBAL              9 (NULL + any)
-                     
-                     247         112 LOAD_CLOSURE             1 (data_)
-                                 114 BUILD_TUPLE              1
-                                 116 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 247>)
-                                 118 MAKE_FUNCTION            8 (closure)
-                                 120 LOAD_DEREF               2 (data)
-                                 122 GET_ITER
-                                 124 PRECALL                  0
-                                 128 CALL                     0
+                                   2 MAKE_CELL                1 (c)
                      
-                     246         138 PRECALL                  1
-                                 142 CALL                     1
-                             >>  152 RETURN_VALUE
+                     256           4 RESUME                   0
+                                   6 LOAD_GLOBAL              1 (NULL + any)
+                                  18 LOAD_CLOSURE             1 (c)
+                                  20 BUILD_TUPLE              1
+                                  22 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 256>)
+                                  24 MAKE_FUNCTION            8 (closure)
+                                  26 LOAD_DEREF               2 (matches)
+                                  28 GET_ITER
+                                  30 PRECALL                  0
+                                  34 CALL                     0
+                                  44 PRECALL                  1
+                                  48 CALL                     1
+                                  58 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 4
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d1e7d0189026a000000000000000000a00100
                               000000000000000000000000000000000000007c01a6010000ab01000000
                               00000000005600970101008c1f64005300
                                          0 COPY_FREE_VARS           1
                            
-                           247           2 RETURN_GENERATOR
+                           256           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                30 (to 72)
-                                        12 STORE_FAST               1 (d)
-                                        14 LOAD_DEREF               2 (data_)
+                                        12 STORE_FAST               1 (m)
+                                        14 LOAD_DEREF               2 (c)
                                         16 LOAD_ATTR                0 (data)
                                         26 LOAD_METHOD              1 (startswith)
-                                        48 LOAD_FAST                1 (d)
+                                        48 LOAD_FAST                1 (m)
                                         50 PRECALL                  1
                                         54 CALL                     1
                                         64 YIELD_VALUE
                                         66 RESUME                   1
                                         68 POP_TOP
                                         70 JUMP_BACKWARD           31 (to 10)
                                    >>   72 LOAD_CONST               0 (None)
                                         74 RETURN_VALUE
                            consts
                               None
                            names      ('data', 'startswith')
-                           varnames   ('.0', 'd')
-                           freevars   ('data_',)
+                           varnames   ('.0', 'm')
+                           freevars   ('c',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 247
+                           firstlineno 256
                            lnotab 0x
-                     names      ('isinstance', 'str', 'data', 'startswith', 'any')
-                     varnames   ('wa', 'data_')
-                     freevars   ('data',)
-                     cellvars   ('data_',)
+                     names      ('any',)
+                     varnames   ('wa', 'c')
+                     freevars   ('matches',)
+                     cellvars   ('c',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 246
-                     lnotab 0x70011aff
+                     firstlineno 256
+                     lnotab 0x
                names      ()
-               varnames   ('data',)
+               varnames   ('matches',)
                freevars   ()
-               cellvars   ('data',)
+               cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 246
-               lnotab 0x
-            'DATA_STARTS_WITH'
+               name       'data_starts_with'
+               firstlineno 253
+               lnotab 0x0403
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (data)
+                             0 MAKE_CELL                0 (matches)
+               
+               258           2 RESUME                   0
                
-               251           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (data)
+               261           4 LOAD_CLOSURE             0 (matches)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 251>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 261>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  'Filter for callbacks their data ends with the given string/s.'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
-                        0x9501870197007401000000000000000000008902740200000000000000
-                        000000a6020000ab020000000000000000721a89016a0200000000000000
-                        00a00300000000000000000000000000000000000000008902a6010000ab
-                        0100000000000000006e1a74090000000000000000000088016601640184
-                        0889024400a6000000ab000000000000000000a6010000ab010000000000
-                        0000005300
+                        0x9501870197007401000000000000000000008801660164018408890244
+                        00a6000000ab000000000000000000a6010000ab01000000000000000053
+                        00
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data_)
-                     
-                     251           4 RESUME                   0
-                                   6 LOAD_GLOBAL              1 (NULL + isinstance)
-                                  18 LOAD_DEREF               2 (data)
-                                  20 LOAD_GLOBAL              2 (str)
-                                  32 PRECALL                  2
-                                  36 CALL                     2
-                                  46 POP_JUMP_FORWARD_IF_FALSE    26 (to 100)
-                                  48 LOAD_DEREF               1 (data_)
-                                  50 LOAD_ATTR                2 (data)
-                                  60 LOAD_METHOD              3 (endswith)
-                                  82 LOAD_DEREF               2 (data)
-                                  84 PRECALL                  1
-                                  88 CALL                     1
-                                  98 JUMP_FORWARD            26 (to 152)
-                             >>  100 LOAD_GLOBAL              9 (NULL + any)
-                     
-                     252         112 LOAD_CLOSURE             1 (data_)
-                                 114 BUILD_TUPLE              1
-                                 116 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 252>)
-                                 118 MAKE_FUNCTION            8 (closure)
-                                 120 LOAD_DEREF               2 (data)
-                                 122 GET_ITER
-                                 124 PRECALL                  0
-                                 128 CALL                     0
+                                   2 MAKE_CELL                1 (c)
                      
-                     251         138 PRECALL                  1
-                                 142 CALL                     1
-                             >>  152 RETURN_VALUE
+                     261           4 RESUME                   0
+                                   6 LOAD_GLOBAL              1 (NULL + any)
+                                  18 LOAD_CLOSURE             1 (c)
+                                  20 BUILD_TUPLE              1
+                                  22 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 261>)
+                                  24 MAKE_FUNCTION            8 (closure)
+                                  26 LOAD_DEREF               2 (matches)
+                                  28 GET_ITER
+                                  30 PRECALL                  0
+                                  34 CALL                     0
+                                  44 PRECALL                  1
+                                  48 CALL                     1
+                                  58 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 4
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d1e7d0189026a000000000000000000a00100
                               000000000000000000000000000000000000007c01a6010000ab01000000
                               00000000005600970101008c1f64005300
                                          0 COPY_FREE_VARS           1
                            
-                           252           2 RETURN_GENERATOR
+                           261           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                30 (to 72)
-                                        12 STORE_FAST               1 (d)
-                                        14 LOAD_DEREF               2 (data_)
+                                        12 STORE_FAST               1 (m)
+                                        14 LOAD_DEREF               2 (c)
                                         16 LOAD_ATTR                0 (data)
                                         26 LOAD_METHOD              1 (endswith)
-                                        48 LOAD_FAST                1 (d)
+                                        48 LOAD_FAST                1 (m)
                                         50 PRECALL                  1
                                         54 CALL                     1
                                         64 YIELD_VALUE
                                         66 RESUME                   1
                                         68 POP_TOP
                                         70 JUMP_BACKWARD           31 (to 10)
                                    >>   72 LOAD_CONST               0 (None)
                                         74 RETURN_VALUE
                            consts
                               None
                            names      ('data', 'endswith')
-                           varnames   ('.0', 'd')
-                           freevars   ('data_',)
+                           varnames   ('.0', 'm')
+                           freevars   ('c',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 252
+                           firstlineno 261
                            lnotab 0x
-                     names      ('isinstance', 'str', 'data', 'endswith', 'any')
-                     varnames   ('wa', 'data_')
-                     freevars   ('data',)
-                     cellvars   ('data_',)
+                     names      ('any',)
+                     varnames   ('wa', 'c')
+                     freevars   ('matches',)
+                     cellvars   ('c',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 251
-                     lnotab 0x70011aff
+                     firstlineno 261
+                     lnotab 0x
                names      ()
-               varnames   ('data',)
+               varnames   ('matches',)
                freevars   ()
-               cellvars   ('data',)
+               cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 251
-               lnotab 0x
-            'DATA_ENDS_WITH'
+               name       'data_ends_with'
+               firstlineno 258
+               lnotab 0x0403
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (data)
+                             0 MAKE_CELL                0 (matches)
+               
+               263           2 RESUME                   0
                
-               256           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (data)
+               266           4 LOAD_CLOSURE             0 (matches)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 256>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 266>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  'Filter for callbacks their data contains the given string/s.'
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
-                        0x9501870197007401000000000000000000008902740200000000000000
-                        000000a6020000ab0200000000000000007209890289016a020000000000
-                        00000076006e1a7407000000000000000000008801660164018408890244
+                        0x9501870197007401000000000000000000008801660164018408890244
                         00a6000000ab000000000000000000a6010000ab01000000000000000053
                         00
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data_)
+                                   2 MAKE_CELL                1 (c)
                      
-                     256           4 RESUME                   0
-                                   6 LOAD_GLOBAL              1 (NULL + isinstance)
-                                  18 LOAD_DEREF               2 (data)
-                                  20 LOAD_GLOBAL              2 (str)
-                                  32 PRECALL                  2
-                                  36 CALL                     2
-                                  46 POP_JUMP_FORWARD_IF_FALSE     9 (to 66)
-                                  48 LOAD_DEREF               2 (data)
-                                  50 LOAD_DEREF               1 (data_)
-                                  52 LOAD_ATTR                2 (data)
-                                  62 CONTAINS_OP              0
-                                  64 JUMP_FORWARD            26 (to 118)
-                             >>   66 LOAD_GLOBAL              7 (NULL + any)
-                     
-                     257          78 LOAD_CLOSURE             1 (data_)
-                                  80 BUILD_TUPLE              1
-                                  82 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 257>)
-                                  84 MAKE_FUNCTION            8 (closure)
-                                  86 LOAD_DEREF               2 (data)
-                                  88 GET_ITER
-                                  90 PRECALL                  0
-                                  94 CALL                     0
-                     
-                     256         104 PRECALL                  1
-                                 108 CALL                     1
-                             >>  118 RETURN_VALUE
+                     266           4 RESUME                   0
+                                   6 LOAD_GLOBAL              1 (NULL + any)
+                                  18 LOAD_CLOSURE             1 (c)
+                                  20 BUILD_TUPLE              1
+                                  22 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 266>)
+                                  24 MAKE_FUNCTION            8 (closure)
+                                  26 LOAD_DEREF               2 (matches)
+                                  28 GET_ITER
+                                  30 PRECALL                  0
+                                  34 CALL                     0
+                                  44 PRECALL                  1
+                                  48 CALL                     1
+                                  58 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 3
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d0d7d017c0189026a00000000000000000076
                               005600970101008c0e64005300
                                          0 COPY_FREE_VARS           1
                            
-                           257           2 RETURN_GENERATOR
+                           266           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                13 (to 38)
-                                        12 STORE_FAST               1 (d)
-                                        14 LOAD_FAST                1 (d)
-                                        16 LOAD_DEREF               2 (data_)
+                                        12 STORE_FAST               1 (m)
+                                        14 LOAD_FAST                1 (m)
+                                        16 LOAD_DEREF               2 (c)
                                         18 LOAD_ATTR                0 (data)
                                         28 CONTAINS_OP              0
                                         30 YIELD_VALUE
                                         32 RESUME                   1
                                         34 POP_TOP
                                         36 JUMP_BACKWARD           14 (to 10)
                                    >>   38 LOAD_CONST               0 (None)
                                         40 RETURN_VALUE
                            consts
                               None
                            names      ('data',)
-                           varnames   ('.0', 'd')
-                           freevars   ('data_',)
+                           varnames   ('.0', 'm')
+                           freevars   ('c',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 257
+                           firstlineno 266
                            lnotab 0x
-                     names      ('isinstance', 'str', 'data', 'any')
-                     varnames   ('wa', 'data_')
-                     freevars   ('data',)
-                     cellvars   ('data_',)
+                     names      ('any',)
+                     varnames   ('wa', 'c')
+                     freevars   ('matches',)
+                     cellvars   ('c',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 256
-                     lnotab 0x4e011aff
+                     firstlineno 266
+                     lnotab 0x
                names      ()
-               varnames   ('data',)
+               varnames   ('matches',)
                freevars   ()
-               cellvars   ('data',)
+               cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 256
-               lnotab 0x
-            'DATA_CONTAINS'
+               name       'data_contains'
+               firstlineno 263
+               lnotab 0x0403
+            'patterns'
+            'str | re.Pattern'
             code
-               argcount  : 1
+               argcount  : 0
                nlocals   : 1
                stacksize : 2
-               flags     : 16777219
+               flags     : 16777223
                code 0x8700970088006601640184085300
-                             0 MAKE_CELL                0 (regex)
+                             0 MAKE_CELL                0 (patterns)
                
-               261           2 RESUME                   0
-                             4 LOAD_CLOSURE             0 (regex)
+               268           2 RESUME                   0
+               
+               274           4 LOAD_CLOSURE             0 (patterns)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 261>)
+                             8 LOAD_CONST               1 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 274>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 RETURN_VALUE
                consts
-                  None
+                  "\n        Filter for callbacks their data matches the given regex/regexes.\n            * It's recommended to pass compiled regexes to save time (``re.compile(your_pattern)``)\n        "
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 16777235
                      code
-                        0x9501870197007401000000000000000000008902740200000000000000
-                        000000a6020000ab020000000000000000721a7405000000000000000000
-                        006a030000000000000000890289016a040000000000000000a6020000ab
-                        0200000000000000006e1a740b0000000000000000000088016601640184
-                        0889024400a6000000ab000000000000000000a6010000ab010000000000
-                        0000005300
+                        0x9501870197007401000000000000000000008801660164018408890244
+                        00a6000000ab000000000000000000a6010000ab01000000000000000053
+                        00
                                    0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (data_)
-                     
-                     261           4 RESUME                   0
-                                   6 LOAD_GLOBAL              1 (NULL + isinstance)
-                                  18 LOAD_DEREF               2 (regex)
-                                  20 LOAD_GLOBAL              2 (str)
-                                  32 PRECALL                  2
-                                  36 CALL                     2
-                                  46 POP_JUMP_FORWARD_IF_FALSE    26 (to 100)
-                                  48 LOAD_GLOBAL              5 (NULL + re)
-                                  60 LOAD_ATTR                3 (match)
-                                  70 LOAD_DEREF               2 (regex)
-                                  72 LOAD_DEREF               1 (data_)
-                                  74 LOAD_ATTR                4 (data)
-                                  84 PRECALL                  2
-                                  88 CALL                     2
-                                  98 JUMP_FORWARD            26 (to 152)
-                             >>  100 LOAD_GLOBAL             11 (NULL + any)
+                                   2 MAKE_CELL                1 (c)
                      
-                     262         112 LOAD_CLOSURE             1 (data_)
-                                 114 BUILD_TUPLE              1
-                                 116 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 262>)
-                                 118 MAKE_FUNCTION            8 (closure)
-                                 120 LOAD_DEREF               2 (regex)
-                                 122 GET_ITER
-                                 124 PRECALL                  0
-                                 128 CALL                     0
-                     
-                     261         138 PRECALL                  1
-                                 142 CALL                     1
-                             >>  152 RETURN_VALUE
+                     274           4 RESUME                   0
+                                   6 LOAD_GLOBAL              1 (NULL + any)
+                                  18 LOAD_CLOSURE             1 (c)
+                                  20 BUILD_TUPLE              1
+                                  22 LOAD_CONST               1 (<code object <genexpr>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 274>)
+                                  24 MAKE_FUNCTION            8 (closure)
+                                  26 LOAD_DEREF               2 (patterns)
+                                  28 GET_ITER
+                                  30 PRECALL                  0
+                                  34 CALL                     0
+                                  44 PRECALL                  1
+                                  48 CALL                     1
+                                  58 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 5
                            flags     : 16777267
                            code
                               0x95014b00010097007c005d1e7d017401000000000000000000006a0100
                               000000000000007c0189026a020000000000000000a6020000ab02000000
                               00000000005600970101008c1f64005300
                                          0 COPY_FREE_VARS           1
                            
-                           262           2 RETURN_GENERATOR
+                           274           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                30 (to 72)
-                                        12 STORE_FAST               1 (r)
+                                        12 STORE_FAST               1 (p)
                                         14 LOAD_GLOBAL              1 (NULL + re)
                                         26 LOAD_ATTR                1 (match)
-                                        36 LOAD_FAST                1 (r)
-                                        38 LOAD_DEREF               2 (data_)
+                                        36 LOAD_FAST                1 (p)
+                                        38 LOAD_DEREF               2 (c)
                                         40 LOAD_ATTR                2 (data)
                                         50 PRECALL                  2
                                         54 CALL                     2
                                         64 YIELD_VALUE
                                         66 RESUME                   1
                                         68 POP_TOP
                                         70 JUMP_BACKWARD           31 (to 10)
                                    >>   72 LOAD_CONST               0 (None)
                                         74 RETURN_VALUE
                            consts
                               None
                            names      ('re', 'match', 'data')
-                           varnames   ('.0', 'r')
-                           freevars   ('data_',)
+                           varnames   ('.0', 'p')
+                           freevars   ('c',)
                            cellvars   ()
                            filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                            name       '<genexpr>'
-                           firstlineno 262
+                           firstlineno 274
                            lnotab 0x
-                     names      ('isinstance', 'str', 're', 'match', 'data', 'any')
-                     varnames   ('wa', 'data_')
-                     freevars   ('regex',)
-                     cellvars   ('data_',)
+                     names      ('any',)
+                     varnames   ('wa', 'c')
+                     freevars   ('patterns',)
+                     cellvars   ('c',)
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                      name       '<lambda>'
-                     firstlineno 261
-                     lnotab 0x70011aff
+                     firstlineno 274
+                     lnotab 0x
                names      ()
-               varnames   ('regex',)
+               varnames   ('patterns',)
                freevars   ()
-               cellvars   ('regex',)
+               cellvars   ('patterns',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       '<lambda>'
-               firstlineno 261
-               lnotab 0x
-            'DATA_REGEX'
+               name       'data_regex'
+               firstlineno 268
+               lnotab 0x0406
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'DATA_EQUALS', '__annotations__', 'DATA_STARTS_WITH', 'DATA_ENDS_WITH', 'DATA_CONTAINS', 'DATA_REGEX')
+            ('matches', 'str', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]')
+            ('patterns', 'str | re.Pattern', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'staticmethod', 'data_equals', 'data_starts_with', 'data_ends_with', 'data_contains', 'data_regex')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'CallbackFilter'
-         firstlineno 237
+         firstlineno 245
          lnotab
-            0x0c01040304ff0c03020304ff0c03020304ff0c03020304ff0c03020304
-            ff0c03
+            0x0a010402020106ff0e010204020106ff0e010204020106ff0e01020402
+            0106ff0e010204020106ff0e01
       'CallbackFilter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a03640284005a046403650564043c
             0000000900640584005a066403650564063c0000000900640784005a0764
             03650564083c00000064095300
-         266           0 RESUME                   0
+         277           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MessageStatusFilter')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         267          12 LOAD_CONST               1 ('Useful filters for message status updates.')
+         278          12 LOAD_CONST               1 ('Useful filters for message status updates.')
                       14 STORE_NAME               3 (__doc__)
          
-         269          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 269>)
+         280          16 LOAD_CONST               2 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 280>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (SENT)
                       22 LOAD_CONST               3 ('Callable[[Wa, Ms], bool]')
                       24 LOAD_NAME                5 (__annotations__)
                       26 LOAD_CONST               4 ('SENT')
                       28 STORE_SUBSCR
          
-         270          32 NOP
+         281          32 NOP
          
-         272          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 272>)
+         283          34 LOAD_CONST               5 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 283>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               6 (DELIVERED)
                       40 LOAD_CONST               3 ('Callable[[Wa, Ms], bool]')
                       42 LOAD_NAME                5 (__annotations__)
                       44 LOAD_CONST               6 ('DELIVERED')
                       46 STORE_SUBSCR
          
-         273          50 NOP
+         284          50 NOP
          
-         275          52 LOAD_CONST               7 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 275>)
+         286          52 LOAD_CONST               7 (<code object <lambda>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 286>)
                       54 MAKE_FUNCTION            0
                       56 STORE_NAME               7 (READ)
                       58 LOAD_CONST               3 ('Callable[[Wa, Ms], bool]')
                       60 LOAD_NAME                5 (__annotations__)
                       62 LOAD_CONST               8 ('READ')
                       64 STORE_SUBSCR
          
-         276          68 LOAD_CONST               9 (None)
+         287          68 LOAD_CONST               9 (None)
                       70 RETURN_VALUE
          consts
             'MessageStatusFilter'
             'Useful filters for message status updates.'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               269           0 RESUME                   0
+               280           0 RESUME                   0
                              2 LOAD_FAST                1 (data)
                              4 LOAD_ATTR                0 (status)
                             14 LOAD_GLOBAL              2 (Mst)
                             26 LOAD_ATTR                2 (SENT)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('status', 'Mst', 'SENT')
                varnames   ('wa', 'data')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 269
+               firstlineno 280
                lnotab 0x
             'Callable[[Wa, Ms], bool]'
             'SENT'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               272           0 RESUME                   0
+               283           0 RESUME                   0
                              2 LOAD_FAST                1 (data)
                              4 LOAD_ATTR                0 (status)
                             14 LOAD_GLOBAL              2 (Mst)
                             26 LOAD_ATTR                2 (DELIVERED)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('status', 'Mst', 'DELIVERED')
                varnames   ('wa', 'data')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 272
+               firstlineno 283
                lnotab 0x
             'DELIVERED'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c016a0000000000000000007402000000000000000000006a0200
                   000000000000006b02000000005300
-               275           0 RESUME                   0
+               286           0 RESUME                   0
                              2 LOAD_FAST                1 (data)
                              4 LOAD_ATTR                0 (status)
                             14 LOAD_GLOBAL              2 (Mst)
                             26 LOAD_ATTR                2 (READ)
                             36 COMPARE_OP               2 (==)
                             42 RETURN_VALUE
                consts
                   None
                names      ('status', 'Mst', 'READ')
                varnames   ('wa', 'data')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       '<lambda>'
-               firstlineno 275
+               firstlineno 286
                lnotab 0x
             'READ'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'SENT', '__annotations__', 'DELIVERED', 'READ')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'MessageStatusFilter'
-         firstlineno 266
+         firstlineno 277
          lnotab 0x0c01040210010202100102021001
       'MessageStatusFilter'
-   names      ('__doc__', '__future__', 'annotations', 're', 'typing', 'Callable', 'TYPE_CHECKING', 'Iterable', 'pywa.types', 'MessageType', 'Mt', 'Message', 'Msg', 'MessageStatus', 'Ms', 'MessageStatusType', 'Mst', 'CallbackButton', 'CallbackSelection', 'pywa', 'utils', 'WhatsApp', 'Wa', 'TextFilter', 'ImageFilter', 'VideoFilter', 'AudioFilter', 'DocumentFilter', 'StickerFilter', 'LocationFilter', 'ReactionFilter', 'ContactsFilter', 'UnsupportedFilter', 'CallbackFilter', 'MessageStatusFilter')
+   names      ('__doc__', '__future__', 'annotations', 're', 'typing', 'Callable', 'TYPE_CHECKING', 'Iterable', 'pywa', 'utils', 'pywa.types', 'MessageType', 'Mt', 'Message', 'Msg', 'MessageStatus', 'Ms', 'MessageStatusType', 'Mst', 'CallbackButton', 'CallbackSelection', 'WhatsApp', 'Wa', '__all__', 'compile', '_ONLY_NUMS_RE', 'TextFilter', 'ImageFilter', 'VideoFilter', 'AudioFilter', 'DocumentFilter', 'StickerFilter', 'LocationFilter', 'ReactionFilter', 'ContactsFilter', 'UnsupportedMsgFilter', 'CallbackFilter', 'MessageStatusFilter')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020104010c020801140120020c0204010c031a3f1a141a111a171a
-      111a0a1a1c1a0b1a1b1a071a1d
+      0x00ff020104010c02080114010c01200304010c02040e20031a381a141a
+      0f1a151a0f1a0c1a1c1a0e1a1b1a071a20
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/types.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4b0a9264 (Tue Jun 20 20:21:31 2023 UTC)
-files sz: 24771
+moddate:  0xfc6f9464 (Thu Jun 22 15:59:56 2023 UTC)
+files sz: 25776
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 16777216
    code
       0x9700640064016c006d015a01010064025a02640064036c036d035a0301
@@ -491,111 +491,111 @@
               1208 CALL                     2
    
    408        1218 PRECALL                  0
               1222 CALL                     0
    
    409        1232 STORE_NAME              35 (BaseUpdate)
    
-   668        1234 PUSH_NULL
+   695        1234 PUSH_NULL
               1236 LOAD_NAME                5 (dataclass)
               1238 LOAD_CONST               9 (True)
               1240 LOAD_CONST               9 (True)
               1242 KW_NAMES                10
               1244 PRECALL                  2
               1248 CALL                     2
    
-   669        1258 PUSH_NULL
+   696        1258 PUSH_NULL
               1260 LOAD_BUILD_CLASS
-              1262 LOAD_CONST              47 (<code object Message, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 668>)
+              1262 LOAD_CONST              47 (<code object Message, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 695>)
               1264 MAKE_FUNCTION            0
               1266 LOAD_CONST              48 ('Message')
               1268 LOAD_NAME               35 (BaseUpdate)
               1270 PRECALL                  3
               1274 CALL                     3
    
-   668        1284 PRECALL                  0
+   695        1284 PRECALL                  0
               1288 CALL                     0
    
-   669        1298 STORE_NAME              36 (Message)
+   696        1298 STORE_NAME              36 (Message)
    
-   728        1300 PUSH_NULL
+   755        1300 PUSH_NULL
               1302 LOAD_NAME                5 (dataclass)
               1304 LOAD_CONST               9 (True)
               1306 LOAD_CONST               9 (True)
               1308 KW_NAMES                10
               1310 PRECALL                  2
               1314 CALL                     2
    
-   729        1324 PUSH_NULL
+   756        1324 PUSH_NULL
               1326 LOAD_BUILD_CLASS
-              1328 LOAD_CONST              49 (<code object CallbackButton, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 728>)
+              1328 LOAD_CONST              49 (<code object CallbackButton, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 755>)
               1330 MAKE_FUNCTION            0
               1332 LOAD_CONST              50 ('CallbackButton')
               1334 LOAD_NAME               35 (BaseUpdate)
               1336 PRECALL                  3
               1340 CALL                     3
    
-   728        1350 PRECALL                  0
+   755        1350 PRECALL                  0
               1354 CALL                     0
    
-   729        1364 STORE_NAME              37 (CallbackButton)
+   756        1364 STORE_NAME              37 (CallbackButton)
    
-   758        1366 PUSH_NULL
+   785        1366 PUSH_NULL
               1368 LOAD_NAME                5 (dataclass)
               1370 LOAD_CONST               9 (True)
               1372 LOAD_CONST               9 (True)
               1374 KW_NAMES                10
               1376 PRECALL                  2
               1380 CALL                     2
    
-   759        1390 PUSH_NULL
+   786        1390 PUSH_NULL
               1392 LOAD_BUILD_CLASS
-              1394 LOAD_CONST              51 (<code object CallbackSelection, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 758>)
+              1394 LOAD_CONST              51 (<code object CallbackSelection, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 785>)
               1396 MAKE_FUNCTION            0
               1398 LOAD_CONST              52 ('CallbackSelection')
               1400 LOAD_NAME               35 (BaseUpdate)
               1402 PRECALL                  3
               1406 CALL                     3
    
-   758        1416 PRECALL                  0
+   785        1416 PRECALL                  0
               1420 CALL                     0
    
-   759        1430 STORE_NAME              38 (CallbackSelection)
+   786        1430 STORE_NAME              38 (CallbackSelection)
    
-   791        1432 PUSH_NULL
+   818        1432 PUSH_NULL
               1434 LOAD_BUILD_CLASS
-              1436 LOAD_CONST              53 (<code object MessageStatusType, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 791>)
+              1436 LOAD_CONST              53 (<code object MessageStatusType, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 818>)
               1438 MAKE_FUNCTION            0
               1440 LOAD_CONST              54 ('MessageStatusType')
               1442 LOAD_NAME                9 (Enum)
               1444 PRECALL                  3
               1448 CALL                     3
               1458 STORE_NAME              39 (MessageStatusType)
    
-   799        1460 PUSH_NULL
+   826        1460 PUSH_NULL
               1462 LOAD_NAME                5 (dataclass)
               1464 LOAD_CONST               9 (True)
               1466 LOAD_CONST               9 (True)
               1468 KW_NAMES                10
               1470 PRECALL                  2
               1474 CALL                     2
    
-   800        1484 PUSH_NULL
+   827        1484 PUSH_NULL
               1486 LOAD_BUILD_CLASS
-              1488 LOAD_CONST              55 (<code object MessageStatus, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 799>)
+              1488 LOAD_CONST              55 (<code object MessageStatus, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 826>)
               1490 MAKE_FUNCTION            0
               1492 LOAD_CONST              56 ('MessageStatus')
               1494 LOAD_NAME               35 (BaseUpdate)
               1496 PRECALL                  3
               1500 CALL                     3
    
-   799        1510 PRECALL                  0
+   826        1510 PRECALL                  0
               1514 CALL                     0
    
-   800        1524 STORE_NAME              40 (MessageStatus)
+   827        1524 STORE_NAME              40 (MessageStatus)
               1526 LOAD_CONST              57 (None)
               1528 RETURN_VALUE
    consts
       0
       ('annotations',)
       ('Message', 'Contact', 'MessageType', 'MessageStatus', 'MessageStatusType', 'CallbackButton', 'CallbackSelection', 'InlineButton', 'SectionRow', 'Section', 'SectionList')
       ('datetime',)
@@ -617,15 +617,15 @@
           28           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('InlineButton')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          30          12 LOAD_CONST               1 ('\n    Represents an inline button in a keyboard.\n\n    Attributes:\n        title: The title of the button.\n        callback_data: The payload to send when the user clicks on the button.\n    ')
+          30          12 LOAD_CONST               1 ('\n    Represents an inline button in a keyboard.\n\n    Attributes:\n        title: The title of the button (up to 20 characters).\n        callback_data: The payload to send when the user clicks on the button (up to 256 characters).\n    ')
                       14 STORE_NAME               3 (__doc__)
          
           37          16 LOAD_CONST               2 ('str')
                       18 LOAD_NAME                4 (__annotations__)
                       20 LOAD_CONST               3 ('title')
                       22 STORE_SUBSCR
          
@@ -638,15 +638,15 @@
                       38 LOAD_CONST               7 (<code object to_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 40>)
                       40 MAKE_FUNCTION            4 (annotations)
                       42 STORE_NAME               5 (to_dict)
                       44 LOAD_CONST               8 (None)
                       46 RETURN_VALUE
          consts
             'InlineButton'
-            '\n    Represents an inline button in a keyboard.\n\n    Attributes:\n        title: The title of the button.\n        callback_data: The payload to send when the user clicks on the button.\n    '
+            '\n    Represents an inline button in a keyboard.\n\n    Attributes:\n        title: The title of the button (up to 20 characters).\n        callback_data: The payload to send when the user clicks on the button (up to 256 characters).\n    '
             'str'
             'title'
             'callback_data'
             'return'
             'dict'
             code
                argcount  : 1
@@ -704,15 +704,15 @@
           44           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SectionRow')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          46          12 LOAD_CONST               1 ('\n    Represents a row in a section.\n\n    Attributes:\n        title: The title of the row.\n        callback_data: The payload to send when the user clicks on the row.\n        description: The description of the row (optional).\n    ')
+          46          12 LOAD_CONST               1 ('\n    Represents a row in a section.\n\n    Attributes:\n        title: The title of the row (up to 24 characters).\n        callback_data: The payload to send when the user clicks on the row (up to 200 characters).\n        description: The description of the row (optional, up to 72 characters).\n    ')
                       14 STORE_NAME               3 (__doc__)
          
           54          16 LOAD_CONST               2 ('str')
                       18 LOAD_NAME                4 (__annotations__)
                       20 LOAD_CONST               3 ('title')
                       22 STORE_SUBSCR
          
@@ -732,15 +732,15 @@
                       52 LOAD_CONST              10 (<code object to_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 58>)
                       54 MAKE_FUNCTION            4 (annotations)
                       56 STORE_NAME               6 (to_dict)
                       58 LOAD_CONST               5 (None)
                       60 RETURN_VALUE
          consts
             'SectionRow'
-            '\n    Represents a row in a section.\n\n    Attributes:\n        title: The title of the row.\n        callback_data: The payload to send when the user clicks on the row.\n        description: The description of the row (optional).\n    '
+            '\n    Represents a row in a section.\n\n    Attributes:\n        title: The title of the row (up to 24 characters).\n        callback_data: The payload to send when the user clicks on the row (up to 200 characters).\n        description: The description of the row (optional, up to 72 characters).\n    '
             'str'
             'title'
             'callback_data'
             None
             'str | None'
             'description'
             'return'
@@ -927,15 +927,15 @@
           86           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SectionList')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          88          12 LOAD_CONST               1 ('\n    Represents a section list in an interactive message.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/reference/messages#section-object\n\n    Attributes:\n        button_title: The title of the button that opens the section list.\n        sections: The sections in the section list (at least 1, no more than 10).\n    ')
+          88          12 LOAD_CONST               1 ('\n    Represents a section list in an interactive message.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/reference/messages#section-object\n\n    Attributes:\n        button_title: The title of the button that opens the section list (up to 20 characters).\n        sections: The sections in the section list (at least 1, no more than 10).\n    ')
                       14 STORE_NAME               3 (__doc__)
          
           97          16 LOAD_CONST               2 ('str')
                       18 LOAD_NAME                4 (__annotations__)
                       20 LOAD_CONST               3 ('button_title')
                       22 STORE_SUBSCR
          
@@ -948,15 +948,15 @@
                       38 LOAD_CONST               8 (<code object to_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 100>)
                       40 MAKE_FUNCTION            4 (annotations)
                       42 STORE_NAME               5 (to_dict)
                       44 LOAD_CONST               9 (None)
                       46 RETURN_VALUE
          consts
             'SectionList'
-            '\n    Represents a section list in an interactive message.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/reference/messages#section-object\n\n    Attributes:\n        button_title: The title of the button that opens the section list.\n        sections: The sections in the section list (at least 1, no more than 10).\n    '
+            '\n    Represents a section list in an interactive message.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/reference/messages#section-object\n\n    Attributes:\n        button_title: The title of the button that opens the section list (up to 20 characters).\n        sections: The sections in the section list (at least 1, no more than 10).\n    '
             'str'
             'button_title'
             'list[Section]'
             'sections'
             'return'
             'dict'
             code
@@ -3316,20 +3316,21 @@
          nlocals   : 0
          stacksize : 5
          flags     : 16777216
          code
             0x970065005a0164005a02550002006503640164016401ac02a6030000ab
             0300000000000000005a046403650564043c0000006405650564063c0000
             006407650564083c00000064096505640a3c000000640b6505640c3c0000
-            0065066436640e8404a6000000ab0000000000000000005a070900090009
-            000900090064376438641984055a08090009000900090009006439643a64
-            2084055a09090009000900090009006439643b642284055a0a0900090009
-            00090009000900643c643d642584055a0b0900643e643f642784055a0c09
-            00090064406441642a84055a0d0900090064426443643084055a0e090064
-            3e6444643384055a0f6445643584045a10640f5300
+            0065066438640e8404a6000000ab0000000000000000005a070900090009
+            00090009006439643a641984055a0809000900090009000900643b643c64
+            2084055a0909000900090009000900643b643d642284055a0a0900090009
+            00090009000900643e643f642584055a0b090064406441642784055a0c09
+            00090064426443642a84055a0d0900090064446445643084055a0e090064
+            406446643384055a0f6447643584045a106438643684045a116448643784
+            045a12640f5300
          408           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseUpdate')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -3365,15 +3366,15 @@
          414          80 LOAD_CONST              11 ('datetime')
                       82 LOAD_NAME                5 (__annotations__)
                       84 LOAD_CONST              12 ('timestamp')
                       86 STORE_SUBSCR
          
          416          90 LOAD_NAME                6 (property)
          
-         417          92 LOAD_CONST              54 (('return', 'str'))
+         417          92 LOAD_CONST              56 (('return', 'str'))
                       94 LOAD_CONST              14 (<code object sender, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 416>)
                       96 MAKE_FUNCTION            4 (annotations)
          
          416          98 PRECALL                  0
                      102 CALL                     0
          
          417         112 STORE_NAME               7 (sender)
@@ -3384,48 +3385,48 @@
          
          425         118 NOP
          
          426         120 NOP
          
          427         122 NOP
          
-         420         124 LOAD_CONST              55 ((False, False, None, None, None))
-                     126 LOAD_CONST              56 (('text', 'str', 'preview_url', 'bool', 'quote', 'bool', 'keyboard', 'list[InlineButton] | SectionList | None', 'header', 'str | None', 'footer', 'str | None', 'return', 'str'))
+         420         124 LOAD_CONST              57 ((False, False, None, None, None))
+                     126 LOAD_CONST              58 (('text', 'str', 'preview_url', 'bool', 'quote', 'bool', 'keyboard', 'list[InlineButton] | SectionList | None', 'header', 'str | None', 'footer', 'str | None', 'return', 'str'))
                      128 LOAD_CONST              25 (<code object reply_text, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 420>)
                      130 MAKE_FUNCTION            5 (defaults, annotations)
                      132 STORE_NAME               8 (reply_text)
          
          456         134 NOP
          
          457         136 NOP
          
          458         138 NOP
          
          459         140 NOP
          
          460         142 NOP
          
-         453         144 LOAD_CONST              57 ((None, False, None, None, None))
-                     146 LOAD_CONST              58 (('image', 'str | bytes', 'caption', 'str | None', 'quote', 'bool', 'buttons', 'list[InlineButton] | None', 'body', 'str | None', 'footer', 'str | None', 'return', 'str'))
+         453         144 LOAD_CONST              59 ((None, False, None, None, None))
+                     146 LOAD_CONST              60 (('image', 'str | bytes', 'caption', 'str | None', 'quote', 'bool', 'buttons', 'list[InlineButton] | None', 'body', 'str | None', 'footer', 'str | None', 'return', 'str'))
                      148 LOAD_CONST              32 (<code object reply_image, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 453>)
                      150 MAKE_FUNCTION            5 (defaults, annotations)
                      152 STORE_NAME               9 (reply_image)
          
          489         154 NOP
          
          490         156 NOP
          
          491         158 NOP
          
          492         160 NOP
          
          493         162 NOP
          
-         486         164 LOAD_CONST              57 ((None, False, None, None, None))
-                     166 LOAD_CONST              59 (('video', 'str | bytes', 'caption', 'str | None', 'quote', 'bool', 'buttons', 'list[InlineButton] | None', 'body', 'str | None', 'footer', 'str | None', 'return', 'str'))
+         486         164 LOAD_CONST              59 ((None, False, None, None, None))
+                     166 LOAD_CONST              61 (('video', 'str | bytes', 'caption', 'str | None', 'quote', 'bool', 'buttons', 'list[InlineButton] | None', 'body', 'str | None', 'footer', 'str | None', 'return', 'str'))
                      168 LOAD_CONST              34 (<code object reply_video, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 486>)
                      170 MAKE_FUNCTION            5 (defaults, annotations)
                      172 STORE_NAME              10 (reply_video)
          
          522         174 NOP
          
          523         176 NOP
@@ -3434,62 +3435,72 @@
          
          525         180 NOP
          
          526         182 NOP
          
          527         184 NOP
          
-         519         186 LOAD_CONST              60 ((None, None, False, None, None, None))
-                     188 LOAD_CONST              61 (('document', 'str | bytes', 'filename', 'str | None', 'caption', 'str | None', 'quote', 'bool', 'buttons', 'list[InlineButton] | None', 'body', 'str | None', 'footer', 'str | None', 'return', 'str'))
+         519         186 LOAD_CONST              62 ((None, None, False, None, None, None))
+                     188 LOAD_CONST              63 (('document', 'str | bytes', 'filename', 'str | None', 'caption', 'str | None', 'quote', 'bool', 'buttons', 'list[InlineButton] | None', 'body', 'str | None', 'footer', 'str | None', 'return', 'str'))
                      190 LOAD_CONST              37 (<code object reply_document, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 519>)
                      192 MAKE_FUNCTION            5 (defaults, annotations)
                      194 STORE_NAME              11 (reply_document)
          
          558         196 NOP
          
-         555         198 LOAD_CONST              62 ((False,))
-                     200 LOAD_CONST              63 (('audio', 'str | bytes', 'quote', 'bool', 'return', 'str'))
+         555         198 LOAD_CONST              64 ((False,))
+                     200 LOAD_CONST              65 (('audio', 'str | bytes', 'quote', 'bool', 'return', 'str'))
                      202 LOAD_CONST              39 (<code object reply_audio, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 555>)
                      204 MAKE_FUNCTION            5 (defaults, annotations)
                      206 STORE_NAME              12 (reply_audio)
          
          579         208 NOP
          
          580         210 NOP
          
-         576         212 LOAD_CONST              64 ((False, False))
-                     214 LOAD_CONST              65 (('sticker', 'str | bytes', 'animated', 'bool', 'quote', 'bool', 'return', 'str'))
+         576         212 LOAD_CONST              66 ((False, False))
+                     214 LOAD_CONST              67 (('sticker', 'str | bytes', 'animated', 'bool', 'quote', 'bool', 'return', 'str'))
                      216 LOAD_CONST              42 (<code object reply_sticker, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 576>)
                      218 MAKE_FUNCTION            5 (defaults, annotations)
                      220 STORE_NAME              13 (reply_sticker)
          
          604         222 NOP
          
          605         224 NOP
          
-         600         226 LOAD_CONST              66 ((None, None))
-                     228 LOAD_CONST              67 (('latitude', 'float', 'longitude', 'float', 'name', 'str | None', 'address', 'str | None', 'return', 'str'))
+         600         226 LOAD_CONST              68 ((None, None))
+                     228 LOAD_CONST              69 (('latitude', 'float', 'longitude', 'float', 'name', 'str | None', 'address', 'str | None', 'return', 'str'))
                      230 LOAD_CONST              48 (<code object reply_location, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 600>)
                      232 MAKE_FUNCTION            5 (defaults, annotations)
                      234 STORE_NAME              14 (reply_location)
          
          630         236 NOP
          
-         627         238 LOAD_CONST              62 ((False,))
-                     240 LOAD_CONST              68 (('contact', 'Contact | Iterable[Contact]', 'quote', 'bool', 'return', 'str'))
+         627         238 LOAD_CONST              64 ((False,))
+                     240 LOAD_CONST              70 (('contact', 'Contact | Iterable[Contact]', 'quote', 'bool', 'return', 'str'))
                      242 LOAD_CONST              51 (<code object reply_contact, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 627>)
                      244 MAKE_FUNCTION            5 (defaults, annotations)
                      246 STORE_NAME              15 (reply_contact)
          
-         648         248 LOAD_CONST              69 (('emoji', 'str', 'return', 'str'))
+         648         248 LOAD_CONST              71 (('emoji', 'str', 'return', 'str'))
                      250 LOAD_CONST              53 (<code object react, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 648>)
                      252 MAKE_FUNCTION            4 (annotations)
                      254 STORE_NAME              16 (react)
-                     256 LOAD_CONST              15 (None)
-                     258 RETURN_VALUE
+         
+         667         256 LOAD_CONST              56 (('return', 'str'))
+                     258 LOAD_CONST              54 (<code object unreact, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 667>)
+                     260 MAKE_FUNCTION            4 (annotations)
+                     262 STORE_NAME              17 (unreact)
+         
+         681         264 LOAD_CONST              72 (('return', 'bool'))
+                     266 LOAD_CONST              55 (<code object mark_as_read, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 681>)
+                     268 MAKE_FUNCTION            4 (annotations)
+                     270 STORE_NAME              18 (mark_as_read)
+                     272 LOAD_CONST              15 (None)
+                     274 RETURN_VALUE
          consts
             'BaseUpdate'
             False
             ('repr', 'hash', 'compare')
             'WhatsApp'
             '_client'
             'str'
@@ -3570,15 +3581,15 @@
                450          76 LOAD_FAST                6 (footer)
                
                443          78 KW_NAMES                 2
                             80 PRECALL                  7
                             84 CALL                     7
                             94 RETURN_VALUE
                consts
-                  '\n        Reply to the message with text.\n\n        Args:\n            text: The text to reply with.\n            preview_url: Whether to show a preview of the URL in the text (default: False).\n            quote: Whether to quote the message (default: False).\n            keyboard: The keyboard to send with the message (optional).\n            header: The header of the message (if keyboard is provided, optional).\n            footer: The footer of the message (if keyboard is provided, optional).\n\n        Returns:\n            The ID of the sent message.\n        '
+                  '\n        Reply to the message with text.\n\n        Args:\n            text: The text to reply with.\n            preview_url: Whether to show a preview of the URL in the text (default: False).\n            quote: Whether to quote the message (default: False).\n            keyboard: The keyboard to send with the message (optional).\n            header: The header of the message (if keyboard is provided, optional, up to 60 characters, no markdown allowed).\n            footer: The footer of the message (if keyboard is provided, optional, up to 60 characters, markdown has no effect).\n\n        Returns:\n            The ID of the sent message.\n        '
                   None
                   ('to', 'text', 'preview_url', 'reply_to_message_id', 'keyboard', 'header', 'footer')
                names      ('_client', 'send_message', 'sender', 'id')
                varnames   ('self', 'text', 'preview_url', 'quote', 'keyboard', 'header', 'footer')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
@@ -3628,15 +3639,15 @@
                483          76 LOAD_FAST                6 (footer)
                
                476          78 KW_NAMES                 2
                             80 PRECALL                  7
                             84 CALL                     7
                             94 RETURN_VALUE
                consts
-                  '\n        Reply to the message with an image.\n\n        Args:\n            image: The image to reply with.\n            caption: The caption of the image (optional).\n            quote: Whether to quote the message (default: False).\n            buttons: The buttons to send with the message (optional).\n            body: The body of the message (if buttons is provided, optional).\n            footer: The footer of the message (if buttons is provided, optional).\n\n        Returns:\n            The ID of the sent message.\n        '
+                  '\n        Reply to the message with an image.\n\n        Args:\n            image: The image to reply with.\n            caption: The caption of the image (optional).\n            quote: Whether to quote the message (default: False).\n            buttons: The buttons to send with the message (optional).\n            body: The body of the message (if buttons is provided, optional).\n            footer: The footer of the message (if buttons is provided, optional, up to 60 characters, markdown has no effect).\n\n        Returns:\n            The ID of the sent message.\n        '
                   None
                   ('to', 'image', 'caption', 'reply_to_message_id', 'buttons', 'body', 'footer')
                names      ('_client', 'send_image', 'sender', 'id')
                varnames   ('self', 'image', 'caption', 'quote', 'buttons', 'body', 'footer')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
@@ -3681,15 +3692,15 @@
                516          76 LOAD_FAST                6 (footer)
                
                509          78 KW_NAMES                 2
                             80 PRECALL                  7
                             84 CALL                     7
                             94 RETURN_VALUE
                consts
-                  '\n        Reply to the message with a video.\n\n        Args:\n            video: The video to reply with.\n            caption: The caption of the video (optional).\n            quote: Whether to quote the message (default: False).\n            buttons: The buttons to send with the message (optional).\n            body: The body of the message (if buttons is provided, optional).\n            footer: The footer of the message (if buttons is provided, optional).\n\n        Returns:\n            The ID of the sent message.\n        '
+                  '\n        Reply to the message with a video.\n\n        Args:\n            video: The video to reply with.\n            caption: The caption of the video (optional).\n            quote: Whether to quote the message (default: False).\n            buttons: The buttons to send with the message (optional).\n            body: The body of the message (if buttons is provided, optional).\n            footer: The footer of the message (if buttons is provided, optional, up to 60 characters, markdown has no effect).\n\n        Returns:\n            The ID of the sent message.\n        '
                   None
                   ('to', 'video', 'caption', 'reply_to_message_id', 'buttons', 'body', 'footer')
                names      ('_client', 'send_video', 'sender', 'id')
                varnames   ('self', 'video', 'caption', 'quote', 'buttons', 'body', 'footer')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
@@ -3737,15 +3748,15 @@
                552          78 LOAD_FAST                7 (footer)
                
                544          80 KW_NAMES                 2
                             82 PRECALL                  8
                             86 CALL                     8
                             96 RETURN_VALUE
                consts
-                  '\n        Reply to the message with a document.\n\n        Args:\n            document: The document to reply with.\n            filename: The filename of the document (optional).\n            caption: The caption of the document (optional).\n            quote: Whether to quote the message (default: False).\n            buttons: The buttons to send with the message (optional).\n            body: The body of the message (if buttons is provided, optional).\n            footer: The footer of the message (if buttons is provided, optional).\n\n        Returns:\n            The ID of the sent message.\n        '
+                  '\n        Reply to the message with a document.\n\n        Args:\n            document: The document to reply with.\n            filename: The filename of the document (optional, The extension of the filename will specify what format the document is displayed as in WhatsApp).\n            caption: The caption of the document (optional).\n            quote: Whether to quote the message (default: False).\n            buttons: The buttons to send with the message (optional).\n            body: The body of the message (if buttons is provided, optional).\n            footer: The footer of the message (if buttons is provided, optional, up to 60 characters, markdown has no effect).\n\n        Returns:\n            The ID of the sent message.\n        '
                   None
                   ('to', 'document', 'filename', 'caption', 'reply_to_message_id', 'buttons', 'body', 'footer')
                names      ('_client', 'send_document', 'sender', 'id')
                varnames   ('self', 'document', 'filename', 'caption', 'quote', 'buttons', 'body', 'footer')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
@@ -3970,14 +3981,83 @@
                varnames   ('self', 'emoji')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
                name       'react'
                firstlineno 648
                lnotab 0x020d22010c0102010cfd
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 4
+               flags     : 16777219
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000007c006a0200000000000000007c006a0300000000000000
+                  00ac01a6020000ab0200000000000000005300
+               667           0 RESUME                   0
+               
+               676           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (_client)
+                            14 LOAD_METHOD              1 (remove_reaction)
+               
+               677          36 LOAD_FAST                0 (self)
+                            38 LOAD_ATTR                2 (sender)
+               
+               678          48 LOAD_FAST                0 (self)
+                            50 LOAD_ATTR                3 (id)
+               
+               676          60 KW_NAMES                 1
+                            62 PRECALL                  2
+                            66 CALL                     2
+                            76 RETURN_VALUE
+               consts
+                  '\n        Remove the reaction from the message.\n\n        Returns:\n            The ID of the sent message.\n        '
+                  ('to', 'message_id')
+               names      ('_client', 'remove_reaction', 'sender', 'id')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
+               name       'unreact'
+               firstlineno 667
+               lnotab 0x020922010c010cfe
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 16777219
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000007c006a020000000000000000ac01a6010000ab01000000
+                  00000000005300
+               681           0 RESUME                   0
+               
+               690           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (_client)
+                            14 LOAD_METHOD              1 (mark_message_as_read)
+               
+               691          36 LOAD_FAST                0 (self)
+                            38 LOAD_ATTR                2 (id)
+               
+               690          48 KW_NAMES                 1
+                            50 PRECALL                  1
+                            54 CALL                     1
+                            64 RETURN_VALUE
+               consts
+                  '\n        Mark the message as read.\n\n        Returns:\n            Whether it was successful.\n        '
+                  ('message_id',)
+               names      ('_client', 'mark_message_as_read', 'id')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
+               name       'mark_as_read'
+               firstlineno 681
+               lnotab 0x020922010cff
             ('return', 'str')
             (False, False, None, None, None)
             ('text', 'str', 'preview_url', 'bool', 'quote', 'bool', 'keyboard', 'list[InlineButton] | SectionList | None', 'header', 'str | None', 'footer', 'str | None', 'return', 'str')
             (None, False, None, None, None)
             ('image', 'str | bytes', 'caption', 'str | None', 'quote', 'bool', 'buttons', 'list[InlineButton] | None', 'body', 'str | None', 'footer', 'str | None', 'return', 'str')
             ('video', 'str | bytes', 'caption', 'str | None', 'quote', 'bool', 'buttons', 'list[InlineButton] | None', 'body', 'str | None', 'footer', 'str | None', 'return', 'str')
             (None, None, False, None, None, None)
@@ -3986,114 +4066,115 @@
             ('audio', 'str | bytes', 'quote', 'bool', 'return', 'str')
             (False, False)
             ('sticker', 'str | bytes', 'animated', 'bool', 'quote', 'bool', 'return', 'str')
             (None, None)
             ('latitude', 'float', 'longitude', 'float', 'name', 'str | None', 'address', 'str | None', 'return', 'str')
             ('contact', 'Contact | Iterable[Contact]', 'quote', 'bool', 'return', 'str')
             ('emoji', 'str', 'return', 'str')
-         names      ('__name__', '__module__', '__qualname__', 'field', '_client', '__annotations__', 'property', 'sender', 'reply_text', 'reply_image', 'reply_video', 'reply_document', 'reply_audio', 'reply_sticker', 'reply_location', 'reply_contact', 'react')
+            ('return', 'bool')
+         names      ('__name__', '__module__', '__qualname__', 'field', '_client', '__annotations__', 'property', 'sender', 'reply_text', 'reply_image', 'reply_video', 'reply_document', 'reply_audio', 'reply_sticker', 'reply_location', 'reply_contact', 'react', 'unreact', 'mark_as_read')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
          name       'BaseUpdate'
          firstlineno 408
          lnotab
             0x0c0226010a010a010a010a02020106ff0e010206020102010201020102
             f90a24020102010201020102f90a24020102010201020102f90a24020102
             0102010201020102f80a2702fd0a18020102fc0a1c020102fb0a1e02fd0a
-            15
+            150813080e
       'BaseUpdate'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a036402650464033c000000640465
             0464053c0000006406650464073c0000006408650464093c000000640a65
             04640b3c000000640c6504640d3c000000640e6504640f3c000000641065
             0464113c0000006412650464133c0000006414650464153c000000641665
             0464173c0000006505641e641c8404a6000000ab0000000000000000005a
             06641d5300
-         668           0 RESUME                   0
+         695           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Message')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         670          12 LOAD_CONST               1 ('\n    A message received from a user.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#messages-object\n\n    Attributes:\n        id: The message ID.\n        metadata: The metadata of the message (to which phone number it was sent).\n        type: The message type (text, image, video, etc).\n        from_user: The user who sent the message.\n        timestamp: The timestamp when the message was sent.\n        reply_to_message: The message to which this message is a reply to. (optional)\n        text: The text of the message (if the message type is text). (optional)\n        image: The image of the message (if the message type is image). (optional)\n        video: The video of the message (if the message type is video). (optional)\n        sticker: The sticker of the message (if the message type is sticker). (optional)\n        document: The document of the message (if the message type is document). (optional)\n        audio: The audio of the message (if the message type is audio). (optional)\n        reaction: The reaction of the message (if the message type is reaction). (optional)\n        location: The location of the message (if the message type is location). (optional)\n        contacts: The contacts of the message (if the message type is contacts). (optional)\n    ')
+         697          12 LOAD_CONST               1 ('\n    A message received from a user.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#messages-object\n\n    Attributes:\n        id: The message ID.\n        metadata: The metadata of the message (to which phone number it was sent).\n        type: The message type (text, image, video, etc).\n        from_user: The user who sent the message.\n        timestamp: The timestamp when the message was sent.\n        reply_to_message: The message to which this message is a reply to. (optional)\n        text: The text of the message (if the message type is text). (optional)\n        image: The image of the message (if the message type is image). (optional)\n        video: The video of the message (if the message type is video). (optional)\n        sticker: The sticker of the message (if the message type is sticker). (optional)\n        document: The document of the message (if the message type is document). (optional)\n        audio: The audio of the message (if the message type is audio). (optional)\n        reaction: The reaction of the message (if the message type is reaction). (optional)\n        location: The location of the message (if the message type is location). (optional)\n        contacts: The contacts of the message (if the message type is contacts). (optional)\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         692          16 LOAD_CONST               2 ('MessageType')
+         719          16 LOAD_CONST               2 ('MessageType')
                       18 LOAD_NAME                4 (__annotations__)
                       20 LOAD_CONST               3 ('type')
                       22 STORE_SUBSCR
          
-         693          26 LOAD_CONST               4 ('ReplyToMessage | None')
+         720          26 LOAD_CONST               4 ('ReplyToMessage | None')
                       28 LOAD_NAME                4 (__annotations__)
                       30 LOAD_CONST               5 ('reply_to_message')
                       32 STORE_SUBSCR
          
-         694          36 LOAD_CONST               6 ('str | None')
+         721          36 LOAD_CONST               6 ('str | None')
                       38 LOAD_NAME                4 (__annotations__)
                       40 LOAD_CONST               7 ('text')
                       42 STORE_SUBSCR
          
-         695          46 LOAD_CONST               8 ('Image | None')
+         722          46 LOAD_CONST               8 ('Image | None')
                       48 LOAD_NAME                4 (__annotations__)
                       50 LOAD_CONST               9 ('image')
                       52 STORE_SUBSCR
          
-         696          56 LOAD_CONST              10 ('Video | None')
+         723          56 LOAD_CONST              10 ('Video | None')
                       58 LOAD_NAME                4 (__annotations__)
                       60 LOAD_CONST              11 ('video')
                       62 STORE_SUBSCR
          
-         697          66 LOAD_CONST              12 ('Sticker | None')
+         724          66 LOAD_CONST              12 ('Sticker | None')
                       68 LOAD_NAME                4 (__annotations__)
                       70 LOAD_CONST              13 ('sticker')
                       72 STORE_SUBSCR
          
-         698          76 LOAD_CONST              14 ('Document | None')
+         725          76 LOAD_CONST              14 ('Document | None')
                       78 LOAD_NAME                4 (__annotations__)
                       80 LOAD_CONST              15 ('document')
                       82 STORE_SUBSCR
          
-         699          86 LOAD_CONST              16 ('Audio | None')
+         726          86 LOAD_CONST              16 ('Audio | None')
                       88 LOAD_NAME                4 (__annotations__)
                       90 LOAD_CONST              17 ('audio')
                       92 STORE_SUBSCR
          
-         700          96 LOAD_CONST              18 ('Reaction | None')
+         727          96 LOAD_CONST              18 ('Reaction | None')
                       98 LOAD_NAME                4 (__annotations__)
                      100 LOAD_CONST              19 ('reaction')
                      102 STORE_SUBSCR
          
-         701         106 LOAD_CONST              20 ('Location | None')
+         728         106 LOAD_CONST              20 ('Location | None')
                      108 LOAD_NAME                4 (__annotations__)
                      110 LOAD_CONST              21 ('location')
                      112 STORE_SUBSCR
          
-         702         116 LOAD_CONST              22 ('list[Contact] | None')
+         729         116 LOAD_CONST              22 ('list[Contact] | None')
                      118 LOAD_NAME                4 (__annotations__)
                      120 LOAD_CONST              23 ('contacts')
                      122 STORE_SUBSCR
          
-         704         126 LOAD_NAME                5 (classmethod)
+         731         126 LOAD_NAME                5 (classmethod)
          
-         705         128 LOAD_CONST              30 (('client', 'WhatsApp', 'value', 'dict'))
-                     130 LOAD_CONST              28 (<code object from_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 704>)
+         732         128 LOAD_CONST              30 (('client', 'WhatsApp', 'value', 'dict'))
+                     130 LOAD_CONST              28 (<code object from_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 731>)
                      132 MAKE_FUNCTION            4 (annotations)
          
-         704         134 PRECALL                  0
+         731         134 PRECALL                  0
                      138 CALL                     0
          
-         705         148 STORE_NAME               6 (from_dict)
+         732         148 STORE_NAME               6 (from_dict)
                      150 LOAD_CONST              29 (None)
                      152 RETURN_VALUE
          consts
             'Message'
             '\n    A message received from a user.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#messages-object\n\n    Attributes:\n        id: The message ID.\n        metadata: The metadata of the message (to which phone number it was sent).\n        type: The message type (text, image, video, etc).\n        from_user: The user who sent the message.\n        timestamp: The timestamp when the message was sent.\n        reply_to_message: The message to which this message is a reply to. (optional)\n        text: The text of the message (if the message type is text). (optional)\n        image: The image of the message (if the message type is image). (optional)\n        video: The video of the message (if the message type is video). (optional)\n        sticker: The sticker of the message (if the message type is sticker). (optional)\n        document: The document of the message (if the message type is document). (optional)\n        audio: The audio of the message (if the message type is audio). (optional)\n        reaction: The reaction of the message (if the message type is reaction). (optional)\n        location: The location of the message (if the message type is location). (optional)\n        contacts: The contacts of the message (if the message type is contacts). (optional)\n    '
             'MessageType'
             'type'
@@ -4162,228 +4243,228 @@
                   006413a6010000ab010000000000000000a6010000ab0100000000000000
                   0093016414741e00000000000000000000a0020000000000000000000000
                   0000000000000000007c03a0080000000000000000000000000000000000
                   0000006414a6010000ab010000000000000000a6010000ab010000000000
                   00000093016407641584007c03a008000000000000000000000000000000
                   000000000064076700a6020000ab0200000000000000004400a6000000ab
                   0000000000000000007001640093018e015300
-               704           0 RESUME                   0
+               731           0 RESUME                   0
                
-               706           2 LOAD_FAST                2 (value)
+               733           2 LOAD_FAST                2 (value)
                              4 LOAD_CONST               1 ('messages')
                              6 BINARY_SUBSCR
                             16 LOAD_CONST               2 (0)
                             18 BINARY_SUBSCR
                             28 STORE_FAST               3 (message)
                
-               707          30 LOAD_GLOBAL              1 (NULL + MessageType)
+               734          30 LOAD_GLOBAL              1 (NULL + MessageType)
                             42 LOAD_FAST                3 (message)
                             44 LOAD_CONST               3 ('type')
                             46 BINARY_SUBSCR
                             56 PRECALL                  1
                             60 CALL                     1
                             70 STORE_FAST               4 (msg_type)
                
-               708          72 PUSH_NULL
+               735          72 PUSH_NULL
                             74 LOAD_FAST                0 (cls)
                             76 LOAD_CONST              22 (())
                             78 BUILD_MAP                0
                             80 LOAD_CONST               4 ('_client')
                
-               709          82 LOAD_FAST                1 (client)
+               736          82 LOAD_FAST                1 (client)
                             84 MAP_ADD                  1
                
-               708          86 LOAD_CONST               5 ('id')
+               735          86 LOAD_CONST               5 ('id')
                
-               710          88 LOAD_FAST                3 (message)
+               737          88 LOAD_FAST                3 (message)
                             90 LOAD_CONST               5 ('id')
                             92 BINARY_SUBSCR
                            102 MAP_ADD                  1
                
-               708         104 LOAD_CONST               3 ('type')
+               735         104 LOAD_CONST               3 ('type')
                
-               711         106 LOAD_FAST                4 (msg_type)
+               738         106 LOAD_FAST                4 (msg_type)
                            108 MAP_ADD                  1
                
-               708         110 LOAD_CONST               6 ('from_user')
+               735         110 LOAD_CONST               6 ('from_user')
                
-               712         112 LOAD_GLOBAL              2 (User)
+               739         112 LOAD_GLOBAL              2 (User)
                            124 LOAD_METHOD              2 (from_dict)
                            146 LOAD_FAST                2 (value)
                            148 LOAD_CONST               7 ('contacts')
                            150 BINARY_SUBSCR
                            160 LOAD_CONST               2 (0)
                            162 BINARY_SUBSCR
                            172 PRECALL                  1
                            176 CALL                     1
                            186 MAP_ADD                  1
                
-               708         188 LOAD_CONST               8 ('timestamp')
+               735         188 LOAD_CONST               8 ('timestamp')
                
-               713         190 LOAD_GLOBAL              7 (NULL + datetime)
+               740         190 LOAD_GLOBAL              7 (NULL + datetime)
                            202 LOAD_ATTR                4 (fromtimestamp)
                            212 LOAD_GLOBAL             11 (NULL + int)
                            224 LOAD_FAST                3 (message)
                            226 LOAD_CONST               8 ('timestamp')
                            228 BINARY_SUBSCR
                            238 PRECALL                  1
                            242 CALL                     1
                            252 PRECALL                  1
                            256 CALL                     1
                            266 MAP_ADD                  1
                
-               708         268 LOAD_CONST               9 ('metadata')
+               735         268 LOAD_CONST               9 ('metadata')
                
-               714         270 LOAD_GLOBAL             13 (NULL + Metadata)
+               741         270 LOAD_GLOBAL             13 (NULL + Metadata)
                            282 LOAD_CONST              22 (())
                            284 BUILD_MAP                0
                            286 LOAD_FAST                2 (value)
                            288 LOAD_CONST               9 ('metadata')
                            290 BINARY_SUBSCR
                            300 DICT_MERGE               1
                            302 CALL_FUNCTION_EX         1
                            304 MAP_ADD                  1
                
-               708         306 LOAD_CONST              10 ('reply_to_message')
+               735         306 LOAD_CONST              10 ('reply_to_message')
                
-               715         308 LOAD_GLOBAL             14 (ReplyToMessage)
+               742         308 LOAD_GLOBAL             14 (ReplyToMessage)
                            320 LOAD_METHOD              2 (from_dict)
                            342 LOAD_FAST                3 (message)
                            344 LOAD_METHOD              8 (get)
                            366 LOAD_CONST              11 ('context')
                            368 PRECALL                  1
                            372 CALL                     1
                            382 PRECALL                  1
                            386 CALL                     1
                            396 MAP_ADD                  1
                
-               708         398 LOAD_CONST              12 ('text')
+               735         398 LOAD_CONST              12 ('text')
                
-               716         400 LOAD_CONST              12 ('text')
+               743         400 LOAD_CONST              12 ('text')
                            402 LOAD_FAST                3 (message)
                            404 CONTAINS_OP              0
                            406 POP_JUMP_FORWARD_IF_FALSE    14 (to 436)
                            408 LOAD_FAST                3 (message)
                            410 LOAD_CONST              12 ('text')
                            412 BINARY_SUBSCR
                            422 LOAD_CONST              13 ('body')
                            424 BINARY_SUBSCR
                            434 JUMP_FORWARD             1 (to 438)
                        >>  436 LOAD_CONST               0 (None)
                        >>  438 MAP_ADD                  1
                
-               708         440 LOAD_CONST              14 ('image')
+               735         440 LOAD_CONST              14 ('image')
                
-               717         442 LOAD_GLOBAL             18 (Image)
+               744         442 LOAD_GLOBAL             18 (Image)
                            454 LOAD_METHOD              2 (from_dict)
                            476 LOAD_FAST                3 (message)
                            478 LOAD_METHOD              8 (get)
                            500 LOAD_CONST              14 ('image')
                            502 PRECALL                  1
                            506 CALL                     1
                            516 PRECALL                  1
                            520 CALL                     1
                            530 MAP_ADD                  1
                
-               708         532 LOAD_CONST              15 ('video')
+               735         532 LOAD_CONST              15 ('video')
                
-               718         534 LOAD_GLOBAL             20 (Video)
+               745         534 LOAD_GLOBAL             20 (Video)
                            546 LOAD_METHOD              2 (from_dict)
                            568 LOAD_FAST                3 (message)
                            570 LOAD_METHOD              8 (get)
                            592 LOAD_CONST              15 ('video')
                            594 PRECALL                  1
                            598 CALL                     1
                            608 PRECALL                  1
                            612 CALL                     1
                            622 MAP_ADD                  1
                
-               708         624 LOAD_CONST              16 ('sticker')
+               735         624 LOAD_CONST              16 ('sticker')
                
-               719         626 LOAD_GLOBAL             22 (Sticker)
+               746         626 LOAD_GLOBAL             22 (Sticker)
                            638 LOAD_METHOD              2 (from_dict)
                            660 LOAD_FAST                3 (message)
                            662 LOAD_METHOD              8 (get)
                            684 LOAD_CONST              16 ('sticker')
                            686 PRECALL                  1
                            690 CALL                     1
                            700 PRECALL                  1
                            704 CALL                     1
                            714 MAP_ADD                  1
                
-               708         716 LOAD_CONST              17 ('document')
+               735         716 LOAD_CONST              17 ('document')
                
-               720         718 LOAD_GLOBAL             24 (Document)
+               747         718 LOAD_GLOBAL             24 (Document)
                            730 LOAD_METHOD              2 (from_dict)
                            752 LOAD_FAST                3 (message)
                            754 LOAD_METHOD              8 (get)
                            776 LOAD_CONST              17 ('document')
                            778 PRECALL                  1
                            782 CALL                     1
                            792 PRECALL                  1
                            796 CALL                     1
                            806 MAP_ADD                  1
                
-               708         808 LOAD_CONST              18 ('audio')
+               735         808 LOAD_CONST              18 ('audio')
                
-               721         810 LOAD_GLOBAL             26 (Audio)
+               748         810 LOAD_GLOBAL             26 (Audio)
                            822 LOAD_METHOD              2 (from_dict)
                            844 LOAD_FAST                3 (message)
                            846 LOAD_METHOD              8 (get)
                            868 LOAD_CONST              18 ('audio')
                            870 PRECALL                  1
                            874 CALL                     1
                            884 PRECALL                  1
                            888 CALL                     1
                            898 MAP_ADD                  1
                
-               708         900 LOAD_CONST              19 ('reaction')
+               735         900 LOAD_CONST              19 ('reaction')
                
-               722         902 LOAD_GLOBAL             28 (Reaction)
+               749         902 LOAD_GLOBAL             28 (Reaction)
                            914 LOAD_METHOD              2 (from_dict)
                            936 LOAD_FAST                3 (message)
                            938 LOAD_METHOD              8 (get)
                            960 LOAD_CONST              19 ('reaction')
                            962 PRECALL                  1
                            966 CALL                     1
                            976 PRECALL                  1
                            980 CALL                     1
                            990 MAP_ADD                  1
                
-               708         992 LOAD_CONST              20 ('location')
+               735         992 LOAD_CONST              20 ('location')
                
-               723         994 LOAD_GLOBAL             30 (Location)
+               750         994 LOAD_GLOBAL             30 (Location)
                           1006 LOAD_METHOD              2 (from_dict)
                           1028 LOAD_FAST                3 (message)
                           1030 LOAD_METHOD              8 (get)
                           1052 LOAD_CONST              20 ('location')
                           1054 PRECALL                  1
                           1058 CALL                     1
                           1068 PRECALL                  1
                           1072 CALL                     1
                           1082 MAP_ADD                  1
                
-               708        1084 LOAD_CONST               7 ('contacts')
+               735        1084 LOAD_CONST               7 ('contacts')
                
-               724        1086 LOAD_CONST              21 (<code object <listcomp>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 724>)
+               751        1086 LOAD_CONST              21 (<code object <listcomp>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 751>)
                           1088 MAKE_FUNCTION            0
                           1090 LOAD_FAST                3 (message)
                           1092 LOAD_METHOD              8 (get)
                           1114 LOAD_CONST               7 ('contacts')
                           1116 BUILD_LIST               0
                           1118 PRECALL                  2
                           1122 CALL                     2
                           1132 GET_ITER
                           1134 PRECALL                  0
                           1138 CALL                     0
                           1148 JUMP_IF_TRUE_OR_POP      1 (to 1152)
                           1150 LOAD_CONST               0 (None)
                        >> 1152 MAP_ADD                  1
                
-               708        1154 CALL_FUNCTION_EX         1
+               735        1154 CALL_FUNCTION_EX         1
                           1156 RETURN_VALUE
                consts
                   None
                   'messages'
                   0
                   'type'
                   '_client'
@@ -4408,15 +4489,15 @@
                      nlocals   : 2
                      stacksize : 5
                      flags     : 16777235
                      code
                         0x970067007c005d1c7d01740000000000000000000000a0010000000000
                         0000000000000000000000000000007c01a6010000ab0100000000000000
                         0091028c1d5300
-                     724           0 RESUME                   0
+                     751           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                28 (to 64)
                                    8 STORE_FAST               1 (contact)
                                   10 LOAD_GLOBAL              0 (Contact)
                                   22 LOAD_METHOD              1 (from_dict)
                                   44 LOAD_FAST                1 (contact)
@@ -4428,80 +4509,80 @@
                      consts
                      names      ('Contact', 'from_dict')
                      varnames   ('.0', 'contact')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
                      name       '<listcomp>'
-                     firstlineno 724
+                     firstlineno 751
                      lnotab 0x
                   ()
                names      ('MessageType', 'User', 'from_dict', 'datetime', 'fromtimestamp', 'int', 'Metadata', 'ReplyToMessage', 'get', 'Image', 'Video', 'Sticker', 'Document', 'Audio', 'Reaction', 'Location')
                varnames   ('cls', 'client', 'value', 'message', 'msg_type')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
                name       'from_dict'
-               firstlineno 704
+               firstlineno 731
                lnotab
                   0x02021c012a010a0104ff020210fe020304fd02044cfc02054efb020624
                   fa02075af9020828f802095af7020a5af6020b5af5020c5af4020d5af302
                   0e5af2020f5af1021044f0
             None
             ('client', 'WhatsApp', 'value', 'dict')
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__annotations__', 'classmethod', 'from_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
          name       'Message'
-         firstlineno 668
+         firstlineno 695
          lnotab
             0x0c0204160a010a010a010a010a010a010a010a010a010a010a02020106
             ff0e01
       'Message'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a036402650464033c000000640265
             0464043c0000006505640b64098404a6000000ab0000000000000000005a
             06640a5300
-         728           0 RESUME                   0
+         755           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CallbackButton')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         730          12 LOAD_CONST               1 ('\n    Represents a callback button.\n\n    Attributes:\n        id: The ID of the message.\n        metadata: The metadata of the message (to which phone number it was sent).\n        from_user: The user who sent the message.\n        timestamp: The timestamp when the message was sent.\n        data: The data of the button.\n        title: The title of the button.\n    ')
+         757          12 LOAD_CONST               1 ('\n    Represents a callback button.\n\n    Attributes:\n        id: The ID of the message.\n        metadata: The metadata of the message (to which phone number it was sent).\n        from_user: The user who sent the message.\n        timestamp: The timestamp when the message was sent.\n        data: The data of the button.\n        title: The title of the button.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         741          16 LOAD_CONST               2 ('str')
+         768          16 LOAD_CONST               2 ('str')
                       18 LOAD_NAME                4 (__annotations__)
                       20 LOAD_CONST               3 ('data')
                       22 STORE_SUBSCR
          
-         742          26 LOAD_CONST               2 ('str')
+         769          26 LOAD_CONST               2 ('str')
                       28 LOAD_NAME                4 (__annotations__)
                       30 LOAD_CONST               4 ('title')
                       32 STORE_SUBSCR
          
-         744          36 LOAD_NAME                5 (classmethod)
+         771          36 LOAD_NAME                5 (classmethod)
          
-         745          38 LOAD_CONST              11 (('client', 'WhatsApp', 'value', 'dict'))
-                      40 LOAD_CONST               9 (<code object from_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 744>)
+         772          38 LOAD_CONST              11 (('client', 'WhatsApp', 'value', 'dict'))
+                      40 LOAD_CONST               9 (<code object from_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 771>)
                       42 MAKE_FUNCTION            4 (annotations)
          
-         744          44 PRECALL                  0
+         771          44 PRECALL                  0
                       48 CALL                     0
          
-         745          58 STORE_NAME               6 (from_dict)
+         772          58 STORE_NAME               6 (from_dict)
                       60 LOAD_CONST              10 (None)
                       62 RETURN_VALUE
          consts
             'CallbackButton'
             '\n    Represents a callback button.\n\n    Attributes:\n        id: The ID of the message.\n        metadata: The metadata of the message (to which phone number it was sent).\n        from_user: The user who sent the message.\n        timestamp: The timestamp when the message was sent.\n        data: The data of the button.\n        title: The title of the button.\n    '
             'str'
             'data'
@@ -4523,79 +4604,79 @@
                   02640519000000000000000000640219000000000000000000a6010000ab
                   0100000000000000007407000000000000000000006a0400000000000000
                   00740b000000000000000000007c03640619000000000000000000a60100
                   00ab010000000000000000a6010000ab0100000000000000007c03640719
                   000000000000000000640819000000000000000000640319000000000000
                   0000007c0364071900000000000000000064081900000000000000000064
                   0919000000000000000000ac0aa6070000ab0700000000000000005300
-               744           0 RESUME                   0
+               771           0 RESUME                   0
                
-               746           2 LOAD_FAST                2 (value)
+               773           2 LOAD_FAST                2 (value)
                              4 LOAD_CONST               1 ('messages')
                              6 BINARY_SUBSCR
                             16 LOAD_CONST               2 (0)
                             18 BINARY_SUBSCR
                             28 STORE_FAST               3 (message)
                
-               747          30 PUSH_NULL
+               774          30 PUSH_NULL
                             32 LOAD_FAST                0 (cls)
                
-               748          34 LOAD_FAST                1 (client)
+               775          34 LOAD_FAST                1 (client)
                
-               749          36 LOAD_FAST                3 (message)
+               776          36 LOAD_FAST                3 (message)
                             38 LOAD_CONST               3 ('id')
                             40 BINARY_SUBSCR
                
-               750          50 LOAD_GLOBAL              1 (NULL + Metadata)
+               777          50 LOAD_GLOBAL              1 (NULL + Metadata)
                             62 LOAD_CONST              11 (())
                             64 BUILD_MAP                0
                             66 LOAD_FAST                2 (value)
                             68 LOAD_CONST               4 ('metadata')
                             70 BINARY_SUBSCR
                             80 DICT_MERGE               1
                             82 CALL_FUNCTION_EX         1
                
-               751          84 LOAD_GLOBAL              2 (User)
+               778          84 LOAD_GLOBAL              2 (User)
                             96 LOAD_METHOD              2 (from_dict)
                            118 LOAD_FAST                2 (value)
                            120 LOAD_CONST               5 ('contacts')
                            122 BINARY_SUBSCR
                            132 LOAD_CONST               2 (0)
                            134 BINARY_SUBSCR
                            144 PRECALL                  1
                            148 CALL                     1
                
-               752         158 LOAD_GLOBAL              7 (NULL + datetime)
+               779         158 LOAD_GLOBAL              7 (NULL + datetime)
                            170 LOAD_ATTR                4 (fromtimestamp)
                            180 LOAD_GLOBAL             11 (NULL + int)
                            192 LOAD_FAST                3 (message)
                            194 LOAD_CONST               6 ('timestamp')
                            196 BINARY_SUBSCR
                            206 PRECALL                  1
                            210 CALL                     1
                            220 PRECALL                  1
                            224 CALL                     1
                
-               753         234 LOAD_FAST                3 (message)
+               780         234 LOAD_FAST                3 (message)
                            236 LOAD_CONST               7 ('interactive')
                            238 BINARY_SUBSCR
                            248 LOAD_CONST               8 ('button_reply')
                            250 BINARY_SUBSCR
                            260 LOAD_CONST               3 ('id')
                            262 BINARY_SUBSCR
                
-               754         272 LOAD_FAST                3 (message)
+               781         272 LOAD_FAST                3 (message)
                            274 LOAD_CONST               7 ('interactive')
                            276 BINARY_SUBSCR
                            286 LOAD_CONST               8 ('button_reply')
                            288 BINARY_SUBSCR
                            298 LOAD_CONST               9 ('title')
                            300 BINARY_SUBSCR
                
-               747         310 KW_NAMES                10
+               774         310 KW_NAMES                10
                            312 PRECALL                  7
                            316 CALL                     7
                            326 RETURN_VALUE
                consts
                   None
                   'messages'
                   0
@@ -4610,71 +4691,71 @@
                   ()
                names      ('Metadata', 'User', 'from_dict', 'datetime', 'fromtimestamp', 'int')
                varnames   ('cls', 'client', 'value', 'message')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
                name       'from_dict'
-               firstlineno 744
+               firstlineno 771
                lnotab 0x02021c01040102010e0122014a014c01260126f9
             None
             ('client', 'WhatsApp', 'value', 'dict')
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__annotations__', 'classmethod', 'from_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
          name       'CallbackButton'
-         firstlineno 728
+         firstlineno 755
          lnotab 0x0c02040b0a010a02020106ff0e01
       'CallbackButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a036402650464033c000000640265
             0464043c0000006405650464063c0000006505640d640b8404a6000000ab
             0000000000000000005a06640c5300
-         758           0 RESUME                   0
+         785           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('CallbackSelection')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         760          12 LOAD_CONST               1 ('\n    Represents a callback selection.\n\n    Attributes:\n        id: The ID of the message.\n        metadata: The metadata of the message (to which phone number it was sent).\n        from_user: The user who sent the message.\n        timestamp: The timestamp when the message was sent.\n        data: The data of the selection.\n        title: The title of the selection.\n        description: The description of the selection (optional).\n    ')
+         787          12 LOAD_CONST               1 ('\n    Represents a callback selection.\n\n    Attributes:\n        id: The ID of the message.\n        metadata: The metadata of the message (to which phone number it was sent).\n        from_user: The user who sent the message.\n        timestamp: The timestamp when the message was sent.\n        data: The data of the selection.\n        title: The title of the selection.\n        description: The description of the selection (optional).\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         772          16 LOAD_CONST               2 ('str')
+         799          16 LOAD_CONST               2 ('str')
                       18 LOAD_NAME                4 (__annotations__)
                       20 LOAD_CONST               3 ('data')
                       22 STORE_SUBSCR
          
-         773          26 LOAD_CONST               2 ('str')
+         800          26 LOAD_CONST               2 ('str')
                       28 LOAD_NAME                4 (__annotations__)
                       30 LOAD_CONST               4 ('title')
                       32 STORE_SUBSCR
          
-         774          36 LOAD_CONST               5 ('str | None')
+         801          36 LOAD_CONST               5 ('str | None')
                       38 LOAD_NAME                4 (__annotations__)
                       40 LOAD_CONST               6 ('description')
                       42 STORE_SUBSCR
          
-         776          46 LOAD_NAME                5 (classmethod)
+         803          46 LOAD_NAME                5 (classmethod)
          
-         777          48 LOAD_CONST              13 (('client', 'WhatsApp', 'value', 'dict'))
-                      50 LOAD_CONST              11 (<code object from_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 776>)
+         804          48 LOAD_CONST              13 (('client', 'WhatsApp', 'value', 'dict'))
+                      50 LOAD_CONST              11 (<code object from_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 803>)
                       52 MAKE_FUNCTION            4 (annotations)
          
-         776          54 PRECALL                  0
+         803          54 PRECALL                  0
                       58 CALL                     0
          
-         777          68 STORE_NAME               6 (from_dict)
+         804          68 STORE_NAME               6 (from_dict)
                       70 LOAD_CONST              12 (None)
                       72 RETURN_VALUE
          consts
             'CallbackSelection'
             '\n    Represents a callback selection.\n\n    Attributes:\n        id: The ID of the message.\n        metadata: The metadata of the message (to which phone number it was sent).\n        from_user: The user who sent the message.\n        timestamp: The timestamp when the message was sent.\n        data: The data of the selection.\n        title: The title of the selection.\n        description: The description of the selection (optional).\n    '
             'str'
             'data'
@@ -4701,89 +4782,89 @@
                   00ab010000000000000000a6010000ab0100000000000000007c03640719
                   000000000000000000640819000000000000000000640319000000000000
                   0000007c0364071900000000000000000064081900000000000000000064
                   09190000000000000000007c036407190000000000000000006408190000
                   00000000000000a006000000000000000000000000000000000000000064
                   0aa6010000ab010000000000000000ac0ba6080000ab0800000000000000
                   005300
-               776           0 RESUME                   0
+               803           0 RESUME                   0
                
-               778           2 LOAD_FAST                2 (value)
+               805           2 LOAD_FAST                2 (value)
                              4 LOAD_CONST               1 ('messages')
                              6 BINARY_SUBSCR
                             16 LOAD_CONST               2 (0)
                             18 BINARY_SUBSCR
                             28 STORE_FAST               3 (message)
                
-               779          30 PUSH_NULL
+               806          30 PUSH_NULL
                             32 LOAD_FAST                0 (cls)
                
-               780          34 LOAD_FAST                1 (client)
+               807          34 LOAD_FAST                1 (client)
                
-               781          36 LOAD_FAST                3 (message)
+               808          36 LOAD_FAST                3 (message)
                             38 LOAD_CONST               3 ('id')
                             40 BINARY_SUBSCR
                
-               782          50 LOAD_GLOBAL              1 (NULL + Metadata)
+               809          50 LOAD_GLOBAL              1 (NULL + Metadata)
                             62 LOAD_CONST              12 (())
                             64 BUILD_MAP                0
                             66 LOAD_FAST                2 (value)
                             68 LOAD_CONST               4 ('metadata')
                             70 BINARY_SUBSCR
                             80 DICT_MERGE               1
                             82 CALL_FUNCTION_EX         1
                
-               783          84 LOAD_GLOBAL              2 (User)
+               810          84 LOAD_GLOBAL              2 (User)
                             96 LOAD_METHOD              2 (from_dict)
                            118 LOAD_FAST                2 (value)
                            120 LOAD_CONST               5 ('contacts')
                            122 BINARY_SUBSCR
                            132 LOAD_CONST               2 (0)
                            134 BINARY_SUBSCR
                            144 PRECALL                  1
                            148 CALL                     1
                
-               784         158 LOAD_GLOBAL              7 (NULL + datetime)
+               811         158 LOAD_GLOBAL              7 (NULL + datetime)
                            170 LOAD_ATTR                4 (fromtimestamp)
                            180 LOAD_GLOBAL             11 (NULL + int)
                            192 LOAD_FAST                3 (message)
                            194 LOAD_CONST               6 ('timestamp')
                            196 BINARY_SUBSCR
                            206 PRECALL                  1
                            210 CALL                     1
                            220 PRECALL                  1
                            224 CALL                     1
                
-               785         234 LOAD_FAST                3 (message)
+               812         234 LOAD_FAST                3 (message)
                            236 LOAD_CONST               7 ('interactive')
                            238 BINARY_SUBSCR
                            248 LOAD_CONST               8 ('list_reply')
                            250 BINARY_SUBSCR
                            260 LOAD_CONST               3 ('id')
                            262 BINARY_SUBSCR
                
-               786         272 LOAD_FAST                3 (message)
+               813         272 LOAD_FAST                3 (message)
                            274 LOAD_CONST               7 ('interactive')
                            276 BINARY_SUBSCR
                            286 LOAD_CONST               8 ('list_reply')
                            288 BINARY_SUBSCR
                            298 LOAD_CONST               9 ('title')
                            300 BINARY_SUBSCR
                
-               787         310 LOAD_FAST                3 (message)
+               814         310 LOAD_FAST                3 (message)
                            312 LOAD_CONST               7 ('interactive')
                            314 BINARY_SUBSCR
                            324 LOAD_CONST               8 ('list_reply')
                            326 BINARY_SUBSCR
                            336 LOAD_METHOD              6 (get)
                            358 LOAD_CONST              10 ('description')
                            360 PRECALL                  1
                            364 CALL                     1
                
-               779         374 KW_NAMES                11
+               806         374 KW_NAMES                11
                            376 PRECALL                  8
                            380 CALL                     8
                            390 RETURN_VALUE
                consts
                   None
                   'messages'
                   0
@@ -4799,55 +4880,55 @@
                   ()
                names      ('Metadata', 'User', 'from_dict', 'datetime', 'fromtimestamp', 'int', 'get')
                varnames   ('cls', 'client', 'value', 'message')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
                name       'from_dict'
-               firstlineno 776
+               firstlineno 803
                lnotab 0x02021c01040102010e0122014a014c012601260140f8
             None
             ('client', 'WhatsApp', 'value', 'dict')
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__annotations__', 'classmethod', 'from_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
          name       'CallbackSelection'
-         firstlineno 758
+         firstlineno 785
          lnotab 0x0c02040c0a010a010a02020106ff0e01
       'CallbackSelection'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a0364025a0464035a0564045a0664
             05650764063c00000064075300
-         791           0 RESUME                   0
+         818           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MessageStatusType')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         792          12 LOAD_CONST               1 ('Message status type.')
+         819          12 LOAD_CONST               1 ('Message status type.')
                       14 STORE_NAME               3 (__doc__)
          
-         793          16 LOAD_CONST               2 ('sent')
+         820          16 LOAD_CONST               2 ('sent')
                       18 STORE_NAME               4 (SENT)
          
-         794          20 LOAD_CONST               3 ('delivered')
+         821          20 LOAD_CONST               3 ('delivered')
                       22 STORE_NAME               5 (DELIVERED)
          
-         795          24 LOAD_CONST               4 ('read')
+         822          24 LOAD_CONST               4 ('read')
                       26 STORE_NAME               6 (READ)
          
-         796          28 LOAD_CONST               5 ('datetime')
+         823          28 LOAD_CONST               5 ('datetime')
                       30 LOAD_NAME                7 (__annotations__)
                       32 LOAD_CONST               6 ('timestamp')
                       34 STORE_SUBSCR
                       38 LOAD_CONST               7 (None)
                       40 RETURN_VALUE
          consts
             'MessageStatusType'
@@ -4860,50 +4941,50 @@
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'SENT', 'DELIVERED', 'READ', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
          name       'MessageStatusType'
-         firstlineno 791
+         firstlineno 818
          lnotab 0x0c010401040104010401
       'MessageStatusType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 16777216
          code
             0x970065005a0164005a02550064015a036402650464033c000000650564
             0a64088404a6000000ab0000000000000000005a0664095300
-         799           0 RESUME                   0
+         826           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MessageStatus')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         801          12 LOAD_CONST               1 ('\n    Represents the status of a message.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#statuses-object\n\n    Attributes:\n        id: The ID of the message that the status is for.\n        metadata: The metadata of the message (to which phone number it was sent).\n        status: The status of the message.\n        timestamp: The timestamp when the status was updated.\n        from_user: The user who the message was sent to.\n    ')
+         828          12 LOAD_CONST               1 ('\n    Represents the status of a message.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#statuses-object\n\n    Attributes:\n        id: The ID of the message that the status is for.\n        metadata: The metadata of the message (to which phone number it was sent).\n        status: The status of the message.\n        timestamp: The timestamp when the status was updated.\n        from_user: The user who the message was sent to.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-         813          16 LOAD_CONST               2 ('MessageStatusType')
+         840          16 LOAD_CONST               2 ('MessageStatusType')
                       18 LOAD_NAME                4 (__annotations__)
                       20 LOAD_CONST               3 ('status')
                       22 STORE_SUBSCR
          
-         815          26 LOAD_NAME                5 (classmethod)
+         842          26 LOAD_NAME                5 (classmethod)
          
-         816          28 LOAD_CONST              10 (('client', 'WhatsApp', 'value', 'dict'))
-                      30 LOAD_CONST               8 (<code object from_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 815>)
+         843          28 LOAD_CONST              10 (('client', 'WhatsApp', 'value', 'dict'))
+                      30 LOAD_CONST               8 (<code object from_dict, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py", line 842>)
                       32 MAKE_FUNCTION            4 (annotations)
          
-         815          34 PRECALL                  0
+         842          34 PRECALL                  0
                       38 CALL                     0
          
-         816          48 STORE_NAME               6 (from_dict)
+         843          48 STORE_NAME               6 (from_dict)
                       50 LOAD_CONST               9 (None)
                       52 RETURN_VALUE
          consts
             'MessageStatus'
             '\n    Represents the status of a message.\n\n    - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#statuses-object\n\n    Attributes:\n        id: The ID of the message that the status is for.\n        metadata: The metadata of the message (to which phone number it was sent).\n        status: The status of the message.\n        timestamp: The timestamp when the status was updated.\n        from_user: The user who the message was sent to.\n    '
             'MessageStatusType'
             'status'
@@ -4922,69 +5003,69 @@
                   000000640a69007c02640419000000000000000000a4018e017403000000
                   000000000000007c03640519000000000000000000a6010000ab01000000
                   00000000007405000000000000000000006a030000000000000000740900
                   0000000000000000007c03640619000000000000000000a6010000ab0100
                   00000000000000a6010000ab010000000000000000740b00000000000000
                   0000007c036407190000000000000000006400ac08a6020000ab02000000
                   0000000000ac09a6060000ab0600000000000000005300
-               815           0 RESUME                   0
+               842           0 RESUME                   0
                
-               817           2 LOAD_FAST                2 (value)
+               844           2 LOAD_FAST                2 (value)
                              4 LOAD_CONST               1 ('statuses')
                              6 BINARY_SUBSCR
                             16 LOAD_CONST               2 (0)
                             18 BINARY_SUBSCR
                             28 STORE_FAST               3 (status)
                
-               818          30 PUSH_NULL
+               845          30 PUSH_NULL
                             32 LOAD_FAST                0 (cls)
                
-               819          34 LOAD_FAST                1 (client)
+               846          34 LOAD_FAST                1 (client)
                
-               820          36 LOAD_FAST                3 (status)
+               847          36 LOAD_FAST                3 (status)
                             38 LOAD_CONST               3 ('id')
                             40 BINARY_SUBSCR
                
-               821          50 LOAD_GLOBAL              1 (NULL + Metadata)
+               848          50 LOAD_GLOBAL              1 (NULL + Metadata)
                             62 LOAD_CONST              10 (())
                             64 BUILD_MAP                0
                             66 LOAD_FAST                2 (value)
                             68 LOAD_CONST               4 ('metadata')
                             70 BINARY_SUBSCR
                             80 DICT_MERGE               1
                             82 CALL_FUNCTION_EX         1
                
-               822          84 LOAD_GLOBAL              3 (NULL + MessageStatusType)
+               849          84 LOAD_GLOBAL              3 (NULL + MessageStatusType)
                             96 LOAD_FAST                3 (status)
                             98 LOAD_CONST               5 ('status')
                            100 BINARY_SUBSCR
                            110 PRECALL                  1
                            114 CALL                     1
                
-               823         124 LOAD_GLOBAL              5 (NULL + datetime)
+               850         124 LOAD_GLOBAL              5 (NULL + datetime)
                            136 LOAD_ATTR                3 (fromtimestamp)
                            146 LOAD_GLOBAL              9 (NULL + int)
                            158 LOAD_FAST                3 (status)
                            160 LOAD_CONST               6 ('timestamp')
                            162 BINARY_SUBSCR
                            172 PRECALL                  1
                            176 CALL                     1
                            186 PRECALL                  1
                            190 CALL                     1
                
-               824         200 LOAD_GLOBAL             11 (NULL + User)
+               851         200 LOAD_GLOBAL             11 (NULL + User)
                            212 LOAD_FAST                3 (status)
                            214 LOAD_CONST               7 ('recipient_id')
                            216 BINARY_SUBSCR
                            226 LOAD_CONST               0 (None)
                            228 KW_NAMES                 8
                            230 PRECALL                  2
                            234 CALL                     2
                
-               818         244 KW_NAMES                 9
+               845         244 KW_NAMES                 9
                            246 PRECALL                  6
                            250 CALL                     6
                            260 RETURN_VALUE
                consts
                   None
                   'statuses'
                   0
@@ -4998,25 +5079,25 @@
                   ()
                names      ('Metadata', 'MessageStatusType', 'datetime', 'fromtimestamp', 'int', 'User')
                varnames   ('cls', 'client', 'value', 'status')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
                name       'from_dict'
-               firstlineno 815
+               firstlineno 842
                lnotab 0x02021c01040102010e01220128014c012cfa
             None
             ('client', 'WhatsApp', 'value', 'dict')
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__annotations__', 'classmethod', 'from_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py'
          name       'MessageStatus'
-         firstlineno 799
+         firstlineno 826
          lnotab 0x0c02040c0a02020106ff0e01
       'MessageStatus'
       None
    names      ('__future__', 'annotations', '__all__', 'datetime', 'dataclasses', 'dataclass', 'field', 'asdict', 'enum', 'Enum', 'typing', 'TYPE_CHECKING', 'Iterable', 'pywa', 'utils', 'pywa.client', 'WhatsApp', 'InlineButton', 'SectionRow', 'Section', 'SectionList', 'User', 'str', 'MessageType', 'MediaBase', 'Image', 'Video', 'Sticker', 'Document', 'Audio', 'Reaction', 'Location', 'Contact', 'ReplyToMessage', 'Metadata', 'BaseUpdate', 'Message', 'CallbackButton', 'CallbackSelection', 'MessageStatusType', 'MessageStatus')
    varnames   ()
    freevars   ()
    cellvars   ()
@@ -5025,9 +5106,9 @@
    firstlineno 1
    lnotab
       0x00ff02010c02040e0c0114010c0110020c0204010c03180118ff0e0102
       0f180118ff0e010214180118ff0e010214180118ff0e010214180118ff0e
       0102101e18180118ff0e01020a18011aff0e01020d18011aff0e01020c18
       011aff0e01020d18011aff0e01020d18011aff0e01020d180118ff0e0102
       10180118ff0e010222180118ff0e01025e180118ff0e010213180118ff0e
-      01020c180118ff0e01027f007f000518011aff0e01023b18011aff0e0102
+      01020c180118ff0e01027f007f002018011aff0e01023b18011aff0e0102
       1d18011aff0e0102201c0818011aff0e01
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py

```diff
@@ -244,7 +244,21 @@
         if reply_to_message_id:
             data["context"] = {"message_id": reply_to_message_id}
         return self._make_request(
             method="POST",
             endpoint=f"/messages",
             json=data
         )['messages'][0]['id']
+
+    def mark_message_as_read(
+            self,
+            message_id: str
+    ) -> bool:
+        return self._make_request(
+            method="POST",
+            endpoint=f"/messages",
+            json={
+                "messaging_product": "whatsapp",
+                "status": "read",
+                "message_id": message_id
+            }
+        )["success"]
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py

```diff
@@ -249,20 +249,20 @@
             ...     ),
             ...     footer="Powered by PyWa",
             ... )
 
 
         Args:
             to: The phone ID of the WhatsApp user.
-            text: The text to send.
+            text: The text to send (markdown allowed, max 4096 characters).
             preview_url: Whether to show a preview of the URL in the message (if any).
             reply_to_message_id: The message ID to reply to (optional).
             keyboard: The keyboard to send with the message (optional).
-            header: The header of the message (if keyboard is provided, optional).
-            footer: The footer of the message (if keyboard is provided, optional).
+            header: The header of the message (if keyboard is provided, optional, up to 60 characters, no markdown allowed).
+            footer: The footer of the message (if keyboard is provided, optional, up to 60 characters, markdown has no effect).
 
         Returns:
             The message ID of the sent message.
         """
         if not keyboard:
             return self.api.send_text_message(
                 to=to,
@@ -301,19 +301,19 @@
             ...     image="https://example.com/image.png",
             ...     caption="This is an image!",
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
             image: The image to send (either a URL or a file ID).
-            caption: The caption of the image (optional).
+            caption: The caption of the image (optional, markdown allowed).
             reply_to_message_id: The message ID to reply to (optional).
             buttons: The buttons to send with the image (optional).
-            body: The body of the message (if buttons are provided, optional).
-            footer: The footer of the message (if buttons are provided, optional).
+            body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).
+            footer: The footer of the message (if buttons is provided, optional, markdown has no effect).
 
         Returns:
             The message ID of the sent image.
         """
         if not buttons:
             return self.api.send_media(
                 to=to,
@@ -358,19 +358,19 @@
             ...     video="https://example.com/video.mp4",
             ...     caption="This is a video",
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
             video: The video to send (either a URL or a file ID).
-            caption: The caption of the video (optional).
+            caption: The caption of the video (optional, markdown allowed).
             reply_to_message_id: The message ID to reply to (optional).
             buttons: The buttons to send with the video (optional).
-            body: The body of the message (if buttons are provided, optional).
-            footer: The footer of the message (if buttons are provided, optional).
+            body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).
+            footer: The footer of the message (if buttons is provided, optional, markdown has no effect).
 
         Returns:
             The message ID of the sent message.
         """
         if not buttons:
             return self.api.send_media(
                 to=to,
@@ -418,20 +418,20 @@
             ...     caption="Example PDF"
             ... )
 
 
         Args:
             to: The phone ID of the WhatsApp user.
             document: The document to send (either a URL or a file ID).
-            filename: The filename of the document (optional).
+            filename: The filename of the document (optional, The extension of the filename will specify what format the document is displayed as in WhatsApp).
             caption: The caption of the document (optional).
             reply_to_message_id: The message ID to reply to (optional).
             buttons: The buttons to send with the document (optional).
-            body: The body of the message (if buttons are provided, optional).
-            footer: The footer of the message (if buttons are provided, optional).
+            body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).
+            footer: The footer of the message (if buttons is provided, optional, markdown has no effect).
 
         Returns:
             The message ID of the sent message.
         """
         if not buttons:
             return self.api.send_media(
                 to=to,
@@ -494,14 +494,16 @@
             to: str,
             sticker: str | bytes,
             animated: bool = False,
             reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send a sticker to a WhatsApp user.
+            - A static sticker needs to be 512x512 pixels and cannot exceed 100 KB.
+            - An animated sticker must be 512x512 pixels and cannot exceed 500 KB.
 
         Example:
 
             >>> wa.send_sticker(
             ...     to='1234567890',
             ...     sticker='https://example.com/sticker.webp',
             ... )
@@ -550,14 +552,35 @@
         """
         return self.api.send_reaction(
             to=to,
             emoji=emoji,
             message_id=message_id,
         )
 
+    def remove_reaction(
+            self,
+            to: str,
+            message_id: str,
+    ) -> str:
+        """
+        Remove a reaction from a message.
+
+        Example:
+
+            >>> wa.remove_reaction(
+            ...     to='1234567890',
+            ...     message_id='wamid.XXX='
+            ... )
+        """
+        return self.api.send_reaction(
+            to=to,
+            message_id=message_id,
+            emoji=""
+        )
+
     def send_location(
             self,
             to: str,
             latitude: float,
             longitude: float,
             name: str | None = None,
             address: str | None = None,
@@ -621,7 +644,22 @@
             The message ID of the sent message.
         """
         return self.api.send_contacts(
             to=to,
             contacts=contact if isinstance(contact, Iterable) else [contact],
             reply_to_message_id=reply_to_message_id,
         )
+
+    def mark_message_as_read(
+            self,
+            message_id: str,
+    ) -> bool:
+        """
+        Mark a message as read.
+
+        Args:
+            message_id: The message ID to mark as read.
+
+        Returns:
+            Whether the message was marked as read.
+        """
+        return self.api.mark_message_as_read(message_id=message_id)
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py

```diff
@@ -1,270 +1,281 @@
 """Usefully filters to use in your handlers."""
 from __future__ import annotations
 
 import re
 from typing import Callable, TYPE_CHECKING, Iterable
-from pywa.types import MessageType as Mt, Message as Msg, MessageStatus as Ms, \
-    MessageStatusType as Mst, CallbackButton, CallbackSelection
 from pywa import utils
+from pywa.types import MessageType as Mt, Message as Msg, MessageStatus as Ms, MessageStatusType as Mst, \
+    CallbackButton, CallbackSelection
 
 if TYPE_CHECKING:
     from pywa import WhatsApp as Wa
 
+__all__ = (
+    "TextFilter",
+    "ImageFilter",
+    "VideoFilter",
+    "AudioFilter",
+    "DocumentFilter",
+    "StickerFilter",
+    "ReactionFilter",
+    "UnsupportedMsgFilter",
+    "LocationFilter",
+    "ContactsFilter",
+    "CallbackFilter",
+)
+
+_ONLY_NUMS_RE = re.compile(r"\D")
+
 
 class TextFilter:
     """Useful filters for text messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.TEXT
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.TEXT
     """Filter for all text messages."""
 
-    EQUALS: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda text: lambda wa, data: data.type == Mt.TEXT and (
-            isinstance(text, str) and text == data.text or
-            isinstance(text, Iterable) and
-            any((t == data.text for t in text)))
-    """Filter for text messages that equal the given text/s."""
-
-    CONTAINS: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda text: lambda wa, data: data.type == Mt.TEXT and (
-            isinstance(text, str) and text in data.text or
-            isinstance(text, Iterable) and
-            any((t in data.text for t in text)))
-    """Filter for text messages that contain the given text/s."""
-
-    STARTS_WITH: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda text: lambda wa, data: data.type == Mt.TEXT and (
-            isinstance(text, str) and data.text.startswith(text) or
-            isinstance(text, Iterable) and
-            any((data.text.startswith(t) for t in text)))
-    """Filter for text messages that start with the given text/s."""
-
-    ENDS_WITH: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda text: lambda wa, data: data.type == Mt.TEXT and (
-            isinstance(text, str) and data.text.endswith(text) or
-            isinstance(text, Iterable) and
-            any((data.text.endswith(t) for t in text)))
-    """Filter for text messages that end with the given text/s."""
-
-    REGEX: Callable[[str | Iterable[str] | re.Pattern | Iterable[re.Pattern]], Callable[[Wa, Msg], bool]] \
-        = lambda reg: lambda wa, data: data.type == Mt.TEXT and (
-            isinstance(reg, (str, re.Pattern)) and re.match(reg, data.text) or
-            isinstance(reg, Iterable) and
-            any((re.match(t, data.text) for t in reg)))
-    """Filter for text messages that match the given regex/regexes."""
-
-    LEN_BETWEEN: Callable[[tuple[int, int] | Iterable[tuple[int, int]]], Callable[[Wa, Msg], bool]] \
-        = lambda length: lambda wa, data: data.type == Mt.TEXT and (
-            isinstance(length, tuple) and length[0] <= len(data.text) <= length[1] or
-            isinstance(length, Iterable) and
-            any((l[0] <= len(data.text) <= l[1] for l in length)))
-    """Filter for text messages that have a length between the given range/s."""
+    @staticmethod
+    def equals(*matches: str) -> Callable[[Wa, Msg], bool]:
+        """Filter for text messages that equal the given text/s."""
+        return lambda wa, m: m.type == Mt.TEXT and any((t == m.text for t in matches))
+
+    @staticmethod
+    def contains(*matches: str) -> Callable[[Wa, Msg], bool]:
+        """Filter for text messages that contain the given text/s."""
+        return lambda wa, m: m.type == Mt.TEXT and any((t in m.text for t in matches))
+
+    @staticmethod
+    def startswith(*matches: str) -> Callable[[Wa, Msg], bool]:
+        """Filter for text messages that start with the given text/s."""
+        return lambda wa, m: m.type == Mt.TEXT and any((m.text.startswith(t) for t in matches))
+
+    @staticmethod
+    def endswith(*matches: str) -> Callable[[Wa, Msg], bool]:
+        """Filter for text messages that end with the given text/s."""
+        return lambda wa, m: m.type == Mt.TEXT and any((m.text.endswith(t) for t in matches))
 
     @staticmethod
-    def COMMAND(cmd: str | Iterable[str], prefix: str = "/") -> Callable[[Wa, Msg], bool]:
+    def regex(*patterns: str | re.Pattern, flags: int = 0) -> Callable[[Wa, Msg], bool]:
+        """
+        Filter for text messages that match the given regex/regexes.
+            * It's recommended to pass compiled regexes to save time (``re.compile(your_pattern)``)
+        """
+        return lambda wa, m: m.type == Mt.TEXT and any(re.match(p, m.text, flags) for p in patterns)
+
+    @staticmethod
+    def length(*lengths: tuple[int, int]) -> Callable[[Wa, Msg], bool]:
+        """
+        Filter for text messages that have a length between the given range/s.
+
+        Args:
+            lengths: The length range/s to filter for (e.g. (1, 10), (50, 100)).
+        """
+        return lambda wa, m: m.type == Mt.TEXT and any((i[0] <= len(m.text) <= i[1] for i in lengths))
+
+    @staticmethod
+    def command(*cmds: str, prefixes: str | Iterable[str] = "!") -> Callable[[Wa, Msg], bool]:
         """
         Filter for text messages that are commands.
 
         Args:
-            cmd: The command/s to filter for.
-            prefix: The prefix to filter for (default: "/").
+            cmds: The command/s to filter for (e.g. "start", "hello").
+            prefixes: The prefix/s to filter for (default: "!", i.e. "!start").
         """
-        return lambda wa, data: data.type == Mt.TEXT and (
-                isinstance(cmd, str) and data.text.startswith(prefix + cmd) or
-                isinstance(cmd, Iterable) and
-                any((data.text.startswith(prefix + c) for c in cmd)))
+        return lambda wa, m: m.type == Mt.TEXT and any(m.text[0] in prefixes and m.text[1:].startswith(c) for c in cmds)
 
 
 class ImageFilter:
     """Useful filters for image messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.IMAGE
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.IMAGE
     """Filter for all image messages."""
 
-    HAS_CAPTION: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.IMAGE and data.image.caption is not None
-    """Filter for image messages that have a caption."""
+    @staticmethod
+    def has_caption(wa: Wa, m: Msg) -> bool:
+        """Filter for image messages that have a caption."""
+        return m.type == Mt.IMAGE and m.image.caption is not None
 
-    MIME_TYPE: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda mime: lambda wa, data: data.type == Mt.IMAGE and (
-            isinstance(mime, str) and data.image.mime_type == mime or
-            isinstance(mime, Iterable) and
-            any((t == data.image.mime_type for t in mime)))
-    """
-    Filter for image messages that have the given mime type/s.
-    See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
-    """
+    @staticmethod
+    def mimetype(*mime_types: str) -> Callable[[Wa, Msg], bool]:
+        """
+        Filter for image messages that have the given mime type/s.
+        See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
+        """
+        return lambda wa, m: m.type == Mt.IMAGE and any((t == m.image.mime_type for t in mime_types))
 
 
 class VideoFilter:
     """Useful filters for video messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.VIDEO
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.VIDEO
     """Filter for all video messages."""
 
-    MIME_TYPE: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda mime: lambda wa, data: data.type == Mt.VIDEO and (
-            isinstance(mime, str) and data.video.mime_type == mime or
-            isinstance(mime, Iterable) and
-            any((t == data.video.mime_type for t in mime)))
-    """
-    Filter for video messages that have the given mime type/s.
-    See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
-    """
+    @staticmethod
+    def mimetype(*mime_types: str) -> Callable[[Wa, Msg], bool]:
+        """
+        Filter for video messages that have the given mime type/s.
+        See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
+        """
+        return lambda wa, m: m.type == Mt.VIDEO and any((t == m.video.mime_type for t in mime_types))
 
 
 class AudioFilter:
     """Useful filters for audio messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.AUDIO
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.AUDIO
     """Filter for all audio messages."""
 
-    IS_VOICE: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.AUDIO and data.audio.voice
+    VOICE: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.AUDIO and m.audio.voice
     """Filter for audio messages that are voice notes."""
 
-    IS_AUDIO: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.AUDIO and not data.audio.voice
+    AUDIO: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.AUDIO and not m.audio.voice
     """Filter for audio messages that are audio files."""
 
-    MIME_TYPE: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda mime: lambda wa, data: data.type == Mt.AUDIO and (
-            isinstance(mime, str) and data.audio.mime_type == mime or
-            isinstance(mime, Iterable) and
-            any((t == data.audio.mime_type for t in mime)))
-    """
-    Filter for audio messages that have the given mime type/s.
-    See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
-    """
+    @staticmethod
+    def mimetype(*mime_types: str) -> Callable[[Wa, Msg], bool]:
+        """
+        Filter for audio messages that have the given mime type/s.
+        See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
+        """
+        return lambda wa, m: m.type == Mt.AUDIO and any((t == m.audio.mime_type for t in mime_types))
 
 
 class DocumentFilter:
     """Useful filters for document messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.DOCUMENT
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.DOCUMENT
     """Filter for all document messages."""
 
-    MIME_TYPE: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda mime: lambda wa, data: data.type == Mt.DOCUMENT and (
-            isinstance(mime, str) and data.document.mime_type == mime or
-            isinstance(mime, Iterable) and
-            any((t == data.document.mime_type for t in mime)))
-    """
-    Filter for document messages that have the given mime type/s. 
-    See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
-    """
+    @staticmethod
+    def mimetype(*mime_types: str) -> Callable[[Wa, Msg], bool]:
+        """
+        Filter for document messages that have the given mime type/s.
+        See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
+        """
+        return lambda wa, m: m.type == Mt.DOCUMENT and any((t == m.document.mime_type for t in mime_types))
 
 
 class StickerFilter:
     """Useful filters for sticker messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.STICKER
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.STICKER
     """Filter for all sticker messages."""
 
-    IS_ANIMATED: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.STICKER and data.sticker.animated
+    ANIMATED: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.STICKER and m.sticker.animated
     """Filter for animated sticker messages."""
 
+    STATIC: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.STICKER and not m.sticker.animated
+
 
 class LocationFilter:
     """Useful filters for location messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.LOCATION
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.LOCATION
     """Filter for all location messages."""
 
     @staticmethod
-    def IN_RADIUS(lat: float, lon: float, radius: float | int) -> Callable[[Wa, Msg], bool]:
+    def in_radius(lat: float, lon: float, radius: float | int) -> Callable[[Wa, Msg], bool]:
         """
         Filter for location messages that are in a given radius.
 
-        >>> LocationFilter.IN_RADIUS(lat=37.48508108998884, lon=-122.14744733542707, radius=1)
+        >>> LocationFilter.in_radius(lat=37.48508108998884, lon=-122.14744733542707, radius=1)
 
         Args:
-            lat (float): Latitude of the center of the radius.
-            lon (float): Longitude of the center of the radius.
-            radius (float | int): Radius in kilometers.
+            lat: Latitude of the center of the radius.
+            lon: Longitude of the center of the radius.
+            radius: Radius in kilometers.
         """
 
         def _in_radius(_: Wa, msg: Msg) -> bool:
             return msg.type == Mt.LOCATION and \
                 utils.get_distance(
                     lat1=lat, lon1=lon, lat2=msg.location.latitude, lon2=msg.location.longitude
                 ) <= radius
 
         return _in_radius
 
 
 class ReactionFilter:
     """Useful filters for reaction messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.REACTION
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.REACTION
     """Filter for all reaction messages."""
 
-    EMOJI: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda reaction: lambda wa, data: data.type == Mt.REACTION and data.reaction.emoji in reaction
-    """Filter for custom reaction messages. pass emojis as a list or a single string."""
+    @staticmethod
+    def emoji(*emojis: str) -> Callable[[Wa, Msg], bool]:
+        """
+        Filter for custom reaction messages. pass emojis as strings.
+        """
+        return lambda wa, m: m.type == Mt.REACTION and m.reaction.emoji in emojis
 
 
 class ContactsFilter:
     """Useful filters for contact messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.CONTACTS
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.CONTACTS
     """Filter for all contacts messages."""
 
-    COUNT_BETWEEN: Callable[[int, int], Callable[[Wa, Msg], bool]] \
-        = lambda min_count, max_count: lambda wa, data: \
-        data.type == Mt.CONTACTS and min_count <= len(data.contacts) <= max_count
-    """Filter for contacts messages that have a number of contacts between min_count and max_count."""
-
-    PHONE_NUMBER: Callable[[str | Iterable[str]], Callable[[Wa, Msg], bool]] \
-        = lambda phone_number: lambda wa, data: data.type == Mt.CONTACTS and (
-            isinstance(phone_number, str) and phone_number in
-            (p.phone for contact in data.contacts for p in contact.phones) or
-            isinstance(phone_number, Iterable) and
-            any((p.phone in phone_number for contact in data.contacts for p in contact.phones)))
-
-    """Filter for contacts messages that have the given phone number/s."""
-
-    HAS_WA: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.CONTACTS and \
-                                                         any((p.wa_id for p in
-                                                              (phone for contact in data.contacts for phone in
-                                                               contact.phones)))
+    HAS_WA: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.CONTACTS and (
+        any((p.wa_id for p in (phone for contact in m.contacts for phone in contact.phones)))
+    )
     """Filter for contacts messages that have a WhatsApp account."""
 
+    @staticmethod
+    def count(min_count: int, max_count: int) -> Callable[[Wa, Msg], bool]:
+        """Filter for contacts messages that have a number of contacts between min_count and max_count."""
+        return lambda wa, m: m.type == Mt.CONTACTS and min_count <= len(m.contacts) <= max_count
+
+    @staticmethod
+    def phone(*phones: str) -> Callable[[Wa, Msg], bool]:
+        """
+        Filter for contacts messages that have the given phone number/s.
+            * Pass only the numbers, without plus sign, spaces, etc.
+        """
+        return lambda wa, m: m.type == Mt.CONTACTS and (
+            any((re.sub(_ONLY_NUMS_RE, "", p.phone) in phones for contact in m.contacts for p in contact.phones))
+        )
+
 
-class UnsupportedFilter:
+class UnsupportedMsgFilter:
     """Useful filters for unsupported messages."""
 
-    ANY: Callable[[Wa, Msg], bool] = lambda wa, data: data.type == Mt.UNSUPPORTED
+    ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.UNSUPPORTED
     """Filter for all unsupported messages."""
 
 
 class CallbackFilter:
     """Useful filters for callback queries."""
 
-    DATA_EQUALS: Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]] \
-        = lambda data: lambda wa, data_: data_.data == data if isinstance(data, str) else any(
-        (data_.data == d for d in data))
-    """Filter for callbacks their data equals the given string/s."""
-
-    DATA_STARTS_WITH: Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]] \
-        = lambda data: lambda wa, data_: data_.data.startswith(data) if isinstance(data, str) else any(
-        (data_.data.startswith(d) for d in data))
-    """Filter for callbacks their data starts with the given string/s."""
-
-    DATA_ENDS_WITH: Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]] \
-        = lambda data: lambda wa, data_: data_.data.endswith(data) if isinstance(data, str) else any(
-        (data_.data.endswith(d) for d in data))
-    """Filter for callbacks their data ends with the given string/s."""
-
-    DATA_CONTAINS: Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]] \
-        = lambda data: lambda wa, data_: data in data_.data if isinstance(data, str) else any(
-        (d in data_.data for d in data))
-    """Filter for callbacks their data contains the given string/s."""
-
-    DATA_REGEX: Callable[[str | Iterable[str]], Callable[[Wa, CallbackButton | CallbackSelection], bool]] \
-        = lambda regex: lambda wa, data_: re.match(regex, data_.data) if isinstance(regex, str) else any(
-        (re.match(r, data_.data) for r in regex))
-    """Filter for callbacks their data matches the given regex/regexes."""
+    @staticmethod
+    def data_equals(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
+        """Filter for callbacks their data equals the given string/s."""
+        return lambda wa, c: any((c.data == m for m in matches))
+
+    @staticmethod
+    def data_starts_with(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
+        """Filter for callbacks their data starts with the given string/s."""
+        return lambda wa, c: any((c.data.startswith(m) for m in matches))
+
+    @staticmethod
+    def data_ends_with(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
+        """Filter for callbacks their data ends with the given string/s."""
+        return lambda wa, c: any((c.data.endswith(m) for m in matches))
+
+    @staticmethod
+    def data_contains(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
+        """Filter for callbacks their data contains the given string/s."""
+        return lambda wa, c: any((m in c.data for m in matches))
+
+    @staticmethod
+    def data_regex(*patterns: str | re.Pattern) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
+        """
+        Filter for callbacks their data matches the given regex/regexes.
+            * It's recommended to pass compiled regexes to save time (``re.compile(your_pattern)``)
+        """
+        return lambda wa, c: any((re.match(p, c.data) for p in patterns))
 
 
 class MessageStatusFilter:
     """Useful filters for message status updates."""
 
     SENT: Callable[[Wa, Ms], bool] = lambda wa, data: data.status == Mst.SENT
     """Filter for messages that have been sent."""
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py

```diff
@@ -27,33 +27,33 @@
 
 @dataclass(frozen=True, slots=True)
 class InlineButton:
     """
     Represents an inline button in a keyboard.
 
     Attributes:
-        title: The title of the button.
-        callback_data: The payload to send when the user clicks on the button.
+        title: The title of the button (up to 20 characters).
+        callback_data: The payload to send when the user clicks on the button (up to 256 characters).
     """
     title: str
     callback_data: str
 
     def to_dict(self) -> dict:
         return {"type": "reply", "reply": {"id": self.callback_data, "title": self.title}}
 
 
 @dataclass(frozen=True, slots=True)
 class SectionRow:
     """
     Represents a row in a section.
 
     Attributes:
-        title: The title of the row.
-        callback_data: The payload to send when the user clicks on the row.
-        description: The description of the row (optional).
+        title: The title of the row (up to 24 characters).
+        callback_data: The payload to send when the user clicks on the row (up to 200 characters).
+        description: The description of the row (optional, up to 72 characters).
     """
     title: str
     callback_data: str
     description: str | None = None
 
     def to_dict(self) -> dict:
         d = {"id": self.callback_data, "title": self.title}
@@ -87,15 +87,15 @@
 class SectionList:
     """
     Represents a section list in an interactive message.
 
     - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/reference/messages#section-object
 
     Attributes:
-        button_title: The title of the button that opens the section list.
+        button_title: The title of the button that opens the section list (up to 20 characters).
         sections: The sections in the section list (at least 1, no more than 10).
     """
     button_title: str
     sections: list[Section]
 
     def to_dict(self) -> dict:
         return {
@@ -430,16 +430,16 @@
         Reply to the message with text.
 
         Args:
             text: The text to reply with.
             preview_url: Whether to show a preview of the URL in the text (default: False).
             quote: Whether to quote the message (default: False).
             keyboard: The keyboard to send with the message (optional).
-            header: The header of the message (if keyboard is provided, optional).
-            footer: The footer of the message (if keyboard is provided, optional).
+            header: The header of the message (if keyboard is provided, optional, up to 60 characters, no markdown allowed).
+            footer: The footer of the message (if keyboard is provided, optional, up to 60 characters, markdown has no effect).
 
         Returns:
             The ID of the sent message.
         """
         return self._client.send_message(
             to=self.sender,
             text=text,
@@ -464,15 +464,15 @@
 
         Args:
             image: The image to reply with.
             caption: The caption of the image (optional).
             quote: Whether to quote the message (default: False).
             buttons: The buttons to send with the message (optional).
             body: The body of the message (if buttons is provided, optional).
-            footer: The footer of the message (if buttons is provided, optional).
+            footer: The footer of the message (if buttons is provided, optional, up to 60 characters, markdown has no effect).
 
         Returns:
             The ID of the sent message.
         """
         return self._client.send_image(
             to=self.sender,
             image=image,
@@ -497,15 +497,15 @@
 
         Args:
             video: The video to reply with.
             caption: The caption of the video (optional).
             quote: Whether to quote the message (default: False).
             buttons: The buttons to send with the message (optional).
             body: The body of the message (if buttons is provided, optional).
-            footer: The footer of the message (if buttons is provided, optional).
+            footer: The footer of the message (if buttons is provided, optional, up to 60 characters, markdown has no effect).
 
         Returns:
             The ID of the sent message.
         """
         return self._client.send_video(
             to=self.sender,
             video=video,
@@ -527,20 +527,20 @@
             footer: str | None = None,
     ) -> str:
         """
         Reply to the message with a document.
 
         Args:
             document: The document to reply with.
-            filename: The filename of the document (optional).
+            filename: The filename of the document (optional, The extension of the filename will specify what format the document is displayed as in WhatsApp).
             caption: The caption of the document (optional).
             quote: Whether to quote the message (default: False).
             buttons: The buttons to send with the message (optional).
             body: The body of the message (if buttons is provided, optional).
-            footer: The footer of the message (if buttons is provided, optional).
+            footer: The footer of the message (if buttons is provided, optional, up to 60 characters, markdown has no effect).
 
         Returns:
             The ID of the sent message.
         """
         return self._client.send_document(
             to=self.sender,
             document=document,
@@ -660,14 +660,41 @@
         """
         return self._client.send_reaction(
             to=self.sender,
             emoji=emoji,
             message_id=self.id
         )
 
+    def unreact(
+            self,
+    ) -> str:
+        """
+        Remove the reaction from the message.
+
+        Returns:
+            The ID of the sent message.
+        """
+        return self._client.remove_reaction(
+            to=self.sender,
+            message_id=self.id
+        )
+
+    def mark_as_read(
+            self
+    ) -> bool:
+        """
+        Mark the message as read.
+
+        Returns:
+            Whether it was successful.
+        """
+        return self._client.mark_message_as_read(
+            message_id=self.id
+        )
+
 
 @dataclass(frozen=True, slots=True)
 class Message(BaseUpdate):
     """
     A message received from a user.
 
     - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/webhooks/components#messages-object
```

