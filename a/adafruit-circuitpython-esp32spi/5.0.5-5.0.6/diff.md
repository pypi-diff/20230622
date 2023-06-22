# Comparing `tmp/adafruit-circuitpython-esp32spi-5.0.5.tar.gz` & `tmp/adafruit-circuitpython-esp32spi-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-esp32spi-5.0.5.tar", last modified: Thu Sep 15 18:08:30 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-esp32spi-5.0.6.tar", last modified: Thu Jun 22 17:43:49 2023, max compression
```

## Comparing `adafruit-circuitpython-esp32spi-5.0.5.tar` & `adafruit-circuitpython-esp32spi-5.0.6.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.415994 adafruit-circuitpython-esp32spi-5.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.407994 adafruit-circuitpython-esp32spi-5.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.411994 adafruit-circuitpython-esp32spi-5.0.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.411994 adafruit-circuitpython-esp32spi-5.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.411994 adafruit-circuitpython-esp32spi-5.0.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3615 2022-09-15 18:08:30.415994 adafruit-circuitpython-esp32spi-5.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.411994 adafruit-circuitpython-esp32spi-5.0.5/adafruit_circuitpython_esp32spi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3615 2022-09-15 18:08:30.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-09-15 18:08:30.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 18:08:30.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-15 18:08:30.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_circuitpython_esp32spi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-15 18:08:30.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.411994 adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3180 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/PWMOut.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38702 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/adafruit_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (121)     8848 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/adafruit_esp32spi_socket.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13094 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
--rw-r--r--   0 runner    (1001) docker     (121)     8634 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/adafruit_esp32spi_wsgiserver.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6292 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/digitalio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.415994 adafruit-circuitpython-esp32spi-5.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.415994 adafruit-circuitpython-esp32spi-5.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5758 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.415994 adafruit-circuitpython-esp32spi-5.0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2320 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_ipconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_localtime.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_simpletest_rp2040.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_tcp_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_udp_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_wpa2ent_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_wpa2ent_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.415994 adafruit-circuitpython-esp32spi-5.0.5/examples/gpio/
--rw-r--r--   0 runner    (1001) docker     (121)     5220 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/gpio/esp32spi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/gpio/gpio.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.415994 adafruit-circuitpython-esp32spi-5.0.5/examples/server/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8400 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/server/esp32spi_wsgiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 18:08:30.415994 adafruit-circuitpython-esp32spi-5.0.5/examples/server/static/
--rwxr-xr-x   0 runner    (1001) docker     (121)      356 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/server/static/index.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     3862 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/examples/server/static/led_color_picker_example.js
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-09-15 18:08:19.000000 adafruit-circuitpython-esp32spi-5.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-15 18:08:11.000000 adafruit-circuitpython-esp32spi-5.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 18:08:30.415994 adafruit-circuitpython-esp32spi-5.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.102824 adafruit-circuitpython-esp32spi-5.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.106824 adafruit-circuitpython-esp32spi-5.0.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.106824 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.106824 adafruit-circuitpython-esp32spi-5.0.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.106824 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 17:43:49.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.110825 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/PWMOut.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38983 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_socket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13094 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_wsgiserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6293 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/digitalio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.114825 adafruit-circuitpython-esp32spi-5.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.114825 adafruit-circuitpython-esp32spi-5.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.114825 adafruit-circuitpython-esp32spi-5.0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_ipconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_simpletest_rp2040.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_tcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_wpa2ent_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_wpa2ent_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/esp32spi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/gpio.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/examples/server/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8400 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/server/esp32spi_wsgiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/examples/server/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/server/static/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3862 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/examples/server/static/led_color_picker_example.js
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-22 17:43:39.000000 adafruit-circuitpython-esp32spi-5.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-22 17:43:27.000000 adafruit-circuitpython-esp32spi-5.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 17:43:49.118826 adafruit-circuitpython-esp32spi-5.0.6/setup.cfg
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-esp32spi-5.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/.gitignore` & `adafruit-circuitpython-esp32spi-5.0.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/.pre-commit-config.yaml` & `adafruit-circuitpython-esp32spi-5.0.6/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/.pylintrc` & `adafruit-circuitpython-esp32spi-5.0.6/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2019 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-esp32spi-5.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/LICENSE` & `adafruit-circuitpython-esp32spi-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-esp32spi-5.0.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/LICENSES/MIT.txt` & `adafruit-circuitpython-esp32spi-5.0.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/LICENSES/Unlicense.txt` & `adafruit-circuitpython-esp32spi-5.0.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/PKG-INFO` & `adafruit-circuitpython-esp32spi-5.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 5.0.5
+Version: 5.0.6
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/README.rst` & `adafruit-circuitpython-esp32spi-5.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO` & `adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 5.0.5
+Version: 5.0.6
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt` & `adafruit-circuitpython-esp32spi-5.0.6/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 README.rst.license
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
 adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
 adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
 adafruit_circuitpython_esp32spi.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/PWMOut.py` & `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/PWMOut.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/adafruit_esp32spi.py` & `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import struct
 import time
 from micropython import const
 from adafruit_bus_device.spi_device import SPIDevice
 from digitalio import Direction
 
