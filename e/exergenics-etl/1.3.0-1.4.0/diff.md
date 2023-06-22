# Comparing `tmp/exergenics-etl-1.3.0.tar.gz` & `tmp/exergenics-etl-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.3.0.tar", last modified: Fri Jun 16 05:32:10 2023, max compression
+gzip compressed data, was "exergenics-etl-1.4.0.tar", last modified: Thu Jun 22 00:06:35 2023, max compression
```

## Comparing `exergenics-etl-1.3.0.tar` & `exergenics-etl-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53219 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    35383 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-16 05:32:09.000000 exergenics-etl-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.405675 exergenics-etl-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 00:06:35.405675 exergenics-etl-1.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.401674 exergenics-etl-1.4.0/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.401674 exergenics-etl-1.4.0/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.401674 exergenics-etl-1.4.0/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54195 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.405675 exergenics-etl-1.4.0/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39213 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.401674 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:06:35.405675 exergenics-etl-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-22 00:06:33.000000 exergenics-etl-1.4.0/setup.py
```

### Comparing `exergenics-etl-1.3.0/LICENSE` & `exergenics-etl-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.3.0/app/exergenics_etl/__init__.py` & `exergenics-etl-1.4.0/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.3.0/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.4.0/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from exergenics import exergenics
 from urllib.parse import quote_plus
 from sqlalchemy import create_engine
 from Levenshtein import distance as levenshtein_distance
 import regex as re
 import dateparser
 from collections import Counter
-from typing import Tuple
+from typing import Tuple, List
 from functools import reduce
 
 
 from dotenv import load_dotenv
 load_dotenv()
 
 
@@ -563,71 +563,62 @@
                 userMessage = "Cannot find timestamp column."
                 raise EtlError(userMessage)
 
         logger.info(
             'Verifying timestamp column header ... Timestamp header is VALID!')
         return True
 
-    def _check_for_wide_format(self, df: pd.DataFrame) -> bool:
+    def _check_for_wide_format(self, df: pd.DataFrame, timestampColumnNames: List[str]) -> bool:
         """Method check whether input dataframe is in a wide format.
 
         Args:
             df (pd.DataFrame): Pandas DataFrame to apply format checking on. 
+            timestampColumnNames (List[str]): Column names of all timestamp columns in the dataframe.
 
         Raises:
             EtlError: If the input dataframe is in a long format. 
             The exception is raised with three arguments: the error message, 
             the names and the values column IDs of the long dataframe.
 
         Returns:
             bool: True if input is in a wide format.
         """
 
+        # Find timestamp column id(s)
+        timestampColumnIds = [list(df.columns).index(n) for n in timestampColumnNames]
+
         # If there are only 3 columns in this data file
         if df.shape[1] == N_COLUMN_LONG_DATA:
 
-            # Check if the 2nd or 3rd column is a variable name column
-
-            # Check the 2nd column
-            namesColumnId = 1  # The column ID of the names column (0-based indexing)
-            valuesColumnId = 2  # The column ID of the values column (0-based indexing)
-
-            # If none of the values in the 2nd column can be converted to float
-            secondColumnName = df.columns[namesColumnId]
-            secondColumn = df[secondColumnName]
-            if not any(secondColumn.apply(convertable_to_float)):
-
-                # If the average length of the strings in the 2nd column is longer than 10
-                if secondColumn.apply(lambda x: len(x)).mean() > LENGTH_THRESHOLD:
-                    
-                    # Raise error when a long format dataset is detected
-                    errorMessage = 'This data file looks like in a long format. ' \
-                        + f'The 2nd column (\"{secondColumnName}\") is likely a variable name column. ' \
-                        + 'However, we currently only accept datasets in a wide format.'
-                    logger.error(errorMessage)
-                    raise EtlError(errorMessage, namesColumnId, valuesColumnId)
+            # Not a long dataframe if there is less than one column after ignoring timestamp columns
+            if (N_COLUMN_LONG_DATA - len(timestampColumnNames) <= 1):
+                return True
+
+            # Loop through all columns except timestamps to find the names column
+            for namesColumnId in range(N_COLUMN_LONG_DATA):
+
+                # Ignore timestamp columns
+                if df.columns[namesColumnId] in timestampColumnNames:
+                    continue
                 
