# Comparing `tmp/spark_llm-0.1.6.tar.gz` & `tmp/spark_llm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_llm-0.1.6.tar", max compression
+gzip compressed data, was "spark_llm-0.1.7.tar", max compression
```

## Comparing `spark_llm-0.1.6.tar` & `spark_llm-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.6/LICENSE
--rw-r--r--   0        0        0     3288 2023-06-21 09:05:46.575487 spark_llm-0.1.6/README.md
--rw-r--r--   0        0        0      947 2023-06-21 20:02:07.581768 spark_llm-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.6/spark_llm/__init__.py
--rw-r--r--   0        0        0     2650 2023-06-21 09:05:46.581124 spark_llm-0.1.6/spark_llm/cache.py
--rw-r--r--   0        0        0     1946 2023-06-21 20:01:50.301401 spark_llm-0.1.6/spark_llm/code_logger.py
--rw-r--r--   0        0        0     1093 2023-06-20 22:40:29.711290 spark_llm-0.1.6/spark_llm/llm_chain_with_cache.py
--rw-r--r--   0        0        0     3023 2023-06-19 20:17:59.831335 spark_llm-0.1.6/spark_llm/llm_utils.py
--rw-r--r--   0        0        0     8842 2023-06-21 20:01:50.301781 spark_llm-0.1.6/spark_llm/prompt.py
--rw-r--r--   0        0        0      688 2023-06-16 21:50:36.342058 spark_llm-0.1.6/spark_llm/search_tool_with_cache.py
--rw-r--r--   0        0        0    13837 2023-06-21 20:01:50.302232 spark_llm-0.1.6/spark_llm/spark_llm_assistant.py
--rw-r--r--   0        0        0     4494 1970-01-01 00:00:00.000000 spark_llm-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 17:49:03.107485 spark_llm-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3288 2023-06-21 09:05:46.575487 spark_llm-0.1.7/README.md
+-rw-r--r--   0        0        0      947 2023-06-22 00:45:00.997343 spark_llm-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-09 17:49:03.120504 spark_llm-0.1.7/spark_llm/__init__.py
+-rw-r--r--   0        0        0     2735 2023-06-22 00:45:00.988620 spark_llm-0.1.7/spark_llm/cache.py
+-rw-r--r--   0        0        0     1844 2023-06-21 21:53:33.423283 spark_llm-0.1.7/spark_llm/code_logger.py
+-rw-r--r--   0        0        0     5224 2023-06-22 00:45:00.988892 spark_llm-0.1.7/spark_llm/file_cache.py
+-rw-r--r--   0        0        0     1081 2023-06-22 00:45:00.989285 spark_llm-0.1.7/spark_llm/llm_chain_with_cache.py
+-rw-r--r--   0        0        0     3023 2023-06-19 20:17:59.831335 spark_llm-0.1.7/spark_llm/llm_utils.py
+-rw-r--r--   0        0        0     8842 2023-06-21 20:01:50.301781 spark_llm-0.1.7/spark_llm/prompt.py
+-rw-r--r--   0        0        0      712 2023-06-22 00:45:00.989632 spark_llm-0.1.7/spark_llm/search_tool_with_cache.py
+-rw-r--r--   0        0        0    13978 2023-06-22 00:45:00.990097 spark_llm-0.1.7/spark_llm/spark_llm_assistant.py
+-rw-r--r--   0        0        0     4494 1970-01-01 00:00:00.000000 spark_llm-0.1.7/PKG-INFO
```

### Comparing `spark_llm-0.1.6/LICENSE` & `spark_llm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.6/README.md` & `spark_llm-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.6/pyproject.toml` & `spark_llm-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "spark-llm"
-version = "0.1.6"
+version = "0.1.7"
 description = "LLM assistant for the development of Spark applications"
 authors = ["Gengliang Wang <gengliang@apache.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/gengliangwang/spark-llm"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `spark_llm-0.1.6/spark_llm/cache.py` & `spark_llm-0.1.7/spark_llm/cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,74 @@
 from typing import Optional, Dict
 
-from langchain.cache import RETURN_VAL_TYPE, SQLiteCache
-from langchain.schema import Generation
+from spark_llm.file_cache import JsonCache, SQLiteCacheWrapper
 
 
 class Cache:
     """
     This class provides an interface for a simple in-memory and persistent cache system. It keeps an in-memory staging
     cache, which gets updated through the `update` method and can be persisted through the `commit` method. Cache
-    lookup is always performed on the persistent cache only.
+    lookup is first performed on the in-memory staging cache, and if not found, it is performed on the persistent
+    cache.
 
     Attributes:
         _staging_updates: A dictionary to keep track of the in-memory staging updates.
-        _sqlite_cache: An SQLiteCache instance that acts as the persistent cache.
+        _file_cache: An instance of either JsonCache or SQLiteCacheWrapper that acts as the persistent cache.
     """
 
-    def __init__(self, database_path: str):
+    def __init__(self,
+                 cache_file_location: str = ".spark_llm.json",
+                 file_format: str = "json"):
         """
         Initializes a new instance of the Cache class.
 
         Args:
-            database_path (str, optional): The path to the database file for the SQLiteCache.
-                Defaults to ".spark_llm.db".
-        """
-        self._staging_updates: Dict[(str, str), str] = {}
-        self._sqlite_cache = SQLiteCache(database_path=database_path)
+            cache_file_location (str, optional): The path to the cache file for the JsonCache or SQLiteCacheWrapper.
+                Defaults to ".spark_llm.json".
+            file_format (str, optional): The format of the file to use for the cache. Defaults to "json".
+        """
+        self._staging_updates: Dict[str, str] = {}
+        if file_format == "json":
+            self._file_cache = JsonCache(cache_file_location)
+        else:
+            self._file_cache = SQLiteCacheWrapper(cache_file_location)
 
-    def lookup(self, prompt: str, llm_string: str) -> Optional[str]:
+    def lookup(self, key: str) -> Optional[str]:
         """
-        Performs a lookup in the persistent cache using the given prompt and llm_string.
+        Performs a lookup in the cache using the given key.
 
         Args:
-            prompt (str): The prompt string for the lookup.
-            llm_string (str): The LLM string for the lookup.
+            key (str): The key string for the lookup.
 
         Returns:
-            Optional[str]: The cached text corresponding to the prompt and LLM string, if available. Otherwise, None.
+            Optional[str]: The cached text corresponding to the key, if available. Otherwise, None.
         """
-        lookup_result = self._sqlite_cache.lookup(prompt, llm_string)
-        if lookup_result is not None and len(lookup_result) > 0:
-            return lookup_result[0].text
-        return None
+        # First look in the staging cache
+        staging_result = self._staging_updates.get(key)
+        if staging_result is not None:
+            return staging_result
+        # If not found in staging cache, look in the persistent cache
+        return self._file_cache.lookup(key)
 
-    def update(self, prompt: str, llm_string: str, return_val: str) -> None:
+    def update(self, key: str, val: str) -> None:
         """
-        Updates the staging cache with the given prompt, llm_string, and return value.
+        Updates the staging cache with the given key and value.
 
         Args:
-            prompt (str): The prompt string.
-            llm_string (str): The LLM string.
-            return_val (str): The return value to be cached.
+            key (str): The key string.
+            val (str): The value to be cached.
         """
-        self._staging_updates[(prompt, llm_string)] = return_val
+        self._staging_updates[key] = val
 
     def clear(self) -> None:
         """
         Clears both the in-memory staging cache and the persistent cache.
         """
-        self._sqlite_cache.clear()
-        self._staging_updates: Dict[(str, str), RETURN_VAL_TYPE] = {}
+        self._file_cache.clear()
+        self._staging_updates = {}
 
     def commit(self) -> None:
         """
         Commits all the staged updates to the persistent cache.
         """
-        for key, value in self._staging_updates.items():
-            stored_value = [Generation(text=value)]
-            self._sqlite_cache.update(key[0], key[1], stored_value)
+        self._file_cache.commit_staging_cache(self._staging_updates)
+        self._staging_updates = {}
```

### Comparing `spark_llm-0.1.6/spark_llm/code_logger.py` & `spark_llm-0.1.7/spark_llm/code_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,10 +43,7 @@
             # Add regular text to the message
             colored_message += parts[i]
             # If there is a code block, colorize it and add it to the message
             if i + 2 < len(parts):
                 colored_message += '\n```\n' + self.colorize_code(parts[i + 2], parts[i + 1]) + '```'
         # Log the message with colored code blocks
         self.logger.info(colored_message)
-
-    def log_code(self, code, language):
-        self.logger.info(self.colorize_code(code, language))
```

### Comparing `spark_llm-0.1.6/spark_llm/llm_chain_with_cache.py` & `spark_llm-0.1.7/spark_llm/llm_chain_with_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def run(
         self,
         *args: Any,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> str:
+        assert not args, "The chain expected no arguments"
         prompt_str = self.prompt.format_prompt(**kwargs).to_string()
-        args_str = self._sort_and_stringify(*args)
-        cached_result = self.cache.lookup(prompt_str, args_str)
+        cached_result = self.cache.lookup(prompt_str)
         if cached_result is not None:
             return cached_result
         result = super().run(*args, callbacks=callbacks, tags=tags, **kwargs)
-        self.cache.update(prompt_str, args_str, result)
+        self.cache.update(prompt_str, result)
         return result
```

### Comparing `spark_llm-0.1.6/spark_llm/llm_utils.py` & `spark_llm-0.1.7/spark_llm/llm_utils.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.6/spark_llm/prompt.py` & `spark_llm-0.1.7/spark_llm/prompt.py`

 * *Files identical despite different names*

### Comparing `spark_llm-0.1.6/spark_llm/spark_llm_assistant.py` & `spark_llm-0.1.7/spark_llm/spark_llm_assistant.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
     def __init__(
         self,
         llm: BaseLanguageModel,
         web_search_tool: Optional[Callable[[str], str]] = None,
         spark_session: Optional[SparkSession] = None,
         enable_cache: bool = True,
-        cache_file_location: str = ".spark_llm.db",
+        cache_file_format: str = "json",
+        cache_file_location: str = "spark_llm_cache.json",
         encoding: Optional[Encoding] = None,
         max_tokens_of_web_content: int = 3000,
         verbose: bool = False,
     ) -> None:
         """
         Initialize the SparkLLMAssistant object with the provided parameters.
 
@@ -58,15 +59,15 @@
         :param encoding: optional Encoding, cl100k_base will be used if not provided
         :param max_tokens_of_web_content: maximum tokens of web content after encoding
         """
         self._spark = spark_session or SparkSession.builder.getOrCreate()
         self._llm = llm
         self._web_search_tool = web_search_tool or self._default_web_search_tool
         if enable_cache:
-            self._cache = Cache(database_path = cache_file_location)
+            self._cache = Cache(cache_file_location=cache_file_location, file_format=cache_file_format)
             self._web_search_tool = SearchToolWithCache(
                 self._web_search_tool, self._cache
             ).search
         else:
             self._cache = None
         self._encoding = encoding or tiktoken.get_encoding("cl100k_base")
         self._max_tokens_of_web_content = max_tokens_of_web_content
@@ -150,18 +151,14 @@
             # If there are no code blocks, treat the whole text as a single block of code.
             return [text]
 
     def log(self, message: str) -> None:
         if self._verbose:
             self._logger.log(message)
 
-    def log_code(self, code: str, language: str) -> None:
-        if self._verbose:
-            self._logger.log_code(code, language)
-
     def _trim_text_from_end(self, text: str, max_tokens: int) -> str:
         """
         Trim text from the end based on the maximum number of tokens allowed.
 
         :param text: text to trim
         :param max_tokens: maximum tokens allowed
         :return: trimmed text
@@ -190,16 +187,16 @@
         sql_columns_hint = self._generate_sql_prompt(columns)
 
         # Run the LLM chain to get an ingestion SQL query
         llm_result = self._sql_llm_chain.run(
             query=desc, web_content=web_content, columns=sql_columns_hint
         )
         sql_query = self._extract_code_blocks(llm_result)[0]
-        self.log(f"SQL query for the ingestion:\n")
-        self.log_code(sql_query, "sql")
+        formatted_sql_query=CodeLogger.colorize_code(sql_query, "sql")
+        self.log(f"SQL query for the ingestion:\n{formatted_sql_query}")
 
         view_name = self._extract_view_name(sql_query)
         self.log(f"Storing data into temp view: {view_name}\n")
         self._spark.sql(sql_query)
         return self._spark.table(view_name)
 
     def _get_df_schema(self, df: DataFrame) -> str:
@@ -263,16 +260,16 @@
         temp_view_name = "temp_view_for_transform"
         df.createOrReplaceTempView(temp_view_name)
         schema_str = self._get_df_schema(df)
         llm_result = self._transform_chain.run(
             view_name=temp_view_name, columns=schema_str, desc=desc
         )
         sql_query = self._extract_code_blocks(llm_result)[0]
-        self.log(f"SQL query for the transform:")
-        self.log_code(sql_query, "sql")
+        formatted_sql_query=CodeLogger.colorize_code(sql_query, "sql")
+        self.log(f"SQL query for the transform:\n{formatted_sql_query}")
         return self._spark.sql(sql_query)
 
     def explain_df(self, df: DataFrame) -> str:
         """
         This method generates a natural language explanation of the SQL plan of the input Spark DataFrame.
 
         :param df: The Spark DataFrame to be explained.
@@ -303,17 +300,16 @@
         """
         This method creates and runs test cases for the provided PySpark dataframe transformation function.
 
         :param df: The Spark DataFrame to be verified
         :param desc: A description of the expectation to be verified
         """
         llm_output = self._verify_chain.run(df=df, desc=desc)
-
-        self.log(f"Generated code:")
-        self.log_code(llm_output, "python")
+        formatted_code=CodeLogger.colorize_code(llm_output, "python")
+        self.log(f"Generated code:\n{formatted_code}")
 
         locals_ = {}
         exec(llm_output, {"df": df}, locals_)
 
         self.log(f"\nResult: {locals_['result']}")
 
     def udf(self, func: Callable) -> Callable:
@@ -328,16 +324,16 @@
         code = self._udf_chain.run(
             input_args_types=input_args_types,
             desc=desc,
             return_type=return_type,
             udf_name=udf_name
         )
 
-        self.log(f"Creating following Python UDF:")
-        self.log_code(code, "python")
+        formatted_code=CodeLogger.colorize_code(code, "python")
+        self.log(f"Creating following Python UDF:\n{formatted_code}")
 
         locals_ = {}
         exec(code, globals(), locals_)
 
         return locals_[udf_name]
 
     def activate(self):
```

### Comparing `spark_llm-0.1.6/PKG-INFO` & `spark_llm-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-llm
-Version: 0.1.6
+Version: 0.1.7
 Summary: LLM assistant for the development of Spark applications
 Home-page: https://github.com/gengliangwang/spark-llm
 License: Apache-2.0
 Author: Gengliang Wang
 Author-email: gengliang@apache.org
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

