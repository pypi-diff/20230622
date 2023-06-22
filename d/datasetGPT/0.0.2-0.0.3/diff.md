# Comparing `tmp/datasetGPT-0.0.2.tar.gz` & `tmp/datasetGPT-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasetGPT-0.0.2.tar", last modified: Wed Mar 29 04:42:22 2023, max compression
+gzip compressed data, was "datasetGPT-0.0.3.tar", last modified: Thu Jun 22 18:19:14 2023, max compression
```

## Comparing `datasetGPT-0.0.2.tar` & `datasetGPT-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 radicho    (501) staff       (20)        0 2023-03-29 04:42:22.125645 datasetGPT-0.0.2/
--rw-r--r--   0 radicho    (501) staff       (20)    11873 2023-03-29 04:42:22.125370 datasetGPT-0.0.2/PKG-INFO
--rw-r--r--   0 radicho    (501) staff       (20)    11563 2023-03-18 21:20:41.000000 datasetGPT-0.0.2/README.md
--rw-r--r--   0 radicho    (501) staff       (20)       86 2023-03-18 20:59:43.000000 datasetGPT-0.0.2/pyproject.toml
--rw-r--r--   0 radicho    (501) staff       (20)       38 2023-03-29 04:42:22.125687 datasetGPT-0.0.2/setup.cfg
--rw-r--r--   0 radicho    (501) staff       (20)      918 2023-03-29 04:41:53.000000 datasetGPT-0.0.2/setup.py
-drwxr-xr-x   0 radicho    (501) staff       (20)        0 2023-03-29 04:42:22.121880 datasetGPT-0.0.2/src/
-drwxr-xr-x   0 radicho    (501) staff       (20)        0 2023-03-29 04:42:22.124097 datasetGPT-0.0.2/src/datasetGPT/
--rw-r--r--   0 radicho    (501) staff       (20)      101 2023-03-18 14:20:10.000000 datasetGPT-0.0.2/src/datasetGPT/__init__.py
--rw-r--r--   0 radicho    (501) staff       (20)       30 2023-03-13 20:04:21.000000 datasetGPT-0.0.2/src/datasetGPT/__main__.py
--rw-r--r--   0 radicho    (501) staff       (20)     2222 2023-03-22 17:56:33.000000 datasetGPT-0.0.2/src/datasetGPT/base.py
--rw-r--r--   0 radicho    (501) staff       (20)     7123 2023-03-27 18:29:52.000000 datasetGPT-0.0.2/src/datasetGPT/cli.py
--rw-r--r--   0 radicho    (501) staff       (20)     5808 2023-03-29 04:42:05.000000 datasetGPT-0.0.2/src/datasetGPT/conversations.py
--rw-r--r--   0 radicho    (501) staff       (20)     2173 2023-03-17 16:27:25.000000 datasetGPT-0.0.2/src/datasetGPT/outputs.py
--rw-r--r--   0 radicho    (501) staff       (20)     3902 2023-03-22 17:55:50.000000 datasetGPT-0.0.2/src/datasetGPT/texts.py
-drwxr-xr-x   0 radicho    (501) staff       (20)        0 2023-03-29 04:42:22.125178 datasetGPT-0.0.2/src/datasetGPT.egg-info/
--rw-r--r--   0 radicho    (501) staff       (20)    11873 2023-03-29 04:42:22.000000 datasetGPT-0.0.2/src/datasetGPT.egg-info/PKG-INFO
--rw-r--r--   0 radicho    (501) staff       (20)      444 2023-03-29 04:42:22.000000 datasetGPT-0.0.2/src/datasetGPT.egg-info/SOURCES.txt
--rw-r--r--   0 radicho    (501) staff       (20)        1 2023-03-29 04:42:22.000000 datasetGPT-0.0.2/src/datasetGPT.egg-info/dependency_links.txt
--rw-r--r--   0 radicho    (501) staff       (20)       53 2023-03-29 04:42:22.000000 datasetGPT-0.0.2/src/datasetGPT.egg-info/entry_points.txt
--rw-r--r--   0 radicho    (501) staff       (20)       30 2023-03-29 04:42:22.000000 datasetGPT-0.0.2/src/datasetGPT.egg-info/requires.txt
--rw-r--r--   0 radicho    (501) staff       (20)       11 2023-03-29 04:42:22.000000 datasetGPT-0.0.2/src/datasetGPT.egg-info/top_level.txt
+drwxr-xr-x   0 radicho    (501) staff       (20)        0 2023-06-22 18:19:14.119086 datasetGPT-0.0.3/
+-rw-r--r--   0 radicho    (501) staff       (20)    11873 2023-06-22 18:19:14.118868 datasetGPT-0.0.3/PKG-INFO
+-rw-r--r--   0 radicho    (501) staff       (20)    11563 2023-03-18 21:20:41.000000 datasetGPT-0.0.3/README.md
+-rw-r--r--   0 radicho    (501) staff       (20)       86 2023-03-18 20:59:43.000000 datasetGPT-0.0.3/pyproject.toml
+-rw-r--r--   0 radicho    (501) staff       (20)       38 2023-06-22 18:19:14.119122 datasetGPT-0.0.3/setup.cfg
+-rw-r--r--   0 radicho    (501) staff       (20)      918 2023-06-22 18:19:00.000000 datasetGPT-0.0.3/setup.py
+drwxr-xr-x   0 radicho    (501) staff       (20)        0 2023-06-22 18:19:14.115299 datasetGPT-0.0.3/src/
+drwxr-xr-x   0 radicho    (501) staff       (20)        0 2023-06-22 18:19:14.117687 datasetGPT-0.0.3/src/datasetGPT/
+-rw-r--r--   0 radicho    (501) staff       (20)      101 2023-03-18 14:20:10.000000 datasetGPT-0.0.3/src/datasetGPT/__init__.py
+-rw-r--r--   0 radicho    (501) staff       (20)       30 2023-03-13 20:04:21.000000 datasetGPT-0.0.3/src/datasetGPT/__main__.py
+-rw-r--r--   0 radicho    (501) staff       (20)     2222 2023-03-22 17:56:33.000000 datasetGPT-0.0.3/src/datasetGPT/base.py
+-rw-r--r--   0 radicho    (501) staff       (20)     7123 2023-06-22 18:01:51.000000 datasetGPT-0.0.3/src/datasetGPT/cli.py
+-rw-r--r--   0 radicho    (501) staff       (20)     5900 2023-06-22 18:16:37.000000 datasetGPT-0.0.3/src/datasetGPT/conversations.py
+-rw-r--r--   0 radicho    (501) staff       (20)     2173 2023-03-17 16:27:25.000000 datasetGPT-0.0.3/src/datasetGPT/outputs.py
+-rw-r--r--   0 radicho    (501) staff       (20)     3904 2023-06-22 18:01:51.000000 datasetGPT-0.0.3/src/datasetGPT/texts.py
+drwxr-xr-x   0 radicho    (501) staff       (20)        0 2023-06-22 18:19:14.118577 datasetGPT-0.0.3/src/datasetGPT.egg-info/
+-rw-r--r--   0 radicho    (501) staff       (20)    11873 2023-06-22 18:19:14.000000 datasetGPT-0.0.3/src/datasetGPT.egg-info/PKG-INFO
+-rw-r--r--   0 radicho    (501) staff       (20)      444 2023-06-22 18:19:14.000000 datasetGPT-0.0.3/src/datasetGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 radicho    (501) staff       (20)        1 2023-06-22 18:19:14.000000 datasetGPT-0.0.3/src/datasetGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 radicho    (501) staff       (20)       53 2023-06-22 18:19:14.000000 datasetGPT-0.0.3/src/datasetGPT.egg-info/entry_points.txt
+-rw-r--r--   0 radicho    (501) staff       (20)       30 2023-06-22 18:19:14.000000 datasetGPT-0.0.3/src/datasetGPT.egg-info/requires.txt
+-rw-r--r--   0 radicho    (501) staff       (20)       11 2023-06-22 18:19:14.000000 datasetGPT-0.0.3/src/datasetGPT.egg-info/top_level.txt
```

### Comparing `datasetGPT-0.0.2/PKG-INFO` & `datasetGPT-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasetGPT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate textual and conversational datasets with LLMs.
 Home-page: https://github.com/radi-cho/datasetGPT
 Author: Radostin Cholakov
 Author-email: radicho123@gmail.com
 Keywords: dataset,llm,langchain,openai
 Description-Content-Type: text/markdown
