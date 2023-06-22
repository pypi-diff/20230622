# Comparing `tmp/postgres_ddl-1.8.tar.gz` & `tmp/postgres_ddl-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres_ddl-1.8.tar", last modified: Tue Feb 21 12:23:11 2023, max compression
+gzip compressed data, was "postgres_ddl-1.9.tar", last modified: Thu Mar  2 08:51:11 2023, max compression
```

## Comparing `postgres_ddl-1.8.tar` & `postgres_ddl-1.9.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 12:23:11.641535 postgres_ddl-1.8/
--rw-rw-rw-   0        0        0    35823 2022-12-13 12:57:02.000000 postgres_ddl-1.8/LICENSE
--rw-rw-rw-   0        0        0     2716 2023-02-21 12:23:11.640535 postgres_ddl-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2247 2022-12-13 13:22:11.000000 postgres_ddl-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-21 12:23:11.636536 postgres_ddl-1.8/postgres_ddl/
--rw-rw-rw-   0        0        0     2240 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Cast.py
--rw-rw-rw-   0        0        0     1446 2023-02-21 12:13:11.000000 postgres_ddl-1.8/postgres_ddl/Comment.py
--rw-rw-rw-   0        0        0      466 2023-02-09 15:01:33.000000 postgres_ddl-1.8/postgres_ddl/Config.py
--rw-rw-rw-   0        0        0     1845 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/DDL.py
--rw-rw-rw-   0        0        0    36880 2023-02-21 12:21:19.000000 postgres_ddl-1.8/postgres_ddl/Database.py
--rw-rw-rw-   0        0        0     6116 2022-12-13 13:22:11.000000 postgres_ddl-1.8/postgres_ddl/Diff.py
--rw-rw-rw-   0        0        0     3219 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/EventTrigger.py
--rw-rw-rw-   0        0        0     2309 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Extension.py
--rw-rw-rw-   0        0        0     4057 2023-02-06 06:37:43.000000 postgres_ddl-1.8/postgres_ddl/ForeignServer.py
--rw-rw-rw-   0        0        0     4174 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/ForeignTable.py
--rw-rw-rw-   0        0        0     5873 2023-02-20 07:33:00.000000 postgres_ddl-1.8/postgres_ddl/Function.py
--rw-rw-rw-   0        0        0     2411 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Grabber.py
--rw-rw-rw-   0        0        0     2399 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Grant.py
--rw-rw-rw-   0        0        0     2935 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Namespace.py
--rw-rw-rw-   0        0        0     1282 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Owner.py
--rw-rw-rw-   0        0        0     5138 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Procedure.py
--rw-rw-rw-   0        0        0     3441 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Publication.py
--rw-rw-rw-   0        0        0     4776 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Sequence.py
--rw-rw-rw-   0        0        0     4515 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/Subscription.py
--rw-rw-rw-   0        0        0     3993 2023-02-20 07:33:04.000000 postgres_ddl-1.8/postgres_ddl/System.py
--rw-rw-rw-   0        0        0     8908 2023-02-06 06:37:43.000000 postgres_ddl-1.8/postgres_ddl/Table.py
--rw-rw-rw-   0        0        0     4421 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/TableColumn.py
--rw-rw-rw-   0        0        0     3385 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/TableConstraint.py
--rw-rw-rw-   0        0        0     2072 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/TableIndex.py
--rw-rw-rw-   0        0        0     3068 2023-02-06 06:37:43.000000 postgres_ddl-1.8/postgres_ddl/TablePolicy.py
--rw-rw-rw-   0        0        0     2268 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/TableSequence.py
--rw-rw-rw-   0        0        0     1718 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/TableSettings.py
--rw-rw-rw-   0        0        0     2695 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/TableTrigger.py
--rw-rw-rw-   0        0        0     1770 2023-02-06 06:37:43.000000 postgres_ddl-1.8/postgres_ddl/UserMapping.py
--rw-rw-rw-   0        0        0     4900 2023-02-06 06:01:35.000000 postgres_ddl-1.8/postgres_ddl/View.py
--rw-rw-rw-   0        0        0       23 2022-12-13 13:22:11.000000 postgres_ddl-1.8/postgres_ddl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-21 12:23:11.639536 postgres_ddl-1.8/postgres_ddl.egg-info/
--rw-rw-rw-   0        0        0     2716 2023-02-21 12:23:11.000000 postgres_ddl-1.8/postgres_ddl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1003 2023-02-21 12:23:11.000000 postgres_ddl-1.8/postgres_ddl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 12:23:11.000000 postgres_ddl-1.8/postgres_ddl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-02-21 12:23:11.000000 postgres_ddl-1.8/postgres_ddl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-21 12:23:11.000000 postgres_ddl-1.8/postgres_ddl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-21 12:23:11.641535 postgres_ddl-1.8/setup.cfg
--rw-rw-rw-   0        0        0      752 2023-02-21 12:23:00.000000 postgres_ddl-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-02 08:51:11.405861 postgres_ddl-1.9/
+-rw-rw-rw-   0        0        0    35823 2022-12-13 12:57:02.000000 postgres_ddl-1.9/LICENSE
+-rw-rw-rw-   0        0        0     2716 2023-03-02 08:51:11.405861 postgres_ddl-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2247 2022-12-13 13:22:11.000000 postgres_ddl-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-02 08:51:11.400862 postgres_ddl-1.9/postgres_ddl/
+-rw-rw-rw-   0        0        0     2240 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Cast.py
+-rw-rw-rw-   0        0        0     1446 2023-02-21 12:13:11.000000 postgres_ddl-1.9/postgres_ddl/Comment.py
+-rw-rw-rw-   0        0        0      557 2023-03-02 08:51:05.000000 postgres_ddl-1.9/postgres_ddl/Config.py
+-rw-rw-rw-   0        0        0     2536 2023-03-02 08:51:05.000000 postgres_ddl-1.9/postgres_ddl/DDL.py
+-rw-rw-rw-   0        0        0    40934 2023-03-02 08:51:05.000000 postgres_ddl-1.9/postgres_ddl/Database.py
+-rw-rw-rw-   0        0        0     6116 2022-12-13 13:22:11.000000 postgres_ddl-1.9/postgres_ddl/Diff.py
+-rw-rw-rw-   0        0        0     3219 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/EventTrigger.py
+-rw-rw-rw-   0        0        0     2309 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Extension.py
+-rw-rw-rw-   0        0        0     4057 2023-02-06 06:37:43.000000 postgres_ddl-1.9/postgres_ddl/ForeignServer.py
+-rw-rw-rw-   0        0        0     4174 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/ForeignTable.py
+-rw-rw-rw-   0        0        0     5873 2023-02-20 07:33:00.000000 postgres_ddl-1.9/postgres_ddl/Function.py
+-rw-rw-rw-   0        0        0     2411 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Grabber.py
+-rw-rw-rw-   0        0        0     2399 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Grant.py
+-rw-rw-rw-   0        0        0     2935 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Namespace.py
+-rw-rw-rw-   0        0        0     1282 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Owner.py
+-rw-rw-rw-   0        0        0     5138 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Procedure.py
+-rw-rw-rw-   0        0        0     3441 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Publication.py
+-rw-rw-rw-   0        0        0     4776 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Sequence.py
+-rw-rw-rw-   0        0        0     4515 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/Subscription.py
+-rw-rw-rw-   0        0        0     3993 2023-02-20 07:33:04.000000 postgres_ddl-1.9/postgres_ddl/System.py
+-rw-rw-rw-   0        0        0     2165 2023-03-02 08:51:05.000000 postgres_ddl-1.9/postgres_ddl/TSDB_Dimension.py
+-rw-rw-rw-   0        0        0     7738 2023-03-02 08:51:05.000000 postgres_ddl-1.9/postgres_ddl/TSDB_HyperTable.py
+-rw-rw-rw-   0        0        0     9293 2023-03-02 08:51:05.000000 postgres_ddl-1.9/postgres_ddl/Table.py
+-rw-rw-rw-   0        0        0     4421 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/TableColumn.py
+-rw-rw-rw-   0        0        0     3385 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/TableConstraint.py
+-rw-rw-rw-   0        0        0     2072 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/TableIndex.py
+-rw-rw-rw-   0        0        0     3068 2023-02-06 06:37:43.000000 postgres_ddl-1.9/postgres_ddl/TablePolicy.py
+-rw-rw-rw-   0        0        0     2268 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/TableSequence.py
+-rw-rw-rw-   0        0        0     1718 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/TableSettings.py
+-rw-rw-rw-   0        0        0     2695 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/TableTrigger.py
+-rw-rw-rw-   0        0        0     1770 2023-02-06 06:37:43.000000 postgres_ddl-1.9/postgres_ddl/UserMapping.py
+-rw-rw-rw-   0        0        0     4900 2023-02-06 06:01:35.000000 postgres_ddl-1.9/postgres_ddl/View.py
+-rw-rw-rw-   0        0        0       23 2022-12-13 13:22:11.000000 postgres_ddl-1.9/postgres_ddl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-02 08:51:11.404861 postgres_ddl-1.9/postgres_ddl.egg-info/
+-rw-rw-rw-   0        0        0     2716 2023-03-02 08:51:11.000000 postgres_ddl-1.9/postgres_ddl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2023-03-02 08:51:11.000000 postgres_ddl-1.9/postgres_ddl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-02 08:51:11.000000 postgres_ddl-1.9/postgres_ddl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-03-02 08:51:11.000000 postgres_ddl-1.9/postgres_ddl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-03-02 08:51:11.000000 postgres_ddl-1.9/postgres_ddl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-02 08:51:11.405861 postgres_ddl-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      752 2023-03-02 08:51:05.000000 postgres_ddl-1.9/setup.py
```

### Comparing `postgres_ddl-1.8/LICENSE` & `postgres_ddl-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/PKG-INFO` & `postgres_ddl-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgres_ddl
-Version: 1.8
+Version: 1.9
 Summary: PostgreSQL metadata grabber and comparer
 Home-page: https://github.com/ish1mura/postgres_ddl
 Author: ish1mura
 Author-email: ek.dummy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `postgres_ddl-1.8/README.md` & `postgres_ddl-1.9/README.md`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Cast.py` & `postgres_ddl-1.9/postgres_ddl/Cast.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Comment.py` & `postgres_ddl-1.9/postgres_ddl/Comment.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/DDL.py` & `postgres_ddl-1.9/postgres_ddl/DDL.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
