# Comparing `tmp/pywa-0.0.1rc3.linux-x86_64.tar.gz` & `tmp/pywa-0.0.1rc4.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywa-0.0.1rc3.linux-x86_64.tar", last modified: Thu Jun 22 16:52:53 2023, max compression
+gzip compressed data, was "pywa-0.0.1rc4.linux-x86_64.tar", last modified: Thu Jun 22 17:16:46 2023, max compression
```

## Comparing `pywa-0.0.1rc3.linux-x86_64.tar` & `pywa-0.0.1rc4.linux-x86_64.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/pywa/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/pywa/venv/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/pywa/venv/lib/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.927556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.951557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.931556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/
--rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-22 16:50:59.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.939556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/
--rw-rw-r--   0 david     (1000) david     (1000)      388 2023-06-22 16:52:53.931556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    10696 2023-06-22 16:52:53.935557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/api.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    26453 2023-06-22 16:52:53.939556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/client.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     1849 2023-06-22 16:52:53.935557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/errors.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    26796 2023-06-22 16:52:53.939556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/filters.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     3401 2023-06-22 16:52:53.939556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/handlers.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    41016 2023-06-22 16:52:53.935557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/types.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     2153 2023-06-22 16:52:53.931556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     6136 2023-06-22 16:52:53.931556 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/webhook.cpython-311.pyc
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.579762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/
+-rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-22 17:14:20.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.567762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/
+-rw-rw-r--   0 david     (1000) david     (1000)      388 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    10696 2023-06-22 17:16:46.563762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/api.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    25954 2023-06-22 17:16:46.567762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/client.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     1849 2023-06-22 17:16:46.563762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/errors.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    26788 2023-06-22 17:16:46.567762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/filters.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     3166 2023-06-22 17:16:46.567762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/handlers.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    41016 2023-06-22 17:16:46.563762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/types.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     2153 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     6136 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/webhook.cpython-311.pyc
 -rw-rw-r--   0 david     (1000) david     (1000)     7965 2023-06-22 15:59:56.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py
--rw-rw-r--   0 david     (1000) david     (1000)    23766 2023-06-22 15:59:56.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py
+-rw-rw-r--   0 david     (1000) david     (1000)    23198 2023-06-22 17:11:51.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py
 -rw-rw-r--   0 david     (1000) david     (1000)      989 2023-06-19 21:14:34.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/errors.py
--rw-rw-r--   0 david     (1000) david     (1000)    11023 2023-06-22 14:58:38.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py
--rw-rw-r--   0 david     (1000) david     (1000)     1656 2023-06-20 09:34:04.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11021 2023-06-22 17:14:20.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1431 2023-06-22 17:11:51.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py
 -rw-rw-r--   0 david     (1000) david     (1000)    25776 2023-06-22 15:59:56.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py
 -rw-rw-r--   0 david     (1000) david     (1000)      991 2023-06-20 16:58:34.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/utils.py
 -rw-rw-r--   0 david     (1000) david     (1000)     4141 2023-06-20 09:37:01.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/webhook.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 16:52:53.951557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    10028 2023-06-22 16:52:53.947557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      301 2023-06-22 16:52:53.951557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-22 16:52:53.947557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       51 2023-06-22 16:52:53.947557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        5 2023-06-22 16:52:53.947557 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.579762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     9996 2023-06-22 17:16:46.575762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      301 2023-06-22 17:16:46.579762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-22 17:16:46.575762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       51 2023-06-22 17:16:46.575762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        5 2023-06-22 17:16:46.575762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/top_level.txt
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Python wrapper for the WhatsApp Cloud API. https://github.com/david-lev/pywa"""
 
-__version__ = "0.0.1rc3"
+__version__ = "0.0.1rc4"
 
 from pywa.client import WhatsApp
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,35 +1,35 @@
 magic:    0xa70d0d0a
-moddate:  0xf37b9464 (Thu Jun 22 16:50:59 2023 UTC)
+moddate:  0x6c819464 (Thu Jun 22 17:14:20 2023 UTC)
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
    
-     3           6 LOAD_CONST               1 ('0.0.1rc3')
+     3           6 LOAD_CONST               1 ('0.0.1rc4')
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
-      '0.0.1rc3'
+      '0.0.1rc4'
       0
       ('WhatsApp',)
       None
    names      ('__doc__', '__version__', 'pywa.client', 'WhatsApp')
    varnames   ()
    freevars   ()
    cellvars   ()
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/client.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xfc6f9464 (Thu Jun 22 15:59:56 2023 UTC)
-files sz: 23766
+moddate:  0xd7809464 (Thu Jun 22 17:11:51 2023 UTC)
+files sz: 23198
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a036d
@@ -109,49 +109,42 @@
          nlocals   : 0
          stacksize : 18
          flags     : 0
          code
             0x970065005a0164005a02090009000900090009000900643b6405650365
             047a070000640665036407650564017a070000640865036409650364017a
             070000640a6503640b6506640c65076a08000000000000000064017a0700
-            006610640d84055a09640e650a6602640f84045a0b0900643c6410650c65
-            0d6400650e6702650f660219000000000000000000190000000000000000
-            00650d6400650e6702650f6602190000000000000000007a070000660264
-            1184055a100900643c6410650c650d640065116702650f66021900000000
-            000000000019000000000000000000650d640065116702650f6602190000
-            000000000000007a0700006602641284055a120900643c6410650c650d64
-            0065136702650f6602190000000000000000001900000000000000000065
-            0d640065136702650f6602190000000000000000007a0700006602641384
-            055a140900643c6410650c650d640065156702650f660219000000000000
-            00000019000000000000000000650d640065156702650f66021900000000
-            00000000007a0700006602641484055a160900643c6410650c650d640065
-            176702650f66021900000000000000000019000000000000000000650d64
-            0065176702650f6602190000000000000000007a0700006602641584055a
-            1809000900090009000900643d64176503641865036419650f641a650364
-            017a070000641b6519651a19000000000000000000651b7a07000064017a
+            006610640d84055a09640e650a6602640f84045a0b6410650c6400650d67
+            02650e6602190000000000000000006602641184045a0f6410650c640065
+            106702650e6602190000000000000000006602641284045a116410650c64
+            0065126702650e6602190000000000000000006602641384045a13641065
+            0c640065146702650e6602190000000000000000006602641484045a1564
+            10650c640065166702650e6602190000000000000000006602641584045a
+            1709000900090009000900643c64176503641865036419650e641a650364
+            017a070000641b6518651919000000000000000000651a7a07000064017a
             070000641c650364017a070000641d650364017a070000641e6503661064
-            1f84055a1c09000900090009000900643e6417650364206503651d7a0700
-            006421650364017a070000641a650364017a07000064226519651a190000
+            1f84055a1b09000900090009000900643d6417650364206503651c7a0700
+            006421650364017a070000641a650364017a070000642265186519190000
             0000000000000064017a0700006423650364017a070000641d650364017a
-            070000641e65036610642484055a1e09000900090009000900643e641765
-            0364256503651d7a0700006421650364017a070000641a650364017a0700
-            0064226519651a1900000000000000000064017a0700006423650364017a
-            070000641d650364017a070000641e65036610642684055a1f0900090009
-            00090009000900643f6417650364276503651d7a0700006428650364017a
-            0700006421650364017a070000641a650364017a07000064226519651a19
+            070000641e65036610642484055a1d09000900090009000900643d641765
+            0364256503651c7a0700006421650364017a070000641a650364017a0700
+            006422651865191900000000000000000064017a0700006423650364017a
+            070000641d650364017a070000641e65036610642684055a1e0900090009
+            00090009000900643e6417650364276503651c7a0700006428650364017a
+            0700006421650364017a070000641a650364017a07000064226518651919
             00000000000000000064017a0700006423650364017a070000641d650364
-            017a0700006610642984055a200900643c64176503642a6503651d7a0700
-            00641a650364017a070000641e65036608642b84055a2109000900644064
-            176503642c6503651d7a070000642d650f641a650364017a070000641e65
-            03660a642e84055a2264176503642f650364306503641e65036608643184
-            045a236417650364306503641e65036606643284045a2409000900644164
+            017a0700006610642984055a1f0900643f64176503642a6503651c7a0700
+            00641a650364017a070000641e65036608642b84055a2009000900644064
+            176503642c6503651c7a070000642d650e641a650364017a070000641e65
+            03660a642e84055a2164176503642f650364306503641e65036608643184
+            045a226417650364306503641e65036606643284045a2309000900644164
             17650364336506643465066435650364017a0700006436650364017a0700
-            00641e6503660c643784055a250900643c6417650364386526650c652619
+            00641e6503660c643784055a240900643f64176503643865256526652519
             0000000000000000007a070000641a650364017a070000641e6503660864
-            3984055a2764306503641e650f6604643a84045a2864015300
+            3984055a2764306503641e650e6604643a84045a2864015300
           11           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('WhatsApp')
                        8 STORE_NAME               2 (__qualname__)
          
           16          10 NOP
@@ -216,594 +209,511 @@
           60          98 LOAD_CONST              14 ('handler')
                      100 LOAD_NAME               10 (Handler)
                      102 BUILD_TUPLE              2
                      104 LOAD_CONST              15 (<code object add_handler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 60>)
                      106 MAKE_FUNCTION            4 (annotations)
                      108 STORE_NAME              11 (add_handler)
          
-          67         110 NOP
+          65         110 LOAD_CONST              16 ('filters')
+                     112 LOAD_NAME               12 (Callable)
+                     114 LOAD_CONST               0 ('WhatsApp')
+                     116 LOAD_NAME               13 (dict)
+                     118 BUILD_LIST               2
+                     120 LOAD_NAME               14 (bool)
+                     122 BUILD_TUPLE              2
+                     124 BINARY_SUBSCR
+                     134 BUILD_TUPLE              2
+                     136 LOAD_CONST              17 (<code object on_raw_update, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 65>)
+                     138 MAKE_FUNCTION            4 (annotations)
+                     140 STORE_NAME              15 (on_raw_update)
+         
+          84         142 LOAD_CONST              16 ('filters')
+                     144 LOAD_NAME               12 (Callable)
+                     146 LOAD_CONST               0 ('WhatsApp')
+                     148 LOAD_NAME               16 (Message)
+                     150 BUILD_LIST               2
+                     152 LOAD_NAME               14 (bool)
+                     154 BUILD_TUPLE              2
+                     156 BINARY_SUBSCR
+                     166 BUILD_TUPLE              2
+                     168 LOAD_CONST              18 (<code object on_message, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 84>)
+                     170 MAKE_FUNCTION            4 (annotations)
+                     172 STORE_NAME              17 (on_message)
+         
+         103         174 LOAD_CONST              16 ('filters')
+                     176 LOAD_NAME               12 (Callable)
+                     178 LOAD_CONST               0 ('WhatsApp')
+                     180 LOAD_NAME               18 (CallbackButton)
+                     182 BUILD_LIST               2
+                     184 LOAD_NAME               14 (bool)
+                     186 BUILD_TUPLE              2
+                     188 BINARY_SUBSCR
+                     198 BUILD_TUPLE              2
+                     200 LOAD_CONST              19 (<code object on_callback_button, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 103>)
+                     202 MAKE_FUNCTION            4 (annotations)
+                     204 STORE_NAME              19 (on_callback_button)
+         
+         122         206 LOAD_CONST              16 ('filters')
+                     208 LOAD_NAME               12 (Callable)
+                     210 LOAD_CONST               0 ('WhatsApp')
+                     212 LOAD_NAME               20 (CallbackSelection)
+                     214 BUILD_LIST               2
+                     216 LOAD_NAME               14 (bool)
+                     218 BUILD_TUPLE              2
+                     220 BINARY_SUBSCR
+                     230 BUILD_TUPLE              2
+                     232 LOAD_CONST              20 (<code object on_callback_selection, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 122>)
+                     234 MAKE_FUNCTION            4 (annotations)
+                     236 STORE_NAME              21 (on_callback_selection)
+         
+         141         238 LOAD_CONST              16 ('filters')
+                     240 LOAD_NAME               12 (Callable)
+                     242 LOAD_CONST               0 ('WhatsApp')
+                     244 LOAD_NAME               22 (MessageStatus)
+                     246 BUILD_LIST               2
+                     248 LOAD_NAME               14 (bool)
+                     250 BUILD_TUPLE              2
+                     252 BINARY_SUBSCR
+                     262 BUILD_TUPLE              2
+                     264 LOAD_CONST              21 (<code object on_message_status_change, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 141>)
+                     266 MAKE_FUNCTION            4 (annotations)
+                     268 STORE_NAME              23 (on_message_status_change)
+         
+         164         270 NOP
+         
+         165         272 NOP
+         
+         166         274 NOP
+         
+         167         276 NOP
+         
+         168         278 NOP
+         
+         160         280 LOAD_CONST              60 ((False, None, None, None, None))
+                     282 LOAD_CONST              23 ('to')
+         
+         162         284 LOAD_NAME                3 (str)
+         
+         160         286 LOAD_CONST              24 ('text')
+         
+         163         288 LOAD_NAME                3 (str)
+         
+         160         290 LOAD_CONST              25 ('preview_url')
+         
+         164         292 LOAD_NAME               14 (bool)
+         
+         160         294 LOAD_CONST              26 ('reply_to_message_id')
+         
+         165         296 LOAD_NAME                3 (str)
+                     298 LOAD_CONST               1 (None)
+                     300 BINARY_OP                7 (|)
          
-          65         112 LOAD_CONST              60 ((None,))
-                     114 LOAD_CONST              16 ('filters')
+         160         304 LOAD_CONST              27 ('keyboard')
          
-          67         116 LOAD_NAME               12 (Iterable)
-                     118 LOAD_NAME               13 (Callable)
-                     120 LOAD_CONST               0 ('WhatsApp')
-                     122 LOAD_NAME               14 (dict)
-                     124 BUILD_LIST               2
-                     126 LOAD_NAME               15 (bool)
-                     128 BUILD_TUPLE              2
-                     130 BINARY_SUBSCR
-                     140 BINARY_SUBSCR
-                     150 LOAD_NAME               13 (Callable)
-                     152 LOAD_CONST               0 ('WhatsApp')
-                     154 LOAD_NAME               14 (dict)
-                     156 BUILD_LIST               2
-                     158 LOAD_NAME               15 (bool)
-                     160 BUILD_TUPLE              2
-                     162 BINARY_SUBSCR
-                     172 BINARY_OP                7 (|)
-         
-          65         176 BUILD_TUPLE              2
-                     178 LOAD_CONST              17 (<code object on_raw_update, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 65>)
-                     180 MAKE_FUNCTION            5 (defaults, annotations)
-                     182 STORE_NAME              16 (on_raw_update)
-         
-          90         184 NOP
-         
-          87         186 LOAD_CONST              60 ((None,))
-                     188 LOAD_CONST              16 ('filters')
-         
-          89         190 LOAD_NAME               12 (Iterable)
-                     192 LOAD_NAME               13 (Callable)
-                     194 LOAD_CONST               0 ('WhatsApp')
-                     196 LOAD_NAME               17 (Message)
-                     198 BUILD_LIST               2
-                     200 LOAD_NAME               15 (bool)
-                     202 BUILD_TUPLE              2
-                     204 BINARY_SUBSCR
-                     214 BINARY_SUBSCR
-         
-          90         224 LOAD_NAME               13 (Callable)
-                     226 LOAD_CONST               0 ('WhatsApp')
-                     228 LOAD_NAME               17 (Message)
-                     230 BUILD_LIST               2
-                     232 LOAD_NAME               15 (bool)
-                     234 BUILD_TUPLE              2
-                     236 BINARY_SUBSCR
-         
-          89         246 BINARY_OP                7 (|)
-         
-          87         250 BUILD_TUPLE              2
-                     252 LOAD_CONST              18 (<code object on_message, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 87>)
-                     254 MAKE_FUNCTION            5 (defaults, annotations)
-                     256 STORE_NAME              18 (on_message)
-         
-         114         258 NOP
-         
-         111         260 LOAD_CONST              60 ((None,))
-                     262 LOAD_CONST              16 ('filters')
-         
-         113         264 LOAD_NAME               12 (Iterable)
-                     266 LOAD_NAME               13 (Callable)
-                     268 LOAD_CONST               0 ('WhatsApp')
-                     270 LOAD_NAME               19 (CallbackButton)
-                     272 BUILD_LIST               2
-                     274 LOAD_NAME               15 (bool)
-                     276 BUILD_TUPLE              2
-                     278 BINARY_SUBSCR
-                     288 BINARY_SUBSCR
-         
-         114         298 LOAD_NAME               13 (Callable)
-                     300 LOAD_CONST               0 ('WhatsApp')
-                     302 LOAD_NAME               19 (CallbackButton)
-                     304 BUILD_LIST               2
-                     306 LOAD_NAME               15 (bool)
-                     308 BUILD_TUPLE              2
+         166         306 LOAD_NAME               24 (list)
+                     308 LOAD_NAME               25 (InlineButton)
                      310 BINARY_SUBSCR
+                     320 LOAD_NAME               26 (SectionList)
+                     322 BINARY_OP                7 (|)
+                     326 LOAD_CONST               1 (None)
+                     328 BINARY_OP                7 (|)
          
-         113         320 BINARY_OP                7 (|)
+         160         332 LOAD_CONST              28 ('header')
          
-         111         324 BUILD_TUPLE              2
-                     326 LOAD_CONST              19 (<code object on_callback_button, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 111>)
-                     328 MAKE_FUNCTION            5 (defaults, annotations)
-                     330 STORE_NAME              20 (on_callback_button)
+         167         334 LOAD_NAME                3 (str)
+                     336 LOAD_CONST               1 (None)
+                     338 BINARY_OP                7 (|)
          