-            # Check the 3rd column
-            namesColumnId = 2  # The column ID of the names column (0-based indexing)
-            valuesColumnId = 1  # The column ID of the values column (0-based indexing)
-
-            # If none of the values in the 3rd column can be converted to float
-            thirdColumnName = df.columns[namesColumnId]
-            thirdColumn = df[thirdColumnName]
-            if not any(thirdColumn.apply(convertable_to_float)):
-
-                # If the average length of the strings in the 3rd column is longer than 10
-                if thirdColumn.apply(lambda x: len(x)).mean() > LENGTH_THRESHOLD:
-
-                    # Raise error when a long format dataset is detected
-                    errorMessage = 'This data file looks like in a long format. ' \
-                        + f'The 3rd column (\"{thirdColumnName}\") is likely a variable name column. ' \
-                        + 'However, we currently only accept datasets in a wide format.'
-                    logger.error(errorMessage)
-                    raise EtlError(errorMessage, namesColumnId, valuesColumnId)
+                valuesColumnId = list(set(range(N_COLUMN_LONG_DATA)) - set(timestampColumnIds) - {namesColumnId})[0]
+
+                # If none of the values in the current column can be converted to float
+                nameColumnName = df.columns[namesColumnId]
+                nameColumn = df[nameColumnName]
+                if not any(nameColumn.apply(convertable_to_float)):
+
+                    # If the average length of the strings in the current column is longer than 10
+                    if nameColumn.apply(lambda x: len(x)).mean() > LENGTH_THRESHOLD:
+                        
+                        # Raise error when a long format dataset is detected
+                        errorMessage = 'The table in this file is in a long format. ' \
+                            + f'This column (column name = \"{nameColumnName}\") is detected to be a variable name column. '
+                        logger.error(errorMessage)
+                        raise EtlError(errorMessage, namesColumnId, valuesColumnId)
 
         return True
 
     def check_input_dataframe(self, df: pd.DataFrame) -> bool:
         """Validate the format of a dataframe read from a data file.
 
         Args:
@@ -734,14 +725,53 @@
 
     else:
         dtSeriesSorted = dtSeries.sort_values(
             ascending=True, ignore_index=True)
         return str(int(dtSeriesSorted.diff().mode()[0].total_seconds()/60))
 
 
+def find_timestamp_columns(df:pd.DataFrame) -> List[str]:
+    """
+    Finds the columns in a pandas DataFrame that represent timestamps.
+
+    The function iterates over the values in the first row of the DataFrame and attempts to
+    convert each value to a timestamp using the `pd.to_datetime` function. Any value that can
+    be successfully converted to a timestamp is considered a timestamp column.
+
+    Args:
+        df (pd.DataFrame): The DataFrame to search for the timestamp column.
+
+    Returns:
+        List[str]: A list of column names representing the detected timestamp columns.
+    
+    Raises:
+        EtlError: If no timestamp column is found in the DataFrame.
+    """
+
+    logger = Logger()
+
+    firstRow = df.iloc[0].astype(str)
+    timestampColumnNames = []
+    for index, possibleTimestamp in firstRow.items():
+        try:
+            pd.to_datetime(possibleTimestamp)
+            timestampColumnNames.append(index)
+            logger.info(f'This is a timestamp column. Column name = "{index}". Tested value = {possibleTimestamp}')
+        except:
+            logger.info(f'This is not a timestamp column. Column name = "{index}". Tested value = {possibleTimestamp}')
+
+    if timestampColumnNames:
+        return timestampColumnNames
+
+    else:
+        errorMessage = "Cannot find any timestamp column."
+        logger.error(errorMessage)
+        raise EtlError(errorMessage)
+
+
 class DatetimeParser():
     """A class to parse a Panda Series of timestamp strings. 
     """
 
     def __init__(self, nTests=100):
         """Constructs all the necessary attributes for the DatetimeParser object.
 
