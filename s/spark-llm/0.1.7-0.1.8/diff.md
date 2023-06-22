# Comparing `tmp/spark_llm-0.1.7.tar.gz` & `tmp/spark_llm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_llm-0.1.7.tar", max compression
+gzip compressed data, was "spark_llm-0.1.8.tar", max compression
```

## Comparing `spark_llm-0.1.7.tar` & `spark_llm-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.7/LICENSE
--rw-r--r--   0        0        0     3288 2023-06-21 09:05:46.575487 spark_llm-0.1.7/README.md
--rw-r--r--   0        0        0      947 2023-06-22 00:45:00.997343 spark_llm-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.7/spark_llm/__init__.py
--rw-r--r--   0        0        0     2735 2023-06-22 00:45:00.988620 spark_llm-0.1.7/spark_llm/cache.py
--rw-r--r--   0        0        0     1844 2023-06-21 21:53:33.423283 spark_llm-0.1.7/spark_llm/code_logger.py
--rw-r--r--   0        0        0     5224 2023-06-22 00:45:00.988892 spark_llm-0.1.7/spark_llm/file_cache.py
--rw-r--r--   0        0        0     1081 2023-06-22 00:45:00.989285 spark_llm-0.1.7/spark_llm/llm_chain_with_cache.py
--rw-r--r--   0        0        0     3023 2023-06-19 20:17:59.831335 spark_llm-0.1.7/spark_llm/llm_utils.py
--rw-r--r--   0        0        0     8842 2023-06-21 20:01:50.301781 spark_llm-0.1.7/spark_llm/prompt.py
--rw-r--r--   0        0        0      712 2023-06-22 00:45:00.989632 spark_llm-0.1.7/spark_llm/search_tool_with_cache.py
--rw-r--r--   0        0        0    13978 2023-06-22 00:45:00.990097 spark_llm-0.1.7/spark_llm/spark_llm_assistant.py
--rw-r--r--   0        0        0     4494 1970-01-01 00:00:00.000000 spark_llm-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3288 2023-06-21 09:05:46.575487 spark_llm-0.1.8/README.md
+-rw-r--r--   0        0        0      947 2023-06-22 06:02:23.553255 spark_llm-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-22 05:46:03.982132 spark_llm-0.1.8/spark_llm/__init__.py
+-rw-r--r--   0        0        0     2715 2023-06-22 06:02:23.553730 spark_llm-0.1.8/spark_llm/cache.py
+-rw-r--r--   0        0        0     1884 2023-06-22 06:02:23.554103 spark_llm-0.1.8/spark_llm/code_logger.py
+-rw-r--r--   0        0        0     5224 2023-06-22 06:02:23.554607 spark_llm-0.1.8/spark_llm/file_cache.py
+-rw-r--r--   0        0        0     1176 2023-06-22 06:02:23.555001 spark_llm-0.1.8/spark_llm/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     4082 2023-06-22 06:02:19.538963 spark_llm-0.1.8/spark_llm/llm_utils.py
+-rw-r--r--   0        0        0     8783 2023-06-22 06:02:23.555428 spark_llm-0.1.8/spark_llm/prompt.py
+-rw-r--r--   0        0        0      712 2023-06-22 05:46:03.990107 spark_llm-0.1.8/spark_llm/search_tool_with_cache.py
+-rw-r--r--   0        0        0    15424 2023-06-22 06:02:23.555849 spark_llm-0.1.8/spark_llm/spark_llm_assistant.py
+-rw-r--r--   0        0        0     4494 1970-01-01 00:00:00.000000 spark_llm-0.1.8/PKG-INFO
```

### Comparing `spark_llm-0.1.7/LICENSE` & `spark_llm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.7/README.md` & `spark_llm-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.7/pyproject.toml` & `spark_llm-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spark-llm"
-version = "0.1.7"
+version = "0.1.8"
 description = "LLM assistant for the development of Spark applications"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/gengliangwang/spark-llm"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `spark_llm-0.1.7/spark_llm/cache.py` & `spark_llm-0.1.8/spark_llm/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     cache.
 
     Attributes:
         _staging_updates: A dictionary to keep track of the in-memory staging updates.
         _file_cache: An instance of either JsonCache or SQLiteCacheWrapper that acts as the persistent cache.
     """
 
-    def __init__(self,
-                 cache_file_location: str = ".spark_llm.json",
-                 file_format: str = "json"):
+    def __init__(
+        self, cache_file_location: str = ".spark_llm.json", file_format: str = "json"
+    ):
         """
         Initializes a new instance of the Cache class.
 
         Args:
             cache_file_location (str, optional): The path to the cache file for the JsonCache or SQLiteCacheWrapper.
                 Defaults to ".spark_llm.json".
             file_format (str, optional): The format of the file to use for the cache. Defaults to "json".