+from postgres_ddl.Config import Config
+
 class DDL(object):
     def __init__(self, parent, data):
         self.Parent = (parent or "").strip().lower()
 
         assert data is not None, \
             "{0} data is null".format(type(self))
 
@@ -22,14 +24,17 @@
 
     def DDL_Drop(self):
         raise NotImplementedError("DDL_Drop method is not implemented for class {0}".format(type(self)))
 
     def GetObjectType(self):
         raise NotImplementedError("GetObjectType method is not implemented for class {0}".format(type(self)))
 
+    def GetObjectTypeComment(self):
+        raise NotImplementedError("GetObjectTypeComment method is not implemented for class {0}".format(type(self)))
+
     def GetObjectName(self):
         raise NotImplementedError("GetObjectName method is not implemented for class {0}".format(type(self)))
 
     def GetObjectTypeFile(self, path):
         return "/".join([path, "{0}.sql".format(self.GetObjectType())])
 
     def GetFullName(self):
@@ -48,7 +53,24 @@
         return None
 
     def GetChildObjects(self):
         return {}
 
     def Diff(self, another):
         return []
+
+    def FillFunctionParams(self, params=[], is_inline=False, sign=Config.FncParamSign):
+        result = []
+
+        sep = Config.NL
+        indent = Config.Indent
+        if is_inline is True:
+            sep = " "
+            indent = ""
+
+        for (name, value, is_quote) in (params or []):
+            if is_quote is True:
+                value = f"'{value}'"
+            result.append(f"{indent}{name} {sign} {value}")
+
+        return f",{sep}".join(sorted(result))
+
```

### Comparing `postgres_ddl-1.8/postgres_ddl/Database.py` & `postgres_ddl-1.9/postgres_ddl/Database.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             @param exclude_schemas: Excluded schemas (namespaces)
         """
         self.Connect        = self.GetConnectionString(connect)
         self.IsSuperUser    = False
         self.Version        = None
         self.Objects        = {}
         self.ExcludeSchemas = exclude_schemas
+        self.HasTimescaleDB = False
 
     def __str__(self):
         """
             String representation
         """
         return str(self.PG)
 
@@ -50,22 +51,22 @@
 
         with psycopg2.connect(self.Connect) as conn:
             conn.set_isolation_level(ISOLATION_LEVEL_READ_COMMITTED)
             with conn.cursor(cursor_factory = RealDictCursor) as cursor:
                 self.GetSuperUser(cursor)
                 self.GetVersion(cursor)
                 self.GetNamespace(cursor)
+                self.GetExtension(cursor)
                 self.GetTable(cursor)
                 self.GetFunction(cursor)
                 self.GetProcedure(cursor)
                 self.GetView(cursor)
                 self.GetSequence(cursor)
                 self.GetForeignServer(cursor)
                 self.GetForeignTable(cursor)
-                self.GetExtension(cursor)
                 self.GetPublication(cursor)
                 self.GetSubscription(cursor)
                 self.GetEventTrigger(cursor)
                 self.GetCast(cursor)
 
     def GetConnectionString(self, connect):
         assert connect is not None, \
@@ -358,14 +359,88 @@
             result[row.get("table_oid")] = row
 
         logging.info("GetTableSequence loaded = {0}".format(cursor.rowcount))
 
         return result
 
     @CalcDuration
+    def GetTSDBHyperTable(self, cursor):
+        result = {}
+
+        if not self.HasTimescaleDB:
+            return result
+
+        cursor.execute("""
+            select
+                h.id,
+                concat_ws('.', h.schema_name, h.table_name) as relation,
+                h.associated_schema_name as parts_schema,
+                h.associated_table_prefix as parts_prefix,
+                h.compression_state > 0 as is_compress,
+                nullif(trim(case
+                    when jc.config is null then null
+                    else format('INTERVAL %L', jc.config ->> 'compress_after')
+                end), '') as compress_after,
+                nullif(trim(cmp.order_by), '') as compress_order_by,
+                nullif(trim(cmp.segment_by), '') as compress_segment_by,
+                nullif(trim(case
+                    when jr.config is null then null
+                    else format('INTERVAL %L', jr.config ->> 'drop_after')
+                end), '') as drop_after,
+                (
+                    select jsonb_agg(q order by q.order_num)
+                    from (
+                        select
+                            d.column_name,
+                            d.num_slices,
+                            nullif(trim(concat_ws('.', d.partitioning_func_schema, d.partitioning_func)), '') as fnc_part,
+                            nullif(trim(concat_ws('.', d.integer_now_func_schema, d.integer_now_func)), '') as fnc_int_now,
+                            row_number() over (partition by d.hypertable_id order by d.id asc) as order_num,
+                            case
+                                when d.interval_length is null then null
+                                when (
+                                    d.column_type::varchar !~* 'timestamp' and
+                                    d.column_type::varchar !~* 'date'
+                                ) then d.interval_length::varchar
+                                else format('INTERVAL %L', format('%s sec', d.interval_length / 1000000))
+                            end as interval
+                        from _timescaledb_catalog.dimension d
+                        where d.hypertable_id = h.id
+                    ) q
+                ) as dimensions
+            from _timescaledb_catalog.hypertable h
+            left join _timescaledb_config.bgw_job jc ON
+                jc.hypertable_id = h.id and
+                jc.proc_name = 'policy_compression'
+            left join _timescaledb_config.bgw_job jr ON
+                jr.hypertable_id = h.id and
+                jr.proc_name = 'policy_retention'
+            left join lateral(
+                SELECT
+                    string_agg(format('"%s" %s NULLS %s',
+                        hc.attname,
+                        case when hc.orderby_asc then 'ASC' else 'DESC' end,
+                        case when hc.orderby_nullsfirst then 'FIRST' else 'LAST' end
+                    ), ', ' order by hc.orderby_column_index asc)
+                        filter (where hc.orderby_column_index > 0) as order_by,
+                    string_agg(format('"%s"', hc.attname), ', ' order by hc.segmentby_column_index asc)
+                        filter (where hc.segmentby_column_index > 0) as segment_by
+                FROM _timescaledb_catalog.hypertable_compression hc
+                where hc.hypertable_id = h.id
+            ) cmp on true
+            where h.num_dimensions > 0
+        """)
+        for row in cursor.fetchall():
+            result[row.get("relation")] = row
+
+        logging.info("GetTSDBHyperTable loaded = {0}".format(cursor.rowcount))
+
+        return result
+
+    @CalcDuration
     def GetTable(self, cursor):
         if self.Version in (9, 9):
             query = """
                 SELECT
                     c.oid,
                     trim(lower(n.nspname)) AS schema,
                     trim(lower(c.relname)) AS name,
