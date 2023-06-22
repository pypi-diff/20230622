# Comparing `tmp/dlt_meta-0.0.2-py3-none-any.whl.zip` & `tmp/dlt_meta-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 19034 bytes, number of entries: 13
--rw-r--r--  2.0 unx       69 b- defN 23-May-18 21:04 src/__init__.py
--rw-r--r--  2.0 unx     1664 b- defN 23-May-18 21:04 src/__main__.py
--rw-r--r--  2.0 unx    16978 b- defN 23-May-18 21:04 src/dataflow_pipeline.py
--rw-r--r--  2.0 unx     9779 b- defN 23-May-18 21:04 src/dataflow_spec.py
--rw-r--r--  2.0 unx     3087 b- defN 23-May-18 21:04 src/metastore_ops.py
--rw-r--r--  2.0 unx    30274 b- defN 23-May-18 21:04 src/onboard_dataflowspec.py
--rw-r--r--  2.0 unx     7658 b- defN 23-May-18 21:04 src/pipeline_readers.py
--rw-r--r--  2.0 unx     3597 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4999 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       34 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1033 b- defN 23-May-18 21:05 dlt_meta-0.0.2.dist-info/RECORD
-13 files, 79268 bytes uncompressed, 17318 bytes compressed:  78.2%
+Zip file size: 19061 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-22 21:00 src/__init__.py
+-rw-r--r--  2.0 unx     1664 b- defN 23-Jun-22 21:00 src/__main__.py
+-rw-r--r--  2.0 unx    17146 b- defN 23-Jun-22 21:00 src/dataflow_pipeline.py
+-rw-r--r--  2.0 unx     9779 b- defN 23-Jun-22 21:00 src/dataflow_spec.py
+-rw-r--r--  2.0 unx     3087 b- defN 23-Jun-22 21:00 src/metastore_ops.py
+-rw-r--r--  2.0 unx    30274 b- defN 23-Jun-22 21:00 src/onboard_dataflowspec.py
+-rw-r--r--  2.0 unx     7658 b- defN 23-Jun-22 21:00 src/pipeline_readers.py
+-rw-r--r--  2.0 unx     3597 b- defN 23-Jun-22 21:01 dlt_meta-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4999 b- defN 23-Jun-22 21:01 dlt_meta-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 21:01 dlt_meta-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-22 21:01 dlt_meta-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-22 21:01 dlt_meta-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Jun-22 21:01 dlt_meta-0.0.3.dist-info/RECORD
+13 files, 79436 bytes uncompressed, 17345 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: src/onboard_dataflowspec.py
 Comment: 
 
 Filename: src/pipeline_readers.py
 Comment: 
 
-Filename: dlt_meta-0.0.2.dist-info/LICENSE.txt
+Filename: dlt_meta-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dlt_meta-0.0.2.dist-info/METADATA
+Filename: dlt_meta-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: dlt_meta-0.0.2.dist-info/WHEEL
+Filename: dlt_meta-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: dlt_meta-0.0.2.dist-info/entry_points.txt
+Filename: dlt_meta-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: dlt_meta-0.0.2.dist-info/top_level.txt
+Filename: dlt_meta-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dlt_meta-0.0.2.dist-info/RECORD
+Filename: dlt_meta-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/dataflow_pipeline.py

```diff
@@ -1,14 +1,14 @@
 """DataflowPipeline provide generic DLT code using dataflowspec."""
 import json
 import logging
 import dlt
 from pyspark.sql import DataFrame
 from pyspark.sql.functions import expr
-from pyspark.sql.types import IntegerType, StructType, StructField
+from pyspark.sql.types import StructType, StructField
 
 from src.dataflow_spec import BronzeDataflowSpec, SilverDataflowSpec, DataflowSpecUtils
 from src.pipeline_readers import PipelineReaders
 
 logger = logging.getLogger("dlt-meta")
 logger.setLevel(logging.INFO)
 
@@ -249,24 +249,28 @@
 
         struct_schema = (
             StructType.fromJson(self.schema_json)
             if type(self.dataflowSpec) == BronzeDataflowSpec
             else self.silver_schema
         )
 
+        sequenced_by_data_type = None
+
         if cdc_apply_changes.except_column_list:
             modified_schema = StructType([])
             for field in struct_schema.fields:
                 if field.name not in cdc_apply_changes.except_column_list:
                     modified_schema.add(field)
+                if field.name == cdc_apply_changes.sequence_by:
+                    sequenced_by_data_type = field.dataType
             struct_schema = modified_schema
 
         if cdc_apply_changes.scd_type == "2":
-            struct_schema.add(StructField("__START_AT", IntegerType()))
-            struct_schema.add(StructField("__END_AT", IntegerType()))
+            struct_schema.add(StructField("__START_AT", sequenced_by_data_type))
+            struct_schema.add(StructField("__END_AT", sequenced_by_data_type))
 
         dlt.create_streaming_live_table(
             name=f"{self.dataflowSpec.targetDetails['table']}",
             table_properties=self.dataflowSpec.tableProperties,
             partition_cols=DataflowSpecUtils.get_partition_cols(self.dataflowSpec.partitionColumns),
             path=self.dataflowSpec.targetDetails["path"],
             schema=struct_schema,
```