```

### Comparing `spark_llm-0.1.7/spark_llm/code_logger.py` & `spark_llm-0.1.8/spark_llm/code_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 import re
 import logging
 from pygments import highlight
 from pygments.lexers import get_lexer_by_name, PythonLexer, SqlLexer
 from pygments.formatters import TerminalFormatter
 
-GREEN = '\033[92m'  # terminal code for green
-RESET = '\033[0m'  # reset terminal color
+GREEN = "\033[92m"  # terminal code for green
+RESET = "\033[0m"  # reset terminal color
 
 
 # Custom Formatter
 class CustomFormatter(logging.Formatter):
     def format(self, record):
         return GREEN + "INFO: " + RESET + super().format(record)
 
 
 class CodeLogger:
     def __init__(self, name):
         self.logger = logging.getLogger(name)
         self.logger.setLevel(logging.INFO)
         handler = logging.StreamHandler()
-        handler.setFormatter(CustomFormatter('%(message)s'))  # output only the message
+        handler.setFormatter(CustomFormatter("%(message)s"))  # output only the message
         self.logger.addHandler(handler)
 
     @staticmethod
     def colorize_code(code, language):
-        if not language or language.lower() == 'python':
+        if not language or language.lower() == "python":
             lexer = PythonLexer()
-        elif language.lower() == 'sql':
+        elif language.lower() == "sql":
             lexer = SqlLexer()
         else:
-            raise ValueError(f'Unsupported language: {language}')
+            raise ValueError(f"Unsupported language: {language}")
         return highlight(code, lexer, TerminalFormatter())
 
     def log(self, message):
         # Define pattern to match code blocks with optional language specifiers
         pattern = r"```(python|sql)?(.*?)```"
         # Split message into parts. Every 3rd part will be a code block.
         parts = re.split(pattern, message, flags=re.DOTALL)
 
         colored_message = ""
         for i in range(0, len(parts), 3):
             # Add regular text to the message
             colored_message += parts[i]
             # If there is a code block, colorize it and add it to the message
             if i + 2 < len(parts):
-                colored_message += '\n```\n' + self.colorize_code(parts[i + 2], parts[i + 1]) + '```'
+                colored_message += (
+                    "\n```\n" + self.colorize_code(parts[i + 2], parts[i + 1]) + "```"
+                )
         # Log the message with colored code blocks
         self.logger.info(colored_message)
```

### Comparing `spark_llm-0.1.7/spark_llm/file_cache.py` & `spark_llm-0.1.8/spark_llm/file_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         Args:
             filepath (str): The path to the JSON file to use for the cache.
         """
         self.filepath = filepath
         # If cache file exists, load it into memory.
         self.cache = {}
         if os.path.exists(self.filepath):
-            with open(self.filepath, 'r') as f:
+            with open(self.filepath, "r") as f:
                 for line in f:
                     if line.strip():  # Avoid empty lines
                         line_cache = json.loads(line)
                         self.cache[line_cache["key"]] = line_cache["value"]
         # Create an empty staging cache for storing changes before they are committed.
         self.staging_cache = {}
 
@@ -134,18 +134,18 @@
         the staging cache.
 
         Args:
             staging_cache (Dict[str, str]): The staging cache to be committed.
         """
         # Append the staging cache to the existing cache
         self.cache.update(staging_cache)
