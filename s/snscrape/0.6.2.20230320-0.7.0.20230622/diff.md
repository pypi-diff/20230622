# Comparing `tmp/snscrape-0.6.2.20230320.tar.gz` & `tmp/snscrape-0.7.0.20230622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/archivebot/snscrape/dist/.tmp-x24ky5vb/snscrape-0.6.2.20230320.tar", last modified: Mon Mar 20 19:56:03 2023, max compression
+gzip compressed data, was "snscrape-0.7.0.20230622.tar", last modified: Thu Jun 22 20:27:08 2023, max compression
```

## Comparing `snscrape-0.6.2.20230320.tar` & `snscrape-0.7.0.20230622.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 archivebot  (1002) archivebot  (1002)        0 2023-03-20 19:56:03.903061 snscrape-0.6.2.20230320/
-drwxr-xr-x   0 archivebot  (1002) archivebot  (1002)        0 2023-03-20 19:56:03.895061 snscrape-0.6.2.20230320/.github/
-drwxr-xr-x   0 archivebot  (1002) archivebot  (1002)        0 2023-03-20 19:56:03.895061 snscrape-0.6.2.20230320/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)     3582 2023-03-20 19:55:44.000000 snscrape-0.6.2.20230320/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)      757 2023-01-13 18:55:40.000000 snscrape-0.6.2.20230320/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)      100 2023-01-13 18:55:40.000000 snscrape-0.6.2.20230320/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)       48 2021-12-08 08:40:41.000000 snscrape-0.6.2.20230320/.gitignore
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)    35149 2021-12-08 08:40:41.000000 snscrape-0.6.2.20230320/LICENSE
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)     4703 2023-03-20 19:56:03.903061 snscrape-0.6.2.20230320/PKG-INFO
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)     4076 2023-03-20 19:55:44.000000 snscrape-0.6.2.20230320/README.md
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)      936 2023-01-13 18:55:40.000000 snscrape-0.6.2.20230320/pyproject.toml
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)       38 2023-03-20 19:56:03.903061 snscrape-0.6.2.20230320/setup.cfg
-drwxr-xr-x   0 archivebot  (1002) archivebot  (1002)        0 2023-03-20 19:56:03.899061 snscrape-0.6.2.20230320/snscrape/
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)        0 2021-12-08 08:40:41.000000 snscrape-0.6.2.20230320/snscrape/__init__.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)    12756 2023-03-03 02:28:47.000000 snscrape-0.6.2.20230320/snscrape/_cli.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)     9083 2023-03-03 02:28:47.000000 snscrape-0.6.2.20230320/snscrape/base.py
-drwxr-xr-x   0 archivebot  (1002) archivebot  (1002)        0 2023-03-20 19:56:03.903061 snscrape-0.6.2.20230320/snscrape/modules/
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)      425 2023-01-13 18:55:40.000000 snscrape-0.6.2.20230320/snscrape/modules/__init__.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)    15972 2023-03-03 02:28:47.000000 snscrape-0.6.2.20230320/snscrape/modules/facebook.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)     9840 2023-03-03 02:28:47.000000 snscrape-0.6.2.20230320/snscrape/modules/instagram.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)    13277 2023-03-03 02:28:47.000000 snscrape-0.6.2.20230320/snscrape/modules/mastodon.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)     9879 2023-01-13 18:55:40.000000 snscrape-0.6.2.20230320/snscrape/modules/reddit.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)     8763 2023-03-03 02:28:47.000000 snscrape-0.6.2.20230320/snscrape/modules/telegram.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)    89949 2023-03-20 19:55:44.000000 snscrape-0.6.2.20230320/snscrape/modules/twitter.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)    17207 2023-03-03 02:28:47.000000 snscrape-0.6.2.20230320/snscrape/modules/vkontakte.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)     5945 2023-03-03 02:28:47.000000 snscrape-0.6.2.20230320/snscrape/modules/weibo.py
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)      155 2021-12-08 08:40:41.000000 snscrape-0.6.2.20230320/snscrape/version.py
-drwxr-xr-x   0 archivebot  (1002) archivebot  (1002)        0 2023-03-20 19:56:03.899061 snscrape-0.6.2.20230320/snscrape.egg-info/
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)     4703 2023-03-20 19:56:03.000000 snscrape-0.6.2.20230320/snscrape.egg-info/PKG-INFO
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)      685 2023-03-20 19:56:03.000000 snscrape-0.6.2.20230320/snscrape.egg-info/SOURCES.txt
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)        1 2023-03-20 19:56:03.000000 snscrape-0.6.2.20230320/snscrape.egg-info/dependency_links.txt
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)       48 2023-03-20 19:56:03.000000 snscrape-0.6.2.20230320/snscrape.egg-info/entry_points.txt
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)       79 2023-03-20 19:56:03.000000 snscrape-0.6.2.20230320/snscrape.egg-info/requires.txt
--rw-r--r--   0 archivebot  (1002) archivebot  (1002)        9 2023-03-20 19:56:03.000000 snscrape-0.6.2.20230320/snscrape.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:27:08.428690 snscrape-0.7.0.20230622/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:27:08.420690 snscrape-0.7.0.20230622/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:27:08.420690 snscrape-0.7.0.20230622/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 root         (0) root         (0)      757 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-06-22 20:27:08.428690 snscrape-0.7.0.20230622/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/README.md
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:27:08.428690 snscrape-0.7.0.20230622/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:27:08.424690 snscrape-0.7.0.20230622/snscrape/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13142 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/_cli.py
+-rw-r--r--   0 root         (0) root         (0)    10495 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:27:08.428690 snscrape-0.7.0.20230622/snscrape/modules/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16004 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/modules/facebook.py
+-rw-r--r--   0 root         (0) root         (0)     9872 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/modules/instagram.py
+-rw-r--r--   0 root         (0) root         (0)    13309 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/modules/mastodon.py
+-rw-r--r--   0 root         (0) root         (0)     9911 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/modules/reddit.py
+-rw-r--r--   0 root         (0) root         (0)     8791 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/modules/telegram.py
+-rw-r--r--   0 root         (0) root         (0)    97065 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/modules/twitter.py
+-rw-r--r--   0 root         (0) root         (0)    17234 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/modules/vkontakte.py
+-rw-r--r--   0 root         (0) root         (0)     5972 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/modules/weibo.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/utils.py
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-22 20:26:58.000000 snscrape-0.7.0.20230622/snscrape/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:27:08.424690 snscrape-0.7.0.20230622/snscrape.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-06-22 20:27:08.000000 snscrape-0.7.0.20230622/snscrape.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-22 20:27:08.000000 snscrape-0.7.0.20230622/snscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:27:08.000000 snscrape-0.7.0.20230622/snscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-22 20:27:08.000000 snscrape-0.7.0.20230622/snscrape.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-22 20:27:08.000000 snscrape-0.7.0.20230622/snscrape.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-22 20:27:08.000000 snscrape-0.7.0.20230622/snscrape.egg-info/top_level.txt
```

### Comparing `snscrape-0.6.2.20230320/.github/ISSUE_TEMPLATE/bug_report.yml` & `snscrape-0.7.0.20230622/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `snscrape-0.6.2.20230320/.github/ISSUE_TEMPLATE/feature_request.yml` & `snscrape-0.7.0.20230622/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `snscrape-0.6.2.20230320/LICENSE` & `snscrape-0.7.0.20230622/LICENSE`

 * *Files identical despite different names*

### Comparing `snscrape-0.6.2.20230320/PKG-INFO` & `snscrape-0.7.0.20230622/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snscrape
-Version: 0.6.2.20230320
+Version: 0.7.0.20230622
 Summary: A social networking service scraper
 Author: JustAnotherArchivist
 Project-URL: repository, https://github.com/JustAnotherArchivist/snscrape
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `snscrape-0.6.2.20230320/README.md` & `snscrape-0.7.0.20230622/README.md`

 * *Files identical despite different names*

### Comparing `snscrape-0.6.2.20230320/pyproject.toml` & `snscrape-0.7.0.20230622/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snscrape-0.6.2.20230320/snscrape/_cli.py` & `snscrape-0.7.0.20230622/snscrape/_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -240,14 +240,15 @@
 	parser.add_argument('--dump-locals', dest = 'dumpLocals', action = 'store_true', default = False, help = 'Dump local variables on serious log messages (warnings or higher)')
 	parser.add_argument('--retry', '--retries', dest = 'retries', type = int, default = 3, metavar = 'N',
 		help = 'When the connection fails or the server returns an unexpected response, retry up to N times with an exponential backoff')
 	parser.add_argument('-n', '--max-results', dest = 'maxResults', type = lambda x: int(x) if int(x) >= 0 else parser.error('--max-results N must be zero or positive'), metavar = 'N', help = 'Only return the first N results')
 	group = parser.add_mutually_exclusive_group(required = False)
 	group.add_argument('-f', '--format', dest = 'format', type = parse_format, default = None, help = 'Output format')
 	group.add_argument('--jsonl', dest = 'jsonl', action = 'store_true', default = False, help = 'Output JSONL')
+	group.add_argument('--jsonl-for-buggy-int-parser', dest = 'jsonlForBuggyIntParser', action = 'store_true', default = False, help = 'Output JSONL and insert extra string fields into objects for integers exceeding double precision limits')
 	parser.add_argument('--with-entity', dest = 'withEntity', action = 'store_true', default = False, help = 'Include the entity (e.g. user, channel) as the first output item')
 	parser.add_argument('--since', type = parse_datetime_arg, metavar = 'DATETIME', help = 'Only return results newer than DATETIME')
 	parser.add_argument('--progress', action = 'store_true', default = False, help = 'Report progress on stderr')
 
 	subparsers = parser.add_subparsers(dest = 'scraper', metavar = 'SCRAPER', title = 'scrapers', required = True)
 	classes = snscrape.base.Scraper.__subclasses__()
 	scrapers = {}
@@ -260,14 +261,16 @@
 		cls._cli_setup_parser(subparser)
 		subparser.set_defaults(cls = cls)
 
 	args = parser.parse_args()
 
 	if not args.withEntity and args.maxResults == 0:
 		parser.error('--max-results 0 is only valid when used with --with-entity')
+	if args.jsonlForBuggyIntParser:
+		args.jsonl = True
 
 	return args
 
 
 def setup_logging():
 	logging.setLoggerClass(Logger)
 	global logger
@@ -307,26 +310,26 @@
 	scraper = args.cls._cli_from_args(args)
 
 	i = 0
 	with _dump_locals_on_exception():
 		try:
 			if args.withEntity and (entity := scraper.entity):
 				if args.jsonl:
-					print(entity.json())
+					print(entity.json(forBuggyIntParser = args.jsonlForBuggyIntParser))
 				else:
 					print(entity)
 			if args.maxResults == 0:
 				logger.info('Exiting after 0 results')
 				return
 			for i, item in enumerate(scraper.get_items(), start = 1):
 				if args.since is not None and item.date < args.since:
 					logger.info(f'Exiting due to reaching older results than {args.since}')
 					break
 				if args.jsonl:
-					print(item.json())
+					print(item.json(forBuggyIntParser = args.jsonlForBuggyIntParser))
 				elif args.format is not None:
 					print(args.format.format(item))
 				else:
 					print(item)
 				if args.progress and i % 100 == 0:
 					print(f'Scraping, {i} results so far', file = sys.stderr)
 				if args.maxResults and i >= args.maxResults:
```

### Comparing `snscrape-0.6.2.20230320/snscrape/base.py` & `snscrape-0.7.0.20230622/snscrape/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-__all__ = ['DeprecatedFeatureWarning', 'IntWithGranularity', 'Item', 'Scraper', 'ScraperException']
+__all__ = ['DeprecatedFeatureWarning', 'Item', 'IntWithGranularity', 'ScraperException', 'EntityUnavailable', 'Scraper']
 
 
 import abc
 import copy
 import dataclasses
 import datetime
+import enum
 import functools
 import json
 import logging
+import random
 import requests
 import requests.adapters
+import snscrape.utils
+import snscrape.version
 import urllib3.connection
 import time
 import warnings
 
 
 _logger = logging.getLogger(__name__)
 
 
-def _module_deprecation_helper(all, **names):
-	def __getattr__(name):
-		if name in names:
-			warnings.warn(f'{name} is deprecated, use {names[name].__name__} instead', DeprecatedFeatureWarning, stacklevel = 2)
-			return names[name]
-		raise AttributeError(f'module {__name__!r} has no attribute {name!r}')
-	def __dir__():
-		return sorted(all + list(names.keys()))
-	return __getattr__, __dir__
-
-
 class DeprecatedFeatureWarning(FutureWarning):
 	pass
 
 
 class _DeprecatedProperty:
 	def __init__(self, name, repl, replStr):
 		self.name = name
@@ -42,65 +35,78 @@
 	def __get__(self, obj, objType):
 		if obj is None: # if the access is through the class using _DeprecatedProperty rather than an instance of the class:
 			return self
 		warnings.warn(f'{self.name} is deprecated, use {self.replStr} instead', DeprecatedFeatureWarning, stacklevel = 2)
 		return self.repl(obj)
 
 
-def _json_serialise_datetime(obj):
-	'''A JSON serialiser that converts datetime.datetime and datetime.date objects to ISO-8601 strings.'''
+def _json_serialise_datetime_enum(obj):
+	'''A JSON serialiser that converts datetime.datetime and datetime.date objects to ISO-8601 strings and enum.Enum objects to their values.'''
 
 	if isinstance(obj, (datetime.datetime, datetime.date)):
 		return obj.isoformat()
+	if isinstance(obj, enum.Enum):
+		return obj.value
 	raise TypeError(f'Object of type {type(obj)} is not JSON serializable')
 
 
-def _json_dataclass_to_dict(obj):
+def _json_dataclass_to_dict(obj, forBuggyIntParser = False):
 	if isinstance(obj, _JSONDataclass) or dataclasses.is_dataclass(obj):
 		out = {}
 		out['_type'] = f'{type(obj).__module__}.{type(obj).__name__}'
 		for field in dataclasses.fields(obj):
 			assert field.name != '_type'
 			if field.name.startswith('_'):
 				continue
-			out[field.name] = _json_dataclass_to_dict(getattr(obj, field.name))
+			out[field.name] = _json_dataclass_to_dict(getattr(obj, field.name), forBuggyIntParser = forBuggyIntParser)
 		# Add properties
 		for k in dir(obj):
 			if isinstance(getattr(type(obj), k, None), (property, _DeprecatedProperty)):
 				assert k != '_type'
 				if k.startswith('_'):
 					continue
-				out[k] = _json_dataclass_to_dict(getattr(obj, k))
-		return out
+				out[k] = _json_dataclass_to_dict(getattr(obj, k), forBuggyIntParser = forBuggyIntParser)
 	elif isinstance(obj, (tuple, list)):
-		return type(obj)(_json_dataclass_to_dict(x) for x in obj)
+		return type(obj)(_json_dataclass_to_dict(x, forBuggyIntParser = forBuggyIntParser) for x in obj)
 	elif isinstance(obj, dict):
-		return {_json_dataclass_to_dict(k): _json_dataclass_to_dict(v) for k, v in obj.items()}
+		out = {_json_dataclass_to_dict(k, forBuggyIntParser = forBuggyIntParser): _json_dataclass_to_dict(v, forBuggyIntParser = forBuggyIntParser) for k, v in obj.items()}
 	elif isinstance(obj, set):
-		return {_json_dataclass_to_dict(v) for v in obj}
+		return {_json_dataclass_to_dict(v, forBuggyIntParser = forBuggyIntParser) for v in obj}
 	else:
 		return copy.deepcopy(obj)
+	# Transform IntWithGranularity and handle buggy int parser output
+	for key, value in list(out.items()): # Modifying the dict below, so make a copy first
+		if isinstance(value, IntWithGranularity):
+			out[key] = int(value)
+			assert f'{key}.granularity' not in out, f'Granularity collision on {key}.granularity'
+			out[f'{key}.granularity'] = value.granularity
+		elif forBuggyIntParser and isinstance(value, int) and abs(value) > 2**53:
+			assert f'{key}.str' not in out, f'Buggy int collision on {key}.str'
+			out[f'{key}.str'] = str(value)
+	return out
 
 
 @dataclasses.dataclass
 class _JSONDataclass:
 	'''A base class for dataclasses for conversion to JSON'''
 
