# Comparing `tmp/spark_llm-0.1.8.tar.gz` & `tmp/spark_llm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_llm-0.1.8.tar", max compression
+gzip compressed data, was "spark_llm-0.1.9.tar", max compression
```

## Comparing `spark_llm-0.1.8.tar` & `spark_llm-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.8/LICENSE
--rw-r--r--   0        0        0     3288 2023-06-21 09:05:46.575487 spark_llm-0.1.8/README.md
--rw-r--r--   0        0        0      947 2023-06-22 06:02:23.553255 spark_llm-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-22 05:46:03.982132 spark_llm-0.1.8/spark_llm/__init__.py
--rw-r--r--   0        0        0     2715 2023-06-22 06:02:23.553730 spark_llm-0.1.8/spark_llm/cache.py
--rw-r--r--   0        0        0     1884 2023-06-22 06:02:23.554103 spark_llm-0.1.8/spark_llm/code_logger.py
--rw-r--r--   0        0        0     5224 2023-06-22 06:02:23.554607 spark_llm-0.1.8/spark_llm/file_cache.py
--rw-r--r--   0        0        0     1176 2023-06-22 06:02:23.555001 spark_llm-0.1.8/spark_llm/llm_chain_with_cache.py
--rw-r--r--   0        0        0     4082 2023-06-22 06:02:19.538963 spark_llm-0.1.8/spark_llm/llm_utils.py
--rw-r--r--   0        0        0     8783 2023-06-22 06:02:23.555428 spark_llm-0.1.8/spark_llm/prompt.py
--rw-r--r--   0        0        0      712 2023-06-22 05:46:03.990107 spark_llm-0.1.8/spark_llm/search_tool_with_cache.py
--rw-r--r--   0        0        0    15424 2023-06-22 06:02:23.555849 spark_llm-0.1.8/spark_llm/spark_llm_assistant.py
--rw-r--r--   0        0        0     4494 1970-01-01 00:00:00.000000 spark_llm-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3158 2023-06-22 20:12:51.627414 spark_llm-0.1.9/README.md
+-rw-r--r--   0        0        0      984 2023-06-22 20:22:53.048362 spark_llm-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-22 20:15:31.551187 spark_llm-0.1.9/spark_llm/__init__.py
+-rw-r--r--   0        0        0     2715 2023-06-22 20:15:31.552455 spark_llm-0.1.9/spark_llm/cache.py
+-rw-r--r--   0        0        0     1905 2023-06-22 20:15:31.553201 spark_llm-0.1.9/spark_llm/code_logger.py
+-rw-r--r--   0        0        0     5224 2023-06-22 20:15:31.554009 spark_llm-0.1.9/spark_llm/file_cache.py
+-rw-r--r--   0        0        0     1232 2023-06-22 20:22:53.041214 spark_llm-0.1.9/spark_llm/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     4034 2023-06-22 20:22:53.041553 spark_llm-0.1.9/spark_llm/llm_utils.py
+-rw-r--r--   0        0        0     8783 2023-06-22 20:15:31.556401 spark_llm-0.1.9/spark_llm/prompt.py
+-rw-r--r--   0        0        0      712 2023-06-22 20:15:31.557246 spark_llm-0.1.9/spark_llm/search_tool_with_cache.py
+-rw-r--r--   0        0        0    15421 2023-06-22 20:22:53.041910 spark_llm-0.1.9/spark_llm/spark_llm_assistant.py
+-rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 spark_llm-0.1.9/PKG-INFO
```

### Comparing `spark_llm-0.1.8/LICENSE` & `spark_llm-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.8/README.md` & `spark_llm-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 ```bash
 pip install spark-llm
 ```
 
 ## Usage
 ### Initialization
 ```python
-from langchain.chat_models import ChatOpenAI
 from spark_llm import SparkLLMAssistant
 
-llm = ChatOpenAI(model_name='gpt-4') # using gpt-4 can achieve better results
-assistant = SparkLLMAssistant(llm=llm)
+assistant = SparkLLMAssistant()
 assistant.activate() # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
 ```python
 auto_df = assistant.create_df("2022 USA national auto sales by brand")
 auto_df.show(n=5)