@@ -1159,36 +1189,39 @@
         # RETURN a pd.Series of datetime objects
         self.logger.info(
             f'Showing the first and the last 2 of the timestamps AFTER parsing: \n{pd.concat([dtObjects.head(2), dtObjects.tail(2)])}')
 
         return dtObjects
 
 
-def transform_columns_to_long_dataframes(wideDf: pd.DataFrame, filesWithNanColumn: set, fileName: str) -> Tuple[dict, set]:
+def transform_columns_to_long_dataframes(wideDf: pd.DataFrame, filesWithNanColumn: set, fileName: str, timestampColumnName: str) -> Tuple[dict, set]:
     """Transform each column in the input dataframe to a new dataframe in long format.
 
     Args:
         wideDf (pd.DataFrame): Pandas Dataframe of a dataset with wide format.
         filesWithNanColumn (set): Set of files with NaN column.
         fileName (str): Absolute file path of dataset to be processed.
+        timestampColumnName (str): Column name of timestamp column.
 
     Raises:
-            EtlError: If duplicate column headers are found in a single data file and for unknown errors.
+        EtlError: If duplicate column headers are found in a single data file and for unknown errors.
 
     Returns:
         Tuple[dict, set]: Dictionary of the new dataframe(s) and a set of files with NaN column.
     """
     
     logger = Logger()
 
     try:
         dfDictFile = {}
 
-        # Loop through all columns (point values) except the first column (where the timestamps should be)
-        for point in wideDf.columns[1:]:
+        # Loop through all columns (point values) except the timestamp column
+        for point in wideDf.columns:
+            if point == timestampColumnName:
+                continue
 
             # Get all non-na values for selected column as temp dataframe
             tempDf = wideDf[wideDf[point].notna()][[TIME, point]].rename(
                 columns={point: VALUE})
 
             # Log the file name if the whole column is NaN
             if not wideDf[point].notna().any():
```

### Comparing `exergenics-etl-1.3.0/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.4.0/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.3.0/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.4.0/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.3.0/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.4.0/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,40 +240,62 @@
     def test_convertable_to_float(self, string, expected):
         assert convertable_to_float(string) == expected
 
 
 class TestInputValidationClass:
 
     @pytest.fixture(scope='class')
-    def my_wide_format_dataframe(self):
-        filePath = 'app/exergenics_etl/test/testData/wideData.csv'
+    def my_check_for_wide_format_test_case_wide1(self):
+        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/wideData1.csv'
         df = pd.read_csv(filePath)
-        return df
-
+        timestampColumnNames = ['ui::timestamp']
+        return df, timestampColumnNames
+    
+    @pytest.fixture(scope='class')
+    def my_check_for_wide_format_test_case_wide2(self):
+        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/wideData2.csv'
+        df = pd.read_csv(filePath)
+        timestampColumnNames = ['Created time', 'Modified time']
+        return df, timestampColumnNames
+    
     @pytest.fixture(scope='class')
     def my_check_for_wide_format_test_case_long1(self):
         """Second test case for the _check_for_wide_format method where the 
-        input is a long dataframe, and the names column is in the 2rd 
+        input is a long dataframe, and the names column is in the 1st 
         column."""
