# Comparing `tmp/es_translator-1.6.0.tar.gz` & `tmp/es_translator-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "es_translator-1.6.0.tar", max compression
+gzip compressed data, was "es_translator-1.6.1.tar", max compression
```

## Comparing `es_translator-1.6.0.tar` & `es_translator-1.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.6.0/LICENSE.txt
--rw-r--r--   0        0        0     3978 2023-05-16 11:15:56.684853 es_translator-1.6.0/README.md
--rw-r--r--   0        0        0      170 2023-06-22 08:22:54.005082 es_translator-1.6.0/es_translator/__init__.py
--rw-r--r--   0        0        0      489 2023-06-22 08:22:53.845080 es_translator-1.6.0/es_translator/alpha.py
--rw-r--r--   0        0        0     7070 2023-06-22 08:22:45.512961 es_translator-1.6.0/es_translator/cli.py
--rw-r--r--   0        0        0     2113 2023-06-22 08:22:54.121084 es_translator-1.6.0/es_translator/es.py
--rw-r--r--   0        0        0    10240 2023-06-22 08:22:49.697021 es_translator-1.6.0/es_translator/es_translator.py
--rw-r--r--   0        0        0       56 2023-06-22 08:22:58.069140 es_translator-1.6.0/es_translator/interpreters/__init__.py
--rw-r--r--   0        0        0     1721 2023-06-22 08:22:58.057140 es_translator-1.6.0/es_translator/interpreters/abstract.py
--rw-r--r--   0        0        0       31 2023-06-22 08:23:26.117539 es_translator-1.6.0/es_translator/interpreters/apertium/__init__.py
--rw-r--r--   0        0        0     6257 2023-06-22 08:23:26.413543 es_translator-1.6.0/es_translator/interpreters/apertium/apertium.py
--rw-r--r--   0        0        0      721 2023-06-22 08:23:26.009537 es_translator-1.6.0/es_translator/interpreters/apertium/pairs.py
--rw-r--r--   0        0        0     5437 2023-06-22 08:23:26.185540 es_translator-1.6.0/es_translator/interpreters/apertium/repository.py
--rw-r--r--   0        0        0       25 2023-06-22 08:23:26.129539 es_translator-1.6.0/es_translator/interpreters/argos/__init__.py
--rw-r--r--   0        0        0     2697 2023-06-22 08:23:26.105538 es_translator-1.6.0/es_translator/interpreters/argos/argos.py
--rw-r--r--   0        0        0      943 2023-06-22 08:22:53.761079 es_translator-1.6.0/es_translator/logger.py
--rw-r--r--   0        0        0      264 2023-06-22 08:22:54.025082 es_translator-1.6.0/es_translator/symlink.py
--rw-r--r--   0        0        0      939 2023-06-22 08:22:53.989082 es_translator-1.6.0/es_translator/tasks.py
--rw-r--r--   0        0        0     1810 2023-06-22 08:22:53.873080 es_translator-1.6.0/es_translator/worker.py
--rw-r--r--   0        0        0     1086 2023-06-22 08:25:56.043672 es_translator-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 es_translator-1.6.0/setup.py
--rw-r--r--   0        0        0     4926 1970-01-01 00:00:00.000000 es_translator-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     3978 2023-05-16 11:15:56.684853 es_translator-1.6.1/README.md
+-rw-r--r--   0        0        0      170 2023-06-22 08:22:54.005082 es_translator-1.6.1/es_translator/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-22 08:22:53.845080 es_translator-1.6.1/es_translator/alpha.py
+-rw-r--r--   0        0        0     7012 2023-06-22 09:40:41.678686 es_translator-1.6.1/es_translator/cli.py
+-rw-r--r--   0        0        0     2113 2023-06-22 08:22:54.121084 es_translator-1.6.1/es_translator/es.py
+-rw-r--r--   0        0        0    10840 2023-06-22 09:51:21.047378 es_translator-1.6.1/es_translator/es_translator.py
+-rw-r--r--   0        0        0       56 2023-06-22 08:22:58.069140 es_translator-1.6.1/es_translator/interpreters/__init__.py
+-rw-r--r--   0        0        0     1721 2023-06-22 08:22:58.057140 es_translator-1.6.1/es_translator/interpreters/abstract.py
+-rw-r--r--   0        0        0       31 2023-06-22 08:23:26.117539 es_translator-1.6.1/es_translator/interpreters/apertium/__init__.py
+-rw-r--r--   0        0        0     6257 2023-06-22 08:23:26.413543 es_translator-1.6.1/es_translator/interpreters/apertium/apertium.py
+-rw-r--r--   0        0        0      721 2023-06-22 08:23:26.009537 es_translator-1.6.1/es_translator/interpreters/apertium/pairs.py
+-rw-r--r--   0        0        0     5437 2023-06-22 08:23:26.185540 es_translator-1.6.1/es_translator/interpreters/apertium/repository.py
+-rw-r--r--   0        0        0       25 2023-06-22 08:23:26.129539 es_translator-1.6.1/es_translator/interpreters/argos/__init__.py
+-rw-r--r--   0        0        0     2697 2023-06-22 08:23:26.105538 es_translator-1.6.1/es_translator/interpreters/argos/argos.py
+-rw-r--r--   0        0        0      943 2023-06-22 08:22:53.761079 es_translator-1.6.1/es_translator/logger.py
+-rw-r--r--   0        0        0      264 2023-06-22 08:22:54.025082 es_translator-1.6.1/es_translator/symlink.py
+-rw-r--r--   0        0        0      939 2023-06-22 08:22:53.989082 es_translator-1.6.1/es_translator/tasks.py
+-rw-r--r--   0        0        0     1810 2023-06-22 08:22:53.873080 es_translator-1.6.1/es_translator/worker.py
+-rw-r--r--   0        0        0     1086 2023-06-22 09:56:32.679196 es_translator-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 es_translator-1.6.1/setup.py
+-rw-r--r--   0        0        0     4926 1970-01-01 00:00:00.000000 es_translator-1.6.1/PKG-INFO
```

### Comparing `es_translator-1.6.0/LICENSE.txt` & `es_translator-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/README.md` & `es_translator-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/es_translator/cli.py` & `es_translator-1.6.1/es_translator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,18 +113,16 @@
     add_syslog_handler(syslog_address, syslog_port, syslog_facility)
     add_stdout_handler(options['stdout_loglevel'])
     # Configure celery app broker url globally
     celery_app.conf.broker_url = options['redis_url']
     # We setup the translator. Etheir if the translation is done now
     # or later, we need initialize the interpreter (Argos, Apertium, ...)
     es_translator = EsTranslator(options)
