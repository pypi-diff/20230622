# Comparing `tmp/martin-binance-1.3.1b3.tar.gz` & `tmp/martin_binance-1.3.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin-binance-1.3.1b3.tar", last modified: Tue Jun 20 15:14:34 2023, max compression
+gzip compressed data, was "martin_binance-1.3.1b5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin-binance-1.3.1b3.tar` & `martin_binance-1.3.1b5.tar`

### file list

```diff
@@ -1,44 +1,27 @@
--rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.1b3/.deepsource.toml
--rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.1b3/.dockerignore
--rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.1b3/.github/FUNDING.yml
--rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.1b3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.1b3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.1b3/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.1b3/.gitignore
--rwxr-xr-x   0        0        0    18795 2023-06-20 11:01:32.418813 martin-binance-1.3.1b3/CHANGELOG.md
--rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.1b3/Dockerfile
--rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.1b3/LICENSE
--rwxr-xr-x   0        0        0     3944 2023-06-19 19:17:03.912066 martin-binance-1.3.1b3/README.md
--rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.1b3/doc/Create_strategy.png
--rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.1b3/doc/Model of logarithmic grid.ods
--rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.1b3/doc/Modified martingale.svg
--rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.1b3/doc/graf1.png
--rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.1b3/doc/tlg_notify.png
--rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.1b3/doc/tmux.png
--rw-r--r--   0        0        0     1968 2023-06-20 14:54:56.871877 martin-binance-1.3.1b3/martin_binance/__init__.py
--rw-r--r--   0        0        0     4187 2023-06-20 15:14:30.461764 martin-binance-1.3.1b3/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2946 2023-06-10 10:09:47.513439 martin-binance-1.3.1b3/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-06-10 10:09:47.513439 martin-binance-1.3.1b3/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    14050 2023-06-19 19:16:08.304258 martin-binance-1.3.1b3/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6721 2023-06-19 17:47:04.745501 martin-binance-1.3.1b3/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6716 2023-06-19 17:47:04.745501 martin-binance-1.3.1b3/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6722 2023-06-19 17:47:04.745501 martin-binance-1.3.1b3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4707 2023-06-10 10:09:47.517442 martin-binance-1.3.1b3/martin_binance/client.py
--rw-r--r--   0        0        0   185525 2023-06-20 10:20:51.033666 martin-binance-1.3.1b3/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.1b3/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.1b3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.1b3/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.1b3/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    85764 2023-06-19 21:29:05.366900 martin-binance-1.3.1b3/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.1b3/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.1b3/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.1b3/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16369 2023-06-19 17:47:04.749497 martin-binance-1.3.1b3/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-06-10 10:09:47.517442 martin-binance-1.3.1b3/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1274 2023-06-20 08:42:34.849378 martin-binance-1.3.1b3/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.1b3/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.1b3/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1360 2023-06-20 15:04:52.248056 martin-binance-1.3.1b3/pyproject.toml
--rw-r--r--   0        0        0      335 2023-06-19 19:16:08.288221 martin-binance-1.3.1b3/requirements.txt
--rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.1b3/uml/architecture.puml
--rw-r--r--   0        0        0     5151 1970-01-01 00:00:00.000000 martin-binance-1.3.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-21 14:52:44.450621 martin_binance-1.3.1b5/LICENSE
+-rwxr-xr-x   0        0        0     3944 2023-06-21 14:52:44.450621 martin_binance-1.3.1b5/README.md
+-rw-r--r--   0        0        0     2013 2023-06-21 14:52:44.494621 martin_binance-1.3.1b5/martin_binance/__init__.py
+-rw-r--r--   0        0        0     4186 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2946 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    14050 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6721 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6716 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6722 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4707 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/client.py
+-rw-r--r--   0        0        0   185525 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2023-06-21 14:52:44.498621 martin_binance-1.3.1b5/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    85764 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16369 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1282 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1354 2023-06-21 14:52:44.502621 martin_binance-1.3.1b5/pyproject.toml
+-rw-r--r--   0        0        0     5145 1970-01-01 00:00:00.000000 martin_binance-1.3.1b5/PKG-INFO
```

### Comparing `martin-binance-1.3.1b3/LICENSE` & `martin_binance-1.3.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/README.md` & `martin_binance-1.3.1b5/README.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/__init__.py` & `martin_binance-1.3.1b5/martin_binance/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,21 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.1b3"
+__version__ = "1.3.1b5"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
-#
-import platform
 