-        filePath = 'app/exergenics_etl/test/testData/longData_nameColumnIn2ndColumn.csv'
+        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/longData_nameColumnIn1stColumn.csv'
+        df = pd.read_csv(filePath)
+        namesColumnId = 0
+        valuesColumnId = 1
+        timestampColumnNames = ['ui::timestamp']
+        return df, timestampColumnNames, namesColumnId, valuesColumnId
+
+    @pytest.fixture(scope='class')
+    def my_check_for_wide_format_test_case_long2(self):
+        """Second test case for the _check_for_wide_format method where the 
+        input is a long dataframe, and the names column is in the 2nd 
+        column."""
+        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/longData_nameColumnIn2ndColumn.csv'
         df = pd.read_csv(filePath)
         namesColumnId = 1
         valuesColumnId = 2
-        return df, namesColumnId, valuesColumnId
+        timestampColumnNames = ['ui::timestamp']
+        return df, timestampColumnNames, namesColumnId, valuesColumnId
     
     @pytest.fixture(scope='class')
-    def my_check_for_wide_format_test_case_long2(self):
+    def my_check_for_wide_format_test_case_long3(self):
         """Second test case for the _check_for_wide_format method where the 
         input is a long dataframe, and the names column is in the 3rd 
         column."""
-        filePath = 'app/exergenics_etl/test/testData/longData_nameColumnIn3rdColumn.csv'
+        filePath = 'app/exergenics_etl/test/testData/testData_check_for_wide_format/longData_nameColumnIn3rdColumn.csv'
         df = pd.read_csv(filePath)
         namesColumnId = 2
         valuesColumnId = 1
-        return df, namesColumnId, valuesColumnId
+        timestampColumnNames = ['ui::timestamp']
+        return df, timestampColumnNames, namesColumnId, valuesColumnId
 
     @pytest.fixture(scope='class')
     def my_valid_timestamp_headers(self):
         return ['datetime', 'timestamp', 'event', 'timepretty', 'ts']
 
     @pytest.fixture(scope='class')
     def my_generic_column_headers(self):
@@ -282,26 +304,28 @@
     @pytest.fixture(scope='class')
     def my_inputValidation_object(self, my_valid_timestamp_headers, my_generic_column_headers):
         """Instantiate an InputValidation object for testing."""
         inputValidation = InputValidation(
             my_valid_timestamp_headers, my_generic_column_headers)
         return inputValidation
 
-    def test_check_for_wide_format(self, my_inputValidation_object, my_wide_format_dataframe):
+    @pytest.mark.parametrize("my_test_case", ['my_check_for_wide_format_test_case_wide1', 'my_check_for_wide_format_test_case_wide2'])
+    def test_check_for_wide_format_on_wide_dataframe(self, my_inputValidation_object, my_test_case, request):
         """Check for wide format when a wide format dataframe is passed."""
+        testDf, myTimestampColumnNames = request.getfixturevalue(my_test_case)
         assert my_inputValidation_object._check_for_wide_format(
-            my_wide_format_dataframe)
+            testDf, myTimestampColumnNames)
 
-    @pytest.mark.parametrize("my_test_case", ['my_check_for_wide_format_test_case_long1', 'my_check_for_wide_format_test_case_long2'])
+    @pytest.mark.parametrize("my_test_case", ['my_check_for_wide_format_test_case_long1', 'my_check_for_wide_format_test_case_long2', 'my_check_for_wide_format_test_case_long3'])
     def test_check_for_wide_format_on_long_dataframe(self, my_inputValidation_object, my_test_case, request):
         """Check for wide format when a long format dataframe is passed."""
-        myLongDf, expectedNamesColumnId, expectedValuesColumnId = request.getfixturevalue(my_test_case)
+        testLongDf, myTimestampColumnNames, expectedNamesColumnId, expectedValuesColumnId = request.getfixturevalue(my_test_case)
         with pytest.raises(EtlError) as errInfo:
             my_inputValidation_object._check_for_wide_format(
-                myLongDf)
+                testLongDf, myTimestampColumnNames)
 
         assert errInfo.value.args[1] == expectedNamesColumnId
         assert errInfo.value.args[2] == expectedValuesColumnId
 
     def test_check_for_generic_header1(self, my_inputValidation_object):
         myDfSameName = pd.read_csv(
             'app/exergenics_etl/test/testData/dfSameName.csv', parse_dates=['timepretty'])
