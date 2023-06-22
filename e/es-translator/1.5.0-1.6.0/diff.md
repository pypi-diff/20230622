# Comparing `tmp/es_translator-1.5.0.tar.gz` & `tmp/es_translator-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "es_translator-1.5.0.tar", max compression
+gzip compressed data, was "es_translator-1.6.0.tar", max compression
```

## Comparing `es_translator-1.5.0.tar` & `es_translator-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     3978 2023-05-16 11:15:56.684853 es_translator-1.5.0/README.md
--rw-r--r--   0        0        0      136 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/__init__.py
--rw-r--r--   0        0        0      490 2022-06-20 12:45:46.183755 es_translator-1.5.0/es_translator/alpha.py
--rw-r--r--   0        0        0     4992 2023-05-16 11:12:42.123154 es_translator-1.5.0/es_translator/cli.py
--rw-r--r--   0        0        0     1893 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/es.py
--rw-r--r--   0        0        0     5882 2023-05-16 11:09:04.245390 es_translator-1.5.0/es_translator/es_translator.py
--rw-r--r--   0        0        0       55 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/__init__.py
--rw-r--r--   0        0        0     1690 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/abstract.py
--rw-r--r--   0        0        0       30 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/apertium/__init__.py
--rw-r--r--   0        0        0     6069 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/apertium/apertium.py
--rw-r--r--   0        0        0      722 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/apertium/pairs.py
--rw-r--r--   0        0        0     5390 2022-12-15 10:03:37.305408 es_translator-1.5.0/es_translator/interpreters/apertium/repository.py
--rw-r--r--   0        0        0       24 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/argos/__init__.py
--rw-r--r--   0        0        0     2553 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/argos/argos.py
--rw-r--r--   0        0        0      912 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/logger.py
--rw-r--r--   0        0        0      267 2022-06-20 12:45:46.183755 es_translator-1.5.0/es_translator/symlink.py
--rw-r--r--   0        0        0     2560 2023-05-16 11:06:33.928295 es_translator-1.5.0/es_translator/worker.py
--rw-r--r--   0        0        0      842 2023-05-16 11:19:12.026637 es_translator-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 es_translator-1.5.0/setup.py
--rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 es_translator-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     3978 2023-05-16 11:15:56.684853 es_translator-1.6.0/README.md
+-rw-r--r--   0        0        0      170 2023-06-22 08:22:54.005082 es_translator-1.6.0/es_translator/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-22 08:22:53.845080 es_translator-1.6.0/es_translator/alpha.py
+-rw-r--r--   0        0        0     7070 2023-06-22 08:22:45.512961 es_translator-1.6.0/es_translator/cli.py
+-rw-r--r--   0        0        0     2113 2023-06-22 08:22:54.121084 es_translator-1.6.0/es_translator/es.py
+-rw-r--r--   0        0        0    10240 2023-06-22 08:22:49.697021 es_translator-1.6.0/es_translator/es_translator.py
+-rw-r--r--   0        0        0       56 2023-06-22 08:22:58.069140 es_translator-1.6.0/es_translator/interpreters/__init__.py
+-rw-r--r--   0        0        0     1721 2023-06-22 08:22:58.057140 es_translator-1.6.0/es_translator/interpreters/abstract.py
+-rw-r--r--   0        0        0       31 2023-06-22 08:23:26.117539 es_translator-1.6.0/es_translator/interpreters/apertium/__init__.py
+-rw-r--r--   0        0        0     6257 2023-06-22 08:23:26.413543 es_translator-1.6.0/es_translator/interpreters/apertium/apertium.py
+-rw-r--r--   0        0        0      721 2023-06-22 08:23:26.009537 es_translator-1.6.0/es_translator/interpreters/apertium/pairs.py
+-rw-r--r--   0        0        0     5437 2023-06-22 08:23:26.185540 es_translator-1.6.0/es_translator/interpreters/apertium/repository.py
+-rw-r--r--   0        0        0       25 2023-06-22 08:23:26.129539 es_translator-1.6.0/es_translator/interpreters/argos/__init__.py
+-rw-r--r--   0        0        0     2697 2023-06-22 08:23:26.105538 es_translator-1.6.0/es_translator/interpreters/argos/argos.py
+-rw-r--r--   0        0        0      943 2023-06-22 08:22:53.761079 es_translator-1.6.0/es_translator/logger.py
+-rw-r--r--   0        0        0      264 2023-06-22 08:22:54.025082 es_translator-1.6.0/es_translator/symlink.py
+-rw-r--r--   0        0        0      939 2023-06-22 08:22:53.989082 es_translator-1.6.0/es_translator/tasks.py
+-rw-r--r--   0        0        0     1810 2023-06-22 08:22:53.873080 es_translator-1.6.0/es_translator/worker.py
+-rw-r--r--   0        0        0     1086 2023-06-22 08:25:56.043672 es_translator-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 es_translator-1.6.0/setup.py
+-rw-r--r--   0        0        0     4926 1970-01-01 00:00:00.000000 es_translator-1.6.0/PKG-INFO
```

### Comparing `es_translator-1.5.0/LICENSE.txt` & `es_translator-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `es_translator-1.5.0/README.md` & `es_translator-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `es_translator-1.5.0/es_translator/es.py` & `es_translator-1.6.0/es_translator/es.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 class TranslatedHit():
-    def __init__(self, hit, source_field = 'content', target_field = 'content_translated'):
+    def __init__(self, hit, source_field='content',
+                 target_field='content_translated'):
         self.hit = hit
         self.source_field = source_field
         self.target_field = target_field
         # Ensure the target field is an array
         self.hit[self.target_field] = self.translations
 
     @property
