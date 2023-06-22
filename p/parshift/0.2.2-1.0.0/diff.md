# Comparing `tmp/parshift-0.2.2.tar.gz` & `tmp/parshift-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parshift-0.2.2.tar", last modified: Fri May 12 08:46:02 2023, max compression
+gzip compressed data, was "parshift-1.0.0.tar", last modified: Thu Jun 22 12:00:05 2023, max compression
```

## Comparing `parshift-0.2.2.tar` & `parshift-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:46:02.804889 parshift-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-12 08:45:55.000000 parshift-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-12 08:46:02.804889 parshift-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-12 08:45:55.000000 parshift-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:46:02.804889 parshift-0.2.2/parshift/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/oo_parshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-12 08:45:55.000000 parshift-0.2.2/parshift/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:46:02.804889 parshift-0.2.2/parshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 08:46:02.000000 parshift-0.2.2/parshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-12 08:45:55.000000 parshift-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:46:02.804889 parshift-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:46:02.804889 parshift-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-12 08:45:55.000000 parshift-0.2.2/tests/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-12 08:45:55.000000 parshift-0.2.2/tests/test_oo_parshift.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-12 08:45:55.000000 parshift-0.2.2/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-12 08:45:55.000000 parshift-0.2.2/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:00:05.098515 parshift-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-22 11:59:57.000000 parshift-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-22 12:00:05.098515 parshift-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-22 11:59:57.000000 parshift-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:00:05.098515 parshift-1.0.0/parshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-22 11:59:57.000000 parshift-1.0.0/parshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-22 11:59:57.000000 parshift-1.0.0/parshift/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-22 11:59:57.000000 parshift-1.0.0/parshift/oo_parshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-22 11:59:57.000000 parshift-1.0.0/parshift/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-22 11:59:57.000000 parshift-1.0.0/parshift/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:00:05.098515 parshift-1.0.0/parshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-22 12:00:05.000000 parshift-1.0.0/parshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-22 12:00:05.000000 parshift-1.0.0/parshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:00:05.000000 parshift-1.0.0/parshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-22 12:00:05.000000 parshift-1.0.0/parshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 12:00:05.000000 parshift-1.0.0/parshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-22 11:59:57.000000 parshift-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 12:00:05.098515 parshift-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:00:05.098515 parshift-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-22 11:59:57.000000 parshift-1.0.0/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-22 11:59:57.000000 parshift-1.0.0/tests/test_oo_parshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-22 11:59:57.000000 parshift-1.0.0/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-22 11:59:57.000000 parshift-1.0.0/tests/test_statistics.py
```

### Comparing `parshift-0.2.2/LICENSE` & `parshift-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parshift-0.2.2/PKG-INFO` & `parshift-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parshift
-Version: 0.2.2
+Version: 1.0.0
 Summary: Python package based on Gibson's framework (2003) for turn-taking in group conversation analysis.
 Author-email: Bruno Saraiva <bruno.saraiva@ulusofona.pt>, João Pedro Carvalho <joao.matos.carvalho@ulusofona.pt>, Nuno Fachada <nuno.fachada@ulusofona.pt>, Manuel Pita <manuel.pita@ulusofona.pt>
 License: MIT
 Project-URL: Homepage, https://github.com/bdfsaraiva/parshift
 Project-URL: Bug Tracker, https://github.com/bdfsaraiva/parshift/issues
 Project-URL: Documentation, https://bdfsaraiva.github.io/parshift/
 Keywords: python,conversation-analysis,participation-shifts,turn-taking