-	def json(self):
-		'''Convert the object to a JSON string'''
+	def json(self, forBuggyIntParser = False):
+		'''
+		Convert the object to a JSON string
+
+		If forBuggyIntParser is True, emit JSON for parsers that can't correctly decode integers exceeding the limits of double-precision IEEE 754 floating point numbers.
+		Specifically, each field x containing an integer with a magnitude above 2**53 results in an additional field x.str with the value as a string.
+		'''
 
 		with warnings.catch_warnings():
 			warnings.filterwarnings(action = 'ignore', category = DeprecatedFeatureWarning)
-			out = _json_dataclass_to_dict(self)
-		for key, value in list(out.items()): # Modifying the dict below, so make a copy first
-			if isinstance(value, IntWithGranularity):
-				out[key] = int(value)
-				assert f'{key}.granularity' not in out, f'Granularity collision on {key}.granularity'
-				out[f'{key}.granularity'] = value.granularity
-		return json.dumps(out, default = _json_serialise_datetime)
+			out = _json_dataclass_to_dict(self, forBuggyIntParser = forBuggyIntParser)
+		assert '_snscrape' not in out, 'Metadata collision on _snscrape'
+		out['_snscrape'] = snscrape.version.__version__
+		return json.dumps(out, default = _json_serialise_datetime_enum)
 
 
 @dataclasses.dataclass
 class Item(_JSONDataclass):
 	'''An abstract base class for an item returned by the scraper.
 
 	An item can really be anything. The string representation should be useful for the CLI output (e.g. a direct URL for the item).
@@ -122,14 +128,24 @@
 		obj.granularity = granularity
 		return obj
 
 	def __reduce__(self):
 		return (IntWithGranularity, (int(self), self.granularity))
 
 
+def _random_user_agent():
+	def lerp(a1, b1, a2, b2, n):
+		return (n - a1) / (b1 - a1) * (b2 - a2) + a2
+	version = int(lerp(datetime.date(2023, 3, 7).toordinal(), datetime.date(2030, 9, 24).toordinal(), 111, 200, datetime.date.today().toordinal()))
+	version += random.randint(-5, 1)
+	version = max(version, 101)
+	return f'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/{version}.0.0.0 Safari/537.36'
+_DEFAULT_USER_AGENT = _random_user_agent()
+
+
 class _HTTPSAdapter(requests.adapters.HTTPAdapter):
 	def init_poolmanager(self, *args, **kwargs):
 		super().init_poolmanager(*args, **kwargs)
 		#FIXME: Uses private urllib3.PoolManager attribute pool_classes_by_scheme.
 		try:
 			self.poolmanager.pool_classes_by_scheme['https'].ConnectionCls = _HTTPSConnection
 		except (AttributeError, KeyError) as e:
@@ -153,14 +169,18 @@
 		return conn
 
 
 class ScraperException(Exception):
 	pass
 
 
+class EntityUnavailable(ScraperException):
+	'''The target entity of the scrape is unavailable, possibly because it does not exist or was suspended.'''
+
+
 class Scraper:
 	'''An abstract base class for a scraper.'''
 
 	name = None
 
 	def __init__(self, *, retries = 3, proxies = None):
 		self._retries = retries
@@ -183,14 +203,18 @@
 		return None
 
 	@functools.cached_property
 	def entity(self):
 		return self._get_entity()
 
 	def _request(self, method, url, params = None, data = None, headers = None, timeout = 10, responseOkCallback = None, allowRedirects = True, proxies = None):
+		if not headers:
+			headers = {}
+		if 'User-Agent' not in headers:
+			headers['User-Agent'] = _DEFAULT_USER_AGENT
 		proxies = proxies or self._proxies or {}
 		errors = []
 		for attempt in range(self._retries + 1):
 			# The request is newly prepared on each retry because of potential cookie updates.
 			req = self._session.prepare_request(requests.Request(method, url, params = params, data = data, headers = headers))
 			environmentSettings = self._session.merge_environment_settings(req.url, proxies, None, None, None)
 			_logger.info(f'Retrieving {req.url}')
@@ -262,18 +286,8 @@
 		return cls._cli_construct(args)
 
 	@classmethod
 	def _cli_construct(cls, argparseArgs, *args, **kwargs):
 		return cls(*args, **kwargs, retries = argparseArgs.retries)
 
 
-def nonempty_string(name):
-	def f(s):
-		s = s.strip()
-		if s:
-			return s
-		raise ValueError('must not be an empty string')
-	f.__name__ = name
-	return f
-
-
-__getattr__, __dir__ = _module_deprecation_helper(__all__, Entity = Item)
+__getattr__, __dir__ = snscrape.utils.module_deprecation_helper(__all__, Entity = Item)
```

### Comparing `snscrape-0.6.2.20230320/snscrape/modules/facebook.py` & `snscrape-0.7.0.20230622/snscrape/modules/facebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import bs4
 import dataclasses
 import datetime
 import json
 import logging
 import re
 import snscrape.base
+import snscrape.utils
 import typing
 import urllib.parse
 
 
 _logger = logging.getLogger(__name__)
 
 
@@ -202,15 +203,15 @@
 			assert response['domops'][0][2] == False
 			assert '__html' in response['domops'][0][3]
 			soup = bs4.BeautifulSoup(response['domops'][0][3]['__html'], 'lxml')
 			yield from self._soup_to_items(soup, self._baseUrl, 'user')
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('username', type = snscrape.base.nonempty_string('username'), help = 'A Facebook username or user ID')
+		subparser.add_argument('username', type = snscrape.utils.nonempty_string_arg('username'), help = 'A Facebook username or user ID')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.username)
 
 
 class FacebookUserScraper(_FacebookUserAndCommunityScraper):
@@ -353,12 +354,12 @@
 				# End of pagination
 				break
 			soup = bs4.BeautifulSoup(obj['payload'], 'lxml')
 			yield from self._soup_to_items(soup, baseUrl, 'group')
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('group', type = snscrape.base.nonempty_string('group'), help = 'A group name or ID')
+		subparser.add_argument('group', type = snscrape.utils.nonempty_string_arg('group'), help = 'A group name or ID')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.group)
```

### Comparing `snscrape-0.6.2.20230320/snscrape/modules/instagram.py` & `snscrape-0.7.0.20230622/snscrape/modules/instagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import dataclasses
 import datetime
 import hashlib
 import json
 import logging
 import re
 import snscrape.base
+import snscrape.utils
 import typing
 
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
@@ -188,15 +189,15 @@
 			followers = followers,
 			following = following,
 			posts = posts,
 		  )
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('username', type = snscrape.base.nonempty_string('username'), help = 'An Instagram username (no leading @)')
+		subparser.add_argument('username', type = snscrape.utils.nonempty_string_arg('username'), help = 'An Instagram username (no leading @)')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.username)
 
 
 class InstagramHashtagScraper(_InstagramCommonScraper):
@@ -210,15 +211,15 @@
 		self._edgeXToMedia = 'edge_hashtag_to_media'
 		self._pageIDKey = 'name'
 		self._queryHash = 'f92f56d47dc7a55b606908374b43a314'
 		self._variablesFormat = '{{"tag_name":"{pageID}","first":50,"after":"{endCursor}"}}'
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('hashtag', type = snscrape.base.nonempty_string('hashtag'), help = 'An Instagram hashtag (no leading #)')
+		subparser.add_argument('hashtag', type = snscrape.utils.nonempty_string_arg('hashtag'), help = 'An Instagram hashtag (no leading #)')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.hashtag)
 
 
 class InstagramLocationScraper(_InstagramCommonScraper):
```

### Comparing `snscrape-0.6.2.20230320/snscrape/modules/mastodon.py` & `snscrape-0.7.0.20230622/snscrape/modules/mastodon.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import bs4
 import dataclasses
 import datetime
 import enum
 import json
 import logging
 import snscrape.base
+import snscrape.utils
 import time
 import typing
 import urllib.parse
 
 
 _logger = logging.getLogger(__name__)
 
@@ -285,15 +286,15 @@
 					nextA = paginationDiv.find('a', class_ = 'next')
 			if not nextA: # End of pagination
 				break
 			url = urllib.parse.urljoin(r.url, nextA['href'])
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('account', type = snscrape.base.nonempty_string('account'), help = 'A Mastodon account. This can be either a URL to the profile page or a string of the form @account@instance.example.org')
+		subparser.add_argument('account', type = snscrape.utils.nonempty_string_arg('account'), help = 'A Mastodon account. This can be either a URL to the profile page or a string of the form @account@instance.example.org')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.account)
 
 
 class MastodonTootScraperMode(enum.Enum):
@@ -329,12 +330,12 @@
 			yield from self._entries_to_items([entry], r.url)
 		elif self._mode is MastodonTootScraperMode.THREAD:
 			yield from self._entries_to_items(soup.find('div', class_ = 'activity-stream').find_all('div', class_ = 'entry'), r.url)
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
 		subparser.add_argument('--thread', action = 'store_true', help = 'Collect thread around the toot referenced by the URL')
-		subparser.add_argument('url', type = snscrape.base.nonempty_string('url'), help = 'A URL for a toot')
+		subparser.add_argument('url', type = snscrape.utils.nonempty_string_arg('url'), help = 'A URL for a toot')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.url, mode = MastodonTootScraperMode._cli_from_args(args))
```

### Comparing `snscrape-0.6.2.20230320/snscrape/modules/reddit.py` & `snscrape-0.7.0.20230622/snscrape/modules/reddit.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 import dataclasses
 import datetime
 import logging
 import re
 import snscrape.base
+import snscrape.utils
 import snscrape.version
 import string
 import time
 import typing
 
 
 _logger = logging.getLogger(__name__)
@@ -220,15 +221,15 @@
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
 		subparser.add_argument('--no-submissions', dest = 'noSubmissions', action = 'store_true', default = False, help = 'Don\'t list submissions')
 		subparser.add_argument('--no-comments', dest = 'noComments', action = 'store_true', default = False, help = 'Don\'t list comments')
 		subparser.add_argument('--before', metavar = 'TIMESTAMP', type = int, help = 'Fetch results before a Unix timestamp')
 		subparser.add_argument('--after', metavar = 'TIMESTAMP', type = int, help = 'Fetch results after a Unix timestamp')
 		name = cls.name.split('-', 1)[1]
-		subparser.add_argument(name, type = snscrape.base.nonempty_string(name))
+		subparser.add_argument(name, type = snscrape.utils.nonempty_string_arg(name))
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		name = cls.name.split('-', 1)[1]
 		return cls._cli_construct(args, getattr(args, name), submissions = not args.noSubmissions, comments = not args.noComments, before = args.before, after = args.after)
 
 
@@ -268,12 +269,12 @@
 		yield self._api_obj_to_item(obj['data'][0])
 
 		# Upstream bug: link_id must be provided in decimal https://old.reddit.com/r/pushshift/comments/zkggt0/update_on_colo_switchover_bug_fixes_reindexing/
 		yield from self._iter_api('https://api.pushshift.io/reddit/search/comment', {'link_id': int(self._submissionId, 36), 'limit': 1000})
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('submissionId', type = snscrape.base.nonempty_string('submissionId'))
+		subparser.add_argument('submissionId', type = snscrape.utils.nonempty_string_arg('submissionId'))
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.submissionId)
```

### Comparing `snscrape-0.6.2.20230320/snscrape/modules/telegram.py` & `snscrape-0.7.0.20230622/snscrape/modules/telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import bs4
 import dataclasses
 import datetime
 import logging
 import re
 import snscrape.base
+import snscrape.utils
 import typing
 import urllib.parse
 
 
 _logger = logging.getLogger(__name__)
 _SINGLE_MEDIA_LINK_PATTERN = re.compile(r'^https://t\.me/[^/]+/\d+\?single$')
 
@@ -148,15 +149,15 @@
 		# /channel has a more accurate member count and bigger profile picture
 		r = self._get(f'https://t.me/{self._name}', headers = self._headers)
 		if r.status_code != 200:
 			raise snscrape.base.ScraperException(f'Got status code {r.status_code}')
 		soup = bs4.BeautifulSoup(r.text, 'lxml')
 		membersDiv = soup.find('div', class_ = 'tgme_page_extra')
 		if membersDiv.text.endswith(' subscribers'):
-			kwargs['members'] = int(membersDiv.text[:-8].replace(' ', ''))
+			kwargs['members'] = int(membersDiv.text[:-12].replace(' ', ''))
 		kwargs['photo'] = soup.find('img', class_ = 'tgme_page_photo_image').attrs['src']
 
 		r, soup = self._initial_page()
 		if '/s/' not in r.url: # Redirect on channels without public posts
 			return
 		channelInfoDiv = soup.find('div', class_ = 'tgme_channel_info')
 		assert channelInfoDiv, 'channel info div not found'
@@ -192,12 +193,12 @@
 			elif type_ in ('photos', 'videos', 'links', 'files'):
 				kwargs[type_] = snscrape.base.IntWithGranularity(value, granularity)
 
 		return Channel(**kwargs)
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('channel', type = snscrape.base.nonempty_string('channel'), help = 'A channel name')
+		subparser.add_argument('channel', type = snscrape.utils.nonempty_string_arg('channel'), help = 'A channel name')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.channel)
```

### Comparing `snscrape-0.6.2.20230320/snscrape/modules/twitter.py` & `snscrape-0.7.0.20230622/snscrape/modules/twitter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,95 @@
 __all__ = [
-	'Tweet', 'Medium', 'Photo', 'VideoVariant', 'Video', 'Gif', 'TextLink', 'Coordinates', 'Place',
-	'User', 'UserLabel',
+	'Tweet',
+	'TextLink',
+	'Medium',
+	'Photo',
+	'VideoVariant',
+	'Video',
+	'Gif',
+	'Coordinates',
+	'Place',
+	'Card',
+	'SummaryCard',
+	'AppCard',
+	'PollCard',
+	'PollOption',
+	'PlayerCard',
+	'PromoConvoCard',
+	'PromoConvoAction',
+	'BroadcastCard',
+	'PeriscopeBroadcastCard',
+	'EventCard',
+	'Event',
+	'NewsletterCard',
+	'NewsletterIssueCard',
+	'AmplifyCard',
+	'AppPlayerCard',
+	'SpacesCard',
+	'MessageMeCard',
+	'UnifiedCard',
+	'UnifiedCardComponentObject',
+	'UnifiedCardDetailComponentObject',
+	'UnifiedCardMediumComponentObject',
+	'UnifiedCardButtonGroupComponentObject',
+	'UnifiedCardButton',
+	'UnifiedCardSwipeableMediaComponentObject',
+	'UnifiedCardSwipeableMediaMedium',
+	'UnifiedCardAppStoreComponentObject',
+	'UnifiedCardTwitterListDetailsComponentObject',
+	'UnifiedCardTwitterCommunityDetailsComponentObject',
+	'UnifiedCardDestination',
+	'UnifiedCardApp',
+	'UnifiedCardSwipeableLayoutSlide',
+	'UnifiedCardCollectionLayoutSlide',
+	'Vibe',
+	'EditState',
+	'ConversationControlPolicy',
+	'TweetRef',
+	'Tombstone',
+	'User',
+	'UserLabel',
+	'UserRef',
+	'ProfileImageShape',
+	'Community',
 	'Trend',
 	'GuestTokenManager',
+	'TwitterSearchScraperMode',
 	'TwitterSearchScraper',
 	'TwitterUserScraper',
 	'TwitterProfileScraper',
 	'TwitterHashtagScraper',
 	'TwitterCashtagScraper',
 	'TwitterTweetScraperMode',
 	'TwitterTweetScraper',
 	'TwitterListPostsScraper',
+	'TwitterCommunityScraper',
 	'TwitterTrendsScraper',
+	'TwitterUsersScraper',
 ]
 
 
 import base64
 import collections
 import copy
 import dataclasses
 import datetime
 import email.utils
 import enum
 import filelock
+import functools
 import itertools
 import json
 import random
 import logging
 import os
 import re
 import requests.adapters
 import snscrape.base
+import snscrape.utils
 import string
 import time
 import typing
 import urllib.parse
 import urllib3.util.ssl_
 import warnings
 
@@ -49,15 +104,15 @@
 @dataclasses.dataclass
 class Tweet(snscrape.base.Item):
 	url: str
 	date: datetime.datetime
 	rawContent: str
 	renderedContent: str
 	id: int
-	user: 'User'
+	user: typing.Union['User', 'UserRef']
 	replyCount: int
 	retweetCount: int
 	likeCount: int
 	quoteCount: int
 	conversationId: int
 	lang: str
 	source: typing.Optional[str] = None
@@ -73,16 +128,20 @@
 	coordinates: typing.Optional['Coordinates'] = None
 	place: typing.Optional['Place'] = None
 	hashtags: typing.Optional[typing.List[str]] = None
 	cashtags: typing.Optional[typing.List[str]] = None
 	card: typing.Optional['Card'] = None
 	viewCount: typing.Optional[int] = None
 	vibe: typing.Optional['Vibe'] = None
+	bookmarkCount: typing.Optional[int] = None
+	pinned: typing.Optional[bool] = None
+	editState: typing.Optional['EditState'] = None
+	conversationControlPolicy: typing.Optional['ConversationControlPolicy'] = None
 
-	username = snscrape.base._DeprecatedProperty('username', lambda self: self.user.username, 'user.username')
+	username = snscrape.base._DeprecatedProperty('username', lambda self: getattr(self.user, 'username', None), 'user.username')
 	outlinks = snscrape.base._DeprecatedProperty('outlinks', lambda self: [x.url for x in self.links] if self.links else [], 'links (url attribute)')
 	outlinksss = snscrape.base._DeprecatedProperty('outlinksss', lambda self: ' '.join(x.url for x in self.links) if self.links else '', 'links (url attribute)')
 	tcooutlinks = snscrape.base._DeprecatedProperty('tcooutlinks', lambda self: [x.tcourl for x in self.links] if self.links else [], 'links (tcourl attribute)')
 	tcooutlinksss = snscrape.base._DeprecatedProperty('tcooutlinksss', lambda self: ' '.join(x.tcourl for x in self.links) if self.links else '', 'links (tcourl attribute)')
 	content = snscrape.base._DeprecatedProperty('content', lambda self: self.rawContent, 'rawContent')
 
 	def __str__(self):
@@ -432,14 +491,38 @@
 class Vibe:
 	text: str
 	imageUrl: str
 	imageDescription: str
 
 
 @dataclasses.dataclass
+class EditState:
+	editTweetIds: typing.List[int]
+	editableUntilDate: datetime.datetime
+	editsRemaining: int
+
+
+class ConversationControlPolicy(enum.Enum):
+	EVERYONE = 'everyone'
+	MENTIONED = 'mentioned'
+	FOLLOWERS = 'followers'
+
+	@classmethod
+	def _from_policy(cls, policy):
+		if policy is None:
+			return cls.EVERYONE
+		elif policy == 'ByInvitation':
+			return cls.MENTIONED
+		elif policy == 'Community':
+			return cls.FOLLOWERS
+		_logger.warning(f'Unknown conversation control policy {policy!r}')
+		return None
+
+
+@dataclasses.dataclass
 class TweetRef(snscrape.base.Item):
 	'''A reference to a tweet for which no proper Tweet object could be produced from the data returned by Twitter'''
 
 	id: int
 
 	def __str__(self):
 		return f'https://twitter.com/i/web/status/{self.id}'
@@ -477,14 +560,17 @@
 	mediaCount: typing.Optional[int] = None
 	location: typing.Optional[str] = None
 	protected: typing.Optional[bool] = None
 	link: typing.Optional[TextLink] = None
 	profileImageUrl: typing.Optional[str] = None
 	profileBannerUrl: typing.Optional[str] = None
 	label: typing.Optional['UserLabel'] = None
+	blue: typing.Optional[bool] = None
+	blueType: typing.Optional[str] = None
+	profileImageShape: typing.Optional['ProfileImageShape'] = None
 
 	descriptionUrls = snscrape.base._DeprecatedProperty('descriptionUrls', lambda self: self.descriptionLinks, 'descriptionLinks')
 	linkUrl = snscrape.base._DeprecatedProperty('linkUrl', lambda self: self.link.url if self.link else None, 'link.url')
 	linkTcourl = snscrape.base._DeprecatedProperty('linkTcourl', lambda self: self.link.tcourl if self.link else None, 'link.tcourl')
 	description = snscrape.base._DeprecatedProperty('description', lambda self: self.renderedDescription, 'renderedDescription')
 
 	@property
@@ -509,14 +595,31 @@
 	text: typing.Optional[str] = None
 	textLinks: typing.Optional[typing.List[TextLink]] = None
 
 	def __str__(self):
 		return f'https://twitter.com/i/user/{self.id}'
 
 
+class ProfileImageShape(enum.Enum):
+	CIRCLE = 'circle'
+	HEXAGON = 'hexagon'
+	SQUARE = 'square'
+
+	@classmethod
+	def _from_twitter_string(cls, s):
+		if s == 'Circle':
+			return cls.CIRCLE
+		elif s == 'Hexagon':
+			return cls.HEXAGON
+		elif s == 'Square':
+			return cls.SQUARE
+		_logger.warning(f'Unknown profile picture shape {s!r}')
+		return None
+
+
 @dataclasses.dataclass
 class Community(snscrape.base.Item):
 	id: int
 	name: str
 	created: datetime.datetime
 	admin: typing.Union[User, UserRef]
 	creator: typing.Union[User, UserRef]
@@ -559,22 +662,23 @@
 		self._token = token
 		self._setTime = time.time()
 
 	@property
 	def setTime(self):
 		return self._setTime
 
-	def reset(self):
+	def reset(self, *, blockUntil = None):
 		self._token = None
 		self._setTime = 0.0
 
 
 class _CLIGuestTokenManager(GuestTokenManager):
 	def __init__(self):
 		super().__init__()
+		self._blockedUntil = 0
 		cacheHome = os.environ.get('XDG_CACHE_HOME')
 		if not cacheHome or not os.path.isabs(cacheHome):
 			# This should be ${HOME}/.cache, but the HOME environment variable may not exist on non-POSIX-compliant systems.
 			# On POSIX-compliant systems, the XDG Base Directory specification is followed exactly since ~ expands to $HOME if it is present.
 			cacheHome = os.path.join(os.path.expanduser('~'), '.cache')
 		dir = os.path.join(cacheHome, 'snscrape')
 		if not os.path.isdir(dir):
@@ -582,37 +686,82 @@
 			# This ensures that the XDG_CACHE_HOME is created with the right permissions.
 			os.makedirs(os.path.dirname(dir), mode = 0o700, exist_ok = True)
 			os.mkdir(dir, mode = 0o700)
 		self._file = os.path.join(dir, 'cli-twitter-guest-token.json')
 		self._lockFile = f'{self._file}.lock'
 		self._lock = filelock.FileLock(self._lockFile)
 
+	def _locked_load(self):
+		if not os.path.exists(self._file):
+			return None
+		_logger.info(f'Reading guest token file {self._file}')
+		with open(self._file, 'r') as fp:
+			try:
+				o = json.load(fp)
+			except json.JSONDecodeError as e:
+				_logger.warning(f'Malformed guest token file {self._file}: {e!s}')
+				self._locked_delete()
+				return None
+		if o.get('version') != 1:
+			_logger.warning(f'Outdated version of guest token file {self._file}')
+			self._locked_delete()
+			return None
+		return o
+
 	def _read(self):
 		with self._lock:
-			if not os.path.exists(self._file):
-				return None
-			_logger.info(f'Reading guest token from {self._file}')
-			with open(self._file, 'r') as fp:
-				try:
-					o = json.load(fp)
-				except json.JSONDecodeError as e:
-					_logger.warning(f'Malformed guest token file {self._file}: {e!s}')
-					self.reset()
-					return None
-		self._token = o['token']
-		self._setTime = o['setTime']
-		if self._setTime < time.time() - _GUEST_TOKEN_VALIDITY:
-			_logger.info('Guest token expired')
+			o = self._locked_load()
+		if not o:
 			self.reset()
+			return None
+		# Select a random non-blocked valid token if there is one
+		currentTime = time.time()
+		setTimeThreshold = currentTime - _GUEST_TOKEN_VALIDITY
+		validTokens = [token for token, t in o['tokens'].items() if t['setTime'] >= setTimeThreshold and t.get('blockedUntil', 0) < currentTime]
+		if not validTokens:
+			return None
+		token = random.choice(validTokens)
+		self._token = token
+		self._setTime = o['tokens'][token]['setTime']
+		self._blockedUntil = 0
 
 	def _write(self):
 		with self._lock:
-			_logger.info(f'Writing guest token to {self._file}')
-			with open(self._file, 'w') as fp:
-				json.dump({'token': self.token, 'setTime': self.setTime}, fp)
+			# Read existing file
+			o = self._locked_load()
+			if not o:
+				o = {'version': 1, 'tokens': {}}
+
+			# Remove expired tokens
+			setTimeThreshold = time.time() - _GUEST_TOKEN_VALIDITY
+			o['tokens'] = {token: details for token, details in o['tokens'].items() if details['setTime'] >= setTimeThreshold}
+
+			# Insert or update current token
+			if self._token:
+				if self._token not in o['tokens']:
+					o['tokens'][self._token] = {}
+				o['tokens'][self._token]['setTime'] = self._setTime
+				if self._blockedUntil:
+					o['tokens'][self._token]['blockedUntil'] = self._blockedUntil
+
+			# Write back out if there are any tokens, else delete
+			if o['tokens']:
+				_logger.info(f'Writing guest token file {self._file}')
+				with open(self._file, 'w') as fp:
+					json.dump(o, fp)
+			else:
+				self._locked_delete()
+
+	def _locked_delete(self):
+		_logger.info(f'Deleting guest token file {self._file}')
+		try:
+			os.remove(self._file)
+		except FileNotFoundError:
+			# Another process likely already removed the file
+			pass
 
 	@property
 	def token(self):
 		if not self._token:
 			self._read()
 		return self._token
 
@@ -622,23 +771,19 @@
 		self._write()
 
 	@property
 	def setTime(self):
 		self.token  # Implicitly reads from the file if necessary
 		return self._setTime
 
-	def reset(self):
+	def reset(self, *, blockUntil = None):
+		self._blockedUntil = blockUntil
+		self._write()
 		super().reset()
-		with self._lock:
-			_logger.info(f'Deleting guest token file {self._file}')
-			try:
-				os.remove(self._file)
-			except FileNotFoundError:
-				# Another process likely already removed the file
-				pass
+		self._blockedUntil = 0
 
 
 class _TwitterTLSAdapter(snscrape.base._HTTPSAdapter):
 	def init_poolmanager(self, *args, **kwargs):
 		#FIXME: When urllib3 2.0.0 is out and can be required, this should use urllib3.util.create_urllib3_context instead of the private, undocumented ssl_ module.
 		kwargs['ssl_context'] = urllib3.util.ssl_.create_urllib3_context(ciphers = _CIPHERS_CHROME)
 		super().init_poolmanager(*args, **kwargs)
@@ -657,38 +802,31 @@
 			global _globalGuestTokenManager
 			if _globalGuestTokenManager is None:
 				_globalGuestTokenManager = GuestTokenManager()
 			guestTokenManager = _globalGuestTokenManager
 		self._guestTokenManager = guestTokenManager
 		self._maxEmptyPages = maxEmptyPages
 		self._apiHeaders = {
-			'User-Agent': None,
 			'Authorization': _API_AUTHORIZATION_HEADER,
 			'Referer': self._baseUrl,
 			'Accept-Language': 'en-US,en;q=0.5',
 		}
 		adapter = _TwitterTLSAdapter()
 		self._session.mount('https://twitter.com', adapter)
 		self._session.mount('https://api.twitter.com', adapter)
-		self._set_random_user_agent()
-
-	def _set_random_user_agent(self):
-		self._userAgent = f'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.5563.{random.randint(0, 9999)} Safari/537.{random.randint(0, 99)}'
-		self._apiHeaders['User-Agent'] = self._userAgent
 
 	def _check_guest_token_response(self, r):
 		if r.status_code != 200:
-			self._set_random_user_agent()
 			return False, ('non-200 response' if r.status_code != 404 else 'blocked') + f' ({r.status_code})'
 		return True, None
 
 	def _ensure_guest_token(self, url = None):
 		if self._guestTokenManager.token is None:
 			_logger.info('Retrieving guest token')
-			r = self._get(self._baseUrl if url is None else url, headers = {'User-Agent': self._userAgent}, responseOkCallback = self._check_guest_token_response)
+			r = self._get(self._baseUrl if url is None else url, responseOkCallback = self._check_guest_token_response)
 			if (match := re.search(r'document\.cookie = decodeURIComponent\("gt=(\d+); Max-Age=10800; Domain=\.twitter\.com; Path=/; Secure"\);', r.text)):
 				_logger.debug('Found guest token in HTML')
 				self._guestTokenManager.token = match.group(1)
 			if 'gt' in r.cookies:
 				_logger.debug('Found guest token in cookies')
 				self._guestTokenManager.token = r.cookies['gt']
 			if not self._guestTokenManager.token:
@@ -700,106 +838,114 @@
 					raise snscrape.base.ScraperException('Unable to retrieve guest token')
 				self._guestTokenManager.token = o['guest_token']
 			assert self._guestTokenManager.token
 		_logger.debug(f'Using guest token {self._guestTokenManager.token}')
 		self._session.cookies.set('gt', self._guestTokenManager.token, domain = '.twitter.com', path = '/', secure = True, expires = self._guestTokenManager.setTime + _GUEST_TOKEN_VALIDITY)
 		self._apiHeaders['x-guest-token'] = self._guestTokenManager.token
 
-	def _unset_guest_token(self):
-		self._guestTokenManager.reset()
+	def _unset_guest_token(self, blockUntil):
+		self._guestTokenManager.reset(blockUntil = blockUntil)
 		del self._session.cookies['gt']
 		del self._apiHeaders['x-guest-token']
 
-	def _check_api_response(self, r):
+	def _check_api_response(self, r, apiType, instructionsPath):
 		if r.status_code in (403, 404, 429):
-			self._unset_guest_token()
+			if r.status_code == 429 and r.headers.get('x-rate-limit-remaining', '') == '0' and 'x-rate-limit-reset' in r.headers:
+				blockUntil = min(int(r.headers['x-rate-limit-reset']), int(time.time()) + 900)
+			else:
+				blockUntil = int(time.time()) + 300
+			self._unset_guest_token(blockUntil)
 			self._ensure_guest_token()
 			return False, f'blocked ({r.status_code})'
 		if r.headers.get('content-type', '').replace(' ', '') != 'application/json;charset=utf-8':
 			return False, 'content type is not JSON'
 		if r.status_code != 200:
 			return False, f'non-200 status code ({r.status_code})'
+		try:
+			obj = r.json()
+		except json.JSONDecodeError as e:
+			return False, f'received invalid JSON from Twitter ({e})'
+		# Pass the already-parsed object outwards so it doesn't need to be decoded twice.
+		r._snscrapeObj = obj
+		if apiType is _TwitterAPIType.GRAPHQL and 'errors' in obj:
+			msg = 'Twitter responded with an error: ' + ', '.join(f'{e["name"]}: {e["message"]}' for e in obj['errors'])
+			instructions = obj
+			for k in instructionsPath:
+				instructions = instructions.get(k, {})
+			if instructions:
+				# Emit a warning if there are instructions since it could indicate incomplete data
+				_logger.warn(msg)
+				return True, None
+			else:
+				return False, msg
 		return True, None
 
-	def _get_api_data(self, endpoint, apiType, params):
+	def _get_api_data(self, endpoint, apiType, params, instructionsPath = None):
 		self._ensure_guest_token()
 		if apiType is _TwitterAPIType.GRAPHQL:
 			params = urllib.parse.urlencode({k: json.dumps(v, separators = (',', ':')) for k, v in params.items()}, quote_via = urllib.parse.quote)
-		r = self._get(endpoint, params = params, headers = self._apiHeaders, responseOkCallback = self._check_api_response)
-		try:
-			obj = r.json()
-		except json.JSONDecodeError as e:
-			raise snscrape.base.ScraperException('Received invalid JSON from Twitter') from e
-		return obj
+		r = self._get(endpoint, params = params, headers = self._apiHeaders, responseOkCallback = functools.partial(self._check_api_response, apiType = apiType, instructionsPath = instructionsPath))
+		return r._snscrapeObj
 
-	def _iter_api_data(self, endpoint, apiType, params, paginationParams = None, cursor = None, direction = _ScrollDirection.BOTTOM):
+	def _iter_api_data(self, endpoint, apiType, params, paginationParams = None, cursor = None, direction = _ScrollDirection.BOTTOM, instructionsPath = None):
 		# Iterate over endpoint with params/paginationParams, optionally starting from a cursor
 		# Handles guest token extraction using the baseUrl passed to __init__ etc.
 		# Order from params and paginationParams is preserved. To insert the cursor at a particular location, insert a 'cursor' key into paginationParams there (value is overwritten).
 		# direction controls in which direction it should scroll from the initial response. BOTH equals TOP followed by BOTTOM.
+		# instructionsPath must be present if apiType is GRAPHQL.
 
 		# Logic for dual scrolling: direction is set to top, but if the bottom cursor is found, bottomCursorAndStop is set accordingly.
 		# Once the top pagination is exhausted, the bottomCursorAndStop is used and reset to None; it isn't set anymore after because the first entry condition will always be true for the bottom cursor.
 
+		assert apiType is _TwitterAPIType.GRAPHQL
 		if cursor is None:
 			reqParams = params
 		else:
 			reqParams = copy.deepcopy(paginationParams)
-			if apiType is _TwitterAPIType.V2:
-				reqParams['cursor'] = cursor
-			else:
-				reqParams['variables']['cursor'] = cursor
+			reqParams['variables']['cursor'] = cursor
 		bottomCursorAndStop = None
 		if direction is _ScrollDirection.TOP or direction is _ScrollDirection.BOTH:
 			dir = 'top'
 		else:
 			dir = 'bottom'
 		stopOnEmptyResponse = False
 		emptyResponsesOnCursor = 0
 		emptyPages = 0
 		while True:
 			_logger.info(f'Retrieving scroll page {cursor}')
-			obj = self._get_api_data(endpoint, apiType, reqParams)
+			obj = self._get_api_data(endpoint, apiType, reqParams, instructionsPath = instructionsPath)
 			yield obj
 
 			# No data format test, just a hard and loud crash if anything's wrong :-)
 			newCursor = None
 			promptCursor = None
 			newBottomCursorAndStop = None
-			if apiType is _TwitterAPIType.V2:
-				instructions = obj['timeline']['instructions']
-			elif apiType is _TwitterAPIType.GRAPHQL:
-				if 'user' in obj['data']:
-					# UserTweets, UserTweetsAndReplies
-					instructions = obj['data']['user']['result']['timeline_v2']['timeline']['instructions']
-				else:
-					# TweetDetail
-					instructions = obj['data'].get('threaded_conversation_with_injections_v2', {}).get('instructions', [])
+			instructions = obj
+			for k in instructionsPath:
+				instructions = instructions[k]
 			entryCount = 0
 			for instruction in instructions:
 				if 'addEntries' in instruction:
 					entries = instruction['addEntries']['entries']
 				elif 'replaceEntry' in instruction:
 					entries = [instruction['replaceEntry']['entry']]
 				elif instruction.get('type') == 'TimelineAddEntries':
 					entries = instruction['entries']
+				elif instruction.get('type') == 'TimelineReplaceEntry':
+					entries = [instruction['entry']]
 				else:
 					continue
 				entryCount += self._count_tweets_and_users(entries)
 				for entry in entries:
 					if not (entry['entryId'].startswith('sq-cursor-') or entry['entryId'].startswith('cursor-')):
 						continue
-					if apiType is _TwitterAPIType.V2:
-						entryCursor = entry['content']['operation']['cursor']['value']
-						entryCursorStop = entry['content']['operation']['cursor'].get('stopOnEmptyResponse', None)
-					elif apiType is _TwitterAPIType.GRAPHQL:
-						cursorContent = entry['content']
-						while cursorContent.get('itemType') == 'TimelineTimelineItem' or cursorContent.get('entryType') == 'TimelineTimelineItem':
-							cursorContent = cursorContent['itemContent']
-						entryCursor, entryCursorStop = cursorContent['value'], cursorContent.get('stopOnEmptyResponse', None)
+					cursorContent = entry['content']
+					while cursorContent.get('itemType') == 'TimelineTimelineItem' or cursorContent.get('entryType') == 'TimelineTimelineItem':
+						cursorContent = cursorContent['itemContent']
+					entryCursor, entryCursorStop = cursorContent['value'], cursorContent.get('stopOnEmptyResponse', None)
 					if entry['entryId'] == f'sq-cursor-{dir}' or entry['entryId'].startswith(f'cursor-{dir}-'):
 						newCursor = entryCursor
 						if entryCursorStop is not None:
 							stopOnEmptyResponse = entryCursorStop
 					elif entry['entryId'].startswith('cursor-showmorethreadsprompt-') or entry['entryId'].startswith('cursor-showmorethreads-'):
 						# E.g. 'offensive' replies and 'Show more replies' button
 						promptCursor = entryCursor
@@ -830,67 +976,45 @@
 					bottomCursorAndStop = None
 				else:
 					break
 			if newCursor != cursor:
 				emptyResponsesOnCursor = 0
 			cursor = newCursor
 			reqParams = copy.deepcopy(paginationParams)
-			if apiType is _TwitterAPIType.V2:
-				reqParams['cursor'] = cursor
-			else:
-				reqParams['variables']['cursor'] = cursor
+			reqParams['variables']['cursor'] = cursor
 
 	def _count_tweets_and_users(self, entries):
 		return sum(entry['entryId'].startswith('sq-I-t-') or entry['entryId'].startswith('tweet-') or entry['entryId'].startswith('user-') for entry in entries)
 
-	def _v2_timeline_instructions_to_tweets_or_users(self, obj):
-		# No data format test, just a hard and loud crash if anything's wrong :-)
-		for instruction in obj['timeline']['instructions']:
-			if 'addEntries' in instruction:
-				entries = instruction['addEntries']['entries']
-			elif 'replaceEntry' in instruction:
-				entries = [instruction['replaceEntry']['entry']]
-			else:
-				continue
-			for entry in entries:
-				if entry['entryId'].startswith('sq-I-t-') or entry['entryId'].startswith('tweet-'):
-					yield from self._v2_instruction_tweet_entry_to_tweet(entry['entryId'], entry['content'], obj)
-				elif entry['entryId'].startswith('user-'):
-					yield self._user_to_user(obj['globalObjects']['users'][entry['content']['item']['content']['user']['id']])
-
-	def _v2_instruction_tweet_entry_to_tweet(self, entryId, entry, obj):
-		if 'tweet' in entry['item']['content']:
-			if 'promotedMetadata' in entry['item']['content']['tweet']: # Promoted tweet aka ads
-				return
-			if entry['item']['content']['tweet']['id'] not in obj['globalObjects']['tweets']:
-				_logger.warning(f'Skipping tweet {entry["item"]["content"]["tweet"]["id"]} which is not in globalObjects')
-				return
-			tweet = obj['globalObjects']['tweets'][entry['item']['content']['tweet']['id']]
-		else:
-			raise snscrape.base.ScraperException(f'Unable to handle entry {entryId!r}')
-		yield self._tweet_to_tweet(tweet, obj)
-
 	def _get_tweet_id(self, tweet):
 		return tweet['id'] if 'id' in tweet else int(tweet['id_str'])
 
-	def _make_tweet(self, tweet, user, retweetedTweet = None, quotedTweet = None, card = None, **kwargs):
+	def _make_tweet(self, tweet, user, retweetedTweet = None, quotedTweet = None, card = None, noteTweet = None, **kwargs):
 		tweetId = self._get_tweet_id(tweet)
 		kwargs['id'] = tweetId
-		kwargs['rawContent'] = tweet['full_text']
-		kwargs['renderedContent'] = self._render_text_with_urls(tweet['full_text'], tweet['entities'].get('urls'))
+		if noteTweet and 'text' in noteTweet:
+			kwargs['rawContent'] = noteTweet['text']
+			entities = noteTweet['entity_set']
+		else:
+			if noteTweet:
+				_logger.warning(f'Twitter returned an empty note tweet in tweet {tweetId}; text and entities might be incomplete')
+			kwargs['rawContent'] = tweet['full_text']
+			entities = tweet['entities']
+		links = entities.get('urls')
+		kwargs['renderedContent'] = self._render_text_with_urls(kwargs['rawContent'], links)
 		kwargs['user'] = user
 		kwargs['date'] = email.utils.parsedate_to_datetime(tweet['created_at'])
-		if tweet['entities'].get('urls'):
+		if links:
 			kwargs['links'] = [TextLink(
 			                     text = u.get('display_url'),
 			                     url = u['expanded_url'],
 			                     tcourl = u['url'],
 			                     indices = tuple(u['indices']),
-			                   ) for u in tweet['entities']['urls']]
-		kwargs['url'] = f'https://twitter.com/{user.username}/status/{tweetId}'
+			                   ) for u in links]
+		kwargs['url'] = f'https://twitter.com/{getattr(user, "username", "i/web")}/status/{tweetId}'
 		kwargs['replyCount'] = tweet['reply_count']
 		kwargs['retweetCount'] = tweet['retweet_count']
 		kwargs['likeCount'] = tweet['favorite_count']
 		kwargs['quoteCount'] = tweet['quote_count']
 		kwargs['conversationId'] = tweet['conversation_id'] if 'conversation_id' in tweet else int(tweet['conversation_id_str'])
 		kwargs['lang'] = tweet['lang']
 		if 'source' in tweet:
@@ -911,22 +1035,22 @@
 		if quotedTweet:
 			kwargs['quotedTweet'] = quotedTweet
 		if (inReplyToTweetId := tweet.get('in_reply_to_status_id_str')):
 			kwargs['inReplyToTweetId'] = int(inReplyToTweetId)
 			inReplyToUserId = int(tweet['in_reply_to_user_id_str'])
 			if inReplyToUserId == kwargs['user'].id:
 				kwargs['inReplyToUser'] = kwargs['user']
-			elif tweet['entities'].get('user_mentions'):
-				for u in tweet['entities']['user_mentions']:
+			elif entities.get('user_mentions'):
+				for u in entities['user_mentions']:
 					if u['id_str'] == tweet['in_reply_to_user_id_str']:
 						kwargs['inReplyToUser'] = User(username = u['screen_name'], id = u['id'] if 'id' in u else int(u['id_str']), displayname = u['name'])
 			if 'inReplyToUser' not in kwargs:
 				kwargs['inReplyToUser'] = User(username = tweet['in_reply_to_screen_name'], id = inReplyToUserId)
-		if tweet['entities'].get('user_mentions'):
-			kwargs['mentionedUsers'] = [User(username = u['screen_name'], id = u['id'] if 'id' in u else int(u['id_str']), displayname = u['name']) for u in tweet['entities']['user_mentions']]
+		if entities.get('user_mentions'):
+			kwargs['mentionedUsers'] = [User(username = u['screen_name'], id = u['id'] if 'id' in u else int(u['id_str']), displayname = u['name']) for u in entities['user_mentions']]
 
 		# https://developer.twitter.com/en/docs/tutorials/filtering-tweets-by-location
 		if tweet.get('coordinates'):
 			# coordinates root key (if present) presents coordinates in the form [LONGITUDE, LATITUDE]
 			if (coords := tweet['coordinates']['coordinates']) and len(coords) == 2:
 				kwargs['coordinates'] = Coordinates(coords[0], coords[1])
 		elif tweet.get('geo'):
@@ -934,18 +1058,18 @@
 			if (coords := tweet['geo']['coordinates']) and len(coords) == 2:
 				kwargs['coordinates'] = Coordinates(coords[1], coords[0])
 		if tweet.get('place'):
 			kwargs['place'] = Place(tweet['place']['id'], tweet['place']['full_name'], tweet['place']['name'], tweet['place']['place_type'], tweet['place']['country'], tweet['place']['country_code'])
 			if 'coordinates' not in kwargs and tweet['place'].get('bounding_box') and (coords := tweet['place']['bounding_box']['coordinates']) and coords[0] and len(coords[0][0]) == 2:
 				# Take the first (longitude, latitude) couple of the "place square"
 				kwargs['coordinates'] = Coordinates(coords[0][0][0], coords[0][0][1])
-		if tweet['entities'].get('hashtags'):
-			kwargs['hashtags'] = [o['text'] for o in tweet['entities']['hashtags']]
-		if tweet['entities'].get('symbols'):
-			kwargs['cashtags'] = [o['text'] for o in tweet['entities']['symbols']]
+		if entities.get('hashtags'):
+			kwargs['hashtags'] = [o['text'] for o in entities['hashtags']]
+		if entities.get('symbols'):
+			kwargs['cashtags'] = [o['text'] for o in entities['symbols']]
 		if card:
 			kwargs['card'] = card
 			if hasattr(card, 'url') and '//t.co/' in card.url:
 				# Try to convert the URL to the non-shortened/t.co one
 				# Retweets inherit the card but not the outlinks; try to get them from the retweeted tweet instead in that case.
 				candidates = []
 				if 'links' in kwargs:
@@ -954,14 +1078,17 @@
 					candidates.extend(retweetedTweet.links)
 				for u in candidates:
 					if u.tcourl == card.url:
 						card.url = u.url
 						break
 				else:
 					_logger.warning(f'Could not translate t.co card URL on tweet {tweetId}')
+		if 'bookmark_count' in tweet:
+			kwargs['bookmarkCount'] = tweet['bookmark_count']
+		kwargs['conversationControlPolicy'] = ConversationControlPolicy._from_policy(tweet.get('conversation_control', {'policy': None})['policy'])
 		return Tweet(**kwargs)
 
 	def _make_medium(self, medium, tweetId):
 		if medium['type'] == 'photo':
 			if '?format=' in medium['media_url_https'] or '&format=' in medium['media_url_https']:
 				return Photo(previewUrl = medium['media_url_https'], fullUrl = medium['media_url_https'])
 			if '.' not in medium['media_url_https']:
@@ -1000,48 +1127,30 @@
 			return cls(**mKwargs)
 		else:
 			_logger.warning(f'Unsupported medium type on tweet {tweetId}: {medium["type"]!r}')
 
 	def _make_card(self, card, apiType, tweetId):
 		bindingValues = {}
 
-		def _kwargs_from_map(keyKwargMap):
-			nonlocal bindingValues
-			return {kwarg: bindingValues[key] for key, kwarg in keyKwargMap.items() if key in bindingValues}
-
 		userRefs = {}
-		if apiType is _TwitterAPIType.V2:
-			for o in card.get('users', {}).values():
-				userId = o['id']
-				assert userId not in userRefs
-				userRefs[userId] = self._user_to_user(o)
-		elif apiType is _TwitterAPIType.GRAPHQL:
-			for o in card['legacy'].get('user_refs_results', []):
-				if 'result' not in o:
-					_logger.warning(f'Empty user ref object in card on tweet {tweetId}')
-					continue
-				o = o['result']
-				if o['__typename'] == 'UserUnavailable':
-					_logger.warning(f'Unavailable user in card on tweet {tweetId}')
-					continue
-				userId = int(o['rest_id'])
-				if 'legacy' in o:
-					user = self._user_to_user(o['legacy'], id_ = userId)
-				else:
-					user = UserRef(id = userId)
-				if userId in userRefs:
-					if userRefs[userId] != user:
-						_logger.warning(f'Duplicate user {userId} with differing data in card on tweet {tweetId}')
-					continue
-				userRefs[userId] = user
+		for o in card['legacy'].get('user_refs_results', []):
+			if 'result' not in o:
+				_logger.warning(f'Empty user ref object in card on tweet {tweetId}')
+				continue
+			user = self._graphql_user_results_to_user(o)
+			if isinstance(user, UserRef) or user is None:
+				_logger.warning(f'Unavailable user in card on tweet {tweetId}')
+				continue
+			if user.id in userRefs:
+				if userRefs[user.id] != user:
+					_logger.warning(f'Duplicate user {user.id} with differing data in card on tweet {tweetId}')
+				continue
+			userRefs[user.id] = user
 
-		if apiType is _TwitterAPIType.V2:
-			messyBindingValues = card['binding_values'].items()
-		elif apiType is _TwitterAPIType.GRAPHQL:
-			messyBindingValues = ((x['key'], x['value']) for x in card['legacy']['binding_values'])
+		messyBindingValues = ((x['key'], x['value']) for x in card['legacy']['binding_values'])
 		for key, value in messyBindingValues:
 			if 'type' not in value:
 				# Silently ignore creator/site entries since they frequently appear like this.
 				if key not in ('creator', 'site'):
 					_logger.warning(f'Skipping type-less card value {key!r} on tweet {tweetId}')
 				continue
 			if value['type'] == 'STRING':
@@ -1059,35 +1168,32 @@
 				userId = int(value['user_value']['id_str'])
 				bindingValues[key] = userRefs.get(userId)
 				if bindingValues[key] is None:
 					_logger.warning(f'User {userId} not found in user refs in card on tweet {tweetId}')
 			else:
 				_logger.warning(f'Unsupported card value type on {key!r} on tweet {tweetId}: {value["type"]!r}')
 
-		if apiType is _TwitterAPIType.V2:
-			cardName = card['name']
-		elif apiType is _TwitterAPIType.GRAPHQL:
-			cardName = card['legacy']['name']
+		cardName = card['legacy']['name']
 
 		if cardName in ('summary', 'summary_large_image', 'app', 'direct_store_link_app'):
-			keyKwargMap = {
+			keyMap = {
 				'title': 'title',
 				'description': 'description',
 				'card_url': 'url',
 				'site': 'siteUser',
 				'creator': 'creatorUser',
 			}
 			if cardName in ('app', 'direct_store_link_app'):
-				keyKwargMap['thumbnail_original'] = 'thumbnailUrl'
-				return AppCard(**_kwargs_from_map(keyKwargMap))
+				keyMap['thumbnail_original'] = 'thumbnailUrl'
+				return AppCard(**snscrape.utils.dict_map(bindingValues, keyMap))
 			else:
-				keyKwargMap['thumbnail_image_original'] = 'thumbnailUrl'
-				return SummaryCard(**_kwargs_from_map(keyKwargMap))
+				keyMap['thumbnail_image_original'] = 'thumbnailUrl'
+				return SummaryCard(**snscrape.utils.dict_map(bindingValues, keyMap))
 		elif any(cardName.startswith(x) for x in ('poll2choice_', 'poll3choice_', 'poll4choice_')) and cardName.split('_', 1)[1] in ('text_only', 'image', 'video'):
-			kwargs = _kwargs_from_map({'end_datetime_utc': 'endDate', 'last_updated_datetime_utc': 'lastUpdateDate', 'duration_minutes': 'duration', 'counts_are_final': 'finalResults'})
+			kwargs = snscrape.utils.dict_map(bindingValues, {'end_datetime_utc': 'endDate', 'last_updated_datetime_utc': 'lastUpdateDate', 'duration_minutes': 'duration', 'counts_are_final': 'finalResults'})
 
 			options = []
 			for key in sorted(bindingValues):
 				if key.startswith('choice') and key.endswith('_label'):
 					optKwargs = {'label': bindingValues[key]}
 					if (count := bindingValues.get(f'{key[:-5]}count')):
 						optKwargs['count'] = int(count)
@@ -1103,17 +1209,17 @@
 				if 'vmap' not in bindingValues['player_stream_url']:
 					_logger.warning(f'Non-VMAP URL in {cardName} player_stream_url on tweet {tweetId}')
 				variants.append(VideoVariant(contentType = 'text/xml', url = bindingValues['player_stream_url'], bitrate = None))
 				kwargs['medium'] = Video(thumbnailUrl = bindingValues['player_image_original'], variants = variants, duration = int(bindingValues['content_duration_seconds']))
 
 			return PollCard(**kwargs)
 		elif cardName == 'player':
-			return PlayerCard(**_kwargs_from_map({'title': 'title', 'description': 'description', 'card_url': 'url', 'player_image_original': 'imageUrl', 'site': 'siteUser'}))
+			return PlayerCard(**snscrape.utils.dict_map(bindingValues, {'title': 'title', 'description': 'description', 'card_url': 'url', 'player_image_original': 'imageUrl', 'site': 'siteUser'}))
 		elif cardName in ('promo_image_convo', 'promo_video_convo'):
-			kwargs = _kwargs_from_map({'thank_you_text': 'thankYouText', 'thank_you_url': 'thankYouUrl', 'thank_you_shortened_url': 'thankYouTcoUrl'})
+			kwargs = snscrape.utils.dict_map(bindingValues, {'thank_you_text': 'thankYouText', 'thank_you_url': 'thankYouUrl', 'thank_you_shortened_url': 'thankYouTcoUrl'})
 			kwargs['actions'] = []
 			for l in ('one', 'two', 'three', 'four'):
 				if f'cta_{l}' in bindingValues:
 					kwargs['actions'].append(PromoConvoAction(label = bindingValues[f'cta_{l}'], tweet = bindingValues[f'cta_{l}_tweet']))
 			if 'image' in cardName:
 				kwargs['medium'] = Photo(previewUrl = bindingValues['promo_image_small'], fullUrl = bindingValues['promo_image_original'])
 				if 'cover_promo_image' in bindingValues:
@@ -1124,41 +1230,44 @@
 				if bindingValues['player_stream_url'] != bindingValues['player_url']:
 					if 'vmap' not in bindingValues['player_url']:
 						_logger.warning(f'Non-VMAP URL in {cardName} player_url on tweet {tweetId}')
 					variants.append(VideoVariant(contentType = 'text/xml', url = bindingValues['player_url'], bitrate = None))
 				kwargs['medium'] = Video(thumbnailUrl = bindingValues['player_image_original'], variants = variants, duration = int(bindingValues['content_duration_seconds']))
 			return PromoConvoCard(**kwargs)
 		elif cardName in ('745291183405076480:broadcast', '3691233323:periscope_broadcast'):
-			keyKwargMap = {'broadcast_state': 'state', 'broadcast_source': 'source', 'site': 'siteUser'}
+			keyMap = {'broadcast_state': 'state', 'broadcast_source': 'source', 'site': 'siteUser'}
 			if cardName == '745291183405076480:broadcast':
-				keyKwargMap = {**keyKwargMap, 'broadcast_id': 'id', 'broadcast_url': 'url', 'broadcast_title': 'title', 'broadcast_thumbnail_original': 'thumbnailUrl'}
+				keyMap = {**keyMap, 'broadcast_id': 'id', 'broadcast_url': 'url', 'broadcast_title': 'title', 'broadcast_thumbnail_original': 'thumbnailUrl'}
 			else:
-				keyKwargMap = {**keyKwargMap, 'id': 'id', 'url': 'url', 'title': 'title', 'description': 'description', 'total_participants': 'totalParticipants', 'full_size_thumbnail_url': 'thumbnailUrl'}
-			kwargs = _kwargs_from_map(keyKwargMap)
+				keyMap = {**keyMap, 'id': 'id', 'url': 'url', 'title': 'title', 'description': 'description', 'total_participants': 'totalParticipants', 'full_size_thumbnail_url': 'thumbnailUrl'}
+			kwargs = snscrape.utils.dict_map(bindingValues, keyMap)
 			if 'broadcaster_twitter_id' in bindingValues:
-				kwargs['broadcaster'] = User(id = int(bindingValues['broadcaster_twitter_id']), username = bindingValues['broadcaster_username'], displayname = bindingValues['broadcaster_display_name'])
+				if int(bindingValues['broadcaster_twitter_id']) in userRefs:
+					kwargs['broadcaster'] = userRefs[int(bindingValues['broadcaster_twitter_id'])]
+				else:
+					kwargs['broadcaster'] = User(id = int(bindingValues['broadcaster_twitter_id']), username = bindingValues['broadcaster_username'], displayname = bindingValues['broadcaster_display_name'])
 			if 'siteUser' not in kwargs:
 				kwargs['siteUser'] = None
 			if cardName == '745291183405076480:broadcast':
 				return BroadcastCard(**kwargs)
 			else:
 				kwargs['totalParticipants'] = int(kwargs['totalParticipants'])
 				return PeriscopeBroadcastCard(**kwargs)
 		elif cardName == '745291183405076480:live_event':
-			kwargs = _kwargs_from_map({'event_id': 'id', 'event_title': 'title', 'event_category': 'category', 'event_subtitle': 'description'})
+			kwargs = snscrape.utils.dict_map(bindingValues, {'event_id': 'id', 'event_title': 'title', 'event_category': 'category', 'event_subtitle': 'description'})
 			kwargs['id'] = int(kwargs['id'])
 			kwargs['photo'] = Photo(previewUrl = bindingValues['event_thumbnail_small'], fullUrl = bindingValues.get('event_thumbnail_original') or bindingValues['event_thumbnail'])
 			return EventCard(event = Event(**kwargs))
 		elif cardName == '3337203208:newsletter_publication':
-			kwargs = _kwargs_from_map({'newsletter_title': 'title', 'newsletter_description': 'description', 'newsletter_image_original': 'imageUrl', 'card_url': 'url', 'revue_account_id': 'revueAccountId', 'issue_count': 'issueCount'})
+			kwargs = snscrape.utils.dict_map(bindingValues, {'newsletter_title': 'title', 'newsletter_description': 'description', 'newsletter_image_original': 'imageUrl', 'card_url': 'url', 'revue_account_id': 'revueAccountId', 'issue_count': 'issueCount'})
 			kwargs['revueAccountId'] = int(kwargs['revueAccountId'])
 			kwargs['issueCount'] = int(kwargs['issueCount'])
 			return NewsletterCard(**kwargs)
 		elif cardName == '3337203208:newsletter_issue':
-			kwargs = _kwargs_from_map({
+			kwargs = snscrape.utils.dict_map(bindingValues, {
 				'newsletter_title': 'newsletterTitle',
 				'newsletter_description': 'newsletterDescription',
 				'issue_title': 'issueTitle',
 				'issue_description': 'issueDescription',
 				'issue_number': 'issueNumber',
 				'issue_image_original': 'imageUrl',
 				'card_url': 'url',
@@ -1172,33 +1281,33 @@
 				id = bindingValues['amplify_content_id'],
 				video = Video(
 					thumbnailUrl = bindingValues['player_image'],
 					variants = [VideoVariant(url = bindingValues['amplify_url_vmap'], contentType = bindingValues.get('player_stream_content_type'), bitrate = None)],
 				),
 			)
 		elif cardName == 'appplayer':
-			kwargs = _kwargs_from_map({'title': 'title', 'app_category': 'appCategory', 'player_owner_id': 'playerOwnerId', 'site': 'siteUser'})
+			kwargs = snscrape.utils.dict_map(bindingValues, {'title': 'title', 'app_category': 'appCategory', 'player_owner_id': 'playerOwnerId', 'site': 'siteUser'})
 			kwargs['playerOwnerId'] = int(kwargs['playerOwnerId'])
 			variants = []
 			variants.append(VideoVariant(contentType = 'application/x-mpegurl', url = bindingValues['player_hls_url'], bitrate = None))
 			if 'vmap' not in bindingValues['player_url']:
 				_logger.warning(f'Non-VMAP URL in {cardName} player_url on tweet {tweetId}')
 			variants.append(VideoVariant(contentType = 'text/xml', url = bindingValues['player_url'], bitrate = None))
 			kwargs['video'] = Video(thumbnailUrl = bindingValues['player_image_original'], variants = variants, duration = int(bindingValues['content_duration_seconds']))
 			return AppPlayerCard(**kwargs)
 		elif cardName == '3691233323:audiospace':
-			return SpacesCard(**_kwargs_from_map({'card_url': 'url', 'id': 'id'}))
+			return SpacesCard(**snscrape.utils.dict_map(bindingValues, {'card_url': 'url', 'id': 'id'}))
 		elif cardName == '2586390716:message_me':
 			# Note that the strings in Twitter's JS appear to have an incorrect mapping that then gets changed somewhere in the 1.8 MiB of JS!
 			# cta_1, 3, and 4 should mean 'Message us', 'Send a private message', and 'Send me a private message', but the correct mapping is currently unknown.
 			ctas = {'message_me_card_cta_2': 'Send us a private message'}
 			if bindingValues['cta'] not in ctas:
 				_logger.warning(f'Unsupported message_me card cta on tweet {tweetId}: {bindingValues["cta"]!r}')
 				return
-			return MessageMeCard(**_kwargs_from_map({'recipient': 'recipient', 'card_url': 'url'}), buttonText = ctas[bindingValues['cta']])
+			return MessageMeCard(**snscrape.utils.dict_map(bindingValues, {'recipient': 'recipient', 'card_url': 'url'}), buttonText = ctas[bindingValues['cta']])
 		elif cardName == 'unified_card':
 			o = json.loads(bindingValues['unified_card'])
 			kwargs = {}
 			if 'type' in o:
 				unifiedCardType = o.get('type')
 				if unifiedCardType not in (
 					'image_app',
@@ -1359,59 +1468,51 @@
 	def _make_vibe(self, vibe):
 		return Vibe(
 			text = vibe['text'],
 			imageUrl = vibe['imgUrl'],
 			imageDescription = vibe['imgDescription'],
 		)
 
-	def _tweet_to_tweet(self, tweet, obj):
-		user = self._user_to_user(obj['globalObjects']['users'][tweet['user_id_str']])
-		kwargs = {}
-		if 'retweeted_status_id_str' in tweet:
-			kwargs['retweetedTweet'] = self._tweet_to_tweet(obj['globalObjects']['tweets'][tweet['retweeted_status_id_str']], obj)
-		if 'quoted_status_id_str' in tweet and tweet['quoted_status_id_str'] in obj['globalObjects']['tweets']:
-			kwargs['quotedTweet'] = self._tweet_to_tweet(obj['globalObjects']['tweets'][tweet['quoted_status_id_str']], obj)
-		if 'card' in tweet:
-			kwargs['card'] = self._make_card(tweet['card'], _TwitterAPIType.V2, self._get_tweet_id(tweet))
-		if 'ext_views' in tweet and 'count' in tweet['ext_views']:
-			kwargs['viewCount'] = int(tweet['ext_views']['count'])
-		if 'vibe' in tweet.get('ext', {}):
-			kwargs['vibe'] = self._make_vibe(tweet['ext']['vibe']['r']['ok'])
-		return self._make_tweet(tweet, user, **kwargs)
+	def _make_edit_state(self, editControl):
+		if 'edit_control_initial' in editControl:
+			return self._make_edit_state(editControl['edit_control_initial'])
+		return EditState(
+			editTweetIds = [int(x) for x in editControl['edit_tweet_ids']],
+			editableUntilDate = datetime.datetime.fromtimestamp(int(editControl['editable_until_msecs']) / 1000, tz = datetime.timezone.utc),
+			editsRemaining = int(editControl['edits_remaining']),
+		)
 
 	def _make_tombstone(self, tweetId, info):
 		if tweetId is None:
 			raise snscrape.base.ScraperException('Cannot create tombstone without tweet ID')
 		if info and (text := info.get('richText', info['text'])):
 			return Tombstone(
 				id = tweetId,
 				text = text['text'],
 				textLinks = [TextLink(text = text['text'][x['fromIndex']:x['toIndex']], url = x['ref']['url'], tcourl = None, indices = (x['fromIndex'], x['toIndex'])) for x in text['entities']],
 			)
 		else:
 			return Tombstone(id = tweetId)
 
-	def _graphql_timeline_tweet_item_result_to_tweet(self, result, tweetId = None):
+	def _graphql_timeline_tweet_item_result_to_tweet(self, result, tweetId = None, **kwargs):
 		if result['__typename'] == 'Tweet':
 			pass
 		elif result['__typename'] == 'TweetWithVisibilityResults':
 			#TODO Include result['softInterventionPivot'] in the Tweet object
 			result = result['tweet']
 		elif result['__typename'] == 'TweetTombstone':
 			return self._make_tombstone(tweetId, result.get('tombstone'))
 		elif result['__typename'] == 'TweetUnavailable':
 			if tweetId is None:
 				raise snscrape.base.ScraperException('Cannot handle unavailable tweet without tweet ID')
 			return TweetRef(id = tweetId)
 		else:
 			raise snscrape.base.ScraperException(f'Unknown result type {result["__typename"]!r}')
 		tweet = result['legacy']
-		userId = int(result['core']['user_results']['result']['rest_id'])
-		user = self._user_to_user(result['core']['user_results']['result']['legacy'], id_ = userId)
-		kwargs = {}
+		user = self._graphql_user_results_to_user(result['core']['user_results'], userId = int(result['legacy']['user_id_str']))
 		if 'retweeted_status_result' in tweet:
 			#TODO Tombstones will cause a crash here.
 			kwargs['retweetedTweet'] = self._graphql_timeline_tweet_item_result_to_tweet(tweet['retweeted_status_result']['result'])
 		if 'quoted_status_result' in result:
 			if 'result' not in result['quoted_status_result']:
 				_logger.warning(f'quoted_status_result for {tweet["quoted_status_id_str"]} without an actual result on tweet {self._get_tweet_id(tweet)}, using TweetRef')
 				kwargs['quotedTweet'] = TweetRef(int(tweet['quoted_status_id_str']))
@@ -1429,51 +1530,58 @@
 				kwargs['quotedTweet'] = TweetRef(id = int(qTweet['rest_id']))
 		elif 'quoted_status_id_str' in tweet:
 			# Omit the TweetRef if this is a retweet and the quoted tweet ID matches the tweet quoted in the retweeted tweet.
 			if tweet['quoted_status_id_str'] != tweet.get('retweeted_status_result', {}).get('result', {}).get('quoted_status_result', {}).get('result', {}).get('rest_id'):
 				kwargs['quotedTweet'] = TweetRef(id = int(tweet['quoted_status_id_str']))
 		if 'card' in result:
 			kwargs['card'] = self._make_card(result['card'], _TwitterAPIType.GRAPHQL, self._get_tweet_id(tweet))
+		if 'note_tweet' in result:
+			kwargs['noteTweet'] = result['note_tweet']['note_tweet_results']['result']
 		if 'views' in result and 'count' in result['views']:
 			kwargs['viewCount'] = int(result['views']['count'])
 		if 'vibe' in result:
 			kwargs['vibe'] = self._make_vibe(result['vibe'])
+		if 'edit_control' in result:
+			kwargs['editState'] = self._make_edit_state(result['edit_control'])
 		return self._make_tweet(tweet, user, **kwargs)
 
-	def _graphql_timeline_instructions_to_tweets(self, instructions, includeConversationThreads = False):
+	def _graphql_timeline_instructions_to_tweets(self, instructions, includeConversationThreads = False, **kwargs):
 		for instruction in instructions:
 			if instruction['type'] != 'TimelineAddEntries':
 				continue
 			for entry in instruction['entries']:
 				if entry['entryId'].startswith('tweet-'):
 					tweetId = int(entry['entryId'].split('-', 1)[1])
 					if entry['content']['entryType'] == 'TimelineTimelineItem' and entry['content']['itemContent']['itemType'] == 'TimelineTweet':
 						if 'result' not in entry['content']['itemContent']['tweet_results']:
 							_logger.warning(f'Skipping empty tweet entry {entry["entryId"]}')
 							continue
-						yield self._graphql_timeline_tweet_item_result_to_tweet(entry['content']['itemContent']['tweet_results']['result'], tweetId = tweetId)
+						yield self._graphql_timeline_tweet_item_result_to_tweet(entry['content']['itemContent']['tweet_results']['result'], tweetId = tweetId, **kwargs)
 					else:
 						_logger.warning('Got unrecognised timeline tweet item(s)')
-				elif entry['entryId'].startswith('homeConversation-'):
+				elif entry['entryId'].startswith(('homeConversation-', 'profile-conversation-')):
 					if entry['content']['entryType'] == 'TimelineTimelineModule':
-						for item in entry['content']['items']:
-							if not item['entryId'].startswith('homeConversation-') or '-tweet-' not in item['entryId']:
-								raise snscrape.base.ScraperException(f'Unexpected home conversation entry ID: {item["entryId"]!r}')
+						for item in reversed(entry['content']['items']):
+							if not item['entryId'].startswith(entry['entryId'].split('ion-', 1)[0] + 'ion-') or '-tweet-' not in item['entryId']:
+								raise snscrape.base.ScraperException(f'Unexpected conversation entry ID: {item["entryId"]!r}')
 							tweetId = int(item['entryId'].split('-tweet-', 1)[1])
 							if item['item']['itemContent']['itemType'] == 'TimelineTweet':
 								if 'result' in item['item']['itemContent']['tweet_results']:
-									yield self._graphql_timeline_tweet_item_result_to_tweet(item['item']['itemContent']['tweet_results']['result'], tweetId = tweetId)
+									yield self._graphql_timeline_tweet_item_result_to_tweet(item['item']['itemContent']['tweet_results']['result'], tweetId = tweetId, **kwargs)
 								else:
 									yield TweetRef(id = tweetId)
 				elif includeConversationThreads and entry['entryId'].startswith('conversationthread-'):  #TODO show more cursor?
 					for item in entry['content']['items']:
 						if item['entryId'].startswith(f'{entry["entryId"]}-tweet-'):
+							if item['entryId'][len(entry['entryId']) + 7:].strip('0123456789'):
+								_logger.warning(f'Skipping promoted tweet entry {item["entryId"]}')
+								continue
 							tweetId = int(item['entryId'][len(entry['entryId']) + 7:])
-							yield self._graphql_timeline_tweet_item_result_to_tweet(item['item']['itemContent']['tweet_results']['result'], tweetId = tweetId)
-				elif not entry['entryId'].startswith('cursor-'):
+							yield self._graphql_timeline_tweet_item_result_to_tweet(item['item']['itemContent']['tweet_results']['result'], tweetId = tweetId, **kwargs)
+				elif not entry['entryId'].startswith(('cursor-', 'toptabsrpusermodule-', 'tweetdetailrelatedtweets-', 'label-')):
 					_logger.warning(f'Skipping unrecognised entry ID: {entry["entryId"]!r}')
 
 	def _render_text_with_urls(self, text, urls):
 		if not urls:
 			return text
 		out = []
 		out.append(text[:urls[0]['indices'][0]])
@@ -1481,16 +1589,15 @@
 		assert all(url['indices'][1] <= nextUrl['indices'][0] for url, nextUrl in zip(urls, urls[1:])), 'broken URL indices'
 		for url, nextUrl in itertools.zip_longest(urls, urls[1:]):
 			if 'display_url' in url:
 				out.append(url['display_url'])
 			out.append(text[url['indices'][1] : nextUrl['indices'][0] if nextUrl is not None else None])
 		return ''.join(out)
 
-	def _user_to_user(self, user, id_ = None):
-		kwargs = {}
+	def _user_to_user(self, user, id_ = None, **kwargs):
 		kwargs['username'] = user['screen_name']
 		kwargs['id'] = id_ if id_ else user['id'] if 'id' in user else int(user['id_str'])
 		kwargs['displayname'] = user['name']
 		kwargs['rawDescription'] = user['description']
 		kwargs['renderedDescription'] = self._render_text_with_urls(user['description'], user['entities']['description'].get('urls'))
 		if user['entities']['description'].get('urls'):
 			kwargs['descriptionLinks'] = [TextLink(
@@ -1514,52 +1621,63 @@
 			if not entity or entity['url'] != user['url']:
 				_logger.warning(f'Link inconsistency on user {kwargs["id"]}')
 			if not entity:
 				entity = {'indices': (0, len(user['url']))}
 			kwargs['link'] = TextLink(text = entity.get('display_url'), url = entity.get('expanded_url', user['url']), tcourl = user['url'], indices = tuple(entity['indices']))
 		kwargs['profileImageUrl'] = user['profile_image_url_https']
 		kwargs['profileBannerUrl'] = user.get('profile_banner_url')
-		if 'ext' in user and 'highlightedLabel' in user['ext'] and (label := user['ext']['highlightedLabel']['r']['ok'].get('label')):
-			kwargs['label'] = self._user_label_to_user_label(label)
+		if 'label' not in kwargs and (labelO := user.get('affiliates_highlighted_label', {}).get('label')):
+			kwargs['label'] = self._user_label_to_user_label(labelO)
+		if 'blue' not in kwargs:
+			kwargs['blue'] = user.get('is_blue_verified')
+		if 'blueType' not in kwargs:
+			kwargs['blueType'] = user.get('verified_type')
 		return User(**kwargs)
 
 	def _user_label_to_user_label(self, label):
 		labelKwargs = {}
 		labelKwargs['description'] = label['description']
 		if 'url' in label and 'url' in label['url']:
 			labelKwargs['url'] = label['url']['url']
 		if 'badge' in label and 'url' in label['badge']:
 			labelKwargs['badgeUrl'] = label['badge']['url']
 		if 'longDescription' in label and 'text' in label['longDescription']:
 			labelKwargs['longDescription'] = label['longDescription']['text']
 		return UserLabel(**labelKwargs)
 
-	def _graphql_user_results_to_user_ref(self, obj):
-		if 'id' not in obj:
-			return None
-		if isinstance(obj['id'], int):
-			userId = obj['id']
-		elif obj['id'].startswith('VXNlclJlc3VsdHM6'):
-			# UserResults:<userid> in base64
-			try:
-				userId = base64.b64decode(obj['id'])
-			except ValueError:
+	def _graphql_user_results_to_user_ref(self, obj, userId = None):
+		if userId is None:
+			if 'id' not in obj:
 				return None
-			assert userId.startswith(b'UserResults:')
-			userId = int(userId.split(b':', 1)[1])
+			if isinstance(obj['id'], int):
+				userId = obj['id']
+			elif obj['id'].startswith('VXNlclJlc3VsdHM6'):
+				# UserResults:<userid> in base64
+				try:
+					userId = base64.b64decode(obj['id'])
+				except ValueError:
+					return None
+				assert userId.startswith(b'UserResults:')
+				userId = int(userId.split(b':', 1)[1])
 		kwargs = {}
 		if 'result' in obj and obj['result']['__typename'] == 'UserUnavailable' and 'unavailable_message' in obj['result']:
 			kwargs['text'] = obj['result']['unavailable_message']['text']
 			kwargs['textLinks'] = [TextLink(text = kwargs['text'][x['fromIndex']:x['toIndex']], url = x['ref']['url'], tcourl = None, indices = (x['fromIndex'], x['toIndex'])) for x in obj['result']['unavailable_message']['entities']]
 		return UserRef(id = userId, **kwargs)
 
-	def _graphql_user_results_to_user(self, results):
+	def _graphql_user_results_to_user(self, results, userId = None):
 		if 'result' not in results or results['result']['__typename'] == 'UserUnavailable':
-			return self._graphql_user_results_to_user_ref(results)
-		return self._user_to_user(results['result']['legacy'], id_ = int(results['result']['rest_id']))
+			return self._graphql_user_results_to_user_ref(results, userId)
+		kwargs = {}
+		kwargs['blue'] = results['result']['is_blue_verified']
+		if (labelO := results['result']['affiliates_highlighted_label'].get('label')):
+			kwargs['label'] = self._user_label_to_user_label(labelO)
+		if 'profile_image_shape' in results['result']:
+			kwargs['profileImageShape'] = ProfileImageShape._from_twitter_string(results['result']['profile_image_shape'])
+		return self._user_to_user(results['result']['legacy'], id_ = userId if userId is not None else int(results['result']['rest_id']), **kwargs)
 
 	@classmethod
 	def _cli_construct(cls, argparseArgs, *args, **kwargs):
 		kwargs['guestTokenManager'] = _CLIGuestTokenManager()
 		return super()._cli_construct(argparseArgs, *args, **kwargs)
 
 
@@ -1596,83 +1714,67 @@
 			warnings.warn(f'`top` argument is deprecated, use `mode = {replacement}` instead of `top = {bool(top)}`', snscrape.base.DeprecatedFeatureWarning, stacklevel = 2)
 			mode = TwitterSearchScraperMode.TOP if top else TwitterSearchScraperMode.LIVE
 		self._mode = mode
 
 	def get_items(self):
 		if not self._query.strip():
 			raise ValueError('empty query')
-		paginationParams = {
-			'include_profile_interstitial_type': '1',
-			'include_blocking': '1',
-			'include_blocked_by': '1',
-			'include_followed_by': '1',
-			'include_want_retweets': '1',
-			'include_mute_edge': '1',
-			'include_can_dm': '1',
-			'include_can_media_tag': '1',
-			'include_ext_has_nft_avatar': '1',
-			'include_ext_is_blue_verified': '1',
-			'include_ext_verified_type': '1',
-			'skip_status': '1',
-			'cards_platform': 'Web-12',
-			'include_cards': '1',
-			'include_ext_alt_text': 'true',
-			'include_ext_limited_action_results': 'false',
-			'include_quote_count': 'true',
-			'include_reply_count': '1',
-			'tweet_mode': 'extended',
-			'include_ext_collab_control': 'true',
-			'include_ext_views': 'true',
-			'include_entities': 'true',
-			'include_user_entities': 'true',
-			'include_ext_media_color': 'true',
-			'include_ext_media_availability': 'true',
-			'include_ext_sensitive_media_warning': 'true',
-			'include_ext_trusted_friends_metadata': 'true',
-			'send_error_codes': 'true',
-			'simple_quoted_tweet': 'true',
-			'q': self._query,
-		}
-		if self._mode is TwitterSearchScraperMode.LIVE:
-			paginationParams = {
-				**paginationParams,
-				'tweet_search_mode': 'live',
-			}
-		elif self._mode is TwitterSearchScraperMode.TOP:
-			pass
-		elif self._mode is TwitterSearchScraperMode.USER:
-			paginationParams = {
-				**paginationParams,
-				'result_filter': 'user',
-				'query_source': '',
-			}
-		paginationParams = {
-			**paginationParams,
-			'count': '20',
-			'query_source': 'spelling_expansion_revert_click',
+		if self._mode is TwitterSearchScraperMode.USER:
+			raise snscrape.base.ScraperException('User searches currently unsupported')
+
+		paginationVariables = {
+			'rawQuery': self._query,
+			'count': 20,
 			'cursor': None,
-			'pc': '1',
-			'spelling_corrections': '1',
-			'include_ext_edit_control': 'true',
-			'ext': 'mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,enrichments,superFollowMetadata,unmentionInfo,editControl,collab_control,vibe',
+			'product': 'Latest' if self._mode is TwitterSearchScraperMode.LIVE else 'Top',
+			'withDownvotePerspective': False,
+			'withReactionsMetadata': False,
+			'withReactionsPerspective': False,
+		}
+		variables = paginationVariables.copy()
+		del variables['cursor']
+		features = {
+			'rweb_lists_timeline_redesign_enabled': False,
+			'blue_business_profile_image_shape_enabled': False,
+			'responsive_web_graphql_exclude_directive_enabled': True,
+			'verified_phone_label_enabled': False,
+			'creator_subscriptions_tweet_preview_api_enabled': False,
+			'responsive_web_graphql_timeline_navigation_enabled': True,
+			'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+			'tweetypie_unmention_optimization_enabled': True,
+			'vibe_api_enabled': True,
+			'responsive_web_edit_tweet_api_enabled': True,
+			'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
+			'view_counts_everywhere_api_enabled': True,
+			'longform_notetweets_consumption_enabled': True,
+			'tweet_awards_web_tipping_enabled': False,
+			'freedom_of_speech_not_reach_fetch_enabled': False,
+			'standardized_nudges_misinfo': True,
+			'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': False,
+			'interactive_text_enabled': True,
+			'responsive_web_text_conversations_enabled': False,
+			'longform_notetweets_rich_text_read_enabled': False,
+			'longform_notetweets_inline_media_enabled': False,
+			'responsive_web_enhance_cards_enabled': False,
+			'responsive_web_twitter_blue_verified_badge_is_enabled': True,
 		}
-		params = paginationParams.copy()
-		del params['cursor']
+		params = {'variables': variables, 'features': features}
+		paginationParams = {'variables': paginationVariables, 'features': features}
 
-		for obj in self._iter_api_data('https://api.twitter.com/2/search/adaptive.json', _TwitterAPIType.V2, params, paginationParams, cursor = self._cursor):
-			yield from self._v2_timeline_instructions_to_tweets_or_users(obj)
+		for obj in self._iter_api_data('https://twitter.com/i/api/graphql/7jT5GT59P8IFjgxwqnEdQw/SearchTimeline', _TwitterAPIType.GRAPHQL, params, paginationParams, cursor = self._cursor, instructionsPath = ['data', 'search_by_raw_query', 'search_timeline', 'timeline', 'instructions']):
+			yield from self._graphql_timeline_instructions_to_tweets(obj['data']['search_by_raw_query']['search_timeline']['timeline']['instructions'])
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
 		subparser.add_argument('--cursor', metavar = 'CURSOR', help = '(deprecated)')
 		group = subparser.add_mutually_exclusive_group(required = False)
 		group.add_argument('--top', action = 'store_true', default = False, help = 'Search top tweets instead of live/chronological')
 		group.add_argument('--user', action = 'store_true', default = False, help = 'Search users instead of tweets')
 		subparser.add_argument('--max-empty-pages', dest = 'maxEmptyPages', metavar = 'N', type = int, default = 20, help = 'Stop after N empty pages from Twitter; set to 0 to disable')
-		subparser.add_argument('query', type = snscrape.base.nonempty_string('query'), help = 'A Twitter search string')
+		subparser.add_argument('query', type = snscrape.utils.nonempty_string_arg('query'), help = 'A Twitter search string')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.query, cursor = args.cursor, mode = TwitterSearchScraperMode._cli_from_args(args), maxEmptyPages = args.maxEmptyPages)
 
 
 class TwitterUserScraper(TwitterSearchScraper):
@@ -1686,67 +1788,34 @@
 		self._user = user
 		self._baseUrl = f'https://twitter.com/{self._user}' if not self._isUserId else f'https://twitter.com/i/user/{self._user}'
 
 	def _get_entity(self):
 		self._ensure_guest_token()
 		if not self._isUserId:
 			fieldName = 'screen_name'
-			endpoint = 'https://twitter.com/i/api/graphql/7mjxD3-C6BxitPMVQ6w0-Q/UserByScreenName'
+			endpoint = 'https://twitter.com/i/api/graphql/pVrmNaXcxPjisIvKtLDMEA/UserByScreenName'
 		else:
 			fieldName = 'userId'
-			endpoint = 'https://twitter.com/i/api/graphql/I5nvpI91ljifos1Y3Lltyg/UserByRestId'
-		variables = {fieldName: str(self._user), 'withSafetyModeUserFields': True, 'withSuperFollowsUserFields': True}
-		obj = self._get_api_data(endpoint, _TwitterAPIType.GRAPHQL, params = {'variables': variables})
+			endpoint = 'https://twitter.com/i/api/graphql/1YAM811Q8Ry4XyPpJclURQ/UserByRestId'
+		variables = {fieldName: str(self._user), 'withSafetyModeUserFields': True}
+		features = {
+			'blue_business_profile_image_shape_enabled': True,
+			'responsive_web_graphql_exclude_directive_enabled': True,
+			'verified_phone_label_enabled': False,
+			'highlights_tweets_tab_ui_enabled': False,
+			'creator_subscriptions_tweet_preview_api_enabled': False,
+			'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+			'responsive_web_graphql_timeline_navigation_enabled': True,
+		}
+		obj = self._get_api_data(endpoint, _TwitterAPIType.GRAPHQL, params = {'variables': variables, 'features': features}, instructionsPath = ['data', 'user'])
 		if not obj['data'] or 'result' not in obj['data']['user']:
-			_logger.warning('Empty response')
-			return None
+			raise snscrape.base.ScraperException('Empty response')
 		if obj['data']['user']['result']['__typename'] == 'UserUnavailable':
-			_logger.warning('User unavailable')
-			return None
-		user = obj['data']['user']['result']
-		rawDescription = user['legacy']['description']
-		renderedDescription = self._render_text_with_urls(rawDescription, user['legacy']['entities']['description']['urls'])
-		link = None
-		if user['legacy'].get('url'):
-			entity = user['legacy']['entities'].get('url', {}).get('urls', [None])[0]
-			if not entity or entity['url'] != user['legacy']['url']:
-				_logger.warning(f'Link inconsistency on user')
-			if not entity:
-				entity = {'indices': (0, len(user['legacy']['url']))}
-			link = TextLink(text = entity.get('display_url'), url = entity.get('expanded_url', user['legacy']['url']), tcourl = user['legacy']['url'], indices = tuple(entity['indices']))
-		label = None
-		if (labelO := user['affiliates_highlighted_label'].get('label')):
-			label = self._user_label_to_user_label(labelO)
-		return User(
-			username = user['legacy']['screen_name'],
-			id = int(user['rest_id']),
-			displayname = user['legacy']['name'],
-			rawDescription = rawDescription,
-			renderedDescription = renderedDescription,
-			descriptionLinks = [TextLink(
-			                      text = x.get('display_url'),
-			                      url = x['expanded_url'],
-			                      tcourl = x['url'],
-			                      indices = tuple(x['indices']),
-			                    ) for x in user['legacy']['entities']['description']['urls']],
-			verified = user['legacy']['verified'],
-			created = email.utils.parsedate_to_datetime(user['legacy']['created_at']),
-			followersCount = user['legacy']['followers_count'],
-			friendsCount = user['legacy']['friends_count'],
-			statusesCount = user['legacy']['statuses_count'],
-			favouritesCount = user['legacy']['favourites_count'],
-			listedCount = user['legacy']['listed_count'],
-			mediaCount = user['legacy']['media_count'],
-			location = user['legacy']['location'],
-			protected = user['legacy']['protected'],
-			link = link,
-			profileImageUrl = user['legacy']['profile_image_url_https'],
-			profileBannerUrl = user['legacy'].get('profile_banner_url'),
-			label = label,
-		  )
+			raise snscrape.base.EntityUnavailable('User unavailable')
+		return self._graphql_user_results_to_user(obj['data']['user'])
 
 	def get_items(self):
 		if self._isUserId:
 			# Resolve user ID to username
 			if self.entity is None:
 				raise snscrape.base.ScraperException(f'Could not resolve user ID {self._user!r} to username')
 			self._user = self.entity.username
@@ -1779,80 +1848,91 @@
 	def get_items(self):
 		if not self._isUserId:
 			if self.entity is None:
 				raise snscrape.base.ScraperException(f'Could not resolve username {self._user!r} to ID')
 			userId = self.entity.id
 		else:
 			userId = self._user
+
 		paginationVariables = {
 			'userId': userId,
 			'count': 100,
 			'cursor': None,
 			'includePromotedContent': True,
 			'withCommunity': True,
-			'withSuperFollowsUserFields': True,
-			'withDownvotePerspective': False,
-			'withReactionsMetadata': False,
-			'withReactionsPerspective': False,
-			'withSuperFollowsTweetFields': True,
 			'withVoice': True,
 			'withV2Timeline': True,
 		}
 		variables = paginationVariables.copy()
 		del variables['cursor']
 		features = {
-			'responsive_web_twitter_blue_verified_badge_is_enabled': True,
-			'responsive_web_graphql_exclude_directive_enabled': False,
+			'rweb_lists_timeline_redesign_enabled': False,
+			'blue_business_profile_image_shape_enabled': True,
+			'responsive_web_graphql_exclude_directive_enabled': True,
 			'verified_phone_label_enabled': False,
+			'creator_subscriptions_tweet_preview_api_enabled': False,
 			'responsive_web_graphql_timeline_navigation_enabled': True,
 			'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
-			'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
 			'tweetypie_unmention_optimization_enabled': True,
 			'vibe_api_enabled': True,
 			'responsive_web_edit_tweet_api_enabled': True,
 			'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
 			'view_counts_everywhere_api_enabled': True,
 			'longform_notetweets_consumption_enabled': True,
 			'tweet_awards_web_tipping_enabled': False,
-			'freedom_of_speech_not_reach_fetch_enabled': False,
+			'freedom_of_speech_not_reach_fetch_enabled': True,
 			'standardized_nudges_misinfo': True,
 			'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': False,
 			'interactive_text_enabled': True,
 			'responsive_web_text_conversations_enabled': False,
+			'longform_notetweets_rich_text_read_enabled': True,
+			'longform_notetweets_inline_media_enabled': False,
 			'responsive_web_enhance_cards_enabled': False,
 		}
 
 		params = {'variables': variables, 'features': features}
 		paginationParams = {'variables': paginationVariables, 'features': features}
 
 		gotPinned = False
-		for obj in self._iter_api_data('https://twitter.com/i/api/graphql/nrdle2catTyGnTyj1Qa7wA/UserTweetsAndReplies', _TwitterAPIType.GRAPHQL, params, paginationParams):
+		previousPagesTweetIds = set()
+		for obj in self._iter_api_data('https://twitter.com/i/api/graphql/fn9oRltM1N4thkh5CVusPg/UserTweetsAndReplies', _TwitterAPIType.GRAPHQL, params, paginationParams, instructionsPath = ['data', 'user', 'result', 'timeline_v2', 'timeline', 'instructions']):
+			if not obj['data'] or 'result' not in obj['data']['user']:
+				raise snscrape.base.ScraperException('Empty response')
 			if obj['data']['user']['result']['__typename'] == 'UserUnavailable':
-				_logger.warning('User unavailable')
-				break
+				raise snscrape.base.EntityUnavailable('User unavailable')
 			instructions = obj['data']['user']['result']['timeline_v2']['timeline']['instructions']
 			if not gotPinned:
 				for instruction in instructions:
 					if instruction['type'] == 'TimelinePinEntry':
 						gotPinned = True
 						tweetId = int(instruction['entry']['entryId'][6:]) if instruction['entry']['entryId'].startswith('tweet-') else None
-						yield self._graphql_timeline_tweet_item_result_to_tweet(instruction['entry']['content']['itemContent']['tweet_results']['result'], tweetId = tweetId)
-			yield from self._graphql_timeline_instructions_to_tweets(instructions)
+						yield self._graphql_timeline_tweet_item_result_to_tweet(instruction['entry']['content']['itemContent']['tweet_results']['result'], tweetId = tweetId, pinned = True)
+			tweets = list(self._graphql_timeline_instructions_to_tweets(instructions, pinned = False))
+			pageTweetIds = frozenset(tweet.id for tweet in tweets)
+			if len(pageTweetIds) > 0 and pageTweetIds in previousPagesTweetIds:
+				_logger.warning("Found duplicate page of tweets, stopping as assumed cycle found in Twitter's pagination")
+				break
+			previousPagesTweetIds.add(pageTweetIds)
+			# Includes tweets by other users on conversations, don't return those
+			for tweet in tweets:
+				if getattr(getattr(tweet, 'user', None), 'id', userId) != userId:
+					continue
+				yield tweet
 
 
 class TwitterHashtagScraper(TwitterSearchScraper):
 	name = 'twitter-hashtag'
 
 	def __init__(self, hashtag, **kwargs):
 		super().__init__(f'#{hashtag}', **kwargs)
 		self._hashtag = hashtag
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('hashtag', type = snscrape.base.nonempty_string('hashtag'), help = 'A Twitter hashtag (without #)')
+		subparser.add_argument('hashtag', type = snscrape.utils.nonempty_string_arg('hashtag'), help = 'A Twitter hashtag (without #)')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.hashtag)
 
 
 class TwitterCashtagScraper(TwitterSearchScraper):
@@ -1860,15 +1940,15 @@
 
 	def __init__(self, cashtag, **kwargs):
 		super().__init__(f'${cashtag}', **kwargs)
 		self._cashtag = cashtag
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('cashtag', type = snscrape.base.nonempty_string('cashtag'), help = 'A Twitter cashtag (without $)')
+		subparser.add_argument('cashtag', type = snscrape.utils.nonempty_string_arg('cashtag'), help = 'A Twitter cashtag (without $)')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.cashtag)
 
 
 class TwitterTweetScraperMode(enum.Enum):
@@ -1899,83 +1979,142 @@
 			'cursor': None,
 			'referrer': 'tweet',
 			'with_rux_injections': False,
 			'includePromotedContent': True,
 			'withCommunity': True,
 			'withQuickPromoteEligibilityTweetFields': True,
 			'withBirdwatchNotes': False,
-			'withSuperFollowsUserFields': True,
-			'withDownvotePerspective': False,
-			'withReactionsMetadata': False,
-			'withReactionsPerspective': False,
-			'withSuperFollowsTweetFields': True,
 			'withVoice': True,
 			'withV2Timeline': True,
 		}
 		variables = paginationVariables.copy()
 		del variables['cursor'], variables['referrer']
 		features = {
-			'responsive_web_twitter_blue_verified_badge_is_enabled': True,
-			'responsive_web_graphql_exclude_directive_enabled': False,
+			'rweb_lists_timeline_redesign_enabled': False,
+			'blue_business_profile_image_shape_enabled': True,
+			'responsive_web_graphql_exclude_directive_enabled': True,
 			'verified_phone_label_enabled': False,
+			'creator_subscriptions_tweet_preview_api_enabled': False,
 			'responsive_web_graphql_timeline_navigation_enabled': True,
 			'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
 			'tweetypie_unmention_optimization_enabled': True,
 			'vibe_api_enabled': True,
 			'responsive_web_edit_tweet_api_enabled': True,
 			'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
 			'view_counts_everywhere_api_enabled': True,
 			'longform_notetweets_consumption_enabled': True,
 			'tweet_awards_web_tipping_enabled': False,
-			'freedom_of_speech_not_reach_fetch_enabled': False,
+			'freedom_of_speech_not_reach_fetch_enabled': True,
 			'standardized_nudges_misinfo': True,
 			'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': False,
 			'interactive_text_enabled': True,
 			'responsive_web_text_conversations_enabled': False,
+			'longform_notetweets_rich_text_read_enabled': True,
+			'longform_notetweets_inline_media_enabled': False,
 			'responsive_web_enhance_cards_enabled': False,
 		}
 
 		params = {'variables': variables, 'features': features}
 		paginationParams = {'variables': paginationVariables, 'features': features}
-		url = 'https://twitter.com/i/api/graphql/NNiD2K-nEYUfXlMwGCocMQ/TweetDetail'
+		url = 'https://twitter.com/i/api/graphql/miKSMGb2R1SewIJv2-ablQ/TweetDetail'
+		instructionsPath = ['data', 'threaded_conversation_with_injections_v2', 'instructions']
 		if self._mode is TwitterTweetScraperMode.SINGLE:
-			obj = self._get_api_data(url, _TwitterAPIType.GRAPHQL, params = params)
+			obj = self._get_api_data(url, _TwitterAPIType.GRAPHQL, params = params, instructionsPath = instructionsPath)
 			if not obj['data']:
 				return
 			for instruction in obj['data']['threaded_conversation_with_injections_v2']['instructions']:
 				if instruction['type'] != 'TimelineAddEntries':
 					continue
 				for entry in instruction['entries']:
 					if entry['entryId'] == f'tweet-{self._tweetId}' and entry['content']['entryType'] == 'TimelineTimelineItem' and entry['content']['itemContent']['itemType'] == 'TimelineTweet':
 						yield self._graphql_timeline_tweet_item_result_to_tweet(entry['content']['itemContent']['tweet_results']['result'], tweetId = self._tweetId)
 						break
 		elif self._mode is TwitterTweetScraperMode.SCROLL:
-			for obj in self._iter_api_data(url, _TwitterAPIType.GRAPHQL, params, paginationParams, direction = _ScrollDirection.BOTH):
+			hasModeratedReplies = False
+			for obj in self._iter_api_data(url, _TwitterAPIType.GRAPHQL, params, paginationParams, direction = _ScrollDirection.BOTH, instructionsPath = instructionsPath):
 				if not obj['data']:
 					continue
 				yield from self._graphql_timeline_instructions_to_tweets(obj['data']['threaded_conversation_with_injections_v2']['instructions'], includeConversationThreads = True)
+				hasModeratedReplies = hasModeratedReplies or self._has_moderated_replies(obj, self._tweetId)
+			if hasModeratedReplies:
+				yield from self._get_moderated_replies(self._tweetId)
 		elif self._mode is TwitterTweetScraperMode.RECURSE:
 			seenTweets = set()
 			queue = collections.deque()
 			queue.append(self._tweetId)
 			while queue:
 				tweetId = queue.popleft()
 				thisPagParams = copy.deepcopy(paginationParams)
 				thisPagParams['variables']['focalTweetId'] = str(tweetId)
 				thisParams = copy.deepcopy(thisPagParams)
 				del thisPagParams['variables']['cursor'], thisPagParams['variables']['referrer']
-				for obj in self._iter_api_data(url, _TwitterAPIType.GRAPHQL, thisParams, thisPagParams, direction = _ScrollDirection.BOTH):
+				hasModeratedReplies = False
+				for obj in self._iter_api_data(url, _TwitterAPIType.GRAPHQL, thisParams, thisPagParams, direction = _ScrollDirection.BOTH, instructionsPath = instructionsPath):
 					if not obj['data']:
 						continue
 					for tweet in self._graphql_timeline_instructions_to_tweets(obj['data']['threaded_conversation_with_injections_v2']['instructions'], includeConversationThreads = True):
 						if tweet.id not in seenTweets:
 							yield tweet
 							seenTweets.add(tweet.id)
 							if tweet.id != self._tweetId:  # Already queued at the beginning
 								queue.append(tweet.id)
+					hasModeratedReplies = hasModeratedReplies or self._has_moderated_replies(obj, tweetId)
+				if hasModeratedReplies:
+					for tweet in self._get_moderated_replies(tweetId):
+						if tweet.id not in seenTweets:
+							yield tweet
+							seenTweets.add(tweet.id)
+							queue.append(tweet.id)
+
+	def _has_moderated_replies(self, obj, tweetId):
+		for instruction in obj['data']['threaded_conversation_with_injections_v2']['instructions']:
+			if instruction['type'] != 'TimelineAddEntries':
+				continue
+			for entry in instruction['entries']:
+				if entry['entryId'] == f'tweet-{tweetId}' and entry['content']['entryType'] == 'TimelineTimelineItem' and entry['content']['itemContent']['itemType'] == 'TimelineTweet':
+					return entry['content']['itemContent'].get('hasModeratedReplies', False)
+		return False
+
+	def _get_moderated_replies(self, tweetId):
+		paginationVariables = {
+			'rootTweetId': str(tweetId),
+			'count': 20,
+			'cursor': None,
+			'includePromotedContent': False,
+		}
+		variables = paginationVariables.copy()
+		del variables['cursor']
+		features = {
+			'rweb_lists_timeline_redesign_enabled': True,
+			'responsive_web_graphql_exclude_directive_enabled': True,
+			'verified_phone_label_enabled': False,
+			'creator_subscriptions_tweet_preview_api_enabled': True,
+			'responsive_web_graphql_timeline_navigation_enabled': True,
+			'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+			'tweetypie_unmention_optimization_enabled': True,
+			'responsive_web_edit_tweet_api_enabled': True,
+			'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
+			'view_counts_everywhere_api_enabled': True,
+			'longform_notetweets_consumption_enabled': True,
+			'tweet_awards_web_tipping_enabled': False,
+			'freedom_of_speech_not_reach_fetch_enabled': True,
+			'standardized_nudges_misinfo': True,
+			'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': False,
+			'longform_notetweets_rich_text_read_enabled': True,
+			'longform_notetweets_inline_media_enabled': False,
+			'responsive_web_enhance_cards_enabled': False,
+		}
+
+		params = {'variables': variables, 'features': features}
+		paginationParams = {'variables': paginationVariables, 'features': features}
+		url = 'https://twitter.com/i/api/graphql/pOVQRe-x12WZeawviP7zxw/ModeratedTimeline'
+		instructionsPath = ['data', 'tweet', 'result', 'timeline_response', 'timeline', 'instructions']
+
+		for obj in self._iter_api_data(url, _TwitterAPIType.GRAPHQL, params, paginationParams, direction = _ScrollDirection.BOTH, instructionsPath = instructionsPath):
+			yield from self._graphql_timeline_instructions_to_tweets(obj['data']['tweet']['result']['timeline_response']['timeline']['instructions'], includeConversationThreads = True)
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
 		group = subparser.add_mutually_exclusive_group(required = False)
 		group.add_argument('--scroll', action = 'store_true', default = False, help = 'Enable scrolling in both directions')
 		group.add_argument('--recurse', '--recursive', action = 'store_true', default = False, help = 'Enable recursion through all tweets encountered (warning: slow, potentially memory-intensive!)')
 		subparser.add_argument('tweetId', type = int, help = 'A tweet ID')
@@ -1990,15 +2129,15 @@
 
 	def __init__(self, listName, **kwargs):
 		super().__init__(f'list:{listName}', **kwargs)
 		self._listName = listName
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('list', type = snscrape.base.nonempty_string('list'), help = 'A Twitter list ID or a string of the form "username/listname" (replace spaces with dashes)')
+		subparser.add_argument('list', type = snscrape.utils.nonempty_string_arg('list'), help = 'A Twitter list ID or a string of the form "username/listname" (replace spaces with dashes)')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.list)
 
 
 class TwitterCommunityScraper(_TwitterAPIScraper):
@@ -2011,31 +2150,28 @@
 	def _get_entity(self):
 		self._ensure_guest_token()
 		params = {
 			'variables': {
 				'communityId': str(self._communityId),
 				'withDmMuting': False,
 				'withSafetyModeUserFields': False,
-				'withSuperFollowsUserFields': True,
 			},
 			'features': {
-				'responsive_web_graphql_exclude_directive_enabled': False,
+				'blue_business_profile_image_shape_enabled': True,
+				'responsive_web_graphql_exclude_directive_enabled': True,
 				'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
 				'responsive_web_graphql_timeline_navigation_enabled': True,
-				'responsive_web_twitter_blue_verified_badge_is_enabled': True,
 				'verified_phone_label_enabled': False,
 			},
 		}
-		obj = self._get_api_data('https://api.twitter.com/graphql/MO8cE7aTvaenXJX_teUGcA/CommunitiesFetchOneQuery', _TwitterAPIType.GRAPHQL, params = params)
+		obj = self._get_api_data('https://twitter.com/i/api/graphql/bC3Saf4niY6YuzJWV2oUGg/CommunitiesFetchOneQuery', _TwitterAPIType.GRAPHQL, params = params, instructionsPath = ['data', 'communityResults'])
 		if not obj['data'] or 'result' not in obj['data']['communityResults']:
-			_logger.warning('Empty response')
-			return None
+			raise snscrape.base.ScraperException('Empty response')
 		if obj['data']['communityResults']['result']['__typename'] == 'CommunityUnavailable':
-			_logger.warning('Community unavailable')
-			return None
+			raise snscrape.base.EntityUnavailable('Community unavailable')
 		community = obj['data']['communityResults']['result']
 		optKwargs = {}
 		if 'description' in community:
 			optKwargs['description'] = community['description']
 		return Community(
 			id = int(community['id_str']),
 			name = community['name'],
@@ -2053,49 +2189,47 @@
 
 	def get_items(self):
 		paginationVariables = {
 			'count': 20,
 			'cursor': None,
 			'communityId': str(self._communityId),
 			'withCommunity': True,
-			'withSuperFollowsUserFields': True,
-			'withDownvotePerspective': False,
-			'withReactionsMetadata': False,
-			'withReactionsPerspective': False,
-			'withSuperFollowsTweetFields': True,
 		}
 		variables = paginationVariables.copy()
 		del variables['count'], variables['cursor']
 		features = {
-			'responsive_web_twitter_blue_verified_badge_is_enabled': True,
-			'responsive_web_graphql_exclude_directive_enabled': False,
+			'rweb_lists_timeline_redesign_enabled': False,
+			'blue_business_profile_image_shape_enabled': True,
+			'responsive_web_graphql_exclude_directive_enabled': True,
 			'verified_phone_label_enabled': False,
+			'creator_subscriptions_tweet_preview_api_enabled': False,
 			'responsive_web_graphql_timeline_navigation_enabled': True,
 			'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
 			'tweetypie_unmention_optimization_enabled': True,
 			'vibe_api_enabled': True,
 			'responsive_web_edit_tweet_api_enabled': True,
 			'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
 			'view_counts_everywhere_api_enabled': True,
 			'longform_notetweets_consumption_enabled': True,
 			'tweet_awards_web_tipping_enabled': False,
-			'freedom_of_speech_not_reach_fetch_enabled': False,
+			'freedom_of_speech_not_reach_fetch_enabled': True,
 			'standardized_nudges_misinfo': True,
 			'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': False,
 			'interactive_text_enabled': True,
 			'responsive_web_text_conversations_enabled': False,
+			'longform_notetweets_rich_text_read_enabled': True,
+			'longform_notetweets_inline_media_enabled': False,
 			'responsive_web_enhance_cards_enabled': False,
 		}
 		params = {'variables': variables, 'features': features}
 		paginationParams = {'variables': paginationVariables, 'features': features}
 
-		for obj in self._iter_api_data('https://api.twitter.com/graphql/Qvst9FkHq45wuqicCvMpVw/CommunityTweetsTimeline', _TwitterAPIType.GRAPHQL, params, paginationParams):
+		for obj in self._iter_api_data('https://twitter.com/i/api/graphql/9nnDM-yum8Te--T2REfgkg/CommunityTweetsTimeline', _TwitterAPIType.GRAPHQL, params, paginationParams, instructionsPath = ['data', 'communityResults', 'result', 'community_timeline', 'timeline', 'instructions']):
 			if obj['data']['communityResults']['result']['__typename'] == 'CommunityUnavailable':
-				_logger.warning('Community unavailable')
-				break
+				raise snscrape.base.EntityUnavailable('Community unavailable')
 			yield from self._graphql_timeline_instructions_to_tweets(obj['data']['communityResults']['result']['community_timeline']['timeline']['instructions'])
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
 		subparser.add_argument('communityId', type = int, help = 'A community ID')
 
 	@classmethod
@@ -2149,8 +2283,39 @@
 				if entry['entryId'] != 'trends':
 					continue
 				for item in entry['content']['timelineModule']['items']:
 					trend = item['item']['content']['trend']
 					yield Trend(name = trend['name'], metaDescription = trend['trendMetadata'].get('metaDescription'), domainContext = trend['trendMetadata']['domainContext'])
 
 
-__getattr__, __dir__ = snscrape.base._module_deprecation_helper(__all__, DescriptionURL = TextLink)
+class TwitterUsersScraper(_TwitterAPIScraper):
+	name = 'twitter-users'
+
+	def __init__(self, userIds, **kwargs):
+		self._userIds = userIds
+		super().__init__(f'https://twitter.com/i/user/{self._userIds[0]}', **kwargs)
+
+	def get_items(self):
+		variables = {'userIds': [str(x) for x in self._userIds]}
+		features = {
+			'responsive_web_graphql_exclude_directive_enabled': True,
+			'verified_phone_label_enabled': False,
+			'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+			'responsive_web_graphql_timeline_navigation_enabled': True,
+		}
+		obj = self._get_api_data('https://twitter.com/i/api/graphql/GD4q8bBE2i6cqWw2iT74Gg/UsersByRestIds', _TwitterAPIType.GRAPHQL, params = {'variables': variables, 'features': features}, instructionsPath = ['data', 'users'])
+		for i, u in enumerate(obj['data']['users']):
+			if not u:
+				_logger.warning(f'Skipping empty response object at position {i}')
+				continue
+			yield self._graphql_user_results_to_user(u)
+
+	@classmethod
+	def _cli_setup_parser(cls, subparser):
+		subparser.add_argument('userId', type = int, nargs = '+', help = 'A numeric user ID')
+
+	@classmethod
+	def _cli_from_args(cls, args):
+		return cls._cli_construct(args, args.userId)
+
+
+__getattr__, __dir__ = snscrape.utils.module_deprecation_helper(__all__, DescriptionURL = TextLink)
```

### Comparing `snscrape-0.6.2.20230320/snscrape/modules/vkontakte.py` & `snscrape-0.7.0.20230622/snscrape/modules/vkontakte.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import dataclasses
 import datetime
 import itertools
 import json
 import logging
 import re
 import snscrape.base
+import snscrape.utils
 import typing
 import urllib.parse
 try:
 	import zoneinfo
 except ImportError:
 	# Python 3.8 support; nowadays, Europe/Moscow is always UTC+3, but it's more complicated before 2014, so need proper zone info
 	import pytz
@@ -380,12 +381,12 @@
 			if (topDiv := followersDiv.find('div', class_ = 'header_top')) and topDiv.find('span', class_ = 'header_label').text == 'Followers':
 				kwargs['followers'] = snscrape.base.IntWithGranularity(*parse_num(topDiv.find('span', class_ = 'header_count').text))
 
 		return User(**kwargs)
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
-		subparser.add_argument('username', type = snscrape.base.nonempty_string('username'), help = 'A VK username')
+		subparser.add_argument('username', type = snscrape.utils.nonempty_string_arg('username'), help = 'A VK username')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, args.username)
```

### Comparing `snscrape-0.6.2.20230320/snscrape/modules/weibo.py` & `snscrape-0.7.0.20230622/snscrape/modules/weibo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __all__ = ['Post', 'User', 'WeiboUserScraper']
 
 
 import dataclasses
 import logging
 import re
 import snscrape.base
+import snscrape.utils
 import typing
 
 
 _logger = logging.getLogger(__name__)
 _userDoesNotExist = object()
 _HTML_STRIP_PATTERN = re.compile(r'<[^>]*>')
 
@@ -142,12 +143,12 @@
 			raise snscrape.base.ScraperException('Could not fetch user info')
 		o = r.json()
 		return self._user_info_to_entity(o['data']['userInfo'])
 
 	@classmethod
 	def _cli_setup_parser(cls, subparser):
 		subparser.add_argument('--name', dest = 'isName', action = 'store_true', help = 'Use username instead of user ID')
-		subparser.add_argument('user', type = snscrape.base.nonempty_string('user'), help = 'A user ID')
+		subparser.add_argument('user', type = snscrape.utils.nonempty_string_arg('user'), help = 'A user ID')
 
 	@classmethod
 	def _cli_from_args(cls, args):
 		return cls._cli_construct(args, user = args.user if args.isName else int(args.user))
```

### Comparing `snscrape-0.6.2.20230320/snscrape.egg-info/PKG-INFO` & `snscrape-0.7.0.20230622/snscrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snscrape
-Version: 0.6.2.20230320
+Version: 0.7.0.20230622
 Summary: A social networking service scraper
 Author: JustAnotherArchivist
 Project-URL: repository, https://github.com/JustAnotherArchivist/snscrape
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `snscrape-0.6.2.20230320/snscrape.egg-info/SOURCES.txt` & `snscrape-0.7.0.20230622/snscrape.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 .github/ISSUE_TEMPLATE/bug_report.yml
 .github/ISSUE_TEMPLATE/feature_request.yml
 .github/ISSUE_TEMPLATE/question.md
 snscrape/__init__.py
 snscrape/_cli.py
 snscrape/base.py
+snscrape/utils.py
 snscrape/version.py
 snscrape.egg-info/PKG-INFO
 snscrape.egg-info/SOURCES.txt
 snscrape.egg-info/dependency_links.txt
 snscrape.egg-info/entry_points.txt
 snscrape.egg-info/requires.txt
 snscrape.egg-info/top_level.txt
```

