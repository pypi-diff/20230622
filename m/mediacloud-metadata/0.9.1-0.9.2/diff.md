# Comparing `tmp/mediacloud-metadata-0.9.1.tar.gz` & `tmp/mediacloud-metadata-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediacloud-metadata-0.9.1.tar", last modified: Sat Dec 24 19:03:55 2022, max compression
+gzip compressed data, was "mediacloud-metadata-0.9.2.tar", last modified: Mon Jan 23 21:17:34 2023, max compression
```

## Comparing `mediacloud-metadata-0.9.1.tar` & `mediacloud-metadata-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 r.bhargava   (502) staff       (20)        0 2022-12-24 19:03:55.968889 mediacloud-metadata-0.9.1/
--rw-r--r--   0 r.bhargava   (502) staff       (20)    10171 2022-03-08 14:30:45.000000 mediacloud-metadata-0.9.1/LICENSE
--rw-r--r--   0 r.bhargava   (502) staff       (20)     5736 2022-12-24 19:03:55.968758 mediacloud-metadata-0.9.1/PKG-INFO
--rw-r--r--   0 r.bhargava   (502) staff       (20)     5254 2022-12-24 19:03:24.000000 mediacloud-metadata-0.9.1/README.md
-drwxr-xr-x   0 r.bhargava   (502) staff       (20)        0 2022-12-24 19:03:55.967526 mediacloud-metadata-0.9.1/mcmetadata/
--rw-r--r--   0 r.bhargava   (502) staff       (20)     4776 2022-12-24 19:03:00.000000 mediacloud-metadata-0.9.1/mcmetadata/__init__.py
--rw-r--r--   0 r.bhargava   (502) staff       (20)    10560 2022-12-06 18:16:33.000000 mediacloud-metadata-0.9.1/mcmetadata/content.py
-drwxr-xr-x   0 r.bhargava   (502) staff       (20)        0 2022-12-24 19:03:55.967800 mediacloud-metadata-0.9.1/mcmetadata/data/
--rw-r--r--   0 r.bhargava   (502) staff       (20)      367 2022-08-12 15:11:23.000000 mediacloud-metadata-0.9.1/mcmetadata/data/domain-skip-list.txt
--rw-r--r--   0 r.bhargava   (502) staff       (20)      937 2022-08-29 16:27:08.000000 mediacloud-metadata-0.9.1/mcmetadata/dates.py
--rw-r--r--   0 r.bhargava   (502) staff       (20)      544 2022-12-06 14:58:12.000000 mediacloud-metadata-0.9.1/mcmetadata/exceptions.py
--rw-r--r--   0 r.bhargava   (502) staff       (20)     1242 2022-12-22 13:00:10.000000 mediacloud-metadata-0.9.1/mcmetadata/feeds.py
--rw-r--r--   0 r.bhargava   (502) staff       (20)     2755 2022-12-06 14:49:39.000000 mediacloud-metadata-0.9.1/mcmetadata/languages.py
--rw-r--r--   0 r.bhargava   (502) staff       (20)     1183 2022-04-25 14:52:02.000000 mediacloud-metadata-0.9.1/mcmetadata/text.py
--rw-r--r--   0 r.bhargava   (502) staff       (20)     5890 2022-12-06 18:16:58.000000 mediacloud-metadata-0.9.1/mcmetadata/titles.py
--rw-r--r--   0 r.bhargava   (502) staff       (20)    13755 2022-12-24 18:56:53.000000 mediacloud-metadata-0.9.1/mcmetadata/urls.py
--rw-r--r--   0 r.bhargava   (502) staff       (20)     7061 2022-07-31 16:34:54.000000 mediacloud-metadata-0.9.1/mcmetadata/urlshortners.py
--rw-r--r--   0 r.bhargava   (502) staff       (20)     1395 2022-12-06 18:22:31.000000 mediacloud-metadata-0.9.1/mcmetadata/webpages.py
-drwxr-xr-x   0 r.bhargava   (502) staff       (20)        0 2022-12-24 19:03:55.968572 mediacloud-metadata-0.9.1/mediacloud_metadata.egg-info/
--rw-r--r--   0 r.bhargava   (502) staff       (20)     5736 2022-12-24 19:03:55.000000 mediacloud-metadata-0.9.1/mediacloud_metadata.egg-info/PKG-INFO
--rw-r--r--   0 r.bhargava   (502) staff       (20)      535 2022-12-24 19:03:55.000000 mediacloud-metadata-0.9.1/mediacloud_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 r.bhargava   (502) staff       (20)        1 2022-12-24 19:03:55.000000 mediacloud-metadata-0.9.1/mediacloud_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 r.bhargava   (502) staff       (20)      255 2022-12-24 19:03:55.000000 mediacloud-metadata-0.9.1/mediacloud_metadata.egg-info/requires.txt
--rw-r--r--   0 r.bhargava   (502) staff       (20)       11 2022-12-24 19:03:55.000000 mediacloud-metadata-0.9.1/mediacloud_metadata.egg-info/top_level.txt
--rw-r--r--   0 r.bhargava   (502) staff       (20)      106 2022-03-07 20:54:47.000000 mediacloud-metadata-0.9.1/pyproject.toml
--rw-r--r--   0 r.bhargava   (502) staff       (20)       38 2022-12-24 19:03:55.968924 mediacloud-metadata-0.9.1/setup.cfg
--rw-r--r--   0 r.bhargava   (502) staff       (20)     1807 2022-12-06 18:20:06.000000 mediacloud-metadata-0.9.1/setup.py
+drwxr-xr-x   0 pgulley  (32314) grd      (10015)        0 2023-01-23 21:17:34.640032 mediacloud-metadata-0.9.2/
+-rw-r--r--   0 pgulley  (32314) grd      (10015)    10171 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/LICENSE
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     5795 2023-01-23 21:17:34.640032 mediacloud-metadata-0.9.2/PKG-INFO
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     5313 2023-01-23 21:00:38.000000 mediacloud-metadata-0.9.2/README.md
+drwxr-xr-x   0 pgulley  (32314) grd      (10015)        0 2023-01-23 21:17:34.628164 mediacloud-metadata-0.9.2/mcmetadata/
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     4776 2023-01-23 21:00:23.000000 mediacloud-metadata-0.9.2/mcmetadata/__init__.py
+-rw-r--r--   0 pgulley  (32314) grd      (10015)    10560 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/mcmetadata/content.py
+drwxr-xr-x   0 pgulley  (32314) grd      (10015)        0 2023-01-23 21:17:34.628164 mediacloud-metadata-0.9.2/mcmetadata/data/
+-rw-r--r--   0 pgulley  (32314) grd      (10015)      367 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/mcmetadata/data/domain-skip-list.txt
+-rw-r--r--   0 pgulley  (32314) grd      (10015)      937 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/mcmetadata/dates.py
+-rw-r--r--   0 pgulley  (32314) grd      (10015)      544 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/mcmetadata/exceptions.py
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     1242 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/mcmetadata/feeds.py
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     2755 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/mcmetadata/languages.py
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     1183 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/mcmetadata/text.py
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     5936 2023-01-23 20:58:24.000000 mediacloud-metadata-0.9.2/mcmetadata/titles.py
+-rw-r--r--   0 pgulley  (32314) grd      (10015)    13755 2023-01-23 20:58:18.000000 mediacloud-metadata-0.9.2/mcmetadata/urls.py
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     7061 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/mcmetadata/urlshortners.py
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     1395 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/mcmetadata/webpages.py
+drwxr-xr-x   0 pgulley  (32314) grd      (10015)        0 2023-01-23 21:17:34.636076 mediacloud-metadata-0.9.2/mediacloud_metadata.egg-info/
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     5795 2023-01-23 21:17:34.000000 mediacloud-metadata-0.9.2/mediacloud_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 pgulley  (32314) grd      (10015)      535 2023-01-23 21:17:34.000000 mediacloud-metadata-0.9.2/mediacloud_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 pgulley  (32314) grd      (10015)        1 2023-01-23 21:17:34.000000 mediacloud-metadata-0.9.2/mediacloud_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 pgulley  (32314) grd      (10015)      255 2023-01-23 21:17:34.000000 mediacloud-metadata-0.9.2/mediacloud_metadata.egg-info/requires.txt
+-rw-r--r--   0 pgulley  (32314) grd      (10015)       11 2023-01-23 21:17:34.000000 mediacloud-metadata-0.9.2/mediacloud_metadata.egg-info/top_level.txt
+-rw-r--r--   0 pgulley  (32314) grd      (10015)      106 2023-01-09 18:09:38.000000 mediacloud-metadata-0.9.2/pyproject.toml
+-rw-r--r--   0 pgulley  (32314) grd      (10015)       38 2023-01-23 21:17:34.640032 mediacloud-metadata-0.9.2/setup.cfg
+-rw-r--r--   0 pgulley  (32314) grd      (10015)     1922 2023-01-10 19:13:03.000000 mediacloud-metadata-0.9.2/setup.py
```

### Comparing `mediacloud-metadata-0.9.1/LICENSE` & `mediacloud-metadata-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/PKG-INFO` & `mediacloud-metadata-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacloud-metadata
-Version: 0.9.1
+Version: 0.9.2
 Summary: Media Cloud news article metadata extraction
 Home-page: http://mediacloud.org
 Maintainer: Rahul Bhargava
 Maintainer-email: rahul@mediacloud.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mediacloud/meta-extractor/issues
 Project-URL: Source, https://github.com/mediacloud/meta-extractor