@@ -92,9 +92,9 @@
 
 ## License
 
 [MIT License](LICENSE)
 
 [Gibson's framework]:https://doi.org/10.1353/sof.2003.0055
 [docs]:https://bdfsaraiva.github.io/parshift/
-[example1]:https://colab.research.google.com/drive/1gYa32dMQDVuKwHDLgl1wJiVyHwUw4_zL?usp=sharing
+[example1]:https://colab.research.google.com/drive/1zjstEdkIZrCSgZFkilNf8kvTkRCS-bYG?usp=sharing
 [issue]:https://github.com/bdfsaraiva/parshift/issues/new/choose
```

### Comparing `parshift-0.2.2/README.md` & `parshift-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -72,9 +72,9 @@
 
 ## License
 
 [MIT License](LICENSE)
 
 [Gibson's framework]:https://doi.org/10.1353/sof.2003.0055
 [docs]:https://bdfsaraiva.github.io/parshift/
-[example1]:https://colab.research.google.com/drive/1gYa32dMQDVuKwHDLgl1wJiVyHwUw4_zL?usp=sharing
+[example1]:https://colab.research.google.com/drive/1zjstEdkIZrCSgZFkilNf8kvTkRCS-bYG?usp=sharing
 [issue]:https://github.com/bdfsaraiva/parshift/issues/new/choose
```

### Comparing `parshift-0.2.2/parshift/__init__.py` & `parshift-1.0.0/parshift/__init__.py`

 * *Files identical despite different names*

### Comparing `parshift-0.2.2/parshift/annotation.py` & `parshift-1.0.0/parshift/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 }
 
 
 def read_ccsv(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     **kwargs: Any,
 ) -> pd.DataFrame:
-    """Read a conversation file in CSV format, validate it and return a dataframe.
+    """Read a conversation file in CSV format, validate it and return a data frame.
 
     The conversation file should have the following columns:
 
     - `utterance_id`: ID of the message (int)
     - `speaker_id`: ID of the user sending the message (str)
     - `utterance`: The message itself (string)
     - `reply_to_id` or `target_id`: The reply ID or the target ID (int)
@@ -86,15 +86,15 @@
     else:
         conversation["target_id"] = conversation["target_id"].fillna("")
 
     return conversation
 
 
 def conv2turns(conv_df: pd.DataFrame) -> List[Dict[str, Any]]:
-    """Take a conversation dataframe and group it into conversation turns.
+    """Take a conversation data frame and group it into conversation turns.
 
     A turn is a group of messages sent by the same user and addressed to the
     same target.
 
     Arguments:
         conv_df: The conversation from where to obtain the conversation turns.
 
@@ -110,18 +110,23 @@
 
     conversation: List[Dict[str, Any]] = []
     turn = 0
 
     for index, row in conv_df.iterrows():
         # If the row being looped has the same "speaker_id" and the "last_col" value,
         # then merge the message text and message utterance_ids into the previous turn.
+
+        if row[last_col] == "" or row[last_col] == "None":
+            row[last_col] = None
+        row[last_col] = int(float(row[last_col])) if row[last_col] != None else None
+
         if (
             index != 0
             and conversation[turn - 1]["speaker_id"] == row["speaker_id"]
-            and str(conversation[turn - 1][last_col]) == row[last_col]
+            and conversation[turn - 1][last_col] == row[last_col]
         ):
             msg_join = ". ".join(
                 [conversation[turn - 1]["utterance"], row["utterance"]]
             )
             list_id = conversation[turn - 1]["utterance_ids"] + [row["utterance_id"]]
             conversation[turn - 1]["utterance_ids"] = list_id
             conversation[turn - 1]["utterance"] = msg_join
@@ -134,15 +139,15 @@
             last_col_val = row[last_col]
 
             conversation.append(
                 {
                     "utterance_ids": [id],
                     "speaker_id": speaker_id,
                     "utterance": utterance,
-                    last_col: int(last_col_val)
+                    last_col: last_col_val
                     if last_col_val != ""
                     and last_col_val != None
                     and last_col_val != "None"
                     else None,
                 }
             )
 
@@ -195,15 +200,15 @@
     be in the same turn, and therefore will be assigned a single participation
     shift code.
 
     Arguments:
         conv_df: The conversation from where to obtain the participation shift codes.
 
     Returns:
-        A dataframe with the participation shift codes for each turn.
+        A data frame with the participation shift codes for each turn.
     """
 
     if not isinstance(conv_df, pd.DataFrame):
         raise TypeError("Parameter conv_df must be a Pandas DataFrame")
 
     conversation = conv2turns(conv_df)
```

### Comparing `parshift-0.2.2/parshift/oo_parshift.py` & `parshift-1.0.0/parshift/oo_parshift.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 import pandas as pd
 from pandas._typing import FilePath, ReadCsvBuffer
 
 from .annotation import annotate, read_ccsv
 from .plotting import frequency_treemap
 from .statistics import cond_probs, propensities
 
-# from parshift.annotation import read_ccsv, annotate
-# from parshift.statistics import cond_probs
-# from parshift.plotting import frequency_treemap
-
 
 class Parshift:
     def __init__(
         self,
         annotation: pd.DataFrame | None = None,
         stats: pd.DataFrame | List[pd.DataFrame] | None = None,
     ):
@@ -52,16 +48,16 @@
             filepath_or_buffer: Any valid string path to CSV file, as accepted by
                 Pandas [`read_csv()`][pandas.read_csv] function.
             N: Number of parts to split the conversation into. Default is 1 (all conversation).
                 `N` should be between 1 and 4.
             **kwargs: Keyword parameters passed to Pandas
                 [`read_csv()`][pandas.read_csv] function.
 
-        - Parshift.annotation will be dataframe equal as returned by [`annotate()`][parshift.annotation.annotate].
-        - Parshift.stats will be dataframe equal as returned by [`cond_probs()`][parshift.statistics.cond_probs].
+        - Parshift.annotation will be data frame equal as returned by [`annotate()`][parshift.annotation.annotate].
+        - Parshift.stats will be data frame equal as returned by [`cond_probs()`][parshift.statistics.cond_probs].
         """
 
         df_annotate = annotate(read_ccsv(filepath_or_buffer, **kwargs))
         self.annotation = df_annotate
 
         if N == 1:
             self.stats = cond_probs(df_annotate)
@@ -74,15 +70,15 @@
                 start = int(parts * i)
                 end = int(parts * (i + 1))
                 list_stats.append(cond_probs(df_annotate.iloc[start:end, :]))
             self.stats = list_stats
         else:
             raise ValueError("N should be between 1 and 4.")
 
-    def get_plot(self, type: str = "Pshift", filename: str | None = None):
+    def show_plot(self, type: str = "Pshift", filename: str | None = None):
         """Shows the frequency treemap plot returned by [`frequency_treemap()`][parshift.plotting.frequency_treemap]
 
         Arguments:
             type: Column name to be used to plot the treemap, either `"Pshift"`
                 (default) or `"Pshift_class"`.
             filename: Name of the file to save the plot. Default to `None` .
 
@@ -108,106 +104,106 @@
                 _, ax = plt.subplots(
                     1, len(self.stats), figsize=(5 * len(self.stats), 5)
                 )
 
                 for i in range(len(self.stats)):
                     frequency_treemap(self.stats[i], type=type, ax=ax[i])
                     ax[i].axis("off")
-                    ax[i].set_title(f"N {i+1}")
+                    ax[i].set_title(f"n {i+1}")
             else:
                 ax = frequency_treemap(self.stats, type=type)
 
             plt.suptitle("Participation-Shift Frequencies")
 
         elif type == "Pshift_class":
             if isinstance(self.stats, list):
                 _, ax = plt.subplots(
                     1, len(self.stats), figsize=(5 * len(self.stats), 5)
                 )
 
                 for i in range(len(self.stats)):
                     frequency_treemap(self.stats[i], type=type, ax=ax[i])
                     ax[i].axis("off")
-                    ax[i].set_title(f"N {i+1}")
+                    ax[i].set_title(f"n {i+1}")
             else:
                 ax = frequency_treemap(self.stats, type=type)
 
             plt.suptitle("Participation Shifts: Class Proportions")
 
         if filename:
             if ".png" not in filename:
                 filename += ".png"
             plt.savefig(filename, dpi=300)
 
         plt.show()
 
-    def get_stats(self, filename: str | None = None):
+    def show_stats(self, filename: str | None = None):
         """Prints the stats returned by [`cond_probs()`][parshift.statistics.cond_probs]
-        Dataframe. If N > 1, prints N dataframes.
+        Dataframe. If kwarg N (see [`process`][parshift.Parshift.process]) > 1, prints N data frames.
 
         Arguments:
-            filename: Name of the file (csv) to save the stats dataframe. Default to `None`.
+            filename: Name of the file (csv) to save the stats data frame. Default to `None`.
         """
 
         if self.stats is None:
             raise ValueError(
                 "Parshift.stats is None. Please run Parshift.process() first."
             )
 
         if isinstance(self.stats, list):
             for i in range(len(self.stats)):
-                print(f"N{i+1}:")
+                print(f"n{i+1}:")
                 print(self.stats[i])
                 print("-" * 80)
 
                 if filename:
                     if ".csv" not in filename:
-                        filename_changed = f"{filename}_N{i+1}.csv"
+                        filename_changed = f"{filename}_n{i+1}.csv"
                     else:
-                        filename_changed = filename.replace(".csv", f"_N{i+1}.csv")
+                        filename_changed = filename.replace(".csv", f"_n{i+1}.csv")
                     self.stats[i].to_csv(filename_changed, index=False)
 
         else:
             print(self.stats)
             if filename:
                 if ".csv" not in filename:
                     filename += ".csv"
                 self.stats.to_csv(filename, index=False)
 
     def get_propensities(self, filename: str | None = None) -> pd.DataFrame:
-        """Returns a dataframe with the Participation Shift propensities.
+        """Returns a data frame with the Participation Shift propensities.
 
         Arguments:
-            filename: Name of the file (csv) to save the propensities dataframe. Default to `None`.
+            filename: Name of the file (csv) to save the propensities data frame. Default to `None`.
 
         Returns:
             A Pandas [`DataFrame`][pandas.DataFrame] containing the propensities.
         """
 
         if self.stats is None:
             raise ValueError(
                 "Parshift.stats is None. Please run Parshift.process() first."
             )
 
         if isinstance(self.stats, list):
             df = propensities(self.stats[0])
-            df.index = ["N1"]  # type: ignore
+            df.index = ["n1"]  # type: ignore
             for i in range(1, len(self.stats)):
                 dfx = propensities(self.stats[i])
-                dfx.index = [f"N{i+1}"]  # type: ignore
+                dfx.index = [f"n{i+1}"]  # type: ignore
                 df = pd.concat([df, dfx])
 
             if filename:
                 if ".csv" not in filename:
                     filename += ".csv"
                 df.to_csv(filename, index=False)
             return df
 
         else:
             df = propensities(self.stats)
-            df.index = ["N"]  # type: ignore
+            df.index = ["n"]  # type: ignore
 
             if filename:
                 if ".csv" not in filename:
                     filename += ".csv"
                 df.to_csv(filename, index=False)
             return df
```

### Comparing `parshift-0.2.2/parshift/plotting.py` & `parshift-1.0.0/parshift/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ax: matplotlib.axes.Axes = None,
     type: str = "Pshift",
 ) -> matplotlib.axes.Axes:
     """Get a matplotlib axes object displaying the conditional probabilities or frequencies.
 
     Arguments:
         cond_probs_df: Dataframe with information about the participation shift
-            conditional probabilities. This dataframe can be obtained with
+            conditional probabilities. This data frame can be obtained with
             [`cond_probs()`][parshift.statistics.cond_probs]
         type: Column name to be used to plot the treemap, either `"Pshift"`
             (default) or `"Pshift_class"`.
         ax: Matplotlib axes with the treemap plot.
 
     Returns:
         ax: Matplotlib axes with the participation shifts probabilities or frequency.
```

### Comparing `parshift-0.2.2/parshift/statistics.py` & `parshift-1.0.0/parshift/statistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,18 @@
         "AB-AY": True,
     }
     return _targeted_remark_dic[ps]
 
 
 def _frequency_table(parshift_annotation_df) -> list:
     """