-        with open(self.filepath, 'a') as f:
+        with open(self.filepath, "a") as f:
             for key, value in staging_cache.items():
                 json.dump({"key": key, "value": value}, f)
-                f.write('\n')
+                f.write("\n")
         # Clear the staging cache
         self.staging_cache = {}
 
     def clear(self, **kwargs: Any) -> None:
         """Clear the cache.
 
         This method removes all entries from the cache and deletes the cache file.
```

### Comparing `spark_llm-0.1.7/spark_llm/llm_chain_with_cache.py` & `spark_llm-0.1.8/spark_llm/llm_chain_with_cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Any, Optional, List
 
 from langchain import LLMChain
 from langchain.callbacks.manager import Callbacks
 
 from spark_llm.cache import Cache
 
+SKIP_CACHE_TAGS = ["SKIP_CACHE"]
+
 
 class LLMChainWithCache(LLMChain):
     cache: Cache
 
     @staticmethod
     def _sort_and_stringify(*args: Any) -> str:
         # Convert all arguments to strings, then sort them
@@ -22,13 +24,15 @@
         *args: Any,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> str:
         assert not args, "The chain expected no arguments"
         prompt_str = self.prompt.format_prompt(**kwargs).to_string()
-        cached_result = self.cache.lookup(prompt_str)
+        cached_result = (
+            self.cache.lookup(prompt_str) if tags != SKIP_CACHE_TAGS else None
+        )
         if cached_result is not None:
             return cached_result
         result = super().run(*args, callbacks=callbacks, tags=tags, **kwargs)
         self.cache.update(prompt_str, result)
         return result
```

### Comparing `spark_llm-0.1.7/spark_llm/prompt.py` & `spark_llm-0.1.8/spark_llm/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,39 +209,45 @@
 
 _udf_output2 = """
 def add_one(x) -> int:
     if x is not None:
         return x + 1
 """
 
-_udf_examples = [{"input_args_types": "(s: str)", 
-                  "desc": "Convert string s to uppercase", 
-                  "return_type": "str", 
-                  "udf_name": "to_upper", 
-                  "output": _udf_output1},
-                {"input_args_types": "(x: int)", 
-                  "desc": "Add 1", 
-                  "return_type": "int", 
-                  "udf_name": "add_one", 
-                  "output": _udf_output2}]
+_udf_examples = [
+    {
+        "input_args_types": "(s: str)",
+        "desc": "Convert string s to uppercase",
+        "return_type": "str",
+        "udf_name": "to_upper",
+        "output": _udf_output1,
+    },
+    {
+        "input_args_types": "(x: int)",
+        "desc": "Add 1",
+        "return_type": "int",
+        "udf_name": "add_one",
+        "output": _udf_output2,
+    },
+]
 
 _udf_formatter = """
 input_args_types: {input_args_types}
 desc: {desc}
 return_type: {return_type}
 udf_name: {udf_name}
 output: {output}
 """
 
 _udf_prompt = PromptTemplate(
-    input_variables=["input_args_types", "desc", "return_type", "udf_name", "output"], template=_udf_formatter
+    input_variables=["input_args_types", "desc", "return_type", "udf_name", "output"],
+    template=_udf_formatter,
 )
 
 UDF_PROMPT = FewShotPromptTemplate(
     examples=_udf_examples,
     example_prompt=_udf_prompt,
     prefix=UDF_PREFIX,
     suffix=UDF_SUFFIX,
     input_variables=["input_args_types", "desc", "return_type", "udf_name"],
     example_separator="\n\n",
 )
-
```

### Comparing `spark_llm-0.1.7/spark_llm/search_tool_with_cache.py` & `spark_llm-0.1.8/spark_llm/search_tool_with_cache.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.7/spark_llm/spark_llm_assistant.py` & `spark_llm-0.1.8/spark_llm/spark_llm_assistant.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 from langchain import LLMChain, GoogleSearchAPIWrapper, BasePromptTemplate
 from langchain.base_language import BaseLanguageModel
 from pyspark.sql import SparkSession, DataFrame
 from tiktoken import Encoding
 
 from spark_llm.cache import Cache
 from spark_llm.code_logger import CodeLogger
-from spark_llm.llm_chain_with_cache import LLMChainWithCache
+from spark_llm.llm_chain_with_cache import LLMChainWithCache, SKIP_CACHE_TAGS
 from spark_llm.prompt import (
     SEARCH_PROMPT,
     SQL_PROMPT,
     EXPLAIN_DF_PROMPT,
     TRANSFORM_PROMPT,
     PLOT_PROMPT,
     VERIFY_PROMPT,
-    UDF_PROMPT
+    UDF_PROMPT,
 )
 from spark_llm.search_tool_with_cache import SearchToolWithCache
 from spark_llm.llm_utils import LLMUtils
 
 
 class SparkLLMAssistant:
     _HTTP_HEADER = {
@@ -59,15 +59,18 @@
         :param encoding: optional Encoding, cl100k_base will be used if not provided
         :param max_tokens_of_web_content: maximum tokens of web content after encoding
         """
         self._spark = spark_session or SparkSession.builder.getOrCreate()
         self._llm = llm
         self._web_search_tool = web_search_tool or self._default_web_search_tool
         if enable_cache:
