# Comparing `tmp/local-first-tistory-0.0.1.tar.gz` & `tmp/local-first-tistory-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-first-tistory-0.0.1.tar", last modified: Tue Jun 20 08:04:12 2023, max compression
+gzip compressed data, was "local-first-tistory-0.0.2.tar", last modified: Thu Jun 22 17:49:23 2023, max compression
```

## Comparing `local-first-tistory-0.0.1.tar` & `local-first-tistory-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-20 08:04:12.410699 local-first-tistory-0.0.1/
--rw-r--r--   0 user1     (1000) users      (984)     5415 2023-06-20 08:04:12.410699 local-first-tistory-0.0.1/PKG-INFO
--rw-r--r--   0 user1     (1000) users      (984)     4759 2023-06-20 07:52:02.000000 local-first-tistory-0.0.1/README.md
-drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-20 08:04:12.410699 local-first-tistory-0.0.1/local_first_tistory.egg-info/
--rw-r--r--   0 user1     (1000) users      (984)     5415 2023-06-20 08:04:12.000000 local-first-tistory-0.0.1/local_first_tistory.egg-info/PKG-INFO
--rw-r--r--   0 user1     (1000) users      (984)      387 2023-06-20 08:04:12.000000 local-first-tistory-0.0.1/local_first_tistory.egg-info/SOURCES.txt
--rw-r--r--   0 user1     (1000) users      (984)        1 2023-06-20 08:04:12.000000 local-first-tistory-0.0.1/local_first_tistory.egg-info/dependency_links.txt
--rw-r--r--   0 user1     (1000) users      (984)       44 2023-06-20 08:04:12.000000 local-first-tistory-0.0.1/local_first_tistory.egg-info/entry_points.txt
--rw-r--r--   0 user1     (1000) users      (984)       87 2023-06-20 08:04:12.000000 local-first-tistory-0.0.1/local_first_tistory.egg-info/requires.txt
--rw-r--r--   0 user1     (1000) users      (984)        4 2023-06-20 08:04:12.000000 local-first-tistory-0.0.1/local_first_tistory.egg-info/top_level.txt
--rw-r--r--   0 user1     (1000) users      (984)       79 2023-06-20 08:04:12.410699 local-first-tistory-0.0.1/setup.cfg
--rw-r--r--   0 user1     (1000) users      (984)     1232 2023-06-20 07:59:27.000000 local-first-tistory-0.0.1/setup.py
-drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-20 08:04:12.410699 local-first-tistory-0.0.1/src/
--rw-r--r--   0 user1     (1000) users      (984)        0 2023-06-20 05:16:25.000000 local-first-tistory-0.0.1/src/__init__.py
--rw-r--r--   0 user1     (1000) users      (984)     4109 2023-06-20 08:03:51.000000 local-first-tistory-0.0.1/src/auth.py
--rw-r--r--   0 user1     (1000) users      (984)     1478 2023-06-20 06:49:51.000000 local-first-tistory-0.0.1/src/category.py
--rw-r--r--   0 user1     (1000) users      (984)      633 2023-06-20 06:49:49.000000 local-first-tistory-0.0.1/src/env.py
--rw-r--r--   0 user1     (1000) users      (984)     2532 2023-06-20 06:49:47.000000 local-first-tistory-0.0.1/src/image.py
--rw-r--r--   0 user1     (1000) users      (984)     6253 2023-06-20 06:49:47.000000 local-first-tistory-0.0.1/src/markdown.py
--rw-r--r--   0 user1     (1000) users      (984)     1163 2023-06-20 06:49:43.000000 local-first-tistory-0.0.1/src/tistory.py
+drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-22 17:49:23.336390 local-first-tistory-0.0.2/
+-rw-r--r--   0 user1     (1000) users      (984)     5425 2023-06-22 17:49:23.336390 local-first-tistory-0.0.2/PKG-INFO
+-rw-r--r--   0 user1     (1000) users      (984)     4769 2023-06-20 08:05:42.000000 local-first-tistory-0.0.2/README.md
+drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-22 17:49:23.336390 local-first-tistory-0.0.2/local_first_tistory.egg-info/
+-rw-r--r--   0 user1     (1000) users      (984)     5425 2023-06-22 17:49:23.000000 local-first-tistory-0.0.2/local_first_tistory.egg-info/PKG-INFO
+-rw-r--r--   0 user1     (1000) users      (984)      387 2023-06-22 17:49:23.000000 local-first-tistory-0.0.2/local_first_tistory.egg-info/SOURCES.txt
+-rw-r--r--   0 user1     (1000) users      (984)        1 2023-06-22 17:49:23.000000 local-first-tistory-0.0.2/local_first_tistory.egg-info/dependency_links.txt
+-rw-r--r--   0 user1     (1000) users      (984)       44 2023-06-22 17:49:23.000000 local-first-tistory-0.0.2/local_first_tistory.egg-info/entry_points.txt
+-rw-r--r--   0 user1     (1000) users      (984)       87 2023-06-22 17:49:23.000000 local-first-tistory-0.0.2/local_first_tistory.egg-info/requires.txt
+-rw-r--r--   0 user1     (1000) users      (984)        4 2023-06-22 17:49:23.000000 local-first-tistory-0.0.2/local_first_tistory.egg-info/top_level.txt
+-rw-r--r--   0 user1     (1000) users      (984)       79 2023-06-22 17:49:23.336390 local-first-tistory-0.0.2/setup.cfg
+-rw-r--r--   0 user1     (1000) users      (984)     1244 2023-06-22 17:49:23.000000 local-first-tistory-0.0.2/setup.py
+drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-22 17:49:23.336390 local-first-tistory-0.0.2/src/
+-rw-r--r--   0 user1     (1000) users      (984)        0 2023-06-20 05:16:25.000000 local-first-tistory-0.0.2/src/__init__.py
+-rw-r--r--   0 user1     (1000) users      (984)     4189 2023-06-20 08:07:35.000000 local-first-tistory-0.0.2/src/auth.py
+-rw-r--r--   0 user1     (1000) users      (984)     1557 2023-06-22 17:17:35.000000 local-first-tistory-0.0.2/src/category.py
+-rw-r--r--   0 user1     (1000) users      (984)      633 2023-06-20 06:49:49.000000 local-first-tistory-0.0.2/src/env.py
+-rw-r--r--   0 user1     (1000) users      (984)     2532 2023-06-20 06:49:47.000000 local-first-tistory-0.0.2/src/image.py
+-rw-r--r--   0 user1     (1000) users      (984)     6391 2023-06-22 17:31:48.000000 local-first-tistory-0.0.2/src/markdown.py
+-rw-r--r--   0 user1     (1000) users      (984)     1163 2023-06-20 06:49:43.000000 local-first-tistory-0.0.2/src/tistory.py
```

### Comparing `local-first-tistory-0.0.1/PKG-INFO` & `local-first-tistory-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local-first-tistory
-Version: 0.0.1
+Version: 0.0.2
 Summary: It will help you to manage locally saved markdown             to upload to Tistory
 Home-page: https://github.com/choikangjae/local-first-tistory
 Author: Kangjae Choi
 Author-email: choikj33@gmail.com
 License: MIT
 Keywords: tistory terminal markdown image
 Classifier: Operating System :: POSIX