-         137         332 NOP
+         160         342 LOAD_CONST              29 ('footer')
          
-         134         334 LOAD_CONST              60 ((None,))
-                     336 LOAD_CONST              16 ('filters')
+         168         344 LOAD_NAME                3 (str)
+                     346 LOAD_CONST               1 (None)
+                     348 BINARY_OP                7 (|)
          
-         136         338 LOAD_NAME               12 (Iterable)
-                     340 LOAD_NAME               13 (Callable)
-                     342 LOAD_CONST               0 ('WhatsApp')
-                     344 LOAD_NAME               21 (CallbackSelection)
-                     346 BUILD_LIST               2
-                     348 LOAD_NAME               15 (bool)
-                     350 BUILD_TUPLE              2
-                     352 BINARY_SUBSCR
-                     362 BINARY_SUBSCR
+         160         352 LOAD_CONST              30 ('return')
          
-         137         372 LOAD_NAME               13 (Callable)
-                     374 LOAD_CONST               0 ('WhatsApp')
-                     376 LOAD_NAME               21 (CallbackSelection)
-                     378 BUILD_LIST               2
-                     380 LOAD_NAME               15 (bool)
-                     382 BUILD_TUPLE              2
-                     384 BINARY_SUBSCR
+         169         354 LOAD_NAME                3 (str)
          
-         136         394 BINARY_OP                7 (|)
+         160         356 BUILD_TUPLE             16
+                     358 LOAD_CONST              31 (<code object send_message, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 160>)
+                     360 MAKE_FUNCTION            5 (defaults, annotations)
+                     362 STORE_NAME              27 (send_message)
          
-         134         398 BUILD_TUPLE              2
-                     400 LOAD_CONST              20 (<code object on_callback_selection, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 134>)
-                     402 MAKE_FUNCTION            5 (defaults, annotations)
-                     404 STORE_NAME              22 (on_callback_selection)
+         268         364 NOP
          
-         160         406 NOP
+         269         366 NOP
          
-         157         408 LOAD_CONST              60 ((None,))
-                     410 LOAD_CONST              16 ('filters')
+         270         368 NOP
          
-         159         412 LOAD_NAME               12 (Iterable)
-                     414 LOAD_NAME               13 (Callable)
-                     416 LOAD_CONST               0 ('WhatsApp')
-                     418 LOAD_NAME               23 (MessageStatus)
-                     420 BUILD_LIST               2
-                     422 LOAD_NAME               15 (bool)
-                     424 BUILD_TUPLE              2
-                     426 BINARY_SUBSCR
-                     436 BINARY_SUBSCR
+         271         370 NOP
          
-         160         446 LOAD_NAME               13 (Callable)
-                     448 LOAD_CONST               0 ('WhatsApp')
-                     450 LOAD_NAME               23 (MessageStatus)
-                     452 BUILD_LIST               2
-                     454 LOAD_NAME               15 (bool)
-                     456 BUILD_TUPLE              2
-                     458 BINARY_SUBSCR
+         272         372 NOP
          
-         159         468 BINARY_OP                7 (|)
+         264         374 LOAD_CONST              61 ((None, None, None, None, None))
+                     376 LOAD_CONST              23 ('to')
          
-         157         472 BUILD_TUPLE              2
-                     474 LOAD_CONST              21 (<code object on_message_status_change, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 157>)
-                     476 MAKE_FUNCTION            5 (defaults, annotations)
-                     478 STORE_NAME              24 (on_message_status_change)
+         266         378 LOAD_NAME                3 (str)
          
-         184         480 NOP
+         264         380 LOAD_CONST              32 ('image')
          
-         185         482 NOP
+         267         382 LOAD_NAME                3 (str)
+                     384 LOAD_NAME               28 (bytes)
+                     386 BINARY_OP                7 (|)
          
-         186         484 NOP
+         264         390 LOAD_CONST              33 ('caption')
          
-         187         486 NOP
+         268         392 LOAD_NAME                3 (str)
+                     394 LOAD_CONST               1 (None)
+                     396 BINARY_OP                7 (|)
          
-         188         488 NOP
+         264         400 LOAD_CONST              26 ('reply_to_message_id')
          
-         180         490 LOAD_CONST              61 ((False, None, None, None, None))
-                     492 LOAD_CONST              23 ('to')
+         269         402 LOAD_NAME                3 (str)
+                     404 LOAD_CONST               1 (None)
+                     406 BINARY_OP                7 (|)
          
-         182         494 LOAD_NAME                3 (str)
+         264         410 LOAD_CONST              34 ('buttons')
          
-         180         496 LOAD_CONST              24 ('text')
+         270         412 LOAD_NAME               24 (list)
+                     414 LOAD_NAME               25 (InlineButton)
+                     416 BINARY_SUBSCR
+                     426 LOAD_CONST               1 (None)
+                     428 BINARY_OP                7 (|)
          
-         183         498 LOAD_NAME                3 (str)
+         264         432 LOAD_CONST              35 ('body')
          
-         180         500 LOAD_CONST              25 ('preview_url')
+         271         434 LOAD_NAME                3 (str)
+                     436 LOAD_CONST               1 (None)
+                     438 BINARY_OP                7 (|)
          
-         184         502 LOAD_NAME               15 (bool)
+         264         442 LOAD_CONST              29 ('footer')
          
-         180         504 LOAD_CONST              26 ('reply_to_message_id')
+         272         444 LOAD_NAME                3 (str)
+                     446 LOAD_CONST               1 (None)
+                     448 BINARY_OP                7 (|)
          
-         185         506 LOAD_NAME                3 (str)
-                     508 LOAD_CONST               1 (None)
-                     510 BINARY_OP                7 (|)
+         264         452 LOAD_CONST              30 ('return')
          
-         180         514 LOAD_CONST              27 ('keyboard')
+         273         454 LOAD_NAME                3 (str)
          
-         186         516 LOAD_NAME               25 (list)
-                     518 LOAD_NAME               26 (InlineButton)
-                     520 BINARY_SUBSCR
-                     530 LOAD_NAME               27 (SectionList)
-                     532 BINARY_OP                7 (|)
-                     536 LOAD_CONST               1 (None)
-                     538 BINARY_OP                7 (|)
-         
-         180         542 LOAD_CONST              28 ('header')
-         
-         187         544 LOAD_NAME                3 (str)
-                     546 LOAD_CONST               1 (None)
-                     548 BINARY_OP                7 (|)
-         
-         180         552 LOAD_CONST              29 ('footer')
-         
-         188         554 LOAD_NAME                3 (str)
-                     556 LOAD_CONST               1 (None)
-                     558 BINARY_OP                7 (|)
-         
-         180         562 LOAD_CONST              30 ('return')
-         
-         189         564 LOAD_NAME                3 (str)
-         
-         180         566 BUILD_TUPLE             16
-                     568 LOAD_CONST              31 (<code object send_message, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 180>)
-                     570 MAKE_FUNCTION            5 (defaults, annotations)
-                     572 STORE_NAME              28 (send_message)
-         
-         288         574 NOP
-         
-         289         576 NOP
+         264         456 BUILD_TUPLE             16
+                     458 LOAD_CONST              36 (<code object send_image, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 264>)
+                     460 MAKE_FUNCTION            5 (defaults, annotations)
+                     462 STORE_NAME              29 (send_image)
          
-         290         578 NOP
+         325         464 NOP
          
-         291         580 NOP
+         326         466 NOP
          
-         292         582 NOP
+         327         468 NOP
          
-         284         584 LOAD_CONST              62 ((None, None, None, None, None))
-                     586 LOAD_CONST              23 ('to')
+         328         470 NOP
          
-         286         588 LOAD_NAME                3 (str)
+         329         472 NOP
          
-         284         590 LOAD_CONST              32 ('image')
+         321         474 LOAD_CONST              61 ((None, None, None, None, None))
+                     476 LOAD_CONST              23 ('to')
          
-         287         592 LOAD_NAME                3 (str)
-                     594 LOAD_NAME               29 (bytes)
-                     596 BINARY_OP                7 (|)
+         323         478 LOAD_NAME                3 (str)
          
-         284         600 LOAD_CONST              33 ('caption')
+         321         480 LOAD_CONST              37 ('video')
          
-         288         602 LOAD_NAME                3 (str)
-                     604 LOAD_CONST               1 (None)
-                     606 BINARY_OP                7 (|)
+         324         482 LOAD_NAME                3 (str)
+                     484 LOAD_NAME               28 (bytes)
+                     486 BINARY_OP                7 (|)
          
-         284         610 LOAD_CONST              26 ('reply_to_message_id')
+         321         490 LOAD_CONST              33 ('caption')
          
-         289         612 LOAD_NAME                3 (str)
-                     614 LOAD_CONST               1 (None)
-                     616 BINARY_OP                7 (|)
+         325         492 LOAD_NAME                3 (str)
+                     494 LOAD_CONST               1 (None)
+                     496 BINARY_OP                7 (|)
          
-         284         620 LOAD_CONST              34 ('buttons')
+         321         500 LOAD_CONST              26 ('reply_to_message_id')
          
-         290         622 LOAD_NAME               25 (list)
-                     624 LOAD_NAME               26 (InlineButton)
-                     626 BINARY_SUBSCR
-                     636 LOAD_CONST               1 (None)
-                     638 BINARY_OP                7 (|)
+         326         502 LOAD_NAME                3 (str)
+                     504 LOAD_CONST               1 (None)
+                     506 BINARY_OP                7 (|)
          
-         284         642 LOAD_CONST              35 ('body')
+         321         510 LOAD_CONST              34 ('buttons')
          
-         291         644 LOAD_NAME                3 (str)
-                     646 LOAD_CONST               1 (None)
-                     648 BINARY_OP                7 (|)
+         327         512 LOAD_NAME               24 (list)
+                     514 LOAD_NAME               25 (InlineButton)
+                     516 BINARY_SUBSCR
+                     526 LOAD_CONST               1 (None)
+                     528 BINARY_OP                7 (|)
          
-         284         652 LOAD_CONST              29 ('footer')
+         321         532 LOAD_CONST              35 ('body')
          
-         292         654 LOAD_NAME                3 (str)
-                     656 LOAD_CONST               1 (None)
-                     658 BINARY_OP                7 (|)
-         
-         284         662 LOAD_CONST              30 ('return')
-         
-         293         664 LOAD_NAME                3 (str)
-         
-         284         666 BUILD_TUPLE             16
-                     668 LOAD_CONST              36 (<code object send_image, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 284>)
-                     670 MAKE_FUNCTION            5 (defaults, annotations)
-                     672 STORE_NAME              30 (send_image)
-         
-         345         674 NOP
-         
-         346         676 NOP
-         
-         347         678 NOP
-         
-         348         680 NOP
-         
-         349         682 NOP
-         
-         341         684 LOAD_CONST              62 ((None, None, None, None, None))
-                     686 LOAD_CONST              23 ('to')
-         
-         343         688 LOAD_NAME                3 (str)
-         
-         341         690 LOAD_CONST              37 ('video')
-         
-         344         692 LOAD_NAME                3 (str)
-                     694 LOAD_NAME               29 (bytes)
-                     696 BINARY_OP                7 (|)
-         
-         341         700 LOAD_CONST              33 ('caption')
-         
-         345         702 LOAD_NAME                3 (str)
-                     704 LOAD_CONST               1 (None)
-                     706 BINARY_OP                7 (|)
-         
-         341         710 LOAD_CONST              26 ('reply_to_message_id')
-         
-         346         712 LOAD_NAME                3 (str)
-                     714 LOAD_CONST               1 (None)
-                     716 BINARY_OP                7 (|)
-         
-         341         720 LOAD_CONST              34 ('buttons')
-         
-         347         722 LOAD_NAME               25 (list)
-                     724 LOAD_NAME               26 (InlineButton)
-                     726 BINARY_SUBSCR
-                     736 LOAD_CONST               1 (None)
-                     738 BINARY_OP                7 (|)
-         
-         341         742 LOAD_CONST              35 ('body')
-         
-         348         744 LOAD_NAME                3 (str)
-                     746 LOAD_CONST               1 (None)
-                     748 BINARY_OP                7 (|)
+         328         534 LOAD_NAME                3 (str)
+                     536 LOAD_CONST               1 (None)
+                     538 BINARY_OP                7 (|)
          
-         341         752 LOAD_CONST              29 ('footer')
+         321         542 LOAD_CONST              29 ('footer')
          
-         349         754 LOAD_NAME                3 (str)
-                     756 LOAD_CONST               1 (None)
-                     758 BINARY_OP                7 (|)
+         329         544 LOAD_NAME                3 (str)
+                     546 LOAD_CONST               1 (None)
+                     548 BINARY_OP                7 (|)
          
-         341         762 LOAD_CONST              30 ('return')
+         321         552 LOAD_CONST              30 ('return')
          
-         350         764 LOAD_NAME                3 (str)
+         330         554 LOAD_NAME                3 (str)
          
-         341         766 BUILD_TUPLE             16
-                     768 LOAD_CONST              38 (<code object send_video, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 341>)
-                     770 MAKE_FUNCTION            5 (defaults, annotations)
-                     772 STORE_NAME              31 (send_video)
+         321         556 BUILD_TUPLE             16
+                     558 LOAD_CONST              38 (<code object send_video, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 321>)
+                     560 MAKE_FUNCTION            5 (defaults, annotations)
+                     562 STORE_NAME              30 (send_video)
          
-         402         774 NOP
+         382         564 NOP
          
-         403         776 NOP
+         383         566 NOP
          
-         404         778 NOP
+         384         568 NOP
          
-         405         780 NOP
+         385         570 NOP
          
-         406         782 NOP
+         386         572 NOP
          
-         407         784 NOP
+         387         574 NOP
          
-         398         786 LOAD_CONST              63 ((None, None, None, None, None, None))
-                     788 LOAD_CONST              23 ('to')
+         378         576 LOAD_CONST              62 ((None, None, None, None, None, None))
+                     578 LOAD_CONST              23 ('to')
          
-         400         790 LOAD_NAME                3 (str)
+         380         580 LOAD_NAME                3 (str)
          
-         398         792 LOAD_CONST              39 ('document')
+         378         582 LOAD_CONST              39 ('document')
          
-         401         794 LOAD_NAME                3 (str)
-                     796 LOAD_NAME               29 (bytes)
-                     798 BINARY_OP                7 (|)
+         381         584 LOAD_NAME                3 (str)
+                     586 LOAD_NAME               28 (bytes)
+                     588 BINARY_OP                7 (|)
          
-         398         802 LOAD_CONST              40 ('filename')
+         378         592 LOAD_CONST              40 ('filename')
          
-         402         804 LOAD_NAME                3 (str)
-                     806 LOAD_CONST               1 (None)
-                     808 BINARY_OP                7 (|)
+         382         594 LOAD_NAME                3 (str)
+                     596 LOAD_CONST               1 (None)
+                     598 BINARY_OP                7 (|)
          
-         398         812 LOAD_CONST              33 ('caption')
+         378         602 LOAD_CONST              33 ('caption')
          
-         403         814 LOAD_NAME                3 (str)
-                     816 LOAD_CONST               1 (None)
-                     818 BINARY_OP                7 (|)
+         383         604 LOAD_NAME                3 (str)
+                     606 LOAD_CONST               1 (None)
+                     608 BINARY_OP                7 (|)
          
-         398         822 LOAD_CONST              26 ('reply_to_message_id')
+         378         612 LOAD_CONST              26 ('reply_to_message_id')
          
-         404         824 LOAD_NAME                3 (str)
-                     826 LOAD_CONST               1 (None)
-                     828 BINARY_OP                7 (|)
+         384         614 LOAD_NAME                3 (str)
+                     616 LOAD_CONST               1 (None)
+                     618 BINARY_OP                7 (|)
          
-         398         832 LOAD_CONST              34 ('buttons')
+         378         622 LOAD_CONST              34 ('buttons')
          
-         405         834 LOAD_NAME               25 (list)
-                     836 LOAD_NAME               26 (InlineButton)
-                     838 BINARY_SUBSCR
-                     848 LOAD_CONST               1 (None)
-                     850 BINARY_OP                7 (|)
+         385         624 LOAD_NAME               24 (list)
+                     626 LOAD_NAME               25 (InlineButton)
+                     628 BINARY_SUBSCR
+                     638 LOAD_CONST               1 (None)
+                     640 BINARY_OP                7 (|)
          
-         398         854 LOAD_CONST              35 ('body')
+         378         644 LOAD_CONST              35 ('body')
          
-         406         856 LOAD_NAME                3 (str)
-                     858 LOAD_CONST               1 (None)
-                     860 BINARY_OP                7 (|)
+         386         646 LOAD_NAME                3 (str)
+                     648 LOAD_CONST               1 (None)
+                     650 BINARY_OP                7 (|)
          
-         398         864 LOAD_CONST              29 ('footer')
+         378         654 LOAD_CONST              29 ('footer')
          
-         407         866 LOAD_NAME                3 (str)
-                     868 LOAD_CONST               1 (None)
-                     870 BINARY_OP                7 (|)
+         387         656 LOAD_NAME                3 (str)
+                     658 LOAD_CONST               1 (None)
+                     660 BINARY_OP                7 (|)
          
-         398         874 BUILD_TUPLE             16
-                     876 LOAD_CONST              41 (<code object send_document, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 398>)
-                     878 MAKE_FUNCTION            5 (defaults, annotations)
-                     880 STORE_NAME              32 (send_document)
+         378         664 BUILD_TUPLE             16
+                     666 LOAD_CONST              41 (<code object send_document, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 378>)
+                     668 MAKE_FUNCTION            5 (defaults, annotations)
+                     670 STORE_NAME              31 (send_document)
          