-            self._cache = Cache(cache_file_location=cache_file_location, file_format=cache_file_format)
+            self._enable_cache = enable_cache
+            self._cache = Cache(
+                cache_file_location=cache_file_location, file_format=cache_file_format
+            )
             self._web_search_tool = SearchToolWithCache(
                 self._web_search_tool, self._cache
             ).search
         else:
             self._cache = None
         self._encoding = encoding or tiktoken.get_encoding("cl100k_base")
         self._max_tokens_of_web_content = max_tokens_of_web_content
@@ -164,38 +167,45 @@
         :return: trimmed text
         """
         tokens = list(self._encoding.encode(text))
         if len(tokens) > max_tokens:
             tokens = tokens[:max_tokens]
         return self._encoding.decode(tokens)
 
-    def _get_url_from_search_tool(self, desc: str, columns: Optional[List[str]]) -> str:
+    def _get_url_from_search_tool(
+        self, desc: str, columns: Optional[List[str]], use_cache: bool
+    ) -> str:
         search_result = self._web_search_tool(desc)
         search_columns_hint = self._generate_search_prompt(columns)
         # Run the LLM chain to pick the best search result
+        tags = self._get_tags(use_cache)
         return self._search_llm_chain.run(
-            query=desc, search_results=search_result, columns={search_columns_hint}
+            tags=tags,
+            query=desc,
+            search_results=search_result,
+            columns={search_columns_hint},
         )
 
     def _create_dataframe_with_llm(
-        self, text: str, desc: str, columns: Optional[List[str]]
+        self, text: str, desc: str, columns: Optional[List[str]], use_cache: bool
     ) -> DataFrame:
         clean_text = " ".join(text.split())
         web_content = self._trim_text_from_end(
             clean_text, self._max_tokens_of_web_content
         )
 
         sql_columns_hint = self._generate_sql_prompt(columns)
 
         # Run the LLM chain to get an ingestion SQL query
+        tags = self._get_tags(use_cache)
         llm_result = self._sql_llm_chain.run(
-            query=desc, web_content=web_content, columns=sql_columns_hint
+            tags=tags, query=desc, web_content=web_content, columns=sql_columns_hint
         )
         sql_query = self._extract_code_blocks(llm_result)[0]
-        formatted_sql_query=CodeLogger.colorize_code(sql_query, "sql")
+        formatted_sql_query = CodeLogger.colorize_code(sql_query, "sql")
         self.log(f"SQL query for the ingestion:\n{formatted_sql_query}")
 
         view_name = self._extract_view_name(sql_query)
         self.log(f"Storing data into temp view: {view_name}\n")
         self._spark.sql(sql_query)
         return self._spark.table(view_name)
 
@@ -208,32 +218,44 @@
         pattern = r"#\d+"
 
         # Remove matching patterns
         trimmed_plan = re.sub(pattern, "", analyzed_plan)
 
         return trimmed_plan
 
-    def _get_df_explain(self, df: DataFrame) -> str:
+    def _get_df_explain(self, df: DataFrame, use_cache: bool) -> str:
         raw_analyzed_str = df._jdf.queryExecution().analyzed().toString()
-        return self._explain_chain.run(input=self._trim_hash_id(raw_analyzed_str))
+        tags = self._get_tags(use_cache)
+        return self._explain_chain.run(
+            tags=tags, input=self._trim_hash_id(raw_analyzed_str)
+        )
 
-    def create_df(self, desc: str, columns: Optional[List[str]] = None) -> DataFrame:
+    def _get_tags(self, use_cache: bool) -> Optional[List[str]]:
+        if self._enable_cache and not use_cache:
+            return SKIP_CACHE_TAGS
+        return None
+
+    def create_df(
+        self, desc: str, columns: Optional[List[str]] = None, use_cache: bool = True
+    ) -> DataFrame:
         """
         Create a Spark DataFrame by querying an LLM from web search result.
 
         :param desc: the description of the result DataFrame, which will be used for
                      web searching
         :param columns: the expected column names in the result DataFrame