@@ -41,20 +41,20 @@
 
 ### Installation
 
 - Python >= 3.9
 - To install package:
 
     ```bash
-    pip install tistory-helper
+    pip install local-first-tistory
     ```
 
 ### Quick Start
 
-You can use `tistory-helper` using `$ tistory [command]`.
+You can use `local-first-tistory` using `$ tistory [command]`.
 
 To start off, you run:
 
 ```bash
 tistory init
 ```
```

### Comparing `local-first-tistory-0.0.1/README.md` & `local-first-tistory-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
 ### Installation
 
 - Python >= 3.9
 - To install package:
 
     ```bash
-    pip install tistory-helper
+    pip install local-first-tistory
     ```
 
 ### Quick Start
 
-You can use `tistory-helper` using `$ tistory [command]`.
+You can use `local-first-tistory` using `$ tistory [command]`.
 
 To start off, you run:
 
 ```bash
 tistory init
 ```
```

### Comparing `local-first-tistory-0.0.1/local_first_tistory.egg-info/PKG-INFO` & `local-first-tistory-0.0.2/local_first_tistory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local-first-tistory
-Version: 0.0.1
+Version: 0.0.2
 Summary: It will help you to manage locally saved markdown             to upload to Tistory
 Home-page: https://github.com/choikangjae/local-first-tistory
 Author: Kangjae Choi
 Author-email: choikj33@gmail.com
 License: MIT
 Keywords: tistory terminal markdown image
 Classifier: Operating System :: POSIX