-         465         882 NOP
+         445         672 NOP
          
-         461         884 LOAD_CONST              60 ((None,))
-                     886 LOAD_CONST              23 ('to')
+         441         674 LOAD_CONST              63 ((None,))
+                     676 LOAD_CONST              23 ('to')
          
-         463         888 LOAD_NAME                3 (str)
+         443         678 LOAD_NAME                3 (str)
          
-         461         890 LOAD_CONST              42 ('audio')
+         441         680 LOAD_CONST              42 ('audio')
          
-         464         892 LOAD_NAME                3 (str)
-                     894 LOAD_NAME               29 (bytes)
-                     896 BINARY_OP                7 (|)
+         444         682 LOAD_NAME                3 (str)
+                     684 LOAD_NAME               28 (bytes)
+                     686 BINARY_OP                7 (|)
          
-         461         900 LOAD_CONST              26 ('reply_to_message_id')
+         441         690 LOAD_CONST              26 ('reply_to_message_id')
          
-         465         902 LOAD_NAME                3 (str)
-                     904 LOAD_CONST               1 (None)
-                     906 BINARY_OP                7 (|)
+         445         692 LOAD_NAME                3 (str)
+                     694 LOAD_CONST               1 (None)
+                     696 BINARY_OP                7 (|)
          
-         461         910 LOAD_CONST              30 ('return')
+         441         700 LOAD_CONST              30 ('return')
          
-         466         912 LOAD_NAME                3 (str)
+         446         702 LOAD_NAME                3 (str)
          
-         461         914 BUILD_TUPLE              8
-                     916 LOAD_CONST              43 (<code object send_audio, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 461>)
-                     918 MAKE_FUNCTION            5 (defaults, annotations)
-                     920 STORE_NAME              33 (send_audio)
+         441         704 BUILD_TUPLE              8
+                     706 LOAD_CONST              43 (<code object send_audio, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 441>)
+                     708 MAKE_FUNCTION            5 (defaults, annotations)
+                     710 STORE_NAME              32 (send_audio)
          
-         496         922 NOP
+         476         712 NOP
          
-         497         924 NOP
+         477         714 NOP
          
-         492         926 LOAD_CONST              64 ((False, None))
-                     928 LOAD_CONST              23 ('to')
+         472         716 LOAD_CONST              64 ((False, None))
+                     718 LOAD_CONST              23 ('to')
          
-         494         930 LOAD_NAME                3 (str)
+         474         720 LOAD_NAME                3 (str)
          
-         492         932 LOAD_CONST              44 ('sticker')
+         472         722 LOAD_CONST              44 ('sticker')
          
-         495         934 LOAD_NAME                3 (str)
-                     936 LOAD_NAME               29 (bytes)
-                     938 BINARY_OP                7 (|)
+         475         724 LOAD_NAME                3 (str)
+                     726 LOAD_NAME               28 (bytes)
+                     728 BINARY_OP                7 (|)
          
-         492         942 LOAD_CONST              45 ('animated')
+         472         732 LOAD_CONST              45 ('animated')
          
-         496         944 LOAD_NAME               15 (bool)
+         476         734 LOAD_NAME               14 (bool)
          
-         492         946 LOAD_CONST              26 ('reply_to_message_id')
+         472         736 LOAD_CONST              26 ('reply_to_message_id')
          
-         497         948 LOAD_NAME                3 (str)
-                     950 LOAD_CONST               1 (None)
-                     952 BINARY_OP                7 (|)
+         477         738 LOAD_NAME                3 (str)
+                     740 LOAD_CONST               1 (None)
+                     742 BINARY_OP                7 (|)
          
-         492         956 LOAD_CONST              30 ('return')
+         472         746 LOAD_CONST              30 ('return')
          
-         498         958 LOAD_NAME                3 (str)
+         478         748 LOAD_NAME                3 (str)
          
-         492         960 BUILD_TUPLE             10
-                     962 LOAD_CONST              46 (<code object send_sticker, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 492>)
-                     964 MAKE_FUNCTION            5 (defaults, annotations)
-                     966 STORE_NAME              34 (send_sticker)
+         472         750 BUILD_TUPLE             10
+                     752 LOAD_CONST              46 (<code object send_sticker, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 472>)
+                     754 MAKE_FUNCTION            5 (defaults, annotations)
+                     756 STORE_NAME              33 (send_sticker)
          
-         528         968 LOAD_CONST              23 ('to')
+         508         758 LOAD_CONST              23 ('to')
          
-         530         970 LOAD_NAME                3 (str)
+         510         760 LOAD_NAME                3 (str)
          
-         528         972 LOAD_CONST              47 ('emoji')
+         508         762 LOAD_CONST              47 ('emoji')
          
-         531         974 LOAD_NAME                3 (str)
+         511         764 LOAD_NAME                3 (str)
          
-         528         976 LOAD_CONST              48 ('message_id')
+         508         766 LOAD_CONST              48 ('message_id')
          
-         532         978 LOAD_NAME                3 (str)
+         512         768 LOAD_NAME                3 (str)
          
-         528         980 LOAD_CONST              30 ('return')
+         508         770 LOAD_CONST              30 ('return')
          
-         533         982 LOAD_NAME                3 (str)
+         513         772 LOAD_NAME                3 (str)
          
-         528         984 BUILD_TUPLE              8
-                     986 LOAD_CONST              49 (<code object send_reaction, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 528>)
-                     988 MAKE_FUNCTION            4 (annotations)
-                     990 STORE_NAME              35 (send_reaction)
+         508         774 BUILD_TUPLE              8
+                     776 LOAD_CONST              49 (<code object send_reaction, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 508>)
+                     778 MAKE_FUNCTION            4 (annotations)
+                     780 STORE_NAME              34 (send_reaction)
          
-         559         992 LOAD_CONST              23 ('to')
+         539         782 LOAD_CONST              23 ('to')
          
-         561         994 LOAD_NAME                3 (str)
+         541         784 LOAD_NAME                3 (str)
          
-         559         996 LOAD_CONST              48 ('message_id')
+         539         786 LOAD_CONST              48 ('message_id')
          
-         562         998 LOAD_NAME                3 (str)
+         542         788 LOAD_NAME                3 (str)
          
-         559        1000 LOAD_CONST              30 ('return')
+         539         790 LOAD_CONST              30 ('return')
          
-         563        1002 LOAD_NAME                3 (str)
+         543         792 LOAD_NAME                3 (str)
          
-         559        1004 BUILD_TUPLE              6
-                    1006 LOAD_CONST              50 (<code object remove_reaction, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 559>)
-                    1008 MAKE_FUNCTION            4 (annotations)
-                    1010 STORE_NAME              36 (remove_reaction)
+         539         794 BUILD_TUPLE              6
+                     796 LOAD_CONST              50 (<code object remove_reaction, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 539>)
+                     798 MAKE_FUNCTION            4 (annotations)
+                     800 STORE_NAME              35 (remove_reaction)
          
-         585        1012 NOP
+         565         802 NOP
          
-         586        1014 NOP
+         566         804 NOP
          
-         580        1016 LOAD_CONST              65 ((None, None))
-                    1018 LOAD_CONST              23 ('to')
+         560         806 LOAD_CONST              65 ((None, None))
+                     808 LOAD_CONST              23 ('to')
          
-         582        1020 LOAD_NAME                3 (str)
+         562         810 LOAD_NAME                3 (str)
          
-         580        1022 LOAD_CONST              51 ('latitude')
+         560         812 LOAD_CONST              51 ('latitude')
          
-         583        1024 LOAD_NAME                6 (float)
+         563         814 LOAD_NAME                6 (float)
          
-         580        1026 LOAD_CONST              52 ('longitude')
+         560         816 LOAD_CONST              52 ('longitude')
          
-         584        1028 LOAD_NAME                6 (float)
+         564         818 LOAD_NAME                6 (float)
          
-         580        1030 LOAD_CONST              53 ('name')
+         560         820 LOAD_CONST              53 ('name')
          
-         585        1032 LOAD_NAME                3 (str)
-                    1034 LOAD_CONST               1 (None)
-                    1036 BINARY_OP                7 (|)
+         565         822 LOAD_NAME                3 (str)
+                     824 LOAD_CONST               1 (None)
+                     826 BINARY_OP                7 (|)
          
-         580        1040 LOAD_CONST              54 ('address')
+         560         830 LOAD_CONST              54 ('address')
          
-         586        1042 LOAD_NAME                3 (str)
-                    1044 LOAD_CONST               1 (None)
-                    1046 BINARY_OP                7 (|)
+         566         832 LOAD_NAME                3 (str)
+                     834 LOAD_CONST               1 (None)
+                     836 BINARY_OP                7 (|)
          
-         580        1050 LOAD_CONST              30 ('return')
+         560         840 LOAD_CONST              30 ('return')
          
-         587        1052 LOAD_NAME                3 (str)
+         567         842 LOAD_NAME                3 (str)
          
-         580        1054 BUILD_TUPLE             12
-                    1056 LOAD_CONST              55 (<code object send_location, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 580>)
-                    1058 MAKE_FUNCTION            5 (defaults, annotations)
-                    1060 STORE_NAME              37 (send_location)
+         560         844 BUILD_TUPLE             12
+                     846 LOAD_CONST              55 (<code object send_location, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 560>)
+                     848 MAKE_FUNCTION            5 (defaults, annotations)
+                     850 STORE_NAME              36 (send_location)
          
-         620        1062 NOP
+         600         852 NOP
          
-         616        1064 LOAD_CONST              60 ((None,))
-                    1066 LOAD_CONST              23 ('to')
+         596         854 LOAD_CONST              63 ((None,))
+                     856 LOAD_CONST              23 ('to')
          
-         618        1068 LOAD_NAME                3 (str)
+         598         858 LOAD_NAME                3 (str)
          
-         616        1070 LOAD_CONST              56 ('contact')
+         596         860 LOAD_CONST              56 ('contact')
          
-         619        1072 LOAD_NAME               38 (Contact)
-                    1074 LOAD_NAME               12 (Iterable)
-                    1076 LOAD_NAME               38 (Contact)
-                    1078 BINARY_SUBSCR
-                    1088 BINARY_OP                7 (|)
+         599         862 LOAD_NAME               37 (Contact)
+                     864 LOAD_NAME               38 (Iterable)
+                     866 LOAD_NAME               37 (Contact)
+                     868 BINARY_SUBSCR
+                     878 BINARY_OP                7 (|)
          
-         616        1092 LOAD_CONST              26 ('reply_to_message_id')
+         596         882 LOAD_CONST              26 ('reply_to_message_id')
          
-         620        1094 LOAD_NAME                3 (str)
-                    1096 LOAD_CONST               1 (None)
-                    1098 BINARY_OP                7 (|)
+         600         884 LOAD_NAME                3 (str)
+                     886 LOAD_CONST               1 (None)
+                     888 BINARY_OP                7 (|)
          
-         616        1102 LOAD_CONST              30 ('return')
+         596         892 LOAD_CONST              30 ('return')
          
-         621        1104 LOAD_NAME                3 (str)
+         601         894 LOAD_NAME                3 (str)
          
-         616        1106 BUILD_TUPLE              8
-                    1108 LOAD_CONST              57 (<code object send_contact, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 616>)
-                    1110 MAKE_FUNCTION            5 (defaults, annotations)
-                    1112 STORE_NAME              39 (send_contact)
+         596         896 BUILD_TUPLE              8
+                     898 LOAD_CONST              57 (<code object send_contact, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 596>)
+                     900 MAKE_FUNCTION            5 (defaults, annotations)
+                     902 STORE_NAME              39 (send_contact)
          
-         652        1114 LOAD_CONST              48 ('message_id')
+         632         904 LOAD_CONST              48 ('message_id')
          
-         654        1116 LOAD_NAME                3 (str)
+         634         906 LOAD_NAME                3 (str)
          
-         652        1118 LOAD_CONST              30 ('return')
+         632         908 LOAD_CONST              30 ('return')
          
-         655        1120 LOAD_NAME               15 (bool)
+         635         910 LOAD_NAME               14 (bool)
          
-         652        1122 BUILD_TUPLE              4
-                    1124 LOAD_CONST              58 (<code object mark_message_as_read, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 652>)
-                    1126 MAKE_FUNCTION            4 (annotations)
-                    1128 STORE_NAME              40 (mark_message_as_read)
-                    1130 LOAD_CONST               1 (None)
-                    1132 RETURN_VALUE
+         632         912 BUILD_TUPLE              4
+                     914 LOAD_CONST              58 (<code object mark_message_as_read, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 632>)
+                     916 MAKE_FUNCTION            4 (annotations)
+                     918 STORE_NAME              40 (mark_message_as_read)
+                     920 LOAD_CONST               1 (None)
+                     922 RETURN_VALUE
          consts
             'WhatsApp'
             None
             '/pywa'
             'https://graph.facebook.com'
             17.0
             'phone_id'
@@ -966,423 +876,423 @@
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'add_handler'
                firstlineno 60
                lnotab 0x02010e011e01
             'filters'
             code
-               argcount  : 2
+               argcount  : 1
                nlocals   : 3
                stacksize : 4
-               flags     : 3
+               flags     : 7
                code
                   0x8700870197006401740000000000000000000000640274020000000000
                   000000000067027404000000000000000000006602190000000000000000
                   0066028801880066026403840c7d027c025300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                1 (filters)
                
                 65           4 RESUME                   0
                
-                82           6 LOAD_CONST               1 ('func')
+                79           6 LOAD_CONST               1 ('func')
                              8 LOAD_GLOBAL              0 (Callable)
                             20 LOAD_CONST               2 ('WhatsApp')
                             22 LOAD_GLOBAL              2 (dict)
                             34 BUILD_LIST               2
                             36 LOAD_GLOBAL              4 (Any)
                             48 BUILD_TUPLE              2
                             50 BINARY_SUBSCR
                             60 BUILD_TUPLE              2
                             62 LOAD_CLOSURE             1 (filters)
                             64 LOAD_CLOSURE             0 (self)
                             66 BUILD_TUPLE              2
-                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 82>)
+                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 79>)
                             70 MAKE_FUNCTION           12 (annotations, closure)
                             72 STORE_FAST               2 (decorator)
                
-                85          74 LOAD_FAST                2 (decorator)
+                82          74 LOAD_FAST                2 (decorator)
                             76 RETURN_VALUE
                consts
                   '\n        Decorator to register a function as a handler for raw updates.\n\n        Example:\n\n            >>> @wa.on_raw_update()\n            ... def raw_update_handler(wa: WhatsApp, update: dict):\n            ...     print(update)\n\n        Args:\n            filters: Filters to apply to the incoming updates (filters are function that take the WhatsApp client and\n                the incoming update and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 6
+                     stacksize : 7
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        03000000000000000000007c008901ac01a6020000ab0200000000000000
-                        00a6010000ab01000000000000000001007c005300
+                        0300000000000000000000890164017c0069018e01a6010000ab01000000
+                        000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
-                      82           2 RESUME                   0
+                      79           2 RESUME                   0
                      
-                      83           4 LOAD_DEREF               2 (self)
+                      80           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + RawUpdateHandler)
-                                  40 LOAD_FAST                0 (func)
-                                  42 LOAD_DEREF               1 (filters)
-                                  44 KW_NAMES                 1
-                                  46 PRECALL                  2
-                                  50 CALL                     2
-                                  60 PRECALL                  1
-                                  64 CALL                     1
-                                  74 POP_TOP
+                                  40 LOAD_DEREF               1 (filters)
+                                  42 LOAD_CONST               1 ('handler')
+                                  44 LOAD_FAST                0 (func)
+                                  46 BUILD_MAP                1
+                                  48 CALL_FUNCTION_EX         1
+                                  50 PRECALL                  1
+                                  54 CALL                     1
+                                  64 POP_TOP
                      
-                      84          76 LOAD_FAST                0 (func)
-                                  78 RETURN_VALUE
+                      81          66 LOAD_FAST                0 (func)
+                                  68 RETURN_VALUE
                      consts
                         None
-                        ('handler', 'filters')
+                        'handler'
                      names      ('add_handler', 'RawUpdateHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
-                     firstlineno 82
-                     lnotab 0x04014801
+                     firstlineno 79
+                     lnotab 0x04013e01
                names      ('Callable', 'dict', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_raw_update'
                firstlineno 65
-               lnotab 0x06114403
+               lnotab 0x060e4403
             code
-               argcount  : 2
+               argcount  : 1
                nlocals   : 3
                stacksize : 4
-               flags     : 3
+               flags     : 7
                code
                   0x8700870197006401740000000000000000000000640274020000000000
                   000000000067027404000000000000000000006602190000000000000000
                   0066028801880066026403840c7d027c025300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                1 (filters)
                
-                87           4 RESUME                   0
+                84           4 RESUME                   0
                
-               106           6 LOAD_CONST               1 ('func')
+                98           6 LOAD_CONST               1 ('func')
                              8 LOAD_GLOBAL              0 (Callable)
                             20 LOAD_CONST               2 ('WhatsApp')
                             22 LOAD_GLOBAL              2 (Message)
                             34 BUILD_LIST               2
                             36 LOAD_GLOBAL              4 (Any)
                             48 BUILD_TUPLE              2
                             50 BINARY_SUBSCR
                             60 BUILD_TUPLE              2
                             62 LOAD_CLOSURE             1 (filters)
                             64 LOAD_CLOSURE             0 (self)
                             66 BUILD_TUPLE              2
-                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 106>)
+                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 98>)
                             70 MAKE_FUNCTION           12 (annotations, closure)
                             72 STORE_FAST               2 (decorator)
                
