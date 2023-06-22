# Comparing `tmp/lamin_logger-0.7.0.tar.gz` & `tmp/lamin_logger-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.7.0.tar` & `lamin_logger-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.0/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.0/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.0/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.0/docs/api.md
--rw-r--r--   0        0        0     4306 2023-06-21 14:29:41.424448 lamin_logger-0.7.0/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.0/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.0/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.0/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-06-21 14:29:33.203168 lamin_logger-0.7.0/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.0/lamin_logger/_core.py
--rw-r--r--   0        0        0     3442 2023-06-21 14:28:14.948996 lamin_logger-0.7.0/lamin_logger/_inspect.py
--rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.7.0/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.7.0/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     6603 2023-06-21 14:28:14.949325 lamin_logger-0.7.0/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.0/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.0/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.0/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.0/tests/test_base.py
--rw-r--r--   0        0        0     3437 2023-06-21 14:28:14.949583 lamin_logger-0.7.0/tests/test_inspect.py
--rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.0/tests/test_lookup.py
--rw-r--r--   0        0        0     5300 2023-06-19 17:49:41.484125 lamin_logger-0.7.0/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.0/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.1/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.1/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.1/docs/api.md
+-rw-r--r--   0        0        0     4471 2023-06-22 14:21:14.438600 lamin_logger-0.7.1/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.1/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.1/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.1/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-06-22 14:21:07.142843 lamin_logger-0.7.1/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.1/lamin_logger/_core.py
+-rw-r--r--   0        0        0     3828 2023-06-22 14:19:30.502828 lamin_logger-0.7.1/lamin_logger/_inspect.py
+-rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.7.1/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.7.1/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     7160 2023-06-22 14:19:30.503212 lamin_logger-0.7.1/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.1/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.7.1/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.1/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.1/tests/test_base.py
+-rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.1/tests/test_inspect.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.1/tests/test_lookup.py
+-rw-r--r--   0        0        0     5769 2023-06-22 14:19:30.503907 lamin_logger-0.7.1/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.1/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.1/PKG-INFO
```

### Comparing `lamin_logger-0.7.0/.github/workflows/build.yml` & `lamin_logger-0.7.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/.github/workflows/latest-changes.yml` & `lamin_logger-0.7.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/.gitignore` & `lamin_logger-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/.pre-commit-config.yaml` & `lamin_logger-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/LICENSE` & `lamin_logger-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/docs/changelog.md` & `lamin_logger-0.7.1/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Fix case sensitivity in map_synonyms | [31](https://github.com/laminlabs/lamin-logger/pull/31) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-22 | 0.7.1
 🚚 Moved inspect from bionty | [30](https://github.com/laminlabs/lamin-logger/pull/30) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-21 | 0.7.0
 🚑️ Map_synonyms only returns mapped synonyms not names | [29](https://github.com/laminlabs/lamin-logger/pull/29) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-20 | 0.6.2
 🧪 Deal with empty dataframes | [28](https://github.com/laminlabs/lamin-logger/pull/28) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.1
 ✨ Add case_sensitive to map_synonyms | [27](https://github.com/laminlabs/lamin-logger/pull/27) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.0
 🧪 Test every line of search | [25](https://github.com/laminlabs/lamin-logger/pull/25) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 | 0.5.3
 🚑️ Fix empty string input for `map_synonyms` | [24](https://github.com/laminlabs/lamin-logger/pull/24) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 |
 💄 Log to stdout rather than stderr | [23](https://github.com/laminlabs/lamin-logger/pull/23) | [falexwolf](https://github.com/falexwolf) | 2023-06-16 | 0.5.2
```

### Comparing `lamin_logger-0.7.0/docs/quickstart.ipynb` & `lamin_logger-0.7.1/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/lamin_logger/_core.py` & `lamin_logger-0.7.1/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/lamin_logger/_inspect.py` & `lamin_logger-0.7.1/lamin_logger/_inspect.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,29 @@
     Returns:
         - A Dictionary of "mapped" and "unmapped" identifiers
         - If `return_df`: A DataFrame indexed by identifiers with a boolean `__mapped__`
             column that indicates compliance with the identifiers.
     """
     import pandas as pd
 
+    def unique_rm_empty(idx: pd.Index):
+        idx = idx.unique()
+        return idx[(idx != "") & (~idx.isnull())]
+
+    uniq_identifiers = unique_rm_empty(pd.Index(identifiers)).tolist()
+    # empty DataFrame or input
+    if df.shape[0] == 0 or len(uniq_identifiers) == 0:
+        if return_df:
+            return pd.DataFrame(index=identifiers, data={"__mapped__": False})
+        else:
+            return {
+                "mapped": [],
+                "not_mapped": uniq_identifiers,
+            }
+
     # check if index is compliant
     mapped_df = check_if_ids_in_field_values(
         identifiers=identifiers,
         field_values=df[field],
         case_sensitive=case_sensitive,
     )
     if case_sensitive is False:
@@ -46,18 +61,14 @@
         )
         if mapped_df_cs["__mapped__"].sum() < mapped_df["__mapped__"].sum():
             logger.warning(
                 "Detected inconsistent casing of mapped terms!\n   For best practice,"
                 " standardize casing via '.map_synonyms()'"
             )
 
-    def unique_rm_empty(idx: pd.Index):
-        idx = idx.unique()
-        return idx[(idx != "") & (~idx.isnull())]
-
     mapped = unique_rm_empty(mapped_df.index[mapped_df["__mapped__"]]).tolist()
     unmapped = unique_rm_empty(mapped_df.index[~mapped_df["__mapped__"]]).tolist()
 
     if inspect_synonyms:
         try:
             synonyms_mapper = map_synonyms(
                 df=df,
```

### Comparing `lamin_logger-0.7.0/lamin_logger/_logger.py` & `lamin_logger-0.7.1/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/lamin_logger/_lookup.py` & `lamin_logger-0.7.1/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/lamin_logger/_map_synonyms.py` & `lamin_logger-0.7.1/lamin_logger/_map_synonyms.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     Returns:
         - If return_mapper is False: a list of mapped field values.
         - If return_mapper is True: a dictionary of mapped values with mappable
             identifiers as keys and values mapped to field as values.
     """
     import pandas as pd
 
-    # empty DataFrame
-    if df.shape[0] == 0:
+    # empty DataFrame or input
+    if df.shape[0] == 0 or len(list(identifiers)) == 0:
         if return_mapper:
             return {}
         else:
             return list(identifiers)
 
     if field not in df.columns:
         raise KeyError(
@@ -55,51 +55,61 @@
         raise KeyError(
             f"synonyms_field '{synonyms_field}' is invalid! Available fields"
             f" are: {list(df.columns)}"
         )
     if field == synonyms_field:
         raise KeyError("synonyms_field must be different from field!")
 
-    # only map synonyms for those ids that don't match the field column
-    df = df[~df[field].isin(identifiers)]
+    # A DataFrame indexed by the passed identifiers
+    mapped_df = pd.DataFrame(data={"orig_ids": identifiers})
+    mapped_df["__agg__"] = to_str(mapped_df["orig_ids"], case_sensitive=case_sensitive)
 
-    # {synonym: name}
-    syn_map = explode_aggregated_column_to_map(
-        df=df,
-        agg_col=synonyms_field,
-        target_col=field,
-        keep=keep,
-        sep=sep,
-    )
+    # __agg__ is a column of identifiers based on case_sensitive
+    df["__agg__"] = to_str(df[field], case_sensitive=case_sensitive)
+    field_map = pd.merge(mapped_df, df, on="__agg__").set_index("__agg__")[field]
+
+    # only runs if synonyms mapping is needed
+    if len(field_map) < mapped_df.shape[0]:
+        # only map synonyms for those ids that don't match the field case insensitively
+        # {synonym: name}
+        syn_map = explode_aggregated_column_to_map(
+            df=df[~df["__agg__"].isin(mapped_df["__agg__"])],
+            agg_col=synonyms_field,
+            target_col=field,
+            keep=keep,
+            sep=sep,
+        )
+
+        if not case_sensitive:
+            # convert the synonyms to the same case_sensitive
+            syn_map.index = syn_map.index.str.lower()
+            # TODO: allow returning duplicated entries
+            syn_map = syn_map[syn_map.index.drop_duplicates()]
+        syn_map = syn_map.to_dict()
+    else:
+        syn_map = {}
 
-    # A DataFrame indexed by the passed identifiers
-    mapped_df = pd.DataFrame(index=identifiers)
-    # _field is a column if identifiers based on case_sensitive
-    mapped_df["_field"] = to_str(mapped_df.index, case_sensitive=case_sensitive)
-    if not case_sensitive:
-        # convert the synonyms to the same case_sensitive
-        syn_map.index = syn_map.index.str.lower()
-        # TODO: allow returning duplicated entries
-        syn_map = syn_map[syn_map.index.drop_duplicates()]
     # mapped synonyms will have values, otherwise NAs
-    mapped = mapped_df["_field"].map(syn_map.to_dict())
+    mapped_df.index = mapped_df["orig_ids"]
+    mapped = mapped_df["__agg__"].map({**field_map.to_dict(), **syn_map})
 
     if return_mapper:
         # only returns mapped synonyms
         mapper = mapped[~mapped.isna()].to_dict()
+        mapper = {k: v for k, v in mapper.items() if k != v}
         if keep is False:
             logger.warning(
                 "Retuning mapper might contain lists as values when 'keep=False'"
             )
             return {k: v[0] if len(v) == 1 else v for k, v in mapper.items()}
         else:
             return mapper
     else:
         # returns a list in the input order with synonyms replaced
-        mapped_list = mapped.fillna(mapped_df.index.to_series()).tolist()
+        mapped_list = mapped.fillna(mapped_df["orig_ids"]).tolist()
         if keep is False:
             logger.warning("Returning list might contain lists when 'keep=False'")
             return [
                 v[0] if isinstance(v, list) and len(v) == 1 else v for v in mapped_list
             ]
         else:
             return mapped_list
```

### Comparing `lamin_logger-0.7.0/lamin_logger/_python_version.py` & `lamin_logger-0.7.1/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/lamin_logger/_search.py` & `lamin_logger-0.7.1/lamin_logger/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/pyproject.toml` & `lamin_logger-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/tests/test_inspect.py` & `lamin_logger-0.7.1/tests/test_inspect.py`

 * *Files 14% similar despite different names*

```diff
@@ -121,7 +121,36 @@
 
     mapping = inspect(
         df=df,
         identifiers=pd.Series(["A1CF", "A1BG", "A1BG", "", None, np.nan]),
         field="symbol",
     )
     assert mapping == {"mapped": ["A1CF", "A1BG"], "not_mapped": []}
+
+
+def test_inspect_empty_df():
+    import numpy as np
+    import pandas as pd
+
+    mapping = inspect(
+        df=pd.DataFrame(),
+        identifiers=pd.Series(["A1CF", "A1BG", "A1BG", "", None, np.nan]),
+        field="symbol",
+    )
+
+    assert mapping == {"mapped": [], "not_mapped": ["A1CF", "A1BG"]}
+
+    mapping = inspect(
+        df=pd.DataFrame(),
+        identifiers=pd.Series(["A1CF", "A1BG", "A1BG", "", None, np.nan]),
+        field="symbol",
+        return_df=True,
+    )
+
+    expected_df = pd.DataFrame(
+        index=["A1CF", "A1BG", "A1BG", "", None, np.nan],
+        data={
+            "__mapped__": [False, False, False, False, False, False],
+        },
+    )
+
+    assert mapping.equals(expected_df)
```

### Comparing `lamin_logger-0.7.0/tests/test_lookup.py` & `lamin_logger-0.7.1/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/tests/test_map_synonyms.py` & `lamin_logger-0.7.1/tests/test_map_synonyms.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,31 @@
     mapper = map_synonyms(
         df=df, identifiers=gene_symbols, field="symbol", return_mapper=True
     )
 
     assert mapper == {"FANCD1": "BRCA2", "GCS": "GCLC"}
 
 
+def test_map_synonyms_case_sensitive(genes):
+    _, df = genes
+
+    mapping = map_synonyms(
+        df=df, identifiers=["A1CF", "FANCD1", "a1CF", "fancd1"], field="symbol"
+    )
+    assert mapping == ["A1CF", "BRCA2", "A1CF", "BRCA2"]
+
+    mapping = map_synonyms(
+        df=df,
+        identifiers=["A1CF", "FANCD1", "a1CF", "fancd1"],
+        field="symbol",
+        case_sensitive=True,
+    )
+    assert mapping == ["A1CF", "BRCA2", "a1CF", "fancd1"]
+
+
 def test_map_synonyms_empty_values(genes):
     _, df = genes
 
     result = map_synonyms(
         df=df,
         identifiers=["", " ", None, "CD3", "FANCD1"],
         field="symbol",
@@ -91,15 +108,15 @@
     ) == [["GCLC", "UGCG"], "A1CF"]
 
     assert map_synonyms(
         df, identifiers=["GCS", "A1CF"], field="symbol", keep=False, return_mapper=True
     ) == {"GCS": ["GCLC", "UGCG"]}
 
 
-def test_unsupported_field(genes):
+def test_map_synonyms_unsupported_field(genes):
     gene_symbols, df = genes
     with pytest.raises(KeyError):
         map_synonyms(df=df, identifiers=gene_symbols, field="name", return_mapper=False)
     with pytest.raises(KeyError):
         map_synonyms(
             df=df,
             identifiers=gene_symbols,
@@ -113,14 +130,24 @@
             identifiers=gene_symbols,
             field="symbol",
             synonyms_field="symbol",
             return_mapper=False,
         )
 
 
+def test_map_synonyms_empty_df():
+    assert (
+        map_synonyms(
+            df=pd.DataFrame(), identifiers=[], field="name", return_mapper=True
+        )
+        == {}
+    )
+    assert map_synonyms(df=pd.DataFrame(), identifiers=[], field="name") == []
+
+
 def test_to_str():
     import numpy as np
 
     assert to_str(pd.Index(["A", "a", None, np.nan])).tolist() == ["a", "a", "", ""]
     assert to_str(pd.Series(["A", "a", None, np.nan])).tolist() == ["a", "a", "", ""]
     assert to_str(
         pd.Series(["A", "a", None, np.nan]), case_sensitive=True
@@ -179,17 +206,7 @@
             df, agg_col="synonyms", target_col="symbol", keep="last"
         ).get("GCS")
         == "UGCG"
     )
     assert explode_aggregated_column_to_map(
         df, agg_col="synonyms", target_col="symbol", keep=False
     ).get("GCS") == ["GCLC", "UGCG"]
-
-
-def test_map_synonyms_empty_df():
-    assert (
-        map_synonyms(
-            df=pd.DataFrame(), identifiers=[], field="name", return_mapper=True
-        )
-        == {}
-    )
-    assert map_synonyms(df=pd.DataFrame(), identifiers=[], field="name") == []
```

### Comparing `lamin_logger-0.7.0/tests/test_search.py` & `lamin_logger-0.7.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.0/PKG-INFO` & `lamin_logger-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.7.0
+Version: 0.7.1
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

