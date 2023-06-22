# Comparing `tmp/ozgursozluk-0.7.3.tar.gz` & `tmp/ozgursozluk-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozgursozluk-0.7.3.tar", last modified: Fri Jun 16 09:40:05 2023, max compression
+gzip compressed data, was "ozgursozluk-0.7.5.tar", last modified: Thu Jun 22 08:09:39 2023, max compression
```

## Comparing `ozgursozluk-0.7.3.tar` & `ozgursozluk-0.7.5.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:05.816853 ozgursozluk-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:05.808853 ozgursozluk-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:05.812853 ozgursozluk-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-16 09:40:05.816853 ozgursozluk-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/TODO.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/gunicorn.conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:05.812853 ozgursozluk-0.7.3/ozgursozluk/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:05.816853 ozgursozluk-0.7.3/ozgursozluk/static/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/amoled.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/dark.css
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/discord.css
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/gruvbox.css
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/gruvboxlight.css
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/light.css
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/startpage.css
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/static/violet.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:05.816853 ozgursozluk-0.7.3/ozgursozluk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/author.html
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/debe.html
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/entry.html
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/paginate.html
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/templates/topic.html
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/ozgursozluk/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:40:05.812853 ozgursozluk-0.7.3/ozgursozluk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-16 09:40:05.000000 ozgursozluk-0.7.3/ozgursozluk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-16 09:40:05.000000 ozgursozluk-0.7.3/ozgursozluk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:40:05.000000 ozgursozluk-0.7.3/ozgursozluk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-16 09:40:05.000000 ozgursozluk-0.7.3/ozgursozluk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 09:40:05.000000 ozgursozluk-0.7.3/ozgursozluk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:40:05.816853 ozgursozluk-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-16 09:39:44.000000 ozgursozluk-0.7.3/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:09:39.330588 ozgursozluk-0.7.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:09:39.326588 ozgursozluk-0.7.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:09:39.326588 ozgursozluk-0.7.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-22 08:09:39.330588 ozgursozluk-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:09:39.326588 ozgursozluk-0.7.5/ozgursozluk/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:09:39.330588 ozgursozluk-0.7.5/ozgursozluk/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/amoled.css
+-rw-r--r--   0 runner    (1001) docker     (123)    46128 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/btc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/discord.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/gruvbox.css
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/gruvboxlight.css
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/light.css
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/startpage.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/violet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    57143 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/static/xmr.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:09:39.330588 ozgursozluk-0.7.5/ozgursozluk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/author.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/debe.html
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/donate.html
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/entry.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/paginate.html
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/templates/topic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/ozgursozluk/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:09:39.326588 ozgursozluk-0.7.5/ozgursozluk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-22 08:09:39.000000 ozgursozluk-0.7.5/ozgursozluk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-22 08:09:39.000000 ozgursozluk-0.7.5/ozgursozluk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:09:39.000000 ozgursozluk-0.7.5/ozgursozluk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-22 08:09:39.000000 ozgursozluk-0.7.5/ozgursozluk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 08:09:39.000000 ozgursozluk-0.7.5/ozgursozluk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 08:09:39.330588 ozgursozluk-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-22 08:09:23.000000 ozgursozluk-0.7.5/tests.py
```

### Comparing `ozgursozluk-0.7.3/.github/workflows/publish.yml` & `ozgursozluk-0.7.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.7.3/.github/workflows/tests.yml` & `ozgursozluk-0.7.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.7.3/.gitignore` & `ozgursozluk-0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.7.3/PKG-INFO` & `ozgursozluk-0.7.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozgursozluk
-Version: 0.7.3
+Version: 0.7.5
 Summary: A free and open source alternative ekşi sözlük front-end
 Author-email: beucismis <beucismis@tutamail.com>
 License:             DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                             Version 2, December 2004
         
          Copyright (C) 2023 beucismis <beucismis@tutamail.com>
