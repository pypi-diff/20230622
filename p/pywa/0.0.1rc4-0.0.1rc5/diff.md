# Comparing `tmp/pywa-0.0.1rc4.linux-x86_64.tar.gz` & `tmp/pywa-0.0.1rc5.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywa-0.0.1rc4.linux-x86_64.tar", last modified: Thu Jun 22 17:16:46 2023, max compression
+gzip compressed data, was "pywa-0.0.1rc5.linux-x86_64.tar", last modified: Thu Jun 22 18:17:18 2023, max compression
```

## Comparing `pywa-0.0.1rc4.linux-x86_64.tar` & `pywa-0.0.1rc5.linux-x86_64.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.579762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/
--rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-22 17:14:20.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.567762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/
--rw-rw-r--   0 david     (1000) david     (1000)      388 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    10696 2023-06-22 17:16:46.563762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/api.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    25954 2023-06-22 17:16:46.567762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/client.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     1849 2023-06-22 17:16:46.563762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/errors.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    26788 2023-06-22 17:16:46.567762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/filters.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     3166 2023-06-22 17:16:46.567762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/handlers.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)    41016 2023-06-22 17:16:46.563762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/types.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     2153 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 david     (1000) david     (1000)     6136 2023-06-22 17:16:46.559762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/webhook.cpython-311.pyc
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.544508 ./
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.544508 ./home/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.548508 ./home/david/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.548508 ./home/david/Documents/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.548508 ./home/david/Documents/private/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.548508 ./home/david/Documents/private/python/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.548508 ./home/david/Documents/private/python/pywa/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.548508 ./home/david/Documents/private/python/pywa/venv/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.548508 ./home/david/Documents/private/python/pywa/venv/lib/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.548508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.572508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.548508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/
+-rw-rw-r--   0 david     (1000) david     (1000)      143 2023-06-22 18:15:47.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.560508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/
+-rw-rw-r--   0 david     (1000) david     (1000)      388 2023-06-22 18:17:18.548508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    10696 2023-06-22 18:17:18.556508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/api.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    25976 2023-06-22 18:17:18.560508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/client.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     1849 2023-06-22 18:17:18.556508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/errors.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    26788 2023-06-22 18:17:18.556508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/filters.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     3166 2023-06-22 18:17:18.560508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/handlers.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)    41016 2023-06-22 18:17:18.556508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/types.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     2153 2023-06-22 18:17:18.548508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/utils.cpython-311.pyc
+-rw-rw-r--   0 david     (1000) david     (1000)     6136 2023-06-22 18:17:18.552508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/webhook.cpython-311.pyc
 -rw-rw-r--   0 david     (1000) david     (1000)     7965 2023-06-22 15:59:56.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/api.py
--rw-rw-r--   0 david     (1000) david     (1000)    23198 2023-06-22 17:11:51.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py
+-rw-rw-r--   0 david     (1000) david     (1000)    23158 2023-06-22 18:15:47.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py
 -rw-rw-r--   0 david     (1000) david     (1000)      989 2023-06-19 21:14:34.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/errors.py
 -rw-rw-r--   0 david     (1000) david     (1000)    11021 2023-06-22 17:14:20.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/filters.py
--rw-rw-r--   0 david     (1000) david     (1000)     1431 2023-06-22 17:11:51.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1431 2023-06-22 18:15:02.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/handlers.py
 -rw-rw-r--   0 david     (1000) david     (1000)    25776 2023-06-22 15:59:56.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/types.py
 -rw-rw-r--   0 david     (1000) david     (1000)      991 2023-06-20 16:58:34.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/utils.py
 -rw-rw-r--   0 david     (1000) david     (1000)     4141 2023-06-20 09:37:01.000000 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/webhook.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 17:16:46.579762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     9996 2023-06-22 17:16:46.575762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      301 2023-06-22 17:16:46.579762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-22 17:16:46.575762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       51 2023-06-22 17:16:46.575762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        5 2023-06-22 17:16:46.575762 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-22 18:17:18.572508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc5-py3.11.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)    10051 2023-06-22 18:17:18.568508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc5-py3.11.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      301 2023-06-22 18:17:18.572508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc5-py3.11.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-22 18:17:18.568508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc5-py3.11.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       51 2023-06-22 18:17:18.568508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc5-py3.11.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        5 2023-06-22 18:17:18.568508 ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc5-py3.11.egg-info/top_level.txt
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Python wrapper for the WhatsApp Cloud API. https://github.com/david-lev/pywa"""
 
