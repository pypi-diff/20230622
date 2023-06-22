# Comparing `tmp/maryam-2.5.1.post3.tar.gz` & `tmp/maryam-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maryam-2.5.1.post3.tar", last modified: Sat Mar  4 06:58:31 2023, max compression
+gzip compressed data, was "maryam-2.5.2.tar", last modified: Thu Jun 22 09:46:46 2023, max compression
```

## Comparing `maryam-2.5.1.post3.tar` & `maryam-2.5.2.tar`

### file list

```diff
@@ -1,205 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.493601 maryam-2.5.1.post3/
--rw-r--r--   0 root         (0) root         (0)    35147 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3188 2023-03-04 06:58:31.493601 maryam-2.5.1.post3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2480 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.469603 maryam-2.5.1.post3/bin/
--rw-r--r--   0 root         (0) root         (0)      119 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/bin/maryam
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.469603 maryam-2.5.1.post3/maryam/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1781 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.469603 maryam-2.5.1.post3/maryam/core/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      103 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/basedir.py
--rwxr-xr-x   0 root         (0) root         (0)    25144 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/core.py
--rwxr-xr-x   0 root         (0) root         (0)    14486 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/initial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.469603 maryam-2.5.1.post3/maryam/core/util/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.473603 maryam-2.5.1.post3/maryam/core/util/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/activesearch.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/baidu.py
--rw-r--r--   0 root         (0) root         (0)     5039 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/bing.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/bing_images.py
--rw-r--r--   0 root         (0) root         (0)     3030 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/carrot2.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/dogpile.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/duckduckgo.py
--rw-r--r--   0 root         (0) root         (0)     2746 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/gigablast.py
--rw-r--r--   0 root         (0) root         (0)     6609 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/google.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/google_images.py
--rw-r--r--   0 root         (0) root         (0)     3603 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/metacrawler.py
--rw-r--r--   0 root         (0) root         (0)     3461 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/millionshort.py
--rw-r--r--   0 root         (0) root         (0)     3427 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/qwant.py
--rw-r--r--   0 root         (0) root         (0)     3177 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/qwant_images.py
--rw-r--r--   0 root         (0) root         (0)     2955 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/searx.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/startpage.py
--rw-r--r--   0 root         (0) root         (0)     3722 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/yahoo.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/engines/yandex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.473603 maryam-2.5.1.post3/maryam/core/util/footprint/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/footprint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7471 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/footprint/cms_identify.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/footprint/lang_identify.py
--rw-r--r--   0 root         (0) root         (0)     2380 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/footprint/os_identify.py
--rw-r--r--   0 root         (0) root         (0)    45321 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/footprint/waf_identify.py
--rw-r--r--   0 root         (0) root         (0)     5455 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/footprint/wapps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.473603 maryam-2.5.1.post3/maryam/core/util/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3392 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/helpers/keywords.py
--rw-r--r--   0 root         (0) root         (0)     9946 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/helpers/page_parse.py
--rw-r--r--   0 root         (0) root         (0)     4983 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/helpers/rand_uagent.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/helpers/reglib.py
--rw-r--r--   0 root         (0) root         (0)     3410 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/helpers/urlib.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/helpers/web_scrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.477603 maryam-2.5.1.post3/maryam/core/util/iris/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/chart.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/cluster.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/meta_search_util.py
--rw-r--r--   0 root         (0) root         (0)     1355 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/plotlyutil.py
--rw-r--r--   0 root         (0) root         (0)     8046 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/retriever.py
--rw-r--r--   0 root         (0) root         (0)     2427 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/safe_searcher.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/tf_histogram.py
--rw-r--r--   0 root         (0) root         (0)     7429 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/topic.py
--rw-r--r--   0 root         (0) root         (0)     1739 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/iris/word_cloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.477603 maryam-2.5.1.post3/maryam/core/util/osint/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/ahmia.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/bing_mobile_view.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/darksearch.py
--rw-r--r--   0 root         (0) root         (0)     1896 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/exalead.py
--rw-r--r--   0 root         (0) root         (0)     2544 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/hunter.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/keyserver.py
--rw-r--r--   0 root         (0) root         (0)     2599 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/netcraft.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/numverify.py
--rw-r--r--   0 root         (0) root         (0)     2019 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/onionland.py
--rw-r--r--   0 root         (0) root         (0)     2798 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/reddit.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/tweet_search.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/urlscan.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/osint/virustotal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.481602 maryam-2.5.1.post3/maryam/core/util/search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/arxiv.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/ask.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/core_ac.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/creativecommons.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/crt.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/dictionary.py
--rw-r--r--   0 root         (0) root         (0)     1875 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/discord.py
--rw-r--r--   0 root         (0) root         (0)     8393 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/instagram.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/openstreetmap.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/pastebin.py
--rw-r--r--   0 root         (0) root         (0)     1901 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/photon.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/piratebay.py
--rw-r--r--   0 root         (0) root         (0)     2370 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/pubmed.py
--rw-r--r--   0 root         (0) root         (0)     3028 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/reddit_pushshift.py
--rw-r--r--   0 root         (0) root         (0)     5218 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/sanctionsearch.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/scholar.py
--rw-r--r--   0 root         (0) root         (0)     2527 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/sepiasearch.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/wikileaks.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/wikipedia.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/worldcat.py
--rw-r--r--   0 root         (0) root         (0)     3978 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/util/search/zlibrary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.481602 maryam-2.5.1.post3/maryam/core/web/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/core/web/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.481602 maryam-2.5.1.post3/maryam/data/
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/data/blacklist.txt
--rw-r--r--   0 root         (0) root         (0)     4782 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/data/dnsnames.txt
--rw-r--r--   0 root         (0) root         (0)      936 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/data/stopwords.csv
--rw-r--r--   0 root         (0) root         (0)    10201 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/data/tlds.txt
--rw-r--r--   0 root         (0) root         (0)    58532 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/data/username_checker.json
--rw-r--r--   0 root         (0) root         (0)   406174 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/data/wapps.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.481602 maryam-2.5.1.post3/maryam/modules/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.485602 maryam-2.5.1.post3/maryam/modules/footprint/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/footprint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3723 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/footprint/crawl_pages.py
--rw-r--r--   0 root         (0) root         (0)     4954 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/footprint/dnsbrute.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/footprint/entry_points.py
--rw-r--r--   0 root         (0) root         (0)     6351 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/footprint/filebrute.py
--rw-r--r--   0 root         (0) root         (0)    16954 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/footprint/interest_files.py
--rw-r--r--   0 root         (0) root         (0)     3266 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/footprint/tldbrute.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/footprint/wapps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.485602 maryam-2.5.1.post3/maryam/modules/iris/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/iris/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1502 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/iris/cluster.py
--rwxr-xr-x   0 root         (0) root         (0)     2527 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/iris/iris.py
--rwxr-xr-x   0 root         (0) root         (0)     1871 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/iris/iris_cluster.py
--rwxr-xr-x   0 root         (0) root         (0)     3088 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/iris/sentiment.py
--rwxr-xr-x   0 root         (0) root         (0)     2844 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/iris/topicmodeling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.489602 maryam-2.5.1.post3/maryam/modules/osint/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/article_search.py
--rw-r--r--   0 root         (0) root         (0)     4910 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/bing_mobile_view.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/cloud_storage.py
--rw-r--r--   0 root         (0) root         (0)     2575 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/crawler.py
--rw-r--r--   0 root         (0) root         (0)     4112 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/cve_search.py
--rw-r--r--   0 root         (0) root         (0)     9928 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/dark_web_crawler.py
--rw-r--r--   0 root         (0) root         (0)    12326 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/dns_search.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/docs_search.py
--rw-r--r--   0 root         (0) root         (0)     6388 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/domain_reputation.py
--rw-r--r--   0 root         (0) root         (0)     2073 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/email_pwned.py
--rw-r--r--   0 root         (0) root         (0)     3147 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/email_search.py
--rw-r--r--   0 root         (0) root         (0)     6371 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/famous_person.py
--rw-r--r--   0 root         (0) root         (0)     5453 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/github_leaks.py
--rw-r--r--   0 root         (0) root         (0)     2087 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/image_search.py
--rw-r--r--   0 root         (0) root         (0)     1503 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/onion_search.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/phone_number_search.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/reddit_search.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/social_nets.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/suggest.py
--rw-r--r--   0 root         (0) root         (0)     4526 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/tweet_search.py
--rw-r--r--   0 root         (0) root         (0)     3947 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/osint/username_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.493601 maryam-2.5.1.post3/maryam/modules/search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/activesearch.py
--rw-r--r--   0 root         (0) root         (0)     1366 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/arxiv.py
--rw-r--r--   0 root         (0) root         (0)     1503 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/bing.py
--rw-r--r--   0 root         (0) root         (0)     1234 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/carrot2.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/core_ac.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/creativecommons.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/crt.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/dictionary.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/discord.py
--rw-r--r--   0 root         (0) root         (0)     1371 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/dogpile.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/duckduckgo.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/facebook.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/gigablast.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/github.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/google.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/instagram.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/linkedin.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/metacrawler.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/millionshort.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/openstreetmap.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/pastebin.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/photon.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/piratebay.py
--rw-r--r--   0 root         (0) root         (0)     1407 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/pubmed.py
--rw-r--r--   0 root         (0) root         (0)     3256 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/quora.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/qwant.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/reddit.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/sanctionsearch.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/scholar.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/searx.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/sepiasearch.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/spotify.py
--rw-r--r--   0 root         (0) root         (0)     3499 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/stackoverflow.py
--rw-r--r--   0 root         (0) root         (0)     1503 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/startpage.py
--rw-r--r--   0 root         (0) root         (0)     4650 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/telegram.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/tiktok.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/trello.py
--rw-r--r--   0 root         (0) root         (0)     3042 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/twitter.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/wikileaks.py
--rw-r--r--   0 root         (0) root         (0)     2187 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/wikipedia.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/worldcat.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/yahoo.py
--rw-r--r--   0 root         (0) root         (0)     2887 2023-03-04 06:47:14.000000 maryam-2.5.1.post3/maryam/modules/search/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 06:58:31.469603 maryam-2.5.1.post3/maryam.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3188 2023-03-04 06:58:31.000000 maryam-2.5.1.post3/maryam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6287 2023-03-04 06:58:31.000000 maryam-2.5.1.post3/maryam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-04 06:58:31.000000 maryam-2.5.1.post3/maryam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      173 2023-03-04 06:58:31.000000 maryam-2.5.1.post3/maryam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-04 06:58:31.000000 maryam-2.5.1.post3/maryam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-04 06:58:31.493601 maryam-2.5.1.post3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1956 2023-03-04 06:58:17.000000 maryam-2.5.1.post3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/
+-rw-r--r--   0 root         (0) root         (0)    35147 2023-06-22 07:37:52.000000 maryam-2.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-22 07:37:52.000000 maryam-2.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-06-22 09:46:46.646822 maryam-2.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-06-22 09:37:46.000000 maryam-2.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.630821 maryam-2.5.2/bin/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-22 07:37:52.000000 maryam-2.5.2/bin/maryam
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.630821 maryam-2.5.2/maryam/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1781 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.634821 maryam-2.5.2/maryam/core/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      103 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/basedir.py
+-rwxr-xr-x   0 root         (0) root         (0)    25144 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/core.py
+-rwxr-xr-x   0 root         (0) root         (0)    14486 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/initial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.634821 maryam-2.5.2/maryam/core/util/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.634821 maryam-2.5.2/maryam/core/util/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/baidu.py
+-rw-r--r--   0 root         (0) root         (0)     5041 2023-06-22 08:17:28.000000 maryam-2.5.2/maryam/core/util/engines/bing.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/bing_images.py
+-rw-r--r--   0 root         (0) root         (0)     3030 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/carrot2.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/dogpile.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/duckduckgo.py
+-rw-r--r--   0 root         (0) root         (0)     6609 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/google.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/google_images.py
+-rw-r--r--   0 root         (0) root         (0)     3603 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/metacrawler.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/qwant.py
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/qwant_images.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/searx.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/startpage.py
+-rw-r--r--   0 root         (0) root         (0)     3722 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/yahoo.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/engines/yandex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.638821 maryam-2.5.2/maryam/core/util/footprint/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7471 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/cms_identify.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/lang_identify.py
+-rw-r--r--   0 root         (0) root         (0)     2380 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/os_identify.py
+-rw-r--r--   0 root         (0) root         (0)    45321 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/waf_identify.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/footprint/wapps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.638821 maryam-2.5.2/maryam/core/util/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-06-22 08:56:59.000000 maryam-2.5.2/maryam/core/util/helpers/keywords.py
+-rw-r--r--   0 root         (0) root         (0)     9945 2023-06-22 08:42:20.000000 maryam-2.5.2/maryam/core/util/helpers/page_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4983 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/rand_uagent.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/reglib.py
+-rw-r--r--   0 root         (0) root         (0)     3410 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/urlib.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/helpers/web_scrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.638821 maryam-2.5.2/maryam/core/util/iris/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/chart.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/meta_search_util.py
+-rw-r--r--   0 root         (0) root         (0)     8046 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/retriever.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-06-22 09:33:59.000000 maryam-2.5.2/maryam/core/util/iris/safe_searcher.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/tf_histogram.py
+-rw-r--r--   0 root         (0) root         (0)     7419 2023-06-22 07:42:30.000000 maryam-2.5.2/maryam/core/util/iris/topic.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/iris/word_cloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.642822 maryam-2.5.2/maryam/core/util/osint/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/ahmia.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/bing_mobile_view.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/darksearch.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/exalead.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/hunter.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/keyserver.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/netcraft.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/numverify.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/onionland.py
+-rw-r--r--   0 root         (0) root         (0)     2798 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/reddit.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/tweet_search.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/urlscan.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/osint/virustotal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/maryam/core/util/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/arxiv.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/ask.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-06-22 09:24:52.000000 maryam-2.5.2/maryam/core/util/search/core_ac.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-06-22 09:43:19.000000 maryam-2.5.2/maryam/core/util/search/crt.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/discord.py
+-rw-r--r--   0 root         (0) root         (0)     8393 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/instagram.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/openstreetmap.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/pastebin.py
+-rw-r--r--   0 root         (0) root         (0)     1901 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/photon.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/piratebay.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/pubmed.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/reddit_pushshift.py
+-rw-r--r--   0 root         (0) root         (0)     5218 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/sanctionsearch.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/scholar.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/sepiasearch.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/wikileaks.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/wikipedia.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/util/search/zlibrary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/maryam/core/web/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/core/web/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/maryam/data/
+-rw-r--r--   0 root         (0) root         (0)     4782 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/dnsnames.txt
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/stopwords.csv
+-rw-r--r--   0 root         (0) root         (0)    10201 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/tlds.txt
+-rw-r--r--   0 root         (0) root         (0)    58532 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/username_checker.json
+-rw-r--r--   0 root         (0) root         (0)   406174 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/data/wapps.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.646822 maryam-2.5.2/maryam/modules/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:37:52.000000 maryam-2.5.2/maryam/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 09:46:46.634821 maryam-2.5.2/maryam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 09:46:46.000000 maryam-2.5.2/maryam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 09:46:46.646822 maryam-2.5.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-06-22 09:38:14.000000 maryam-2.5.2/setup.py
```

### Comparing `maryam-2.5.1.post3/LICENSE` & `maryam-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/PKG-INFO` & `maryam-2.5.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maryam
-Version: 2.5.1.post3
+Version: 2.5.2
 Summary: OWASP Maryam is a modular/optional open-source framework based on OSINT and data gathering.
 Home-page: https://github.com/saeeddhqan/Maryam
 Author: Saeed Dehqan
 Author-email: saeed.dehghan@owasp.org
 License: GPL-V3
 Keywords: OWASP,OSINT,search-engine,social-networks,Maryam
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://app.travis-ci.com/saeeddhqan/Maryam.svg?branch=master)](https://app.travis-ci.com/github/saeeddhqan/Maryam)
-![Version 2.5.1](https://img.shields.io/badge/Version-2.5.1-green.svg)
+![Version 2.5.2](https://img.shields.io/badge/Version-2.5.1-green.svg)
 ![GPLv3 License](https://img.shields.io/badge/License-GPLv3-green.svg)
 ![Python 3.10.x](https://img.shields.io/badge/Python-3.10.x-green.svg)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4577/badge)](https://bestpractices.coreinfrastructure.org/projects/4577)
 
 # OWASP Maryam
 
 OWASP Maryam is a modular open-source framework based on OSINT and data gathering. It is designed to provide a robust environment to harvest data from open sources and search engines quickly and thoroughly.
@@ -33,14 +33,18 @@
  - FreeBSD
  - Darwin
  - OSX
 
 ```bash
 $ pip install maryam
 ```
+Alternatively, you can install the latest version with the following command (Recommended):
+```bash
+pip install git+https://github.com/saeeddhqan/maryam.git
+```
 
 # Usage
 
 ```bash
 # Using dns_search. --max means all of resources. --api shows the results as json.
 # .. -t means use multi-threading.
 maryam -e dns_search -d ibm.com -t 5 --max --api --form 
@@ -65,26 +69,26 @@
  - Iris: the first beta version
  - Added famous_person
  - Core speedup optimizations
  - Added setup.py
 
 
 
-
 # Contribution
 
 Contributes are welcome! Here is a start guide: [Development Guide](https://github.com/saeeddhqan/maryam/wiki/Development-Guide)
 You can add a new search engine to the util classes or use the current search engines to write a new module.
 The best help to write a new module is checking the current modules.
 
 # Roadmap
 
+ - Improving Iris page ranking
  - Write a complete metacrawler engine based on OSINT by using the current search engines
  - Add clustering algorithms: Done
- - Web User Interface
+ - Web user interface
 
 # Links
 ### [OWASP](https://owasp.org/www-project-maryam/)
 ### [Wiki](https://github.com/saeeddhqan/maryam/wiki)
 ### [Install](https://github.com/saeeddhqan/maryam/wiki#install)
 ### [Modules Guide](https://github.com/saeeddhqan/maryam/wiki/modules)
 ### [Development Guide](https://github.com/saeeddhqan/maryam/wiki/Development-Guide)
```

### Comparing `maryam-2.5.1.post3/README.md` & `maryam-2.5.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Build Status](https://app.travis-ci.com/saeeddhqan/Maryam.svg?branch=master)](https://app.travis-ci.com/github/saeeddhqan/Maryam)
-![Version 2.5.1](https://img.shields.io/badge/Version-2.5.1-green.svg)
+![Version 2.5.2](https://img.shields.io/badge/Version-2.5.1-green.svg)
 ![GPLv3 License](https://img.shields.io/badge/License-GPLv3-green.svg)
 ![Python 3.10.x](https://img.shields.io/badge/Python-3.10.x-green.svg)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4577/badge)](https://bestpractices.coreinfrastructure.org/projects/4577)
 
 # OWASP Maryam
 
 OWASP Maryam is a modular open-source framework based on OSINT and data gathering. It is designed to provide a robust environment to harvest data from open sources and search engines quickly and thoroughly.
@@ -15,14 +15,18 @@
  - FreeBSD
  - Darwin
  - OSX
 
 ```bash
 $ pip install maryam
 ```
+Alternatively, you can install the latest version with the following command (Recommended):
+```bash
+pip install git+https://github.com/saeeddhqan/maryam.git
+```
 
 # Usage
 
 ```bash
 # Using dns_search. --max means all of resources. --api shows the results as json.
 # .. -t means use multi-threading.
 maryam -e dns_search -d ibm.com -t 5 --max --api --form 
@@ -47,26 +51,26 @@
  - Iris: the first beta version
  - Added famous_person
  - Core speedup optimizations
  - Added setup.py
 
 
 
-
 # Contribution
 
 Contributes are welcome! Here is a start guide: [Development Guide](https://github.com/saeeddhqan/maryam/wiki/Development-Guide)
 You can add a new search engine to the util classes or use the current search engines to write a new module.
 The best help to write a new module is checking the current modules.
 
 # Roadmap
 
+ - Improving Iris page ranking
  - Write a complete metacrawler engine based on OSINT by using the current search engines
  - Add clustering algorithms: Done
- - Web User Interface
+ - Web user interface
 
 # Links
 ### [OWASP](https://owasp.org/www-project-maryam/)
 ### [Wiki](https://github.com/saeeddhqan/maryam/wiki)
 ### [Install](https://github.com/saeeddhqan/maryam/wiki#install)
 ### [Modules Guide](https://github.com/saeeddhqan/maryam/wiki/modules)
 ### [Development Guide](https://github.com/saeeddhqan/maryam/wiki/Development-Guide)
```

### Comparing `maryam-2.5.1.post3/maryam/__main__.py` & `maryam-2.5.2/maryam/__main__.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/core.py` & `maryam-2.5.2/maryam/core/core.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/initial.py` & `maryam-2.5.2/maryam/core/initial.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/activesearch.py` & `maryam-2.5.2/maryam/core/util/search/wikileaks.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,122 +12,87 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import re
-import html
-import urllib.parse
 
 class main:
 
-		def __init__(self, q, limit=15):
-			""" activesearchresults.com search engine
+	def __init__(self, q, limit=1):
+		""" wikileaks.org search engine
 
-					q     : Query for search
-					limit : Maximum result count
-			"""
-			self.framework = main.framework
-			self.q = q
-			self._max = limit
-			self._cookie = ''
-			self._rawhtml = ''
-			self._clubbedrows = []
-			self._rows = []
-			self._links = []
-			self._links_with_data = []
-			self._pageno = 0
-			self._soup = ''
-			self.active_search = 'www.activesearchresults.com'
-			
-
-		def run_crawl(self):
-			from bs4 import BeautifulSoup as bs
-
-			payload = { 
-				'wordsall': self.q,
-				'asrtech' : 'yes',
-				'perpage' : '100',
-				'adultfilter': '5',
-				'buttonall': ''
-				}
-			header = {
-				'Cookie' : f'{self._cookie}'
-				}
-
-			self.framework.verbose('Searching the activesearchresults domain...')
-
-			while True:
-				self._pageno += 1
-				url = f'https://{self.active_search}/searchsubmit.php?pageno={self._pageno}'
-
-				try:
-					req = self.framework.request(url=url,
-						method='POST',
-						data=payload,
-						headers=header
-						)
-				except:
-					self.framework.error('ConnectionError', 'util/activesearch', 'run_crawl')
-					self.framework.error('activesearchresults is missed!', 'util/activesearch', 'run_crawl')
-					return
-
-				self._rawhtml += req.text
-
-				if self._pageno==1:
-					max_pages = list(map(int, re.findall(
-						r"<a href='/searchsubmit.php\?pageno=(\d+[^']+)'>LAST",
-						req.text)))
-
-					if len(max_pages)==0:
-						return
-
-					else:
-						max_pages = max_pages[0]
+			q		: Query for search
+			limit	: Number of Pages
 
-					self._cookie = req.headers.get('Set-Cookie')
+		"""
 
-
-				if self._pageno > max_pages or self._pageno*100>self._max:
+		self.framework = main.framework
+		self.q = q
+		self.agent = 'Mozilla/5.0 (X11; Linux x86_64; rv:86.0) Gecko/20100101 Firefox/86.0'
+		self._pages = ''
+		self.limit = limit
+		self._links = []
+		self._results = []
+		self._links_with_data = []
+
+	def run_crawl(self):
+		from bs4 import BeautifulSoup as bs
+
+		max_attempts = 0
+		url = 'https://search.wikileaks.org/advanced'
+		params = {'query': self.q, 'include_external_sources': True, 'page': 1}
+		while True:
+			self.framework.verbose(f"[WIKILEAKS] Searching in {params['page']} page ....", end='\r')
+			try:
+				req = self.framework.request(
+					url=url,
+					params=params,
+					headers={'User-Agent': self.agent},
+					allow_redirects=True)
+			except Exception as e:
+				self.framework.error(f"ConnectionError: {e}", 'util/wikileaks', 'run_crawl')
+				max_attempts += 1
+				if max_attempts == self.limit:
+					self.framework.error('Wikileaks is missed!', 'util/wikileaks', 'run_crawl')
+					return
+			else:
+				self._pages += req.text
+				params['page'] += 1
+				if params['page'] >= self.limit:
 					break
 
-			self._soup = bs(self._rawhtml,'html.parser')
-			self._clubbedrows = self._soup.find_all('small')[5]
-			self._rows = self._clubbedrows.find_all('a')
-
-			for count, row in enumerate(self._rows):
-				if count>=self._max:
-					break
-				self._links.append(row['href'])
-				self._links_with_data.append({
-					'title': row['href'],
-					'link' : row.text
-					})
-
-		@property
-		def raw(self):
-			return self._rawhtml
-
-		@property
-		def rows(self):
-			return self._rows
-
-		@property
-		def links(self):
-			return self._links
-
-		@property
-		def dns(self):
-			return self.framework.page_parse(self._rawhtml).get_dns(self.q)
-
-		@property
-		def emails(self):
-			return self.framework.page_parse(self._rawhtml).get_emails(self.q)
-
-		@property
-		def docs(self):
-			return self.framework.page_parse(self._rawhtml).get_docs(self.q, self.links)
-
-		@property
-		def links_with_data(self):
-			return self._links_with_data 
+		soup = bs(self._pages, 'html.parser')
+		self._results = soup.find_all('div', class_='info')
+		for result in self._results:
+			self._links.append(result.find_all('a')[0]['href'])
+
+	@property
+	def pages(self):
+		return self._pages
+	
+	@property
+	def links(self):
+		return self._links
+
+	@property
+	def links_with_data(self):
+		for result in self._results:
+			self._links_with_data.append({
+				'title': result.find_all('a')[0].text,
+				'link': result.find_all('a')[0]['href']
+				})
+		
+		return self._links_with_data
+
+	@property
+	def dns(self):
+		return self.framework.page_parse(self._pages).get_dns(self.q)
+
+	@property
+	def emails(self):
+		return self.framework.page_parse(self._pages).get_emails(self.q)
+
+	@property
+	def docs(self):
+		return self.framework.page_parse(self._pages).get_docs(self.q, self.links)
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/baidu.py` & `maryam-2.5.2/maryam/core/util/engines/baidu.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/bing.py` & `maryam-2.5.2/maryam/core/util/engines/bing.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 				self._pages += req.text
 				if page == 1:
 					self._first_page += req.text
 				page += 1
 				payload['first'] = set_page(page)
 				if page >= self.limit or 'title="Next page"' not in req.text:
 					break
+	
 	# TODO: Finish it
 	@property
 	def bing_card(self):
 		card_xpath_name = {
 			'card': '//div[@class="lite-entcard-main"]',
 			'card_names': '//div[@class="l_ecrd_hero"]',
 			'card_description': './/span[@class="l_ecrd_txt_pln"]',
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/bing_images.py` & `maryam-2.5.2/maryam/core/util/engines/bing_images.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/carrot2.py` & `maryam-2.5.2/maryam/core/util/engines/carrot2.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/dogpile.py` & `maryam-2.5.2/maryam/core/util/engines/dogpile.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/duckduckgo.py` & `maryam-2.5.2/maryam/core/util/engines/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/gigablast.py` & `maryam-2.5.2/maryam/core/util/engines/searx.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,85 +10,100 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
-import re
-import json
 
 class main:
 
-		def __init__(self, q, limit=15):
-			""" Gigablast search engine
-					q     : Query to search
-					limit : Number of pages
-			"""
-			self.framework = main.framework
-			self.q = q
-			self._max = limit
-			self._json = ''
-			self._results = []
-
-		def run_crawl(self):
-			from bs4 import BeautifulSoup as bs
-
-			self.q = self.framework.urlib(self.q).quote
-			self.framework.verbose('Searching Gigablast...')
-			first_url = 'https://www.gigablast.com/search'
-			payload = {'q': self.q, 'format': 'json'}
-			try:
-				req = self.framework.request(url=first_url,
-						params=payload)
-			except:
-				self.framework.error('ConnectionError.', 'util/gigablast', 'run_crawl')
-				self.framework.error('Gigablast is missed!', 'util/gigablast', 'run_crawl')
-			else:
-				soup = bs(req.text,'html.parser')
-				script = soup.find('body')['onload']
-				params1 = re.findall(r"var uxrl='/search(.*?)'", script)[0]
-				params2 = re.findall(r"uxrl=uxrl\+'(.*?)'", script)[0]
-				final_url = first_url + params1 + params2
+	def __init__(self, q, limit=1):
+		""" searx search engine
+
+			q	: Query for search
+			limit	: Number of Pages
+
+		"""
+		self.framework = main.framework
+		self.q = q
+		self._pages = ''
+		self.limit = limit
+		self._links = []
+		self._json = {}
+		self.searx = ['https://searx.prvcy.eu/search', 'https://searx.xyz/search', 'https://searx.nevrlands.de/searx/search', 'https://searx.info/search']
+
+	def run_crawl(self):
+		page = 1
+		self._json['results'] = [] 
+		params = {'category_general': 1, 'q': self.q, 
+			  'pageno': 1, 'time_range': None, 
+			  'format': 'json'}
+		max_attempts = 0
+		for url in self.searx:
+			while True:
+				self.framework.verbose(f"[SEARX] Searching {url} page {params['pageno']}...", end='\r')
 				try:
-					req = self.framework.request(url=final_url)
-				except:
-					self.framework.error('ConnectionError.', 'util/gigablast', 'run_crawl')
-					self.framework.error('Gigablast is missed!', 'util/gigablast', 'run_crawl')
+					req = self.framework.request(
+						url=url,
+						params=params,
+						allow_redirects= True)
+				except Exception as e:
+					self.framework.error(f"ConnectionError: {e}", 'util/searx', 'run_crawl')
+					max_attempts += 1
+					if max_attempts == self.limit:
+						self.framework.error(f"Searx {url} is missed!", 'util/searx', 'run_crawl')
+						return
 				else:
-					self._json = req.json()['results']
-
-		@property
-		def json(self):
-			return self._json
-
-		@property
-		def raw(self):
-			return json.dumps(self._json)
-
-		@property
-		def dns(self):
-			return self.framework.page_parse(self.raw).get_dns(self.q)
-
-		@property
-		def emails(self):
-			return self.framework.page_parse(self.raw).get_emails(self.q)
-
-		@property
-		def docs(self):
-			return self.framework.page_parse(self.raw).get_docs(self.q)
-
-		@property
-		def results(self):
-			for count, result in enumerate(self._json):
-				if count >= self._max:
-					break
-				urlib = self.framework.urlib(result['url'])
-				a = urlib.unquote
-				cite = result.get('subTitle') or self.framework.meta_search_util().make_cite(a)
-				self._results.append({
-					't': result['title'],
-					'a': a,
-					'c': cite,
-					'd': result['sum'],
-					})
-			return self._results
+					self._pages += req.text
+					if req.status_code == 200 and 'results' in req.json():
+						self._json['results'] += req.json()['results']
+					else:
+						self.framework.error(f"Searx {url} is missed!", 'util/searcx', 'run_crawl')
+						break
+					if params['pageno'] >= self.limit:
+						return
+					params['pageno'] += 1
+
+	@property
+	def pages(self):
+		return self._pages
+
+	@property
+	def links(self):
+		for result in self._json['results']:
+			self._links.append(result['url'])
+		return self._links
+
+	@property
+	def results(self):
+		results = []
+		for result in self._json['results']:
+			if 'content' in result:
+				content = result['content']
+			else:
+				content = 'No description provided'
+			cite = self.framework.meta_search_util().make_cite(result['url'])
+			results.append({
+				't': result['title'],
+				'a': result['url'],
+				'c': cite,
+				'd': content
+			})
+
+		return results
+	
+	@property
+	def json(self):
+		return self._json
+
+	@property
+	def dns(self):
+		return self.framework.page_parse(self._pages).get_dns(self.q)
+
+	@property
+	def emails(self):
+		return self.framework.page_parse(self._pages).get_emails(self.q)
+	
+	@property
+	def docs(self):
+		return self.framework.page_parse(self._pages).get_docs(self.q)
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/google.py` & `maryam-2.5.2/maryam/core/util/engines/google.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/google_images.py` & `maryam-2.5.2/maryam/core/util/engines/google_images.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/metacrawler.py` & `maryam-2.5.2/maryam/core/util/engines/metacrawler.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/millionshort.py` & `maryam-2.5.2/maryam/core/util/engines/qwant.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,98 +11,99 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-import re
 
 class main:
 
 	def __init__(self, q, limit=2):
-		""" millionshort.com search engine
+		""" qwant.com search engine
 
-			q 		  : query for search
+			q 		  : Query for search
 			limit	  : Number of pages
 		"""
 		self.framework = main.framework
 		self.q = q
 		self.limit = limit
 		self._pages = ''
 		self._json = []
 		self._links = []
-		self._links_with_title = {}
-		self.millionshort = 'https://millionshort.com/api/search'
+		self._links_with_title = []
+		self.qwant = 'https://api.qwant.com/v3/search/web'
 
 	def run_crawl(self):
 		page = 1
-		set_page = lambda x: (x - 1) * 10 + 1
-		payload = {'keywords': self.q, 'remove': '0', 'offset': '0'}
-		headers = {
-			"Host": 'millionshort.com',
-			"User-Agent": 'Mozilla/5.0 (X11; Linux x86_64; rv:68.0) Gecko/20100101 Firefox/68.0',
-			"Accept": 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8',
-			"Accept-Language": 'en-US,en;q=0.5',
-			"Accept-Encoding": 'gzip, deflate, br',
-			"Connection": 'keep-alive',
-			"Cookie": 'connect.sid=s%3AVZd6oWjMPfegJTrCK6iVYs8p1S4q3Q-h.OC7iYFkDE5A2u6%2BsJkCa96q6ituwLnNDh0EjzEJhvNk',
-			"Upgrade-Insecure-Requests": '1',
-			"If-None-Match": 'W/"9fc-Kb1JjxDz/K4kA1S7nkbpkibKV94"',
-			"Cache-Control": 'max-age=0'
-		}
+		set_page = lambda x: (x-1)*10
+		payload = {'q': self.q, 'offset': set_page(page), 'count': '10', 'safesearch': '0', 'device': 'desktop', 'locale': 'en_us'}
 		while True:
-			self.framework.verbose(f"[MILLIONSHORT] Searching in {page} page...")
+			self.framework.verbose(f"[QWANT] Searching in {page+1} page...")
 			try:
-				req = self.framework.request(url=self.millionshort, params=payload, headers=headers)
+				req = self.framework.request(url=self.qwant, params=payload)
 			except Exception as e:
-				self.framework.error(f"ConnectionError {e}.", 'util/engines/millionshort', 'name_crawl')
-				self.framework.error('millionshort is missed!', 'util/engines/millionshort', 'name_crawl')
+				self.framework.error(f"ConnectionError {e}.", 'util/engines/qwant', 'util/engines/qwant', 'run_crawl')
+				self.framework.error('Qwant is missed!', 'util/engines/qwant', 'util/engines/qwant', 'run_crawl')
 				break
 			else:
-				if 'captcha' in req.json():
-					self.framework.error('CaptchaError', 'util/engines/millionshort', 'run_crawl')
-					self.framework.error('millionshort is missed!', 'util/engines/millionshort', 'name_crawl')
+				if req.status_code == 429 and "I can't let you do that..." in req.text and '<div class="error-code">' in req.text:
+					self.framework.error('429 Too Many Requests', 'util/engines/qwant', 'run_crawl')
 					return
-				self._json.append(req.json())
 				self._pages += req.text
-				if page == self.limit:
-					break
-				page += 1
-				payload['offset'] = set_page(page)
+				try:
+					self._json.append(req.json())
+				except Exception as e:
+					self.framework.error('429 Too Many Requests', 'util/engines/qwant', 'run_crawl')
+					return
+				else:
+					if req.json() == {'status': 'error', 'data': {'error_code': 22}}:
+						self.framework.error('429 Too Many Requests', 'util/engines/qwant', 'run_crawl')
+						return
+					else:
+						if page == self.limit:
+							break
+						page += 1
+						payload['offset'] = set_page(page)
 
 	@property
 	def pages(self):
 		return self._pages
 
 	@property
 	def json(self):
 		return self._json
 
 	@property
 	def links(self):
 		for page in self._json:
-			results = page.get('content', {}).get('webPages', {})
-			self._links.extend([x.get('displayUrl') for x in results])
+			results = page.get('data', {}).get('result', {}).get('items', {})
+			self._links.extend([x.get('url') for x in results])
 		return self._links
 
 	@property
 	def results(self):
 		results = []
 		for page in self._json:
-			items = page.get('content', {}).get('webPages', {})
+			items = page.get('data', {}).get('result', {})
+			if items:
+				items = items.get('items', {})
+				if items:
+					items = items.get('mainline', {})
 			for item in items:
-				a = item['displayUrl']
-				result = {
-					't': item['name'],
-					'a': a,
-					'c': self.framework.meta_search_util().make_cite(a),
-					'd': item['snippet'],
-				}
-				results.append(result)
+				inside_items = item.get('items')
+				for i in inside_items:
+					a = i['url']
+					result = {
+						't': i['title'],
+						'a': a,
+						'c': self.framework.meta_search_util().make_cite(a),
+						'd': '' if 'desc' not in i else i.get('desc'),
+					}
+					results.append(result)
 		return results
 
 	@property
 	def dns(self):
 		return self.framework.page_parse(self._pages).get_dns(self.q, self.links)
 
 	@property
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/qwant.py` & `maryam-2.5.2/maryam/core/util/engines/qwant_images.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,54 +14,55 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 
 class main:
 
-	def __init__(self, q, limit=2):
-		""" qwant.com search engine
+	def __init__(self, q, limit=1, count=50):
+		""" qwant.com image search engine
 
-			q 		  : Query for search
+			q 	  : Query for search
 			limit	  : Number of pages
+			count	  : Number of results
 		"""
 		self.framework = main.framework
 		self.q = q
-		self.limit = limit
+		self.limit = 10 if limit > 10 else limit
+		self.count = 50 if count > 50 else count
 		self._pages = ''
 		self._json = []
-		self._links = []
-		self._links_with_title = []
-		self.qwant = 'https://api.qwant.com/v3/search/web'
+		self.qwant = 'https://api.qwant.com/v3/search/images'
 
 	def run_crawl(self):
 		page = 1
 		set_page = lambda x: (x-1)*10
-		payload = {'q': self.q, 'offset': set_page(page), 'count': '10', 'safesearch': '0', 'device': 'desktop', 'locale': 'en_us'}
+		payload = {'t': 'images', 'q': self.q, 'offset': set_page(page), 'count': '10', \
+			'safesearch': '0', 'device': 'desktop', 'locale': 'en_GB', 'device': 'desktop'}
 		while True:
 			self.framework.verbose(f"[QWANT] Searching in {page+1} page...")
 			try:
 				req = self.framework.request(url=self.qwant, params=payload)
 			except Exception as e:
-				self.framework.error(f"ConnectionError {e}.", 'util/engines/qwant', 'util/engines/qwant', 'run_crawl')
-				self.framework.error('Qwant is missed!', 'util/engines/qwant', 'util/engines/qwant', 'run_crawl')
+				self.framework.error(f"ConnectionError {e}.", 'util/engines/qwant_images', 'run_crawl')
+				self.framework.error('Qwant is missed!', 'util/engines/qwant_images', 'run_crawl')
 				break
 			else:
 				if req.status_code == 429 and "I can't let you do that..." in req.text and '<div class="error-code">' in req.text:
-					self.framework.error('429 Too Many Requests', 'util/engines/qwant', 'run_crawl')
+					self.framework.error('429 Too Many Requests', 'util/engines/qwant_images', 'run_crawl')
 					return
 				self._pages += req.text
 				try:
 					self._json.append(req.json())
 				except Exception as e:
-					self.framework.error('429 Too Many Requests', 'util/engines/qwant', 'run_crawl')
+					self.framework.error('429 Too Many Requests', 'util/engines/qwant_images', 'run_crawl')
 					return
 				else:
 					if req.json() == {'status': 'error', 'data': {'error_code': 22}}:
-						self.framework.error('429 Too Many Requests', 'util/engines/qwant', 'run_crawl')
+						self.framework.error('429 Too Many Requests', 'util/engines/qwant_images', 'run_crawl')
 						return
 					else:
 						if page == self.limit:
 							break
 						page += 1
 						payload['offset'] = set_page(page)
 
@@ -70,46 +71,35 @@
 		return self._pages
 
 	@property
 	def json(self):
 		return self._json
 
 	@property
-	def links(self):
-		for page in self._json:
-			results = page.get('data', {}).get('result', {}).get('items', {})
-			self._links.extend([x.get('url') for x in results])
-		return self._links
-
-	@property
 	def results(self):
 		results = []
 		for page in self._json:
 			items = page.get('data', {}).get('result', {})
 			if items:
-				items = items.get('items', {})
-				if items:
-					items = items.get('mainline', {})
+				items = items.get('items', [])
 			for item in items:
-				inside_items = item.get('items')
-				for i in inside_items:
-					a = i['url']
-					result = {
-						't': i['title'],
-						'a': a,
-						'c': self.framework.meta_search_util().make_cite(a),
-						'd': '' if 'desc' not in i else i.get('desc'),
-					}
-					results.append(result)
+				results.append({
+					"a": item.get("url"),
+					"i": item.get("media"),
+					"t": item.get("title"),
+					"d": f"{item.get('width')}*{item.get('height')} {item.get('size')}B"}
+				)
+
 		return results
 
 	@property
 	def dns(self):
 		return self.framework.page_parse(self._pages).get_dns(self.q, self.links)
 
 	@property
 	def emails(self):
 		return self.framework.page_parse(self._pages).get_emails(self.q)
 
 	@property
 	def docs(self):
 		return self.framework.page_parse(self._pages).get_docs(self.q, self.links)
+
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/qwant_images.py` & `maryam-2.5.2/maryam/core/util/engines/startpage.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,95 +11,108 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-
 class main:
 
-	def __init__(self, q, limit=1, count=50):
-		""" qwant.com image search engine
+	def __init__(self, q, limit=2):
+		""" startpage.com search engine
 
-			q 	  : Query for search
+			q 		  : Query for search
 			limit	  : Number of pages
-			count	  : Number of results
 		"""
 		self.framework = main.framework
-		self.q = q
-		self.limit = 10 if limit > 10 else limit
-		self.count = 50 if count > 50 else count
+		self.q = self.framework.urlib(q).quote
+		self.limit = limit
+		self.xpath_name = {
+			'results': '/html/body/div[2]/div/div[2]/div[1]/div[2]/div[1]/div/section[2]/div',
+			'results_content': './/div[1]/p',
+			'results_links': './/div[1]/div[2]/a',
+			'results_title': './/div[1]/div[2]/a/h3'
+		}
+		self.xpath = {
+			self.xpath_name['results']: [
+				self.xpath_name['results_content'],
+				self.xpath_name['results_links'],
+				self.xpath_name['results_title']
+			]
+		}
 		self._pages = ''
-		self._json = []
-		self.qwant = 'https://api.qwant.com/v3/search/images'
+		self.startpage = 'startpage.com'
 
 	def run_crawl(self):
-		page = 1
-		set_page = lambda x: (x-1)*10
-		payload = {'t': 'images', 'q': self.q, 'offset': set_page(page), 'count': '10', \
-			'safesearch': '0', 'device': 'desktop', 'locale': 'en_GB', 'device': 'desktop'}
-		while True:
-			self.framework.verbose(f"[QWANT] Searching in {page+1} page...")
+		url = f"https://{self.startpage}/sp/search"
+
+		headers = {
+			'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:90.0) Gecko/20100101 Firefox/90.0',
+			'Content-Type': 'application/x-www-form-urlencoded'
+		}
+
+		data = {
+				'query': self.q
+		}
+
+		self.framework.verbose(f"[STARTPAGE] Searching in {self.startpage}...")
+
+		for i in range(self.limit):
+			data['page'] = i
+
 			try:
-				req = self.framework.request(url=self.qwant, params=payload)
+				req = self.framework.request(
+						url=url,
+						method='POST',
+						headers=headers,
+						data=data
+				)
 			except Exception as e:
-				self.framework.error(f"ConnectionError {e}.", 'util/engines/qwant_images', 'run_crawl')
-				self.framework.error('Qwant is missed!', 'util/engines/qwant_images', 'run_crawl')
-				break
+				self.framework.error(f"ConnectionError {e}.", 'util/startpage', 'run_crawl')
+				self.framework.error('Startpage is missed!', 'util/startpage', 'run_crawl')
+				return
+
 			else:
-				if req.status_code == 429 and "I can't let you do that..." in req.text and '<div class="error-code">' in req.text:
-					self.framework.error('429 Too Many Requests', 'util/engines/qwant_images', 'run_crawl')
-					return
-				self._pages += req.text
-				try:
-					self._json.append(req.json())
-				except Exception as e:
-					self.framework.error('429 Too Many Requests', 'util/engines/qwant_images', 'run_crawl')
-					return
-				else:
-					if req.json() == {'status': 'error', 'data': {'error_code': 22}}:
-						self.framework.error('429 Too Many Requests', 'util/engines/qwant_images', 'run_crawl')
-						return
-					else:
-						if page == self.limit:
-							break
-						page += 1
-						payload['offset'] = set_page(page)
+				page = req.text
+				self._pages += page
 
-	@property
-	def pages(self):
-		return self._pages
+				if '> Next <' not in page:
+					break
 
-	@property
-	def json(self):
-		return self._json
 
 	@property
 	def results(self):
+		parser = self.framework.page_parse(self._pages)
+		xpath_results = parser.html_fromstring(self.xpath)
 		results = []
-		for page in self._json:
-			items = page.get('data', {}).get('result', {})
-			if items:
-				items = items.get('items', [])
-			for item in items:
-				results.append({
-					"a": item.get("url"),
-					"i": item.get("media"),
-					"t": item.get("title"),
-					"d": f"{item.get('width')}*{item.get('height')} {item.get('size')}B"}
-				)
-
+		if not xpath_results:
+			return results
+		root = xpath_results[self.xpath_name['results']]
+		for i in range(len(root[self.xpath_name['results_links']])):
+			link = root[self.xpath_name['results_links']][i].get('href')
+			title = root[self.xpath_name['results_title']][i].text_content().strip()
+			desc = root[self.xpath_name['results_content']][i].text_content().strip()
+			cite = self.framework.meta_search_util().make_cite(link)
+			result = {
+				't': title,
+				'a': link,
+				'c': cite,
+				'd': desc,
+			}
+			results.append(result)
 		return results
 
 	@property
+	def pages(self):
+		return self._pages
+
+	@property
 	def dns(self):
-		return self.framework.page_parse(self._pages).get_dns(self.q, self.links)
+		return self.framework.page_parse(self._pages).get_dns(self.q)
 
 	@property
 	def emails(self):
 		return self.framework.page_parse(self._pages).get_emails(self.q)
 
 	@property
 	def docs(self):
-		return self.framework.page_parse(self._pages).get_docs(self.q, self.links)
-
+		return self.framework.page_parse(self._pages).get_docs(self.q)
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/searx.py` & `maryam-2.5.2/maryam/core/util/engines/yandex.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,99 +11,65 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-class main:
+import re
+import webbrowser
 
-	def __init__(self, q, limit=1):
-		""" searx search engine
+class main:
 
-			q	: Query for search
-			limit	: Number of Pages
+	def __init__(self, q, limit=2, count=100):
+		""" yandex.com search engine
 
+			q 		  : query for search
+			limit	  : Number of pages
+			count	  : Number of links
 		"""
 		self.framework = main.framework
-		self.q = q
-		self._pages = ''
+		self.q = self.framework.urlib(q).quote
+		self.count = count
 		self.limit = limit
-		self._links = []
-		self._json = {}
-		self.searx = ['https://searx.prvcy.eu/search', 'https://searx.xyz/search', 'https://searx.nevrlands.de/searx/search', 'https://searx.info/search']
+		self._pages = ''
+		self.yandex = 'yandex.com'
 
 	def run_crawl(self):
-		page = 1
-		self._json['results'] = [] 
-		params = {'category_general': 1, 'q': self.q, 
-			  'pageno': 1, 'time_range': None, 
-			  'format': 'json'}
-		max_attempts = 0
-		for url in self.searx:
-			while True:
-				self.framework.verbose(f"[SEARX] Searching {url} page {params['pageno']}...", end='\r')
-				try:
-					req = self.framework.request(
-						url=url,
-						params=params,
-						allow_redirects= True)
-				except Exception as e:
-					self.framework.error(f"ConnectionError: {e}", 'util/searx', 'run_crawl')
-					max_attempts += 1
-					if max_attempts == self.limit:
-						self.framework.error(f"Searx {url} is missed!", 'util/searx', 'run_crawl')
-						return
-				else:
-					self._pages += req.text
-					if req.status_code == 200 and 'results' in req.json():
-						self._json['results'] += req.json()['results']
-					else:
-						self.framework.error(f"Searx {url} is missed!", 'util/searcx', 'run_crawl')
-						break
-					if params['pageno'] >= self.limit:
-						return
-					params['pageno'] += 1
+		urls = [f"https://{self.yandex}/search?text={self.q}&numdoc={self.count}&p={i}" for i in range(1, self.limit+1)]
+		max_attempt = len(urls)
+		for url in range(len(urls)):
+			self.framework.debug(f"[YANDEX] Searching in {url} page...")
+			try:
+				req = self.framework.request(url=urls[url], allow_redirects=True)
+			except:
+				self.framework.error('ConnectionError', 'util/yandex', 'run_crawl')
+				max_attempt -= 1
+				if max_attempt == 0:
+					self.framework.error('Yandex is missed!', 'util/yandex', 'run_crawl')
+					break
+			else:
+				if '<title>Oops!</title>' in req.text:
+					self.framework.error('Yandex CAPTCHA triggered.', 'util/yandex', 'run_crawl')
+					return
+
+				page = req.text
+				if ']">next</a>' not in page:
+					self._pages += page
+					break
+				self._pages += page
 
 	@property
 	def pages(self):
 		return self._pages
 
 	@property
-	def links(self):
-		for result in self._json['results']:
-			self._links.append(result['url'])
-		return self._links
-
-	@property
-	def results(self):
-		results = []
-		for result in self._json['results']:
-			if 'content' in result:
-				content = result['content']
-			else:
-				content = 'No description provided'
-			cite = self.framework.meta_search_util().make_cite(result['url'])
-			results.append({
-				't': result['title'],
-				'a': result['url'],
-				'c': cite,
-				'd': content
-			})
-
-		return results
-	
-	@property
-	def json(self):
-		return self._json
-
-	@property
 	def dns(self):
 		return self.framework.page_parse(self._pages).get_dns(self.q)
 
 	@property
 	def emails(self):
 		return self.framework.page_parse(self._pages).get_emails(self.q)
-	
+
 	@property
 	def docs(self):
 		return self.framework.page_parse(self._pages).get_docs(self.q)
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/startpage.py` & `maryam-2.5.2/maryam/core/util/osint/reddit.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,108 +11,105 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
+import datetime
+
 class main:
 
-	def __init__(self, q, limit=2):
-		""" startpage.com search engine
+	def __init__(self, q, count=20, sortby='relevance', verbose=False):
+		""" Reddit search engine
 
-			q 		  : Query for search
-			limit	  : Number of pages
+				q         : query for search
+				count     : maximum result count
+				verbose   : print entire json 
 		"""
 		self.framework = main.framework
-		self.q = self.framework.urlib(q).quote
-		self.limit = limit
-		self.xpath_name = {
-			'results': '/html/body/div[2]/div/div[2]/div[1]/div[2]/div[1]/div/section[2]/div',
-			'results_content': './/div[1]/p',
-			'results_links': './/div[1]/div[2]/a',
-			'results_title': './/div[1]/div[2]/a/h3'
-		}
-		self.xpath = {
-			self.xpath_name['results']: [
-				self.xpath_name['results_content'],
-				self.xpath_name['results_links'],
-				self.xpath_name['results_title']
-			]
-		}
-		self._pages = ''
-		self.startpage = 'startpage.com'
+		self.q = q
+		self.count = count
+		self.sortby = sortby
+		self._json = {}
+		self._posts = []
+		self._verbose = verbose
 
 	def run_crawl(self):
-		url = f"https://{self.startpage}/sp/search"
-
-		headers = {
-			'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:90.0) Gecko/20100101 Firefox/90.0',
-			'Content-Type': 'application/x-www-form-urlencoded'
+		self.framework.verbose('[REDDIT] Searching the reddit domain...')
+		url = f'https://gateway.reddit.com/desktopapi/v1/search'
+		payload = {
+			'q': self.q,
+			'sort': self.sortby,
+			't': 'all'
 		}
 
-		data = {
-				'query': self.q
-		}
-
-		self.framework.verbose(f"[STARTPAGE] Searching in {self.startpage}...")
-
-		for i in range(self.limit):
-			data['page'] = i
-
+		for _ in range(self.count//25+1):
 			try:
-				req = self.framework.request(
-						url=url,
-						method='POST',
-						headers=headers,
-						data=data
+				res = self.framework.request(
+						url, 
+						params=payload,
 				)
+
 			except Exception as e:
-				self.framework.error(f"ConnectionError {e}.", 'util/startpage', 'run_crawl')
-				self.framework.error('Startpage is missed!', 'util/startpage', 'run_crawl')
-				return
+				self.framework.error(f"ConnectionError {e}.", 'util/osint/reddit', 'run_crawl')
+				self.framework.error('Reddit is missed!', 'util/osint/reddit', 'run_crawl')
 
 			else:
-				page = req.text
-				self._pages += page
+				self._json.update(res.json())
+				self._posts.extend(list(self._json['posts'].values()))
 
-				if '> Next <' not in page:
-					break
+	@property
+	def json(self):
+		return self._json
 
+	@property
+	def posts(self):
+		return self._posts
 
 	@property
 	def results(self):
-		parser = self.framework.page_parse(self._pages)
-		xpath_results = parser.html_fromstring(self.xpath)
 		results = []
-		if not xpath_results:
-			return results
-		root = xpath_results[self.xpath_name['results']]
-		for i in range(len(root[self.xpath_name['results_links']])):
-			link = root[self.xpath_name['results_links']][i].get('href')
-			title = root[self.xpath_name['results_title']][i].text_content().strip()
-			desc = root[self.xpath_name['results_content']][i].text_content().strip()
-			cite = self.framework.meta_search_util().make_cite(link)
-			result = {
-				't': title,
-				'a': link,
-				'c': cite,
-				'd': desc,
-			}
-			results.append(result)
-		return results
+		for count, post in enumerate(self._posts, 1):
+			if count > self.count:
+				break
 
-	@property
-	def pages(self):
-		return self._pages
+			date = datetime.datetime.fromtimestamp(int(post['created'])//1000).strftime("%m/%d/%Y, %H:%M:%S")
 
-	@property
-	def dns(self):
-		return self.framework.page_parse(self._pages).get_dns(self.q)
+			media = post['media']
+			if media is not None:
+				type = media['type']
 
-	@property
-	def emails(self):
-		return self.framework.page_parse(self._pages).get_emails(self.q)
+				if type == 'embed':
+					desc = media['content']
+
+				elif type == 'text':
+					desc = media.get('markdownContent')
+
+				elif type == 'video':
+					desc = 'Video description currently not supported'
+
+				elif type == 'gallery':
+					desc = []
+					for item in media['gallery']['items']:
+						id = item['mediaId']
+						desc.append(media['mediaMetadata'][id]['s']['u'])
+					desc = '\n'.join(desc)
+
+				elif type == 'image':
+					desc = media['content']
+
+			elif post['source'] is not None:
+				desc = post['source']['url']
+
+			else:
+				desc = 'Description not available'
+
+			results.append({
+				't': post['title'],
+				'a': post['permalink'],
+				'c': f"author: {post['author']} | date: {date}",
+				'd': desc
+			})
+
+		return results
 
-	@property
-	def docs(self):
-		return self.framework.page_parse(self._pages).get_docs(self.q)
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/yahoo.py` & `maryam-2.5.2/maryam/core/util/engines/yahoo.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/engines/yandex.py` & `maryam-2.5.2/maryam/core/util/osint/keyserver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 """
 OWASP Maryam!
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 any later version.
@@ -11,65 +12,50 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-import re
-import webbrowser
-
 class main:
 
-	def __init__(self, q, limit=2, count=100):
-		""" yandex.com search engine
+	def __init__(self, q, limit=10):
+		""" keyserver.ubuntu.com search engine
 
 			q 		  : query for search
 			limit	  : Number of pages
-			count	  : Number of links
 		"""
 		self.framework = main.framework
-		self.q = self.framework.urlib(q).quote
-		self.count = count
+		self.q = q
 		self.limit = limit
 		self._pages = ''
-		self.yandex = 'yandex.com'
+		self._json_pages = ''
+		self.keyserver_api = f"https://keyserver.ubuntu.com/pks/lookup?search=@{self.q}&op=index"
+		self.acceptable = False
 
 	def run_crawl(self):
-		urls = [f"https://{self.yandex}/search?text={self.q}&numdoc={self.count}&p={i}" for i in range(1, self.limit+1)]
-		max_attempt = len(urls)
-		for url in range(len(urls)):
-			self.framework.debug(f"[YANDEX] Searching in {url} page...")
-			try:
-				req = self.framework.request(url=urls[url], allow_redirects=True)
-			except:
-				self.framework.error('ConnectionError', 'util/yandex', 'run_crawl')
-				max_attempt -= 1
-				if max_attempt == 0:
-					self.framework.error('Yandex is missed!', 'util/yandex', 'run_crawl')
-					break
-			else:
-				if '<title>Oops!</title>' in req.text:
-					self.framework.error('Yandex CAPTCHA triggered.', 'util/yandex', 'run_crawl')
-					return
-
-				page = req.text
-				if ']">next</a>' not in page:
-					self._pages += page
-					break
-				self._pages += page
+		self.framework.verbose('[KEYSERVER] Searching in keyserver...')
+		try:
+			req = self.framework.request(self.keyserver_api)
+		except:
+			self.framework.debug('ConnectionError', 'util/keyserver', 'run_crawl')
+			self.framework.error('Keyserver is missed!', 'util/keyserver', 'run_crawl')
+			return
+		self._pages += req.text
+		return self.framework.page_parse(self._pages).get_emails(self.q)
 
 	@property
 	def pages(self):
 		return self._pages
-
+	
 	@property
-	def dns(self):
-		return self.framework.page_parse(self._pages).get_dns(self.q)
+	def json_pages(self):
+		return self._json_pages
 
 	@property
 	def emails(self):
 		return self.framework.page_parse(self._pages).get_emails(self.q)
 
 	@property
-	def docs(self):
-		return self.framework.page_parse(self._pages).get_docs(self.q)
+	def dns(self):
+		return self.framework.page_parse(self.pages).get_dns(self.q)
+
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/footprint/cms_identify.py` & `maryam-2.5.2/maryam/core/util/footprint/cms_identify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/footprint/lang_identify.py` & `maryam-2.5.2/maryam/core/util/footprint/lang_identify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/footprint/os_identify.py` & `maryam-2.5.2/maryam/core/util/footprint/os_identify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/footprint/waf_identify.py` & `maryam-2.5.2/maryam/core/util/footprint/waf_identify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/footprint/wapps.py` & `maryam-2.5.2/maryam/core/util/footprint/wapps.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/helpers/keywords.py` & `maryam-2.5.2/maryam/core/util/helpers/keywords.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,27 +30,24 @@
 		"""
 		self.framework = main.framework
 		self.q = self.framework.urlib(q).quote
 		self._keys_category = []
 		self._keys = []
 		self._yahoo = \
 			'https://search.yahoo.com/sugg/gossip/gossip-us-ura/?f=1&output=sd1&command=<Q>&pq=a&l=3&nresults=30000&b=3&s=1c&callback=<b>'
-		self._google = 'https://www.google.com/complete/search?q=<Q>&cp=&client=psy-ab&xssi=t&gs_ri=gws-wiz&hl=&authuser=0&psi='
+		self._google = 'https://www.google.com/complete/search?q=<Q>&cp=10&client=gws-wiz&xssi=t&gs_pcrt=undefined&hl=en&authuser=0'
 		self._bing = 'https://www.bing.com/AS/Suggestions?pt=&mkt=de-de&qry=<Q>&cp=0&css=0&cvid=1'
-		self._millionshort = 'https://millionshort.com/api/suggestions?q=<Q>'
-		self._zapmeta = 'https://www.zapmeta.com/suggest?q=<Q>'
+		# self._zapmeta = 'https://www.zapmeta.com/suggest?q=<Q>'
 		self._searx = 'https://searx.be/autocompleter?q=<Q>'
-		self._peekier = {'url': 'https://search.peekier.com/suggestions', 'payload': {'q': '<Q>', 'region': ''}, 'method': 'POST'}
-		self._gigablast = 'https://gigablast.com/qs?rwp=0&lang=en&q=<Q>'
 
 	def run_crawl(self):
 		keys = {}
-		for source in ('yahoo', 'google', 'bing', 'millionshort',\
-						'zapmeta', 'searx', 'peekier', 'gigablast'):
-			attr = getattr(self, '_'+source)
+		for source in ('yahoo', 'google', 'bing',\
+						'searx'):
+			attr = getattr(self, '_' + source)
 			if isinstance(attr, dict):
 				url = attr['url']
 				method = 'POST'
 				data = attr.get('payload', {'q':'<Q>'})
 				data['q'] = self.q
 			else:
 				url = attr.replace('<Q>', self.q)
@@ -66,22 +63,20 @@
 		keys['yahoo'] = [x['k'] for x in keys['yahoo'].json().get('r', [])]
 		try:
 			google = json.loads(f"{keys['google'].text[5:]}")[0]
 			keys['google'] = [re.sub(r"<b>|<\\/b>|</b>", '', x[0]) for x in google]
 		except:
 			keys['google'] = []
 		keys['bing'] = re.findall(r'<span class="sa_tm_text">([^<]+)</span>', re.sub(r'<.?strong>', '', keys['bing'].text))
-		keys['zapmeta'] = [x[0] for x in keys['zapmeta'].json()] if hasattr(keys['zapmeta'], 'json') else []
-		keys['millionshort'] = keys['millionshort'].json().get('suggestions', []) if hasattr(keys['millionshort'], 'json') else []
+		# keys['zapmeta'] = [x[0] for x in keys['zapmeta'].json()] if hasattr(keys['zapmeta'], 'json') else []
 		try:
 			keys['searx'] = keys['searx'].json()[self.q]
 		except:
 			keys['searx'] = []
-		keys['peekier'] = keys['peekier'].json()['results']
-		keys['gigablast'] = re.findall(r'" >([^\n]+?)</td', keys['gigablast'].text)
+
 		self._keys_category = keys
 		for s in keys:
 			for i in keys[s]:
 				self._keys.append(i)
 
 	@property
 	def keys_category(self):
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/helpers/page_parse.py` & `maryam-2.5.2/maryam/core/util/helpers/page_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 		self.page = re.sub(subs, '', self.page)
 		self.page = re.sub(r"%3a", ' ', self.page)
 		self.page = re.sub(r"%2f", ' ', self.page)
 		self.page = re.sub(r"%2f", ' ', self.page)
 
 	def html_fromstring(self, xpath, parent=None, results={}):
 		if self.page == '':
-			self.framework.error(f"document is nil", 'util/page_parse', 'html_fromstring')
+			self.framework.error('document is nil', 'util/page_parse', 'html_fromstring')
 			return False
 
 		if isinstance(xpath, dict):
 			for root in xpath:
 				results[root] = self.html_fromstring(xpath[root], root)
 		elif isinstance(xpath, list):
 			results = {}
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/helpers/rand_uagent.py` & `maryam-2.5.2/maryam/core/util/helpers/rand_uagent.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/helpers/reglib.py` & `maryam-2.5.2/maryam/core/util/helpers/reglib.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/helpers/urlib.py` & `maryam-2.5.2/maryam/core/util/helpers/urlib.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/helpers/web_scrap.py` & `maryam-2.5.2/maryam/core/util/helpers/web_scrap.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/iris/chart.py` & `maryam-2.5.2/maryam/core/util/iris/chart.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/iris/cluster.py` & `maryam-2.5.2/maryam/core/util/iris/cluster.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/iris/meta_search_util.py` & `maryam-2.5.2/maryam/core/util/iris/meta_search_util.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/iris/plotlyutil.py` & `maryam-2.5.2/maryam/core/util/iris/word_cloud.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,30 +8,45 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-import plotlyutil
+import re
+import os
+from wordcloud import WordCloud
+import matplotlib.pyplot as plt
 
-class main:
-
-	def __init__(self):
-		""" a class for plotly framework. currently it just supports common methods """
+class main:	
+	def __init__(self):	
 		self.framework = main.framework
 
-	def tf_pie(self, docs: 'documents', form: 'documet form. e.g html',
-				last: 'number of words', without_punc=True, remove_stopwords=False):
+	def _remove_url(self, data):
+		return re.sub(r"(http|ftp|https)://([\w_-]+(?:(?:\.[\w_-]+)+))([\w.,@?^=%&:/~+#-]*[\w@?^=%&/~+#-])?", '', data)	
+	
+	def plot_wcloud(self, title, docs: 'documents', form: 'documet form. e.g html', limit: 'number of words', 
+	without_punc=True, remove_stopwords=False, should_show=True):
+		docs = str(docs)
+		docs = self._remove_url(docs)
 		tf = self.framework.tf_histogram(docs, form, without_punc)
+
 		if remove_stopwords:
 			tf.remove_stopwords()
-		bow = tf._counter(last)
-		values = []
-		labels = []
-		for word, count in bow:
-			values.append(count)
-			labels.append(word)
-		fig = plotly.graph_objects.Figure(plotly.graph_objects.Pie(values=values,labels=labels,
-			texttemplate = "%{label}: %{value:s} <br>(%{percent})",
-			textposition = "inside"))
-		fig.show()
+		bow = tf._counter(limit)
+		cloud_data = ' '.join(i[0] for i in bow)
+
+		if not cloud_data:
+			self.framework.error('NoDataToPrintError.', 'util/iris/word_cloud', 'plot_wcloud')
+			return False
+
+		wcd = WordCloud().generate(cloud_data)
+		plt.imshow(wcd, interpolation='bilinear')
+		plt.axis("off")
+		plt.title(title)
+		filename = os.path.join(self.framework.workspace,title.replace(' ','_')+'.png')
+		plt.savefig(filename, format="png")
+		if should_show:
+			plt.show()
+
+		return filename
+
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/iris/retriever.py` & `maryam-2.5.2/maryam/core/util/iris/retriever.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/iris/safe_searcher.py` & `maryam-2.5.2/maryam/core/util/iris/safe_searcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,23 +19,20 @@
 		self.framework = main.framework
 
 		if engine_q is None:
 			self._engine_q = [
 					self.framework.google,
 					self.framework.duckduckgo,
 					self.framework.bing,
-					self.framework.millionshort,
 					self.framework.startpage,
 					self.framework.dogpile,
 					self.framework.qwant,
 					self.framework.yandex,
 					self.framework.yahoo,
 					self.framework.ask,
-					self.framework.gigablast,
-					self.framework.activesearch
 				]
 		else:
 			self._engine_q = engine_q
 
 		self._error_record = []
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/iris/tf_histogram.py` & `maryam-2.5.2/maryam/core/util/iris/tf_histogram.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/iris/topic.py` & `maryam-2.5.2/maryam/core/util/iris/topic.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,114 +54,114 @@
 				print("\n\n json file (before preprocessing) = ")
 				print(tmp)
 
 			tmp['td'] = tmp['t'] + ' ' + tmp['d']
 			self.corpus = tmp['td'].str.lower().apply(remove_stopwords).to_numpy()
 
 		else:
-			print("ERROR, only accept csv or json file!")
+			print('ERROR, only accept csv or json file!')
 
 		if verbose == True:
-			print("\n\n number of corpus = ")
+			print('\n\n number of corpus = ')
 			print(len(self.corpus))
-			print("\n\n self.corpus[0] = ")
+			print('\n\n self.corpus[0] = ')
 			print(self.corpus[0])
-			print("\n\n all self.corpus = ")
+			print('\n\n all self.corpus = ')
 			print(self.corpus)
 
 		if showcharts == True:
-			print("\n\n histogram of the number of words in each corpus")
+			print('\n\n histogram of the number of words in each corpus')
 			pd.Series([len(e.split()) for e in self.corpus]).hist()
 			plt.show()
 
 	def run_sklearn_cluster_kmeans(self, selected_pretrained_model, showcharts, verbose):
 
 		from sklearn.cluster import KMeans
 		import scipy
 		import umap
 
 		pretrained_model = selected_pretrained_model
 		if verbose == True:
-			print("\n\n Model selection")
+			print('\n\n Model selection')
 			# https://www.sbert.net/docs/pretrained_models.html
 			print(pretrained_model)
 
 		model = SentenceTransformer(pretrained_model)
 		if verbose == True:
 			print(model)
 
 		corpus_embeddings = model.encode(self.corpus)
 		if verbose == True:
-			print("\n\n CORPUS EMBEDDING")
+			print('\n\n CORPUS EMBEDDING')
 			print(corpus_embeddings.shape)
 			print(corpus_embeddings)
 
 		K = 5
 		kmeans = KMeans(n_clusters=5, random_state=0).fit(corpus_embeddings)
 		if verbose == True:
-			print("\n\n Show Cluster using SkLearn KMeans")
+			print('\n\n Show Cluster using SkLearn KMeans')
 			print(kmeans)
 
 		corpus_labeled = pd.DataFrame({'ClusterLabel': kmeans.labels_, 'Sentence': self.corpus})
-		print("\n\n corpus_labeled = ")
+		print('\n\n corpus_labeled = ')
 		print(corpus_labeled)
 
 		cls_dist = pd.Series(kmeans.labels_).value_counts()
 		if verbose == True:
-			print("\n\n frequency of cluster label = ")
+			print('\n\n frequency of cluster label = ')
 			print(cls_dist)
 
 		distances = scipy.spatial.distance.cdist(kmeans.cluster_centers_, corpus_embeddings)
 		if verbose == True:
 			print("\n\n calculate distance of cluster's center point = ")
 			print(distances)
 
 		print("\n\n Cluster's center example = ")
 
 		centers = {}
-		print("Cluster", "Size", "Center-idx", "Center-Example", sep="\t\t")
+		print('Cluster', 'Size', 'Center-idx', 'Center-Example', sep='\t\t')
 		for i, d in enumerate(distances):
 			ind = np.argsort(d, axis=0)[0]
 			centers[i] = ind
 			print(i, cls_dist[i], ind, self.corpus[ind], sep="\t\t")
 
 		if showcharts == True:
-			print("\n\n Visualization of the cluster points")
+			print('\n\n Visualization of the cluster points')
 
 			X = umap.UMAP(n_components=2, min_dist=0.0).fit_transform(corpus_embeddings)
 			labels = kmeans.labels_
 
 			fig, ax = plt.subplots(figsize=(12, 8))
 			plt.scatter(X[:, 0], X[:, 1], c=labels, s=1, cmap='Paired')
 			for c in centers:
-				plt.text(X[centers[c], 0], X[centers[c], 1], "CLS-" + str(c), fontsize=24)
+				plt.text(X[centers[c], 0], X[centers[c], 1], 'CLS-' + str(c), fontsize=24)
 			plt.colorbar()
 			plt.show()
 
 	def run_topic_modeling_bertopic(self, selected_pretrained_model, verbose):
 
 		from bertopic import BERTopic
 
 		pretrained_model = selected_pretrained_model
 		if verbose == True:
-			print("\n\n Model selection")
+			print('\n\n Model selection')
 			# https://www.sbert.net/docs/pretrained_models.html
 			print(pretrained_model)
 
 		model = SentenceTransformer(pretrained_model)
 		if verbose == True:
 			print(model)
 
 		corpus_embeddings = model.encode(self.corpus)
 		if verbose == True:
-			print("\n\n CORPUS EMBEDDING")
+			print('\n\n CORPUS EMBEDDING')
 			print(corpus_embeddings.shape)
 			print(corpus_embeddings)
 
-		print("\n\n Topic Modeling with BERTopic")
+		print('\n\n Topic Modeling with BERTopic')
 
 		sentence_model = SentenceTransformer(pretrained_model)
 		if verbose == True:
 			print(sentence_model)
 
 		topic_model = BERTopic(embedding_model=sentence_model)
 		if verbose == True:
@@ -172,66 +172,66 @@
 		output = topic_model.get_topic_info()
 
 		corpus_labeled = pd.DataFrame({'ClusterLabel': topics, 'Sentence': self.corpus})
 		if verbose == True:
 			print("\n\n corpus_labeled = ")
 			print(corpus_labeled)
 
-		print("\n\n topics for each cluster = ")
+		print('\n\n topics for each cluster = ')
 
 		i = 0
 		while i < len(topic_model.get_topic_info()):
-			print("Cluster #" + str(i) + " = ")
+			print(f"Cluster #{i} = ")
 			print(topic_model.get_topic(i))
 			i += 1
 
 		return output
 
 
 	def run_search_topics_top2vec(self, keyword, showcharts, verbose):
 
 		from top2vec import Top2Vec
 
-		print("\n\n Search Topics Using Top2Vec (caution: might not work well for a small dataset)")
-		print("\n the Search Keyword = " + keyword)
+		print('\n\n Search Topics Using Top2Vec (caution: might not work well for a small dataset)')
+		print('\n the Search Keyword = ' + keyword)
 
-		pretrained_embedding_model = "universal-sentence-encoder-multilingual"
+		pretrained_embedding_model = 'universal-sentence-encoder-multilingual'
 		if verbose == True:
-			print("\n\n Pretrained Embedding Model")
+			print('\n\n Pretrained Embedding Model')
 			# https://tfhub.dev/google/universal-sentence-encoder-multilingual/
 			# 16 languages (Arabic, Chinese-simplified, Chinese-traditional, English, French, German, Italian, Japanese, Korean, Dutch, Polish, Portuguese, Spanish, Thai, Turkish, Russian) text encoder.
 			print(pretrained_embedding_model)
 
-		model = Top2Vec(documents=self.corpus.tolist(), speed="learn", workers=8)
+		model = Top2Vec(documents=self.corpus.tolist(), speed='learn', workers=8)
 		if verbose == True:
-			print("\n Model = ")
+			print('\n Model = ')
 			print(model)
 
 		if model.get_num_topics() < 5:
 			ntopics = model.get_num_topics()
 		else:
 			ntopics = 5
 
 		topic_words, word_scores, topic_nums = model.get_topics(ntopics)
 		print(topic_words)
 		print(word_scores)
 		print(topic_nums)
 
-		print("\n Semantic Search Documents by Keywords = ")
+		print('\n Semantic Search Documents by Keywords = ')
 		documents, document_scores, document_ids = model.search_documents_by_keywords(keywords=[keyword], num_docs=5)
 		for doc, score, doc_id in zip(documents, document_scores, document_ids):
 			print(f"Document: {doc_id}, Score: {score}")
-			print("-----------")
+			print('-----------')
 			print(doc)
-			print("-----------")
+			print('-----------')
 			print()
 
 		if showcharts == True:
-			print("\n\n Generate Word Clouds = ")
+			print('\n\n Generate Word Clouds = ')
 			topic_words, word_scores, topic_scores, topic_nums = model.search_topics(keywords=[keyword], num_topics=ntopics)
 			for topic in topic_nums:
 				model.generate_topic_wordcloud(topic)
 
-		print("\n Similar Keywords = ")
+		print('\n Similar Keywords = ')
 		words, word_scores = model.similar_words(keywords=[keyword], keywords_neg=[], num_words=20)
 		for word, score in zip(words, word_scores):
 			print(f"{word} {score}")
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/ahmia.py` & `maryam-2.5.2/maryam/core/util/osint/ahmia.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/bing_mobile_view.py` & `maryam-2.5.2/maryam/core/util/osint/bing_mobile_view.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/darksearch.py` & `maryam-2.5.2/maryam/core/util/osint/darksearch.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/exalead.py` & `maryam-2.5.2/maryam/core/util/osint/exalead.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/hunter.py` & `maryam-2.5.2/maryam/core/util/osint/hunter.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/keyserver.py` & `maryam-2.5.2/maryam/core/util/search/crt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 """
 OWASP Maryam!
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 any later version.
@@ -14,48 +13,47 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 class main:
 
-	def __init__(self, q, limit=10):
-		""" keyserver.ubuntu.com search engine
+	def __init__(self, q):
+		""" crt.sh search engine
 
-			q 		  : query for search
-			limit	  : Number of pages
+			q 		  : Query for search
 		"""
 		self.framework = main.framework
 		self.q = q
-		self.limit = limit
 		self._pages = ''
-		self._json_pages = ''
-		self.keyserver_api = f"https://keyserver.ubuntu.com/pks/lookup?search=@{self.q}&op=index"
-		self.acceptable = False
+		self._json_page = ''
+		self.crt = f"https://crt.sh/?q={q}&output=json"
 
 	def run_crawl(self):
-		self.framework.verbose('[KEYSERVER] Searching in keyserver...')
+		self.framework.verbose('[CRT] Starting Search...')
 		try:
-			req = self.framework.request(self.keyserver_api)
+			req = self.framework.request(self.crt)
 		except:
-			self.framework.debug('ConnectionError', 'util/keyserver', 'run_crawl')
-			self.framework.error('Keyserver is missed!', 'util/keyserver', 'run_crawl')
+			self.framework.debug('[CRT] ConnectionError')
+			self.framework.error('CRT is missed!', 'util/crt', 'run_crawl')
 			return
-		self._pages += req.text
-		return self.framework.page_parse(self._pages).get_emails(self.q)
+		self._pages = req.text
+		self._json_page = req.json()
+		try:
+			self._json_page = req.json()
+			if self._json_page == []:
+				self._json_page = {}
+		except:
+			self.framework.error('CRT is missed!', 'util/crt', 'run_crawl')
+			self._json_page = []
 
 	@property
 	def pages(self):
 		return self._pages
 	
 	@property
-	def json_pages(self):
-		return self._json_pages
-
-	@property
-	def emails(self):
-		return self.framework.page_parse(self._pages).get_emails(self.q)
+	def json_page(self):
+		return self._json_page
 
 	@property
 	def dns(self):
 		return self.framework.page_parse(self.pages).get_dns(self.q)
-
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/netcraft.py` & `maryam-2.5.2/maryam/core/util/osint/netcraft.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/numverify.py` & `maryam-2.5.2/maryam/core/util/osint/numverify.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/onionland.py` & `maryam-2.5.2/maryam/core/util/osint/onionland.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/reddit.py` & `maryam-2.5.2/maryam/core/util/search/photon.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,66 @@
 """
 OWASP Maryam!
-
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 any later version.
-
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
-
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-import datetime
-
 class main:
 
-	def __init__(self, q, count=20, sortby='relevance', verbose=False):
-		""" Reddit search engine
-
-				q         : query for search
-				count     : maximum result count
-				verbose   : print entire json 
+	def __init__(self, q, limit):
 		"""
+		photon uses osm data for locations and reverse geolocation
+		q       :   query
+		limit   :   max result count
+		"""
+
 		self.framework = main.framework
-		self.q = q
-		self.count = count
-		self.sortby = sortby
+		self.q = q.split('_')[0]
+		self.lat = q.split('_')[1]
+		self.lon = q.split('_')[2]
+		self._pages = ''
 		self._json = {}
-		self._posts = []
-		self._verbose = verbose
+		self.ph = 'https://photon.komoot.io/'
 
 	def run_crawl(self):
-		self.framework.verbose('[REDDIT] Searching the reddit domain...')
-		url = f'https://gateway.reddit.com/desktopapi/v1/search'
-		payload = {
-			'q': self.q,
-			'sort': self.sortby,
-			't': 'all'
-		}
-
-		for _ in range(self.count//25+1):
-			try:
-				res = self.framework.request(
-						url, 
-						params=payload,
-				)
-
-			except Exception as e:
-				self.framework.error(f"ConnectionError {e}.", 'util/osint/reddit', 'run_crawl')
-				self.framework.error('Reddit is missed!', 'util/osint/reddit', 'run_crawl')
-
+		urls = [f"{self.ph}api/?",f"{self.ph}reverse?"]
+		if self.q and self.lat and self.lon:
+			if self.q == 'q':
+				url = urls[1]
+				payloads = {'lat': self.lat, 'lon': self.lon}
 			else:
-				self._json.update(res.json())
-				self._posts.extend(list(self._json['posts'].values()))
+				url = urls[0]
+				payloads = {'q': self.q, 'lat': self.lat, 'lon': self.lon}
+		else:
+			url = urls[0]
+			payloads = {'q': self.q}
+		self.framework.verbose("[PHOTON]Searching in photon.komoot.io...")
+		try:
+			req = self.framework.request(
+				url = url,
+				params = payloads
+			)
+			result = req.text
+			result_json = req.json()
+		except:
+			self.framework.error('ConnectionError', 'util/photon', 'run_crawl')
+		else:
+			if 'message' in req.text:
+				self.framework.verbose(f"[PHOTON] Search ended with the message: {req.json()['message'].split(',')[0]}")
+		self._pages = result
+		self._json = result_json
 
 	@property
-	def json(self):
-		return self._json
+	def pages(self):
+		return self._pages
 
 	@property
-	def posts(self):
-		return self._posts
-
-	@property
-	def results(self):
-		results = []
-		for count, post in enumerate(self._posts, 1):
-			if count > self.count:
-				break
-
-			date = datetime.datetime.fromtimestamp(int(post['created'])//1000).strftime("%m/%d/%Y, %H:%M:%S")
-
-			media = post['media']
-			if media is not None:
-				type = media['type']
-
-				if type == 'embed':
-					desc = media['content']
-
-				elif type == 'text':
-					desc = media.get('markdownContent')
-
-				elif type == 'video':
-					desc = 'Video description currently not supported'
-
-				elif type == 'gallery':
-					desc = []
-					for item in media['gallery']['items']:
-						id = item['mediaId']
-						desc.append(media['mediaMetadata'][id]['s']['u'])
-					desc = '\n'.join(desc)
-
-				elif type == 'image':
-					desc = media['content']
-
-			elif post['source'] is not None:
-				desc = post['source']['url']
-
-			else:
-				desc = 'Description not available'
-
-			results.append({
-				't': post['title'],
-				'a': post['permalink'],
-				'c': f"author: {post['author']} | date: {date}",
-				'd': desc
-			})
-
-		return results
-
+	def json(self):
+		return self._json
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/tweet_search.py` & `maryam-2.5.2/maryam/core/util/osint/tweet_search.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/urlscan.py` & `maryam-2.5.2/maryam/core/util/osint/urlscan.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/osint/virustotal.py` & `maryam-2.5.2/maryam/core/util/osint/virustotal.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/arxiv.py` & `maryam-2.5.2/maryam/core/util/search/arxiv.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/ask.py` & `maryam-2.5.2/maryam/core/util/search/ask.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/core_ac.py` & `maryam-2.5.2/maryam/core/util/search/core_ac.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,58 +19,67 @@
 
 class main:
 
 	def __init__(self, q, limit=10):
 		""" core.ac.uk search engine
 
 				q         : query for search
-				limit     : maximum result count
+				limit     : maximum page search
 		"""
 		self.framework = main.framework
 		self.q = q
 		self.limit = limit
-		self._json = []
+		self._pages = ''
+		self._jsons = []
 		self._results = []
-		self.url = 'https://core.ac.uk/search/api/search'
+		self.url = 'https://core.ac.uk/search/_next/data/-JCaNMETLG_pZxb60WhOp/search.json'
 
 	def run_crawl(self):
 		self.framework.verbose('Searching the CORE domain...')
-
-		data = f'{{"basicQuery":{{"count":"{self.limit}","searchCriteria":"{self.q}","offset":0}}}}'
-		try:
-			req = self.framework.request(
-					url=self.url,
-					method='POST',
-					data=data,
-					)
-		except Exception as e:
-			self.framework.error(f"ConnectionError {e}.", 'util/search/core_ac', 'run_crawl')
-			self.framework.error('CORE.AC.UK is missed!', 'util/search/core_ac', 'run_crawl')
-			return
-		else:
-			self._json = req.json()
+		page = 1
+		payload = {'q': self.q, 'page': 1}
+		max_attempt = 0
+		while True:
+			try:
+				req = self.framework.request(
+						url=self.url,
+						method='GET',
+						params=payload,
+						)
+			except Exception as e:
+				self.framework.error(f"ConnectionError {e}.", 'util/search/core_ac', 'run_crawl')
+				max_attempt += 1
+				if max_attempt == self.limit:
+					self.framework.error('CORE.AC.UK is missed!', 'util/search/core_ac', 'run_crawl')
+					break
+			else:
+				self._pages += req.text
+				self._jsons.append(req.json())
+				page += 1
+				payload['page'] = page
+				if page >= self.limit:
+					break
 
 	@property
 	def json(self):
 		return self._json
 
 	@property
 	def results(self):
-		findlink = lambda x: x["downloadUrl"]
-		findauthors = lambda x: x.get("authorsString")
-		findtitle = lambda x: x["title"]
-		findsummary = lambda x: x.get("snippet")
-
-		for count,article in enumerate(self._json['results']):
-			if count == self.limit:
-				break
-			d = findsummary(article)
-			c = findauthors(article)
-			self._results.append({
-				't': findtitle(article),
-				'a': findlink(article),
-				'c': c if c is not None else 'Authors not available',
-				'd': re.sub('<[^<]+?>', '', d) if d is not None\
-						else 'Abstract not available'
+		findlink = lambda x: x['downloadUrl']
+		findauthors = lambda x: [i.get('name', '') for i in x.get('authors', [])]
+		findtitle = lambda x: x['title']
+		findsummary = lambda x: x.get('abstract')
+		for page in self._jsons:
+			for article in enumerate(page['pageProps']['data']['results']):
+				article = article[1]
+				d = findsummary(article)[:100] + '...'
+				c = findauthors(article)
+				c = ','.join(c)[:100] or '' + '...'
+				self._results.append({
+					't': findtitle(article),
+					'a': findlink(article),
+					'c': c,
+					'd': d,
 				})
 
 		return self._results
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/creativecommons.py` & `maryam-2.5.2/maryam/core/util/search/sepiasearch.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,69 +11,54 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 
 class main :
     def __init__(self, q, limit=15):
-        """ search.creativecommons.org search
+        """ sepiasearch.org search
         
             q 		  : The query for search
             limit	  : The number of details min 15 if exist
         """
         self.q = q
         self.limit = limit
-        self.url = 'https://api.creativecommons.engineering/v1/images'
-        self.params = {'q': self.q}
+        self.url = 'https://sepiasearch.org/api/v1/search/videos?'
+        self.params = {'search': self.q, 'boostLanguages[]': 'en', 'nsfw': 'false', 'start': 0, 'count': self.limit, 'sort': '-match'}
+        self.headers = {'Content-Type': 'application/x-www-form-urlencoded'}
         self._collected_data = []
         self._result_found = 0
         
     def run_crawl(self):
-        self.framework.verbose('[creativecommons] Extracting Data From API')
-        
-        # first page
-        success, response = self.send_request(params=self.params)
-        if not success: 
+        self.framework.verbose('[SEPIASEARCH] Extracting Data From API')
+        response = self.framework.request(self.url, params=self.params, headers=self.headers)
+        if response.status_code != 200:
+            self.framework.error('Request Fail', 'util/sepiasearch', 'run_crawl')
             return
-
-        self._result_found = response['result_count']
-        self.extract_data(response['results']) 
-        total_pages = response['page_count']
-        page_size = response['page_size']
-
-        # all next pages
-        if total_pages > 1 and len(self._collected_data) < self.limit:
-            self.params['shouldPersistImages'] = 'true' 
-            for i in range(self.limit//page_size + 1):
-                self.framework.verbose(f"[creativecommons] Extracting Data From API request-{i+1}")
-                success, response = self.send_request(params={**self.params, 'page': i+1})
-                if not success: 
-                    continue
-                self.extract_data(response['results'])
         
-    def send_request(self, params):
-        try:
-            response = self.framework.request(self.url, params=params)
-        except:
-            self.framework.error('Request Fail', 'util/creativecommons', 'send_request')
-        else:
-            if response.status_code != 200:
-                self.framework.error('Request Fail - Invalid request', 'util/creativecommons', 'send_request')
-                return False, None
-            return True, response.json()
-
-    def extract_data(self, data):
-        for result in data:
+        response = response.json()
+        self._result_found = response['total']
+        for result in response['data']:
             self._collected_data.append({
-                'Title': result['title'],
-                'Creator': result['creator'],
-                'Creator_url': result['creator_url'],
-                'Image-URL': result['url'],
+                'Title': result['name'],
+                'Author': result['account']['displayName'],
+                'URL': result['url'],
+                'Length': self.sec_to_hours(int(result.get('duration'))),
+                'Thumbnail': result['thumbnailUrl'],
+                'Embeded URL': result.get('embedUrl'),
+                'Published Date': result['publishedAt'],
             })
 
+    def sec_to_hours(self, minute):
+        """Convert minutes in hours"""
+        if isinstance(minute, int):
+            minu, sec = divmod(minute, 60)
+            return "{}:{}:{} hours".format(*divmod(minu, 60), sec)
+        return None
+
     @property
     def collected_data(self):
         return self._collected_data
 
     @property
     def total_result_found(self):
         return self._result_found
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/dictionary.py` & `maryam-2.5.2/maryam/core/util/search/dictionary.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/discord.py` & `maryam-2.5.2/maryam/core/util/search/discord.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/instagram.py` & `maryam-2.5.2/maryam/core/util/search/instagram.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/openstreetmap.py` & `maryam-2.5.2/maryam/core/util/search/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/pastebin.py` & `maryam-2.5.2/maryam/core/util/search/pastebin.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/piratebay.py` & `maryam-2.5.2/maryam/core/util/search/piratebay.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/pubmed.py` & `maryam-2.5.2/maryam/core/util/search/pubmed.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/reddit_pushshift.py` & `maryam-2.5.2/maryam/core/util/search/reddit_pushshift.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/sanctionsearch.py` & `maryam-2.5.2/maryam/core/util/search/sanctionsearch.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/scholar.py` & `maryam-2.5.2/maryam/core/util/search/scholar.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/wikileaks.py` & `maryam-2.5.2/maryam/core/util/search/wikipedia.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,105 @@
 """
 OWASP Maryam!
-
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 any later version.
-
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
-
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-import re
-
 class main:
 
-	def __init__(self, q, limit=1):
-		""" wikileaks.org search engine
-
-			q		: Query for search
-			limit	: Number of Pages
-
+	def __init__(self, q, count=10):
+		""" wikipedia.org search 
+			q          : Query for search
+			count      : Number of results
 		"""
-
 		self.framework = main.framework
 		self.q = q
-		self.agent = 'Mozilla/5.0 (X11; Linux x86_64; rv:86.0) Gecko/20100101 Firefox/86.0'
-		self._pages = ''
-		self.limit = limit
+		self.num = count
 		self._links = []
-		self._results = []
-		self._links_with_data = []
+		self._titles = []
+		self._pids = []
+		self.url = 'https://en.wikipedia.org/w/api.php'		
+		self.headers = {'User-Agent' : 'OWASP Maryam(github.com/saeeddhqan/maryam)'}
 
-	def run_crawl(self):
-		from bs4 import BeautifulSoup as bs
 
-		max_attempts = 0
-		url = 'https://search.wikileaks.org/advanced'
-		params = {'query': self.q, 'include_external_sources': True, 'page': 1}
-		while True:
-			self.framework.verbose(f"[WIKILEAKS] Searching in {params['page']} page ....", end='\r')
-			try:
-				req = self.framework.request(
-					url=url,
-					params=params,
-					headers={'User-Agent': self.agent},
-					allow_redirects=True)
-			except Exception as e:
-				self.framework.error(f"ConnectionError: {e}", 'util/wikileaks', 'run_crawl')
-				max_attempts += 1
-				if max_attempts == self.limit:
-					self.framework.error('Wikileaks is missed!', 'util/wikileaks', 'run_crawl')
-					return
-			else:
-				self._pages += req.text
-				params['page'] += 1
-				if params['page'] >= self.limit:
-					break
-
-		soup = bs(self._pages, 'html.parser')
-		self._results = soup.find_all('div', class_='info')
-		for result in self._results:
-			self._links.append(result.find_all('a')[0]['href'])
+	def run_crawl(self):
+		self.framework.verbose('[WIKIPEDIA] Searching...', end='\r')
+		payload = {
+			'action': 'query',
+			'list': 'search',
+			'prop': '', 
+			'srsearch': self.q, 
+			'srlimit': self.num, 
+			'utf8': '', 
+			'format': 'json'
+		}
+
+		res = self.wiki_request(payload)
+		if res is None:
+			return 
+
+		res = res.json()
+		results = res['query']['search']
+
+		for result in results:
+			title = result['title']
+			pid = result['pageid']
+			link = 'https://en.wikipedia.org/wiki/' + '_'.join(title.split(' '))
+			self._titles.append(title)
+			self._links.append(link)
+			self._pids.append(pid)
+
+
+	def page(self):
+		self.framework.verbose(f"[WIKIPEDIA] Getting page {self.q}...", end='\r')
+		payload = {
+			'action': 'query', 
+			'pageids': self.q,
+			'prop': 'info|extracts', 
+			'inprop': 'url',  
+			'explaintext': '',
+			'exintro': '',
+			'format': 'json'
+		}
+
+		res = self.wiki_request(payload)
+		if not res:
+			return
+
+		res = res.json()
+		return res['query']['pages'][str(self.q)]
+
+	def wiki_request(self, payload):
+		try:
+			req = self.framework.request(
+					url=self.url,
+					params=payload,
+					headers=self.headers,
+					allow_redirects=False)
+			return req
+		except Exception as e:
+			self.framework.error(f"ConnectionError: {e}", 'util/wikipedia', 'wiki_request')
+			return None
 
 	@property
-	def pages(self):
-		return self._pages
-	
-	@property
 	def links(self):
 		return self._links
 
 	@property
-	def links_with_data(self):
-		for result in self._results:
-			self._links_with_data.append({
-				'title': result.find_all('a')[0].text,
-				'link': result.find_all('a')[0]['href']
-				})
-		
-		return self._links_with_data
-
-	@property
-	def dns(self):
-		return self.framework.page_parse(self._pages).get_dns(self.q)
+	def titles(self):
+		return self._titles
 
 	@property
-	def emails(self):
-		return self.framework.page_parse(self._pages).get_emails(self.q)
+	def pids(self):
+		return self._pids
 
 	@property
-	def docs(self):
-		return self.framework.page_parse(self._pages).get_docs(self.q, self.links)
+	def links_with_title(self):
+		return zip(self._links, self._titles , self._pids)
```

### Comparing `maryam-2.5.1.post3/maryam/core/util/search/zlibrary.py` & `maryam-2.5.2/maryam/core/util/search/zlibrary.py`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/core/web/api.py` & `maryam-2.5.2/maryam/core/web/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,17 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import flask
 from flask import request, jsonify, Response
-from flask_cors import CORS
 
 framework = None
 app = flask.Flask('OWASP Maryam')
-CORS(app)
 
 @app.route('/', methods=['GET', 'POST'])
 def home():
 	page = Response('<pre>current pages:<br>/api/modules => running modules<br>/api/framework => framework commands</pre>', headers={'X-Content-Type-Options': '*'}) 
 	return page
```

### Comparing `maryam-2.5.1.post3/maryam/data/dnsnames.txt` & `maryam-2.5.2/maryam/data/dnsnames.txt`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/data/stopwords.csv` & `maryam-2.5.2/maryam/data/stopwords.csv`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/data/tlds.txt` & `maryam-2.5.2/maryam/data/tlds.txt`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/data/username_checker.json` & `maryam-2.5.2/maryam/data/username_checker.json`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam/data/wapps.json` & `maryam-2.5.2/maryam/data/wapps.json`

 * *Files identical despite different names*

### Comparing `maryam-2.5.1.post3/maryam.egg-info/PKG-INFO` & `maryam-2.5.2/maryam.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maryam
-Version: 2.5.1.post3
+Version: 2.5.2
 Summary: OWASP Maryam is a modular/optional open-source framework based on OSINT and data gathering.
 Home-page: https://github.com/saeeddhqan/Maryam
 Author: Saeed Dehqan
 Author-email: saeed.dehghan@owasp.org
 License: GPL-V3
 Keywords: OWASP,OSINT,search-engine,social-networks,Maryam
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://app.travis-ci.com/saeeddhqan/Maryam.svg?branch=master)](https://app.travis-ci.com/github/saeeddhqan/Maryam)
-![Version 2.5.1](https://img.shields.io/badge/Version-2.5.1-green.svg)
+![Version 2.5.2](https://img.shields.io/badge/Version-2.5.1-green.svg)
 ![GPLv3 License](https://img.shields.io/badge/License-GPLv3-green.svg)
 ![Python 3.10.x](https://img.shields.io/badge/Python-3.10.x-green.svg)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4577/badge)](https://bestpractices.coreinfrastructure.org/projects/4577)
 
 # OWASP Maryam
 
 OWASP Maryam is a modular open-source framework based on OSINT and data gathering. It is designed to provide a robust environment to harvest data from open sources and search engines quickly and thoroughly.
@@ -33,14 +33,18 @@
  - FreeBSD
  - Darwin
  - OSX
 
 ```bash
 $ pip install maryam
 ```
+Alternatively, you can install the latest version with the following command (Recommended):
+```bash
+pip install git+https://github.com/saeeddhqan/maryam.git
+```
 
 # Usage
 
 ```bash
 # Using dns_search. --max means all of resources. --api shows the results as json.
 # .. -t means use multi-threading.
 maryam -e dns_search -d ibm.com -t 5 --max --api --form 
@@ -65,26 +69,26 @@
  - Iris: the first beta version
  - Added famous_person
  - Core speedup optimizations
  - Added setup.py
 
 
 
-
 # Contribution
 
 Contributes are welcome! Here is a start guide: [Development Guide](https://github.com/saeeddhqan/maryam/wiki/Development-Guide)
 You can add a new search engine to the util classes or use the current search engines to write a new module.
 The best help to write a new module is checking the current modules.
 
 # Roadmap
 
+ - Improving Iris page ranking
  - Write a complete metacrawler engine based on OSINT by using the current search engines
  - Add clustering algorithms: Done
- - Web User Interface
+ - Web user interface
 
 # Links
 ### [OWASP](https://owasp.org/www-project-maryam/)
 ### [Wiki](https://github.com/saeeddhqan/maryam/wiki)
 ### [Install](https://github.com/saeeddhqan/maryam/wiki#install)
 ### [Modules Guide](https://github.com/saeeddhqan/maryam/wiki/modules)
 ### [Development Guide](https://github.com/saeeddhqan/maryam/wiki/Development-Guide)
```

### Comparing `maryam-2.5.1.post3/setup.py` & `maryam-2.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from setuptools import setup, find_packages
 
 setup(
 	name='maryam',
-	version='2.5.1-3',
+	version='2.5.2',
 	url='https://github.com/saeeddhqan/Maryam',
 	author='Saeed Dehqan',
 	author_email='saeed.dehghan@owasp.org',
 	packages=find_packages(),
 	include_package_data=True,
 	package_data={"maryam": ['data/*']},
 	license='GPL-V3',
@@ -37,15 +37,14 @@
         'requests',
         'cloudscraper',
         'bs4',
         'lxml',
         'flask',
         'vaderSentiment',
         'plotly',
-        'nltk',
         'matplotlib',
         'pandas',
         'wordcloud',
         'numpy',
         'dask',
         'scikit-learn',
         'scipy',
```