```

### Comparing `datasetGPT-0.0.2/README.md` & `datasetGPT-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `datasetGPT-0.0.2/setup.py` & `datasetGPT-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding = "utf-8") as readme:
     long_description = readme.read()
 
 setup(
     name="datasetGPT",
-    version="0.0.2",
+    version="0.0.3",
     description="Generate textual and conversational datasets with LLMs.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author="Radostin Cholakov",
     author_email="radicho123@gmail.com",
     url="https://github.com/radi-cho/datasetGPT",
     # download_url="https://github.com/radi-cho/datasetGPT/archive/v0.0.1.tar.gz",
```

### Comparing `datasetGPT-0.0.2/src/datasetGPT/base.py` & `datasetGPT-0.0.3/src/datasetGPT/base.py`

 * *Files identical despite different names*

### Comparing `datasetGPT-0.0.2/src/datasetGPT/cli.py` & `datasetGPT-0.0.3/src/datasetGPT/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
               type=str,
               required=True,
               help="Agent role description.")
 @click.option("--initial-utterance",
               "-u",
               "initial_utterances",
               type=str,
-              default=["Hello!"],
+              default=["Hello."],
               multiple=True,
               help="Utterance to be provisioned to the first agent. For many use cases a \"Hello\" is enough.")
 @click.option("--interruption",
               "-i",
               "interruption",
               type=click.Choice(["length", "end_phrase"]),
               default="length",
```

### Comparing `datasetGPT-0.0.2/src/datasetGPT/conversations.py` & `datasetGPT-0.0.3/src/datasetGPT/conversations.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 class ConversationsGeneratorConfig:
     openai_api_key: str
     """OpenAI API key."""
     agent1: str
     """Description of the first agent used to construct its system message."""
     agent2: str
     """Description of the second agent used to construct its system message."""
-    initial_utterances: List[str]
+    initial_utterances: List[str] = field(default_factory=lambda: ["Hello."])
     """Utterances to be provisioned to the first agent."""
     num_samples: int = 1
     """Number of conversations to generate for each options combination."""
     interruption: str = "length"
     """Interruption mode."""
     end_phrase: str = "Goodbye!"
     """Phrase to look for when checking whether to interrupt a conversation."""
     end_agent: str = "both"
     """Agent whose messages to check for the interruption phrase."""
     lengths: List[int] = field(default_factory=lambda: [5])
     """Possible lengths of the conversations. If end_phrase interruption is enabled these will be used for maximum lengths."""
-    temperatures: List[int] = field(default_factory=lambda: [0])
+    temperatures: List[float] = field(default_factory=lambda: [0])
     """Possible temperatures for the backend LLM."""
     options: List[Tuple[str, str]] = field(default_factory=lambda: [])
     """Additional options defined in the system prompts with curly brackets."""
 
 
 class ConversationsGenerator(DatasetGenerator):
     """Generator producing conversations between two AI agents."""
@@ -57,14 +57,15 @@
 
     def initialize_options_configs(
         self,
         options_config_keys: List[str] = OPTIONS_CONFIG_KEYS,
         generator_config_keys: List[str] = GENERATOR_CONFIG_KEYS
     ) -> None:
         """Prepare options combinations."""
+        print(self.config.initial_utterances)
         super().initialize_options_configs(options_config_keys, generator_config_keys)
 
     def initialize_chain(
         self,
         agent: str,
         system_prompt: str,
         conversation_config: Dict[str, Any]
```

### Comparing `datasetGPT-0.0.2/src/datasetGPT/outputs.py` & `datasetGPT-0.0.3/src/datasetGPT/outputs.py`

 * *Files identical despite different names*

### Comparing `datasetGPT-0.0.2/src/datasetGPT/texts.py` & `datasetGPT-0.0.3/src/datasetGPT/texts.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """Text prompt."""
     backends: List[Tuple[str, str, str]]
     """LLM APIs to use as backends."""
     num_samples: int = 1
     """Number of texts to generate for each options combination."""
     max_lengths: List[int] = field(default_factory=lambda: [5])
     """Maximum lengths in tokens for the output of each generation."""
-    temperatures: List[int] = field(default_factory=lambda: [0])
+    temperatures: List[float] = field(default_factory=lambda: [0])
     """Possible temperatures for the backend LLM."""
     options: List[Tuple[str, str]] = field(default_factory=lambda: [])
     """Additional options defined in the system prompts with curly brackets."""
 
 
 class TextsGenerator(DatasetGenerator):
     """Generator producing texts by varying model parameters and prompt options."""
```

### Comparing `datasetGPT-0.0.2/src/datasetGPT.egg-info/PKG-INFO` & `datasetGPT-0.0.3/src/datasetGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasetGPT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate textual and conversational datasets with LLMs.
 Home-page: https://github.com/radi-cho/datasetGPT
 Author: Radostin Cholakov
 Author-email: radicho123@gmail.com
 Keywords: dataset,llm,langchain,openai
 Description-Content-Type: text/markdown
```