@@ -34,20 +35,31 @@
     @property
     def body(self):
         body = dict(doc=dict())
         body['doc'][self.target_field] = self.translations
         return body
 
     def save(self, client):
-        client.update(index = self.index, doc_type = self.doc_type, id = self.id, routing = self.routing, body = self.body)
+        client.update(
+            index=self.index,
+            doc_type=self.doc_type,
+            id=self.id,
+            routing=self.routing,
+            body=self.body)
 
     def add_translation(self, interpreter):
-        if not self.is_translated(interpreter.source_name, interpreter.target_name):
+        if not self.is_translated(
+                interpreter.source_name,
+                interpreter.target_name,
+                interpreter.name):
             self.hit[self.target_field].append(dict(
-                translator = interpreter.name,
-                source_language = interpreter.source_name.upper(),
-                target_language = interpreter.target_name.upper(),
-                content = interpreter.translate(self.source_value)))
-
-    def is_translated(self, source_language, target_language):
-        same_languages = lambda t: t['source_language'] == source_language.upper() and t['target_language'] == target_language.upper()
+                translator=interpreter.name,
+                source_language=interpreter.source_name.upper(),
+                target_language=interpreter.target_name.upper(),
+                content=interpreter.translate(self.source_value)))
+
+    def is_translated(self, source_language, target_language, translator):
+        def same_languages(t):
+            return t['source_language'] == source_language.upper() and \
+                t['target_language'] == target_language.upper() and \
+                t['translator'] == translator
         return any(t for t in self.translations if same_languages(t))
```

### Comparing `es_translator-1.5.0/es_translator/interpreters/abstract.py` & `es_translator-1.6.0/es_translator/interpreters/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from abc import ABC, abstractmethod
 from os.path import abspath
 
 from ..alpha import to_alpha_2, to_alpha_3, to_name
 
+
 class AbstractInterpreter(ABC):
     name = 'ABSTRACT'
-    
-    def __init__(self, source = None, target = None, intermediary = None, pack_dir = None):
+
+    def __init__(
+            self,
+            source=None,
+            target=None,
+            intermediary=None,
+            pack_dir=None):
         self.source = source
         self.target = target
         self.intermediary = intermediary
         # Create a temporary pack dir (if needed) to download language packs
         if pack_dir is not None:
-            self.pack_dir = abspath(pack_dir) 
-  
+            self.pack_dir = abspath(pack_dir)
+
     @property
     def name(self):
         return self.__class__.name
-    
+
     @property
     def source_alpha_2(self):
         return to_alpha_2(self.source)
 
     @property
     def source_alpha_3(self):
         return to_alpha_3(self.source)
@@ -53,15 +59,15 @@
     @property
     def pair_alpha_3(self):
         return '%s-%s' % (self.source_alpha_3, self.target_alpha_3)
 
     @property
     def pair_inverse(self):
         return '%s-%s' % (self.target, self.source)
-      
+
     @property
     def has_pair(self):
         return self.source is not None and self.target is not None
-      
+
     @abstractmethod
     def translate(self, input):
         return input