-    This function takes in a dataframe of ParShift annotations and returns a frequency table of ParShift codes.
+    This function takes in a data frame of ParShift annotations and returns a frequency table of ParShift codes.
 
     Arguments:
-        parshift_annotation_df: A Pandas dataframe containing ParShift annotations
+        parshift_annotation_df: A Pandas data frame containing ParShift annotations
 
     Returns:
         A list containing a dictionary of ParShift codes and their frequencies,
         the total number of times a ParShift code starting with "A0" appears,
         the total number of times a Parshift code starting with "AB" appears,
         the total number of times a Parshift code with "A0" assuming change of speaker,
         and the total number of times a ParShift code with "AB" appears assuming
@@ -127,20 +127,20 @@
     """Determine the conditional probabilities for a sequence of participation shift codes.
 
     Arguments:
         pshift_codes: A sequence of participation shift code obtained with
             [`annotate()`][parshift.annotation.annotate].
 
     Returns:
-        A dataframe containing the frequency, probability and conditional probabilities
-            (two) for each parshift code. This dataframe is divided into two 'subgroups':
+        A data frame containing the frequency, probability and conditional probabilities
+            (two) for each parshift code. This data frame is divided into two 'subgroups':
             (1) those beginning with an undirected remark (A0-); and, (2) those beginning
             with a directed one (AB-). The `P(S|D)` (Probability of a participation shift
             given a Directed or Undirected remark (D)) column contains the frequency divided
-            by total occurrences in each subgroup, while the `P(S|D and C)` (Probability of
+            by total occurrences in each subgroup, while the `P(S|D,C)` (Probability of
             a participation shift given a Directed or Undirected remark (D) and assuming
             Change of Speaker (C)) column contains the frequency divided by total occurrences
             in each subgroup, for each participation shift where the change of speaker occurs.
     """
 
     if not isinstance(pshift_codes, pd.DataFrame):
         raise TypeError("Parameter parshift_annotation_df must be a Dataframe")