-               109          74 LOAD_FAST                2 (decorator)
+               101          74 LOAD_FAST                2 (decorator)
                             76 RETURN_VALUE
                consts
-                  '\n        Decorator to register a function as a handler for incoming messages.\n\n        Example:\n\n            >>> @wa.on_message(filters=TextFilter.EQUALS(("hello", "hi"))\n            ... def hello_handler(wa: WhatsApp, msg: Message):\n            ...     msg.react("👋")\n            ...     msg.reply_text(text="Hello from PyWa!", quote=True, buttons=[InlineButton("Help", data="help")\n\n        Args:\n            filters: Filters to apply to the incoming messages (filters are function that take the WhatsApp client and\n                the incoming message and return a boolean).\n        '
+                  '\n        Decorator to register a function as a handler for incoming messages.\n\n        Example:\n            >>> @wa.on_message(TextFilter.equals("hello", "hi")\n            ... def hello_handler(wa: WhatsApp, msg: Message):\n            ...     msg.react("👋")\n            ...     msg.reply_text(text="Hello from PyWa!", quote=True, buttons=[InlineButton("Help", data="help")\n\n        Args:\n            filters: Filters to apply to the incoming messages (filters are function that take the WhatsApp client and\n                the incoming message and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 6
+                     stacksize : 7
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        03000000000000000000007c008901ac01a6020000ab0200000000000000
-                        00a6010000ab01000000000000000001007c005300
+                        0300000000000000000000890164017c0069018e01a6010000ab01000000
+                        000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
-                     106           2 RESUME                   0
+                      98           2 RESUME                   0
                      
-                     107           4 LOAD_DEREF               2 (self)
+                      99           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + MessageHandler)
-                                  40 LOAD_FAST                0 (func)
-                                  42 LOAD_DEREF               1 (filters)
-                                  44 KW_NAMES                 1
-                                  46 PRECALL                  2
-                                  50 CALL                     2
-                                  60 PRECALL                  1
-                                  64 CALL                     1
-                                  74 POP_TOP
+                                  40 LOAD_DEREF               1 (filters)
+                                  42 LOAD_CONST               1 ('handler')
+                                  44 LOAD_FAST                0 (func)
+                                  46 BUILD_MAP                1
+                                  48 CALL_FUNCTION_EX         1
+                                  50 PRECALL                  1
+                                  54 CALL                     1
+                                  64 POP_TOP
                      
-                     108          76 LOAD_FAST                0 (func)
-                                  78 RETURN_VALUE
+                     100          66 LOAD_FAST                0 (func)
+                                  68 RETURN_VALUE
                      consts
                         None
-                        ('handler', 'filters')
+                        'handler'
                      names      ('add_handler', 'MessageHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
-                     firstlineno 106
-                     lnotab 0x04014801
+                     firstlineno 98
+                     lnotab 0x04013e01
                names      ('Callable', 'Message', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_message'
-               firstlineno 87
-               lnotab 0x06134403
+               firstlineno 84
+               lnotab 0x060e4403
             code
-               argcount  : 2
+               argcount  : 1
                nlocals   : 3
                stacksize : 4
-               flags     : 3
+               flags     : 7
                code
                   0x8700870197006401740000000000000000000000640274020000000000
                   000000000067027404000000000000000000006602190000000000000000
                   0066028801880066026403840c7d027c025300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                1 (filters)
                
-               111           4 RESUME                   0
+               103           4 RESUME                   0
                
-               129           6 LOAD_CONST               1 ('func')
+               117           6 LOAD_CONST               1 ('func')
                              8 LOAD_GLOBAL              0 (Callable)
                             20 LOAD_CONST               2 ('WhatsApp')
                             22 LOAD_GLOBAL              2 (CallbackButton)
                             34 BUILD_LIST               2
                             36 LOAD_GLOBAL              4 (Any)
                             48 BUILD_TUPLE              2
                             50 BINARY_SUBSCR
                             60 BUILD_TUPLE              2
                             62 LOAD_CLOSURE             1 (filters)
                             64 LOAD_CLOSURE             0 (self)
                             66 BUILD_TUPLE              2
-                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 129>)
+                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 117>)
                             70 MAKE_FUNCTION           12 (annotations, closure)
                             72 STORE_FAST               2 (decorator)
                
-               132          74 LOAD_FAST                2 (decorator)
+               120          74 LOAD_FAST                2 (decorator)
                             76 RETURN_VALUE
                consts
-                  '\n        Decorator to register a function as a handler for incoming callback button presses.\n\n        Example:\n\n            >>> @wa.on_callback_button(filters=CallbackFilter.DATA_EQUALS("help"))\n            ... def help_handler(wa: WhatsApp, btn: CallbackButton):\n            ...     btn.reply_text(text="What can I help you with?")\n\n        Args:\n            filters: Filters to apply to the incoming callback button presses (filters are function that take the\n                WhatsApp client and the incoming callback button and return a boolean).\n        '
+                  '\n        Decorator to register a function as a handler for incoming callback button presses.\n\n        Example:\n\n            >>> @wa.on_callback_button(CallbackFilter.data_equals("help"))\n            ... def help_handler(wa: WhatsApp, btn: CallbackButton):\n            ...     btn.reply_text(text="What can I help you with?")\n\n        Args:\n            filters: Filters to apply to the incoming callback button presses (filters are function that take the\n                WhatsApp client and the incoming callback button and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 6
+                     stacksize : 7
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        03000000000000000000007c008901ac01a6020000ab0200000000000000
-                        00a6010000ab01000000000000000001007c005300
+                        0300000000000000000000890164017c0069018e01a6010000ab01000000
+                        000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
-                     129           2 RESUME                   0
+                     117           2 RESUME                   0
                      
-                     130           4 LOAD_DEREF               2 (self)
+                     118           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + ButtonCallbackHandler)
-                                  40 LOAD_FAST                0 (func)
-                                  42 LOAD_DEREF               1 (filters)
-                                  44 KW_NAMES                 1
-                                  46 PRECALL                  2
-                                  50 CALL                     2
-                                  60 PRECALL                  1
-                                  64 CALL                     1
-                                  74 POP_TOP
+                                  40 LOAD_DEREF               1 (filters)
+                                  42 LOAD_CONST               1 ('handler')
+                                  44 LOAD_FAST                0 (func)
+                                  46 BUILD_MAP                1
+                                  48 CALL_FUNCTION_EX         1
+                                  50 PRECALL                  1
+                                  54 CALL                     1
+                                  64 POP_TOP
                      
-                     131          76 LOAD_FAST                0 (func)
-                                  78 RETURN_VALUE
+                     119          66 LOAD_FAST                0 (func)
+                                  68 RETURN_VALUE
                      consts
                         None
-                        ('handler', 'filters')
+                        'handler'
                      names      ('add_handler', 'ButtonCallbackHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
-                     firstlineno 129
-                     lnotab 0x04014801
+                     firstlineno 117
+                     lnotab 0x04013e01
                names      ('Callable', 'CallbackButton', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_callback_button'
-               firstlineno 111
-               lnotab 0x06124403
+               firstlineno 103
+               lnotab 0x060e4403
             code
-               argcount  : 2
+               argcount  : 1
                nlocals   : 3
                stacksize : 4
-               flags     : 3
+               flags     : 7
                code
                   0x8700870197006401740000000000000000000000640274020000000000
                   000000000067027404000000000000000000006602190000000000000000
                   0066028801880066026403840c7d027c025300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                1 (filters)
                
-               134           4 RESUME                   0
+               122           4 RESUME                   0
                
-               152           6 LOAD_CONST               1 ('func')
+               136           6 LOAD_CONST               1 ('func')
                              8 LOAD_GLOBAL              0 (Callable)
                             20 LOAD_CONST               2 ('WhatsApp')
                             22 LOAD_GLOBAL              2 (CallbackSelection)
                             34 BUILD_LIST               2
                             36 LOAD_GLOBAL              4 (Any)
                             48 BUILD_TUPLE              2
                             50 BINARY_SUBSCR
                             60 BUILD_TUPLE              2
                             62 LOAD_CLOSURE             1 (filters)
                             64 LOAD_CLOSURE             0 (self)
                             66 BUILD_TUPLE              2
-                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 152>)
+                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 136>)
                             70 MAKE_FUNCTION           12 (annotations, closure)
                             72 STORE_FAST               2 (decorator)
                
-               155          74 LOAD_FAST                2 (decorator)
+               139          74 LOAD_FAST                2 (decorator)
                             76 RETURN_VALUE
                consts
-                  '\n        Decorator to register a function as a handler for incoming callback selections.\n\n        Example:\n\n            >>> @wa.on_callback_selection(filters=CallbackFilter.DATA_STARTS_WITH("id:"))\n            ... def id_handler(wa: WhatsApp, sel: CallbackSelection):\n            ...     sel.reply_text(text=f"Your ID is {sel.data.split(\':\', 1)[1]}")\n\n        Args:\n            filters: Filters to apply to the incoming callback selections (filters are function that take the\n                WhatsApp client and the incoming callback selection and return a boolean).\n        '
+                  '\n        Decorator to register a function as a handler for incoming callback selections.\n\n        Example:\n\n            >>> @wa.on_callback_selection(CallbackFilter.data_startswith("id:"))\n            ... def id_handler(wa: WhatsApp, sel: CallbackSelection):\n            ...     sel.reply_text(text=f"Your ID is {sel.data.split(\':\', 1)[1]}")\n\n        Args:\n            filters: Filters to apply to the incoming callback selections (filters are function that take the\n                WhatsApp client and the incoming callback selection and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 6
+                     stacksize : 7
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        03000000000000000000007c008901ac01a6020000ab0200000000000000
-                        00a6010000ab01000000000000000001007c005300
+                        0300000000000000000000890164017c0069018e01a6010000ab01000000
+                        000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
-                     152           2 RESUME                   0
+                     136           2 RESUME                   0
                      
-                     153           4 LOAD_DEREF               2 (self)
+                     137           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + SelectionCallbackHandler)
-                                  40 LOAD_FAST                0 (func)
-                                  42 LOAD_DEREF               1 (filters)
-                                  44 KW_NAMES                 1
-                                  46 PRECALL                  2
-                                  50 CALL                     2
-                                  60 PRECALL                  1
-                                  64 CALL                     1
-                                  74 POP_TOP
+                                  40 LOAD_DEREF               1 (filters)
+                                  42 LOAD_CONST               1 ('handler')
+                                  44 LOAD_FAST                0 (func)
+                                  46 BUILD_MAP                1
+                                  48 CALL_FUNCTION_EX         1
+                                  50 PRECALL                  1
+                                  54 CALL                     1
+                                  64 POP_TOP
                      
-                     154          76 LOAD_FAST                0 (func)
-                                  78 RETURN_VALUE
+                     138          66 LOAD_FAST                0 (func)
+                                  68 RETURN_VALUE
                      consts
                         None