+        :param use_cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
+
         :return: a Spark DataFrame
         """
         url = desc.strip()  # Remove leading and trailing whitespace
         is_url = self._is_http_or_https_url(url)
         # If the input is not a valid URL, use search tool to get the dataset.
         if not is_url:
-            url = self._get_url_from_search_tool(desc, columns)
+            url = self._get_url_from_search_tool(desc, columns, use_cache)
 
         self.log(f"Parsing URL: {url}\n")
         try:
             response = requests.get(url, headers=self._HTTP_HEADER)
             response.raise_for_status()
         except requests.exceptions.HTTPError as http_err:
             self.log(f"HTTP error occurred: {http_err}")
@@ -242,73 +264,86 @@
             self.log(f"Other error occurred: {err}")
             return
 
         soup = BeautifulSoup(response.text, "html.parser")
         # If the input is a URL link, use the title of web page as the dataset's description.
         if is_url:
             desc = soup.title.string
-        return self._create_dataframe_with_llm(soup.get_text(), desc, columns)
+        return self._create_dataframe_with_llm(
+            soup.get_text(), desc, columns, use_cache
+        )
 
-    def transform_df(self, df: DataFrame, desc: str) -> DataFrame:
+    def transform_df(
+        self, df: DataFrame, desc: str, use_cache: bool = True
+    ) -> DataFrame:
         """
         This method applies a transformation to a provided Spark DataFrame, the specifics of which are determined by the 'desc' parameter.
 
         :param df: The Spark DataFrame that is to be transformed.
         :param desc: A natural language string that outlines the specific transformation to be applied on the DataFrame.