```

### Comparing `es_translator-1.5.0/es_translator/interpreters/apertium/apertium.py` & `es_translator-1.6.0/es_translator/interpreters/apertium/apertium.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,24 @@
 from sh import apertium, ErrorReturnCode
 # Module from the same package
 from .repository import ApertiumRepository
 from ..abstract import AbstractInterpreter
 from ...alpha import to_alpha_3_pair
 from ...logger import logger
 
+
 class Apertium(AbstractInterpreter):
     name = 'APERTIUM'
-    
-    def __init__(self, source = None, target = None, intermediary = None, pack_dir = None):
+
+    def __init__(
+            self,
+            source=None,
+            target=None,
+            intermediary=None,
+            pack_dir=None):
         super().__init__(source, target, intermediary, pack_dir)
         # A class to download necessary pair package
         self.repository = ApertiumRepository(self.pack_dir)
         # Raise an exception if the language pair is unkown
         if not self.is_pair_available and self.has_pair:
             try:
                 self.download_necessary_pairs()
@@ -30,15 +36,17 @@
     @property
     def is_pair_available(self):
         return not self.intermediary and self.pair in self.local_pairs
 
     @property
     def pairs_pipeline(self):
         if self.intermediary:
-            return [self.intermediary_source_pair, self.intermediary_target_pair]
+            return [
+                self.intermediary_source_pair,
+                self.intermediary_target_pair]
         else:
             return [self.pair_alpha_3]
 
     @property
     def intermediary_source_pair(self):
         return '%s-%s' % (self.source_alpha_3, self.intermediary_alpha_3)
 
@@ -54,41 +62,43 @@
     def intermediary_target_pair_package(self):
         return self.pair_to_pair_package(self.intermediary_target_pair)
 
     @property
     def intermediary_pairs(self):
         # Find the intermediary lang only if not given
         if self.intermediary is None:
-            trunk_packages = [ s.split('-') for s in self.remote_pairs ]
+            trunk_packages = [s.split('-') for s in self.remote_pairs]
             # Build a tree of languages and their children
             packages_tree = self.lang_tree(self.source, trunk_packages)
-            # Find the first path between self.source (the root) and self.target in the given tree
-            self.intermediary = self.first_pairs_path(packages_tree, self.target)[0]
+            # Find the first path between self.source (the root) and
+            # self.target in the given tree
+            self.intermediary = self.first_pairs_path(
+                packages_tree, self.target)[0]
         # We build the two intermediary pairs
-        return [ self.intermediary_source_pair, self.intermediary_target_pair ]
+        return [self.intermediary_source_pair, self.intermediary_target_pair]
 
     @property
     def local_pairs(self):
         output = apertium('-d', self.pack_dir, '-l').strip()
-        return [ s.strip() for s in output.split('\n') ]
+        return [s.strip() for s in output.split('\n')]
 
     @property
     @lru_cache()
-    def remote_pairs(self, module = 'trunk'):
+    def remote_pairs(self, module='trunk'):
         packages = self.repository.pair_packages
         pairs = []
-        package_name_to_pair = lambda n: '-'.join(n.split('-')[-2:])
+        def package_name_to_pair(n): return '-'.join(n.split('-')[-2:])
         # Extract package within these two properties
         for attr in ['Package', 'Provides']:
             for package in packages:
                 for value in package.get(attr, '').split(','):
                     pair = package_name_to_pair(value.strip())
                     pairs.append(pair)
         # Remove empty values
-        return [ p for p in pairs if p != '']
+        return [p for p in pairs if p != '']
 
     def pair_to_pair_package(self, pair):
         pair_inversed = '-'.join(pair.split('-')[::-1])
         combinations = [to_alpha_3_pair(pair), to_alpha_3_pair(pair_inversed)]
         try:
             return next(p for p in self.remote_pairs if p in combinations)
         except StopIteration:
@@ -97,15 +107,15 @@
     def download_necessary_pairs(self):
         logger.info('Downloading necessary package(s) for %s' % self.pair)
         if self.any_pair_variant_in_packages:
             self.download_pair()
         else:
             self.download_intermediary_pairs()
 
-    def download_pair(self, pair = None):
+    def download_pair(self, pair=None):
         if pair is None:
             pair = self.pair_alpha_3
         else:
             pair = to_alpha_3_pair(pair)
         # All commands must be run from the pack dir
         return self.repository.install_pair_package(pair)
 
@@ -113,44 +123,49 @@
     def any_pair_variant_in_packages(self):
         return self.pair_alpha_3 in self.remote_pairs
 
     def download_intermediary_pairs(self):
         for pair in self.intermediary_pairs:
             self.download_pair(pair)
 
