# Comparing `tmp/xhs-0.2.2.tar.gz` & `tmp/xhs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.2.2.tar", last modified: Sun May 21 02:03:15 2023, max compression
+gzip compressed data, was "xhs-0.2.3.tar", last modified: Thu Jun 22 02:45:57 2023, max compression
```

## Comparing `xhs-0.2.2.tar` & `xhs-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:03:15.621158 xhs-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-21 02:03:04.000000 xhs-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-21 02:03:04.000000 xhs-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-21 02:03:04.000000 xhs-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-21 02:03:15.621158 xhs-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-21 02:03:04.000000 xhs-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 02:03:04.000000 xhs-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 02:03:15.621158 xhs-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-21 02:03:04.000000 xhs-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:03:15.621158 xhs-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-21 02:03:04.000000 xhs-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-21 02:03:04.000000 xhs-0.2.2/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-21 02:03:04.000000 xhs-0.2.2/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 02:03:04.000000 xhs-0.2.2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:03:15.621158 xhs-0.2.2/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-05-21 02:03:04.000000 xhs-0.2.2/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:03:15.621158 xhs-0.2.2/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-21 02:03:15.000000 xhs-0.2.2/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:45:57.478889 xhs-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-22 02:45:44.000000 xhs-0.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-22 02:45:44.000000 xhs-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-22 02:45:44.000000 xhs-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-22 02:45:57.478889 xhs-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-22 02:45:44.000000 xhs-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 02:45:44.000000 xhs-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-22 02:45:57.478889 xhs-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-22 02:45:44.000000 xhs-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:45:57.474889 xhs-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-22 02:45:44.000000 xhs-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-22 02:45:44.000000 xhs-0.2.3/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-22 02:45:44.000000 xhs-0.2.3/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 02:45:44.000000 xhs-0.2.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:45:57.478889 xhs-0.2.3/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-06-22 02:45:44.000000 xhs-0.2.3/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:45:57.478889 xhs-0.2.3/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 02:45:57.000000 xhs-0.2.3/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.2.2/CHANGELOG.md` & `xhs-0.2.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.2.3
+
+### Added
+
+- add get self info v2 api
+- add get home feed categories api
+
+### Fixed
+
+- fix basic usage is not work
+
 ## 0.2.2
 
 ### Added
 
 - add a custom sign func to constructor
 
 ## 0.2.1
```

### Comparing `xhs-0.2.2/LICENSE` & `xhs-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.2.2/setup.py` & `xhs-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.2/tests/__init__.py` & `xhs-0.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.2/tests/test_help.py` & `xhs-0.2.3/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.2.2/tests/test_xhs.py` & `xhs-0.2.3/tests/test_xhs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,52 @@
-import pytest
-import requests
+from time import sleep
 
-from xhs import DataFetchError, FeedType, IPBlockError, XhsClient
+import pytest
+from playwright.sync_api import sync_playwright
 
+from xhs import FeedType, IPBlockError, XhsClient
+from xhs.exception import SignError
 from . import test_cookie
 from .utils import beauty_print
 
 
+def get_context_page(playwright):
+    chromium = playwright.chromium
+    browser = chromium.launch(headless=True)
+    browser_context = browser.new_context(
+        viewport={"width": 1920, "height": 1080},
+        user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
+    )
+    browser_context.add_init_script(path="stealth.min.js")
+    context_page = browser_context.new_page()
+    return browser_context, context_page
+
+
+playwright = sync_playwright().start()
+browser_context, context_page = get_context_page(playwright)
+
+
 @pytest.fixture
 def xhs_client():
-    def sign(uri, data=None, a1=""):
-        res = requests.post("http://35.78.99.223:5000/xhs/sign", json={
-            "uri": uri,
-            "data": data,
-            "a1": a1
-        })
-        return res.json()
+    def sign(uri, data, a1="", web_session=""):
+        context_page.goto("https://www.xiaohongshu.com")
+        cookie_list = browser_context.cookies()
+        web_session_cookie = list(filter(lambda cookie: cookie["name"] == "web_session", cookie_list))
+        if not web_session_cookie:
+            browser_context.add_cookies([
+                {'name': 'web_session', 'value': web_session, 'domain': ".xiaohongshu.com", 'path': "/"},
+                {'name': 'a1', 'value': a1, 'domain': ".xiaohongshu.com", 'path': "/"}]
+            )
+            sleep(1)
+        encrypt_params = context_page.evaluate("([url, data]) => window._webmsxyw(url, data)", [uri, data])
+        return {
+            "x-s": encrypt_params["X-s"],
+            "x-t": str(encrypt_params["X-t"])
+        }
+
     return XhsClient(cookie=test_cookie, sign=sign)
 
 
 # def test_xhs_client_init():
 #     xhs_client = XhsClient()
 #     assert xhs_client
 
