# Comparing `tmp/tidy_tweet-1.0.0a2.tar.gz` & `tmp/tidy_tweet-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy_tweet-1.0.0a2.tar", last modified: Fri Jun  2 05:18:21 2023, max compression
+gzip compressed data, was "tidy_tweet-1.0.0a3.tar", last modified: Thu Jun 22 05:47:43 2023, max compression
```

## Comparing `tidy_tweet-1.0.0a2.tar` & `tidy_tweet-1.0.0a3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.278354 tidy_tweet-1.0.0a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.270354 tidy_tweet-1.0.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-02 05:18:21.278354 tidy_tweet-1.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/docs/data_model.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/docs/data_model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/docs/schema.md
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/generate_schema_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-02 05:18:21.278354 tidy_tweet-1.0.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.270354 tidy_tweet-1.0.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/src/tidy_tweet/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/tweet_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/src/tidy_tweet/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 05:18:21.000000 tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:18:21.274354 tidy_tweet-1.0.0a2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/tests/data/ObservatoryTeam.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-02 05:18:04.000000 tidy_tweet-1.0.0a2/tests/test_overall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.245827 tidy_tweet-1.0.0a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-22 05:47:43.253827 tidy_tweet-1.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/docs/data_model.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    39299 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/docs/data_model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/docs/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/generate_schema_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-22 05:47:43.253827 tidy_tweet-1.0.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.245827 tidy_tweet-1.0.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/src/tidy_tweet/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/tweet_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/src/tidy_tweet/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 05:47:43.000000 tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:47:43.249827 tidy_tweet-1.0.0a3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   586918 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/tests/data/ObservatoryTeam.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-22 05:47:24.000000 tidy_tweet-1.0.0a3/tests/test_overall.py
```

### Comparing `tidy_tweet-1.0.0a2/.github/workflows/pypi_publish.yml` & `tidy_tweet-1.0.0a3/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/.github/workflows/tests.yml` & `tidy_tweet-1.0.0a3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/LICENSE` & `tidy_tweet-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/PKG-INFO` & `tidy_tweet-1.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy_tweet
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a2/README.md` & `tidy_tweet-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/contributing.md` & `tidy_tweet-1.0.0a3/contributing.md`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/docs/data_model.drawio` & `tidy_tweet-1.0.0a3/docs/data_model.drawio`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/docs/data_model.svg` & `tidy_tweet-1.0.0a3/docs/data_model.svg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/docs/schema.md` & `tidy_tweet-1.0.0a3/docs/schema.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         text url
         text preview_image_url
         integer height
         integer width
         text type
         integer duration_ms
         integer view_count
-        string alt_text
+        text alt_text
         text media_key PK
     }
     "user_by_page" {
         text name
         text profile_image_url
         text id PK
         text created_at
@@ -89,15 +89,15 @@
         integer directly_collected
     }
     "results_page" {
         integer id PK
         text file_name
         text oldest_id
         text newest_id
-        text result_count
+        integer result_count
         text inserted_at
         text twarc_version
         text tidy_tweet_version
         text retrieved_at
         text request_url
         text additional_metadata
     }
@@ -183,15 +183,15 @@
 - **url** (text)
 - **preview_image_url** (text)
 - **height** (integer)
 - **width** (integer)
 - **type** (text)
 - **duration_ms** (integer)
 - **view_count** (integer)
-- **alt_text** (string)
+- **alt_text** (text)
 - **media_key** (text primary key)
 
 
 Table **user_by_page**:
 
 - **name** (text)
 - **profile_image_url** (text)
@@ -201,15 +201,15 @@
 - **description** (text)
 - **location** (text)
 - **pinned_tweet_id** (text)
 - **verified** (integer): boolean
 - **url** (text)
 - **username** (text)
 - **page_id** (integer primary key references results_page (id))
-- **source_file** (text references results_page (filename))
+- **source_file** (text references results_page (file_name))
 
 primary key 
 
 
 Table **tweet_by_page**:
 
 - **id** (text primary key )
@@ -226,27 +226,27 @@
 - **lang** (text)
 - **source** (text)
 - **possibly_sensitive** (integer): boolean
 - **like_count** (integer)
 - **quote_count** (integer)
 - **reply_count** (integer)
 - **retweet_count** (integer)
-- **source_file** (text references results_page (filename))
+- **source_file** (text references results_page (file_name))
 - **directly_collected** (integer): boolean
 
 primary key 
 
 
 Table **results_page**:
 
 - **id** (integer primary key)
 - **file_name** (text)
 - **oldest_id** (text): oldest tweet id in page
 - **newest_id** (text): newest tweet id in page
-- **result_count** (text): count given in API response
+- **result_count** (integer): count given in API response
 - **inserted_at** (text default current_timestamp)
 - **twarc_version** (text)
 - **tidy_tweet_version** (text)
 - **retrieved_at** (text): time response from twitter was recorded
 - **request_url** (text)
 - **additional_metadata** (text): extra metadata from twarc and twitter