-    def lang_tree(self, lang, pairs, depth = 2):
-        tree = dict(lang = lang, children = dict())
+    def lang_tree(self, lang, pairs, depth=2):
+        tree = dict(lang=lang, children=dict())
         for pair in pairs:
             if lang in pair and depth > 0:
                 child_lang = next(l for l in pair if l != lang)
-                tree["children"][child_lang] = self.lang_tree(child_lang, pairs, depth - 1)
+                tree["children"][child_lang] = self.lang_tree(
+                    child_lang, pairs, depth - 1)
         return tree
 
     def first_pairs_path(self, leaf, lang):
         path = []
         for child_leaf in leaf['children'].values():
             if self.leaf_has_lang(child_leaf, lang):
                 path.append(child_leaf['lang'])
                 path = path + self.first_pairs_path(child_leaf, lang)
                 break
         return path
 
     def leaf_has_lang(self, leaf, lang):
         children = leaf['children'].values()
-        return lang in leaf['children'] or any(self.leaf_has_lang(child_leaf, lang) for child_leaf in children)
+        return lang in leaf['children'] or any(
+            self.leaf_has_lang(
+                child_leaf,
+                lang) for child_leaf in children)
 
     def translate(self, input):
         for pair in self.pairs_pipeline:
             # Create a sub-process witch can receive a input
             input = self.translate_with_apertium(input, pair)
         return input
 
     def translate_with_apertium(self, input, pair):
         try:
             # Works with a temporary file as buffer (opened in text mode)
             with NamedTemporaryFile(mode='w+t') as temp_input_file:
                 temp_input_file.writelines(input)
                 temp_input_file.seek(0)
-                input_translated = apertium('-ud', self.pack_dir, pair, temp_input_file.name)
+                input_translated = apertium(
+                    '-ud', self.pack_dir, pair, temp_input_file.name)
         except ErrorReturnCode as e:
             raise Exception('Unable to translate this string.')
         return str(input_translated)
```

### Comparing `es_translator-1.5.0/es_translator/interpreters/apertium/pairs.py` & `es_translator-1.6.0/es_translator/interpreters/apertium/pairs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Module from the same package
 from .apertium import Apertium
 
+
 class Pairs:
-    def __init__(self, data_dir, local = False):
+    def __init__(self, data_dir, local=False):
         self.apertium = Apertium(pack_dir=data_dir)
         self.local = local
 
     @property
     def local_pairs(self):
         return self.apertium.local_pairs
```

### Comparing `es_translator-1.5.0/es_translator/interpreters/apertium/repository.py` & `es_translator-1.6.0/es_translator/interpreters/apertium/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,66 +9,69 @@
 from es_translator.alpha import to_alpha_2, to_alpha_3, to_alpha_3_pair
 from es_translator.logger import logger
 from es_translator.symlink import create_symlink
 
 REPOSITORY_URL = "https://apertium.projectjj.com/apt/nightly"
 PACKAGES_FILE_URL = "%s/dists/focal/main/binary-amd64/Packages" % REPOSITORY_URL
 
+
 class ApertiumRepository:
-    def __init__(self, cache_dir = None):
+    def __init__(self, cache_dir=None):
         # Create a temporary pack dir (if needed)
         self.cache_dir = abspath(cache_dir)
 
     @property
     @lru_cache()
     def control_file_content(self):
         response = request.urlopen(PACKAGES_FILE_URL)
         data = response.read()
         return data.decode('utf-8')
 
     @property
     @lru_cache()
     def packages(self):
-        isnt_empty = lambda c: c is not None and c != ''
+        def isnt_empty(c): return c is not None and c != ''
         control_strings = self.control_file_content.split('\n\n')
         control_strings = list(filter(isnt_empty, control_strings))
         return list(map(parse_deb822, control_strings))
 
     @property
     @lru_cache()
     def pair_packages(self):
         return list(filter(self.is_apertium_pair, self.packages))
 
     def find_package(self, package):
-        is_package = lambda c: c.get('Package') == package or c.get('Provides') == package
+        def is_package(c): return c.get(
+            'Package') == package or c.get('Provides') == package
         try:
             return next(filter(is_package, self.packages))
         except StopIteration:
             logger.warning('Unable to found package %s' % package)
             return None
 
     def find_pair_package(self, pair):
         pair = to_alpha_3_pair(pair)
         pair_inversed = '-'.join(pair.split('-')[::-1])