-__version__ = "5.0.5"
+__version__ = "5.0.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI.git"
 
 _SET_NET_CMD = const(0x10)
 _SET_PASSPHRASE_CMD = const(0x11)
 _SET_IP_CONFIG = const(0x14)
 _SET_DNS_CONFIG = const(0x15)
 _SET_HOSTNAME = const(0x16)
@@ -137,17 +137,26 @@
 
     TCP_MODE = const(0)
     UDP_MODE = const(1)
     TLS_MODE = const(2)
 
     # pylint: disable=too-many-arguments
     def __init__(
-        self, spi, cs_dio, ready_dio, reset_dio, gpio0_dio=None, *, debug=False
+        self,
+        spi,
+        cs_dio,
+        ready_dio,
+        reset_dio,
+        gpio0_dio=None,
+        *,
+        debug=False,
+        debug_show_secrets=False,
     ):
         self._debug = debug
+        self._debug_show_secrets = debug_show_secrets
         self.set_psk = False
         self.set_crt = False
         self._buffer = bytearray(10)
         self._pbuf = bytearray(1)  # buffer for param read
         self._sendbuf = bytearray(256)  # buffer for command sending
         self._socknum_ll = [[0]]  # pre-made list of list of socket #
 
@@ -321,15 +330,15 @@
     def _send_command_get_response(
         self,
         cmd,
         params=None,
         *,
         reply_params=1,
         sent_param_len_16=False,
-        recv_param_len_16=False
+        recv_param_len_16=False,
     ):
         """Send a high level SPI command, wait and return the response"""
         self._send_command(cmd, params, param_len_16=sent_param_len_16)
         return self._wait_response_cmd(
             cmd, reply_params, param_len_16=recv_param_len_16
         )
 
@@ -377,15 +386,16 @@
             print("Start scan")
         resp = self._send_command_get_response(_START_SCAN_NETWORKS)
         if resp[0][0] != 1:
             raise OSError("Failed to start AP scan")
 
     def get_scan_networks(self):
         """The results of the latest SSID scan. Returns a list of dictionaries with
-        'ssid', 'rssi', 'encryption', bssid, and channel entries, one for each AP found"""
+        'ssid', 'rssi', 'encryption', bssid, and channel entries, one for each AP found
+        """
         self._send_command(_SCAN_NETWORKS)
         names = self._wait_response_cmd(_SCAN_NETWORKS)
         # print("SSID names:", names)
         APs = []  # pylint: disable=invalid-name
         for i, name in enumerate(names):
             a_p = {"ssid": name}
             rssi = self._send_command_get_response(_GET_IDX_RSSI_CMD, ((i,),))[0]
@@ -569,15 +579,18 @@
         or raise an exception on failure.
 
         :param ssid: the SSID to connect to
         :param passphrase: the password of the access point
         :param timeout_s: number of seconds until we time out and fail to create AP
         """
         if self._debug:
-            print("Connect to AP", ssid, password)
+            print(
+                f"Connect to AP: {ssid=}, password=\
+                    {repr(password if self._debug_show_secrets else '*' * len(password))}"
+            )
         if isinstance(ssid, str):
             ssid = bytes(ssid, "utf-8")
         if password:
             if isinstance(password, str):
                 password = bytes(password, "utf-8")
             self.wifi_set_passphrase(ssid, password)
         else:
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/adafruit_esp32spi_socket.py` & `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,26 +30,28 @@
 SOCK_STREAM = const(0)
 SOCK_DGRAM = const(1)
 AF_INET = const(2)
 NO_SOCKET_AVAIL = const(255)
 
 MAX_PACKET = const(4000)
 
+
 # pylint: disable=too-many-arguments, unused-argument
 def getaddrinfo(host, port, family=0, socktype=0, proto=0, flags=0):
     """Given a hostname and a port name, return a 'socket.getaddrinfo'
     compatible list of tuples. Honestly, we ignore anything but host & port"""
     if not isinstance(port, int):
         raise ValueError("Port must be an integer")
     ipaddr = _the_interface.get_host_by_name(host)
     return [(AF_INET, socktype, proto, "", (ipaddr, port))]
 
 
 # pylint: enable=too-many-arguments, unused-argument
 
+
 # pylint: disable=unused-argument, redefined-builtin, invalid-name
 class socket:
     """A simplified implementation of the Python 'socket' class, for connecting
     through an interface to a remote device"""
 
     # pylint: disable=too-many-arguments
     def __init__(
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py` & `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/adafruit_esp32spi_wsgiserver.py` & `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/adafruit_esp32spi_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/adafruit_esp32spi/digitalio.py` & `adafruit-circuitpython-esp32spi-5.0.6/adafruit_esp32spi/digitalio.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,15 @@
     """Implementation of DigitalIO module for ESP32SPI.
 
     :param ESP_SPIcontrol esp: The ESP object we are using.
     :param int pin: Valid ESP32 GPIO Pin, predefined in ESP32_GPIO_PINS.
     """
 
     _pin = None
+
     # pylint: disable = attribute-defined-outside-init
     def __init__(self, esp, pin):
         self._esp = esp
         self._pin = Pin(pin, self._esp)
         self.direction = Direction.INPUT
 
     def __enter__(self):
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/docs/_static/favicon.ico` & `adafruit-circuitpython-esp32spi-5.0.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/docs/api.rst` & `adafruit-circuitpython-esp32spi-5.0.6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/docs/conf.py` & `adafruit-circuitpython-esp32spi-5.0.6/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/docs/index.rst` & `adafruit-circuitpython-esp32spi-5.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_aio_post.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_cheerlights.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_ipconfig.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_ipconfig.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_localtime.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_localtime.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_simpletest.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_simpletest_rp2040.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_simpletest_rp2040.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_tcp_client.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_tcp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_udp_client.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_udp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_wpa2ent_aio_post.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_wpa2ent_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/esp32spi_wpa2ent_simpletest.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/esp32spi_wpa2ent_simpletest.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import busio
 from digitalio import DigitalInOut
 
 import adafruit_requests as requests
 import adafruit_esp32spi.adafruit_esp32spi_socket as socket
 from adafruit_esp32spi import adafruit_esp32spi
 
+
 # Version number comparison code. Credit to gnud on stackoverflow
 # (https://stackoverflow.com/a/1714190), swapping out cmp() to
 # support Python 3.x and thus, CircuitPython
 def version_compare(version1, version2):
     def normalize(v):
         return [int(x) for x in re.sub(r"(\.0+)*$", "", v).split(".")]
```

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/gpio/esp32spi_gpio.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/esp32spi_gpio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/gpio/gpio.md` & `adafruit-circuitpython-esp32spi-5.0.6/examples/gpio/gpio.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/server/esp32spi_wsgiserver.py` & `adafruit-circuitpython-esp32spi-5.0.6/examples/server/esp32spi_wsgiserver.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/examples/server/static/led_color_picker_example.js` & `adafruit-circuitpython-esp32spi-5.0.6/examples/server/static/led_color_picker_example.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32spi-5.0.5/pyproject.toml` & `adafruit-circuitpython-esp32spi-5.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-esp32spi"
 description = "CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI"
-version = "5.0.5"
+version = "5.0.6"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI"}
 keywords = [
     "adafruit",
```