@@ -473,24 +548,27 @@
 
         columns = self.GetTableColumn(cursor)
         constraints = self.GetTableConstraint(cursor)
         indexes = self.GetTableIndex(cursor)
         sequences = self.GetTableSequence(cursor)
         triggers = self.GetTableTrigger(cursor)
         policies = self.GetTablePolicy(cursor)
+        tsdb_hypertable = self.GetTSDBHyperTable(cursor)
 
         cursor.execute(query, [self.ExcludeSchemas])
         for row in cursor.fetchall():
             table_oid = row.get("oid") or 0
+            table_name = ".".join([row.get("schema"), row.get("name")])
             row["columns"] = columns.get(table_oid)
             row["constraints"] = constraints.get(table_oid)
             row["sequence"] = sequences.get(table_oid)
             row["indexes"] = indexes.get(table_oid)
             row["triggers"] = triggers.get(table_oid)
             row["policies"] = policies.get(table_oid)
+            row["tsdb_hypertable"] = tsdb_hypertable.get(table_name)
             self.Objects.update(Table(None, row).Export())
 
         logging.info("GetTable loaded = {0}".format(cursor.rowcount))
 
     @CalcDuration
     def GetFunction(self, cursor):
         cursor.execute("""
@@ -796,14 +874,17 @@
             JOIN pg_roles o ON
                 o.oid = e.extowner
         """)
 
         for row in cursor.fetchall():
             self.Objects.update(Extension(None, row).Export())
 