+
         def is_pair(c):
-            return c.get('Package',  '').endswith(pair) \
-                or c.get('Package',  '').endswith(pair_inversed)
+            return c.get('Package', '').endswith(pair) \
+                or c.get('Package', '').endswith(pair_inversed)
         try:
             return next(filter(is_pair, self.pair_packages))
         except StopIteration:
             return None
 
     def is_apertium_pair(self, control):
         try:
             parts = control['Package'].split('-')
             return len(parts) == 3 and parts[0] == 'apertium'
         except KeyError:
             return False
 
-    def download_package(self, name, force = False):
+    def download_package(self, name, force=False):
         package = self.find_package(name)
         package_url = REPOSITORY_URL + '/' + package['Filename']
         package_dir = join(self.cache_dir, name)
         package_file = join(package_dir, 'package') + '.deb'
         mkdir('-p', package_dir)
         # Don't download the file twice
         if force or not isfile(package_file):
@@ -84,15 +87,15 @@
             raise Exception('No pair package  available for "%s"' % pair)
 
     def replace_in_file(self, file, target, replacement):
         with FileInput(file, inplace=True) as fileinput:
             for line in fileinput:
                 print(line.replace(target, replacement), end='')
 
-    def extract_pair_package(self, file, extraction_dir = '.'):
+    def extract_pair_package(self, file, extraction_dir='.'):
         workdir = dirname(file)
         with pushd(workdir):
             # Extract the file from the .deb
             dpkg_deb('-x', file, extraction_dir)
             # Copy the files we need
             cp('-rlf', glob('usr/share/apertium/*'), extraction_dir)
             # Remove everything else
@@ -100,38 +103,41 @@
             # Rewrite paths in modes files
             for mode in glob('modes/*.mode'):
                 self.replace_in_file(mode, '/usr/share/apertium', workdir)
         return workdir
 
     def create_pair_package_alias(self, package_dir):
         extraction_dir = dirname(package_dir) + '/'
-        [source, target] = basename(package_dir).split('apertium-')[-1].split('-')
+        [source, target] = basename(package_dir).split(
+            'apertium-')[-1].split('-')
         if len(source) == 2:
             aliases = (to_alpha_3(source), to_alpha_3(target))
         else:
             aliases = (to_alpha_2(source), to_alpha_2(target))
         # Build the alias dir using the alias
         alias_dir = join(extraction_dir, 'apertium-%s-%s' % aliases)
-        mode_file = join(extraction_dir, 'modes', '%s-%s.mode' % (source, target))
+        mode_file = join(
+            extraction_dir, 'modes', '%s-%s.mode' %
+            (source, target))
         mode_alias_file = join(extraction_dir, 'modes', '%s-%s.mode' % aliases)
         # Use a symbolic links
         create_symlink(package_dir, alias_dir)
         create_symlink(mode_file, mode_alias_file)
         return alias_dir
 
     def install_pair_package(self, pair):
         logger.info('Installing pair package %s' % pair)
         package_file = self.download_pair_package(pair)
         package_dir = self.extract_pair_package(package_file)
         alias_dir = self.create_pair_package_alias(package_dir)
-        self.import_modes(clear = False)
+        self.import_modes(clear=False)
         return package_dir
 
     def clear_modes(self):
         with pushd(self.cache_dir):
             rm('-Rf', 'modes')
 
-    def import_modes(self, clear = True):
+    def import_modes(self, clear=True):
         with pushd(self.cache_dir):
             mkdir('-p', 'modes')
             # Copy all the mode files
             cp(glob('./*/modes/*.mode'), './modes')
```

### Comparing `es_translator-1.5.0/es_translator/interpreters/argos/argos.py` & `es_translator-1.6.0/es_translator/interpreters/argos/argos.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,76 @@
 from argostranslate import package as argospackage
 from argostranslate import translate as argostranslate
 from argostranslate.utils import logger as argoslogger
 
 from ..abstract import AbstractInterpreter
 from ...logger import logger
 
-class ArgosPairNotAvailable(Exception): pass
+
+class ArgosPairNotAvailable(Exception):
+    pass
+
 
 class Argos(AbstractInterpreter):
     name = 'ARGOS'