@@ -206,40 +206,40 @@
     )
 
     result["Directed Remark (D)"] = result["pshift"].apply(
         lambda ps: _targeted_remark(ps)
     )
 
     result.rename(
-        columns={"pshift": "Pshift", "CP": "P(S|D)", "CPeTC": "P(S|D and C)"},
+        columns={"pshift": "Pshift", "CP": "P(S|D)", "CPeTC": "P(S|D,C)"},
         inplace=True,
     )
 
     return result
 
 
 def propensities(cond_probs_df: pd.DataFrame) -> pd.DataFrame:
-    """Determine the propensities from a conditional probabilities dataframe.
+    """Determine the propensities from a conditional probabilities data frame.
 
     Arguments:
-        cond_probs_df: A dataframe with statistics obtained with
+        cond_probs_df: A data frame with statistics obtained with
             [`cond_probs()`][parshift.statistics.cond_probs].
 
     Returns:
-        A dataframe containing the propensities proposed by Gibson.
+        A data frame containing the propensities proposed by Gibson.
     """
 
     dic_propensities = {}
 
     # turn-receiving propensity -> AB-BA, AB-BO, and AB-BY ( P(S|D) )
     p_s_d = cond_probs_df["P(S|D)"]
-    p_s_d_c = cond_probs_df["P(S|D and C)"]
+    p_s_d_c = cond_probs_df["P(S|D,C)"]
 
     dic_propensities["turn-receiving"] = p_s_d[4] + p_s_d[5] + p_s_d[10]
 
-    # targeting propensity -> AO-XY, AB-BY and AB-XY ( P(S|D and C) )
+    # targeting propensity -> AO-XY, AB-BY and AB-XY ( P(S|D,C) )
     dic_propensities["targeting"] = p_s_d_c[2] + p_s_d_c[10] + p_s_d_c[11]
 
     # termination propensity -> AO-AY, AB-AO and AB-AY ( P(S|D) )
     dic_propensities["termination"] = p_s_d[2] + p_s_d[9] + p_s_d[12]
 
     return pd.DataFrame([dic_propensities])
```

### Comparing `parshift-0.2.2/parshift.egg-info/PKG-INFO` & `parshift-1.0.0/parshift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parshift
-Version: 0.2.2
+Version: 1.0.0
 Summary: Python package based on Gibson's framework (2003) for turn-taking in group conversation analysis.
 Author-email: Bruno Saraiva <bruno.saraiva@ulusofona.pt>, João Pedro Carvalho <joao.matos.carvalho@ulusofona.pt>, Nuno Fachada <nuno.fachada@ulusofona.pt>, Manuel Pita <manuel.pita@ulusofona.pt>
 License: MIT
 Project-URL: Homepage, https://github.com/bdfsaraiva/parshift
 Project-URL: Bug Tracker, https://github.com/bdfsaraiva/parshift/issues
 Project-URL: Documentation, https://bdfsaraiva.github.io/parshift/
 Keywords: python,conversation-analysis,participation-shifts,turn-taking
@@ -92,9 +92,9 @@
 
 ## License
 
 [MIT License](LICENSE)
 
 [Gibson's framework]:https://doi.org/10.1353/sof.2003.0055
 [docs]:https://bdfsaraiva.github.io/parshift/
-[example1]:https://colab.research.google.com/drive/1gYa32dMQDVuKwHDLgl1wJiVyHwUw4_zL?usp=sharing
+[example1]:https://colab.research.google.com/drive/1zjstEdkIZrCSgZFkilNf8kvTkRCS-bYG?usp=sharing
 [issue]:https://github.com/bdfsaraiva/parshift/issues/new/choose
```

### Comparing `parshift-0.2.2/pyproject.toml` & `parshift-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["parshift"]
 
 [project]
 name = "parshift"
-version = "0.2.2"
+version = "1.0.0"
 description = "Python package based on Gibson's framework (2003) for turn-taking in group conversation analysis."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "python",
     "conversation-analysis",
     "participation-shifts",
```

### Comparing `parshift-0.2.2/tests/test_annotation.py` & `parshift-1.0.0/tests/test_annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     # Apply the annotate() function on the conversation
     conv_annot = annotate(df_read_ccsv)
 
     # Check that the annotate() function returns the expected type
     assert type(conv_annot) == type(parshift_annotation_df)
 
-    # Check that the annotate() function returns a dataframe with the expected
+    # Check that the annotate() function returns a data frame with the expected
     # shape/size
     assert conv_annot.shape == parshift_annotation_df.shape
 
     # Check that the participation shifts are as expected
     assert (
         parshift_annotation_df["pshift"].values == conv_annot["pshift"].values
     ).all()
```

### Comparing `parshift-0.2.2/tests/test_oo_parshift.py` & `parshift-1.0.0/tests/test_oo_parshift.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,71 +28,71 @@
 @pytest.mark.parametrize("N,expecterr", [(5, ValueError)])
 def test_process_error(file_csv_good, N, expecterr):
     model = Parshift()
     with pytest.raises(expecterr):
         model.process(file_csv_good["csv_in"], **(file_csv_good["kwargs"]), N=N)
 
 
-def test_get_plot(file_csv_good, monkeypatch):
+def test_show_plot(file_csv_good, monkeypatch):
     # Patch plt.show() so that it doesn't do anything, otherwise tests will hang
     monkeypatch.setattr(plt, "show", lambda *args, **kwargs: None)
 
     model = Parshift()
     model.process(file_csv_good["csv_in"], **(file_csv_good["kwargs"]))
-    model.get_plot()
-    model.get_plot(type="Pshift_class")
+    model.show_plot()
+    model.show_plot(type="Pshift_class")
 
     model = Parshift()
     model.process(file_csv_good["csv_in"], N=2, **(file_csv_good["kwargs"]))
-    model.get_plot()
-    model.get_plot(type="Pshift_class")
+    model.show_plot()
+    model.show_plot(type="Pshift_class")
 
-    model.get_plot(filename="test.png")
+    model.show_plot(filename="test")
     assert path.exists("test.png")
     if path.exists("test.png"):
         os.remove("test.png")
 
 
 @pytest.mark.parametrize("type,expecterr", [(1, TypeError), ("Bye", ValueError)])
-def test_get_plot_errors(file_csv_good, type, expecterr):
+def test_show_plot_errors(file_csv_good, type, expecterr):
     model = Parshift()
 
     with pytest.raises(ValueError):
-        model.get_plot()
+        model.show_plot()
 
     model.process(file_csv_good["csv_in"], **(file_csv_good["kwargs"]))
     with pytest.raises(expecterr):
-        model.get_plot(type=type)
+        model.show_plot(type=type)
 
     with pytest.raises(TypeError):
-        model.get_plot(filename=1)
+        model.show_plot(filename=1)
 
 
-def test_get_stats(file_csv_good):
+def test_show_stats(file_csv_good):
     model = Parshift()
     model.process(file_csv_good["csv_in"], **(file_csv_good["kwargs"]))
-    model.get_stats(filename="test.csv")
+    model.show_stats(filename="test")
     assert path.exists("test.csv")
     if path.exists("test.csv"):
         os.remove("test.csv")
 
     model = Parshift()
     n = 2
     model.process(file_csv_good["csv_in"], N=n, **(file_csv_good["kwargs"]))
-    model.get_stats(filename="test")
+    model.show_stats(filename="test")
     for i in range(n):
-        assert path.exists(f"test_N{i+1}.csv")
-        if path.exists(f"test_N{i+1}.csv"):
-            os.remove(f"test_N{i+1}.csv")
+        assert path.exists(f"test_n{i+1}.csv")
+        if path.exists(f"test_n{i+1}.csv"):
+            os.remove(f"test_n{i+1}.csv")
 
 
-def test_get_stats_errors():
+def test_show_stats_errors():
     model = Parshift()
     with pytest.raises(ValueError):
-        model.get_stats()
+        model.show_stats()
 
 
 def test_get_propensities_error():
     model = Parshift()
     with pytest.raises(ValueError):
         model.get_propensities()
 
@@ -104,12 +104,12 @@
     assert isinstance(result, pd.DataFrame)
     assert list(result.columns) == ["turn-receiving", "targeting", "termination"]
 
     model.process(file_csv_good["csv_in"], **(file_csv_good["kwargs"]), N=2)
     result = model.get_propensities()
     assert isinstance(result, pd.DataFrame)
     assert list(result.columns) == ["turn-receiving", "targeting", "termination"]
-    assert list(result.index) == ["N1", "N2"]
-    model.get_propensities(filename="test")
-    assert path.exists("test.csv")
-    if path.exists("test.csv"):
-        os.remove("test.csv")
+    assert list(result.index) == ["n1", "n2"]
+    model.get_propensities(filename="test_propensities")
+    assert path.exists("test_propensities.csv")
+    if path.exists("test_propensities.csv"):
+        os.remove("test_propensities.csv")
```

### Comparing `parshift-0.2.2/tests/test_plotting.py` & `parshift-1.0.0/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `parshift-0.2.2/tests/test_statistics.py` & `parshift-1.0.0/tests/test_statistics.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     result = cond_probs(pshift_freq_table["df_ps"])
     assert isinstance(result, pd.DataFrame)
     assert list(result.columns) == [
         "Pshift",
         "Frequency",
         "Probability",
         "P(S|D)",
-        "P(S|D and C)",
+        "P(S|D,C)",
         "Change of Speaker (C)",
         "Directed Remark (D)",
     ]
 
 
 @pytest.mark.parametrize(
     "pscodes,expecterr", [(1, TypeError), ("Bye", TypeError), ({}, TypeError)]
```