@@ -59,15 +59,15 @@
 
 Distribution
 ------------
 
 This is setup to automatically publish new releases to PyPi via GitHub Actions:
 
 1. Run `pytest` to make sure all the test pass
-2. Update the version number in `mcextractor/__init__.py`
+2. Update the version number in `metadata-lib/__init__.py`
 3. Make a brief note in the version history section below about the changes
 4. Commit the changes
 5. Tag the commit with a semantic version number - 'v*.*.*'
 6. Push to repo to GitHub
 
 ### Manual Release
 
@@ -83,14 +83,15 @@
 This can be change with the use of '--use-cache=False' when running tests
 
 When adding new tests, re-run 'scripts/get-test-web-content.py' 
 
 Version History
 ---------------
 
+* __v0.9.2__: fixed a bug related to title regex matching
 * __v0.9.1__: better support for some non-US government domains
 * __v0.9.0__: adds `feeds.normalize_url` helper
 * __v0.8.2__: small fix to url parsing
 * __v0.8.1__: handle IP addresses in canonical_domain helper
 * __v0.8.0__: update dependencies, fix various edge-case bugs
 * __v0.7.9__: fix `include_other_metadata` processing, upgrade underlying libraries to latest, remove leading and 
               trailing whitespace from extracted text
```

### Comparing `mediacloud-metadata-0.9.1/README.md` & `mediacloud-metadata-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 Distribution
 ------------
 
 This is setup to automatically publish new releases to PyPi via GitHub Actions:
 
 1. Run `pytest` to make sure all the test pass
