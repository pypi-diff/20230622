# Comparing `tmp/mycoinlib-1.0.tar.gz` & `tmp/mycoinlib-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycoinlib-1.0.tar", last modified: Tue Jun 20 01:55:09 2023, max compression
+gzip compressed data, was "mycoinlib-1.1.tar", last modified: Thu Jun 22 07:10:04 2023, max compression
```

## Comparing `mycoinlib-1.0.tar` & `mycoinlib-1.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 01:55:09.589681 mycoinlib-1.0/
--rw-rw-rw-   0        0        0       54 2023-06-20 01:55:09.535048 mycoinlib-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 01:55:09.407385 mycoinlib-1.0/mycoinlib/
--rw-rw-rw-   0        0        0       36 2023-06-19 20:15:24.000000 mycoinlib-1.0/mycoinlib/__init__.py
--rw-rw-rw-   0        0        0     5865 2023-06-20 01:49:19.000000 mycoinlib-1.0/mycoinlib/mycoinlib.py
-drwxrwxrwx   0        0        0        0 2023-06-20 01:55:09.523128 mycoinlib-1.0/mycoinlib.egg-info/
--rw-rw-rw-   0        0        0       54 2023-06-20 01:55:08.000000 mycoinlib-1.0/mycoinlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-20 01:55:09.000000 mycoinlib-1.0/mycoinlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 01:55:08.000000 mycoinlib-1.0/mycoinlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-20 01:55:08.000000 mycoinlib-1.0/mycoinlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 01:55:09.000000 mycoinlib-1.0/mycoinlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 01:55:09.595647 mycoinlib-1.0/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-06-20 01:54:26.000000 mycoinlib-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:10:04.037168 mycoinlib-1.1/
+-rw-rw-rw-   0        0        0       54 2023-06-22 07:10:04.030216 mycoinlib-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 07:10:03.769404 mycoinlib-1.1/mycoinlib/
+-rw-rw-rw-   0        0        0      130 2023-06-22 06:40:32.000000 mycoinlib-1.1/mycoinlib/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-06-22 06:55:17.000000 mycoinlib-1.1/mycoinlib/btc.py
+-rw-rw-rw-   0        0        0     1955 2023-06-22 07:03:16.000000 mycoinlib-1.1/mycoinlib/eth.py
+-rw-rw-rw-   0        0        0     2070 2023-06-22 06:54:59.000000 mycoinlib-1.1/mycoinlib/ltc.py
+-rw-rw-rw-   0        0        0      637 2023-06-22 06:44:33.000000 mycoinlib-1.1/mycoinlib/mycoin.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:10:04.018295 mycoinlib-1.1/mycoinlib.egg-info/
+-rw-rw-rw-   0        0        0       54 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:10:04.038162 mycoinlib-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-06-22 07:09:43.000000 mycoinlib-1.1/setup.py
```