@@ -28,20 +55,19 @@
 #     xhs_client = XhsClient()
 #     cd = xhs_client.cookie_dict
 #     beauty_print(cd)
 #     assert "web_session" in cd
 
 
 def test_external_sign_func():
-
     def sign(url, data=None, a1=""):
         """signature url and data in here"""
         return {}
 
-    with pytest.raises(DataFetchError):
+    with pytest.raises(SignError):
         xhs_client = XhsClient(sign=sign)
         xhs_client.get_qrcode()
 
 
 def test_get_note_by_id(xhs_client: XhsClient):
     note_id = "6413cf6b00000000270115b5"
     data = xhs_client.get_note_by_id(note_id)
@@ -57,36 +83,64 @@
 
     note_id = "64426c3d000000001303eb83"
     data = xhs_client.get_note_by_id_from_html(note_id)
     beauty_print(data)
     assert data["note_id"] == note_id
 
 
+def test_report_note_metrics(xhs_client: XhsClient):
+    res = xhs_client.report_note_metrics(
+        note_id="646837b9000000001300a4c3",
+        note_type=1,
+        note_user_id="6037a89b0000000001007e72",
+        viewer_user_id="63273a77000000002303cc9b")
+    beauty_print(res)
+    assert res["success"]
+
+
 def test_get_self_info(xhs_client: XhsClient):
     data = xhs_client.get_self_info()
     beauty_print(data)
     assert isinstance(data, dict)
 
 
+def test_get_self_info2(xhs_client: XhsClient):
+    data = xhs_client.get_self_info2()
+    beauty_print(data)
+    assert isinstance(data, dict)
+
+
 def test_get_user_info(xhs_client: XhsClient):
     user_id = "5ff0e6410000000001008400"
     data = xhs_client.get_user_info(user_id)
     basic_info = data["basic_info"]
     beauty_print(data)
     assert (basic_info["red_id"] == "hh06ovo"
             or basic_info["nickname"] == "小王不爱睡")
 
 
+def test_get_home_feed_category(xhs_client: XhsClient):
+    data = xhs_client.get_home_feed_category()
+    beauty_print(data)
+    assert len(data)
+
+
 def test_get_home_feed(xhs_client: XhsClient):
     recommend_type = FeedType.RECOMMEND
     data = xhs_client.get_home_feed(recommend_type)
     beauty_print(data)
     assert len(data["items"]) > 0
 
 
+def test_get_search_suggestion(xhs_client: XhsClient):
+    res = xhs_client.get_search_suggestion("jvm")
+    beauty_print(res)
+    assert len(res)
+
+
 def test_get_note_by_keyword(xhs_client: XhsClient):
     keyword = "小红书"
     data = xhs_client.get_note_by_keyword(keyword)
     beauty_print(data)
     assert len(data["items"]) > 0
 
 
@@ -132,18 +186,19 @@
 
 def test_get_qrcode(xhs_client: XhsClient):
     data = xhs_client.get_qrcode()
     beauty_print(data)
     assert data["url"].startswith("xhsdiscover://")
 
 
-@pytest.mark.skip()
 def test_check_qrcode(xhs_client: XhsClient):
-    data = xhs_client.check_qrcode("901061680834121471", "658742")
-    assert data.get("code_status")
+    qrcode = xhs_client.get_qrcode()
+    data = xhs_client.check_qrcode(qr_id=qrcode["qr_id"], code=qrcode["code"])
+    beauty_print(data)
+    assert "code_status" in data
 
 
 @pytest.mark.skip()
 def test_comment_note(xhs_client: XhsClient):
     data = xhs_client.comment_note("642b96640000000014027cd2", "你最好说你在说你自己")
     beauty_print(data)
     assert data["comment"]["id"]