-2. Update the version number in `mcextractor/__init__.py`
+2. Update the version number in `metadata-lib/__init__.py`
 3. Make a brief note in the version history section below about the changes
 4. Commit the changes
 5. Tag the commit with a semantic version number - 'v*.*.*'
 6. Push to repo to GitHub
 
 ### Manual Release
 
@@ -68,14 +68,15 @@
 This can be change with the use of '--use-cache=False' when running tests
 
 When adding new tests, re-run 'scripts/get-test-web-content.py' 
 
 Version History
 ---------------
 
+* __v0.9.2__: fixed a bug related to title regex matching
 * __v0.9.1__: better support for some non-US government domains
 * __v0.9.0__: adds `feeds.normalize_url` helper
 * __v0.8.2__: small fix to url parsing
 * __v0.8.1__: handle IP addresses in canonical_domain helper
 * __v0.8.0__: update dependencies, fix various edge-case bugs
 * __v0.7.9__: fix `include_other_metadata` processing, upgrade underlying libraries to latest, remove leading and 
               trailing whitespace from extracted text
```

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/__init__.py` & `mediacloud-metadata-0.9.2/mcmetadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from . import webpages
 from . import content
 from . import urls
 from . import titles
 from . import languages
 from . import dates
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 logger = logging.getLogger(__name__)
 
 # Publication dates more than this many days in the future will be ignored (because they are probably bad guesses)
 MAX_FUTURE_PUB_DATE = 90
 
 STAT_NAMES = ['total', 'fetch', 'url', 'pub_date', 'content', 'title', 'language']
```

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/content.py` & `mediacloud-metadata-0.9.2/mcmetadata/content.py`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/dates.py` & `mediacloud-metadata-0.9.2/mcmetadata/dates.py`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/exceptions.py` & `mediacloud-metadata-0.9.2/mcmetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/feeds.py` & `mediacloud-metadata-0.9.2/mcmetadata/feeds.py`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/languages.py` & `mediacloud-metadata-0.9.2/mcmetadata/languages.py`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/text.py` & `mediacloud-metadata-0.9.2/mcmetadata/text.py`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/titles.py` & `mediacloud-metadata-0.9.2/mcmetadata/titles.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 title_tag_pattern = re.compile(r"<title(?: [^>]*)?>(.*?)</title>", re.S | re.I)
 
 h1_tag_pattern = re.compile(r"<h1(?: [^>]*)?>(.*?)</h1>", re.S | re.I)
 
 whitespace_pattern = re.compile(r'\s+')
 
-home_pattern = re.compile(r'^\W*home\W*', re.I)
+home_pattern = re.compile(r'^\W+home\W+', re.I)
 
 
 def from_html(html_text: str, fallback_title: str = None, trim_to_length: int = 0) -> Optional[str]:
     """
     Parse the content for tags that might indicate the story's title. Tuned for online news webpages.
     src: https://github.com/mediacloud/backend/blob/master/apps/common/src/python/mediawords/util/parse_html.py#L160
     Arguments:
@@ -88,15 +88,15 @@
             else:  # probably one or more suffixes
                 title = title_parts[0]
 
     # if a single h1 on page, and it is subset of found title, go with that (to eliminate post-fixed titles in meta tags)
     match = h1_tag_pattern.search(html_text)
     if match and len(match.groups()) == 1:
         h1_title = unescape(text.strip_tags(match.group(1))).strip()
-        if h1_title in title.strip():
+        if (len(h1_title) > SHORT_TITLE_THRESHOLD) and (h1_title in title.strip()):
             title = h1_title
 
     # optionally trim to a max length
     if trim_to_length > 0:
         title = title[0:trim_to_length]
 
     # strip again here because there might be dangling spaces from prefix/suffix cleaning
```

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/urls.py` & `mediacloud-metadata-0.9.2/mcmetadata/urls.py`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/urlshortners.py` & `mediacloud-metadata-0.9.2/mcmetadata/urlshortners.py`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/mcmetadata/webpages.py` & `mediacloud-metadata-0.9.2/mcmetadata/webpages.py`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/mediacloud_metadata.egg-info/PKG-INFO` & `mediacloud-metadata-0.9.2/mediacloud_metadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacloud-metadata
-Version: 0.9.1
+Version: 0.9.2
 Summary: Media Cloud news article metadata extraction
 Home-page: http://mediacloud.org
 Maintainer: Rahul Bhargava
 Maintainer-email: rahul@mediacloud.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mediacloud/meta-extractor/issues
 Project-URL: Source, https://github.com/mediacloud/meta-extractor
@@ -59,15 +59,15 @@
 
 Distribution
 ------------
 
 This is setup to automatically publish new releases to PyPi via GitHub Actions:
 
 1. Run `pytest` to make sure all the test pass
-2. Update the version number in `mcextractor/__init__.py`
+2. Update the version number in `metadata-lib/__init__.py`
 3. Make a brief note in the version history section below about the changes
 4. Commit the changes
 5. Tag the commit with a semantic version number - 'v*.*.*'
 6. Push to repo to GitHub
 
 ### Manual Release
 
@@ -83,14 +83,15 @@
 This can be change with the use of '--use-cache=False' when running tests
 
 When adding new tests, re-run 'scripts/get-test-web-content.py' 
 
 Version History
 ---------------
 
+* __v0.9.2__: fixed a bug related to title regex matching
 * __v0.9.1__: better support for some non-US government domains
 * __v0.9.0__: adds `feeds.normalize_url` helper
 * __v0.8.2__: small fix to url parsing
 * __v0.8.1__: handle IP addresses in canonical_domain helper
 * __v0.8.0__: update dependencies, fix various edge-case bugs
 * __v0.7.9__: fix `include_other_metadata` processing, upgrade underlying libraries to latest, remove leading and 
               trailing whitespace from extracted text
```

### Comparing `mediacloud-metadata-0.9.1/mediacloud_metadata.egg-info/SOURCES.txt` & `mediacloud-metadata-0.9.2/mediacloud_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mediacloud-metadata-0.9.1/setup.py` & `mediacloud-metadata-0.9.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     "py3langid==0.2.*",
     # various content extractors we try to use
     "newspaper3k==0.2.*", "goose3==3.1.*", "BeautifulSoup4==4.11.*", "readability-lxml==0.8.*", "trafilatura==1.4.*",
     "boilerpy3==1.0.*",
     # support
     "requests",         # leave un-versioned so dependencies can sort of which version is best
     "cchardet==2.1.*",  # BeautifulSoup4 speedup
-    "surt==0.3.1"
+    "surt==0.3.1",
+    #"charset-normalizer<3" # requests have not yet updated to support newer charset-normalizer, so freeze at 2.x
 ]
 
 with open('mcmetadata/__init__.py', 'r') as fd:
     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE).group(1)
 
 # add README.md to distribution
 this_directory = os.path.abspath(os.path.dirname(__file__))
```