-        
-    def __init__(self, source = None, target = None, intermediary = None, pack_dir = None):
+
+    def __init__(
+            self,
+            source=None,
+            target=None,
+            intermediary=None,
+            pack_dir=None):
         super().__init__(source, target)
         # Raise an exception if an intermediary language is provded
         if intermediary is not None:
-            logger.warn('Argos interpreter doesnt support intermediary language')
+            logger.warn(
+                'Argos interpreter doesnt support intermediary language')
         if pack_dir is not None:
-            logger.warn('Argos interpreter doesnt support custom pack directory')
+            logger.warn(
+                'Argos interpreter doesnt support custom pack directory')
         # Raise an exception if the language pair is unkown
         if not self.is_pair_available and self.has_pair:
             try:
                 self.download_necessary_languages()
             except ArgosPairNotAvailable:
                 raise Exception('The pair %s is not available' % self.pair)
         else:
             logger.info('Existing package(s) found for pair %s' % self.pair)
-    
-    @property    
+
+    @property
     def is_pair_available(self):
         for package in argospackage.get_installed_packages():
             if package.from_code == self.source_alpha_2 and package.to_code == self.target_alpha_2:
                 return True
         return False
-    
+
     @property
-    def local_languages(self):        
+    def local_languages(self):
         try:
             installed_languages = argostranslate.get_installed_languages()
-            return [ lang.code for lang in installed_languages ]
+            return [lang.code for lang in installed_languages]
         except AttributeError:
             return []
-    
+
     def download_necessary_languages(self):
         argospackage.update_package_index()
         for package in argospackage.get_available_packages():
             if package.from_code == self.source_alpha_2 and package.to_code == self.target_alpha_2:
                 download_path = package.download()
                 return argospackage.install_from_path(download_path)
         raise ArgosPairNotAvailable
-    
+
     @property
     def translation(self):
         installed_languages = argostranslate.get_installed_languages()
-        source = list(filter(lambda x: x.code == self.source_alpha_2, installed_languages))[0]
-        target = list(filter(lambda x: x.code == self.target_alpha_2, installed_languages))[0]
+        source = list(
+            filter(
+                lambda x: x.code == self.source_alpha_2,
+                installed_languages))[0]
+        target = list(
+            filter(
+                lambda x: x.code == self.target_alpha_2,
+                installed_languages))[0]
         return source.get_translation(target)
-    
+
     def translate(self, input):
-        return self.translation.translate(input)
+        return self.translation.translate(input)
```

### Comparing `es_translator-1.5.0/es_translator/logger.py` & `es_translator-1.6.0/es_translator/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 
 import coloredlogs
 from logging.handlers import SysLogHandler
 
 logger = logging.getLogger('es-translator')
 logger.setLevel(logging.INFO)
 
+
 def default_log_formatter() -> logging.Formatter:
-    return logging.Formatter('%(asctime)s :: %(name)s :: %(levelname)s :: %(message)s')
+    return logging.Formatter(
+        '%(asctime)s :: %(name)s :: %(levelname)s :: %(message)s')
 
 
-def add_syslog_handler(address: str = 'localhost', port: int = 514, facility: int = LOG_LOCAL7) -> None:
+def add_syslog_handler(
+        address: str = 'localhost',
+        port: int = 514,
+        facility: int = LOG_LOCAL7) -> None:
     sysLogFormatter = default_log_formatter()
-    sysLogHandler = SysLogHandler(address = (address, port), facility = facility)
+    sysLogHandler = SysLogHandler(address=(address, port), facility=facility)
     sysLogHandler.setLevel(logging.INFO)
     sysLogHandler.setFormatter(sysLogFormatter)
     logger.addHandler(sysLogHandler)
 
 
 def add_stdout_handler(level: int = logging.ERROR) -> None:
     fmt = '%(levelname)s %(message)s'
```

### Comparing `es_translator-1.5.0/es_translator/worker.py` & `es_translator-1.6.0/es_translator/worker.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
 from time import sleep
-from elasticsearch import Elasticsearch, ElasticsearchException
+from elasticsearch import ElasticsearchException
 from queue import Full
 # Module from the same package
 from es_translator.logger import logger
-from es_translator.es import TranslatedHit
 
-class FatalTranslationException(Exception): pass
+
+class FatalTranslationException(Exception):
+    pass
+
 
 def translation_worker(queue, shared_fatal_error):
     """
     Worker function that translates documents from the queue in parallel.
 
     Args:
         queue: JoinableQueue for retrieving documents to be translated.
@@ -18,48 +20,37 @@
 
     Notes:
         This function continuously retrieves documents from the queue and translates them until a fatal error occurs
         or the queue is empty. It handles different types of exceptions and updates the shared_fatal_error if needed.
     """
     while not shared_fatal_error.value:
         try:
-            es_translator, hit, index = queue.get(True)
-            translate_document(es_translator, hit, index)
+            es_translator, hit = queue.get(True)
+            es_translator.translate_document(hit)
             sleep(es_translator.throttle / 1000)
         except ElasticsearchException as error:
-            handle_elasticsearch_exception(error, index, hit)
+            handle_elasticsearch_exception(error, hit)
             shared_fatal_error.value = error
         except Full:
             handle_timeout_reached(es_translator.pool_timeout)
         except Exception as error:
-            handle_exception(error, index, hit)
+            handle_exception(error, hit)
         finally:
             queue.task_done()
     queue.close()
 
 
-def translate_document(es_translator, hit, index):
-    # Translate the document
-    logger.info('Translating doc %s (%s)' % (index, hit.meta.id))
-    translated_hit = TranslatedHit(hit, es_translator.source_field, es_translator.target_field)
-    translated_hit.add_translation(es_translator.interpreter)
-    logger.info('Translated doc %s (%s)' % (index, hit.meta.id))
-    
-    # Save the translated document if not in dry run mode
-    if not es_translator.dry_run:
-        client = Elasticsearch(es_translator.url)
-        translated_hit.save(client)
-        logger.info('Saved translation for doc %s (%s)' % (index, hit.meta.id))
-
-def handle_elasticsearch_exception(error, index, hit):
+def handle_elasticsearch_exception(error, index):
     # Handle Elasticsearch exception
-    logger.error('An error occurred when saving doc %s (%s)' % (index, hit.meta.id))
+    logger.error('An error occurred when saving doc %s' % index.meta.id)
     logger.error(error)
 
+
 def handle_timeout_reached(pool_timeout):
     # Handle timeout reached
     logger.warning('Timeout reached (%ss).' % pool_timeout)
 
-def handle_exception(error, index, hit):
+
+def handle_exception(error, hit):
     # Handle other exceptions
-    logger.warning('Unable to translate doc %s (%s)' % (index, hit.meta.id))
+    logger.warning('Unable to translate doc %s' % hit.meta.id)
     logger.warning(error)
```

### Comparing `es_translator-1.5.0/pyproject.toml` & `es_translator-1.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 [tool.poetry]
 name = "es-translator"
-version = "1.5.0"
+version = "1.6.0"
 description = "A lazy yet bulletproof machine translation tool for Elastichsearch."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 license = "GNU AFFERO GENERAL PUBLIC LICENSE"
 packages = [{include = "es_translator"}]
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.11"
+python = "^3.8.2,<3.11"
 click = "^8"
 elasticsearch = ">=7.10,<7.11"
 elasticsearch-dsl = ">=7.4.0,<8.0.0"
 sh = "^1"
 pycountry = "^22.3"
 deb-pkg-tools = "^8.4"
 coloredlogs = "*"
 urllib3 = "^1.26"
 argostranslate = "^1.7"
 rich = "^12"
 torch = "^1.13"
+celery = {extras = ["redis"], version = "^5.3.1"}
 
 [tool.poetry.group.dev.dependencies]
 pyyaml = "*"
 argh = "*"
 pytest = "^7.2"
 