-__version__ = "0.0.1rc4"
+__version__ = "0.0.1rc5"
 
 from pywa.client import WhatsApp
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/__init__.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,35 +1,35 @@
 magic:    0xa70d0d0a
-moddate:  0x6c819464 (Thu Jun 22 17:14:20 2023 UTC)
+moddate:  0xd38f9464 (Thu Jun 22 18:15:47 2023 UTC)
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
    
-     3           6 LOAD_CONST               1 ('0.0.1rc4')
+     3           6 LOAD_CONST               1 ('0.0.1rc5')
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
-      '0.0.1rc4'
+      '0.0.1rc5'
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
-moddate:  0xd7809464 (Thu Jun 22 17:11:51 2023 UTC)
-files sz: 23198
+moddate:  0xd38f9464 (Thu Jun 22 18:15:47 2023 UTC)
+files sz: 23158
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a036d
@@ -914,49 +914,49 @@
                consts
                   '\n        Decorator to register a function as a handler for raw updates.\n\n        Example:\n\n            >>> @wa.on_raw_update()\n            ... def raw_update_handler(wa: WhatsApp, update: dict):\n            ...     print(update)\n\n        Args:\n            filters: Filters to apply to the incoming updates (filters are function that take the WhatsApp client and\n                the incoming update and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 7
+                     stacksize : 6
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        0300000000000000000000890164017c0069018e01a6010000ab01000000
-                        000000000001007c005300
+                        03000000000000000000007c0067018901a20152008e00a6010000ab0100
+                        0000000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
                       79           2 RESUME                   0
                      
                       80           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + RawUpdateHandler)
-                                  40 LOAD_DEREF               1 (filters)
-                                  42 LOAD_CONST               1 ('handler')
-                                  44 LOAD_FAST                0 (func)
-                                  46 BUILD_MAP                1
-                                  48 CALL_FUNCTION_EX         1
-                                  50 PRECALL                  1
-                                  54 CALL                     1
-                                  64 POP_TOP
+                                  40 LOAD_FAST                0 (func)
+                                  42 BUILD_LIST               1
+                                  44 LOAD_DEREF               1 (filters)
+                                  46 LIST_EXTEND              1
+                                  48 LIST_TO_TUPLE
+                                  50 CALL_FUNCTION_EX         0
+                                  52 PRECALL                  1
+                                  56 CALL                     1
+                                  66 POP_TOP
                      
-                      81          66 LOAD_FAST                0 (func)
-                                  68 RETURN_VALUE
+                      81          68 LOAD_FAST                0 (func)
+                                  70 RETURN_VALUE
                      consts
                         None
