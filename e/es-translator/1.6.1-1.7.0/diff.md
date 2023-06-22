# Comparing `tmp/es_translator-1.6.1.tar.gz` & `tmp/es_translator-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "es_translator-1.6.1.tar", max compression
+gzip compressed data, was "es_translator-1.7.0.tar", max compression
```

## Comparing `es_translator-1.6.1.tar` & `es_translator-1.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.6.1/LICENSE.txt
--rw-r--r--   0        0        0     3978 2023-05-16 11:15:56.684853 es_translator-1.6.1/README.md
--rw-r--r--   0        0        0      170 2023-06-22 08:22:54.005082 es_translator-1.6.1/es_translator/__init__.py
--rw-r--r--   0        0        0      489 2023-06-22 08:22:53.845080 es_translator-1.6.1/es_translator/alpha.py
--rw-r--r--   0        0        0     7012 2023-06-22 09:40:41.678686 es_translator-1.6.1/es_translator/cli.py
--rw-r--r--   0        0        0     2113 2023-06-22 08:22:54.121084 es_translator-1.6.1/es_translator/es.py
--rw-r--r--   0        0        0    10840 2023-06-22 09:51:21.047378 es_translator-1.6.1/es_translator/es_translator.py
--rw-r--r--   0        0        0       56 2023-06-22 08:22:58.069140 es_translator-1.6.1/es_translator/interpreters/__init__.py
--rw-r--r--   0        0        0     1721 2023-06-22 08:22:58.057140 es_translator-1.6.1/es_translator/interpreters/abstract.py
--rw-r--r--   0        0        0       31 2023-06-22 08:23:26.117539 es_translator-1.6.1/es_translator/interpreters/apertium/__init__.py
--rw-r--r--   0        0        0     6257 2023-06-22 08:23:26.413543 es_translator-1.6.1/es_translator/interpreters/apertium/apertium.py
--rw-r--r--   0        0        0      721 2023-06-22 08:23:26.009537 es_translator-1.6.1/es_translator/interpreters/apertium/pairs.py
--rw-r--r--   0        0        0     5437 2023-06-22 08:23:26.185540 es_translator-1.6.1/es_translator/interpreters/apertium/repository.py
--rw-r--r--   0        0        0       25 2023-06-22 08:23:26.129539 es_translator-1.6.1/es_translator/interpreters/argos/__init__.py
--rw-r--r--   0        0        0     2697 2023-06-22 08:23:26.105538 es_translator-1.6.1/es_translator/interpreters/argos/argos.py
--rw-r--r--   0        0        0      943 2023-06-22 08:22:53.761079 es_translator-1.6.1/es_translator/logger.py
--rw-r--r--   0        0        0      264 2023-06-22 08:22:54.025082 es_translator-1.6.1/es_translator/symlink.py
--rw-r--r--   0        0        0      939 2023-06-22 08:22:53.989082 es_translator-1.6.1/es_translator/tasks.py
--rw-r--r--   0        0        0     1810 2023-06-22 08:22:53.873080 es_translator-1.6.1/es_translator/worker.py
--rw-r--r--   0        0        0     1086 2023-06-22 09:56:32.679196 es_translator-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 es_translator-1.6.1/setup.py
--rw-r--r--   0        0        0     4926 1970-01-01 00:00:00.000000 es_translator-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     3998 2023-06-22 10:58:57.612690 es_translator-1.7.0/README.md
+-rw-r--r--   0        0        0      170 2023-06-22 08:22:54.005082 es_translator-1.7.0/es_translator/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-22 08:22:53.845080 es_translator-1.7.0/es_translator/alpha.py
+-rw-r--r--   0        0        0     7043 2023-06-22 10:56:35.367338 es_translator-1.7.0/es_translator/cli.py
+-rw-r--r--   0        0        0     2113 2023-06-22 08:22:54.121084 es_translator-1.7.0/es_translator/es.py
+-rw-r--r--   0        0        0    10888 2023-06-22 11:14:23.660028 es_translator-1.7.0/es_translator/es_translator.py
+-rw-r--r--   0        0        0       56 2023-06-22 08:22:58.069140 es_translator-1.7.0/es_translator/interpreters/__init__.py
+-rw-r--r--   0        0        0     1721 2023-06-22 08:22:58.057140 es_translator-1.7.0/es_translator/interpreters/abstract.py
+-rw-r--r--   0        0        0       31 2023-06-22 08:23:26.117539 es_translator-1.7.0/es_translator/interpreters/apertium/__init__.py
+-rw-r--r--   0        0        0     6257 2023-06-22 08:23:26.413543 es_translator-1.7.0/es_translator/interpreters/apertium/apertium.py
+-rw-r--r--   0        0        0      721 2023-06-22 08:23:26.009537 es_translator-1.7.0/es_translator/interpreters/apertium/pairs.py
+-rw-r--r--   0        0        0     5437 2023-06-22 08:23:26.185540 es_translator-1.7.0/es_translator/interpreters/apertium/repository.py
+-rw-r--r--   0        0        0       25 2023-06-22 08:23:26.129539 es_translator-1.7.0/es_translator/interpreters/argos/__init__.py
+-rw-r--r--   0        0        0     2697 2023-06-22 08:23:26.105538 es_translator-1.7.0/es_translator/interpreters/argos/argos.py
+-rw-r--r--   0        0        0      943 2023-06-22 08:22:53.761079 es_translator-1.7.0/es_translator/logger.py
+-rw-r--r--   0        0        0      264 2023-06-22 08:22:54.025082 es_translator-1.7.0/es_translator/symlink.py
+-rw-r--r--   0        0        0      939 2023-06-22 08:22:53.989082 es_translator-1.7.0/es_translator/tasks.py
+-rw-r--r--   0        0        0     1810 2023-06-22 08:22:53.873080 es_translator-1.7.0/es_translator/worker.py
+-rw-r--r--   0        0        0     1086 2023-06-22 11:16:24.641039 es_translator-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5398 1970-01-01 00:00:00.000000 es_translator-1.7.0/setup.py
+-rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 es_translator-1.7.0/PKG-INFO
```

### Comparing `es_translator-1.6.1/LICENSE.txt` & `es_translator-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/README.md` & `es_translator-1.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# ES Translator
+# ES Translator [![](https://img.shields.io/github/actions/workflow/status/icij/es-translator/main.yml)](https://github.com/ICIJ/es-translator/actions)
 