-                        ('handler', 'filters')
+                        'handler'
                      names      ('add_handler', 'SelectionCallbackHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
-                     firstlineno 152
-                     lnotab 0x04014801
+                     firstlineno 136
+                     lnotab 0x04013e01
                names      ('Callable', 'CallbackSelection', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_callback_selection'
-               firstlineno 134
-               lnotab 0x06124403
+               firstlineno 122
+               lnotab 0x060e4403
             code
-               argcount  : 2
+               argcount  : 1
                nlocals   : 3
                stacksize : 4
-               flags     : 3
+               flags     : 7
                code
                   0x8700870197006401740000000000000000000000640274020000000000
                   000000000067027404000000000000000000006602190000000000000000
                   0066028801880066026403840c7d027c025300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                1 (filters)
                
-               157           4 RESUME                   0
+               141           4 RESUME                   0
                
-               175           6 LOAD_CONST               1 ('func')
+               155           6 LOAD_CONST               1 ('func')
                              8 LOAD_GLOBAL              0 (Callable)
                             20 LOAD_CONST               2 ('WhatsApp')
                             22 LOAD_GLOBAL              2 (MessageStatus)
                             34 BUILD_LIST               2
                             36 LOAD_GLOBAL              4 (Any)
                             48 BUILD_TUPLE              2
                             50 BINARY_SUBSCR
                             60 BUILD_TUPLE              2
                             62 LOAD_CLOSURE             1 (filters)
                             64 LOAD_CLOSURE             0 (self)
                             66 BUILD_TUPLE              2
-                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 175>)
+                            68 LOAD_CONST               3 (<code object decorator, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py", line 155>)
                             70 MAKE_FUNCTION           12 (annotations, closure)
                             72 STORE_FAST               2 (decorator)
                
-               178          74 LOAD_FAST                2 (decorator)
+               158          74 LOAD_FAST                2 (decorator)
                             76 RETURN_VALUE
                consts
-                  '\n        Decorator to register a function as a handler for incoming message status changes.\n\n        Example:\n\n            >>> @wa.on_message_status_change(filters=MessageStatusFilter.READ)\n            ... def delivered_handler(wa: WhatsApp, status: MessageStatus):\n            ...     print(f"Message {status.id} was read by {status.from_user.wa_id}")\n\n        Args:\n            filters: Filters to apply to the incoming message status changes (filters are function that take the\n                WhatsApp client and the incoming message status change and return a boolean).\n        '
+                  '\n        Decorator to register a function as a handler for incoming message status changes.\n\n        Example:\n\n            >>> @wa.on_message_status_change(MessageStatusFilter.READ)\n            ... def delivered_handler(wa: WhatsApp, status: MessageStatus):\n            ...     print(f"Message {status.id} was read by {status.from_user.wa_id}")\n\n        Args:\n            filters: Filters to apply to the incoming message status changes (filters are function that take the\n                WhatsApp client and the incoming message status change and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 6
+                     stacksize : 7
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        03000000000000000000007c008901ac01a6020000ab0200000000000000
-                        00a6010000ab01000000000000000001007c005300
+                        0300000000000000000000890164017c0069018e01a6010000ab01000000
+                        000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
-                     175           2 RESUME                   0
+                     155           2 RESUME                   0
                      
-                     176           4 LOAD_DEREF               2 (self)
+                     156           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + MessageStatusHandler)
-                                  40 LOAD_FAST                0 (func)
-                                  42 LOAD_DEREF               1 (filters)
-                                  44 KW_NAMES                 1
-                                  46 PRECALL                  2
-                                  50 CALL                     2
-                                  60 PRECALL                  1
-                                  64 CALL                     1
-                                  74 POP_TOP
+                                  40 LOAD_DEREF               1 (filters)
+                                  42 LOAD_CONST               1 ('handler')
+                                  44 LOAD_FAST                0 (func)
+                                  46 BUILD_MAP                1
+                                  48 CALL_FUNCTION_EX         1
+                                  50 PRECALL                  1
+                                  54 CALL                     1
+                                  64 POP_TOP
                      
-                     177          76 LOAD_FAST                0 (func)
-                                  78 RETURN_VALUE
+                     157          66 LOAD_FAST                0 (func)
+                                  68 RETURN_VALUE
                      consts
                         None
-                        ('handler', 'filters')
+                        'handler'
                      names      ('add_handler', 'MessageStatusHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
-                     firstlineno 175
-                     lnotab 0x04014801
+                     firstlineno 155
+                     lnotab 0x04013e01
                names      ('Callable', 'MessageStatus', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_message_status_change'
-               firstlineno 157
-               lnotab 0x06124403
+               firstlineno 141
+               lnotab 0x060e4403
             False
             'to'
             'text'
             'preview_url'
             'reply_to_message_id'
             'keyboard'
             'header'
@@ -1395,63 +1305,63 @@
                flags     : 3
                code
                   0x97007c05731e7c006a000000000000000000a001000000000000000000
                   00000000000000000000007c017c027c037c04ac01a6040000ab04000000
                   000000000053007c006a000000000000000000a002000000000000000000
                   00000000000000000000007c017c057c06720564027c0664039c026e0164
                   047c027c07ac05a6050000ab0500000000000000005300
-               180           0 RESUME                   0
+               160           0 RESUME                   0
                
-               266           2 LOAD_FAST                5 (keyboard)
+               246           2 LOAD_FAST                5 (keyboard)
                              4 POP_JUMP_FORWARD_IF_TRUE    30 (to 66)
                
-               267           6 LOAD_FAST                0 (self)
+               247           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (api)
                             18 LOAD_METHOD              1 (send_text_message)
                
-               268          40 LOAD_FAST                1 (to)
+               248          40 LOAD_FAST                1 (to)
                
-               269          42 LOAD_FAST                2 (text)
+               249          42 LOAD_FAST                2 (text)
                
-               270          44 LOAD_FAST                3 (preview_url)
+               250          44 LOAD_FAST                3 (preview_url)
                
-               271          46 LOAD_FAST                4 (reply_to_message_id)
+               251          46 LOAD_FAST                4 (reply_to_message_id)
                
-               267          48 KW_NAMES                 1
+               247          48 KW_NAMES                 1
                             50 PRECALL                  4
                             54 CALL                     4
                             64 RETURN_VALUE
                
-               273     >>   66 LOAD_FAST                0 (self)
+               253     >>   66 LOAD_FAST                0 (self)
                             68 LOAD_ATTR                0 (api)
                             78 LOAD_METHOD              2 (send_interactive_message)
                
-               274         100 LOAD_FAST                1 (to)
+               254         100 LOAD_FAST                1 (to)
                
-               275         102 LOAD_FAST                5 (keyboard)
+               255         102 LOAD_FAST                5 (keyboard)
                
-               279         104 LOAD_FAST                6 (header)
+               259         104 LOAD_FAST                6 (header)
                
-               276         106 POP_JUMP_FORWARD_IF_FALSE     5 (to 118)
+               256         106 POP_JUMP_FORWARD_IF_FALSE     5 (to 118)
                
-               277         108 LOAD_CONST               2 ('text')
+               257         108 LOAD_CONST               2 ('text')
                
-               278         110 LOAD_FAST                6 (header)
+               258         110 LOAD_FAST                6 (header)
                
-               276         112 LOAD_CONST               3 (('type', 'text'))
+               256         112 LOAD_CONST               3 (('type', 'text'))
                            114 BUILD_CONST_KEY_MAP      2
                            116 JUMP_FORWARD             1 (to 120)
                
-               279     >>  118 LOAD_CONST               4 (None)
+               259     >>  118 LOAD_CONST               4 (None)
                
-               280     >>  120 LOAD_FAST                2 (text)
+               260     >>  120 LOAD_FAST                2 (text)
                
-               281         122 LOAD_FAST                7 (footer)
+               261         122 LOAD_FAST                7 (footer)
                
-               273         124 KW_NAMES                 5
+               253         124 KW_NAMES                 5
                            126 PRECALL                  5
                            130 CALL                     5
                            140 RETURN_VALUE
                consts
                   '\n        Send a message to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_message(\n            ...     to="1234567890",\n            ...     text="Hello from PyWa! (https://github.com/david-lev/pywa)",\n            ...     preview_url=True,\n            ... )\n\n        Example with keyboard buttons:\n\n            >>> wa.send_message(\n            ...     to="1234567890",\n            ...     header="Hello from PyWa!",\n            ...     text="What can I help you with?",\n            ...     keyboard=[\n            ...         InlineButton("Help", data="help"),\n            ...         InlineButton("About", data="about"),\n            ...     ],\n            ...     footer="Powered by PyWa",\n            ... )\n\n        Example with a section list:\n\n            >>> wa.send_message(\n            ...     to="1234567890",\n            ...     header="Hello from PyWa!",\n            ...     text="What can I help you with?",\n            ...     keyboard=SectionList(\n            ...         button_title="Choose an option",\n            ...         sections=[\n            ...             Section(\n            ...                 title="Help",\n            ...                 rows=[\n            ...                     SectionRow(\n            ...                         title="Help",\n            ...                         callback_data="help",\n            ...                         description="Get help with PyWa",\n            ...                     ),\n            ...                     SectionRow(\n            ...                         title="About",\n            ...                         callback_data="about",\n            ...                         description="Learn more about PyWa",\n            ...                     ),\n            ...                 ],\n            ...             ),\n            ...            Section(\n            ...                 title="Other",\n            ...                 rows=[\n            ...                     SectionRow(\n            ...                         title="GitHub",\n            ...                         callback_data="github",\n            ...                         description="View the PyWa GitHub repository",\n            ...                     ),\n            ...                 ],\n            ...             ),\n            ...         ],\n            ...     ),\n            ...     footer="Powered by PyWa",\n            ... )\n\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            text: The text to send (markdown allowed, max 4096 characters).\n            preview_url: Whether to show a preview of the URL in the message (if any).\n            reply_to_message_id: The message ID to reply to (optional).\n            keyboard: The keyboard to send with the message (optional).\n            header: The header of the message (if keyboard is provided, optional, up to 60 characters, no markdown allowed).\n            footer: The footer of the message (if keyboard is provided, optional, up to 60 characters, markdown has no effect).\n\n        Returns:\n            The message ID of the sent message.\n        '
                   ('to', 'text', 'preview_url', 'reply_to_message_id')
                   'text'
@@ -1460,15 +1370,15 @@
                   ('to', 'keyboard', 'header', 'body', 'footer')
                names      ('api', 'send_text_message', 'send_interactive_message')
                varnames   ('self', 'to', 'text', 'preview_url', 'reply_to_message_id', 'keyboard', 'header', 'footer')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_message'
-               firstlineno 180
+               firstlineno 160
                lnotab
                   0x02560401220102010201020102fc120622010201020402fd0201020102
                   fe06030201020102f8
             'image'
             'caption'
             'buttons'
             'body'
@@ -1482,84 +1392,84 @@
                   00000000000000000000007c017c0264017c047c03ac02a6050000ab0500
                   0000000000000053007c0673117c03730f74050000000000000000000064
                   03a6010000ab01000000000000000082017c006a000000000000000000a0
                   0300000000000000000000000000000000000000007c017c0564017c02a0
                   0400000000000000000000000000000000000000006404a6010000ab0100
                   00000000000000720264056e0164067c02690164079c027c0670017c037c
                   077c04ac08a6060000ab0600000000000000005300
-               284           0 RESUME                   0
+               264           0 RESUME                   0
                
-               317           2 LOAD_FAST                5 (buttons)
+               297           2 LOAD_FAST                5 (buttons)
                              4 POP_JUMP_FORWARD_IF_TRUE    31 (to 68)
                
-               318           6 LOAD_FAST                0 (self)
+               298           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (api)
                             18 LOAD_METHOD              1 (send_media)
                
-               319          40 LOAD_FAST                1 (to)
+               299          40 LOAD_FAST                1 (to)
                
-               320          42 LOAD_FAST                2 (image)
+               300          42 LOAD_FAST                2 (image)
                
-               321          44 LOAD_CONST               1 ('image')
+               301          44 LOAD_CONST               1 ('image')
                
-               322          46 LOAD_FAST                4 (reply_to_message_id)
+               302          46 LOAD_FAST                4 (reply_to_message_id)
                
-               323          48 LOAD_FAST                3 (caption)
+               303          48 LOAD_FAST                3 (caption)
                
-               318          50 KW_NAMES                 2
+               298          50 KW_NAMES                 2
                             52 PRECALL                  5
                             56 CALL                     5
                             66 RETURN_VALUE
                
-               325     >>   68 LOAD_FAST                6 (body)
+               305     >>   68 LOAD_FAST                6 (body)
                             70 POP_JUMP_FORWARD_IF_TRUE    17 (to 106)
                             72 LOAD_FAST                3 (caption)
                             74 POP_JUMP_FORWARD_IF_TRUE    15 (to 106)
                
-               326          76 LOAD_GLOBAL              5 (NULL + ValueError)
+               306          76 LOAD_GLOBAL              5 (NULL + ValueError)
                             88 LOAD_CONST               3 ('Either body or caption must be provided when sending an image with buttons.')
                             90 PRECALL                  1
                             94 CALL                     1
                            104 RAISE_VARARGS            1
                
-               327     >>  106 LOAD_FAST                0 (self)
+               307     >>  106 LOAD_FAST                0 (self)
                            108 LOAD_ATTR                0 (api)
                            118 LOAD_METHOD              3 (send_interactive_message)
                
-               328         140 LOAD_FAST                1 (to)
+               308         140 LOAD_FAST                1 (to)
                
-               329         142 LOAD_FAST                5 (buttons)
+               309         142 LOAD_FAST                5 (buttons)
                
-               331         144 LOAD_CONST               1 ('image')
+               311         144 LOAD_CONST               1 ('image')
                
-               333         146 LOAD_FAST                2 (image)
+               313         146 LOAD_FAST                2 (image)
                            148 LOAD_METHOD              4 (startswith)
                            170 LOAD_CONST               4 (('https://', 'http://'))
                            172 PRECALL                  1
                            176 CALL                     1
                            186 POP_JUMP_FORWARD_IF_FALSE     2 (to 192)
                            188 LOAD_CONST               5 ('link')
                            190 JUMP_FORWARD             1 (to 194)
                        >>  192 LOAD_CONST               6 ('id')
                        >>  194 LOAD_FAST                2 (image)
                
-               332         196 BUILD_MAP                1
+               312         196 BUILD_MAP                1
                
-               330         198 LOAD_CONST               7 (('type', 'image'))
+               310         198 LOAD_CONST               7 (('type', 'image'))
                            200 BUILD_CONST_KEY_MAP      2
                
-               336         202 LOAD_FAST                6 (body)
+               316         202 LOAD_FAST                6 (body)
                            204 JUMP_IF_TRUE_OR_POP      1 (to 208)
                            206 LOAD_FAST                3 (caption)
                
-               337     >>  208 LOAD_FAST                7 (footer)
+               317     >>  208 LOAD_FAST                7 (footer)
                
-               338         210 LOAD_FAST                4 (reply_to_message_id)
+               318         210 LOAD_FAST                4 (reply_to_message_id)
                
-               327         212 KW_NAMES                 8
+               307         212 KW_NAMES                 8
                            214 PRECALL                  6
                            218 CALL                     6
                            228 RETURN_VALUE
                consts
                   '\n        Send an image to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_image(\n            ...     to="1234567890",\n            ...     image="https://example.com/image.png",\n            ...     caption="This is an image!",\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            image: The image to send (either a URL or a file ID).\n            caption: The caption of the image (optional, markdown allowed).\n            reply_to_message_id: The message ID to reply to (optional).\n            buttons: The buttons to send with the image (optional).\n            body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).\n            footer: The footer of the message (if buttons is provided, optional, markdown has no effect).\n\n        Returns:\n            The message ID of the sent image.\n        '
                   'image'
                   ('to', 'media_id_or_url', 'media_type', 'reply_to_message_id', 'caption')
@@ -1571,15 +1481,15 @@
                   ('to', 'keyboard', 'header', 'body', 'footer', 'reply_to_message_id')
                names      ('api', 'send_media', 'ValueError', 'send_interactive_message', 'startswith')
                varnames   ('self', 'to', 'image', 'caption', 'reply_to_message_id', 'buttons', 'body', 'footer')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_image'
-               firstlineno 284
+               firstlineno 264
                lnotab
                   0x022104012201020102010201020102fb120708011e0122010201020202
                   0232ff02fe04060601020102f5
             'video'
             code
                argcount  : 8
                nlocals   : 8
@@ -1590,84 +1500,84 @@
                   00000000000000000000007c017c0264017c047c03ac02a6050000ab0500
                   0000000000000053007c0673117c03730f74050000000000000000000064
                   03a6010000ab01000000000000000082017c006a000000000000000000a0
                   0300000000000000000000000000000000000000007c017c0564017c02a0
                   0400000000000000000000000000000000000000006404a6010000ab0100
                   00000000000000720264056e0164067c02690164079c027c0670017c037c
                   077c04ac08a6060000ab0600000000000000005300
-               341           0 RESUME                   0
+               321           0 RESUME                   0
                
-               374           2 LOAD_FAST                5 (buttons)
+               354           2 LOAD_FAST                5 (buttons)
                              4 POP_JUMP_FORWARD_IF_TRUE    31 (to 68)
                
-               375           6 LOAD_FAST                0 (self)
+               355           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (api)
                             18 LOAD_METHOD              1 (send_media)
                
-               376          40 LOAD_FAST                1 (to)
+               356          40 LOAD_FAST                1 (to)
                
-               377          42 LOAD_FAST                2 (video)
+               357          42 LOAD_FAST                2 (video)
                
-               378          44 LOAD_CONST               1 ('video')
+               358          44 LOAD_CONST               1 ('video')
                
-               379          46 LOAD_FAST                4 (reply_to_message_id)
+               359          46 LOAD_FAST                4 (reply_to_message_id)
                
-               380          48 LOAD_FAST                3 (caption)
+               360          48 LOAD_FAST                3 (caption)
                
-               375          50 KW_NAMES                 2
+               355          50 KW_NAMES                 2
                             52 PRECALL                  5
                             56 CALL                     5
                             66 RETURN_VALUE
                
-               382     >>   68 LOAD_FAST                6 (body)
+               362     >>   68 LOAD_FAST                6 (body)
                             70 POP_JUMP_FORWARD_IF_TRUE    17 (to 106)
                             72 LOAD_FAST                3 (caption)
                             74 POP_JUMP_FORWARD_IF_TRUE    15 (to 106)
                
-               383          76 LOAD_GLOBAL              5 (NULL + ValueError)
+               363          76 LOAD_GLOBAL              5 (NULL + ValueError)
                             88 LOAD_CONST               3 ('Either body or caption must be provided when sending a video with buttons.')
                             90 PRECALL                  1
                             94 CALL                     1
                            104 RAISE_VARARGS            1
                
-               384     >>  106 LOAD_FAST                0 (self)
+               364     >>  106 LOAD_FAST                0 (self)
                            108 LOAD_ATTR                0 (api)
                            118 LOAD_METHOD              3 (send_interactive_message)
                
-               385         140 LOAD_FAST                1 (to)
+               365         140 LOAD_FAST                1 (to)
                
-               386         142 LOAD_FAST                5 (buttons)
+               366         142 LOAD_FAST                5 (buttons)
                
-               388         144 LOAD_CONST               1 ('video')
+               368         144 LOAD_CONST               1 ('video')
                
-               390         146 LOAD_FAST                2 (video)
+               370         146 LOAD_FAST                2 (video)
                            148 LOAD_METHOD              4 (startswith)
                            170 LOAD_CONST               4 (('https://', 'http://'))
                            172 PRECALL                  1
                            176 CALL                     1
                            186 POP_JUMP_FORWARD_IF_FALSE     2 (to 192)
                            188 LOAD_CONST               5 ('link')
                            190 JUMP_FORWARD             1 (to 194)
                        >>  192 LOAD_CONST               6 ('id')
                        >>  194 LOAD_FAST                2 (video)
                
-               389         196 BUILD_MAP                1
+               369         196 BUILD_MAP                1
                
-               387         198 LOAD_CONST               7 (('type', 'video'))
+               367         198 LOAD_CONST               7 (('type', 'video'))
                            200 BUILD_CONST_KEY_MAP      2
                
-               393         202 LOAD_FAST                6 (body)
+               373         202 LOAD_FAST                6 (body)
                            204 JUMP_IF_TRUE_OR_POP      1 (to 208)
                            206 LOAD_FAST                3 (caption)
                
-               394     >>  208 LOAD_FAST                7 (footer)
+               374     >>  208 LOAD_FAST                7 (footer)
                
-               395         210 LOAD_FAST                4 (reply_to_message_id)
+               375         210 LOAD_FAST                4 (reply_to_message_id)
                
-               384         212 KW_NAMES                 8
+               364         212 KW_NAMES                 8
                            214 PRECALL                  6
                            218 CALL                     6
                            228 RETURN_VALUE
                consts
                   '\n        Send a video to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_video(\n            ...     to="1234567890",\n            ...     video="https://example.com/video.mp4",\n            ...     caption="This is a video",\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            video: The video to send (either a URL or a file ID).\n            caption: The caption of the video (optional, markdown allowed).\n            reply_to_message_id: The message ID to reply to (optional).\n            buttons: The buttons to send with the video (optional).\n            body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).\n            footer: The footer of the message (if buttons is provided, optional, markdown has no effect).\n\n        Returns:\n            The message ID of the sent message.\n        '
                   'video'
                   ('to', 'media_id_or_url', 'media_type', 'reply_to_message_id', 'caption')
@@ -1679,15 +1589,15 @@
                   ('to', 'keyboard', 'header', 'body', 'footer', 'reply_to_message_id')
                names      ('api', 'send_media', 'ValueError', 'send_interactive_message', 'startswith')
                varnames   ('self', 'to', 'video', 'caption', 'reply_to_message_id', 'buttons', 'body', 'footer')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_video'
-               firstlineno 341
+               firstlineno 321
                lnotab
                   0x022104012201020102010201020102fb120708011e0122010201020202
                   0232ff02fe04060601020102f5
             'document'
             'filename'
             code
                argcount  : 9
@@ -1699,89 +1609,89 @@
                   00000000000000000000007c017c0264017c057c037c04ac02a6060000ab
                   06000000000000000053007c0773117c04730f7405000000000000000000
                   006403a6010000ab01000000000000000082017c006a0000000000000000
                   00a00300000000000000000000000000000000000000007c017c0664017c
                   02a00400000000000000000000000000000000000000006404a6010000ab
                   010000000000000000720264056e0164067c0264077c03690264089c027c
                   0770017c047c087c05ac09a6060000ab0600000000000000005300
-               398           0 RESUME                   0
+               378           0 RESUME                   0
                
-               435           2 LOAD_FAST                6 (buttons)
+               415           2 LOAD_FAST                6 (buttons)
                              4 POP_JUMP_FORWARD_IF_TRUE    32 (to 70)
                
-               436           6 LOAD_FAST                0 (self)
+               416           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (api)
                             18 LOAD_METHOD              1 (send_media)
                
-               437          40 LOAD_FAST                1 (to)
+               417          40 LOAD_FAST                1 (to)
                
-               438          42 LOAD_FAST                2 (document)
+               418          42 LOAD_FAST                2 (document)
                
-               439          44 LOAD_CONST               1 ('document')
+               419          44 LOAD_CONST               1 ('document')
                
-               440          46 LOAD_FAST                5 (reply_to_message_id)
+               420          46 LOAD_FAST                5 (reply_to_message_id)
                
-               441          48 LOAD_FAST                3 (filename)
+               421          48 LOAD_FAST                3 (filename)
                
-               442          50 LOAD_FAST                4 (caption)
+               422          50 LOAD_FAST                4 (caption)
                
-               436          52 KW_NAMES                 2
+               416          52 KW_NAMES                 2
                             54 PRECALL                  6
                             58 CALL                     6
                             68 RETURN_VALUE
                
-               444     >>   70 LOAD_FAST                7 (body)
+               424     >>   70 LOAD_FAST                7 (body)
                             72 POP_JUMP_FORWARD_IF_TRUE    17 (to 108)
                             74 LOAD_FAST                4 (caption)
                             76 POP_JUMP_FORWARD_IF_TRUE    15 (to 108)
                
-               445          78 LOAD_GLOBAL              5 (NULL + ValueError)
+               425          78 LOAD_GLOBAL              5 (NULL + ValueError)
                             90 LOAD_CONST               3 ('Either body or caption must be provided when sending a document with buttons.')
                             92 PRECALL                  1
                             96 CALL                     1
                            106 RAISE_VARARGS            1
                
-               446     >>  108 LOAD_FAST                0 (self)
+               426     >>  108 LOAD_FAST                0 (self)
                            110 LOAD_ATTR                0 (api)
                            120 LOAD_METHOD              3 (send_interactive_message)
                
-               447         142 LOAD_FAST                1 (to)
+               427         142 LOAD_FAST                1 (to)
                
-               448         144 LOAD_FAST                6 (buttons)
+               428         144 LOAD_FAST                6 (buttons)
                
-               450         146 LOAD_CONST               1 ('document')
+               430         146 LOAD_CONST               1 ('document')
                
-               452         148 LOAD_FAST                2 (document)
+               432         148 LOAD_FAST                2 (document)
                            150 LOAD_METHOD              4 (startswith)
                            172 LOAD_CONST               4 (('https://', 'http://'))
                            174 PRECALL                  1
                            178 CALL                     1
                            188 POP_JUMP_FORWARD_IF_FALSE     2 (to 194)
                            190 LOAD_CONST               5 ('link')
                            192 JUMP_FORWARD             1 (to 196)
                        >>  194 LOAD_CONST               6 ('id')
                        >>  196 LOAD_FAST                2 (document)
                
-               453         198 LOAD_CONST               7 ('filename')
+               433         198 LOAD_CONST               7 ('filename')
                            200 LOAD_FAST                3 (filename)
                
-               451         202 BUILD_MAP                2
+               431         202 BUILD_MAP                2
                
-               449         204 LOAD_CONST               8 (('type', 'document'))
+               429         204 LOAD_CONST               8 (('type', 'document'))
                            206 BUILD_CONST_KEY_MAP      2
                
-               456         208 LOAD_FAST                7 (body)
+               436         208 LOAD_FAST                7 (body)
                            210 JUMP_IF_TRUE_OR_POP      1 (to 214)
                            212 LOAD_FAST                4 (caption)
                
-               457     >>  214 LOAD_FAST                8 (footer)
+               437     >>  214 LOAD_FAST                8 (footer)
                
-               458         216 LOAD_FAST                5 (reply_to_message_id)
+               438         216 LOAD_FAST                5 (reply_to_message_id)
                
-               446         218 KW_NAMES                 9
+               426         218 KW_NAMES                 9
                            220 PRECALL                  6
                            224 CALL                     6
                            234 RETURN_VALUE
                consts
                   '\n        Send a document to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_document(\n            ...     to="1234567890",\n            ...     document="https://example.com/example_123.pdf",\n            ...     filename="Example PDF",\n            ...     caption="Example PDF"\n            ... )\n\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            document: The document to send (either a URL or a file ID).\n            filename: The filename of the document (optional, The extension of the filename will specify what format the document is displayed as in WhatsApp).\n            caption: The caption of the document (optional).\n            reply_to_message_id: The message ID to reply to (optional).\n            buttons: The buttons to send with the document (optional).\n            body: The body of the message (if buttons are provided, optional, up to 1024 characters, markdown allowed).\n            footer: The footer of the message (if buttons is provided, optional, markdown has no effect).\n\n        Returns:\n            The message ID of the sent message.\n        '
                   'document'
                   ('to', 'media_id_or_url', 'media_type', 'reply_to_message_id', 'filename', 'caption')
@@ -1794,278 +1704,278 @@
                   ('to', 'keyboard', 'header', 'body', 'footer', 'reply_to_message_id')
                names      ('api', 'send_media', 'ValueError', 'send_interactive_message', 'startswith')
                varnames   ('self', 'to', 'document', 'filename', 'caption', 'reply_to_message_id', 'buttons', 'body', 'footer')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_document'
-               firstlineno 398
+               firstlineno 378
                lnotab
                   0x0225040122010201020102010201020102fa120808011e012201020102
                   020202320104fe02fe04070601020102f4
             'audio'
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c0264017c03ac02a6040000ab0400000000000000
                   005300
-               461           0 RESUME                   0
+               441           0 RESUME                   0
                
-               485           2 LOAD_FAST                0 (self)
+               465           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_media)
                
-               486          36 LOAD_FAST                1 (to)
+               466          36 LOAD_FAST                1 (to)
                
-               487          38 LOAD_FAST                2 (audio)
+               467          38 LOAD_FAST                2 (audio)
                
-               488          40 LOAD_CONST               1 ('audio')
+               468          40 LOAD_CONST               1 ('audio')
                
-               489          42 LOAD_FAST                3 (reply_to_message_id)
+               469          42 LOAD_FAST                3 (reply_to_message_id)
                
-               485          44 KW_NAMES                 2
+               465          44 KW_NAMES                 2
                             46 PRECALL                  4
                             50 CALL                     4
                             60 RETURN_VALUE
                consts
                   "\n        Send an audio file to a WhatsApp user.\n\n        Example:\n\n            >>> wa.send_audio(\n            ...     to='1234567890',\n            ...     audio='https://example.com/audio.mp3',\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            audio: The audio file to send (either a URL or a file ID).\n            reply_to_message_id: The message ID to reply to (optional).\n\n        Returns:\n            The message ID of the sent message.\n        "
                   'audio'
                   ('to', 'media_id_or_url', 'media_type', 'reply_to_message_id')
                names      ('api', 'send_media')
                varnames   ('self', 'to', 'audio', 'reply_to_message_id')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_audio'
-               firstlineno 461
+               firstlineno 441
                lnotab 0x0218220102010201020102fc
             'sticker'
             'animated'
             code
                argcount  : 5
                nlocals   : 5
                stacksize : 7
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c0264017c047c03ac02a6050000ab050000000000
                   0000005300
-               492           0 RESUME                   0
+               472           0 RESUME                   0
                
-               520           2 LOAD_FAST                0 (self)
+               500           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_media)
                
-               521          36 LOAD_FAST                1 (to)
+               501          36 LOAD_FAST                1 (to)
                
-               522          38 LOAD_FAST                2 (sticker)
+               502          38 LOAD_FAST                2 (sticker)
                
-               523          40 LOAD_CONST               1 ('sticker')
+               503          40 LOAD_CONST               1 ('sticker')
                
-               524          42 LOAD_FAST                4 (reply_to_message_id)
+               504          42 LOAD_FAST                4 (reply_to_message_id)
                
-               525          44 LOAD_FAST                3 (animated)
+               505          44 LOAD_FAST                3 (animated)
                
-               520          46 KW_NAMES                 2
+               500          46 KW_NAMES                 2
                             48 PRECALL                  5
                             52 CALL                     5
                             62 RETURN_VALUE
                consts
                   "\n        Send a sticker to a WhatsApp user.\n            - A static sticker needs to be 512x512 pixels and cannot exceed 100 KB.\n            - An animated sticker must be 512x512 pixels and cannot exceed 500 KB.\n\n        Example:\n\n            >>> wa.send_sticker(\n            ...     to='1234567890',\n            ...     sticker='https://example.com/sticker.webp',\n            ... )\n\n        Args:\n            to: The phone ID of the WhatsApp user.\n            sticker: The sticker to send (either a URL or a file ID).\n            animated: Whether the sticker is animated (optional).\n            reply_to_message_id: The message ID to reply to (optional).\n\n        Returns:\n            The message ID of the sent message.\n        "
                   'sticker'
                   ('to', 'media_id_or_url', 'media_type', 'reply_to_message_id', 'animated')
                names      ('api', 'send_media')
                varnames   ('self', 'to', 'sticker', 'animated', 'reply_to_message_id')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'send_sticker'
-               firstlineno 492
+               firstlineno 472
                lnotab 0x021c2201020102010201020102fb
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
-               528           0 RESUME                   0
+               508           0 RESUME                   0
                
-               553           2 LOAD_FAST                0 (self)
+               533           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_reaction)
                