+            if row.get("name") == 'timescaledb':
+                self.HasTimescaleDB = True
+
         logging.info("GetExtension loaded = {0}".format(cursor.rowcount))
 
     @CalcDuration
     def GetPublication(self, cursor):
         query = """
             select
                 p.oid,
```

### Comparing `postgres_ddl-1.8/postgres_ddl/Diff.py` & `postgres_ddl-1.9/postgres_ddl/Diff.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/EventTrigger.py` & `postgres_ddl-1.9/postgres_ddl/EventTrigger.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Extension.py` & `postgres_ddl-1.9/postgres_ddl/Extension.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/ForeignServer.py` & `postgres_ddl-1.9/postgres_ddl/ForeignServer.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/ForeignTable.py` & `postgres_ddl-1.9/postgres_ddl/ForeignTable.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Function.py` & `postgres_ddl-1.9/postgres_ddl/Function.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Grabber.py` & `postgres_ddl-1.9/postgres_ddl/Grabber.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Grant.py` & `postgres_ddl-1.9/postgres_ddl/Grant.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Namespace.py` & `postgres_ddl-1.9/postgres_ddl/Namespace.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Owner.py` & `postgres_ddl-1.9/postgres_ddl/Owner.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Procedure.py` & `postgres_ddl-1.9/postgres_ddl/Procedure.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Publication.py` & `postgres_ddl-1.9/postgres_ddl/Publication.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Sequence.py` & `postgres_ddl-1.9/postgres_ddl/Sequence.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Subscription.py` & `postgres_ddl-1.9/postgres_ddl/Subscription.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/System.py` & `postgres_ddl-1.9/postgres_ddl/System.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/Table.py` & `postgres_ddl-1.9/postgres_ddl/Table.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from postgres_ddl.TableColumn import TableColumn
 from postgres_ddl.TableConstraint import TableConstraint
 from postgres_ddl.TableIndex import TableIndex
 from postgres_ddl.TablePolicy import TablePolicy
 from postgres_ddl.TableSequence import TableSequence
 from postgres_ddl.TableSettings import TableSettings
 from postgres_ddl.TableTrigger import TableTrigger
+from postgres_ddl.TSDB_HyperTable import TSDB_HyperTable
 
 class Table(DDL):
     def __init__(self, parent, data):
         super().__init__(parent, data)
 
         self.Oid = (data.get("oid") or 0)
         assert self.Oid > 0, \
@@ -125,14 +126,18 @@
         self.Policies = []
         for plc in (data.get("policies") or []):
             plc["schema"] = self.Schema
             plc["table"] = self.Name
             plc = TablePolicy(self.GetObjectName(), plc)
             self.Policies.append(plc)
 
+        self.TSDB_HyperTable = None
+        if data.get("tsdb_hypertable") is not None:
+            self.TSDB_HyperTable = TSDB_HyperTable(self.GetFullName(), data.get("tsdb_hypertable") or [])
+
     def __str__(self):
         return self.GetFullName()
 
     def GetObjectType(self):
         return "table"
 
     def GetObjectName(self):
@@ -234,14 +239,18 @@
             r += trg.DDL_Create()
             r += Config.NL + Config.NL
 
         for plc in sorted(self.Policies, key=lambda x: x.GetFullName()):
             r += plc.DDL_Create()
             r += Config.NL + Config.NL
 
+        if self.TSDB_HyperTable is not None:
+            r += self.TSDB_HyperTable.DDL_Create()
+            r += Config.NL
+
         return r.strip() + Config.NL
 
     def GetPath(self):
         return [self.Schema, "table"]
 
     def GetFileName(self):
         return f"{self.Name}.sql"
```

### Comparing `postgres_ddl-1.8/postgres_ddl/TableColumn.py` & `postgres_ddl-1.9/postgres_ddl/TableColumn.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/TableConstraint.py` & `postgres_ddl-1.9/postgres_ddl/TableConstraint.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/TableIndex.py` & `postgres_ddl-1.9/postgres_ddl/TableIndex.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/TablePolicy.py` & `postgres_ddl-1.9/postgres_ddl/TablePolicy.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/TableSequence.py` & `postgres_ddl-1.9/postgres_ddl/TableSequence.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/TableSettings.py` & `postgres_ddl-1.9/postgres_ddl/TableSettings.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/TableTrigger.py` & `postgres_ddl-1.9/postgres_ddl/TableTrigger.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/UserMapping.py` & `postgres_ddl-1.9/postgres_ddl/UserMapping.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl/View.py` & `postgres_ddl-1.9/postgres_ddl/View.py`

 * *Files identical despite different names*

### Comparing `postgres_ddl-1.8/postgres_ddl.egg-info/PKG-INFO` & `postgres_ddl-1.9/postgres_ddl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgres-ddl
-Version: 1.8
+Version: 1.9
 Summary: PostgreSQL metadata grabber and comparer
 Home-page: https://github.com/ish1mura/postgres_ddl
 Author: ish1mura
 Author-email: ek.dummy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `postgres_ddl-1.8/postgres_ddl.egg-info/SOURCES.txt` & `postgres_ddl-1.9/postgres_ddl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 postgres_ddl/Namespace.py
 postgres_ddl/Owner.py
 postgres_ddl/Procedure.py
 postgres_ddl/Publication.py
 postgres_ddl/Sequence.py
 postgres_ddl/Subscription.py
 postgres_ddl/System.py
+postgres_ddl/TSDB_Dimension.py
+postgres_ddl/TSDB_HyperTable.py
 postgres_ddl/Table.py
 postgres_ddl/TableColumn.py
 postgres_ddl/TableConstraint.py
 postgres_ddl/TableIndex.py
 postgres_ddl/TablePolicy.py
 postgres_ddl/TableSequence.py
 postgres_ddl/TableSettings.py
```

### Comparing `postgres_ddl-1.8/setup.py` & `postgres_ddl-1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="postgres_ddl",
-    version="1.8",
+    version="1.9",
     author="ish1mura",
     author_email="ek.dummy@gmail.com",
     description="PostgreSQL metadata grabber and comparer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ish1mura/postgres_ddl",
     packages=setuptools.find_packages(),
```