@@ -162,17 +217,17 @@
 def test_delete_comment(xhs_client: XhsClient):
     data = xhs_client.delete_note_comment("642b96640000000014027cd2",
                                           "642f801000000000150037f8")
     beauty_print(data)
 
 
 @pytest.mark.parametrize("note_id", [
-        "6413cf6b00000000270115b5",
-        "641718a200000000130143f2"
-    ])
+    "6413cf6b00000000270115b5",
+    "641718a200000000130143f2"
+])
 @pytest.mark.skip()
 def test_save_files_from_note_id(xhs_client: XhsClient, note_id: str):
     xhs_client.save_files_from_note_id(note_id, r"C:\Users\ReaJason\Desktop")
 
 
 @pytest.mark.parametrize("note_id", [
     "639a7064000000001f0098a8",
@@ -203,11 +258,17 @@
 def test_ip_block_error(xhs_client: XhsClient):
     with pytest.raises(IPBlockError):
         note_id = "6413cf6b00000000270115b5"
         for _ in range(150):
             xhs_client.get_note_by_id(note_id)
 
 
-# def test_activate(xhs_client: XhsClient):
-#     info = xhs_client.activate()
-#     beauty_print(info)
-#     assert info["session"]
+def test_activate(xhs_client: XhsClient):
+    info = xhs_client.activate()
+    beauty_print(info)
+    assert info["session"]
+
+
+def test_get_emojis(xhs_client: XhsClient):
+    emojis = xhs_client.get_emojis()
+    beauty_print(emojis)
+    assert len(emojis)
```

### Comparing `xhs-0.2.2/xhs/core.py` & `xhs-0.2.3/xhs/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import time
 from enum import Enum
 from typing import NamedTuple
 
 import requests
 
-from xhs.exception import DataFetchError, IPBlockError
+from xhs.exception import DataFetchError, IPBlockError, SignError, ErrorEnum
 
 from .help import (cookie_jar_to_cookie_str, download_file,
                    get_imgs_url_from_note, get_search_id, get_valid_path_name,
                    get_video_url_from_note, sign,
                    update_session_cookies_from_cookie)
 
 
@@ -105,18 +105,14 @@
                                     "AppleWebKit/537.36 "
                                     "(KHTML, like Gecko) "
                                     "Chrome/111.0.0.0 Safari/537.36")
         self.__session.headers = {
             "user-agent": user_agent,
             "Content-Type": "application/json"
         }
-        self.IP_ERROR_STR = "网络连接异常，请检查网络设置或重启试试"
-        self.IP_ERROR_CODE = 300012
-        self.NOTE_ABNORMAL_STR = "笔记状态异常，请稍后查看"
-        self.NOTE_ABNORMAL_CODE = -510001
         self.cookie = cookie
 
     @property
     def cookie(self):
         return cookie_jar_to_cookie_str(self.__session.cookies)
 
     @cookie.setter
@@ -139,30 +135,34 @@
 
     @user_agent.setter
     def user_agent(self, user_agent: str):
         self.__session.headers.update({"user-agent": user_agent})
 
     def _pre_headers(self, url: str, data=None):
         if self.sign:
-            self.__session.headers.update(self.sign(url, data, a1=self.cookie_dict.get("a1")))
+            self.__session.headers.update(
+                self.sign(url, data, a1=self.cookie_dict.get("a1"),
+                          web_session=self.cookie_dict.get("web_session")))
         else:
             signs = sign(url, data, a1=self.cookie_dict.get("a1"))
             self.__session.headers.update({"x-s": signs["x-s"]})
             self.__session.headers.update({"x-t": signs["x-t"]})
             self.__session.headers.update({"x-s-common": signs["x-s-common"]})
 
     def request(self, method, url, **kwargs):
         response = self.__session.request(
-                        method, url, timeout=self.timeout,
-                        proxies=self.proxies, **kwargs)
+            method, url, timeout=self.timeout,
+            proxies=self.proxies, **kwargs)
         data = response.json()
         if data["success"]:
             return data.get("data", data.get("success"))