```

### Comparing `ozgursozluk-0.7.3/README.md` & `ozgursozluk-0.7.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,97 @@
 <img src="https://github.com/beucismis/ozgursozluk/assets/40023234/4f145030-2376-4d2d-acb0-39167212793f" width="380">
 
 ![](https://img.shields.io/badge/python-3.8%2B-blue)
+![](https://img.shields.io/pypi/v/ozgursozluk)
+![](https://img.shields.io/pypi/dm/ozgursozluk)
 ![](https://img.shields.io/badge/code%20style-black-black)
-![](https://img.shields.io/github/v/release/beucismis/ozgursozluk)
 ![](https://img.shields.io/github/actions/workflow/status/beucismis/ozgursozluk/tests.yml?label=tests)
+![](https://img.shields.io/github/actions/workflow/status/beucismis/ozgursozluk/publish.yml?label=publish)
 
-A free and open source alternative ekşi sözlük front-end. Does not use the API, only scrapes the web. Official instance: https://ozgursozluk.freedns.rocks
+A free and open source alternative ekşi sözlük front-end. Does not use the API, only scrapes the web.
+
+Official instance: https://ozgursozluk.freedns.rocks</br>
+Donate: https://ozgursozluk.freedns.rocks/donate
 
 ## Features
+
 - No JavaScript
 - Docker support
 - Topic searching
 - Viewing topic, entry and author
 - Gündem and debe page support
 - Optional displaying author nickname
 - 8 different theme support
 - Self-hosted, ad-free, simple and fast
 - Responsive support for small screens
 
-## Installing and Running
-Clone the repository:
+## Installation
+
+Install from the `pip`:
 ```
-git clone https://github.com/beucismis/ozgursozluk
-cd ozgursozluk/
+pip3 install ozgursozluk
 ```
 
-Normal running:
+Install from the repo:
 ```
-pip3 install -r requirements.txt
-gunicorn
+pip3 install git+https://github.com/beucismis/ozgursozluk.git
 ```
-Deploy using a different port: `gunicorn --bind 127.0.0.1:3131`
 
-Running with Docker:
+Updating:
+```
+pip3 install ozgursozluk --upgrade
+```
+
+## Deploying
+
 ```
+flask --app ozgursozluk run
+# or
+gunicorn ozgursozluk:app
+```
+
+Alternatively, with Docker:
+```
+git clone https://github.com/beucismis/ozgursozluk
+cd ozgursozluk
 docker build -t ozgursozluk .
-docker run -p 3131:80 ozgursozluk
+docker run -p 8080:80 ozgursozluk
 ```
 
 See also, https://github.com/beucismis/ozgursozluk/wiki/Main
 
-### Environment Variables
+## Environment Variables
 
 | Key | Type | Default Value |
 | - | - | - |
 | `SECRET_KEY` | `str` |  |
+| `FLASK_RUN_HOST` | `str` | `127.0.0.1` |
+| `FLASK_RUN_PORT` | `str` | `5000` |
 | `EKSI_SOZLUK_BASE_URL` | `str` | `https://eksisozluk1923.com` |
 
 ## Redirection
+
 [Redirector](https://einaregilsson.com/redirector) browser extension is recommended for use. Configuration:
 ```
 Description: ekşi sözlük to özgürsözlük
 Example URL: https://eksisozluk.com/linux--32084
 Include pattern: ^https?://(?:.*\.)*(?<!link.)eksisozluk(.*)\.com(/.*)?$
 Redirect to: https://ozgursozluk.freedns.rocks$1
 Pattern type: Regular Expression
 Example result: https://ozgursozluk.freedns.rocks/linux--32084
 ```
 
 ## Preview
+
 <table>
   <tbody>
     <tr>
       <td><img src="https://github.com/beucismis/ozgursozluk/assets/40023234/620558a0-f518-42c8-9b2a-cc67067f63f3"></td>
       <td><img src="https://github.com/beucismis/ozgursozluk/assets/40023234/2c4d2fc7-d5dc-4a20-bc09-03b8ea36caad"></td>
       <td><img src="https://github.com/beucismis/ozgursozluk/assets/40023234/8dfd442c-cddb-41cd-ac3c-d95f0436e2e5"></td>
     </tr>
   </tbody>
 </table>
 
 ## License
+
 This project is licensed under WTFPL for details, check [LICENSE](LICENSE) file.
```

#### html2text {}

```diff
@@ -1,29 +1,34 @@
 [https://github.com/beucismis/ozgursozluk/assets/40023234/4f145030-2376-4d2d-
 acb0-39167212793f] ![](https://img.shields.io/badge/python-3.8%2B-blue) ![]
-(https://img.shields.io/badge/code%20style-black-black) ![](https://
-img.shields.io/github/v/release/beucismis/ozgursozluk) ![](https://
-img.shields.io/github/actions/workflow/status/beucismis/ozgursozluk/
-tests.yml?label=tests) A free and open source alternative ekÅi sÃ¶zlÃ¼k front-
-end. Does not use the API, only scrapes the web. Official instance: https://
-ozgursozluk.freedns.rocks ## Features - No JavaScript - Docker support - Topic
-searching - Viewing topic, entry and author - GÃ¼ndem and debe page support -
-Optional displaying author nickname - 8 different theme support - Self-hosted,
-ad-free, simple and fast - Responsive support for small screens ## Installing
-and Running Clone the repository: ``` git clone https://github.com/beucismis/
-ozgursozluk cd ozgursozluk/ ``` Normal running: ``` pip3 install -
-r requirements.txt gunicorn ``` Deploy using a different port: `gunicorn --bind
-127.0.0.1:3131` Running with Docker: ``` docker build -t ozgursozluk . docker
-run -p 3131:80 ozgursozluk ``` See also, https://github.com/beucismis/
-ozgursozluk/wiki/Main ### Environment Variables | Key | Type | Default Value |
-| - | - | - | | `SECRET_KEY` | `str` | | | `EKSI_SOZLUK_BASE_URL` | `str` |
-`https://eksisozluk1923.com` | ## Redirection [Redirector](https://
-einaregilsson.com/redirector) browser extension is recommended for use.
-Configuration: ``` Description: ekÅi sÃ¶zlÃ¼k to Ã¶zgÃ¼rsÃ¶zlÃ¼k Example URL:
-https://eksisozluk.com/linux--32084 Include pattern: ^https?://(?:.*\.)*(?
+(https://img.shields.io/pypi/v/ozgursozluk) ![](https://img.shields.io/pypi/dm/
+ozgursozluk) ![](https://img.shields.io/badge/code%20style-black-black) ![]
+(https://img.shields.io/github/actions/workflow/status/beucismis/ozgursozluk/
+tests.yml?label=tests) ![](https://img.shields.io/github/actions/workflow/
+status/beucismis/ozgursozluk/publish.yml?label=publish) A free and open source
+alternative ekÅi sÃ¶zlÃ¼k front-end. Does not use the API, only scrapes the
+web. Official instance: https://ozgursozluk.freedns.rocks Donate: https://
+ozgursozluk.freedns.rocks/donate ## Features - No JavaScript - Docker support -
+Topic searching - Viewing topic, entry and author - GÃ¼ndem and debe page
+support - Optional displaying author nickname - 8 different theme support -
+Self-hosted, ad-free, simple and fast - Responsive support for small screens ##
+Installation Install from the `pip`: ``` pip3 install ozgursozluk ``` Install
+from the repo: ``` pip3 install git+https://github.com/beucismis/
+ozgursozluk.git ``` Updating: ``` pip3 install ozgursozluk --upgrade ``` ##
+Deploying ``` flask --app ozgursozluk run # or gunicorn ozgursozluk:app ```
+Alternatively, with Docker: ``` git clone https://github.com/beucismis/
+ozgursozluk cd ozgursozluk docker build -t ozgursozluk . docker run -p 8080:80
+ozgursozluk ``` See also, https://github.com/beucismis/ozgursozluk/wiki/Main ##
+Environment Variables | Key | Type | Default Value | | - | - | - | |
+`SECRET_KEY` | `str` | | | `FLASK_RUN_HOST` | `str` | `127.0.0.1` | |
+`FLASK_RUN_PORT` | `str` | `5000` | | `EKSI_SOZLUK_BASE_URL` | `str` | `https:/
+/eksisozluk1923.com` | ## Redirection [Redirector](https://einaregilsson.com/
+redirector) browser extension is recommended for use. Configuration: ```
+Description: ekÅi sÃ¶zlÃ¼k to Ã¶zgÃ¼rsÃ¶zlÃ¼k Example URL: https://
+eksisozluk.com/linux--32084 Include pattern: ^https?://(?:.*\.)*(?
 )eksisozluk(.*)\.com(/.*)?$ Redirect to: https://ozgursozluk.freedns.rocks$1
 Pattern type: Regular Expression Example result: https://
 ozgursozluk.freedns.rocks/linux--32084 ``` ## Preview
 [https://github.com/      [https://github.com/      [https://github.com/
 beucismis/ozgursozluk/    beucismis/ozgursozluk/    beucismis/ozgursozluk/
 assets/40023234/620558a0- assets/40023234/2c4d2fc7- assets/40023234/8dfd442c-
 f518-42c8-9b2a-           d5dc-4a20-bc09-           cddb-41cd-ac3c-
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/api.py` & `ozgursozluk-0.7.5/ozgursozluk/scraper.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,94 +2,97 @@
 
 import requests
 from flask import abort
 from bs4 import BeautifulSoup
 from fake_useragent import UserAgent
 
 from ozgursozluk.configs import EKSI_SOZLUK_BASE_URL
-from ozgursozluk.models import Entry, EntryTopic, Topic, Author, Gundem, Debe
+from ozgursozluk.models import Entry, EntryTopic, Topic, Author, Gundem, Debe, SearchResult
 
 
 class EksiSozluk:
     def __init__(
         self,
         base_url: str = EKSI_SOZLUK_BASE_URL,
         headers: Optional[dict] = None,
     ) -> None:
         self.base_url = base_url
         self.session = requests.Session()
         headers = headers or {"User-Agent": UserAgent().random}
         self.session.headers.update(headers)
 
-    def request(self, method: str, path: str = "/", **params) -> BeautifulSoup:
+    def request(self, method: str, path: str = "/", params: dict = {}) -> BeautifulSoup:
         """Make a request."""
 
         response = self.session.request(
             method,
-            f"{self.base_url}/{path}",
+            f"{self.base_url}{path}",
             params=params,
         )
 
         if response.status_code != 200:
             abort(response.status_code)
 
         return BeautifulSoup(response.content, "html.parser")
 
     def entrys(self, response: BeautifulSoup) -> Iterator[Entry]:
-        """Get entrys for the given topic."""
+        """Get entrys with given topic."""
 
         entry_items = response.find_all("li", id="entry-item")
 
         for entry in entry_items:
             yield Entry(
                 int(entry.attrs["data-id"]),
                 entry.find("div", class_="content").text,
                 entry.find("div", class_="content"),
                 entry.find("a", class_="entry-author").text,
                 entry.find("a", class_="entry-date permalink", href=True).text,
                 int(entry.attrs["data-favorite-count"]),
             )
 
-    def search_topic(self, query: str) -> Topic:
-        """Search topic for the given query."""
+    def search_topic(self, keywords: str) -> Iterator[SearchResult]:
+        """Return titles that match the query parameters."""
 
-        response = self.request("GET", q=query)
-        h1 = response.find("h1", id="title")
-        pager = response.find("div", class_="pager")
+        payload = {
+            "SearchForm.Keywords": keywords,
+            "SearchForm.NiceOnly": True,
+            "SearchForm.SortOrder": "Count",
+        }
+        response = self.request("GET", "/basliklar/ara", payload)
+        topic_list = response.find("ul", class_="topic-list").find_all("a", href=True)
 
-        return Topic(
-            int(h1.attrs["data-id"]),
-            h1.attrs["data-title"],
-            h1.find("a")["href"][1:],
-            self.entrys(response),
-            int(pager.attrs["data-pagecount"]) if pager else 0,
-        )
+        for topic in topic_list:
+            yield SearchResult(
+                topic.contents[0],
+                topic["href"].split("?")[0],
+                None if len(topic.contents) < 2 else topic.contents[1].text,
+            )
 
     def get_topic(self, path: str, page: int = 1, a: Optional[str] = None) -> Topic:
-        """Get topic for the given path."""
+        """Get topic with given path."""
 
         if a is None:
-            response = self.request("GET", f"/{path}", p=page)
+            response = self.request("GET", f"/{path}", {"p": page})
         else:
-            response = self.request("GET", f"/{path}", p=page, a=a)
+            response = self.request("GET", f"/{path}", {"p": page, "a": a})
 
         h1 = response.find("h1", id="title")
         pager = response.find("div", class_="pager")
 
         return Topic(
             int(h1.attrs["data-id"]),
             h1.attrs["data-title"],
             h1.find("a")["href"][1:],
             self.entrys(response),
             int(pager.attrs["data-pagecount"]) if pager else 0,
             a == "nice",
         )
 
     def get_entry(self, id: int) -> EntryTopic:
-        """Get entry for the given ID."""
+        """Get entry with given ID."""
 
         response = self.request("GET", f"/entry/{id}")
         h1 = response.find("h1", id="title")
         entry = response.find("li", id="entry-item")
 
         return EntryTopic(
             int(entry.attrs["data-id"]),
@@ -100,15 +103,15 @@
             int(entry.attrs["data-favorite-count"]),
             int(h1.attrs["data-id"]),
             h1.attrs["data-title"],
             h1.find("a")["href"][1:],
         )
 
     def get_author(self, nickname: str) -> Author:
-        """Get author for the give nickname."""
+        """Get author with given nickname."""
 
         response = self.request("GET", f"/biri/{nickname}")
         muted = response.find("p", class_="muted")
         biography = response.find("div", id="profile-biography")
 
         return Author(
             nickname,
@@ -119,32 +122,32 @@
             muted.text if muted else None,
             biography.find("div").text if biography else None,
             biography.find("div") if biography else None,
         )
 
     def get_gundem(self, page: int = 1) -> Iterator[Gundem]:
         """
-        Get gündem page.
+        Return latest news titles.
         https://eksisozluk.com/basliklar/gundem
         """
 
-        response = self.request("GET", "/basliklar/gundem", p=page)
+        response = self.request("GET", "/basliklar/gundem", {"p": page})
         topic_list = response.find("ul", class_="topic-list").find_all("a", href=True)
 
         for topic in topic_list:
             yield Gundem(
                 topic.contents[0],
                 topic["href"].split("?")[0][1:],
                 topic.has_attr("class"),
                 None if len(topic.contents) < 2 else topic.contents[1].text,
             )
 
     def get_debe(self) -> Iterator[Debe]:
         """
-        Get debe page.
+        Return highly rated titles from yesterday.
         https://eksisozluk.com/debe
         """
 
         response = self.request("GET", "/debe")
         topic_list = response.find("ul", class_="topic-list").find_all("a", href=True)
 
         for topic in topic_list:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/configs.py` & `ozgursozluk-0.7.5/ozgursozluk/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from os import environ
 from typing import Final
 
 
 SECRET_KEY: Final = environ.get("OZGURSOZLUK_SECRET_KEY", "")
-EKSI_SOZLUK_BASE_URL: Final = environ.get("EKSI_SOZLUK_BASE_URL", "https://eksisozluk1923.com")
+EKSI_SOZLUK_BASE_URL: Final = environ.get(
+    "EKSI_SOZLUK_BASE_URL", "https://eksisozluk1923.com"
+)
 
 DEFAULT_THEME: Final = "light"
 DEFAULT_DISPLAY_PINNED_TOPICS: Final = "true"
 DEFAULT_DISPLAY_ENTRY_FAVORITE_COUNT: Final = "false"
 DEFAULT_DISPLAY_ENTRY_AUTHOR: Final = "false"
 DEFAULT_DISPLAY_ENTRY_DATETIME: Final = "true"
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/models.py` & `ozgursozluk-0.7.5/ozgursozluk/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,7 +49,14 @@
     entry_count: Union[str, None] = None
 
 
 @dataclass
 class Debe:
     id: int
     title: str
+
+
+@dataclass
+class SearchResult:
+    title: str
+    path: str
+    entry_count: Union[str, None] = None
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/static/favicon.png` & `ozgursozluk-0.7.5/ozgursozluk/static/favicon.png`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.7.3/ozgursozluk/static/style.css` & `ozgursozluk-0.7.5/ozgursozluk/static/style.css`

 * *Files 5% similar despite different names*

```diff
@@ -114,15 +114,25 @@
 
 .topic {
     width: 100%;
     margin: 0 auto;
     max-width: 900px;
 }
 
-.topic > .entry {
+.entry_wrapper {
+    gap: 1rem;
+    display: grid;
+    grid-template-columns: repeat(2, minmax(0, 1fr));
+}
+
+.entry_wrapper .entry {
+    margin: 0;
+}
+
+.entry {
     display: block;
     padding: 0.5rem;
     margin: 1rem 0 1rem 0;
     text-decoration: none;
     background-color: var(--entry-bg);
 }
 
@@ -176,24 +186,32 @@
 .settings {
     width: 100%;
     margin: 0 auto;
     max-width: 600px;
     padding-top: 1rem;
 }
 
-@media screen and (max-width: 992px) {
+@media screen and (max-width: 1000px) {
     nav {
         max-width: none;
     }
 
     main, nav {
         width: 100%;
     }
 
     nav, .title, .description {
         text-align: left;
     }
 
+    header a, .author a, .info a, .settings a {
+        font-size: larger;
+    }
+
     form input, form select {
         width: 30%;
     }
+
+    .entry_wrapper {
+        grid-template-columns: none;
+    }
 }
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/404.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/404.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/author.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/author.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/base.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/base.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 <!DOCTYPE html>
-<html>
+<html lang="tr">
     <head>
-        <meta charset="utf-8">
+        <meta charset="UTF-8">
+        <meta content="origin" name="referrer">
         {% block meta %}{% endblock %}
         <meta name="viewport" content="width=device-width, initial-scale=1">
         <link rel="icon" href="{{ url_for('static', filename='favicon.png') }}">
         <link rel="stylesheet" href="{{ url_for('static', filename='style.css') }}">
         {% if request.cookies.get('theme') is none %}
             <link rel="stylesheet" href="{{ url_for('static', filename='light.css') }}">
         {% else %}
             {% set filename = '{}.css'.format(request.cookies.get('theme')) %}
             <link rel="stylesheet" href="{{ url_for('static', filename=filename) }}">
         {% endif %}
-        <title>
-            {% block title %}{% endblock %}
-        </title>
+        <title>{% block title %}{% endblock %}</title>
     </head>
     <body>
         <header>
             <div>
 				<a href="{{ url_for('random') }}">random</a>
+                <a href="{{ url_for('donate') }}">donate</a>
                 <a href="{{ url_for('settings') }}">settings</a>
-                <a href="{{ source }}" target="_blank">source code</a>
+                <a href="{{ source_code }}" target="_blank">source code</a>
             </div>
         </header>
         <main>
             <h1 class="title">
                 <a href="/">
                     <span class="ozgur">özgür</span><span class="sozluk">sözlük</span>
                 </a>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
+
  {% block meta %}{% endblock %}
 
 
  {% if request.cookies.get('theme') is none %}
  {% else %} {% set filename = '{}.css'.format(request.cookies.get('theme')) %}
  {% endif %}
-random settings source_code
+random donate settings source_code
 
 ****** Ã¶zgÃ¼rsÃ¶zlÃ¼k ******
 {{ description }}
 {% block main %}{% endblock %}
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/debe.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/search.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 {% extends "base.html" %}
-{% block title %}debe - özgürsözlük{% endblock %}
+{% block title %}search - özgürsözlük{% endblock %}
 {% block meta %}
-    <meta name="title" content="debe - özgürsözlük">
-    <meta name="description" content="{{ description }}">
+    <meta name="title" content="search - özgürsözlük">
+    <meta name="description" content="{{ q }}">
 {% endblock %}
 {% block main %}
     <nav>{% include "navigation.html" %}</nav>
     <div class="topic">
         <div class="info">
-            <div>
-                <p>debe - <a href="/">gündem</a></p>
-            </div>
+            <div><p>search result: {{ q }}</p></div>
             <div></div>
         </div>
-        {% for entry in debe %}
-            <a class="entry" style="text-decoration: none;" href="{{ url_for('entry', id=entry.id) }}">
-                <div>
-                    <div>{{ entry.title }}</div>
+        {% for topic in search_result %}
+            <a href="{{ url_for('topic', path=topic.path) }}" class="entry">
+                <div style="display: flex; justify-content: space-between;">
+                    <div>{{ topic.title }}</div>
+                    <div>
+                        {% if topic.entry_count %}
+                            <small style="opacity: 0.5;">{{ topic.entry_count }}</small>
+                        {% endif %}
+                    </div>
                 </div>
             </a>
         {% endfor %}
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-{% extends "base.html" %} {% block title %}debe - Ã¶zgÃ¼rsÃ¶zlÃ¼k{% endblock %}
-{% block meta %}
+{% extends "base.html" %} {% block title %}search - Ã¶zgÃ¼rsÃ¶zlÃ¼k{% endblock
+%} {% block meta %}
 
  {% endblock %} {% block main %} {% include "navigation.html" %}
-debe - gÃ¼ndem
-{% for entry in debe %}
-{{_entry.title_}}
+search result: {{ q }}
+{% for topic in search_result %}
+{{_topic.title_}}
+{%_if_topic.entry_count_%}_{{_topic.entry_count_}}_{%_endif_%}
  {% endfor %}
 {% endblock %}
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/entry.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/entry.html`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,7 @@
                 </p>
             </div>
         </div>
         {% from "macros.html" import render_entry %}
         {{ render_entry(entry, False) }}
     </div>
 {% endblock %}
-
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/index.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/index.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/macros.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/macros.html`

 * *Files 7% similar despite different names*

```diff
@@ -35,19 +35,17 @@
     </div>
 </div>
 {% endmacro %}
 
 {% macro render_gundem(topic) %}
 <a href="{{ url_for('topic', path=topic.path, a='popular') }}" class="entry">
 	<div style="display: flex; justify-content: space-between;">
-		<div>
-			{{ topic.title }}
-		</div>
+		<div>{{ topic.title }}</div>
 		<div>
 			{% if topic.pinned %}<small style="opacity: 0.5;">pinned</small>{% endif %}
 			{% if topic.entry_count %}
 				<small style="opacity: 0.5;">{{ topic.entry_count }}</small>
 			{% endif %}
 		</div>
 	</div>
 </a>
-{% endmacro %}
+{% endmacro %}
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/paginate.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/paginate.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/settings.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/settings.html`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         <div style="text-align: center;">
             note: settings are saved in browser cookies, clearing your cookies will reset them.
             also this website does not have an official affiliation with eksisozluk.com.
             </br></br>
             v{{ version }}
             -
             last commit:
-            <a href="{{ source }}/commit/{{ last_commit }}" target="_blank">{{ last_commit[:8] }}</a>
+            <a href="{{ source_code }}/commit/{{ last_commit }}" target="_blank">{{ last_commit[:8] }}</a>
             -
             made with <3 on the <a href="{{ url_for('topic', path='thinkpad-t61--1883047') }}">t61</a>
             </br></br>
             contributors:
             {% for contributor in contributors %}
                 <a href="https://github.com/{{ contributor['username'] }}">{{ contributor['username'] }}</a>
                 ({{ contributor['total-commit'] }})
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/templates/topic.html` & `ozgursozluk-0.7.5/ozgursozluk/templates/topic.html`

 * *Files identical despite different names*

### Comparing `ozgursozluk-0.7.3/ozgursozluk/utils.py` & `ozgursozluk-0.7.5/ozgursozluk/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 
     return datetime.now() + timedelta(days=365)
 
 
 def last_commit() -> str:
     """Return the last commit ID."""
 
-    request = requests.get(
-        "https://api.github.com/repos/beucismis/ozgursozluk/commits"
-    )
+    request = requests.get("https://api.github.com/repos/beucismis/ozgursozluk/commits")
 
     return request.json()[0]["sha"]
 
 
 def contributors() -> list:
     """Get GitHub contributors."""
 
     request = requests.get(
         "https://api.github.com/repos/beucismis/ozgursozluk/contributors"
     )
 
     for contributor in request.json():
-        yield {"username": contributor["login"], "total-commit": contributor["contributions"]}
+        yield {
+            "username": contributor["login"],
+            "total-commit": contributor["contributions"],
+        }
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk/views.py` & `ozgursozluk-0.7.5/ozgursozluk/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from random import randint
 
 from flask import url_for, redirect, request, render_template
 
 import ozgursozluk
-from ozgursozluk.api import EksiSozluk
+from ozgursozluk.scraper import EksiSozluk
 from ozgursozluk.utils import last_commit, expires, contributors
 from ozgursozluk.configs import THEMES, DEFAULT_COOKIES
 
 
 es = EksiSozluk()
 
 
@@ -16,15 +16,15 @@
     """Return the gloabal template variables."""
 
     return dict(
         themes=THEMES,
         last_commit=last_commit(),
         contributors=contributors(),
         version=ozgursozluk.__version__,
-        source=ozgursozluk.__source__,
+        source_code=ozgursozluk.__source_code__,
         description=ozgursozluk.__description__,
     )
 
 
 @ozgursozluk.app.route("/", methods=["GET", "POST"])
 def index():
     """Index route."""
@@ -32,15 +32,15 @@
     q = request.args.get("q", default=None, type=str)
     p = request.args.get("p", default=1, type=int)
 
     if q is not None:
         return redirect(url_for("search", q=q))
 
     if request.method == "POST":
-        return redirect(url_for("search", q=request.form["q"]))
+        return redirect(url_for("search", q=request.form["q"] or None))
 
     gundem = es.get_gundem(p)
 
     return render_template("index.html", gundem=gundem, p=p)
 
 
 @ozgursozluk.app.route("/<path>")
@@ -70,24 +70,38 @@
 @ozgursozluk.app.route("/debe")
 def debe():
     """Debe route."""
 
     return render_template("debe.html", debe=es.get_debe())
 
 
-@ozgursozluk.app.route("/search/<q>")
-def search(q: str):
+@ozgursozluk.app.route("/search")
+def search():
     """Search route."""
 
-    return render_template("topic.html", topic=es.search_topic(q), p=1, a=None)
+    q = request.args.get("q", default=None, type=str)
+
+    if q is None or not bool(len(q)):
+        return render_template("404.html"), 404
+
+    return render_template("search.html", search_result=es.search_topic(q), q=q)
 
 
 @ozgursozluk.app.route("/random")
 def random():
-	return redirect(url_for("entry", id=randint(1, 500_000_000)))
+    """Random entry route."""
+
+    return redirect(url_for("entry", id=randint(1, 300_000_000)))
+
+
+@ozgursozluk.app.route("/donate")
+def donate():
+    """Donate route."""
+
+    return render_template("donate.html")
 
 
 @ozgursozluk.app.route("/settings", methods=["GET", "POST"])
 def settings():
     """Settings route."""
 
     if request.method == "POST":
@@ -106,10 +120,10 @@
             for cookie in DEFAULT_COOKIES
         },
     )
 
 
 @ozgursozluk.app.errorhandler(404)
 def page_not_found(error):
-    """Error handler."""
+    """Error handler route."""
 
     return render_template("404.html"), 404
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk.egg-info/PKG-INFO` & `ozgursozluk-0.7.5/ozgursozluk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozgursozluk
-Version: 0.7.3
+Version: 0.7.5
 Summary: A free and open source alternative ekşi sözlük front-end
 Author-email: beucismis <beucismis@tutamail.com>
 License:             DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                             Version 2, December 2004
         
          Copyright (C) 2023 beucismis <beucismis@tutamail.com>
```

### Comparing `ozgursozluk-0.7.3/ozgursozluk.egg-info/SOURCES.txt` & `ozgursozluk-0.7.5/ozgursozluk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 .gitignore
 Dockerfile
 LICENSE
 README.md
 TODO.md
-gunicorn.conf.py
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 tests.py
+.github/FUNDING.yml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 ozgursozluk/__init__.py
-ozgursozluk/api.py
 ozgursozluk/configs.py
 ozgursozluk/models.py
+ozgursozluk/scraper.py
 ozgursozluk/utils.py
 ozgursozluk/views.py
 ozgursozluk.egg-info/PKG-INFO
 ozgursozluk.egg-info/SOURCES.txt
 ozgursozluk.egg-info/dependency_links.txt
 ozgursozluk.egg-info/requires.txt
 ozgursozluk.egg-info/top_level.txt
 ozgursozluk/static/amoled.css
+ozgursozluk/static/btc.png
 ozgursozluk/static/dark.css
 ozgursozluk/static/discord.css
 ozgursozluk/static/favicon.png
 ozgursozluk/static/gruvbox.css
 ozgursozluk/static/gruvboxlight.css
 ozgursozluk/static/light.css
 ozgursozluk/static/startpage.css
 ozgursozluk/static/style.css
 ozgursozluk/static/violet.css
+ozgursozluk/static/xmr.png
 ozgursozluk/templates/404.html
 ozgursozluk/templates/author.html
 ozgursozluk/templates/base.html
 ozgursozluk/templates/debe.html
+ozgursozluk/templates/donate.html
 ozgursozluk/templates/entry.html
 ozgursozluk/templates/index.html
 ozgursozluk/templates/macros.html
 ozgursozluk/templates/navigation.html
 ozgursozluk/templates/paginate.html
+ozgursozluk/templates/search.html
 ozgursozluk/templates/settings.html
 ozgursozluk/templates/topic.html
```

### Comparing `ozgursozluk-0.7.3/pyproject.toml` & `ozgursozluk-0.7.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ozgursozluk"
-authors = [
-    {name = "beucismis", email = "beucismis@tutamail.com"},
-]
+authors = [{name = "beucismis", email = "beucismis@tutamail.com"}]
 description = "A free and open source alternative ekşi sözlük front-end"
 requires-python = ">=3.8"
 keywords = [
     "alternative", "flask", "front-end", "eksisozluk", "self-hosted",
     "beautifulsoup", "eksi", "sozluk", "debe", "gundem", "sukela",
 ]
 license = {file = "LICENSE"}
@@ -19,17 +17,15 @@
     "Framework :: Flask",
     "Programming Language :: Python",
 ]
 dynamic = ["version", "dependencies"]
 
 [tool.poetry]
 readme = "README.md"
-include = [
-    "ozgursozluk/static/*", "ozgursozluk/templates/*",
-]
+include = ["ozgursozluk/static/*", "ozgursozluk/templates/*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "ozgursozluk.__version__"}
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 Homepage = "https://github.com/beucismis/ozgursozluk"
```

### Comparing `ozgursozluk-0.7.3/tests.py` & `ozgursozluk-0.7.5/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 from ozgursozluk.api import EksiSozluk
 
 
 es = EksiSozluk()
-topic = es.search_topic("linux")
+topic = es.get_topic("linux--32084")
 entry = es.get_entry(1)
 
 
 class TestTopic(unittest.TestCase):
     def test_topic_id(self):
         self.assertEqual(topic.id, 32084)
```