-    if options['plan']:
-        es_translator.plan()
-    else:
-        es_translator.start()
+    es_translator.start()
+        
 
 
 @click.command()
 @click.option('--broker', default='redis://redis', help='Celery broker URL.')
 @click.option('--concurrency', default=1, help='Celery broker URL.')
 @click.option('--stdout-loglevel',
               help='Change the default log level for stdout error handler',
```

### Comparing `es_translator-1.6.0/es_translator/es.py` & `es_translator-1.6.1/es_translator/es.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/es_translator/es_translator.py` & `es_translator-1.6.1/es_translator/es_translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from contextlib import contextmanager
 from elasticsearch import Elasticsearch, ElasticsearchException
 from elasticsearch_dsl import Document, Search
 from multiprocessing import Pool, JoinableQueue, Manager
 from queue import Full
 from os import path
 from rich.progress import Progress
-from typing import Any, ContextManager, Dict
+from typing import Any, ContextManager, Dict, List
 
 # Module from the same package
 from es_translator.interpreters import Apertium, Argos
 from es_translator.logger import logger
 from es_translator.worker import translation_worker, FatalTranslationException
 from es_translator.tasks import translate_document_task
 from es_translator.es import TranslatedHit
@@ -36,44 +36,53 @@
         self.scan_scroll = options['scan_scroll']
         self.dry_run = options['dry_run']
         self.pool_size = options['pool_size']
         self.pool_timeout = options['pool_timeout']
         self.throttle = options['throttle']
         self.progressbar = options['progressbar']
         self.interpreter_name = options['interpreter']
+        self.plan = options['plan']
 
     @property
     def no_progressbar(self) -> bool:
         """Check if the progressbar option is set to False.
 
         Returns:
             bool: True if the progressbar option is False, else False.
         """
         return not self.progressbar
 
     def start(self) -> None:
+        """Starts or plans the translation process."""
+        if self.plan:
+            self.start_later()
+        else:
+            self.start_now()
+
+    def start_now(self) -> None:
         """Starts the translation process."""
         self.instantiate_interpreter()
         total = self.search().count()
         desc = 'Translating %s document(s)' % total
         with self.print_done(desc):
             search = self.configure_search()
             translation_queue = self.create_translation_queue()
             with self.with_shared_fatal_error() as shared_fatal_error:
                 self.translate_documents_in_pool(
                     search, translation_queue, shared_fatal_error, total)
 
-    def plan(self):
+    def start_later(self):
         """Plan the translation process."""
         self.instantiate_interpreter()
         total = self.search().count()
         desc = f"Planning translation for {total} document{'s'[:total^1]}"
         with self.print_done(desc):
             search = self.configure_search()
             for hit in search.scan():
+                logger.info(f'Planned translation for doc {hit.meta.id}')
                 translate_document_task.delay(self.options, hit.meta.to_dict())
 
     @property
     def options(self):
         return {
             'url': self.url,
             'index': self.index,
@@ -107,18 +116,29 @@
     def configure_search(self) -> Search:
         """Configures the search object.
 
         Returns:
             Search: A configured search object.
         """
         search = self.search()
-        search = search.source(
-            [self.source_field, self.target_field, '_routing', '_id'])
+        search = search.source(self.search_source)
         search = search.params(scroll=self.scan_scroll, size=self.pool_size)
         return search
+    
+    @property
+    def search_source(self) -> List[str]:
+        """Gets the list of fields to use in the search.
+
+        Returns: 
+            List[str]: list of fields to use in the search.
+        """
+        if self.plan:
+            return ['_routing', '_id']
+        return [self.source_field, self.target_field, '_routing', '_id']
+
 
     def create_translation_queue(self) -> JoinableQueue:
         """Creates a queue that can translate documents in parallel.
 
         Returns:
             JoinableQueue: A queue for parallel document translation.
         """
```

### Comparing `es_translator-1.6.0/es_translator/interpreters/abstract.py` & `es_translator-1.6.1/es_translator/interpreters/abstract.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/es_translator/interpreters/apertium/apertium.py` & `es_translator-1.6.1/es_translator/interpreters/apertium/apertium.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/es_translator/interpreters/apertium/pairs.py` & `es_translator-1.6.1/es_translator/interpreters/apertium/pairs.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/es_translator/interpreters/apertium/repository.py` & `es_translator-1.6.1/es_translator/interpreters/apertium/repository.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/es_translator/interpreters/argos/argos.py` & `es_translator-1.6.1/es_translator/interpreters/argos/argos.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/es_translator/logger.py` & `es_translator-1.6.1/es_translator/logger.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/es_translator/tasks.py` & `es_translator-1.6.1/es_translator/tasks.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/es_translator/worker.py` & `es_translator-1.6.1/es_translator/worker.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.6.0/pyproject.toml` & `es_translator-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "es-translator"
-version = "1.6.0"
+version = "1.6.1"
 description = "A lazy yet bulletproof machine translation tool for Elastichsearch."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 license = "GNU AFFERO GENERAL PUBLIC LICENSE"
 packages = [{include = "es_translator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `es_translator-1.6.0/setup.py` & `es_translator-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 entry_points = \
 {'console_scripts': ['es-translator = es_translator.cli:translate',
                      'es-translator-pairs = es_translator.cli:pairs',
                      'es-translator-tasks = es_translator.cli:tasks']}
 
 setup_kwargs = {
     'name': 'es-translator',
-    'version': '1.6.0',
+    'version': '1.6.1',
     'description': 'A lazy yet bulletproof machine translation tool for Elastichsearch.',
     'long_description': '# ES Translator\n\n[![CircleCI](https://circleci.com/gh/ICIJ/es-translator.svg?style=svg)](https://circleci.com/gh/ICIJ/es-translator)\n\nA lazy yet bulletproof machine translation tool for Elastichsearch.\n\n```\nUsage: es-translator [OPTIONS]\n\nOptions:\n  -u, --url TEXT                  Elastichsearch URL\n  -i, --index TEXT                Elastichsearch Index  [required]\n  -r, --interpreter TEXT          Interpreter to use to perform the\n                                  translation\n  -s, --source-language TEXT      Source language to translate from\n                                  [required]\n  -t, --target-language TEXT      Target language to translate to  [required]\n  --intermediary-language TEXT    An intermediary language to use when no\n                                  translation is available between the source\n                                  and the target. If none is provided this\n                                  will be calculated automatically.\n  --source-field TEXT             Document field to translate\n  --target-field TEXT             Document field where the translations are\n                                  stored\n  -q, --query-string TEXT         Search query string to filter result\n  -d, --data-dir PATH             Path to the directory where to language\n                                  model will be downloaded\n  --scan-scroll TEXT              Scroll duration (set to higher value if\n                                  you\'re processing a lot of documents)\n  --dry-run                       Don\'t save anything in Elasticsearch\n  --pool-size INTEGER             Number of parallel processes to start\n  --pool-timeout INTEGER          Timeout to add a translation\n  --throttle INTEGER              Throttle between each translation (in ms)\n  --syslog-address TEXT           Syslog address\n  --syslog-port INTEGER           Syslog port\n  --syslog-facility TEXT          Syslog facility\n  --stdout-loglevel TEXT          Change the default log level for stdout\n                                  error handler\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --help                          Show this message and exit.\n```\n\n## Installation (Ubuntu)\n\nInstall Apertium:\n\n```\nwget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash\nsudo apt install apertium-all-dev\n```\n\nCreate a Virtualenv and install Pip packages with Poetry:\n\n```\nmake install\n```\n\nOn Ubuntu 22.04 some additional packages might be needed if you use the version from Ubuntu\'s repository:\n\n```\nsudo apt install cg3 apertium-get apertium-lex-tools\n```\n\n\n## Installation (Docker)\n\nNothing to do as long as you have Docker on your system:\n\n```\ndocker run -it icij/es-translator poetry run es-translator --help\n```\n\n## Examples\n\nTranslates documents from French to Spanish on a local Elasticsearch. The translated field is `content` (the default).\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es\n```\n\nTranslates documents from French to English on a local Elasticsearch using Apertium:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language en --interpreter apertium\n```\n\nTo translate the `title` field we could do:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es --source-field title\n```\n\nTranslates documents from English to Spanish on a local Elasticsearch using 4 threads:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language en --target-language es --pool-size 4\n```\n\nTranslates documents from Portuguese to English, using an intermediary language (Apertium doesn\'t offer this translation pair):\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language pt --intermediary-language es --target-language en\n```\n',
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `es_translator-1.6.0/PKG-INFO` & `es_translator-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: es-translator
-Version: 1.6.0
+Version: 1.6.1
 Summary: A lazy yet bulletproof machine translation tool for Elastichsearch.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.2,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