-print(f"Python {platform.python_version()}")
-#
 STANDALONE = True
 if 'margin' in str(Path().resolve()):
     print('margin detected')
     STANDALONE = False
 WORK_PATH = Path(Path.home(), ".MartinBinance")
 CONFIG_PATH = Path(WORK_PATH, "config")
 CONFIG_FILE = Path(CONFIG_PATH, "ms_cfg.toml")
@@ -29,28 +25,31 @@
     LOG_PATH = Path(WORK_PATH, "log")
     LAST_STATE_PATH = Path(WORK_PATH, "last_state")
     BACKTEST_PATH = Path(WORK_PATH, "back_test")
 else:
     LOG_PATH = None
     LAST_STATE_PATH = None
     BACKTEST_PATH = None
-if CONFIG_FILE.exists():
-    print(f"Client config found at {CONFIG_FILE}")
-else:
-    print("Can't find config file! Creating it...")
-    CONFIG_PATH.mkdir(parents=True, exist_ok=True)
-    if STANDALONE:
-        LOG_PATH.mkdir(parents=True, exist_ok=True)
-        LAST_STATE_PATH.mkdir(parents=True, exist_ok=True)
-    copy(Path(Path(__file__).parent.absolute(), "ms_cfg.toml.template"), CONFIG_FILE)
-    copy(Path(Path(__file__).parent.absolute(), "funds_rate.db.template"), DB_FILE)
-    copy(Path(Path(__file__).parent.absolute(), "cli_0_BTCUSDT.py.template"), Path(WORK_PATH, "cli_0_BTCUSDT.py"))
-    copy(Path(Path(__file__).parent.absolute(), "cli_1_BTCUSDT.py.template"), Path(WORK_PATH, "cli_1_BTCUSDT.py"))
-    copy(Path(Path(__file__).parent.absolute(), "cli_2_TESTBTCTESTUSDT.py.template"),
-         Path(WORK_PATH, "cli_2_TESTBTCTESTUSDT.py"))
-    print(f"Before the first run, set the parameters in {CONFIG_FILE}")
-    if STANDALONE:
-        raise SystemExit(1)
-    raise UserWarning()
 
 def init():
-    pass
+    if CONFIG_FILE.exists():
+        print(f"Client config found at {CONFIG_FILE}")
+    else:
+        print("Can't find client config file! Creating it...")
+        CONFIG_PATH.mkdir(parents=True, exist_ok=True)
+        if STANDALONE:
+            LOG_PATH.mkdir(parents=True, exist_ok=True)
+            LAST_STATE_PATH.mkdir(parents=True, exist_ok=True)
+        copy(Path(Path(__file__).parent.absolute(), "ms_cfg.toml.template"), CONFIG_FILE)
+        copy(Path(Path(__file__).parent.absolute(), "funds_rate.db.template"), DB_FILE)
+        copy(Path(Path(__file__).parent.absolute(), "cli_0_BTCUSDT.py.template"), Path(WORK_PATH, "cli_0_BTCUSDT.py"))
+        copy(Path(Path(__file__).parent.absolute(), "cli_1_BTCUSDT.py.template"), Path(WORK_PATH, "cli_1_BTCUSDT.py"))
+        copy(Path(Path(__file__).parent.absolute(), "cli_2_TESTBTCTESTUSDT.py.template"),
+             Path(WORK_PATH, "cli_2_TESTBTCTESTUSDT.py"))
+        print(f"Before the first run, set the parameters in {CONFIG_FILE}")
+        if STANDALONE:
+            raise SystemExit(1)
+        raise UserWarning()
+
+
+if __name__ == '__main__':
+    init()
```

### Comparing `martin-binance-1.3.1b3/martin_binance/backtest/OoTSP.py` & `martin_binance-1.3.1b5/martin_binance/backtest/OoTSP.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Optimization of Trading Strategy Parameters
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-3"
+__version__ = "1.3.1b5"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 import importlib.util
 from decimal import Decimal
 import optuna
@@ -60,15 +60,15 @@
             choices=["New", "Plot from saved"],
         ),
         inquirer.Text(
             "n_trials",
             message="Enter number of cycles, from 50 to 500",
             ignore=lambda x: x["mode"] == "Plot from saved",
             default='150',
-            validate=lambda _, c: 10 <= int(c) < 500,
+            validate=lambda _, c: 2 <= int(c) < 500,
         ),
     ]
 
     answers = inquirer.prompt(questions, theme=GreenPassion())
 
     study_name = answers.get('path')  # Unique identifier of the study
     storage_name = f"sqlite:///{Path(BACKTEST_PATH, study_name, f'{study_name}.db')}"
