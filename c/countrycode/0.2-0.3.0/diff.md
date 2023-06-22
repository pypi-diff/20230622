# Comparing `tmp/countrycode-0.2.tar.gz` & `tmp/countrycode-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/countrycode-0.2.tar", last modified: Fri Jun 28 15:50:48 2013, max compression
+gzip compressed data, was "countrycode-0.3.0.tar", max compression
```

## Comparing `countrycode-0.2.tar` & `countrycode-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,7 @@
-drwxr-xr-x   0 hotsauce   (501) staff       (20)        0 2013-06-28 15:50:48.000000 countrycode-0.2/
-drwxr-xr-x   0 hotsauce   (501) staff       (20)        0 2013-06-28 15:50:48.000000 countrycode-0.2/countrycode/
--rw-r--r--   0 hotsauce   (501) staff       (20)       36 2013-06-28 15:41:26.000000 countrycode-0.2/countrycode/__init__.py
--rw-r--r--   0 hotsauce   (501) staff       (20)     2632 2013-06-28 15:44:58.000000 countrycode-0.2/countrycode/countrycode.py
-drwxr-xr-x   0 hotsauce   (501) staff       (20)        0 2013-06-28 15:50:48.000000 countrycode-0.2/countrycode/data/
--rw-r--r--   0 hotsauce   (501) staff       (20)    26904 2013-06-28 15:41:26.000000 countrycode-0.2/countrycode/data/countrycode_data.csv
--rw-r--r--   0 hotsauce   (501) staff       (20)      496 2013-06-28 15:41:26.000000 countrycode-0.2/countrycode/test_countrycode.py
--rw-r--r--   0 hotsauce   (501) staff       (20)     1500 2013-06-28 15:50:48.000000 countrycode-0.2/PKG-INFO
--rw-r--r--   0 hotsauce   (501) staff       (20)      915 2013-06-28 15:41:26.000000 countrycode-0.2/README.txt
--rw-r--r--   0 hotsauce   (501) staff       (20)      437 2013-06-28 15:46:42.000000 countrycode-0.2/setup.py
+-rw-r--r--   0        0        0    35149 2023-06-21 19:11:57.100561 countrycode-0.3.0/LICENSE
+-rw-r--r--   0        0        0    13446 2023-06-22 13:01:23.427021 countrycode-0.3.0/README.md
+-rw-r--r--   0        0        0       70 2023-06-22 12:45:49.387203 countrycode-0.3.0/countrycode/__init__.py
+-rwxr-xr-x   0        0        0     5080 2023-06-22 12:47:23.187181 countrycode-0.3.0/countrycode/countrycode.py
+-rwxr-xr-x   0        0        0  2263615 2023-06-21 19:31:27.460311 countrycode-0.3.0/countrycode/data/codelist.csv
+-rw-r--r--   0        0        0      386 2023-06-22 13:00:19.577034 countrycode-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13899 1970-01-01 00:00:00.000000 countrycode-0.3.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

