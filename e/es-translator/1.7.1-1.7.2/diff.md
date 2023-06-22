# Comparing `tmp/es_translator-1.7.1.tar.gz` & `tmp/es_translator-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "es_translator-1.7.1.tar", max compression
+gzip compressed data, was "es_translator-1.7.2.tar", max compression
```

## Comparing `es_translator-1.7.1.tar` & `es_translator-1.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.7.1/LICENSE.txt
--rw-r--r--   0        0        0     3998 2023-06-22 10:58:57.612690 es_translator-1.7.1/README.md
--rw-r--r--   0        0        0      170 2023-06-22 08:22:54.005082 es_translator-1.7.1/es_translator/__init__.py
--rw-r--r--   0        0        0      489 2023-06-22 08:22:53.845080 es_translator-1.7.1/es_translator/alpha.py
--rw-r--r--   0        0        0     7043 2023-06-22 10:56:35.367338 es_translator-1.7.1/es_translator/cli.py
--rw-r--r--   0        0        0     2113 2023-06-22 08:22:54.121084 es_translator-1.7.1/es_translator/es.py
--rw-r--r--   0        0        0    10873 2023-06-22 11:45:04.655543 es_translator-1.7.1/es_translator/es_translator.py
--rw-r--r--   0        0        0       56 2023-06-22 08:22:58.069140 es_translator-1.7.1/es_translator/interpreters/__init__.py
--rw-r--r--   0        0        0     1721 2023-06-22 08:22:58.057140 es_translator-1.7.1/es_translator/interpreters/abstract.py
--rw-r--r--   0        0        0       31 2023-06-22 08:23:26.117539 es_translator-1.7.1/es_translator/interpreters/apertium/__init__.py
--rw-r--r--   0        0        0     6257 2023-06-22 08:23:26.413543 es_translator-1.7.1/es_translator/interpreters/apertium/apertium.py
--rw-r--r--   0        0        0      721 2023-06-22 08:23:26.009537 es_translator-1.7.1/es_translator/interpreters/apertium/pairs.py
--rw-r--r--   0        0        0     5437 2023-06-22 08:23:26.185540 es_translator-1.7.1/es_translator/interpreters/apertium/repository.py
--rw-r--r--   0        0        0       25 2023-06-22 08:23:26.129539 es_translator-1.7.1/es_translator/interpreters/argos/__init__.py
--rw-r--r--   0        0        0     2697 2023-06-22 08:23:26.105538 es_translator-1.7.1/es_translator/interpreters/argos/argos.py
--rw-r--r--   0        0        0      943 2023-06-22 08:22:53.761079 es_translator-1.7.1/es_translator/logger.py
--rw-r--r--   0        0        0      264 2023-06-22 08:22:54.025082 es_translator-1.7.1/es_translator/symlink.py
--rw-r--r--   0        0        0      939 2023-06-22 08:22:53.989082 es_translator-1.7.1/es_translator/tasks.py
--rw-r--r--   0        0        0     1810 2023-06-22 08:22:53.873080 es_translator-1.7.1/es_translator/worker.py
--rw-r--r--   0        0        0     1086 2023-06-22 11:46:23.508169 es_translator-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     5398 1970-01-01 00:00:00.000000 es_translator-1.7.1/setup.py
--rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 es_translator-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.7.2/LICENSE.txt
+-rw-r--r--   0        0        0     4100 2023-06-22 12:52:39.253316 es_translator-1.7.2/README.md
+-rw-r--r--   0        0        0      170 2023-06-22 08:22:54.005082 es_translator-1.7.2/es_translator/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-22 08:22:53.845080 es_translator-1.7.2/es_translator/alpha.py
+-rw-r--r--   0        0        0     7043 2023-06-22 10:56:35.367338 es_translator-1.7.2/es_translator/cli.py
+-rw-r--r--   0        0        0     2113 2023-06-22 08:22:54.121084 es_translator-1.7.2/es_translator/es.py
+-rw-r--r--   0        0        0    10873 2023-06-22 11:45:04.655543 es_translator-1.7.2/es_translator/es_translator.py
+-rw-r--r--   0        0        0       56 2023-06-22 08:22:58.069140 es_translator-1.7.2/es_translator/interpreters/__init__.py
+-rw-r--r--   0        0        0     1721 2023-06-22 08:22:58.057140 es_translator-1.7.2/es_translator/interpreters/abstract.py
+-rw-r--r--   0        0        0       31 2023-06-22 08:23:26.117539 es_translator-1.7.2/es_translator/interpreters/apertium/__init__.py
+-rw-r--r--   0        0        0     6257 2023-06-22 08:23:26.413543 es_translator-1.7.2/es_translator/interpreters/apertium/apertium.py
+-rw-r--r--   0        0        0      721 2023-06-22 08:23:26.009537 es_translator-1.7.2/es_translator/interpreters/apertium/pairs.py
+-rw-r--r--   0        0        0     5437 2023-06-22 08:23:26.185540 es_translator-1.7.2/es_translator/interpreters/apertium/repository.py
+-rw-r--r--   0        0        0       25 2023-06-22 08:23:26.129539 es_translator-1.7.2/es_translator/interpreters/argos/__init__.py
+-rw-r--r--   0        0        0     2806 2023-06-22 13:06:16.747494 es_translator-1.7.2/es_translator/interpreters/argos/argos.py
+-rw-r--r--   0        0        0      943 2023-06-22 08:22:53.761079 es_translator-1.7.2/es_translator/logger.py
+-rw-r--r--   0        0        0      264 2023-06-22 08:22:54.025082 es_translator-1.7.2/es_translator/symlink.py
+-rw-r--r--   0        0        0      939 2023-06-22 08:22:53.989082 es_translator-1.7.2/es_translator/tasks.py
+-rw-r--r--   0        0        0     1810 2023-06-22 08:22:53.873080 es_translator-1.7.2/es_translator/worker.py
+-rw-r--r--   0        0        0     1086 2023-06-22 13:08:05.112331 es_translator-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 es_translator-1.7.2/setup.py
+-rw-r--r--   0        0        0     5048 1970-01-01 00:00:00.000000 es_translator-1.7.2/PKG-INFO
```

### Comparing `es_translator-1.7.1/LICENSE.txt` & `es_translator-1.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/README.md` & `es_translator-1.7.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ES Translator [![](https://img.shields.io/github/actions/workflow/status/icij/es-translator/main.yml)](https://github.com/ICIJ/es-translator/actions)
+# ES Translator [![](https://img.shields.io/github/actions/workflow/status/icij/es-translator/main.yml)](https://github.com/ICIJ/es-translator/actions) [![](https://img.shields.io/pypi/pyversions/es-translator)](https://pypi.org/project/es-translator/) 
 
 
 A lazy yet bulletproof machine translation tool for Elastichsearch.
 
 ```
 Usage: es-translator [OPTIONS]
```

### Comparing `es_translator-1.7.1/es_translator/cli.py` & `es_translator-1.7.2/es_translator/cli.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/es_translator/es.py` & `es_translator-1.7.2/es_translator/es.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/es_translator/es_translator.py` & `es_translator-1.7.2/es_translator/es_translator.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/es_translator/interpreters/abstract.py` & `es_translator-1.7.2/es_translator/interpreters/abstract.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/es_translator/interpreters/apertium/apertium.py` & `es_translator-1.7.2/es_translator/interpreters/apertium/apertium.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/es_translator/interpreters/apertium/pairs.py` & `es_translator-1.7.2/es_translator/interpreters/apertium/pairs.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/es_translator/interpreters/apertium/repository.py` & `es_translator-1.7.2/es_translator/interpreters/apertium/repository.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/es_translator/interpreters/argos/argos.py` & `es_translator-1.7.2/es_translator/interpreters/argos/argos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from argostranslate import package as argospackage
 from argostranslate import translate as argostranslate
-from argostranslate.utils import logger as argoslogger
 
 from ..abstract import AbstractInterpreter
 from ...logger import logger
 
 
 class ArgosPairNotAvailable(Exception):
     pass
@@ -51,18 +50,22 @@
         except AttributeError:
             return []
 
     def download_necessary_languages(self):
         argospackage.update_package_index()
         for package in argospackage.get_available_packages():
             if package.from_code == self.source_alpha_2 and package.to_code == self.target_alpha_2:
+                if package in argospackage.get_installed_packages():
+                    return
                 download_path = package.download()
+                logger.info(f'Installing Argos package {package}')
                 return argospackage.install_from_path(download_path)
         raise ArgosPairNotAvailable
 
+
     @property
     def translation(self):
         installed_languages = argostranslate.get_installed_languages()
         source = list(
             filter(
                 lambda x: x.code == self.source_alpha_2,
                 installed_languages))[0]
```

### Comparing `es_translator-1.7.1/es_translator/logger.py` & `es_translator-1.7.2/es_translator/logger.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/es_translator/tasks.py` & `es_translator-1.7.2/es_translator/tasks.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/es_translator/worker.py` & `es_translator-1.7.2/es_translator/worker.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.7.1/pyproject.toml` & `es_translator-1.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "es-translator"
-version = "1.7.1"
+version = "1.7.2"
 description = "A lazy yet bulletproof machine translation tool for Elastichsearch."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 license = "GNU AFFERO GENERAL PUBLIC LICENSE"
 packages = [{include = "es_translator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `es_translator-1.7.1/setup.py` & `es_translator-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 entry_points = \
 {'console_scripts': ['es-translator = es_translator.cli:translate',
                      'es-translator-pairs = es_translator.cli:pairs',
                      'es-translator-tasks = es_translator.cli:tasks']}
 
 setup_kwargs = {
     'name': 'es-translator',
-    'version': '1.7.1',
+    'version': '1.7.2',
     'description': 'A lazy yet bulletproof machine translation tool for Elastichsearch.',
-    'long_description': '# ES Translator [![](https://img.shields.io/github/actions/workflow/status/icij/es-translator/main.yml)](https://github.com/ICIJ/es-translator/actions)\n\n\nA lazy yet bulletproof machine translation tool for Elastichsearch.\n\n```\nUsage: es-translator [OPTIONS]\n\nOptions:\n  -u, --url TEXT                  Elastichsearch URL\n  -i, --index TEXT                Elastichsearch Index  [required]\n  -r, --interpreter TEXT          Interpreter to use to perform the\n                                  translation\n  -s, --source-language TEXT      Source language to translate from\n                                  [required]\n  -t, --target-language TEXT      Target language to translate to  [required]\n  --intermediary-language TEXT    An intermediary language to use when no\n                                  translation is available between the source\n                                  and the target. If none is provided this\n                                  will be calculated automatically.\n  --source-field TEXT             Document field to translate\n  --target-field TEXT             Document field where the translations are\n                                  stored\n  -q, --query-string TEXT         Search query string to filter result\n  -d, --data-dir PATH             Path to the directory where to language\n                                  model will be downloaded\n  --scan-scroll TEXT              Scroll duration (set to higher value if\n                                  you\'re processing a lot of documents)\n  --dry-run                       Don\'t save anything in Elasticsearch\n  --pool-size INTEGER             Number of parallel processes to start\n  --pool-timeout INTEGER          Timeout to add a translation\n  --throttle INTEGER              Throttle between each translation (in ms)\n  --syslog-address TEXT           Syslog address\n  --syslog-port INTEGER           Syslog port\n  --syslog-facility TEXT          Syslog facility\n  --stdout-loglevel TEXT          Change the default log level for stdout\n                                  error handler\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --help                          Show this message and exit.\n```\n\n## Installation (Ubuntu)\n\nInstall Apertium:\n\n```\nwget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash\nsudo apt install apertium-all-dev\n```\n\nCreate a Virtualenv and install Pip packages with Poetry:\n\n```\nmake install\n```\n\nOn Ubuntu 22.04 some additional packages might be needed if you use the version from Ubuntu\'s repository:\n\n```\nsudo apt install cg3 apertium-get apertium-lex-tools\n```\n\n\n## Installation (Docker)\n\nNothing to do as long as you have Docker on your system:\n\n```\ndocker run -it icij/es-translator poetry run es-translator --help\n```\n\n## Examples\n\nTranslates documents from French to Spanish on a local Elasticsearch. The translated field is `content` (the default).\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es\n```\n\nTranslates documents from French to English on a local Elasticsearch using Apertium:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language en --interpreter apertium\n```\n\nTo translate the `title` field we could do:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es --source-field title\n```\n\nTranslates documents from English to Spanish on a local Elasticsearch using 4 threads:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language en --target-language es --pool-size 4\n```\n\nTranslates documents from Portuguese to English, using an intermediary language (Apertium doesn\'t offer this translation pair):\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language pt --intermediary-language es --target-language en\n```\n',
+    'long_description': '# ES Translator [![](https://img.shields.io/github/actions/workflow/status/icij/es-translator/main.yml)](https://github.com/ICIJ/es-translator/actions) [![](https://img.shields.io/pypi/pyversions/es-translator)](https://pypi.org/project/es-translator/) \n\n\nA lazy yet bulletproof machine translation tool for Elastichsearch.\n\n```\nUsage: es-translator [OPTIONS]\n\nOptions:\n  -u, --url TEXT                  Elastichsearch URL\n  -i, --index TEXT                Elastichsearch Index  [required]\n  -r, --interpreter TEXT          Interpreter to use to perform the\n                                  translation\n  -s, --source-language TEXT      Source language to translate from\n                                  [required]\n  -t, --target-language TEXT      Target language to translate to  [required]\n  --intermediary-language TEXT    An intermediary language to use when no\n                                  translation is available between the source\n                                  and the target. If none is provided this\n                                  will be calculated automatically.\n  --source-field TEXT             Document field to translate\n  --target-field TEXT             Document field where the translations are\n                                  stored\n  -q, --query-string TEXT         Search query string to filter result\n  -d, --data-dir PATH             Path to the directory where to language\n                                  model will be downloaded\n  --scan-scroll TEXT              Scroll duration (set to higher value if\n                                  you\'re processing a lot of documents)\n  --dry-run                       Don\'t save anything in Elasticsearch\n  --pool-size INTEGER             Number of parallel processes to start\n  --pool-timeout INTEGER          Timeout to add a translation\n  --throttle INTEGER              Throttle between each translation (in ms)\n  --syslog-address TEXT           Syslog address\n  --syslog-port INTEGER           Syslog port\n  --syslog-facility TEXT          Syslog facility\n  --stdout-loglevel TEXT          Change the default log level for stdout\n                                  error handler\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --help                          Show this message and exit.\n```\n\n## Installation (Ubuntu)\n\nInstall Apertium:\n\n```\nwget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash\nsudo apt install apertium-all-dev\n```\n\nCreate a Virtualenv and install Pip packages with Poetry:\n\n```\nmake install\n```\n\nOn Ubuntu 22.04 some additional packages might be needed if you use the version from Ubuntu\'s repository:\n\n```\nsudo apt install cg3 apertium-get apertium-lex-tools\n```\n\n\n## Installation (Docker)\n\nNothing to do as long as you have Docker on your system:\n\n```\ndocker run -it icij/es-translator poetry run es-translator --help\n```\n\n## Examples\n\nTranslates documents from French to Spanish on a local Elasticsearch. The translated field is `content` (the default).\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es\n```\n\nTranslates documents from French to English on a local Elasticsearch using Apertium:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language en --interpreter apertium\n```\n\nTo translate the `title` field we could do:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es --source-field title\n```\n\nTranslates documents from English to Spanish on a local Elasticsearch using 4 threads:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language en --target-language es --pool-size 4\n```\n\nTranslates documents from Portuguese to English, using an intermediary language (Apertium doesn\'t offer this translation pair):\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language pt --intermediary-language es --target-language en\n```\n',
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `es_translator-1.7.1/PKG-INFO` & `es_translator-1.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: es-translator
-Version: 1.7.1
+Version: 1.7.2
 Summary: A lazy yet bulletproof machine translation tool for Elastichsearch.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8.2,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Requires-Dist: pycountry (>=22.3,<23.0)
 Requires-Dist: rich (>=12,<13)
 Requires-Dist: sh (>=1,<2)
 Requires-Dist: torch (>=1.13,<2.0)
 Requires-Dist: urllib3 (>=1.26,<2.0)
 Description-Content-Type: text/markdown
 
-# ES Translator [![](https://img.shields.io/github/actions/workflow/status/icij/es-translator/main.yml)](https://github.com/ICIJ/es-translator/actions)
+# ES Translator [![](https://img.shields.io/github/actions/workflow/status/icij/es-translator/main.yml)](https://github.com/ICIJ/es-translator/actions) [![](https://img.shields.io/pypi/pyversions/es-translator)](https://pypi.org/project/es-translator/) 
 
 
 A lazy yet bulletproof machine translation tool for Elastichsearch.
 
 ```
 Usage: es-translator [OPTIONS]
```