-               554          36 LOAD_FAST                1 (to)
+               534          36 LOAD_FAST                1 (to)
                
-               555          38 LOAD_FAST                2 (emoji)
+               535          38 LOAD_FAST                2 (emoji)
                
-               556          40 LOAD_FAST                3 (message_id)
+               536          40 LOAD_FAST                3 (message_id)
                
-               553          42 KW_NAMES                 1
+               533          42 KW_NAMES                 1
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
-               firstlineno 528
+               firstlineno 508
                lnotab 0x021922010201020102fd
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c026401ac02a6030000ab03000000000000000053
                   00
-               559           0 RESUME                   0
+               539           0 RESUME                   0
                
-               574           2 LOAD_FAST                0 (self)
+               554           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_reaction)
                
-               575          36 LOAD_FAST                1 (to)
+               555          36 LOAD_FAST                1 (to)
                
-               576          38 LOAD_FAST                2 (message_id)
+               556          38 LOAD_FAST                2 (message_id)
                
-               577          40 LOAD_CONST               1 ('')
+               557          40 LOAD_CONST               1 ('')
                
-               574          42 KW_NAMES                 2
+               554          42 KW_NAMES                 2
                             44 PRECALL                  3
                             48 CALL                     3
                             58 RETURN_VALUE
                consts
                   "\n        Remove a reaction from a message.\n\n        Example:\n\n            >>> wa.remove_reaction(\n            ...     to='1234567890',\n            ...     message_id='wamid.XXX='\n            ... )\n        "
                   ''
                   ('to', 'message_id', 'emoji')
                names      ('api', 'send_reaction')
                varnames   ('self', 'to', 'message_id')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'remove_reaction'
-               firstlineno 559
+               firstlineno 539
                lnotab 0x020f22010201020102fd
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
-               580           0 RESUME                   0
+               560           0 RESUME                   0
                
-               608           2 LOAD_FAST                0 (self)
+               588           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_location)
                
-               609          36 LOAD_FAST                1 (to)
+               589          36 LOAD_FAST                1 (to)
                
-               610          38 LOAD_FAST                2 (latitude)
+               590          38 LOAD_FAST                2 (latitude)
                
-               611          40 LOAD_FAST                3 (longitude)
+               591          40 LOAD_FAST                3 (longitude)
                
-               612          42 LOAD_FAST                4 (name)
+               592          42 LOAD_FAST                4 (name)
                
-               613          44 LOAD_FAST                5 (address)
+               593          44 LOAD_FAST                5 (address)
                
-               608          46 KW_NAMES                 1
+               588          46 KW_NAMES                 1
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
-               firstlineno 580
+               firstlineno 560
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
-               616           0 RESUME                   0
+               596           0 RESUME                   0
                
-               646           2 LOAD_FAST                0 (self)
+               626           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (send_contacts)
                
-               647          36 LOAD_FAST                1 (to)
+               627          36 LOAD_FAST                1 (to)
                
-               648          38 LOAD_GLOBAL              5 (NULL + isinstance)
+               628          38 LOAD_GLOBAL              5 (NULL + isinstance)
                             50 LOAD_FAST                2 (contact)
                             52 LOAD_GLOBAL              6 (Iterable)
                             64 PRECALL                  2
                             68 CALL                     2
                             78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
                             80 LOAD_FAST                2 (contact)
                             82 JUMP_FORWARD             2 (to 88)
                        >>   84 LOAD_FAST                2 (contact)
                             86 BUILD_LIST               1
                
-               649     >>   88 LOAD_FAST                3 (reply_to_message_id)
+               629     >>   88 LOAD_FAST                3 (reply_to_message_id)
                
-               646          90 KW_NAMES                 1
+               626          90 KW_NAMES                 1
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
-               firstlineno 616
+               firstlineno 596
                lnotab 0x021e22010201320102fd
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01ac01a6010000ab0100000000000000005300
-               652           0 RESUME                   0
+               632           0 RESUME                   0
                
-               665           2 LOAD_FAST                0 (self)
+               645           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (api)
                             14 LOAD_METHOD              1 (mark_message_as_read)
                             36 LOAD_FAST                1 (message_id)
                             38 KW_NAMES                 1
                             40 PRECALL                  1
                             44 CALL                     1
                             54 RETURN_VALUE
@@ -2074,46 +1984,44 @@
                   ('message_id',)
                names      ('api', 'mark_message_as_read')
                varnames   ('self', 'message_id')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'mark_message_as_read'
-               firstlineno 652
+               firstlineno 632
                lnotab 0x020d
             (None, '/pywa', None, 'https://graph.facebook.com', 17.0, None)
-            (None,)
             (False, None, None, None, None)
             (None, None, None, None, None)
             (None, None, None, None, None, None)
+            (None,)
             (False, None)
             (None, None)
-         names      ('__name__', '__module__', '__qualname__', 'str', 'int', 'Any', 'float', 'requests', 'Session', '__init__', 'Handler', 'add_handler', 'Iterable', 'Callable', 'dict', 'bool', 'on_raw_update', 'Message', 'on_message', 'CallbackButton', 'on_callback_button', 'CallbackSelection', 'on_callback_selection', 'MessageStatus', 'on_message_status_change', 'list', 'InlineButton', 'SectionList', 'send_message', 'bytes', 'send_image', 'send_video', 'send_document', 'send_audio', 'send_sticker', 'send_reaction', 'remove_reaction', 'send_location', 'Contact', 'send_contact', 'mark_message_as_read')
+         names      ('__name__', '__module__', '__qualname__', 'str', 'int', 'Any', 'float', 'requests', 'Session', '__init__', 'Handler', 'add_handler', 'Callable', 'dict', 'bool', 'on_raw_update', 'Message', 'on_message', 'CallbackButton', 'on_callback_button', 'CallbackSelection', 'on_callback_selection', 'MessageStatus', 'on_message_status_change', 'list', 'InlineButton', 'SectionList', 'send_message', 'bytes', 'send_image', 'send_video', 'send_document', 'send_audio', 'send_sticker', 'send_reaction', 'remove_reaction', 'send_location', 'Contact', 'Iterable', 'send_contact', 'mark_message_as_read')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
          name       'WhatsApp'
          firstlineno 11
          lnotab
             0x0a050201020102010201020102f7040208fe020302fd020408fc020502
-            fb020608fa020702f9020802f8020912f708300c0702fe04023cfe081902
-            fd0402220116ff04fe081b02fd0402220116ff04fe081a02fd0402220116
-            ff04fe081a02fd0402220116ff04fe081b020102010201020102f8040202
-            fe020302fd020402fc020508fb02061afa020708f9020808f8020902f708
-            6c020102010201020102f8040202fe020308fd020408fc020508fb020614
-            fa020708f9020808f8020902f7083d020102010201020102f8040202fe02
+            fb020608fa020702f9020802f8020912f708300c05201320132013201320
+            17020102010201020102f8040202fe020302fd020402fc020508fb02061a
+            fa020708f9020808f8020902f7086c020102010201020102f8040202fe02
             0308fd020408fc020508fb020614fa020708f9020808f8020902f7083d02
-            01020102010201020102f7040202fe020308fd020408fc020508fb020608
-            fa020714f9020808f8020908f7084302fc040202fe020308fd020408fc02
-            0502fb0823020102fb040202fe020308fd020402fc020508fb020602fa08
-            24020202fe020302fd020402fc020502fb081f020202fe020302fd020402
-            fc081a020102fa040202fe020302fd020402fc020508fb020608fa020702
-            f9082802fc040202fe020314fd020408fc020502fb0824020202fe020302
-            fd
+            0102010201020102f8040202fe020308fd020408fc020508fb020614fa02
+            0708f9020808f8020902f7083d0201020102010201020102f7040202fe02
+            0308fd020408fc020508fb020608fa020714f9020808f8020908f7084302
+            fc040202fe020308fd020408fc020502fb0823020102fb040202fe020308
+            fd020402fc020508fb020602fa0824020202fe020302fd020402fc020502
+            fb081f020202fe020302fd020402fc081a020102fa040202fe020302fd02
+            0402fc020508fb020608fa020702f9082802fc040202fe020314fd020408
+            fc020502fb0824020202fe020302fd
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
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x9e619464 (Thu Jun 22 14:58:38 2023 UTC)
-files sz: 11023
+moddate:  0x6c819464 (Thu Jun 22 17:14:20 2023 UTC)
+files sz: 11021
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 16777216
    code
       0x970064005a00640164026c016d025a020100640164036c035a03640164
