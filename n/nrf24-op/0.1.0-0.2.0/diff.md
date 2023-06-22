# Comparing `tmp/nrf24_op-0.1.0.tar.gz` & `tmp/nrf24_op-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrf24_op-0.1.0.tar", last modified: Wed Jun 21 11:10:21 2023, max compression
+gzip compressed data, was "nrf24_op-0.2.0.tar", last modified: Thu Jun 22 12:11:55 2023, max compression
```

## Comparing `nrf24_op-0.1.0.tar` & `nrf24_op-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 nofal     (1000) nofal     (1000)        0 2023-06-21 11:10:21.021119 nrf24_op-0.1.0/
--rw-rw-r--   0 nofal     (1000) nofal     (1000)     1065 2023-06-21 10:24:36.000000 nrf24_op-0.1.0/LICENSE
--rw-rw-r--   0 nofal     (1000) nofal     (1000)      221 2023-06-21 11:10:21.021119 nrf24_op-0.1.0/PKG-INFO
--rw-rw-r--   0 nofal     (1000) nofal     (1000)       24 2023-06-21 10:36:34.000000 nrf24_op-0.1.0/README.md
-drwxrwxr-x   0 nofal     (1000) nofal     (1000)        0 2023-06-21 11:10:21.021119 nrf24_op-0.1.0/nrf24_op.egg-info/
--rw-rw-r--   0 nofal     (1000) nofal     (1000)      221 2023-06-21 11:10:21.000000 nrf24_op-0.1.0/nrf24_op.egg-info/PKG-INFO
--rw-rw-r--   0 nofal     (1000) nofal     (1000)      185 2023-06-21 11:10:21.000000 nrf24_op-0.1.0/nrf24_op.egg-info/SOURCES.txt
--rw-rw-r--   0 nofal     (1000) nofal     (1000)        1 2023-06-21 11:10:21.000000 nrf24_op-0.1.0/nrf24_op.egg-info/dependency_links.txt
--rw-rw-r--   0 nofal     (1000) nofal     (1000)       16 2023-06-21 11:10:21.000000 nrf24_op-0.1.0/nrf24_op.egg-info/requires.txt
--rw-rw-r--   0 nofal     (1000) nofal     (1000)        1 2023-06-21 11:10:21.000000 nrf24_op-0.1.0/nrf24_op.egg-info/top_level.txt
--rw-rw-r--   0 nofal     (1000) nofal     (1000)       38 2023-06-21 11:10:21.021119 nrf24_op-0.1.0/setup.cfg
--rw-rw-r--   0 nofal     (1000) nofal     (1000)      312 2023-06-21 11:10:13.000000 nrf24_op-0.1.0/setup.py
+drwxrwxr-x   0 nofal     (1000) nofal     (1000)        0 2023-06-22 12:11:55.902448 nrf24_op-0.2.0/
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)     1065 2023-06-21 10:24:36.000000 nrf24_op-0.2.0/LICENSE
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)      221 2023-06-22 12:11:55.902448 nrf24_op-0.2.0/PKG-INFO
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)       24 2023-06-21 10:36:34.000000 nrf24_op-0.2.0/README.md
+drwxrwxr-x   0 nofal     (1000) nofal     (1000)        0 2023-06-22 12:11:55.902448 nrf24_op-0.2.0/nrf24_op/
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)        0 2023-06-21 10:24:36.000000 nrf24_op-0.2.0/nrf24_op/__init__.py
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)    12824 2023-06-22 11:55:33.000000 nrf24_op-0.2.0/nrf24_op/nrf24_op.py
+drwxrwxr-x   0 nofal     (1000) nofal     (1000)        0 2023-06-22 12:11:55.902448 nrf24_op-0.2.0/nrf24_op.egg-info/
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)      221 2023-06-22 12:11:55.000000 nrf24_op-0.2.0/nrf24_op.egg-info/PKG-INFO
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)      227 2023-06-22 12:11:55.000000 nrf24_op-0.2.0/nrf24_op.egg-info/SOURCES.txt
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)        1 2023-06-22 12:11:55.000000 nrf24_op-0.2.0/nrf24_op.egg-info/dependency_links.txt
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)       16 2023-06-22 12:11:55.000000 nrf24_op-0.2.0/nrf24_op.egg-info/requires.txt
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)        9 2023-06-22 12:11:55.000000 nrf24_op-0.2.0/nrf24_op.egg-info/top_level.txt
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)       38 2023-06-22 12:11:55.902448 nrf24_op-0.2.0/setup.cfg
+-rw-rw-r--   0 nofal     (1000) nofal     (1000)      312 2023-06-22 12:11:34.000000 nrf24_op-0.2.0/setup.py
```

### Comparing `nrf24_op-0.1.0/LICENSE` & `nrf24_op-0.2.0/LICENSE`

 * *Files identical despite different names*