@@ -378,14 +402,68 @@
     def test_calculate_time_interval(self, my_calculate_time_interval_test_case, request):
         myTestDtSeries, expectedTimeInterval = request.getfixturevalue(
             my_calculate_time_interval_test_case)
 
         assert calculate_time_interval(myTestDtSeries) == expectedTimeInterval
 
 
+class TestFindTimestampColumn:
+
+    @pytest.fixture(scope='class')
+    def my_test_dataframe1(self):
+        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/two timestamp columns.csv"
+        df = pd.read_csv(filePath)
+        return df
+
+    @pytest.fixture(scope='class')
+    def my_test_dataframe2(self):
+        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/timestamps in second column.csv"
+        df = pd.read_csv(filePath)
+        return df
+
+    @pytest.fixture(scope='class')
+    def my_test_dataframe3(self):
+        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/timestamps in second column (unix timestamps in first column).csv"
+        df = pd.read_csv(filePath)
+        return df
+
+    @pytest.fixture(scope='class')
+    def my_test_dataframe4(self):
+        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/timestamps in third column.csv"
+        df = pd.read_csv(filePath)
+        return df
+
+    @pytest.fixture(scope='class')
+    def my_test_dataframe5(self):
+        filePath = "app/exergenics_etl/test/testData/testData_for_find_timestamp_column/no timestamp column.csv"
+        df = pd.read_csv(filePath)
+        return df
+    
+    @pytest.fixture(scope='class')
+    def my_expected_timestamp_column_names(self):
+        return ['Target column1', 'Target column2']
+
+    @pytest.fixture(scope='class')
+    def my_expected_timestamp_column_name(self):
+        return ['Target column']
+    
+    def test_find_two_timestamp_columns(self, my_test_dataframe1, my_expected_timestamp_column_names):
+        assert find_timestamp_columns(my_test_dataframe1) == my_expected_timestamp_column_names
+    
+    @pytest.mark.parametrize("testDf", ["my_test_dataframe2", "my_test_dataframe3", "my_test_dataframe4"])
+    def test_find_timestamp_column(self, testDf, my_expected_timestamp_column_name, request):
+        testDf = request.getfixturevalue(testDf)
+
+        assert find_timestamp_columns(testDf) == my_expected_timestamp_column_name
+
+    def test_timestamp_column_not_found(self, my_test_dataframe5):
+        with pytest.raises(EtlError):
+            find_timestamp_columns(my_test_dataframe5)
+
+
 class TestDatetimeParserClass:
 
     @pytest.fixture(scope='function')
     def my_datetimeParser(self):
         datetimeParser = DatetimeParser()
         return datetimeParser
 
@@ -605,15 +683,15 @@
                                               'datapoint': [0, 0, 1]}),
                                 'Cooling Tower Fan Power':
                                     pd.DataFrame({'timepretty': [Timestamp('2023-05-19 15:08:00'), Timestamp('2023-05-19 15:10:00')],
                                                   'observation': ['Cooling Tower Fan Power', 'Cooling Tower Fan Power'],
                                                   'datapoint': [0.0, 3.0]})}
 
         dfDict, newFilesWithNanColumn = transform_columns_to_long_dataframes(
-            myTestWideDataframe, myTestFilesWithNanColumn, myTestFileName)
+            myTestWideDataframe, myTestFilesWithNanColumn, myTestFileName, 'timepretty')
 
         assert dfDict.keys() == expectedDfDictOutput.keys()
 
         # Compare DataFrames for each key
         for key in dfDict.keys():
             df1 = dfDict[key]
             df2 = expectedDfDictOutput[key]
```

### Comparing `exergenics-etl-1.3.0/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.4.0/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.3.0/setup.py` & `exergenics-etl-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.3.0",
+    version="v1.4.0",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