-        elif data["code"] == self.IP_ERROR_CODE:
-            raise IPBlockError(self.IP_ERROR_STR)
+        elif data["code"] == ErrorEnum.IP_BLOCK.value.code:
+            raise IPBlockError(ErrorEnum.IP_BLOCK.value.msg)
+        elif data["code"] == ErrorEnum.SIGN_FAULT.value.code:
+            raise SignError(ErrorEnum.SIGN_FAULT.value.msg)
         else:
             raise DataFetchError(data.get("msg", None))
 
     def get(self, uri: str, params=None):
         final_uri = uri
         if isinstance(params, dict):
             final_uri = (f"{uri}?"
@@ -213,22 +213,57 @@
                 else:
                     new_dict[new_key] = value
             return new_dict
 
         url = "https://www.xiaohongshu.com/explore/" + note_id
         res = self.session.get(url, headers={"user-agent": self.user_agent})
         html = res.text
-        state = re.findall(r'window.__INITIAL_STATE__=({.*})</script>', html)[0].replace("undefined", '""')
+        state = re.findall(
+            r'window.__INITIAL_STATE__=({.*})</script>', html)[0].replace("undefined", '""')
         if state != "{}":
             new_dict = transform_json_keys(state)
             return new_dict["note"]["note"]
         elif self.IP_ERROR_STR in html:
             raise IPBlockError(self.IP_ERROR_STR)
         raise DataFetchError()
 
+    def report_note_metrics(self, note_id: str, note_type: int, note_user_id: str, viewer_user_id: str, followed_author=0, report_type=1, stay_seconds=0):
+        """report note stay seconds and other interaction info
+
+        :param note_id: note_id which you want to report
+        :type note_id: str
+        :param note_type: input value -> 1: note is images, 2: note is video
+        :type note_type: int
+        :param note_user_id: note author id
+        :type note_user_id: str
+        :param viewer_user_id: report user id
+        :type viewer_user_id: str
+        :param followed_author: 1: the viewer user follow note's author, 0: the viewer user don't follow note's author
+        :type followed_author: int
+        :param report_type: 1: the first report, 2: the second report, so you must report twice, defaults to 1
+        :type report_type: int, optional
+        :param stay_seconds: report metric -> note you stay seconds, defaults to 0
+        :type stay_seconds: int, optional
+        :return: same as api
+        :rtype: dict
+        """
+        uri = "/api/sns/web/v1/note/metrics_report"
+        data = {
+            "note_id": note_id,
+            "note_type": note_type,
+            "report_type": report_type,
+            "stress_test": False,
+            "viewer": {"user_id": viewer_user_id, "followed_author": followed_author},
+            "author": {"user_id": note_user_id},
+            "interaction": {"like": 0, "collect": 0, "comment": 0, "comment_read": 0},
+            "note": {"stay_seconds": stay_seconds},
+            "other": {"platform": "web"}
+        }
+        return self.post(uri, data)
+
     def save_files_from_note_id(self, note_id: str, dir_path: str):
         """this function will fetch note and save file in dir_path/note_title
 
         :param note_id: note_id that you want to fetch
         :type note_id: str
         :param dir_path: in fact, files will be stored in your dir_path/note_title directory
         :type dir_path: str
@@ -247,49 +282,64 @@
         if note["type"] == NoteType.VIDEO.value:
             video_url = get_video_url_from_note(note)
             video_filename = os.path.join(new_dir_path, f"{title}.mp4")
             download_file(video_url, video_filename)
         else:
             img_urls = get_imgs_url_from_note(note)
             for index, img_url in enumerate(img_urls):
-                img_file_name = os.path.join(new_dir_path, f"{title}{index}.png")
+                img_file_name = os.path.join(
+                    new_dir_path, f"{title}{index}.png")
                 download_file(img_url, img_file_name)
 
     def get_self_info(self):
         uri = "/api/sns/web/v1/user/selfinfo"
-        res = self.get(uri)
-        return res
+        return self.get(uri)
+
+    def get_self_info2(self):
+        uri = "/api/sns/web/v2/user/me"
+        return self.get(uri)
 
     def get_user_info(self, user_id: str):
         """
         :param user_id: user_id you want fetch
         :type user_id: str
         :return: {"basic_info":{"imageb":"imageb","nickname":"nickname","images":"images","red_id":"red_id","gender":1,"ip_location":"ip_location","desc":"desc"},"interactions":[{"count":"5","type":"follows","name":"关注"},{"type":"fans","name":"粉丝","count":"16736"},{"type":"interaction","name":"获赞与收藏","count":"293043"}],"tags":[{"icon":"icon","tagType":"info"}],"tab_public":{"collection":false},"extra_info":{"fstatus":"none"},"result":{"success":true,"code":0,"message":"success"}}
         :rtype: dict
         """
         uri = "/api/sns/web/v1/user/otherinfo"
         params = {
             "target_user_id": user_id
         }
         return self.get(uri, params)
 
+    def get_home_feed_category(self):
+        uri = "/api/sns/web/v1/homefeed/category"
+        return self.get(uri)["categories"]
+
     def get_home_feed(self, feed_type: FeedType):
         uri = "/api/sns/web/v1/homefeed"
         data = {
             "cursor_score": "",
             "num": 40,
             "refresh_type": 1,
             "note_index": 0,
             "unread_begin_note_id": "",
             "unread_end_note_id": "",
             "unread_note_count": 0,
             "category": feed_type.value
         }
         return self.post(uri, data)
 
+    def get_search_suggestion(self, keyword: str):
+        uri = "/api/sns/web/v1/sug/recommend"
+        params = {
+            "keyword": keyword
+        }
+        return [sug["text"] for sug in self.get(uri, params)["sug_items"]]
+
     def get_note_by_keyword(self, keyword: str,
                             page: int = 1, page_size: int = 20,
                             sort: SearchSortType = SearchSortType.GENERAL,
                             note_type: SearchNoteType = SearchNoteType.ALL):
         """search note by keyword
 
         :param keyword: what notes you want to search
@@ -353,15 +403,15 @@
             cursor = res["cursor"]
             note_ids = map(lambda note: note["note_id"], res["notes"])
 
             for note_id in note_ids:
                 try:
                     note = self.get_note_by_id(note_id)
                 except DataFetchError as e:
-                    if self.NOTE_ABNORMAL_STR in str(e):
+                    if ErrorEnum.NOTE_ABNORMAL.value.msg in str(e):
                         continue
                     else:
                         raise
                 interact_info = note["interact_info"]
                 note_info = Note(
                     note_id=note["note_id"],
                     title=note["title"],
@@ -440,21 +490,24 @@
             comments_cursor = comments_res.get("cursor", "")
             comments = comments_res["comments"]
             for comment in comments:
                 result.append(comment)
                 cur_sub_comment_count = int(comment["sub_comment_count"])
                 cur_sub_comments = comment["sub_comments"]
                 result.extend(cur_sub_comments)
-                sub_comments_has_more = comment["sub_comment_has_more"] and len(cur_sub_comments) < cur_sub_comment_count
+                sub_comments_has_more = comment["sub_comment_has_more"] and len(
+                    cur_sub_comments) < cur_sub_comment_count
                 sub_comment_cursor = comment["sub_comment_cursor"]
                 while sub_comments_has_more:
                     page_num = 30
-                    sub_comments_res = self.get_note_sub_comments(note_id, comment["id"], num=page_num, cursor=sub_comment_cursor)
+                    sub_comments_res = self.get_note_sub_comments(
+                        note_id, comment["id"], num=page_num, cursor=sub_comment_cursor)
                     sub_comments = sub_comments_res["comments"]
-                    sub_comments_has_more = sub_comments_res["has_more"] and len(sub_comments) == page_num
+                    sub_comments_has_more = sub_comments_res["has_more"] and len(
+                        sub_comments) == page_num
                     sub_comment_cursor = sub_comments_res["cursor"]
                     result.extend(sub_comments)
                     time.sleep(crawl_interval)
             time.sleep(crawl_interval)
         return result
 
     def comment_note(self, note_id: str, content: str):
@@ -585,7 +638,11 @@
         uri = "/api/sns/web/v1/note/like/page"
         params = {
             "user_id": user_id,
             "num": num,
             "cursor": cursor
         }
         return self.get(uri, params)
+
+    def get_emojis(self):
+        uri = "/api/im/redmoji/detail"
+        return self.get(uri)["emoji"]["tabs"][0]["collection"]
```

### Comparing `xhs-0.2.2/xhs/help.py` & `xhs-0.2.3/xhs/help.py`

 * *Files identical despite different names*