```

### Comparing `tidy_tweet-1.0.0a2/generate_schema_diagram.py` & `tidy_tweet-1.0.0a3/generate_schema_diagram.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/setup.cfg` & `tidy_tweet-1.0.0a3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/src/tidy_tweet/__main__.py` & `tidy_tweet-1.0.0a3/src/tidy_tweet/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/src/tidy_tweet/database.py` & `tidy_tweet-1.0.0a3/src/tidy_tweet/database.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/src/tidy_tweet/processing.py` & `tidy_tweet-1.0.0a3/src/tidy_tweet/processing.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/src/tidy_tweet/tweet_mapping.py` & `tidy_tweet-1.0.0a3/src/tidy_tweet/tweet_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "be fetched. If running tidy_tweet from source, try installing package in "
         "editable mode."
     )
 
 
 # --- SCHEMA VERSION ---
 # Update this every time the database schema is changed!
-SCHEMA_VERSION = "2022-05-22"
+SCHEMA_VERSION = "2023-06-22"
 
 
 sql_by_table: Dict[str, Dict[str, str]] = {}
 sql_views: Dict[str, str] = {}
 
 # --- Entities tables ---
 # URLs
@@ -254,15 +254,15 @@
     url text,
     preview_image_url text,
     height integer,
     width integer,
     type text,
     duration_ms integer,
     view_count integer,
-    alt_text string,
+    alt_text text,
     media_key text primary key
 )
     """,
     "insert": """
 insert or replace into media (
     media_key, url, type,
     height, width, preview_image_url, alt_text,
@@ -316,15 +316,15 @@
     description text,
     location text,
     pinned_tweet_id text,
     verified integer, -- boolean
     url text,
     username text,
     page_id integer references results_page (id),
-    source_file text references results_page (filename),
+    source_file text references results_page (file_name),
     primary key (id, page_id)
 )
     """,
     "insert": """
 insert or ignore into user_by_page (
     id, username, name, url,
     profile_image_url, description,
@@ -345,15 +345,15 @@
     """,
 }
 sql_views[
     "user"
 ] = """
 create view user as
 select
-    id, username, name, url,
+    user_by_page.id, username, name, url,
     profile_image_url, description,
     created_at,
     protected, verified,
     location,
     pinned_tweet_id,
     max(retrieved_at) as retrieved_at
 from user_by_page
@@ -413,15 +413,15 @@
     lang text,
     source text,
     possibly_sensitive integer, -- boolean
     like_count integer,
     quote_count integer,
     reply_count integer,
     retweet_count integer,
-    source_file text references results_page (filename),
+    source_file text references results_page (file_name),
     directly_collected integer, -- boolean
     primary key (id, page_id)
 )
     """,
     "insert": """
 insert or ignore into tweet_by_page (
     id, author_id,
@@ -534,15 +534,15 @@
 sql_by_table["results_page"] = {
     "create": """
 create table results_page (
     id integer primary key,
     file_name text,
     oldest_id text,  -- oldest tweet id in page
     newest_id text,  -- newest tweet id in page
-    result_count text,  -- count given in API response
+    result_count integer,  -- count given in API response
     inserted_at text default current_timestamp,
     twarc_version text,
     tidy_tweet_version text,
     retrieved_at text, -- time response from twitter was recorded
     request_url text,
     additional_metadata text -- extra metadata from twarc and twitter
 )
@@ -605,24 +605,24 @@
 
     if len(page_metadata_json) > 0:
         extras["twarc"] = page_metadata_json
 
     if len(twarc_metadata_json) > 0:
         extras["twarc"] = twarc_metadata_json
 
-    metadata["additional_metadata"] = dumps(extras)
+    metadata["additional_metadata"] = dumps(extras, ensure_ascii=False)
 
     return metadata
 
 
 # --- Validation ---
 
 # We have both create and assert statements for all tables
 for table_sql in sql_by_table.values():
     assert {"create", "insert"} <= table_sql.keys()
 
 
 # --- Convenience lists ---
 
 create_table_statements = [
-    clean_sql_statement(tbl["create"]) for tbl in sql_by_table.values()
+    clean_sql_statement(tbl["create"] + " strict") for tbl in sql_by_table.values()
 ]
```

### Comparing `tidy_tweet-1.0.0a2/src/tidy_tweet/utilities.py` & `tidy_tweet-1.0.0a3/src/tidy_tweet/utilities.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/PKG-INFO` & `tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy-tweet
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Tidies Twitter json collected with Twarc into relational tables
 Home-page: https://github.com/QUT-Digital-Observatory/tidy_tweet
 Author: QUT Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/tidy_tweet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy_tweet-1.0.0a2/src/tidy_tweet.egg-info/SOURCES.txt` & `tidy_tweet-1.0.0a3/src/tidy_tweet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/tests/data/ObservatoryTeam.jsonl` & `tidy_tweet-1.0.0a3/tests/data/ObservatoryTeam.jsonl`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/tests/test_cli.py` & `tidy_tweet-1.0.0a3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy_tweet-1.0.0a2/tests/test_overall.py` & `tidy_tweet-1.0.0a3/tests/test_overall.py`

 * *Files identical despite different names*