@@ -41,20 +41,20 @@
 
 ### Installation
 
 - Python >= 3.9
 - To install package:
 
     ```bash
-    pip install tistory-helper
+    pip install local-first-tistory
     ```
 
 ### Quick Start
 
-You can use `tistory-helper` using `$ tistory [command]`.
+You can use `local-first-tistory` using `$ tistory [command]`.
 
 To start off, you run:
 
 ```bash
 tistory init
 ```
```

### Comparing `local-first-tistory-0.0.1/setup.py` & `local-first-tistory-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import bump
 from setuptools import setup, find_packages
 
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as fh:
     long_description = fh.read()
 
 
@@ -13,15 +14,15 @@
     "mdx_truly_sane_lists",
     "markdown_link_attr_modifier",
     "click",
 ]
 
 setup(
     name="local-first-tistory",
-    version="0.0.1",
+    version="0.0.2",
     author="Kangjae Choi",
     author_email="choikj33@gmail.com",
     description="It will help you to manage locally saved markdown \
             to upload to Tistory",
     license="MIT",
     keywords="tistory terminal markdown image",
     url="https://github.com/choikangjae/local-first-tistory",
```

### Comparing `local-first-tistory-0.0.1/src/auth.py` & `local-first-tistory-0.0.2/src/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,46 +70,51 @@
         set_key(key_to_set="BLOG_NAME", value_to_set=blog_name, dotenv_path=DOTENV_PATH)
         set_key(
             key_to_set="REDIRECT_URI",
             value_to_set=f"{blog_name}.tistory.com",
             dotenv_path=DOTENV_PATH,
         )
         print("블로그 이름 저장 완료")
+        print()
 
     if APP_ID is None:
         print(
             """https://www.tistory.com/guide/api/manage/register \
 에서 App ID와 Secret Key를 발급받아주세요."""
         )
         app_id = input("App ID를 입력해주세요: ")
         set_key(key_to_set="APP_ID", value_to_set=app_id, dotenv_path=DOTENV_PATH)
         print("App ID 저장 완료")
+        print()
 
     if SECRET_KEY is None:
         secret_key = input("Secret Key를 입력해주세요: ")
         set_key(
             key_to_set="SECRET_KEY", value_to_set=secret_key, dotenv_path=DOTENV_PATH
         )
         print("Secret Key 저장 완료")
+        print()
 
     if AUTHORIZATION_CODE is None:
         print("다음 url로 접속한 후 code를 발급받아주세요")
         print(generate_auth_url())
+        print()
 
         code = input(
             """code를 입력해주세요. \
 code는 다음과 같은 형태이며 \
 리다이렉트 된 주소를 통해 확인할 수 있습니다.
 https://www.tistory.com/oauth/your_blog_name.tistory.com?code={{{code}}}&state=: """
         )
         set_key(
             key_to_set="AUTHORIZATION_CODE", value_to_set=code, dotenv_path=DOTENV_PATH
         )
 
         print("code 저장 완료")
+        print()
 
     if ACCESS_TOKEN is None:
         print("access token 발급 요청 중..")
         access_token = retrieve_access_token()
         set_key(
             key_to_set="ACCESS_TOKEN",
             value_to_set=access_token,
```

### Comparing `local-first-tistory-0.0.1/src/category.py` & `local-first-tistory-0.0.2/src/category.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from dotenv import load_dotenv
 import os
 import configparser
 from pathlib import Path
-from .env import MARKDOWNS, CATEGORIES_TOML
+from .env import MARKDOWNS, CATEGORIES_TOML, DOTENV_PATH
 
 category_data = configparser.ConfigParser()
 
 
 def save_category(category):
     category_name = category["label"].lower()
     id = category["id"]
@@ -18,33 +18,37 @@
 
 
 def category_mkdir(category_name):
     Path(os.path.join(MARKDOWNS, category_name)).mkdir(parents=True, exist_ok=True)
 
 
 def load_categories_from_tistory():
-    load_dotenv(override=True)
+    load_dotenv(dotenv_path=DOTENV_PATH, override=True)
     BLOG_NAME = os.getenv("BLOG_NAME")
     ACCESS_TOKEN = os.getenv("ACCESS_TOKEN")
 
     category_params = {
         "access_token": ACCESS_TOKEN,
         "blogName": BLOG_NAME,
         "output": "json",
     }
 
     print(
         f"카테고리를 서버에 요청하는 중입니다.. \
             결과는 {CATEGORIES_TOML}에 저장됩니다."
     )
     category_url = "https://www.tistory.com/apis/category/list"
-    category_from_tistory = requests.get(category_url, params=category_params).json()
+    category_from_tistory = requests.get(category_url, params=category_params).json()[
+        "tistory"
+    ]["item"]["categories"]
 
     category_data.read(CATEGORIES_TOML)
-    for category in category_from_tistory["tistory"]["item"]["categories"]:
+    category_data.clear()
+
+    for category in category_from_tistory:
         category_name = save_category(category)
         category_mkdir(category_name)
     print("카테고리 저장 및 디렉토리 생성 완료.")
 
 
 if __name__ == "__main__":
     load_categories_from_tistory()
```

### Comparing `local-first-tistory-0.0.1/src/env.py` & `local-first-tistory-0.0.2/src/env.py`

 * *Files identical despite different names*

### Comparing `local-first-tistory-0.0.1/src/image.py` & `local-first-tistory-0.0.2/src/image.py`

 * *Files identical despite different names*

### Comparing `local-first-tistory-0.0.1/src/markdown.py` & `local-first-tistory-0.0.2/src/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pyright: reportGeneralTypeIssues = false
+
 import requests
 import markdown
 from dotenv import load_dotenv
 import os
 import hashlib
 import configparser
 from .env import CATEGORIES_TOML, DOTENV_PATH, METADATA_TOML, MARKDOWNS
@@ -21,15 +23,15 @@
 default_params = {
     "access_token": ACCESS_TOKEN,
     "blogName": BLOG_NAME,
     "output": "json",
 }
 
 
-def convert_metadata(meta, path: str, category: str) -> dict:
+def convert_metadata(meta, path: str, category_id: str) -> dict:
     metadata = {}
 
     # title
     if "title" in meta:
         metadata["title"] = meta["title"][0]
     elif "t" in meta:
         metadata["title"] = meta["t"][0]
@@ -70,23 +72,20 @@
                 metadata["acceptComment"] = "1"
             elif accept_comment in ("no", "n", "false", "f", "거부", "0"):
                 metadata["acceptComment"] = "0"
             else:
                 metadata["acceptComment"] = "1"
 
     # category
-    if category != "markdowns":
-        metadata["category"] = category_data[category]["id"]
-    else:
-        metadata["category"] = "0"
+    metadata["category"] = category_id
 
     return metadata
 
 
-def convert_md_to_html_and_metadata(path: str, category: str):
+def convert_md_to_html_and_metadata(path: str, category_id: str):
     raw_md = open(path, "r").read()
     sha1 = hashlib.sha1(raw_md.encode()).hexdigest()
     # Convert it to HTML metadata and content
     extension_configs = {
         "markdown_link_attr_modifier": {
             "new_tab": "on",
             "no_referrer": "external_only",
@@ -101,15 +100,15 @@
             "mdx_truly_sane_lists",
             "markdown_link_attr_modifier",
         ],
         extension_configs=extension_configs,
     )
     html_content = md.convert(raw_md)
     meta = md.Meta
-    metadata = convert_metadata(meta, path, category)
+    metadata = convert_metadata(meta, path, category_id)
     return html_content, sha1, metadata
 
 
 def modify_post_in_tistory(post_id: str, metadata: dict, content: str):
     modify_url = "https://www.tistory.com/apis/post/modify"
     modify_params = {
         "postId": post_id,
@@ -133,58 +132,65 @@
     write_result = requests.post(write_url, data=write_params).json()
     post_id = write_result["tistory"]["postId"]
     post_url = write_result["tistory"]["url"]
     print(f"티스토리에 새로운 포스트 등록 완료. url = {post_url}")
     return post_id
 
 
-def save_metadata(md_metadata, md_rel_path: str, post_id: str, sha1: str):
-    md_metadata[md_rel_path] = {}
-    md_metadata[md_rel_path]["post_id"] = post_id
-    md_metadata[md_rel_path]["sha1"] = sha1
+def save_metadata(md_metadata, file: str, post_id: str, sha1: str, category_id: str):
+    md_metadata[file] = {}
+    md_metadata[file]["post_id"] = post_id
+    md_metadata[file]["category_id"] = category_id
+    md_metadata[file]["sha1"] = sha1
+
     md_metadata.write(open(METADATA_TOML, "w"))
 
 
-def modify_metadata(md_metadata, md_rel_path: str, sha1: str):
-    md_metadata[md_rel_path]["sha1"] = sha1
+def modify_metadata(md_metadata, file: str, sha1: str):
+    md_metadata[file]["sha1"] = sha1
     md_metadata.write(open(METADATA_TOML, "w"))
 
 
 # Traverse the directory and save or modify post
 def traverse_markdowns():
     uploaded_count = 0
     modified_count = 0
     for subdir, _, files in os.walk(MARKDOWNS):
         for file in files:
             if not file.endswith(".md"):
                 continue
 
             md_rel_path = os.path.join(subdir, file)
             category = subdir.removeprefix(MARKDOWNS + "/")
+            category_id = category_data.get(category, "id", fallback="0")
+
             html_content, sha1, metadata = convert_md_to_html_and_metadata(
-                md_rel_path, category
+                md_rel_path, category_id
             )
 
             md_metadata.read(METADATA_TOML)
             # If saved metadata does not exist, upload the post
-            if md_rel_path not in md_metadata:
+            if file not in md_metadata:
                 post_id = save_post_to_tistory(metadata, html_content)
-                save_metadata(md_metadata, md_rel_path, post_id, sha1)
+                save_metadata(md_metadata, file, post_id, sha1, category_id)
                 uploaded_count += 1
 
             # If sha1 is different from saved sha1, modify the post
-            elif sha1 != md_metadata[md_rel_path]["sha1"]:
-                post_id = md_metadata[md_rel_path]["post_id"]
+            elif (
+                sha1 != md_metadata[file]["sha1"]
+                and category_id == md_metadata[file]["category_id"]
+            ):
+                post_id = md_metadata[file]["post_id"]
                 print(
                     f"post_id:{post_id} 변경 감지. \
                         티스토리 서버로 수정 요청 중.."
                 )
 
                 modify_post_in_tistory(post_id, metadata, html_content)
-                modify_metadata(md_metadata, md_rel_path, sha1)
+                modify_metadata(md_metadata, file, sha1)
                 modified_count += 1
 
     print(
         f"""{uploaded_count} 개의 포스트 업로드 완료.
 {modified_count} 개의 포스트 수정 완료.
 스크립트를 종료합니다."""
     )
```

### Comparing `local-first-tistory-0.0.1/src/tistory.py` & `local-first-tistory-0.0.2/src/tistory.py`

 * *Files identical despite different names*