```

### Comparing `spark_llm-0.1.8/pyproject.toml` & `spark_llm-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spark-llm"
-version = "0.1.8"
+version = "0.1.9"
 description = "LLM assistant for the development of Spark applications"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/gengliangwang/spark-llm"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -26,11 +26,12 @@
 tiktoken = "0.4.0"
 beautifulsoup4 = "^4.12.2"
 pyspark = "^3.4.0"
 openai = "^0.27.8"
 langchain = "^0.0.201"
 pandas = "^2.0.2"
 pygments = "^2.15.1"
+google-api-python-client = "^2.90.0"
 
 
 [tool.poetry.dev-dependencies]
```

### Comparing `spark_llm-0.1.8/spark_llm/cache.py` & `spark_llm-0.1.9/spark_llm/cache.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.8/spark_llm/code_logger.py` & `spark_llm-0.1.9/spark_llm/code_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import logging
+import sys
 from pygments import highlight
 from pygments.lexers import get_lexer_by_name, PythonLexer, SqlLexer
 from pygments.formatters import TerminalFormatter
 
 GREEN = "\033[92m"  # terminal code for green
 RESET = "\033[0m"  # reset terminal color
 
@@ -14,15 +15,15 @@
         return GREEN + "INFO: " + RESET + super().format(record)
 
 
 class CodeLogger:
     def __init__(self, name):
         self.logger = logging.getLogger(name)
         self.logger.setLevel(logging.INFO)
-        handler = logging.StreamHandler()
+        handler = logging.StreamHandler(sys.stdout)
         handler.setFormatter(CustomFormatter("%(message)s"))  # output only the message
         self.logger.addHandler(handler)
 
     @staticmethod
     def colorize_code(code, language):
         if not language or language.lower() == "python":
             lexer = PythonLexer()
```

### Comparing `spark_llm-0.1.8/spark_llm/file_cache.py` & `spark_llm-0.1.9/spark_llm/file_cache.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.8/spark_llm/llm_chain_with_cache.py` & `spark_llm-0.1.9/spark_llm/llm_chain_with_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,17 @@
         *args: Any,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> str:
         assert not args, "The chain expected no arguments"
         prompt_str = self.prompt.format_prompt(**kwargs).to_string()
+        use_cache = tags != SKIP_CACHE_TAGS
         cached_result = (
-            self.cache.lookup(prompt_str) if tags != SKIP_CACHE_TAGS else None
+            self.cache.lookup(prompt_str) if use_cache else None
         )
         if cached_result is not None:
             return cached_result
         result = super().run(*args, callbacks=callbacks, tags=tags, **kwargs)
-        self.cache.update(prompt_str, result)
+        if use_cache:
+            self.cache.update(prompt_str, result)
         return result
```

### Comparing `spark_llm-0.1.8/spark_llm/llm_utils.py` & `spark_llm-0.1.9/spark_llm/llm_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,67 +17,67 @@
         Args:
             assistant: The SparkLLMAssistant instance containing the LLM utility methods.
             df_instance: The DataFrame instance on which the utility methods will be used.
         """
         self.assistant = assistant
         self.df_instance = df_instance
 
-    def transform(self, desc: str, use_cache: bool = True) -> DataFrame:
+    def transform(self, desc: str, cache: bool = True) -> DataFrame:
         """
         Transform the DataFrame using the given description.
 
         Args:
             desc: A string description specifying the transformation.
-            use_cache: Indicates whether to utilize a cache for this method.
+            cache: Indicates whether to utilize a cache for this method.
                 If `True`, fetches cached data, if available.
                 If `False`, retrieves fresh data and updates cache.
 
         Returns:
             The transformed DataFrame.
         """
-        return self.assistant.transform_df(self.df_instance, desc, use_cache)
+        return self.assistant.transform_df(self.df_instance, desc, cache)
 
-    def explain(self, use_cache: bool = True) -> str:
+    def explain(self, cache: bool = True) -> str:
         """
         Explain the DataFrame.
 
         Args:
-            use_cache: Indicates whether to utilize a cache for this method.
+            cache: Indicates whether to utilize a cache for this method.
                 If `True`, fetches cached data, if available.
                 If `False`, retrieves fresh data and updates cache.
 
         Returns:
             A string explanation of the DataFrame.
 
         """
-        return self.assistant.explain_df(self.df_instance, use_cache)
+        return self.assistant.explain_df(self.df_instance, cache)
 
-    def plot(self, desc: Optional[str] = None, use_cache: bool = True) -> None:
+    def plot(self, desc: Optional[str] = None, cache: bool = True) -> None:
         """
         Plot the DataFrame.
 
         Args:
             desc: A string description specifying the plot.
-            use_cache: Indicates whether to utilize a cache for this method.
+            cache: Indicates whether to utilize a cache for this method.
                 If `True`, fetches cached data, if available.
                 If `False`, retrieves fresh data and updates cache.
         """
-        return self.assistant.plot_df(self.df_instance, desc, use_cache)
+        return self.assistant.plot_df(self.df_instance, desc, cache)
 
-    def verify(self, desc: str, use_cache: bool = True) -> None:
+    def verify(self, desc: str, cache: bool = True) -> None:
         """
         Verify the DataFrame using the given description.
 
         Args:
             desc: A string description specifying what to verify in the DataFrame.
-            use_cache: Indicates whether to utilize a cache for this method.
+            cache: Indicates whether to utilize a cache for this method.
                 If `True`, fetches cached data, if available.
                 If `False`, retrieves fresh data and updates cache.
         """
-        return self.assistant.verify_df(self.df_instance, desc, use_cache)
+        return self.assistant.verify_df(self.df_instance, desc, cache)
 
 
 class LLMUtils:
     """
     This class is a descriptor that is used to add LLM utility methods to DataFrame instances.
     When the utility methods are accessed, it returns a new LLMMethodWrapper instance with the
     DataFrame instance and LLM assistant passed to it.
```

### Comparing `spark_llm-0.1.8/spark_llm/prompt.py` & `spark_llm-0.1.9/spark_llm/prompt.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.8/spark_llm/search_tool_with_cache.py` & `spark_llm-0.1.9/spark_llm/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.8/spark_llm/spark_llm_assistant.py` & `spark_llm-0.1.9/spark_llm/spark_llm_assistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from urllib.parse import urlparse
 
 import requests
 import tiktoken
 from bs4 import BeautifulSoup
 from langchain import LLMChain, GoogleSearchAPIWrapper, BasePromptTemplate
 from langchain.base_language import BaseLanguageModel