@@ -3057,32 +3057,32 @@
                       26 CALL                     0
          
          249          36 STORE_NAME               5 (data_equals)
          
          253          38 LOAD_NAME                4 (staticmethod)
          
          254          40 LOAD_CONST              14 (('matches', 'str', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]'))
-                      42 LOAD_CONST               7 (<code object data_starts_with, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 253>)
+                      42 LOAD_CONST               7 (<code object data_startswith, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 253>)
                       44 MAKE_FUNCTION            4 (annotations)
          
          253          46 PRECALL                  0
                       50 CALL                     0
          
-         254          60 STORE_NAME               6 (data_starts_with)
+         254          60 STORE_NAME               6 (data_startswith)
          
          258          62 LOAD_NAME                4 (staticmethod)
          
          259          64 LOAD_CONST              14 (('matches', 'str', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]'))
-                      66 LOAD_CONST               8 (<code object data_ends_with, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 258>)
+                      66 LOAD_CONST               8 (<code object data_endswith, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 258>)
                       68 MAKE_FUNCTION            4 (annotations)
          
          258          70 PRECALL                  0
                       74 CALL                     0
          
-         259          84 STORE_NAME               7 (data_ends_with)
+         259          84 STORE_NAME               7 (data_endswith)
          
          263          86 LOAD_NAME                4 (staticmethod)
          
          264          88 LOAD_CONST              14 (('matches', 'str', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]'))
                       90 LOAD_CONST               9 (<code object data_contains, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py", line 263>)
                       92 MAKE_FUNCTION            4 (annotations)
          
@@ -3298,15 +3298,15 @@
                      firstlineno 256
                      lnotab 0x
                names      ()
                varnames   ('matches',)
                freevars   ()
                cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       'data_starts_with'
+               name       'data_startswith'
                firstlineno 253
                lnotab 0x0403
             code
                argcount  : 0
                nlocals   : 1
                stacksize : 2
                flags     : 16777223
@@ -3397,15 +3397,15 @@
                      firstlineno 261
                      lnotab 0x
                names      ()
                varnames   ('matches',)
                freevars   ()
                cellvars   ('matches',)
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
-               name       'data_ends_with'
+               name       'data_endswith'
                firstlineno 258
                lnotab 0x0403
             code
                argcount  : 0
                nlocals   : 1
                stacksize : 2
                flags     : 16777223
@@ -3601,15 +3601,15 @@
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
                name       'data_regex'
                firstlineno 268
                lnotab 0x0406
             None
             ('matches', 'str', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]')
             ('patterns', 'str | re.Pattern', 'return', 'Callable[[Wa, CallbackButton | CallbackSelection], bool]')
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'staticmethod', 'data_equals', 'data_starts_with', 'data_ends_with', 'data_contains', 'data_regex')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'staticmethod', 'data_equals', 'data_startswith', 'data_endswith', 'data_contains', 'data_regex')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py'
          name       'CallbackFilter'
          firstlineno 245
          lnotab
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/handlers.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,231 +1,197 @@
 magic:    0xa70d0d0a
-moddate:  0x8c729164 (Tue Jun 20 09:34:04 2023 UTC)
-files sz: 1656
+moddate:  0xd7809464 (Thu Jun 22 17:11:51 2023 UTC)
+files sz: 1431
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a026d035a036d045a040100650372
-      06640064026c056d065a06010002004700640384006404a6020000ab0200
-      000000000000005a07020047006405840064066507a6030000ab03000000
-      00000000005a08020047006407840064086507a6030000ab030000000000
-      0000005a090200470064098400640a6507a6030000ab0300000000000000
-      005a0a02004700640b8400640c6507a6030000ab0300000000000000005a
-      0b02004700640d8400640e6507a6030000ab0300000000000000005a0c64
-      0f5300
+      0x9700640064016c006d015a016d025a026d035a03010065037206640064
+      026c046d055a05010002004700640384006404a6020000ab020000000000
+      0000005a06020047006405840064066506a6030000ab0300000000000000
+      005a07020047006407840064086506a6030000ab0300000000000000005a
+      080200470064098400640a6506a6030000ab0300000000000000005a0902
+      004700640b8400640c6506a6030000ab0300000000000000005a0a020047
+      00640d8400640e6506a6030000ab0300000000000000005a0b640f5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Callable', 'Any', 'TYPE_CHECKING', 'Iterable'))
+                 4 LOAD_CONST               1 (('Callable', 'Any', 'TYPE_CHECKING'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Callable)
                 10 STORE_NAME               1 (Callable)
                 12 IMPORT_FROM              2 (Any)
                 14 STORE_NAME               2 (Any)
                 16 IMPORT_FROM              3 (TYPE_CHECKING)
                 18 STORE_NAME               3 (TYPE_CHECKING)
-                20 IMPORT_FROM              4 (Iterable)
-                22 STORE_NAME               4 (Iterable)
-                24 POP_TOP
+                20 POP_TOP
    
-     3          26 LOAD_NAME                3 (TYPE_CHECKING)
-                28 POP_JUMP_FORWARD_IF_FALSE     6 (to 42)
+     3          22 LOAD_NAME                3 (TYPE_CHECKING)
+                24 POP_JUMP_FORWARD_IF_FALSE     6 (to 38)
    
-     4          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               2 (('WhatsApp',))
-                34 IMPORT_NAME              5 (pywa)
-                36 IMPORT_FROM              6 (WhatsApp)
-                38 STORE_NAME               6 (WhatsApp)
-                40 POP_TOP
+     4          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               2 (('WhatsApp',))
+                30 IMPORT_NAME              4 (pywa)
+                32 IMPORT_FROM              5 (WhatsApp)
+                34 STORE_NAME               5 (WhatsApp)
+                36 POP_TOP
    
-     7     >>   42 PUSH_NULL
-                44 LOAD_BUILD_CLASS
-                46 LOAD_CONST               3 (<code object Handler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 7>)
-                48 MAKE_FUNCTION            0
-                50 LOAD_CONST               4 ('Handler')
-                52 PRECALL                  2
-                56 CALL                     2
-                66 STORE_NAME               7 (Handler)
+     7     >>   38 PUSH_NULL
+                40 LOAD_BUILD_CLASS
+                42 LOAD_CONST               3 (<code object Handler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 7>)
+                44 MAKE_FUNCTION            0
+                46 LOAD_CONST               4 ('Handler')
+                48 PRECALL                  2
+                52 CALL                     2
+                62 STORE_NAME               6 (Handler)
    
-    33          68 PUSH_NULL
-                70 LOAD_BUILD_CLASS
-                72 LOAD_CONST               5 (<code object MessageHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 33>)
-                74 MAKE_FUNCTION            0
-                76 LOAD_CONST               6 ('MessageHandler')
-                78 LOAD_NAME                7 (Handler)
-                80 PRECALL                  3
-                84 CALL                     3
-                94 STORE_NAME               8 (MessageHandler)
+    33          64 PUSH_NULL
+                66 LOAD_BUILD_CLASS
+                68 LOAD_CONST               5 (<code object MessageHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 33>)
+                70 MAKE_FUNCTION            0
+                72 LOAD_CONST               6 ('MessageHandler')
+                74 LOAD_NAME                6 (Handler)
+                76 PRECALL                  3
+                80 CALL                     3
+                90 STORE_NAME               7 (MessageHandler)
    
-    38          96 PUSH_NULL
-                98 LOAD_BUILD_CLASS
-               100 LOAD_CONST               7 (<code object ButtonCallbackHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 38>)
-               102 MAKE_FUNCTION            0
-               104 LOAD_CONST               8 ('ButtonCallbackHandler')
-               106 LOAD_NAME                7 (Handler)
-               108 PRECALL                  3
-               112 CALL                     3
-               122 STORE_NAME               9 (ButtonCallbackHandler)
+    37          92 PUSH_NULL
+                94 LOAD_BUILD_CLASS
+                96 LOAD_CONST               7 (<code object ButtonCallbackHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 37>)
+                98 MAKE_FUNCTION            0
+               100 LOAD_CONST               8 ('ButtonCallbackHandler')
+               102 LOAD_NAME                6 (Handler)
+               104 PRECALL                  3
+               108 CALL                     3
+               118 STORE_NAME               8 (ButtonCallbackHandler)
    
-    43         124 PUSH_NULL
-               126 LOAD_BUILD_CLASS
-               128 LOAD_CONST               9 (<code object SelectionCallbackHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 43>)
-               130 MAKE_FUNCTION            0
-               132 LOAD_CONST              10 ('SelectionCallbackHandler')
-               134 LOAD_NAME                7 (Handler)
-               136 PRECALL                  3
-               140 CALL                     3
-               150 STORE_NAME              10 (SelectionCallbackHandler)
+    42         120 PUSH_NULL
+               122 LOAD_BUILD_CLASS
+               124 LOAD_CONST               9 (<code object SelectionCallbackHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 42>)
+               126 MAKE_FUNCTION            0
+               128 LOAD_CONST              10 ('SelectionCallbackHandler')
+               130 LOAD_NAME                6 (Handler)
+               132 PRECALL                  3
+               136 CALL                     3
+               146 STORE_NAME               9 (SelectionCallbackHandler)
    
-    48         152 PUSH_NULL
-               154 LOAD_BUILD_CLASS
-               156 LOAD_CONST              11 (<code object RawUpdateHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 48>)
-               158 MAKE_FUNCTION            0
-               160 LOAD_CONST              12 ('RawUpdateHandler')
-               162 LOAD_NAME                7 (Handler)
-               164 PRECALL                  3
-               168 CALL                     3
-               178 STORE_NAME              11 (RawUpdateHandler)
+    47         148 PUSH_NULL
+               150 LOAD_BUILD_CLASS
+               152 LOAD_CONST              11 (<code object RawUpdateHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 47>)
+               154 MAKE_FUNCTION            0
+               156 LOAD_CONST              12 ('RawUpdateHandler')
+               158 LOAD_NAME                6 (Handler)
+               160 PRECALL                  3
+               164 CALL                     3
+               174 STORE_NAME              10 (RawUpdateHandler)
    
-    53         180 PUSH_NULL
-               182 LOAD_BUILD_CLASS
-               184 LOAD_CONST              13 (<code object MessageStatusHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 53>)
-               186 MAKE_FUNCTION            0
-               188 LOAD_CONST              14 ('MessageStatusHandler')
-               190 LOAD_NAME                7 (Handler)
-               192 PRECALL                  3
-               196 CALL                     3
-               206 STORE_NAME              12 (MessageStatusHandler)
-               208 LOAD_CONST              15 (None)
-               210 RETURN_VALUE
+    52         176 PUSH_NULL
+               178 LOAD_BUILD_CLASS
+               180 LOAD_CONST              13 (<code object MessageStatusHandler, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 52>)
+               182 MAKE_FUNCTION            0
+               184 LOAD_CONST              14 ('MessageStatusHandler')
+               186 LOAD_NAME                6 (Handler)
+               188 PRECALL                  3
+               192 CALL                     3
+               202 STORE_NAME              11 (MessageStatusHandler)
+               204 LOAD_CONST              15 (None)
+               206 RETURN_VALUE
    consts
       0
-      ('Callable', 'Any', 'TYPE_CHECKING', 'Iterable')
+      ('Callable', 'Any', 'TYPE_CHECKING')
       ('WhatsApp',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 8
+         stacksize : 6
          flags     : 0
          code
-            0x970065005a0164005a0264015a0364025a040900640a64036505640465
-            066702650666021900000000000000000064056507650564046506670265
-            086602190000000000000000001900000000000000000065056404650667
-            0265086602190000000000000000007a07000064027a0700006604640684
-            055a0964076404640865066604640984045a0a64025300
+            0x970065005a0164005a0264015a0364025a046403650564046506670265
+            066602190000000000000000006405650564046506670265076602190000
+            000000000000006604640684045a0864076404640865066604640984045a
+            0964025300
            7           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Handler')
                        8 STORE_NAME               2 (__qualname__)
          
            8          10 LOAD_CONST               1 ('Base class for all handlers.')
                       12 STORE_NAME               3 (__doc__)
          
            9          14 LOAD_CONST               2 (None)
                       16 STORE_NAME               4 (__handler_type__)
          
-          14          18 NOP
+          11          18 LOAD_CONST               3 ('handler')
          
-          11          20 LOAD_CONST              10 ((None,))
-                      22 LOAD_CONST               3 ('handler')
-         
-          13          24 LOAD_NAME                5 (Callable)
-                      26 LOAD_CONST               4 ('WhatsApp')
+          13          20 LOAD_NAME                5 (Callable)
+                      22 LOAD_CONST               4 ('WhatsApp')
+                      24 LOAD_NAME                6 (Any)
+                      26 BUILD_LIST               2
                       28 LOAD_NAME                6 (Any)
-                      30 BUILD_LIST               2
-                      32 LOAD_NAME                6 (Any)
-                      34 BUILD_TUPLE              2
-                      36 BINARY_SUBSCR
-         
-          11          46 LOAD_CONST               5 ('filters')
-         
-          14          48 LOAD_NAME                7 (Iterable)
-                      50 LOAD_NAME                5 (Callable)
-                      52 LOAD_CONST               4 ('WhatsApp')
-                      54 LOAD_NAME                6 (Any)
-                      56 BUILD_LIST               2
-                      58 LOAD_NAME                8 (bool)
-                      60 BUILD_TUPLE              2
-                      62 BINARY_SUBSCR
-                      72 BINARY_SUBSCR
-                      82 LOAD_NAME                5 (Callable)
-                      84 LOAD_CONST               4 ('WhatsApp')
-                      86 LOAD_NAME                6 (Any)
-                      88 BUILD_LIST               2
-                      90 LOAD_NAME                8 (bool)
-                      92 BUILD_TUPLE              2
-                      94 BINARY_SUBSCR
-                     104 BINARY_OP                7 (|)
-                     108 LOAD_CONST               2 (None)
-                     110 BINARY_OP                7 (|)
-         
-          11         114 BUILD_TUPLE              4
-                     116 LOAD_CONST               6 (<code object __init__, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 11>)
-                     118 MAKE_FUNCTION            5 (defaults, annotations)
-                     120 STORE_NAME               9 (__init__)
-         
-          28         122 LOAD_CONST               7 ('wa')
-                     124 LOAD_CONST               4 ('WhatsApp')
-                     126 LOAD_CONST               8 ('data')
-                     128 LOAD_NAME                6 (Any)
-                     130 BUILD_TUPLE              4
-                     132 LOAD_CONST               9 (<code object __call__, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 28>)
-                     134 MAKE_FUNCTION            4 (annotations)
-                     136 STORE_NAME              10 (__call__)
-                     138 LOAD_CONST               2 (None)
-                     140 RETURN_VALUE
+                      30 BUILD_TUPLE              2
+                      32 BINARY_SUBSCR
+         
+          11          42 LOAD_CONST               5 ('filters')
+         
+          14          44 LOAD_NAME                5 (Callable)
+                      46 LOAD_CONST               4 ('WhatsApp')
+                      48 LOAD_NAME                6 (Any)
+                      50 BUILD_LIST               2
+                      52 LOAD_NAME                7 (bool)
+                      54 BUILD_TUPLE              2
+                      56 BINARY_SUBSCR
+         
+          11          66 BUILD_TUPLE              4
+                      68 LOAD_CONST               6 (<code object __init__, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 11>)
+                      70 MAKE_FUNCTION            4 (annotations)
+                      72 STORE_NAME               8 (__init__)
+         
+          28          74 LOAD_CONST               7 ('wa')
+                      76 LOAD_CONST               4 ('WhatsApp')
+                      78 LOAD_CONST               8 ('data')
+                      80 LOAD_NAME                6 (Any)
+                      82 BUILD_TUPLE              4
+                      84 LOAD_CONST               9 (<code object __call__, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 28>)
+                      86 MAKE_FUNCTION            4 (annotations)
+                      88 STORE_NAME               9 (__call__)
+                      90 LOAD_CONST               2 (None)
+                      92 RETURN_VALUE
          consts
             'Handler'
             'Base class for all handlers.'
             None
             'handler'
             'WhatsApp'
             'filters'
             code
-               argcount  : 3
+               argcount  : 2
                nlocals   : 3
-               stacksize : 4
-               flags     : 3
+               stacksize : 2
+               flags     : 7
                code
-                  0x97007c017c005f0000000000000000007403000000000000000000007c
-                  02740400000000000000000000a6020000ab02000000000000000072027c
-                  026e067c0272037c0266016e0164017c005f030000000000000000640153
-                  00
+                  0x97007c017c005f0000000000000000007c027c005f0100000000000000
+                  0064015300
                 11           0 RESUME                   0
                
                 25           2 LOAD_FAST                1 (handler)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (handler)
                
-                26          16 LOAD_GLOBAL              3 (NULL + isinstance)
-                            28 LOAD_FAST                2 (filters)
-                            30 LOAD_GLOBAL              4 (Iterable)
-                            42 PRECALL                  2
-                            46 CALL                     2
-                            56 POP_JUMP_FORWARD_IF_FALSE     2 (to 62)
-                            58 LOAD_FAST                2 (filters)
-                            60 JUMP_FORWARD             6 (to 74)
-                       >>   62 LOAD_FAST                2 (filters)
-                            64 POP_JUMP_FORWARD_IF_FALSE     3 (to 72)
-                            66 LOAD_FAST                2 (filters)
-                            68 BUILD_TUPLE              1
-                            70 JUMP_FORWARD             1 (to 74)
-                       >>   72 LOAD_CONST               1 (None)
-                       >>   74 LOAD_FAST                0 (self)
-                            76 STORE_ATTR               3 (filters)
-                            86 LOAD_CONST               1 (None)
-                            88 RETURN_VALUE
+                26          16 LOAD_FAST                2 (filters)
+                            18 LOAD_FAST                0 (self)
+                            20 STORE_ATTR               1 (filters)
+                            30 LOAD_CONST               1 (None)
+                            32 RETURN_VALUE
                consts
-                  '\n        Initialize a new handler.\n\n        Args:\n            handler: The handler function. (gets the WhatsApp instance and the data as\n                arguments)\n            filters: A list of filters to apply to the handler. (filter functions get the WhatsApp instance and the\n                data as arguments and return a boolean value)\n        '
+                  '\n        Initialize a new handler.\n\n        Args:\n            handler: The handler function. (gets the WhatsApp instance and the data as\n                arguments)\n            filters: The filters to apply to the handler. (gets the WhatsApp instance and\n                the data as arguments and returns a boolean)\n        '
                   None
-               names      ('handler', 'isinstance', 'Iterable', 'filters')
+               names      ('handler', 'filters')
                varnames   ('self', 'handler', 'filters')
                freevars   ()
                cellvars   ()
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
                name       '__init__'
                firstlineno 11
                lnotab 0x020e0e01
@@ -233,56 +199,51 @@
             'data'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
-                  0x8701870297007c006a0000000000000000007222740300000000000000
-                  000000880288016602640184087c006a0000000000000000004400a60000
-                  00ab000000000000000000a6010000ab010000000000000000721a6e0109
-                  007c00a002000000000000000000000000000000000000000089018902a6
-                  020000ab02000000000000000001006400530064005300
+                  0x870187029700740100000000000000000000880288016602640184087c
+                  006a0100000000000000004400a6000000ab000000000000000000a60100
+                  00ab01000000000000000072187c00a00200000000000000000000000000
+                  0000000000000089018902a6020000ab0200000000000000000100640053
+                  0064005300
                              0 MAKE_CELL                1 (wa)
                              2 MAKE_CELL                2 (data)
                
                 28           4 RESUME                   0
                
-                29           6 LOAD_FAST                0 (self)
-                             8 LOAD_ATTR                0 (filters)
-                            18 POP_JUMP_FORWARD_IF_FALSE    34 (to 88)
-                            20 LOAD_GLOBAL              3 (NULL + all)
-                            32 LOAD_CLOSURE             2 (data)
-                            34 LOAD_CLOSURE             1 (wa)
-                            36 BUILD_TUPLE              2
-                            38 LOAD_CONST               1 (<code object <listcomp>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 29>)
-                            40 MAKE_FUNCTION            8 (closure)
-                            42 LOAD_FAST                0 (self)
-                            44 LOAD_ATTR                0 (filters)
-                            54 GET_ITER
-                            56 PRECALL                  0
-                            60 CALL                     0
-                            70 PRECALL                  1
-                            74 CALL                     1
-                            84 POP_JUMP_FORWARD_IF_FALSE    26 (to 138)
-                            86 JUMP_FORWARD             1 (to 90)
-                       >>   88 NOP
+                29           6 LOAD_GLOBAL              1 (NULL + all)
+                            18 LOAD_CLOSURE             2 (data)
+                            20 LOAD_CLOSURE             1 (wa)
+                            22 BUILD_TUPLE              2
+                            24 LOAD_CONST               1 (<code object <listcomp>, file "/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py", line 29>)
+                            26 MAKE_FUNCTION            8 (closure)
+                            28 LOAD_FAST                0 (self)
+                            30 LOAD_ATTR                1 (filters)
+                            40 GET_ITER
+                            42 PRECALL                  0
+                            46 CALL                     0
+                            56 PRECALL                  1
+                            60 CALL                     1
+                            70 POP_JUMP_FORWARD_IF_FALSE    24 (to 120)
                
-                30     >>   90 LOAD_FAST                0 (self)
-                            92 LOAD_METHOD              2 (handler)
-                           114 LOAD_DEREF               1 (wa)
-                           116 LOAD_DEREF               2 (data)
-                           118 PRECALL                  2
-                           122 CALL                     2
-                           132 POP_TOP
-                           134 LOAD_CONST               0 (None)
-                           136 RETURN_VALUE
+                30          72 LOAD_FAST                0 (self)
+                            74 LOAD_METHOD              2 (handler)
+                            96 LOAD_DEREF               1 (wa)
+                            98 LOAD_DEREF               2 (data)
+                           100 PRECALL                  2
+                           104 CALL                     2
+                           114 POP_TOP
+                           116 LOAD_CONST               0 (None)
+                           118 RETURN_VALUE
                
-                29     >>  138 LOAD_CONST               0 (None)
-                           140 RETURN_VALUE
+                29     >>  120 LOAD_CONST               0 (None)
+                           122 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
@@ -310,184 +271,182 @@
                      varnames   ('.0', 'f')
                      freevars   ('data', 'wa')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
                      name       '<listcomp>'
                      firstlineno 29
                      lnotab 0x
-               names      ('filters', 'all', 'handler')
+               names      ('all', 'filters', 'handler')
                varnames   ('self', 'wa', 'data')
                freevars   ()
                cellvars   ('wa', 'data')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
                name       '__call__'
                firstlineno 28
-               lnotab 0x0601540130ff
-            (None,)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', '__handler_type__', 'Callable', 'Any', 'Iterable', 'bool', '__init__', '__call__')
+               lnotab 0x0601420130ff
+         names      ('__name__', '__module__', '__qualname__', '__doc__', '__handler_type__', 'Callable', 'Any', 'bool', '__init__', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
          name       'Handler'
          firstlineno 7
-         lnotab 0x0a010401040502fd040216fe020342fd0811
+         lnotab 0x0a0104010402020216fe020316fd0811
       'Handler'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
           33           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MessageHandler')
                        8 STORE_NAME               2 (__qualname__)
          
-          34          10 LOAD_CONST               1 ('message')
-                      12 STORE_NAME               3 (__handler_type__)
-         
-          35          14 LOAD_CONST               2 (None)
+          34          10 LOAD_CONST               1 ('A message handler (e.g. text, image, video, audio, etc.).')
+                      12 STORE_NAME               3 (__doc__)
+                      14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'MessageHandler'
-            'message'
+            'A message handler (e.g. text, image, video, audio, etc.).'
             None
-         names      ('__name__', '__module__', '__qualname__', '__handler_type__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
          name       'MessageHandler'
          firstlineno 33
-         lnotab 0x0a010401
+         lnotab 0x0a01
       'MessageHandler'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-          38           0 RESUME                   0
+          37           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ButtonCallbackHandler')
                        8 STORE_NAME               2 (__qualname__)
          
-          39          10 LOAD_CONST               1 ('button')
+          38          10 LOAD_CONST               1 ('button')
                       12 STORE_NAME               3 (__handler_type__)
          
-          40          14 LOAD_CONST               2 (None)
+          39          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'ButtonCallbackHandler'
             'button'
             None
          names      ('__name__', '__module__', '__qualname__', '__handler_type__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
          name       'ButtonCallbackHandler'
-         firstlineno 38
+         firstlineno 37
          lnotab 0x0a010401
       'ButtonCallbackHandler'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-          43           0 RESUME                   0
+          42           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SelectionCallbackHandler')
                        8 STORE_NAME               2 (__qualname__)
          
-          44          10 LOAD_CONST               1 ('selection')
+          43          10 LOAD_CONST               1 ('selection')
                       12 STORE_NAME               3 (__handler_type__)
          
-          45          14 LOAD_CONST               2 (None)
+          44          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'SelectionCallbackHandler'
             'selection'
             None
          names      ('__name__', '__module__', '__qualname__', '__handler_type__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
          name       'SelectionCallbackHandler'
-         firstlineno 43
+         firstlineno 42
          lnotab 0x0a010401
       'SelectionCallbackHandler'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-          48           0 RESUME                   0
+          47           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('RawUpdateHandler')
                        8 STORE_NAME               2 (__qualname__)
          
-          49          10 LOAD_CONST               1 ('raw_update')
+          48          10 LOAD_CONST               1 ('raw_update')
                       12 STORE_NAME               3 (__handler_type__)
          
-          50          14 LOAD_CONST               2 (None)
+          49          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'RawUpdateHandler'
             'raw_update'
             None
          names      ('__name__', '__module__', '__qualname__', '__handler_type__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
          name       'RawUpdateHandler'
-         firstlineno 48
+         firstlineno 47
          lnotab 0x0a010401
       'RawUpdateHandler'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-          53           0 RESUME                   0
+          52           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MessageStatusHandler')
                        8 STORE_NAME               2 (__qualname__)
          
-          54          10 LOAD_CONST               1 ('message_status')
+          53          10 LOAD_CONST               1 ('message_status')
                       12 STORE_NAME               3 (__handler_type__)
          
-          55          14 LOAD_CONST               2 (None)
+          54          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'MessageStatusHandler'
             'message_status'
             None
          names      ('__name__', '__module__', '__qualname__', '__handler_type__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
          name       'MessageStatusHandler'
-         firstlineno 53
+         firstlineno 52
          lnotab 0x0a010401
       'MessageStatusHandler'
       None
-   names      ('typing', 'Callable', 'Any', 'TYPE_CHECKING', 'Iterable', 'pywa', 'WhatsApp', 'Handler', 'MessageHandler', 'ButtonCallbackHandler', 'SelectionCallbackHandler', 'RawUpdateHandler', 'MessageStatusHandler')
+   names      ('typing', 'Callable', 'Any', 'TYPE_CHECKING', 'pywa', 'WhatsApp', 'Handler', 'MessageHandler', 'ButtonCallbackHandler', 'SelectionCallbackHandler', 'RawUpdateHandler', 'MessageStatusHandler')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201180204010c031a1a1c051c051c051c05
+   lnotab 0x00ff0201140204010c031a1a1c041c051c051c05
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py

```diff
@@ -58,126 +58,106 @@
             self._handlers = None
 
     def add_handler(self, handler: Handler):
         if self._handlers is None:
             raise ValueError("You must initialize the WhatsApp client with an app (Flask or FastAPI) to add handlers.")
         self._handlers[handler.__handler_type__].append(handler)
 
-    def on_raw_update(
-            self,
-            filters: Iterable[Callable[["WhatsApp", dict], bool]] | Callable[["WhatsApp", dict], bool] = None
-    ):
+    def on_raw_update(self, *filters: Callable[["WhatsApp", dict], bool]):
         """
         Decorator to register a function as a handler for raw updates.
 
         Example:
 
             >>> @wa.on_raw_update()
             ... def raw_update_handler(wa: WhatsApp, update: dict):
             ...     print(update)
 
         Args:
             filters: Filters to apply to the incoming updates (filters are function that take the WhatsApp client and
                 the incoming update and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", dict], Any]):
-            self.add_handler(RawUpdateHandler(handler=func, filters=filters))
+            self.add_handler(RawUpdateHandler(handler=func, *filters))
             return func
         return decorator
 
-    def on_message(
-            self,
-            filters: Iterable[Callable[["WhatsApp", Message], bool]] |
-            Callable[["WhatsApp", Message], bool] = None
-    ):
+    def on_message(self, *filters: Callable[["WhatsApp", Message], bool]):
         """
         Decorator to register a function as a handler for incoming messages.
 
         Example:
-
-            >>> @wa.on_message(filters=TextFilter.EQUALS(("hello", "hi"))
+            >>> @wa.on_message(TextFilter.equals("hello", "hi")
             ... def hello_handler(wa: WhatsApp, msg: Message):
             ...     msg.react("👋")
             ...     msg.reply_text(text="Hello from PyWa!", quote=True, buttons=[InlineButton("Help", data="help")
 
         Args:
             filters: Filters to apply to the incoming messages (filters are function that take the WhatsApp client and
                 the incoming message and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", Message], Any]):
-            self.add_handler(MessageHandler(handler=func, filters=filters))
+            self.add_handler(MessageHandler(handler=func, *filters))
             return func
         return decorator
 
-    def on_callback_button(
-            self,
-            filters: Iterable[Callable[["WhatsApp", CallbackButton], bool]] |
-            Callable[["WhatsApp", CallbackButton], bool] = None
-    ):
+    def on_callback_button(self, *filters: Callable[["WhatsApp", CallbackButton], bool]):
         """
         Decorator to register a function as a handler for incoming callback button presses.
 
         Example:
 
-            >>> @wa.on_callback_button(filters=CallbackFilter.DATA_EQUALS("help"))
+            >>> @wa.on_callback_button(CallbackFilter.data_equals("help"))
             ... def help_handler(wa: WhatsApp, btn: CallbackButton):
             ...     btn.reply_text(text="What can I help you with?")
 
         Args:
             filters: Filters to apply to the incoming callback button presses (filters are function that take the
                 WhatsApp client and the incoming callback button and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", CallbackButton], Any]):
-            self.add_handler(ButtonCallbackHandler(handler=func, filters=filters))
+            self.add_handler(ButtonCallbackHandler(handler=func, *filters))
             return func
         return decorator
 
-    def on_callback_selection(
-            self,
-            filters: Iterable[Callable[["WhatsApp", CallbackSelection], bool]] |
-            Callable[["WhatsApp", CallbackSelection], bool] = None
-    ):
+    def on_callback_selection(self, *filters: Callable[["WhatsApp", CallbackSelection], bool]):
         """
         Decorator to register a function as a handler for incoming callback selections.
 
         Example:
 
-            >>> @wa.on_callback_selection(filters=CallbackFilter.DATA_STARTS_WITH("id:"))
+            >>> @wa.on_callback_selection(CallbackFilter.data_startswith("id:"))
             ... def id_handler(wa: WhatsApp, sel: CallbackSelection):
             ...     sel.reply_text(text=f"Your ID is {sel.data.split(':', 1)[1]}")
 
         Args:
             filters: Filters to apply to the incoming callback selections (filters are function that take the
                 WhatsApp client and the incoming callback selection and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", CallbackSelection], Any]):
-            self.add_handler(SelectionCallbackHandler(handler=func, filters=filters))
+            self.add_handler(SelectionCallbackHandler(handler=func, *filters))
             return func
         return decorator
 
-    def on_message_status_change(
-            self,
-            filters: Iterable[Callable[["WhatsApp", MessageStatus], bool]] |
-            Callable[["WhatsApp", MessageStatus], bool] = None
-    ):
+    def on_message_status_change(self, *filters: Callable[["WhatsApp", MessageStatus], bool]):
         """
         Decorator to register a function as a handler for incoming message status changes.
 
         Example:
 
-            >>> @wa.on_message_status_change(filters=MessageStatusFilter.READ)
+            >>> @wa.on_message_status_change(MessageStatusFilter.READ)
             ... def delivered_handler(wa: WhatsApp, status: MessageStatus):
             ...     print(f"Message {status.id} was read by {status.from_user.wa_id}")
 
         Args:
             filters: Filters to apply to the incoming message status changes (filters are function that take the
                 WhatsApp client and the incoming message status change and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", MessageStatus], Any]):
-            self.add_handler(MessageStatusHandler(handler=func, filters=filters))
+            self.add_handler(MessageStatusHandler(handler=func, *filters))
             return func
         return decorator
 
     def send_message(
             self,
             to: str,
             text: str,
@@ -658,8 +638,8 @@
 
         Args:
             message_id: The message ID to mark as read.
 
         Returns:
             Whether the message was marked as read.
         """
-        return self.api.mark_message_as_read(message_id=message_id)
+        return self.api.mark_message_as_read(message_id=message_id)
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py

```diff
@@ -247,20 +247,20 @@
 
     @staticmethod
     def data_equals(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
         """Filter for callbacks their data equals the given string/s."""
         return lambda wa, c: any((c.data == m for m in matches))
 
     @staticmethod
-    def data_starts_with(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
+    def data_startswith(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
         """Filter for callbacks their data starts with the given string/s."""
         return lambda wa, c: any((c.data.startswith(m) for m in matches))
 
     @staticmethod
-    def data_ends_with(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
+    def data_endswith(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
         """Filter for callbacks their data ends with the given string/s."""
         return lambda wa, c: any((c.data.endswith(m) for m in matches))
 
     @staticmethod
     def data_contains(*matches: str) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
         """Filter for callbacks their data contains the given string/s."""
         return lambda wa, c: any((m in c.data for m in matches))
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py

```diff
@@ -1,41 +1,40 @@
-from typing import Callable, Any, TYPE_CHECKING, Iterable
+from typing import Callable, Any, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pywa import WhatsApp
 
 
 class Handler:
     """Base class for all handlers."""
     __handler_type__ = None
 
     def __init__(
             self,
             handler: Callable[["WhatsApp", Any], Any],
-            filters: Iterable[Callable[["WhatsApp", Any], bool]] | Callable[["WhatsApp", Any], bool] | None = None
+            *filters: Callable[["WhatsApp", Any], bool]
     ):
         """
         Initialize a new handler.
 
         Args:
             handler: The handler function. (gets the WhatsApp instance and the data as
                 arguments)
-            filters: A list of filters to apply to the handler. (filter functions get the WhatsApp instance and the
-                data as arguments and return a boolean value)
+            filters: The filters to apply to the handler. (gets the WhatsApp instance and
+                the data as arguments and returns a boolean)
         """
         self.handler = handler
-        self.filters = filters if isinstance(filters, Iterable) else (filters,) if filters else None
+        self.filters = filters
 
     def __call__(self, wa: "WhatsApp", data: Any):
-        if all([f(wa, data) for f in self.filters]) if self.filters else True:
+        if all([f(wa, data) for f in self.filters]):
             self.handler(wa, data)
 
 
 class MessageHandler(Handler):
-    __handler_type__ = "message"
     """A message handler (e.g. text, image, video, audio, etc.)."""
 
 
 class ButtonCallbackHandler(Handler):
     __handler_type__ = "button"
     """A button handler."""
```

### Comparing `./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc3-py3.11.egg-info/PKG-INFO` & `./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
@@ -82,30 +82,30 @@
 wa = WhatsApp(
     phone_id='1234567890',
     token='xxxxxxxxxxxxxxx',
     app=flask_app,
     verify_token='XYZXYZ',
 )
 
-@wa.on_message(filters=TextFilter.EQUALS(('Hello', 'Hi')))
+@wa.on_message(TextFilter.equals('Hello', 'Hi'))
 def hello(client: WhatsApp, message: Message):
     message.react('👋')
     message.reply_text(
         text='Hello from PyWa!',
         keyboard=[
             InlineButton(
                 title='Click me!',
-                callback_data='click_me'
+                callback_data='id:123'
             )
         ]
     )
 
-@wa.on_callback_button(filters=CallbackFilter.DATA_EQUALS('click_me'))
+@wa.on_callback_button(CallbackFilter.data_starts_with('id:'))
 def click_me(client: WhatsApp, clb: CallbackButton):
-    clb.reply_text('You clicked me!', quote=True)
+    clb.reply_text('You clicked me!')
 
 flask_app.run()  # Run the flask app to start the webhook
 ```
 
 ## Getting started
 - Back to [Contents](#contents)
```