+        :param use_cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
 
         :return: Returns a new Spark DataFrame that is the result of applying the specified transformation on the input DataFrame.
         """
         temp_view_name = "temp_view_for_transform"
         df.createOrReplaceTempView(temp_view_name)
         schema_str = self._get_df_schema(df)
+        tags = self._get_tags(use_cache)
         llm_result = self._transform_chain.run(
-            view_name=temp_view_name, columns=schema_str, desc=desc
+            tags=tags, view_name=temp_view_name, columns=schema_str, desc=desc
         )
         sql_query = self._extract_code_blocks(llm_result)[0]
-        formatted_sql_query=CodeLogger.colorize_code(sql_query, "sql")
+        formatted_sql_query = CodeLogger.colorize_code(sql_query, "sql")
         self.log(f"SQL query for the transform:\n{formatted_sql_query}")
         return self._spark.sql(sql_query)
 
-    def explain_df(self, df: DataFrame) -> str:
+    def explain_df(self, df: DataFrame, use_cache: bool = True) -> str:
         """
         This method generates a natural language explanation of the SQL plan of the input Spark DataFrame.
 
         :param df: The Spark DataFrame to be explained.
+        :param use_cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
 
         :return: A string explanation of the DataFrame's SQL plan, detailing what the DataFrame is intended to retrieve.
         """
-        explain_result = self._get_df_explain(df)
+        explain_result = self._get_df_explain(df, use_cache)
         # If there is code block in the explain result, ignore it.
         if "```" in explain_result:
             summary = explain_result.split("```")[-1]
             return summary.strip()
         else:
             return explain_result
 
-    def plot_df(self, df: DataFrame, desc: Optional[str] = None) -> None:
+    def plot_df(
+        self, df: DataFrame, desc: Optional[str] = None, use_cache: bool = True
+    ) -> None:
         instruction = f"The purpose of the plot: {desc}" if desc is not None else ""
+        tags = self._get_tags(use_cache)
         response = self._plot_chain.run(
+            tags=tags,
             columns=self._get_df_schema(df),
-            explain=self._get_df_explain(df),
+            explain=self._get_df_explain(df, use_cache),
             instruction=instruction,
         )
         self.log(response)
         codeblocks = self._extract_code_blocks(response)
         for code in codeblocks:
             exec(code)
 
-    def verify_df(self, df: DataFrame, desc: str) -> None:
+    def verify_df(self, df: DataFrame, desc: str, use_cache: bool = True) -> None:
         """
         This method creates and runs test cases for the provided PySpark dataframe transformation function.
 
         :param df: The Spark DataFrame to be verified
         :param desc: A description of the expectation to be verified
+        :param use_cache: If `True`, fetches cached data, if available. If `False`, retrieves fresh data and updates cache.
         """
-        llm_output = self._verify_chain.run(df=df, desc=desc)
-        formatted_code=CodeLogger.colorize_code(llm_output, "python")
+        tags = self._get_tags(use_cache)
+        llm_output = self._verify_chain.run(tags=tags, df=df, desc=desc)
+        formatted_code = CodeLogger.colorize_code(llm_output, "python")
         self.log(f"Generated code:\n{formatted_code}")
 
         locals_ = {}
         exec(llm_output, {"df": df}, locals_)
 
         self.log(f"\nResult: {locals_['result']}")
 
@@ -321,18 +356,18 @@
         return_type = func_signature.split("->")[1].strip()
         udf_name = func.__name__
 
         code = self._udf_chain.run(
             input_args_types=input_args_types,
             desc=desc,
             return_type=return_type,
-            udf_name=udf_name
+            udf_name=udf_name,
         )
 
-        formatted_code=CodeLogger.colorize_code(code, "python")
+        formatted_code = CodeLogger.colorize_code(code, "python")
         self.log(f"Creating following Python UDF:\n{formatted_code}")
 
         locals_ = {}
         exec(code, globals(), locals_)
 
         return locals_[udf_name]
```

### Comparing `spark_llm-0.1.7/PKG-INFO` & `spark_llm-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-llm
-Version: 0.1.7
+Version: 0.1.8
 Summary: LLM assistant for the development of Spark applications
 Home-page: https://github.com/gengliangwang/spark-llm
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