## Comparing `dlt_meta-0.0.2.dist-info/LICENSE.txt` & `dlt_meta-0.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dlt_meta-0.0.2.dist-info/METADATA` & `dlt_meta-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt-meta
-Version: 0.0.2
+Version: 0.0.3
 Summary: DLT-META Framework
 Author: Ravi Gawai
 Author-email: databrickslabs@databricks.com
 License: Databricks License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dlt-meta Version: 0.0.2 Summary: DLT-META Framework
+Metadata-Version: 2.1 Name: dlt-meta Version: 0.0.3 Summary: DLT-META Framework
 Author: Ravi Gawai Author-email: databrickslabs@databricks.com License:
 Databricks License Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Classifier: Topic :: Software Development ::
 Testing Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: System Administrators Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE.txt Requires-Dist: setuptools
 Provides-Extra: it Requires-Dist: typer[all] (==0.6.1) ; extra == 'it'
```

## Comparing `dlt_meta-0.0.2.dist-info/RECORD` & `dlt_meta-0.0.3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 src/__init__.py,sha256=3C9Ch9IJrWYMCi3xihpEyh8iL44svXDoNsaz2729GyA,69
 src/__main__.py,sha256=b6bnc9sF1RU9oH305dfanBjzFAWJEvGOqZ7FDDSJWU8,1664
-src/dataflow_pipeline.py,sha256=ni57x1v_vvv6_WHX5TqL0Hsno1O4BOddAJGGrkK6bg4,16978
+src/dataflow_pipeline.py,sha256=x_0QGX_5RmcITVk5irEfZzfZ940f6VivsIfmrJj6wBo,17146
 src/dataflow_spec.py,sha256=8yt9HcMjcneHqlpr3i6JuVfe7kecvBUCmCSFJHKgJbA,9779
 src/metastore_ops.py,sha256=JaX5BjzrWREaMVdd8Qd8nsitYgwL4nhp96CY6EUQre4,3087
 src/onboard_dataflowspec.py,sha256=dO3VLXmz-l-5WTJq6vY4zoGJExK8BIRqmvVx9IpfTtA,30274
 src/pipeline_readers.py,sha256=vq0L2x-tqviZ97nHxUtPhkpXRPFwGMlLkz1NAuVxCKo,7658
-dlt_meta-0.0.2.dist-info/LICENSE.txt,sha256=0yZPLusP5T6Abmovk1Wbboan2y0PNJtTXZjmYzVJqqc,3597
-dlt_meta-0.0.2.dist-info/METADATA,sha256=6vIBpPwl0sBFF3ZM6wjlEmPcUmB-zoFLl4EODA4VvkE,4999
-dlt_meta-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-dlt_meta-0.0.2.dist-info/entry_points.txt,sha256=oDWOW9SsBlk4Uejj1ftYPBxfhJ5ZJctb4JOUIG1rc-4,34
-dlt_meta-0.0.2.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
-dlt_meta-0.0.2.dist-info/RECORD,,
+dlt_meta-0.0.3.dist-info/LICENSE.txt,sha256=0yZPLusP5T6Abmovk1Wbboan2y0PNJtTXZjmYzVJqqc,3597
+dlt_meta-0.0.3.dist-info/METADATA,sha256=ST_g_cnJ12VgJKaG2Wbo-m9MFxdhPuLqQjwSVihsZck,4999
+dlt_meta-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+dlt_meta-0.0.3.dist-info/entry_points.txt,sha256=oDWOW9SsBlk4Uejj1ftYPBxfhJ5ZJctb4JOUIG1rc-4,34
+dlt_meta-0.0.3.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
+dlt_meta-0.0.3.dist-info/RECORD,,
```