-[![CircleCI](https://circleci.com/gh/ICIJ/es-translator.svg?style=svg)](https://circleci.com/gh/ICIJ/es-translator)
 
 A lazy yet bulletproof machine translation tool for Elastichsearch.
 
 ```
 Usage: es-translator [OPTIONS]
 
 Options:
```

### Comparing `es_translator-1.6.1/es_translator/cli.py` & `es_translator-1.7.0/es_translator/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,40 +101,40 @@
               help='Display a progressbar',
               default=None,
               callback=validate_progressbar)
 @click.option('--plan',
               help='Plan translations into a queue instead of processing them npw',
               is_flag=True,
               default=False)
-@click.option('--redis-url',
-              help='Redis URL (only needed when planning translation)',
+@click.option('--broker-url',
+              help='Celery broker URL (only needed when planning translation)',
               default='redis://localhost:6379')
 def translate(syslog_address, syslog_port, syslog_facility, **options):
     # Configure Syslog handler
     add_syslog_handler(syslog_address, syslog_port, syslog_facility)
     add_stdout_handler(options['stdout_loglevel'])
     # Configure celery app broker url globally
-    celery_app.conf.broker_url = options['redis_url']
+    celery_app.conf.broker_url = options['broker_url']
     # We setup the translator. Etheir if the translation is done now
     # or later, we need initialize the interpreter (Argos, Apertium, ...)
     es_translator = EsTranslator(options)
     es_translator.start()
         
 
 
 @click.command()
-@click.option('--broker', default='redis://redis', help='Celery broker URL.')
-@click.option('--concurrency', default=1, help='Celery broker URL.')
+@click.option('--broker-url', default='redis://redis', help='Celery broker URL')
+@click.option('--concurrency', default=1, help='Number of concurrent workers')
 @click.option('--stdout-loglevel',
               help='Change the default log level for stdout error handler',
               default='ERROR',
               callback=validate_loglevel)
-def tasks(broker, concurrency, stdout_loglevel):
+def tasks(broker_url, concurrency, stdout_loglevel):
     """Starts a Celery worker."""
-    celery_app.conf.broker_url = broker
+    celery_app.conf.broker_url = broker_url
     argv = [
         'worker',
         '--concurrency',
         concurrency,
         '--loglevel',
         stdout_loglevel]
     celery_app.worker_main(argv)
```

### Comparing `es_translator-1.6.1/es_translator/es.py` & `es_translator-1.7.0/es_translator/es.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/es_translator/es_translator.py` & `es_translator-1.7.0/es_translator/es_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,21 +30,21 @@
         self.target_language = options['target_language']
         self.intermediary_language = options['intermediary_language']
         self.source_field = options['source_field']
         self.target_field = options['target_field']
         self.query_string = options['query_string']
         self.data_dir = options['data_dir']
         self.scan_scroll = options['scan_scroll']
-        self.dry_run = options['dry_run']
+        self.dry_run = getattr(options, 'dry_run', False)
         self.pool_size = options['pool_size']
         self.pool_timeout = options['pool_timeout']
         self.throttle = options['throttle']
-        self.progressbar = options['progressbar']
+        self.progressbar = getattr(options, 'progressbar', False)
         self.interpreter_name = options['interpreter']
-        self.plan = options['plan']
+        self.plan = getattr(options, 'plan', False)
 
     @property
     def no_progressbar(self) -> bool:
         """Check if the progressbar option is set to False.
 
         Returns:
             bool: True if the progressbar option is False, else False.
```

### Comparing `es_translator-1.6.1/es_translator/interpreters/abstract.py` & `es_translator-1.7.0/es_translator/interpreters/abstract.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/es_translator/interpreters/apertium/apertium.py` & `es_translator-1.7.0/es_translator/interpreters/apertium/apertium.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/es_translator/interpreters/apertium/pairs.py` & `es_translator-1.7.0/es_translator/interpreters/apertium/pairs.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/es_translator/interpreters/apertium/repository.py` & `es_translator-1.7.0/es_translator/interpreters/apertium/repository.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/es_translator/interpreters/argos/argos.py` & `es_translator-1.7.0/es_translator/interpreters/argos/argos.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/es_translator/logger.py` & `es_translator-1.7.0/es_translator/logger.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/es_translator/tasks.py` & `es_translator-1.7.0/es_translator/tasks.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/es_translator/worker.py` & `es_translator-1.7.0/es_translator/worker.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.1/pyproject.toml` & `es_translator-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "es-translator"
-version = "1.6.1"
+version = "1.7.0"
 description = "A lazy yet bulletproof machine translation tool for Elastichsearch."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 license = "GNU AFFERO GENERAL PUBLIC LICENSE"
 packages = [{include = "es_translator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `es_translator-1.6.1/setup.py` & `es_translator-1.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 entry_points = \
 {'console_scripts': ['es-translator = es_translator.cli:translate',
                      'es-translator-pairs = es_translator.cli:pairs',
                      'es-translator-tasks = es_translator.cli:tasks']}
 
 setup_kwargs = {
     'name': 'es-translator',
-    'version': '1.6.1',
+    'version': '1.7.0',
     'description': 'A lazy yet bulletproof machine translation tool for Elastichsearch.',
-    'long_description': '# ES Translator\n\n[![CircleCI](https://circleci.com/gh/ICIJ/es-translator.svg?style=svg)](https://circleci.com/gh/ICIJ/es-translator)\n\nA lazy yet bulletproof machine translation tool for Elastichsearch.\n\n```\nUsage: es-translator [OPTIONS]\n\nOptions:\n  -u, --url TEXT                  Elastichsearch URL\n  -i, --index TEXT                Elastichsearch Index  [required]\n  -r, --interpreter TEXT          Interpreter to use to perform the\n                                  translation\n  -s, --source-language TEXT      Source language to translate from\n                                  [required]\n  -t, --target-language TEXT      Target language to translate to  [required]\n  --intermediary-language TEXT    An intermediary language to use when no\n                                  translation is available between the source\n                                  and the target. If none is provided this\n                                  will be calculated automatically.\n  --source-field TEXT             Document field to translate\n  --target-field TEXT             Document field where the translations are\n                                  stored\n  -q, --query-string TEXT         Search query string to filter result\n  -d, --data-dir PATH             Path to the directory where to language\n                                  model will be downloaded\n  --scan-scroll TEXT              Scroll duration (set to higher value if\n                                  you\'re processing a lot of documents)\n  --dry-run                       Don\'t save anything in Elasticsearch\n  --pool-size INTEGER             Number of parallel processes to start\n  --pool-timeout INTEGER          Timeout to add a translation\n  --throttle INTEGER              Throttle between each translation (in ms)\n  --syslog-address TEXT           Syslog address\n  --syslog-port INTEGER           Syslog port\n  --syslog-facility TEXT          Syslog facility\n  --stdout-loglevel TEXT          Change the default log level for stdout\n                                  error handler\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --help                          Show this message and exit.\n```\n\n## Installation (Ubuntu)\n\nInstall Apertium:\n\n```\nwget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash\nsudo apt install apertium-all-dev\n```\n\nCreate a Virtualenv and install Pip packages with Poetry:\n\n```\nmake install\n```\n\nOn Ubuntu 22.04 some additional packages might be needed if you use the version from Ubuntu\'s repository:\n\n```\nsudo apt install cg3 apertium-get apertium-lex-tools\n```\n\n\n## Installation (Docker)\n\nNothing to do as long as you have Docker on your system:\n\n```\ndocker run -it icij/es-translator poetry run es-translator --help\n```\n\n## Examples\n\nTranslates documents from French to Spanish on a local Elasticsearch. The translated field is `content` (the default).\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es\n```\n\nTranslates documents from French to English on a local Elasticsearch using Apertium:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language en --interpreter apertium\n```\n\nTo translate the `title` field we could do:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es --source-field title\n```\n\nTranslates documents from English to Spanish on a local Elasticsearch using 4 threads:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language en --target-language es --pool-size 4\n```\n\nTranslates documents from Portuguese to English, using an intermediary language (Apertium doesn\'t offer this translation pair):\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language pt --intermediary-language es --target-language en\n```\n',
+    'long_description': '# ES Translator [![](https://img.shields.io/github/actions/workflow/status/icij/es-translator/main.yml)](https://github.com/ICIJ/es-translator/actions)\n\n\nA lazy yet bulletproof machine translation tool for Elastichsearch.\n\n```\nUsage: es-translator [OPTIONS]\n\nOptions:\n  -u, --url TEXT                  Elastichsearch URL\n  -i, --index TEXT                Elastichsearch Index  [required]\n  -r, --interpreter TEXT          Interpreter to use to perform the\n                                  translation\n  -s, --source-language TEXT      Source language to translate from\n                                  [required]\n  -t, --target-language TEXT      Target language to translate to  [required]\n  --intermediary-language TEXT    An intermediary language to use when no\n                                  translation is available between the source\n                                  and the target. If none is provided this\n                                  will be calculated automatically.\n  --source-field TEXT             Document field to translate\n  --target-field TEXT             Document field where the translations are\n                                  stored\n  -q, --query-string TEXT         Search query string to filter result\n  -d, --data-dir PATH             Path to the directory where to language\n                                  model will be downloaded\n  --scan-scroll TEXT              Scroll duration (set to higher value if\n                                  you\'re processing a lot of documents)\n  --dry-run                       Don\'t save anything in Elasticsearch\n  --pool-size INTEGER             Number of parallel processes to start\n  --pool-timeout INTEGER          Timeout to add a translation\n  --throttle INTEGER              Throttle between each translation (in ms)\n  --syslog-address TEXT           Syslog address\n  --syslog-port INTEGER           Syslog port\n  --syslog-facility TEXT          Syslog facility\n  --stdout-loglevel TEXT          Change the default log level for stdout\n                                  error handler\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --help                          Show this message and exit.\n```\n\n## Installation (Ubuntu)\n\nInstall Apertium:\n\n```\nwget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash\nsudo apt install apertium-all-dev\n```\n\nCreate a Virtualenv and install Pip packages with Poetry:\n\n```\nmake install\n```\n\nOn Ubuntu 22.04 some additional packages might be needed if you use the version from Ubuntu\'s repository:\n\n```\nsudo apt install cg3 apertium-get apertium-lex-tools\n```\n\n\n## Installation (Docker)\n\nNothing to do as long as you have Docker on your system:\n\n```\ndocker run -it icij/es-translator poetry run es-translator --help\n```\n\n## Examples\n\nTranslates documents from French to Spanish on a local Elasticsearch. The translated field is `content` (the default).\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es\n```\n\nTranslates documents from French to English on a local Elasticsearch using Apertium:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language en --interpreter apertium\n```\n\nTo translate the `title` field we could do:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es --source-field title\n```\n\nTranslates documents from English to Spanish on a local Elasticsearch using 4 threads:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language en --target-language es --pool-size 4\n```\n\nTranslates documents from Portuguese to English, using an intermediary language (Apertium doesn\'t offer this translation pair):\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language pt --intermediary-language es --target-language en\n```\n',
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `es_translator-1.6.1/PKG-INFO` & `es_translator-1.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: es-translator
-Version: 1.6.1
+Version: 1.7.0
 Summary: A lazy yet bulletproof machine translation tool for Elastichsearch.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.2,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -20,17 +20,16 @@
 Requires-Dist: pycountry (>=22.3,<23.0)
 Requires-Dist: rich (>=12,<13)
 Requires-Dist: sh (>=1,<2)
 Requires-Dist: torch (>=1.13,<2.0)
 Requires-Dist: urllib3 (>=1.26,<2.0)
 Description-Content-Type: text/markdown
 
-# ES Translator
+# ES Translator [![](https://img.shields.io/github/actions/workflow/status/icij/es-translator/main.yml)](https://github.com/ICIJ/es-translator/actions)
 
-[![CircleCI](https://circleci.com/gh/ICIJ/es-translator.svg?style=svg)](https://circleci.com/gh/ICIJ/es-translator)
 
 A lazy yet bulletproof machine translation tool for Elastichsearch.
 
 ```
 Usage: es-translator [OPTIONS]
 
 Options:
```