-                        'handler'
                      names      ('add_handler', 'RawUpdateHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
                      firstlineno 79
-                     lnotab 0x04013e01
+                     lnotab 0x04014001
                names      ('Callable', 'dict', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_raw_update'
                firstlineno 65
@@ -996,49 +996,49 @@
                consts
                   '\n        Decorator to register a function as a handler for incoming messages.\n\n        Example:\n            >>> @wa.on_message(TextFilter.equals("hello", "hi")\n            ... def hello_handler(wa: WhatsApp, msg: Message):\n            ...     msg.react("👋")\n            ...     msg.reply_text(text="Hello from PyWa!", quote=True, buttons=[InlineButton("Help", data="help")\n\n        Args:\n            filters: Filters to apply to the incoming messages (filters are function that take the WhatsApp client and\n                the incoming message and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 7
+                     stacksize : 6
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        0300000000000000000000890164017c0069018e01a6010000ab01000000
-                        000000000001007c005300
+                        03000000000000000000007c0067018901a20152008e00a6010000ab0100
+                        0000000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
                       98           2 RESUME                   0
                      
                       99           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + MessageHandler)
-                                  40 LOAD_DEREF               1 (filters)
-                                  42 LOAD_CONST               1 ('handler')
-                                  44 LOAD_FAST                0 (func)
-                                  46 BUILD_MAP                1
-                                  48 CALL_FUNCTION_EX         1
-                                  50 PRECALL                  1
-                                  54 CALL                     1
-                                  64 POP_TOP
+                                  40 LOAD_FAST                0 (func)
+                                  42 BUILD_LIST               1
+                                  44 LOAD_DEREF               1 (filters)
+                                  46 LIST_EXTEND              1
+                                  48 LIST_TO_TUPLE
+                                  50 CALL_FUNCTION_EX         0
+                                  52 PRECALL                  1
+                                  56 CALL                     1
+                                  66 POP_TOP
                      
-                     100          66 LOAD_FAST                0 (func)
-                                  68 RETURN_VALUE
+                     100          68 LOAD_FAST                0 (func)
+                                  70 RETURN_VALUE
                      consts
                         None
-                        'handler'
                      names      ('add_handler', 'MessageHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
                      firstlineno 98
-                     lnotab 0x04013e01
+                     lnotab 0x04014001
                names      ('Callable', 'Message', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_message'
                firstlineno 84
@@ -1078,49 +1078,49 @@
                consts
                   '\n        Decorator to register a function as a handler for incoming callback button presses.\n\n        Example:\n\n            >>> @wa.on_callback_button(CallbackFilter.data_equals("help"))\n            ... def help_handler(wa: WhatsApp, btn: CallbackButton):\n            ...     btn.reply_text(text="What can I help you with?")\n\n        Args:\n            filters: Filters to apply to the incoming callback button presses (filters are function that take the\n                WhatsApp client and the incoming callback button and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 7
+                     stacksize : 6
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        0300000000000000000000890164017c0069018e01a6010000ab01000000
-                        000000000001007c005300
+                        03000000000000000000007c0067018901a20152008e00a6010000ab0100
+                        0000000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
                      117           2 RESUME                   0
                      
                      118           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + ButtonCallbackHandler)
-                                  40 LOAD_DEREF               1 (filters)
-                                  42 LOAD_CONST               1 ('handler')
-                                  44 LOAD_FAST                0 (func)
-                                  46 BUILD_MAP                1
-                                  48 CALL_FUNCTION_EX         1
-                                  50 PRECALL                  1
-                                  54 CALL                     1
-                                  64 POP_TOP
+                                  40 LOAD_FAST                0 (func)
+                                  42 BUILD_LIST               1
+                                  44 LOAD_DEREF               1 (filters)
+                                  46 LIST_EXTEND              1
+                                  48 LIST_TO_TUPLE
+                                  50 CALL_FUNCTION_EX         0
+                                  52 PRECALL                  1
+                                  56 CALL                     1
+                                  66 POP_TOP
                      
-                     119          66 LOAD_FAST                0 (func)
-                                  68 RETURN_VALUE
+                     119          68 LOAD_FAST                0 (func)
+                                  70 RETURN_VALUE
                      consts
                         None
-                        'handler'
                      names      ('add_handler', 'ButtonCallbackHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
                      firstlineno 117
-                     lnotab 0x04013e01
+                     lnotab 0x04014001
                names      ('Callable', 'CallbackButton', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_callback_button'
                firstlineno 103
@@ -1160,49 +1160,49 @@
                consts
                   '\n        Decorator to register a function as a handler for incoming callback selections.\n\n        Example:\n\n            >>> @wa.on_callback_selection(CallbackFilter.data_startswith("id:"))\n            ... def id_handler(wa: WhatsApp, sel: CallbackSelection):\n            ...     sel.reply_text(text=f"Your ID is {sel.data.split(\':\', 1)[1]}")\n\n        Args:\n            filters: Filters to apply to the incoming callback selections (filters are function that take the\n                WhatsApp client and the incoming callback selection and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 7
+                     stacksize : 6
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        0300000000000000000000890164017c0069018e01a6010000ab01000000
-                        000000000001007c005300
+                        03000000000000000000007c0067018901a20152008e00a6010000ab0100
+                        0000000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
                      136           2 RESUME                   0
                      
                      137           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + SelectionCallbackHandler)
-                                  40 LOAD_DEREF               1 (filters)
-                                  42 LOAD_CONST               1 ('handler')
-                                  44 LOAD_FAST                0 (func)
-                                  46 BUILD_MAP                1
-                                  48 CALL_FUNCTION_EX         1
-                                  50 PRECALL                  1
-                                  54 CALL                     1
-                                  64 POP_TOP
+                                  40 LOAD_FAST                0 (func)
+                                  42 BUILD_LIST               1
+                                  44 LOAD_DEREF               1 (filters)
+                                  46 LIST_EXTEND              1
+                                  48 LIST_TO_TUPLE
+                                  50 CALL_FUNCTION_EX         0
+                                  52 PRECALL                  1
+                                  56 CALL                     1
+                                  66 POP_TOP
                      
-                     138          66 LOAD_FAST                0 (func)
-                                  68 RETURN_VALUE
+                     138          68 LOAD_FAST                0 (func)
+                                  70 RETURN_VALUE
                      consts
                         None
-                        'handler'
                      names      ('add_handler', 'SelectionCallbackHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
                      firstlineno 136
-                     lnotab 0x04013e01
+                     lnotab 0x04014001
                names      ('Callable', 'CallbackSelection', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_callback_selection'
                firstlineno 122
@@ -1242,49 +1242,49 @@
                consts
                   '\n        Decorator to register a function as a handler for incoming message status changes.\n\n        Example:\n\n            >>> @wa.on_message_status_change(MessageStatusFilter.READ)\n            ... def delivered_handler(wa: WhatsApp, status: MessageStatus):\n            ...     print(f"Message {status.id} was read by {status.from_user.wa_id}")\n\n        Args:\n            filters: Filters to apply to the incoming message status changes (filters are function that take the\n                WhatsApp client and the incoming message status change and return a boolean).\n        '
                   'func'
                   'WhatsApp'
                   code
                      argcount  : 1
                      nlocals   : 1
-                     stacksize : 7
+                     stacksize : 6
                      flags     : 19
                      code
                         0x950297008902a000000000000000000000000000000000000000000074
-                        0300000000000000000000890164017c0069018e01a6010000ab01000000
-                        000000000001007c005300
+                        03000000000000000000007c0067018901a20152008e00a6010000ab0100
+                        0000000000000001007c005300
                                    0 COPY_FREE_VARS           2
                      
                      155           2 RESUME                   0
                      
                      156           4 LOAD_DEREF               2 (self)
                                    6 LOAD_METHOD              0 (add_handler)
                                   28 LOAD_GLOBAL              3 (NULL + MessageStatusHandler)
-                                  40 LOAD_DEREF               1 (filters)
-                                  42 LOAD_CONST               1 ('handler')
-                                  44 LOAD_FAST                0 (func)
-                                  46 BUILD_MAP                1
-                                  48 CALL_FUNCTION_EX         1
-                                  50 PRECALL                  1
-                                  54 CALL                     1
-                                  64 POP_TOP
+                                  40 LOAD_FAST                0 (func)
+                                  42 BUILD_LIST               1
+                                  44 LOAD_DEREF               1 (filters)
+                                  46 LIST_EXTEND              1
+                                  48 LIST_TO_TUPLE
+                                  50 CALL_FUNCTION_EX         0
+                                  52 PRECALL                  1
+                                  56 CALL                     1
+                                  66 POP_TOP
                      
-                     157          66 LOAD_FAST                0 (func)
-                                  68 RETURN_VALUE
+                     157          68 LOAD_FAST                0 (func)
+                                  70 RETURN_VALUE
                      consts
                         None
-                        'handler'
                      names      ('add_handler', 'MessageStatusHandler')
                      varnames   ('func',)
                      freevars   ('filters', 'self')
                      cellvars   ()
                      filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                      name       'decorator'
                      firstlineno 155
-                     lnotab 0x04013e01
+                     lnotab 0x04014001
                names      ('Callable', 'MessageStatus', 'Any')
                varnames   ('self', 'filters', 'decorator')
                freevars   ()
                cellvars   ('self', 'filters')
                filename   '/home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py'
                name       'on_message_status_change'
                firstlineno 141
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/__pycache__/handlers.cpython-311.pyc

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd7809464 (Thu Jun 22 17:11:51 2023 UTC)
+moddate:  0xa68f9464 (Thu Jun 22 18:15:02 2023 UTC)
 files sz: 1431
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### ./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa/client.py

```diff
@@ -73,15 +73,15 @@
             ...     print(update)
 
         Args:
             filters: Filters to apply to the incoming updates (filters are function that take the WhatsApp client and
                 the incoming update and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", dict], Any]):
-            self.add_handler(RawUpdateHandler(handler=func, *filters))
+            self.add_handler(RawUpdateHandler(func, *filters))
             return func
         return decorator
 
     def on_message(self, *filters: Callable[["WhatsApp", Message], bool]):
         """
         Decorator to register a function as a handler for incoming messages.
 
@@ -92,15 +92,15 @@
             ...     msg.reply_text(text="Hello from PyWa!", quote=True, buttons=[InlineButton("Help", data="help")
 
         Args:
             filters: Filters to apply to the incoming messages (filters are function that take the WhatsApp client and
                 the incoming message and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", Message], Any]):
-            self.add_handler(MessageHandler(handler=func, *filters))
+            self.add_handler(MessageHandler(func, *filters))
             return func
         return decorator
 
     def on_callback_button(self, *filters: Callable[["WhatsApp", CallbackButton], bool]):
         """
         Decorator to register a function as a handler for incoming callback button presses.
 
@@ -111,15 +111,15 @@
             ...     btn.reply_text(text="What can I help you with?")
 
         Args:
             filters: Filters to apply to the incoming callback button presses (filters are function that take the
                 WhatsApp client and the incoming callback button and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", CallbackButton], Any]):
-            self.add_handler(ButtonCallbackHandler(handler=func, *filters))
+            self.add_handler(ButtonCallbackHandler(func, *filters))
             return func
         return decorator
 
     def on_callback_selection(self, *filters: Callable[["WhatsApp", CallbackSelection], bool]):
         """
         Decorator to register a function as a handler for incoming callback selections.
 
@@ -130,15 +130,15 @@
             ...     sel.reply_text(text=f"Your ID is {sel.data.split(':', 1)[1]}")
 
         Args:
             filters: Filters to apply to the incoming callback selections (filters are function that take the
                 WhatsApp client and the incoming callback selection and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", CallbackSelection], Any]):
-            self.add_handler(SelectionCallbackHandler(handler=func, *filters))
+            self.add_handler(SelectionCallbackHandler(func, *filters))
             return func
         return decorator
 
     def on_message_status_change(self, *filters: Callable[["WhatsApp", MessageStatus], bool]):
         """
         Decorator to register a function as a handler for incoming message status changes.
 
@@ -149,15 +149,15 @@
             ...     print(f"Message {status.id} was read by {status.from_user.wa_id}")
 
         Args:
             filters: Filters to apply to the incoming message status changes (filters are function that take the
                 WhatsApp client and the incoming message status change and return a boolean).
         """
         def decorator(func: Callable[["WhatsApp", MessageStatus], Any]):
-            self.add_handler(MessageStatusHandler(handler=func, *filters))
+            self.add_handler(MessageStatusHandler(func, *filters))
             return func
         return decorator
 
     def send_message(
             self,
             to: str,
             text: str,
```

### Comparing `./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc4-py3.11.egg-info/PKG-INFO` & `./home/david/Documents/private/python/pywa/venv/lib/python3.11/site-packages/pywa-0.0.1rc5-py3.11.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
@@ -23,14 +23,16 @@
 Provides-Extra: flask
 Provides-Extra: fastapi
 License-File: LICENSE
 
 # PyWa
 - Python wrapper for the WhatsApp Cloud API
 
+THIS IS A WORK IN PROGRESS. DO NOT USE IN PRODUCTION.
+
 ## Contents
 - [Installation](#installation)
 - [Usage](#usage)
 - [Getting started](#getting-started)
 - [Examples](#examples)
   - [Sending messages](#sending-messages)
   - [Handling incoming messages](#handling-incoming-messages)
```