+[tool.pytest.ini_options]
+filterwarnings = [
+    "error",
+    "ignore::UserWarning",
+    'ignore:pkg_resources is deprecated as an API',
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
+    
 [tool.poetry.scripts]
 es-translator = "es_translator.cli:translate"
+es-translator-tasks = "es_translator.cli:tasks"
 es-translator-pairs = "es_translator.cli:pairs"
```

### Comparing `es_translator-1.5.0/setup.py` & `es_translator-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,41 +8,43 @@
  'es_translator.interpreters.argos']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['argostranslate>=1.7,<2.0',
+ 'celery[redis]>=5.3.1,<6.0.0',
  'click>=8,<9',
  'coloredlogs',
  'deb-pkg-tools>=8.4,<9.0',
  'elasticsearch-dsl>=7.4.0,<8.0.0',
  'elasticsearch>=7.10,<7.11',
  'pycountry>=22.3,<23.0',
  'rich>=12,<13',
  'sh>=1,<2',
  'torch>=1.13,<2.0',
  'urllib3>=1.26,<2.0']
 
 entry_points = \
 {'console_scripts': ['es-translator = es_translator.cli:translate',
-                     'es-translator-pairs = es_translator.cli:pairs']}
+                     'es-translator-pairs = es_translator.cli:pairs',
+                     'es-translator-tasks = es_translator.cli:tasks']}
 
 setup_kwargs = {
     'name': 'es-translator',
-    'version': '1.5.0',
+    'version': '1.6.0',
     'description': 'A lazy yet bulletproof machine translation tool for Elastichsearch.',
     'long_description': '# ES Translator\n\n[![CircleCI](https://circleci.com/gh/ICIJ/es-translator.svg?style=svg)](https://circleci.com/gh/ICIJ/es-translator)\n\nA lazy yet bulletproof machine translation tool for Elastichsearch.\n\n```\nUsage: es-translator [OPTIONS]\n\nOptions:\n  -u, --url TEXT                  Elastichsearch URL\n  -i, --index TEXT                Elastichsearch Index  [required]\n  -r, --interpreter TEXT          Interpreter to use to perform the\n                                  translation\n  -s, --source-language TEXT      Source language to translate from\n                                  [required]\n  -t, --target-language TEXT      Target language to translate to  [required]\n  --intermediary-language TEXT    An intermediary language to use when no\n                                  translation is available between the source\n                                  and the target. If none is provided this\n                                  will be calculated automatically.\n  --source-field TEXT             Document field to translate\n  --target-field TEXT             Document field where the translations are\n                                  stored\n  -q, --query-string TEXT         Search query string to filter result\n  -d, --data-dir PATH             Path to the directory where to language\n                                  model will be downloaded\n  --scan-scroll TEXT              Scroll duration (set to higher value if\n                                  you\'re processing a lot of documents)\n  --dry-run                       Don\'t save anything in Elasticsearch\n  --pool-size INTEGER             Number of parallel processes to start\n  --pool-timeout INTEGER          Timeout to add a translation\n  --throttle INTEGER              Throttle between each translation (in ms)\n  --syslog-address TEXT           Syslog address\n  --syslog-port INTEGER           Syslog port\n  --syslog-facility TEXT          Syslog facility\n  --stdout-loglevel TEXT          Change the default log level for stdout\n                                  error handler\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --help                          Show this message and exit.\n```\n\n## Installation (Ubuntu)\n\nInstall Apertium:\n\n```\nwget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash\nsudo apt install apertium-all-dev\n```\n\nCreate a Virtualenv and install Pip packages with Poetry:\n\n```\nmake install\n```\n\nOn Ubuntu 22.04 some additional packages might be needed if you use the version from Ubuntu\'s repository:\n\n```\nsudo apt install cg3 apertium-get apertium-lex-tools\n```\n\n\n## Installation (Docker)\n\nNothing to do as long as you have Docker on your system:\n\n```\ndocker run -it icij/es-translator poetry run es-translator --help\n```\n\n## Examples\n\nTranslates documents from French to Spanish on a local Elasticsearch. The translated field is `content` (the default).\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es\n```\n\nTranslates documents from French to English on a local Elasticsearch using Apertium:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language en --interpreter apertium\n```\n\nTo translate the `title` field we could do:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es --source-field title\n```\n\nTranslates documents from English to Spanish on a local Elasticsearch using 4 threads:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language en --target-language es --pool-size 4\n```\n\nTranslates documents from Portuguese to English, using an intermediary language (Apertium doesn\'t offer this translation pair):\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language pt --intermediary-language es --target-language en\n```\n',
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8.2,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `es_translator-1.5.0/PKG-INFO` & `es_translator-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: es-translator
-Version: 1.5.0
+Version: 1.6.0
 Summary: A lazy yet bulletproof machine translation tool for Elastichsearch.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Author: ICIJ
 Author-email: engineering@icij.org
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8.2,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: argostranslate (>=1.7,<2.0)
+Requires-Dist: celery[redis] (>=5.3.1,<6.0.0)
 Requires-Dist: click (>=8,<9)
 Requires-Dist: coloredlogs
 Requires-Dist: deb-pkg-tools (>=8.4,<9.0)
 Requires-Dist: elasticsearch (>=7.10,<7.11)
 Requires-Dist: elasticsearch-dsl (>=7.4.0,<8.0.0)
 Requires-Dist: pycountry (>=22.3,<23.0)
 Requires-Dist: rich (>=12,<13)
```