+from langchain.chat_models import ChatOpenAI
 from pyspark.sql import SparkSession, DataFrame
 from tiktoken import Encoding
 
 from spark_llm.cache import Cache
 from spark_llm.code_logger import CodeLogger
 from spark_llm.llm_chain_with_cache import LLMChainWithCache, SKIP_CACHE_TAGS
 from spark_llm.prompt import (
@@ -34,15 +35,15 @@
         " (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
         "Accept-Language": "en-US,en;q=0.5",
     }
 
     def __init__(
         self,
-        llm: BaseLanguageModel,
+        llm: BaseLanguageModel = ChatOpenAI(model_name='gpt-4', temperature=0),
         web_search_tool: Optional[Callable[[str], str]] = None,
         spark_session: Optional[SparkSession] = None,
         enable_cache: bool = True,
         cache_file_format: str = "json",
         cache_file_location: str = "spark_llm_cache.json",
         encoding: Optional[Encoding] = None,
         max_tokens_of_web_content: int = 3000,
@@ -168,39 +169,39 @@
         """
         tokens = list(self._encoding.encode(text))
         if len(tokens) > max_tokens:
             tokens = tokens[:max_tokens]
         return self._encoding.decode(tokens)
 
     def _get_url_from_search_tool(
-        self, desc: str, columns: Optional[List[str]], use_cache: bool
+        self, desc: str, columns: Optional[List[str]], cache: bool
     ) -> str:
         search_result = self._web_search_tool(desc)
         search_columns_hint = self._generate_search_prompt(columns)
         # Run the LLM chain to pick the best search result
-        tags = self._get_tags(use_cache)
+        tags = self._get_tags(cache)
         return self._search_llm_chain.run(
             tags=tags,
             query=desc,
             search_results=search_result,
             columns={search_columns_hint},
         )
 
     def _create_dataframe_with_llm(
-        self, text: str, desc: str, columns: Optional[List[str]], use_cache: bool
+        self, text: str, desc: str, columns: Optional[List[str]], cache: bool
     ) -> DataFrame:
         clean_text = " ".join(text.split())
         web_content = self._trim_text_from_end(
             clean_text, self._max_tokens_of_web_content
         )
 
         sql_columns_hint = self._generate_sql_prompt(columns)
 
         # Run the LLM chain to get an ingestion SQL query
-        tags = self._get_tags(use_cache)
+        tags = self._get_tags(cache)
         llm_result = self._sql_llm_chain.run(
             tags=tags, query=desc, web_content=web_content, columns=sql_columns_hint
         )
         sql_query = self._extract_code_blocks(llm_result)[0]
         formatted_sql_query = CodeLogger.colorize_code(sql_query, "sql")
         self.log(f"SQL query for the ingestion:\n{formatted_sql_query}")
 
@@ -218,44 +219,44 @@
         pattern = r"#\d+"
 
         # Remove matching patterns
         trimmed_plan = re.sub(pattern, "", analyzed_plan)
 
         return trimmed_plan
 
-    def _get_df_explain(self, df: DataFrame, use_cache: bool) -> str:
+    def _get_df_explain(self, df: DataFrame, cache: bool) -> str:
         raw_analyzed_str = df._jdf.queryExecution().analyzed().toString()
-        tags = self._get_tags(use_cache)
+        tags = self._get_tags(cache)
         return self._explain_chain.run(
             tags=tags, input=self._trim_hash_id(raw_analyzed_str)
         )
 
-    def _get_tags(self, use_cache: bool) -> Optional[List[str]]:
-        if self._enable_cache and not use_cache:
+    def _get_tags(self, cache: bool) -> Optional[List[str]]:
+        if self._enable_cache and not cache:
             return SKIP_CACHE_TAGS
         return None
 
     def create_df(
-        self, desc: str, columns: Optional[List[str]] = None, use_cache: bool = True
+        self, desc: str, columns: Optional[List[str]] = None, cache: bool = True
     ) -> DataFrame:
         """
         Create a Spark DataFrame by querying an LLM from web search result.
 
         :param desc: the description of the result DataFrame, which will be used for
                      web searching
         :param columns: the expected column names in the result DataFrame
-        :param use_cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
+        :param cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
 
         :return: a Spark DataFrame
         """
         url = desc.strip()  # Remove leading and trailing whitespace
         is_url = self._is_http_or_https_url(url)
         # If the input is not a valid URL, use search tool to get the dataset.
         if not is_url:
-            url = self._get_url_from_search_tool(desc, columns, use_cache)
+            url = self._get_url_from_search_tool(desc, columns, cache)
 
         self.log(f"Parsing URL: {url}\n")
         try:
             response = requests.get(url, headers=self._HTTP_HEADER)
             response.raise_for_status()
         except requests.exceptions.HTTPError as http_err:
             self.log(f"HTTP error occurred: {http_err}")
@@ -265,83 +266,83 @@
             return
 
         soup = BeautifulSoup(response.text, "html.parser")
         # If the input is a URL link, use the title of web page as the dataset's description.
         if is_url:
             desc = soup.title.string
         return self._create_dataframe_with_llm(
-            soup.get_text(), desc, columns, use_cache
+            soup.get_text(), desc, columns, cache
         )
 
     def transform_df(
-        self, df: DataFrame, desc: str, use_cache: bool = True
+        self, df: DataFrame, desc: str, cache: bool = True
     ) -> DataFrame:
         """
         This method applies a transformation to a provided Spark DataFrame, the specifics of which are determined by the 'desc' parameter.
 
         :param df: The Spark DataFrame that is to be transformed.
         :param desc: A natural language string that outlines the specific transformation to be applied on the DataFrame.
-        :param use_cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
+        :param cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
 
         :return: Returns a new Spark DataFrame that is the result of applying the specified transformation on the input DataFrame.
         """
         temp_view_name = "temp_view_for_transform"
         df.createOrReplaceTempView(temp_view_name)
         schema_str = self._get_df_schema(df)
-        tags = self._get_tags(use_cache)
+        tags = self._get_tags(cache)
         llm_result = self._transform_chain.run(
             tags=tags, view_name=temp_view_name, columns=schema_str, desc=desc
         )
         sql_query = self._extract_code_blocks(llm_result)[0]
         formatted_sql_query = CodeLogger.colorize_code(sql_query, "sql")
         self.log(f"SQL query for the transform:\n{formatted_sql_query}")
         return self._spark.sql(sql_query)
 
-    def explain_df(self, df: DataFrame, use_cache: bool = True) -> str:
+    def explain_df(self, df: DataFrame, cache: bool = True) -> str:
         """
         This method generates a natural language explanation of the SQL plan of the input Spark DataFrame.
 
         :param df: The Spark DataFrame to be explained.
-        :param use_cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
+        :param cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
 
         :return: A string explanation of the DataFrame's SQL plan, detailing what the DataFrame is intended to retrieve.
         """
-        explain_result = self._get_df_explain(df, use_cache)
+        explain_result = self._get_df_explain(df, cache)
         # If there is code block in the explain result, ignore it.
         if "```" in explain_result:
             summary = explain_result.split("```")[-1]
             return summary.strip()
         else:
             return explain_result
 
     def plot_df(
-        self, df: DataFrame, desc: Optional[str] = None, use_cache: bool = True
+        self, df: DataFrame, desc: Optional[str] = None, cache: bool = True
     ) -> None:
         instruction = f"The purpose of the plot: {desc}" if desc is not None else ""
-        tags = self._get_tags(use_cache)
+        tags = self._get_tags(cache)
         response = self._plot_chain.run(
             tags=tags,
             columns=self._get_df_schema(df),
-            explain=self._get_df_explain(df, use_cache),
+            explain=self._get_df_explain(df, cache),
             instruction=instruction,
         )
         self.log(response)
         codeblocks = self._extract_code_blocks(response)
         for code in codeblocks:
             exec(code)
 
-    def verify_df(self, df: DataFrame, desc: str, use_cache: bool = True) -> None:
+    def verify_df(self, df: DataFrame, desc: str, cache: bool = True) -> None:
         """
         This method creates and runs test cases for the provided PySpark dataframe transformation function.
 
         :param df: The Spark DataFrame to be verified
         :param desc: A description of the expectation to be verified
-        :param use_cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
+        :param cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
         """
-        tags = self._get_tags(use_cache)
+        tags = self._get_tags(cache)
         llm_output = self._verify_chain.run(tags=tags, df=df, desc=desc)
         formatted_code = CodeLogger.colorize_code(llm_output, "python")
         self.log(f"Generated code:\n{formatted_code}")
 
         locals_ = {}
         exec(llm_output, {"df": df}, locals_)
```

### Comparing `spark_llm-0.1.8/PKG-INFO` & `spark_llm-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-llm
-Version: 0.1.8
+Version: 0.1.9
 Summary: LLM assistant for the development of Spark applications
 Home-page: https://github.com/gengliangwang/spark-llm
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: google-api-python-client (>=2.90.0,<3.0.0)
 Requires-Dist: langchain (>=0.0.201,<0.0.202)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: pyspark (>=3.4.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tiktoken (==0.4.0)
@@ -35,19 +36,17 @@
 ```bash
 pip install spark-llm
 ```
 
 ## Usage
 ### Initialization
 ```python
-from langchain.chat_models import ChatOpenAI
 from spark_llm import SparkLLMAssistant
 
-llm = ChatOpenAI(model_name='gpt-4') # using gpt-4 can achieve better results
-assistant = SparkLLMAssistant(llm=llm)
+assistant = SparkLLMAssistant()
 assistant.activate() # active partial functions for Spark DataFrame
 ```
 
 ### Data Ingestion
 ```python
 auto_df = assistant.create_df("2022 USA national auto sales by brand")
 auto_df.show(n=5)
```

