# Comparing `tmp/optigatrust-1.3.7.tar.gz` & `tmp/optigatrust-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optigatrust-1.3.7.tar", last modified: Fri Nov 25 13:41:59 2022, max compression
+gzip compressed data, was "optigatrust-1.3.8.tar", last modified: Thu Jun 22 09:30:35 2023, max compression
```

## Comparing `optigatrust-1.3.7.tar` & `optigatrust-1.3.8.tar`

### file list

```diff
@@ -1,51 +1,69 @@
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:59.066796 optigatrust-1.3.7/
--rw-rw-rw-   0        0        0     1103 2021-07-14 11:22:47.000000 optigatrust-1.3.7/LICENSE
--rw-rw-rw-   0        0        0      149 2021-08-16 08:53:48.000000 optigatrust-1.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2895 2022-11-25 13:41:59.065505 optigatrust-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     1816 2021-07-14 11:22:47.000000 optigatrust-1.3.7/README.md
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:58.986505 optigatrust-1.3.7/optigatrust/
--rw-rw-rw-   0        0        0    40782 2022-11-25 13:27:01.000000 optigatrust-1.3.7/optigatrust/__init__.py
--rw-rw-rw-   0        0        0      156 2021-08-20 12:22:46.000000 optigatrust-1.3.7/optigatrust/__main__.py
--rw-rw-rw-   0        0        0    12559 2022-11-25 13:27:01.000000 optigatrust-1.3.7/optigatrust/_backend.py
--rw-rw-rw-   0        0        0    34913 2022-11-25 13:29:51.000000 optigatrust-1.3.7/optigatrust/clidriver.py
--rw-rw-rw-   0        0        0    42601 2022-11-25 13:29:51.000000 optigatrust-1.3.7/optigatrust/crypto.py
--rw-rw-rw-   0        0        0    17154 2021-08-20 12:22:46.000000 optigatrust-1.3.7/optigatrust/csr.py
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:58.930504 optigatrust-1.3.7/optigatrust/csrc/
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:59.041508 optigatrust-1.3.7/optigatrust/csrc/lib/
--rw-rw-rw-   0        0        0   125696 2021-11-21 07:47:37.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-i2c-linux-armv7l.so
--rw-rw-rw-   0        0        0   102072 2021-11-18 13:34:31.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-i2c-linux-x86_64.so
--rw-rw-rw-   0        0        0   125112 2021-11-21 07:47:37.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-libusb-linux-armv7l.so
--rw-rw-rw-   0        0        0   101592 2021-11-18 13:34:31.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-libusb-linux-x86_64.so
--rw-rw-rw-   0        0        0   238080 2021-11-18 13:34:31.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-libusb-win-amd64.dll
--rw-rw-rw-   0        0        0   161792 2021-11-18 13:34:31.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-libusb-win-i686.dll
--rw-rw-rw-   0        0        0   123884 2021-11-19 22:16:00.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-uart-linux-armv7l.so
--rw-rw-rw-   0        0        0   124752 2021-11-21 07:47:37.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-uart-linux-x86_64.so
--rw-rw-rw-   0        0        0   131072 2021-12-07 10:54:09.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-uart-win-amd64.dll
--rw-rw-rw-   0        0        0    60416 2021-11-21 07:47:37.000000 optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-uart-win-i686.dll
--rw-rw-rw-   0        0        0        5 2022-11-25 13:27:01.000000 optigatrust-1.3.7/optigatrust/csrc/lib/optiga_comms.ini
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:58.932508 optigatrust-1.3.7/optigatrust/csrc/optiga-trust-m/
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:58.932508 optigatrust-1.3.7/optigatrust/csrc/optiga-trust-m/pal/
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:58.933506 optigatrust-1.3.7/optigatrust/csrc/optiga-trust-m/pal/libusb/
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:59.044558 optigatrust-1.3.7/optigatrust/csrc/optiga-trust-m/pal/libusb/include/
--rw-rw-rw-   0        0        0      123 2021-07-14 11:22:50.000000 optigatrust-1.3.7/optigatrust/csrc/optiga-trust-m/pal/libusb/include/90-optigatrust.rules
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:59.062506 optigatrust-1.3.7/optigatrust/enums/
--rw-rw-rw-   0        0        0      191 2021-08-20 12:22:46.000000 optigatrust-1.3.7/optigatrust/enums/__init__.py
--rw-rw-rw-   0        0        0     2236 2021-08-20 12:22:46.000000 optigatrust-1.3.7/optigatrust/enums/charge.py
--rw-rw-rw-   0        0        0     2274 2021-07-14 11:22:51.000000 optigatrust-1.3.7/optigatrust/enums/conf_template.xml
--rw-rw-rw-   0        0        0     2290 2021-08-20 12:22:46.000000 optigatrust-1.3.7/optigatrust/enums/m1.py
--rw-rw-rw-   0        0        0     2266 2021-08-20 12:22:46.000000 optigatrust-1.3.7/optigatrust/enums/m2id2.py
--rw-rw-rw-   0        0        0     2547 2022-11-25 13:29:51.000000 optigatrust-1.3.7/optigatrust/enums/m3.py
--rw-rw-rw-   0        0        0     2185 2021-08-20 12:22:46.000000 optigatrust-1.3.7/optigatrust/enums/x.py
--rw-rw-rw-   0        0        0    11178 2021-08-20 12:22:46.000000 optigatrust-1.3.7/optigatrust/objects.py
--rw-rw-rw-   0        0        0    10597 2021-08-20 12:22:46.000000 optigatrust-1.3.7/optigatrust/port.py
--rw-rw-rw-   0        0        0      140 2022-11-25 13:37:47.000000 optigatrust-1.3.7/optigatrust/version.py
-drwxrwxrwx   0        0        0        0 2022-11-25 13:41:59.007507 optigatrust-1.3.7/optigatrust.egg-info/
--rw-rw-rw-   0        0        0     2895 2022-11-25 13:41:58.000000 optigatrust-1.3.7/optigatrust.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1337 2022-11-25 13:41:58.000000 optigatrust-1.3.7/optigatrust.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-25 13:41:58.000000 optigatrust-1.3.7/optigatrust.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2022-11-25 13:41:58.000000 optigatrust-1.3.7/optigatrust.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2022-11-25 13:41:58.000000 optigatrust-1.3.7/optigatrust.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-11-25 13:41:58.000000 optigatrust-1.3.7/optigatrust.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-07-14 11:22:51.000000 optigatrust-1.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-25 13:41:59.066796 optigatrust-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0     4211 2021-08-16 08:46:34.000000 optigatrust-1.3.7/setup.py
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.632081 optigatrust-1.3.8/
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     1103 2023-06-22 08:49:21.000000 optigatrust-1.3.8/LICENSE
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)      149 2023-06-22 08:49:21.000000 optigatrust-1.3.8/MANIFEST.in
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2818 2023-06-22 09:30:35.628081 optigatrust-1.3.8/PKG-INFO
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     1816 2023-06-22 08:49:21.000000 optigatrust-1.3.8/README.md
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.404082 optigatrust-1.3.8/optigatrust/
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)    40782 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/__init__.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)      156 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/__main__.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)    12559 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/_backend.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)    34913 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/clidriver.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)    42601 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/crypto.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)    17154 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csr.py
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.348083 optigatrust-1.3.8/optigatrust/csrc/
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.552082 optigatrust-1.3.8/optigatrust/csrc/lib/
+-rwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)   132632 2023-06-22 09:09:36.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-i2c-linux-aarch64.so
+-rwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)   125696 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-i2c-linux-armv7l.so
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)   102072 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-i2c-linux-x86_64.so
+-rwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)   131984 2023-06-22 09:09:26.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-libusb-linux-aarch64.so
+-rwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)   125112 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-libusb-linux-armv7l.so
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)   101592 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-libusb-linux-x86_64.so
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)   238080 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-libusb-win-amd64.dll
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)   161792 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-libusb-win-i686.dll
+-rwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)   126944 2023-06-22 09:01:49.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-uart-linux-aarch64.so
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)   123884 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-uart-linux-armv7l.so
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)   124752 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-uart-linux-x86_64.so
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)   131072 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-uart-win-amd64.dll
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)    60416 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-uart-win-i686.dll
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)        5 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/lib/optiga_comms.ini
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.352083 optigatrust-1.3.8/optigatrust/csrc/optiga-trust-m/
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.352083 optigatrust-1.3.8/optigatrust/csrc/optiga-trust-m/pal/
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.352083 optigatrust-1.3.8/optigatrust/csrc/optiga-trust-m/pal/libusb/
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.556082 optigatrust-1.3.8/optigatrust/csrc/optiga-trust-m/pal/libusb/include/
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)      123 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/csrc/optiga-trust-m/pal/libusb/include/90-optigatrust.rules
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.580082 optigatrust-1.3.8/optigatrust/enums/
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)      191 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/enums/__init__.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2236 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/enums/charge.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2274 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/enums/conf_template.xml
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2290 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/enums/m1.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2266 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/enums/m2id2.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2547 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/enums/m3.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2185 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/enums/x.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)    11178 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/objects.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)    10597 2023-06-22 08:49:22.000000 optigatrust-1.3.8/optigatrust/port.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)      140 2023-06-22 09:27:59.000000 optigatrust-1.3.8/optigatrust/version.py
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.420082 optigatrust-1.3.8/optigatrust.egg-info/
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2818 2023-06-22 09:30:35.000000 optigatrust-1.3.8/optigatrust.egg-info/PKG-INFO
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     1792 2023-06-22 09:30:35.000000 optigatrust-1.3.8/optigatrust.egg-info/SOURCES.txt
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)        1 2023-06-22 09:30:35.000000 optigatrust-1.3.8/optigatrust.egg-info/dependency_links.txt
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)       59 2023-06-22 09:30:35.000000 optigatrust-1.3.8/optigatrust.egg-info/entry_points.txt
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)       58 2023-06-22 09:30:35.000000 optigatrust-1.3.8/optigatrust.egg-info/requires.txt
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)       12 2023-06-22 09:30:35.000000 optigatrust-1.3.8/optigatrust.egg-info/top_level.txt
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)      108 2023-06-22 08:49:22.000000 optigatrust-1.3.8/pyproject.toml
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)       38 2023-06-22 09:30:35.632081 optigatrust-1.3.8/setup.cfg
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     4211 2023-06-22 08:49:22.000000 optigatrust-1.3.8/setup.py
+drwxr-xr-x   0 koblbauer  (1000) koblbauer  (1000)        0 2023-06-22 09:30:35.624081 optigatrust-1.3.8/tests/
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2348 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_cert.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)      703 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_chip_control.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     1036 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_csr.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     5791 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_ecc.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     2799 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_ecdh.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     4588 2023-06-22 08:49:33.000000 optigatrust-1.3.8/tests/test_ecdsa.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     1217 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_hmac.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     3955 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_kdf.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     5611 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_meta.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     1527 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_pbkdf2.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)      828 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_port.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)      612 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_rand.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)     1264 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_rsa.py
+-rw-r--r--   0 koblbauer  (1000) koblbauer  (1000)    12646 2023-06-22 08:49:22.000000 optigatrust-1.3.8/tests/test_rsapkcs1v15.py
```

### Comparing `optigatrust-1.3.7/LICENSE` & `optigatrust-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/PKG-INFO` & `optigatrust-1.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-Metadata-Version: 2.1
-Name: optigatrust
-Version: 1.3.7
-Summary: The ctypes Python wrapper for the Infineon OPTIGA(TM) Trust family of security solutions
-Home-page: https://github.com/infineon/python-optiga-trust
-Author: Infineon Technologies AG
-Author-email: DSSTechnicalSupport@infineon.com
-License: MIT
-Keywords: ECDHE ECDSA RSA ECC X509 NISTP256 NIST384 OPTIGA TRUST TRUSTX TRUSTM
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Microsoft :: Windows :: Windows 8
-Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# optigatrust Python library
-
-A ctypes based Python wrapper to work with the OPTIGA™ Trust security solutions.
-
-[![PyPI](https://img.shields.io/pypi/v/optigatrust.svg)](https://pypi.org/project/optigatrust/)
-
-## Features
-
-*optigatrust* is a library which helps to manage the OPTIGA Trust family of security solutions
-Find more about these products here:
-* [OPTIGA™ Trust M](https://github.com/Infineon/optiga-trust-m)
-* [OPTIGA™ Trust Charge](https://github.com/Infineon/optiga-trust-charge)
-* [OPTIGA™ Trust X](https://github.com/Infineon/optiga-trust-x)
-
-[**Documentation**](https://infineon.github.io/python-optiga-trust)
- 
-## Required Hardware
-
-* Any of the following
-    - OPTIGA™ Trust [M](https://www.infineon.com/cms/en/product/evaluation-boards/optiga-trust-m-eval-kit/)/[Charge](https://www.infineon.com/cms/en/product/evaluation-boards/optiga-trust-ch-eval-kit/) Evaluation Kit
-    - OPTIGA™ Trust Personalisation Board (SP005405452), or any FTDI USB-HID/I2C Converter board
-    - Raspberry Pi + [Shield2Go RPi Adapter](https://www.infineon.com/cms/en/product/evaluation-boards/s2go-adapter-rasp-pi-iot/)
-* OPTIGA™ Trust X/M/Charge sample or a Security Shield2Go
-
-## Installation
-
-```bash
-$ pip install optigatrust
-```
-
-### Examples
-
-```python
-import optigatrust as optiga
-from optigatrust import objects, crypto
-import json
-
-chip = optiga.Chip()
-chip.current_limit = 15
-
-ecc_key_0 = objects.ECCKey(0xe0f0) 
-
-print('Pretty metadata: {0}'.format(json.dumps(ecc_key_0.meta, indent=4)))
-
-public_key, private_key = crypto.generate_pair(ecc_key_0, curve='secp256r1', export=True)
-
-print('Pulic Key = {0}, Privat key = {1}'.format(public_key, private_key))
-
-```
-
-## License
-
-*optigatrust* is licensed under the terms of the MIT license. See the
-[LICENSE](LICENSE) file for the exact license text.
+Metadata-Version: 2.1
+Name: optigatrust
+Version: 1.3.8
+Summary: The ctypes Python wrapper for the Infineon OPTIGA(TM) Trust family of security solutions
+Home-page: https://github.com/infineon/python-optiga-trust
+Author: Infineon Technologies AG
+Author-email: DSSTechnicalSupport@infineon.com
+License: MIT
+Keywords: ECDHE ECDSA RSA ECC X509 NISTP256 NIST384 OPTIGA TRUST TRUSTX TRUSTM
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# optigatrust Python library
+
+A ctypes based Python wrapper to work with the OPTIGA™ Trust security solutions.
+
+[![PyPI](https://img.shields.io/pypi/v/optigatrust.svg)](https://pypi.org/project/optigatrust/)
+
+## Features
+
+*optigatrust* is a library which helps to manage the OPTIGA Trust family of security solutions
+Find more about these products here:
+* [OPTIGA™ Trust M](https://github.com/Infineon/optiga-trust-m)
+* [OPTIGA™ Trust Charge](https://github.com/Infineon/optiga-trust-charge)
+* [OPTIGA™ Trust X](https://github.com/Infineon/optiga-trust-x)
+
+[**Documentation**](https://infineon.github.io/python-optiga-trust)
+ 
+## Required Hardware
+
+* Any of the following
+    - OPTIGA™ Trust [M](https://www.infineon.com/cms/en/product/evaluation-boards/optiga-trust-m-eval-kit/)/[Charge](https://www.infineon.com/cms/en/product/evaluation-boards/optiga-trust-ch-eval-kit/) Evaluation Kit
+    - OPTIGA™ Trust Personalisation Board (SP005405452), or any FTDI USB-HID/I2C Converter board
+    - Raspberry Pi + [Shield2Go RPi Adapter](https://www.infineon.com/cms/en/product/evaluation-boards/s2go-adapter-rasp-pi-iot/)
+* OPTIGA™ Trust X/M/Charge sample or a Security Shield2Go
+
+## Installation
+
+```bash
+$ pip install optigatrust
+```
+
+### Examples
+
+```python
+import optigatrust as optiga
+from optigatrust import objects, crypto
+import json
+
+chip = optiga.Chip()
+chip.current_limit = 15
+
+ecc_key_0 = objects.ECCKey(0xe0f0) 
+
+print('Pretty metadata: {0}'.format(json.dumps(ecc_key_0.meta, indent=4)))
+
+public_key, private_key = crypto.generate_pair(ecc_key_0, curve='secp256r1', export=True)
+
+print('Pulic Key = {0}, Privat key = {1}'.format(public_key, private_key))
+
+```
+
+## License
+
+*optigatrust* is licensed under the terms of the MIT license. See the
+[LICENSE](LICENSE) file for the exact license text.
```

### Comparing `optigatrust-1.3.7/README.md` & `optigatrust-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/__init__.py` & `optigatrust-1.3.8/optigatrust/__init__.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/_backend.py` & `optigatrust-1.3.8/optigatrust/_backend.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/clidriver.py` & `optigatrust-1.3.8/optigatrust/clidriver.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/crypto.py` & `optigatrust-1.3.8/optigatrust/crypto.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csr.py` & `optigatrust-1.3.8/optigatrust/csr.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-i2c-linux-armv7l.so` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-i2c-linux-armv7l.so`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-i2c-linux-x86_64.so` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-i2c-linux-x86_64.so`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-libusb-linux-armv7l.so` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-libusb-linux-armv7l.so`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-libusb-linux-x86_64.so` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-libusb-linux-x86_64.so`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-libusb-win-amd64.dll` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-libusb-win-amd64.dll`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-libusb-win-i686.dll` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-libusb-win-i686.dll`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-uart-linux-armv7l.so` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-uart-linux-armv7l.so`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-uart-linux-x86_64.so` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-uart-linux-x86_64.so`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-uart-win-amd64.dll` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-uart-win-amd64.dll`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/csrc/lib/liboptigatrust-uart-win-i686.dll` & `optigatrust-1.3.8/optigatrust/csrc/lib/liboptigatrust-uart-win-i686.dll`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/enums/charge.py` & `optigatrust-1.3.8/optigatrust/enums/charge.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/enums/conf_template.xml` & `optigatrust-1.3.8/optigatrust/enums/conf_template.xml`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/enums/m1.py` & `optigatrust-1.3.8/optigatrust/enums/m1.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/enums/m2id2.py` & `optigatrust-1.3.8/optigatrust/enums/m2id2.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/enums/m3.py` & `optigatrust-1.3.8/optigatrust/enums/m3.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/enums/x.py` & `optigatrust-1.3.8/optigatrust/enums/x.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/objects.py` & `optigatrust-1.3.8/optigatrust/objects.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust/port.py` & `optigatrust-1.3.8/optigatrust/port.py`

 * *Files identical despite different names*

### Comparing `optigatrust-1.3.7/optigatrust.egg-info/PKG-INFO` & `optigatrust-1.3.8/optigatrust.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-Metadata-Version: 2.1
-Name: optigatrust
-Version: 1.3.7
-Summary: The ctypes Python wrapper for the Infineon OPTIGA(TM) Trust family of security solutions
-Home-page: https://github.com/infineon/python-optiga-trust
-Author: Infineon Technologies AG
-Author-email: DSSTechnicalSupport@infineon.com
-License: MIT
-Keywords: ECDHE ECDSA RSA ECC X509 NISTP256 NIST384 OPTIGA TRUST TRUSTX TRUSTM
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Microsoft :: Windows :: Windows 8
-Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# optigatrust Python library
-
-A ctypes based Python wrapper to work with the OPTIGA™ Trust security solutions.
-
-[![PyPI](https://img.shields.io/pypi/v/optigatrust.svg)](https://pypi.org/project/optigatrust/)
-
-## Features
-
-*optigatrust* is a library which helps to manage the OPTIGA Trust family of security solutions
-Find more about these products here:
-* [OPTIGA™ Trust M](https://github.com/Infineon/optiga-trust-m)
-* [OPTIGA™ Trust Charge](https://github.com/Infineon/optiga-trust-charge)
-* [OPTIGA™ Trust X](https://github.com/Infineon/optiga-trust-x)
-
-[**Documentation**](https://infineon.github.io/python-optiga-trust)
- 
-## Required Hardware
-
-* Any of the following
-    - OPTIGA™ Trust [M](https://www.infineon.com/cms/en/product/evaluation-boards/optiga-trust-m-eval-kit/)/[Charge](https://www.infineon.com/cms/en/product/evaluation-boards/optiga-trust-ch-eval-kit/) Evaluation Kit
-    - OPTIGA™ Trust Personalisation Board (SP005405452), or any FTDI USB-HID/I2C Converter board
-    - Raspberry Pi + [Shield2Go RPi Adapter](https://www.infineon.com/cms/en/product/evaluation-boards/s2go-adapter-rasp-pi-iot/)
-* OPTIGA™ Trust X/M/Charge sample or a Security Shield2Go
-
-## Installation
-
-```bash
-$ pip install optigatrust
-```
-
-### Examples
-
-```python
-import optigatrust as optiga
-from optigatrust import objects, crypto
-import json
-
-chip = optiga.Chip()
-chip.current_limit = 15
-
-ecc_key_0 = objects.ECCKey(0xe0f0) 
-
-print('Pretty metadata: {0}'.format(json.dumps(ecc_key_0.meta, indent=4)))
-
-public_key, private_key = crypto.generate_pair(ecc_key_0, curve='secp256r1', export=True)
-
-print('Pulic Key = {0}, Privat key = {1}'.format(public_key, private_key))
-
-```
-
-## License
-
-*optigatrust* is licensed under the terms of the MIT license. See the
-[LICENSE](LICENSE) file for the exact license text.
+Metadata-Version: 2.1
+Name: optigatrust
+Version: 1.3.8
+Summary: The ctypes Python wrapper for the Infineon OPTIGA(TM) Trust family of security solutions
+Home-page: https://github.com/infineon/python-optiga-trust
+Author: Infineon Technologies AG
+Author-email: DSSTechnicalSupport@infineon.com
+License: MIT
+Keywords: ECDHE ECDSA RSA ECC X509 NISTP256 NIST384 OPTIGA TRUST TRUSTX TRUSTM
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# optigatrust Python library
+
+A ctypes based Python wrapper to work with the OPTIGA™ Trust security solutions.
+
+[![PyPI](https://img.shields.io/pypi/v/optigatrust.svg)](https://pypi.org/project/optigatrust/)
+
+## Features
+
+*optigatrust* is a library which helps to manage the OPTIGA Trust family of security solutions
+Find more about these products here:
+* [OPTIGA™ Trust M](https://github.com/Infineon/optiga-trust-m)
+* [OPTIGA™ Trust Charge](https://github.com/Infineon/optiga-trust-charge)
+* [OPTIGA™ Trust X](https://github.com/Infineon/optiga-trust-x)
+
+[**Documentation**](https://infineon.github.io/python-optiga-trust)
+ 
+## Required Hardware
+
+* Any of the following
+    - OPTIGA™ Trust [M](https://www.infineon.com/cms/en/product/evaluation-boards/optiga-trust-m-eval-kit/)/[Charge](https://www.infineon.com/cms/en/product/evaluation-boards/optiga-trust-ch-eval-kit/) Evaluation Kit
+    - OPTIGA™ Trust Personalisation Board (SP005405452), or any FTDI USB-HID/I2C Converter board
+    - Raspberry Pi + [Shield2Go RPi Adapter](https://www.infineon.com/cms/en/product/evaluation-boards/s2go-adapter-rasp-pi-iot/)
+* OPTIGA™ Trust X/M/Charge sample or a Security Shield2Go
+
+## Installation
+
+```bash
+$ pip install optigatrust
+```
+
+### Examples
+
+```python
+import optigatrust as optiga
+from optigatrust import objects, crypto
+import json
+
+chip = optiga.Chip()
+chip.current_limit = 15
+
+ecc_key_0 = objects.ECCKey(0xe0f0) 
+
+print('Pretty metadata: {0}'.format(json.dumps(ecc_key_0.meta, indent=4)))
+
+public_key, private_key = crypto.generate_pair(ecc_key_0, curve='secp256r1', export=True)
+
+print('Pulic Key = {0}, Privat key = {1}'.format(public_key, private_key))
+
+```
+
+## License
+
+*optigatrust* is licensed under the terms of the MIT license. See the
+[LICENSE](LICENSE) file for the exact license text.
```

### Comparing `optigatrust-1.3.7/optigatrust.egg-info/SOURCES.txt` & `optigatrust-1.3.8/optigatrust.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -14,26 +14,43 @@
 optigatrust/version.py
 optigatrust.egg-info/PKG-INFO
 optigatrust.egg-info/SOURCES.txt
 optigatrust.egg-info/dependency_links.txt
 optigatrust.egg-info/entry_points.txt
 optigatrust.egg-info/requires.txt
 optigatrust.egg-info/top_level.txt
+optigatrust/csrc/lib/liboptigatrust-i2c-linux-aarch64.so
 optigatrust/csrc/lib/liboptigatrust-i2c-linux-armv7l.so
 optigatrust/csrc/lib/liboptigatrust-i2c-linux-x86_64.so
+optigatrust/csrc/lib/liboptigatrust-libusb-linux-aarch64.so
 optigatrust/csrc/lib/liboptigatrust-libusb-linux-armv7l.so
 optigatrust/csrc/lib/liboptigatrust-libusb-linux-x86_64.so
 optigatrust/csrc/lib/liboptigatrust-libusb-win-amd64.dll
 optigatrust/csrc/lib/liboptigatrust-libusb-win-i686.dll
+optigatrust/csrc/lib/liboptigatrust-uart-linux-aarch64.so
 optigatrust/csrc/lib/liboptigatrust-uart-linux-armv7l.so
 optigatrust/csrc/lib/liboptigatrust-uart-linux-x86_64.so
 optigatrust/csrc/lib/liboptigatrust-uart-win-amd64.dll
 optigatrust/csrc/lib/liboptigatrust-uart-win-i686.dll
 optigatrust/csrc/lib/optiga_comms.ini
 optigatrust/csrc/optiga-trust-m/pal/libusb/include/90-optigatrust.rules
 optigatrust/enums/__init__.py
 optigatrust/enums/charge.py
 optigatrust/enums/conf_template.xml
 optigatrust/enums/m1.py
 optigatrust/enums/m2id2.py
 optigatrust/enums/m3.py
-optigatrust/enums/x.py
+optigatrust/enums/x.py
+tests/test_cert.py
+tests/test_chip_control.py
+tests/test_csr.py
+tests/test_ecc.py
+tests/test_ecdh.py
+tests/test_ecdsa.py
+tests/test_hmac.py
+tests/test_kdf.py
+tests/test_meta.py
+tests/test_pbkdf2.py
+tests/test_port.py
+tests/test_rand.py
+tests/test_rsa.py
+tests/test_rsapkcs1v15.py
```

### Comparing `optigatrust-1.3.7/setup.py` & `optigatrust-1.3.8/setup.py`

 * *Files identical despite different names*