```

### Comparing `martin-binance-1.3.1b3/martin_binance/backtest/VCoSEL.py` & `martin_binance-1.3.1b5/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/backtest/exchange_simulator.py` & `martin_binance-1.3.1b5/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/cli_0_BTCUSDT.py.template` & `martin_binance-1.3.1b5/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/cli_1_BTCUSDT.py.template` & `martin_binance-1.3.1b5/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin_binance-1.3.1b5/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/client.py` & `martin_binance-1.3.1b5/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/executor.py` & `martin_binance-1.3.1b5/martin_binance/executor.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/funds_rate.db.template` & `martin_binance-1.3.1b5/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin_binance-1.3.1b5/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/margin_wrapper.py` & `martin_binance-1.3.1b5/martin_binance/margin_wrapper.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/ms_cfg.toml.template` & `martin_binance-1.3.1b5/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/service/funds_rate_exporter.py` & `martin_binance-1.3.1b5/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/service/grafana.json` & `martin_binance-1.3.1b5/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.1b3/martin_binance/service/relaunch.py` & `martin_binance-1.3.1b5/martin_binance/service/relaunch.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 ####################################################################
 # Restart trade sessions saved in /last_state
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0-4"
+__version__ = "1.3.1"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 
 import libtmux
 import time
 from martin_binance import Path, WORK_PATH, LAST_STATE_PATH
@@ -22,14 +22,14 @@
 session = server.find_where({"session_name": "Trade"})
 
 if session:
     for window in session.list_windows():
         window_name = window.get('window_name')
         pane = window.attached_pane
         if window_name == 'srv':
-            pane.send_keys('exch_srv.py', enter=True)
+            pane.send_keys('exchanges-wrapper-srv', enter=True)
         else:
             last_state = Path(LAST_STATE_PATH, f"{window_name.replace('-', '_').replace('/', '')}.json")
             pair = Path(WORK_PATH, f"cli_{window_name.replace('-', '_').replace('/', '')}.py")
             if pair.exists() and last_state.exists():
                 pane.send_keys(f"{pair} 1", enter=True)
         time.sleep(4)
```

### Comparing `martin-binance-1.3.1b3/pyproject.toml` & `martin_binance-1.3.1b5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "exchanges-wrapper==1.3.0.post2",
+    "exchanges-wrapper==1.3.1",
     "margin-strategy-sdk==0.0.11",
     "aiohttp==3.8.4",
     "grpcio==1.48.1",
     "grpcio-tools==1.48.1",
     "jsonpickle==3.0.1",
     "psutil==5.9.5",
     "requests==2.31.0",
```

### Comparing `martin-binance-1.3.1b3/PKG-INFO` & `martin_binance-1.3.1b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.1b3
+Version: 1.3.1b5
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==1.3.0.post2
+Requires-Dist: exchanges-wrapper==1.3.1
 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: grpcio==1.48.1
 Requires-Dist: grpcio-tools==1.48.1
 Requires-Dist: jsonpickle==3.0.1
 Requires-Dist: psutil==5.9.5
 Requires-Dist: requests==2.31.0
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.1b3 Summary: Free
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.1b5 Summary: Free
 trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: exchanges-wrapper==1.3.0.post2 Requires-Dist: margin-strategy-sdk==0.0.11
+Dist: exchanges-wrapper==1.3.1 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.48.1 Requires-Dist:
 grpcio-tools==1.48.1 Requires-Dist: jsonpickle==3.0.1 Requires-Dist:
 psutil==5.9.5 Requires-Dist: requests==2.31.0 Requires-Dist: simplejson==3.19.1
 Requires-Dist: toml==0.10.2 Requires-Dist: libtmux==0.22.1 Requires-Dist:
 colorama==0.4.6 Requires-Dist: prometheus-client==0.17.0 Requires-Dist:
 optuna==3.2.0 Requires-Dist: plotly==5.15.0 Requires-Dist: pandas==2.0.2
 Requires-Dist: dash==2.10.2 Requires-Dist: future==0.18.3 Requires-Dist:
```

