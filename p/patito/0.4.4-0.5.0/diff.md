# Comparing `tmp/patito-0.4.4.tar.gz` & `tmp/patito-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patito-0.4.4.tar", max compression
+gzip compressed data, was "patito-0.5.0.tar", max compression
```

## Comparing `patito-0.4.4.tar` & `patito-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1077 2022-12-02 17:38:36.845788 patito-0.4.4/LICENSE
--rw-r--r--   0        0        0    12932 2022-12-02 17:38:36.845788 patito-0.4.4/README.md
--rw-r--r--   0        0        0     3194 2022-12-02 17:38:36.849788 patito-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1079 2022-12-02 17:38:36.849788 patito-0.4.4/src/patito/__init__.py
--rw-r--r--   0        0        0      161 2022-12-02 17:38:36.849788 patito-0.4.4/src/patito/_docs.py
--rw-r--r--   0        0        0   113624 2022-12-02 17:38:36.849788 patito-0.4.4/src/patito/duckdb.py
--rw-r--r--   0        0        0     1262 2022-12-02 17:38:36.849788 patito-0.4.4/src/patito/exceptions.py
--rw-r--r--   0        0        0    26850 2022-12-02 17:38:36.849788 patito-0.4.4/src/patito/polars.py
--rw-r--r--   0        0        0    55016 2022-12-02 17:38:36.849788 patito-0.4.4/src/patito/pydantic.py
--rw-r--r--   0        0        0     3263 2022-12-02 17:38:36.849788 patito-0.4.4/src/patito/sql.py
--rw-r--r--   0        0        0     8061 2022-12-02 17:38:36.849788 patito-0.4.4/src/patito/validators.py
--rw-r--r--   0        0        0    14525 1970-01-01 00:00:00.000000 patito-0.4.4/setup.py
--rw-r--r--   0        0        0    14551 1970-01-01 00:00:00.000000 patito-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1139 2023-06-21 23:24:02.891944 patito-0.5.0/LICENSE
+-rw-r--r--   0        0        0    12944 2023-06-21 23:24:02.891944 patito-0.5.0/README.md
+-rw-r--r--   0        0        0     3330 2023-06-21 23:24:02.895943 patito-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1169 2023-06-21 23:24:02.895943 patito-0.5.0/src/patito/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-21 23:24:02.895943 patito-0.5.0/src/patito/_docs.py
+-rw-r--r--   0        0        0    27917 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/database.py
+-rw-r--r--   0        0        0   111015 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/duckdb.py
+-rw-r--r--   0        0        0     1262 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/exceptions.py
+-rw-r--r--   0        0        0    26161 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/polars.py
+-rw-r--r--   0        0        0    54832 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/pydantic.py
+-rw-r--r--   0        0        0     3218 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/sql.py
+-rw-r--r--   0        0        0    10659 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/validators.py
+-rw-r--r--   0        0        0      686 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/xdg.py
+-rw-r--r--   0        0        0    14562 1970-01-01 00:00:00.000000 patito-0.5.0/PKG-INFO
```

### Comparing `patito-0.4.4/README.md` & `patito-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -245,15 +245,15 @@
 class Product(pt.Model):
     product_id: int = pt.Field(unique=True)
     name: str
 
     @property
     def url(self) -> str:
         return (
-            "https://oda.com/no/products/"
+            "https://example.com/no/products/"
             f"{self.product_id}-"
             f"{self.name.lower().replace(' ', '-')}"
         )
 ```
 
 The class can be instantiated from a single row of a data frame by using the `from_row()` method:
 
@@ -263,24 +263,24 @@
         "product_id": [1, 2],
         "name": ["Skimmed milk", "Eggs"],
     }
 )
 milk_row = products.filter(pl.col("product_id" == 1))
 milk = Product.from_row(milk_row)
 print(milk.url)
-# https://oda.com/no/products/1-skimmed-milk
+# https://example.com/no/products/1-skimmed-milk
 ```
 
 If you "connect" the `Product` model with the `DataFrame` by the use of `patito.DataFrame.set_model()`, or alternatively by using `Product.DataFrame` directly, you can use the `.get()` method in order to filter the data frame down to a single row _and_ cast it to the respective model class:
 
 ```py
 
 products = Product.DataFrame(
     {
         "product_id": [1, 2],
         "name": ["Skimmed milk", "Eggs"],
     }
 )
 milk = products.get(pl.col("product_id") == 1)
 print(milk.url)
-# https://oda.com/no/products/1-skimmed-milk
+# https://example.com/no/products/1-skimmed-milk
 ```
```

### Comparing `patito-0.4.4/pyproject.toml` & `patito-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 [tool.poetry]
 name = "patito"
-version = "0.4.4"
+version = "0.5.0"
 description = "A dataframe modelling library built on top of polars and pydantic."
 authors = ["Jakob Gerhard Martinussen <jakobgm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/patito"
 repository = "https://github.com/kolonialno/patito"
 documentation = "https://patito.readthedocs.io"
 keywords = ["validation", "dataframe"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 pydantic = ">=1.7.0"
-polars = ">=0.15.2"
+polars = ">=0.18.3"
 # Required for typing.Literal in python3.7
 typing-extensions = "*"
 pandas = {version = "*", optional = true, python = "^3.8"}
 duckdb = {version = ">=0.6.0", optional = true, python = "^3.8"}
 pyarrow = {version = ">=5.0.0", optional = true, python = "^3.8"}
-importlib-metadata = {version = "*", python = "<3.8"}
 # Optional docs dependencies
-Sphinx = {version = "*", optional = true}
+Sphinx = {version = "<7", optional = true}
 sphinx-rtd-theme = {version = "*", optional = true}
 sphinx-autobuild = {version = "*", optional = true}
 sphinx-autodoc-typehints = {version = "*", optional = true}
+sphinx-toolbox = {version = "*", optional = true}
 sphinxcontrib-mermaid = {version = "*", optional = true}
 
 [tool.poetry.extras]
+# The pyarrow.parquet module is required for writing parquet caches to disk
+caching = ["pyarrow"]
 duckdb = ["duckdb", "pyarrow"]
 pandas = ["pandas"]
-docs = ["Sphinx", "sphinx-rtd-theme", "sphinx-autobuild", "sphinx-autodoc-typehints", "sphinxcontrib-mermaid"]
+docs = [
+  "Sphinx",
+  "sphinx-autobuild",
+  "sphinx-autodoc-typehints",
+  "sphinx-rtd-theme",
+  "sphinx-toolbox",
+  "sphinxcontrib-mermaid",
+]
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = ">=22.3.0"
 coverage = {version = "*", extras = ["toml"]}
 flake8 = "3.9.2"
 flake8-annotations = "*"
 flake8-bandit = "*"
 flake8-black = "*"
 flake8-bugbear = "*"
@@ -76,15 +85,15 @@
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
   "if TYPE_CHECKING:",
   "if not _PANDAS_AVAILABLE:",
   "except ImportError:",
 ]
-fail_under = 100
+fail_under = 99.64
 show_missing = true
 
 [tool.isort]
 profile = "black"
 
 [tool.pyright]
 exclude = ["noxfile.py"]
```

### Comparing `patito-0.4.4/src/patito/__init__.py` & `patito-0.5.0/src/patito/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,43 +2,49 @@
 from polars import Expr, Series, col
 
 from patito import exceptions, sql
 from patito.exceptions import ValidationError
 from patito.polars import DataFrame, LazyFrame
 from patito.pydantic import Field, Model
 
+_CACHING_AVAILABLE = False
 _DUCKDB_AVAILABLE = False
 field = col("_")
 __all__ = [
     "DataFrame",
     "Expr",
     "Field",
     "LazyFrame",
     "Model",
     "Series",
     "ValidationError",
+    "_CACHING_AVAILABLE",
     "_DUCKDB_AVAILABLE",
     "col",
     "exceptions",
     "field",
     "sql",
 ]
 
 try:
-    from patito.duckdb import Database, Relation, RelationSource
+    from patito import duckdb
 
     _DUCKDB_AVAILABLE = True
-    __all__ += [
-        "Database",
-        "Relation",
-        "RelationSource",
-    ]
+    __all__ += ["duckdb"]
 except ImportError:  # pragma: no cover
     pass
 
+try:
+    from patito.database import Database
+
+    _CACHING_AVAILABLE = True
+    __all__ += ["Database"]
+except ImportError:
+    pass
+
 
 try:
     from importlib.metadata import PackageNotFoundError, version
 except ImportError:  # pragma: no cover
     from importlib_metadata import PackageNotFoundError, version  # type: ignore
 
 try:
```

### Comparing `patito-0.4.4/src/patito/duckdb.py` & `patito-0.5.0/src/patito/duckdb.py`

 * *Files 17% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 def create_pydantic_model(relation: "duckdb.DuckDBPyRelation") -> Type[Model]:
     """Create pydantic model deserialization of the given relation."""
     pydantic_annotations = {column: (Any, ...) for column in relation.columns}
     return create_model(  # type: ignore
         relation.alias,
         __base__=Model,
-        **pydantic_annotations,
+        **pydantic_annotations,  # pyright: ignore
     )
 
 
 def _enum_type_name(field_properties: dict) -> str:
     """
     Return enum DuckDB SQL type name based on enum values.
 
@@ -166,32 +166,32 @@
 
                 - A pandas or polars DataFrame.
                 - An SQL query represented as a string.
                 - A ``Path`` object pointing to a CSV or a parquet file.
                   The path must point to an existing file with either a ``.csv``
                   or ``.parquet`` file extension.
                 - A native DuckDB relation object (``duckdb.DuckDBPyRelation``).
-                - A ``patito.Relation`` object.
+                - A ``patito.duckdb.Relation`` object.
 
             database: Which database to load the relation into. If not provided,
                 the default DuckDB database will be used.
 
             model: Sub-class of ``patito.Model`` which specifies how to deserialize rows
-                when fetched with methods such as :ref:`Relation.get()<Relation.get>`
-                and ``__iter__()``.
+                when fetched with methods such as
+                :ref:`Relation.get()<duckdb.Relation.get>` and ``__iter__()``.
 
                 Will also be used to create a strict table schema if
-                :ref:`Relation.create_table()<Relation.create_table>`.
+                :ref:`Relation.create_table()<duckdb.Relation.create_table>`.
                 schema should be constructed.
 
-                If not provided, a dynamic model fitting the relation schema will be created
-                when required.
+                If not provided, a dynamic model fitting the relation schema will be
+                created when required.
 
                 Can also be set later dynamically by invoking
-                :ref:`Relation.set_model()<Relation.set_model>`.
+                :ref:`Relation.set_model()<duckdb.Relation.set_model>`.
 
         Raises:
             ValueError: If any one of the following cases are encountered:
 
                 - If a provided ``Path`` object does not have a ``.csv`` or
                   ``.parquet`` file extension.
                 - If a database and relation object is provided, but the relation object
@@ -200,27 +200,27 @@
             TypeError: If the type of ``derived_from`` is not supported.
 
         Examples:
             Instantiated from a dataframe:
 
             >>> import patito as pt
             >>> df = pt.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
-            >>> pt.Relation(df).filter("a > 2").to_df()
+            >>> pt.duckdb.Relation(df).filter("a > 2").to_df()
             shape: (1, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
             │ 3   ┆ 6   │
             └─────┴─────┘
 
             Instantiated from an SQL query:
 
-            >>> pt.Relation("select 1 as a, 2 as b").to_df()
+            >>> pt.duckdb.Relation("select 1 as a, 2 as b").to_df()
             shape: (1, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
             │ 1   ┆ 2   │
@@ -292,30 +292,29 @@
                 ``"sum(column_name) as my_column"`` in the executed SQL query.
             group_by: A single column name or iterable collection of column names to
                 group by.
 
         Examples:
             >>> import patito as pt
             >>> df = pt.DataFrame({"a": [1, 2, 3], "b": ["X", "Y", "X"]})
-            >>> relation = pt.Relation(df)
+            >>> relation = pt.duckdb.Relation(df)
             >>> relation.aggregate(
             ...     "b",
             ...     "sum(a)",
             ...     "greatest(b)",
             ...     max_a="max(a)",
             ...     group_by="b",
             ... ).to_df()
             shape: (2, 4)
             ┌─────┬────────┬─────────────┬───────┐
             │ b   ┆ sum(a) ┆ greatest(b) ┆ max_a │
             │ --- ┆ ---    ┆ ---         ┆ ---   │
             │ str ┆ f64    ┆ str         ┆ i64   │
             ╞═════╪════════╪═════════════╪═══════╡
             │ X   ┆ 4.0    ┆ X           ┆ 3     │
-            ├╌╌╌╌╌┼╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌┤
             │ Y   ┆ 2.0    ┆ Y           ┆ 2     │
             └─────┴────────┴─────────────┴───────┘
         """
         expression = ", ".join(
             aggregations
             + tuple(
                 f"{expression} as {column_name}"
@@ -343,15 +342,15 @@
             exclude: If provided, the given columns will `not` be renamed.
 
         Raises:
             TypeError: If both include `and` exclude are provided at the same time.
 
         Examples:
             >>> import patito as pt
-            >>> relation = pt.Relation("select 1 as column_1, 2 as column_2")
+            >>> relation = pt.duckdb.Relation("select 1 as column_1, 2 as column_2")
             >>> relation.add_suffix("_renamed").to_df()
             shape: (1, 2)
             ┌──────────────────┬──────────────────┐
             │ column_1_renamed ┆ column_2_renamed │
             │ ---              ┆ ---              │
             │ i64              ┆ i64              │
             ╞══════════════════╪══════════════════╡
@@ -409,15 +408,15 @@
             exclude: If provided, the given columns will `not` be renamed.
 
         Raises:
             TypeError: If both include `and` exclude are provided at the same time.
 
         Examples:
             >>> import patito as pt
-            >>> relation = pt.Relation("select 1 as column_1, 2 as column_2")
+            >>> relation = pt.duckdb.Relation("select 1 as column_1, 2 as column_2")
             >>> relation.add_prefix("renamed_").to_df()
             shape: (1, 2)
             ┌──────────────────┬──────────────────┐
             │ renamed_column_1 ┆ renamed_column_2 │
             │ ---              ┆ ---              │
             │ i64              ┆ i64              │
             ╞══════════════════╪══════════════════╡
@@ -460,31 +459,31 @@
             )
         )
 
     def all(self, *filters: str, **equalities: Union[int, float, str]) -> bool:
         """
         Return ``True`` if the given predicate(s) are true for all rows in the relation.
 
-        See :ref:`Relation.filter()<Relation.filter>` for additional information
-        regarding the parameters.
+        See :func:`Relation.filter()` for additional information regarding the
+        parameters.
 
         Args:
             filters: SQL predicates to satisfy.
             equalities: SQL equality predicates to satisfy.
 
         Examples:
             >>> import patito as pt
             >>> df = pt.DataFrame(
             ...     {
             ...         "even_number": [2, 4, 6],
             ...         "odd_number": [1, 3, 5],
             ...         "zero": [0, 0, 0],
             ...     }
             ... )
-            >>> relation = pt.Relation(df)
+            >>> relation = pt.duckdb.Relation(df)
             >>> relation.all(zero=0)
             True
             >>> relation.all(
             ...     "even_number % 2 = 0",
             ...     "odd_number % 2 = 1",
             ...     zero=0,
             ... )
@@ -516,30 +515,29 @@
                 value.
             default: Default output value for inputs which have no provided mapping.
 
         Examples:
             The following case statement...
 
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> relation = db.to_relation("select 1 as a union select 2 as a")
             >>> relation.case(
             ...     from_column="a",
             ...     to_column="b",
             ...     mapping={1: "one", 2: "two"},
             ...     default="three",
             ... ).order(by="a").to_df()
             shape: (2, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ str │
             ╞═════╪═════╡
             │ 1   ┆ one │
-            ├╌╌╌╌╌┼╌╌╌╌╌┤
             │ 2   ┆ two │
             └─────┴─────┘
 
             ... is equivalent with:
 
             >>> case_statement = pt.sql.Case(
             ...     on_column="a",
@@ -551,15 +549,14 @@
             shape: (2, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ str │
             ╞═════╪═════╡
             │ 1   ┆ one │
-            ├╌╌╌╌╌┼╌╌╌╌╌┤
             │ 2   ┆ two │
             └─────┴─────┘
         """
 
         case_statement = sql.Case(
             on_column=from_column,
             mapping=mapping,
@@ -576,23 +573,23 @@
         include: Optional[Collection[str]] = None,
         exclude: Optional[Collection[str]] = None,
     ) -> RelationType:
         """
         Cast the columns of the relation to types compatible with the associated model.
 
         The associated model must either be set by invoking
-        :ref:`Relation.set_model() <Relation.set_model>` or provided with the ``model``
-        parameter.
+        :ref:`Relation.set_model() <duckdb.Relation.set_model>` or provided with the
+        ``model`` parameter.
 
         Any columns of the relation that are not part of the given model schema will be
         left as-is.
 
         Args:
-            model: If :ref:`Relation.set_model() <Relation.set_model>` has not been
-                invoked or is intended to be overwritten.
+            model: If :ref:`Relation.set_model() <duckdb.Relation.set_model>` has not
+                been invoked or is intended to be overwritten.
             strict: If set to ``False``, columns which are technically compliant with
                 the specified field type, will not be casted. For example, a column
                 annotated with ``int`` is technically compliant with ``SMALLINT``, even
                 if ``INTEGER`` is the default SQL type associated with ``int``-annotated
                 fields. If ``strict`` is set to ``True``, the resulting dtypes will
                 be forced to the default dtype associated with each python type.
             include: If provided, only the given columns will be casted.
@@ -603,39 +600,39 @@
             schema.
 
         Examples:
             >>> import patito as pt
             >>> class Schema(pt.Model):
             ...     float_column: float
             ...
-            >>> relation = pt.Relation("select 1 as float_column")
+            >>> relation = pt.duckdb.Relation("select 1 as float_column")
             >>> relation.types["float_column"]
-            'INTEGER'
+            INTEGER
             >>> relation.cast(model=Schema).types["float_column"]
-            'DOUBLE'
+            DOUBLE
 
-            >>> relation = pt.Relation("select 1::FLOAT as float_column")
+            >>> relation = pt.duckdb.Relation("select 1::FLOAT as float_column")
             >>> relation.cast(model=Schema).types["float_column"]
-            'FLOAT'
+            FLOAT
             >>> relation.cast(model=Schema, strict=True).types["float_column"]
-            'DOUBLE'
+            DOUBLE
 
             >>> class Schema(pt.Model):
             ...     column_1: float
             ...     column_2: float
             ...
-            >>> relation = pt.Relation("select 1 as column_1, 2 as column_2").set_model(
-            ...     Schema
-            ... )
+            >>> relation = pt.duckdb.Relation(
+            ...     "select 1 as column_1, 2 as column_2"
+            ... ).set_model(Schema)
             >>> relation.types
-            {'column_1': 'INTEGER', 'column_2': 'INTEGER'}
+            {'column_1': INTEGER, 'column_2': INTEGER}
             >>> relation.cast(include=["column_1"]).types
-            {'column_1': 'DOUBLE', 'column_2': 'INTEGER'}
+            {'column_1': DOUBLE, 'column_2': INTEGER}
             >>> relation.cast(exclude=["column_1"]).types
-            {'column_1': 'INTEGER', 'column_2': 'DOUBLE'}
+            {'column_1': INTEGER, 'column_2': DOUBLE}
         """
         if model is not None:
             relation = self.set_model(model)
             schema = model
         elif self.model is not None:
             relation = self
             schema = cast(ModelType, self.model)
@@ -646,15 +643,16 @@
                 f"{class_name}.model having been set! "
                 f"You should invoke {class_name}.set_model() first "
                 "or explicitly provide a model to .cast()."
             )
 
         if include is not None and exclude is not None:
             raise ValueError(
-                f"Both include and exclude provided to {self.__class__.__name__}.cast()!"
+                "Both include and exclude provided to "
+                f"{self.__class__.__name__}.cast()!"
             )
         elif include is not None:
             include = set(include)
         elif exclude is not None:
             include = set(relation.columns) - set(exclude)
         else:
             include = set(relation.columns)
@@ -697,26 +695,24 @@
             >>> df = pt.DataFrame(
             ...     {
             ...         "a": [1, None, 3],
             ...         "b": ["four", "five", None],
             ...         "c": [None, 8.0, 9.0],
             ...     }
             ... )
-            >>> relation = pt.Relation(df)
+            >>> relation = pt.duckdb.Relation(df)
             >>> relation.coalesce(a=2, b="six").to_df()
             shape: (3, 3)
             ┌─────┬──────┬──────┐
             │ a   ┆ b    ┆ c    │
             │ --- ┆ ---  ┆ ---  │
             │ i64 ┆ str  ┆ f64  │
             ╞═════╪══════╪══════╡
             │ 1   ┆ four ┆ null │
-            ├╌╌╌╌╌┼╌╌╌╌╌╌┼╌╌╌╌╌╌┤
             │ 2   ┆ five ┆ 8.0  │
-            ├╌╌╌╌╌┼╌╌╌╌╌╌┼╌╌╌╌╌╌┤
             │ 3   ┆ six  ┆ 9.0  │
             └─────┴──────┴──────┘
         """
         projections = []
         for column in self.columns:
             if column in column_expressions:
                 expression = column_expressions[column]
@@ -728,15 +724,15 @@
     @property
     def columns(self) -> List[str]:
         """
         Return the columns of the relation as a list of strings.
 
         Examples:
             >>> import patito as pt
-            >>> pt.Relation("select 1 as a, 2 as b").columns
+            >>> pt.duckdb.Relation("select 1 as a, 2 as b").columns
             ['a', 'b']
         """
         # Under certain specific circumstances columns are suffixed with
         # :1, which need to be removed from the column name.
         return [column.partition(":")[0] for column in self._relation.columns]
 
     def count(self) -> int:
@@ -744,55 +740,56 @@
         Return the number of rows in the given relation.
 
         Returns:
             Number of rows in the relation as an integer.
 
         Examples:
             >>> import patito as pt
-            >>> relation = pt.Relation("select 1 as a")
+            >>> relation = pt.duckdb.Relation("select 1 as a")
             >>> relation.count()
             1
             >>> (relation + relation).count()
             2
 
-            The :ref:`Relation.__len__()<Relation.__len__>` method invokes
+            The :ref:`Relation.__len__()<duckdb.Relation.__len__>` method invokes
             ``Relation.count()`` under the hood, and is equivalent:
 
             >>> len(relation)
             1
             >>> len(relation + relation)
             2
         """
         return cast(Tuple[int], self._relation.aggregate("count(*)").fetchone())[0]
 
     def create_table(self: RelationType, name: str) -> RelationType:
         """
         Create new database table based on relation.
 
-        If ``self.model`` is set with :ref:`Relation.set_model()<Relation.set_model>`,
-        then the model is used to infer the table schema.
-        Otherwise, a permissive table schema is created based on the relation data.
+        If ``self.model`` is set with
+        :ref:`Relation.set_model()<duckdb.Relation.set_model>`, then the model is used
+        to infer the table schema. Otherwise, a permissive table schema is created based
+        on the relation data.
 
         Returns:
             Relation: A relation pointing to the newly created table.
 
         Examples:
             >>> from typing import Literal
             >>> import patito as pt
 
             >>> df = pt.DataFrame({"enum_column": ["A", "A", "B"]})
-            >>> relation = pt.Relation(df)
+            >>> relation = pt.duckdb.Relation(df)
             >>> relation.create_table("permissive_table").types
-            {'enum_column': 'VARCHAR'}
+            {'enum_column': VARCHAR}
 
             >>> class TableSchema(pt.Model):
             ...     enum_column: Literal["A", "B", "C"]
             ...
             >>> relation.set_model(TableSchema).create_table("strict_table").types
-            {'enum_column': 'enum__7ba49365cc1b0fd57e61088b3bc9aa25'}
+            {'enum_column': enum__7ba49365cc1b0fd57e61088b3bc9aa25}
         """
         if self.model is not None:
             self.database.create_table(name=name, model=self.model)
             self.insert_into(table=name)
         else:
             self._relation.create(table_name=name)
         return cast(RelationType, self.database.table(name))
@@ -806,29 +803,27 @@
         Create new database view based on relation.
 
         Returns:
             Relation: A relation pointing to the newly created view.
 
         Examples:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> df = pt.DataFrame({"column": ["A", "A", "B"]})
             >>> relation = db.to_relation(df)
             >>> relation.create_view("my_view")
             >>> db.query("select * from my_view").to_df()
             shape: (3, 1)
             ┌────────┐
             │ column │
             │ ---    │
             │ str    │
             ╞════════╡
             │ A      │
-            ├╌╌╌╌╌╌╌╌┤
             │ A      │
-            ├╌╌╌╌╌╌╌╌┤
             │ B      │
             └────────┘
         """
         self._relation.create_view(view_name=name, replace=replace)
         return cast(RelationType, self.database.view(name))
 
     def drop(self, *columns: str) -> Relation:
@@ -836,15 +831,15 @@
         Remove specified column(s) from relation.
 
         Args:
             columns (str): Any number of string column names to be dropped.
 
         Examples:
             >>> import patito as pt
-            >>> relation = pt.Relation("select 1 as a, 2 as b, 3 as c")
+            >>> relation = pt.duckdb.Relation("select 1 as a, 2 as b, 3 as c")
             >>> relation.columns
             ['a', 'b', 'c']
             >>> relation.drop("c").columns
             ['a', 'b']
             >>> relation.drop("b", "c").columns
             ['a']
         """
@@ -857,40 +852,37 @@
         """
         Drop all duplicate rows of the relation.
 
         Example:
             >>> import patito as pt
             >>> df = pt.DataFrame(
             ...     [[1, 2, 3], [1, 2, 3], [3, 2, 1]],
-            ...     columns=["a", "b", "c"],
+            ...     schema=["a", "b", "c"],
             ...     orient="row",
             ... )
-            >>> relation = pt.Relation(df)
+            >>> relation = pt.duckdb.Relation(df)
             >>> relation.to_df()
             shape: (3, 3)
             ┌─────┬─────┬─────┐
             │ a   ┆ b   ┆ c   │
             │ --- ┆ --- ┆ --- │
             │ i64 ┆ i64 ┆ i64 │
             ╞═════╪═════╪═════╡
             │ 1   ┆ 2   ┆ 3   │
-            ├╌╌╌╌╌┼╌╌╌╌╌┼╌╌╌╌╌┤
             │ 1   ┆ 2   ┆ 3   │
-            ├╌╌╌╌╌┼╌╌╌╌╌┼╌╌╌╌╌┤
             │ 3   ┆ 2   ┆ 1   │
             └─────┴─────┴─────┘
             >>> relation.distinct().to_df()
             shape: (2, 3)
             ┌─────┬─────┬─────┐
             │ a   ┆ b   ┆ c   │
             │ --- ┆ --- ┆ --- │
             │ i64 ┆ i64 ┆ i64 │
             ╞═════╪═════╪═════╡
             │ 1   ┆ 2   ┆ 3   │
-            ├╌╌╌╌╌┼╌╌╌╌╌┼╌╌╌╌╌┤
             │ 3   ┆ 2   ┆ 1   │
             └─────┴─────┴─────┘
         """
         return self._wrap(self._relation.distinct(), schema_change=False)
 
     def except_(self: RelationType, other: RelationSource) -> RelationType:
         """
@@ -900,29 +892,29 @@
             other: Another relation or something that can be casted to a relation.
 
         Returns:
             New relation without the rows that can be found in the other relation.
 
         Example:
             >>> import patito as pt
-            >>> relation_123 = pt.Relation("select 1 union select 2 union select 3")
+            >>> relation_123 = pt.duckdb.Relation(
+            ...     "select 1 union select 2 union select 3"
+            ... )
             >>> relation_123.order(by="1").to_df()
             shape: (3, 1)
             ┌─────┐
             │ 1   │
             │ --- │
             │ i64 │
             ╞═════╡
             │ 1   │
-            ├╌╌╌╌╌┤
             │ 2   │
-            ├╌╌╌╌╌┤
             │ 3   │
             └─────┘
-            >>> relation_2 = pt.Relation("select 2")
+            >>> relation_2 = pt.duckdb.Relation("select 2")
             >>> relation_2.to_df()
             shape: (1, 1)
             ┌─────┐
             │ 2   │
             │ --- │
             │ i64 │
             ╞═════╡
@@ -932,37 +924,36 @@
             shape: (2, 1)
             ┌─────┐
             │ 1   │
             │ --- │
             │ i64 │
             ╞═════╡
             │ 1   │
-            ├╌╌╌╌╌┤
             │ 3   │
             └─────┘
         """
         return self._wrap(
             self._relation.except_(self.database.to_relation(other)._relation),
             schema_change=False,
         )
 
-    def execute(self) -> duckdb.DuckDBPyResult:
+    def execute(self) -> duckdb.DuckDBPyRelation:
         """
         Execute built relation query and return result object.
 
         Returns:
             A native ``duckdb.DuckDBPyResult`` object representing the executed query.
 
         Examples:
             >>> import patito as pt
-            >>> relation = pt.Relation(
+            >>> relation = pt.duckdb.Relation(
             ...     "select 1 as a, 2 as b union select 3 as a, 4 as b"
             ... )
             >>> result = relation.aggregate("sum(a)", group_by="").execute()
-            >>> result.description()
+            >>> result.description
             [('sum(a)', 'NUMBER', None, None, None, None, None)]
             >>> result.fetchall()
             [(4,)]
         """
         # A star-select is here performed in order to work around certain DuckDB bugs
         return self._relation.project("*").execute()
 
@@ -985,25 +976,25 @@
         Returns:
             Model: A Patito model representing the given row.
 
         Examples:
             >>> import patito as pt
             >>> import polars as pl
             >>> df = pt.DataFrame({"product_id": [1, 2, 3], "price": [10, 10, 20]})
-            >>> relation = pt.Relation(df).set_alias("my_relation")
+            >>> relation = pt.duckdb.Relation(df).set_alias("my_relation")
 
             The ``.get()`` method will by default return a dynamically constructed
             Patito model if no model has been associated with the given relation:
 
             >>> relation.get(product_id=1)
             my_relation(product_id=1, price=10)
 
             If a Patito model has been associated with the relation, by the use of
-            :ref:`Relation.set_model()<Relation.set_model>`, then the given model will
-            be used to represent the return type:
+            :ref:`Relation.set_model()<duckdb.Relation.set_model>`, then the given model
+            will be used to represent the return type:
 
             >>> class Product(pt.Model):
             ...     product_id: int = pt.Field(unique=True)
             ...     price: float
             ...
             >>> relation.set_model(Product).get(product_id=1)
             Product(product_id=1, price=10.0)
@@ -1035,15 +1026,15 @@
             Relation.get(price=0) returned 0 rows!
         """
         if filters or equalities:
             relation = self.filter(*filters, **equalities)
         else:
             relation = self
         result = relation.execute()
-        row = cast(tuple, result.fetchone())
+        row = result.fetchone()
         if row is None or result.fetchone() is not None:
             args = [repr(f) for f in filters]
             args.extend(f"{key}={value!r}" for key, value in equalities.items())
             args_string = ",".join(args)
 
             num_rows = relation.count()
             if num_rows == 0:
@@ -1095,24 +1086,23 @@
             >>> import patito as pt
             >>> df = pt.DataFrame(
             ...     {
             ...         "number": [1, 2, 3, 4],
             ...         "string": ["A", "A", "B", "B"],
             ...     }
             ... )
-            >>> relation = pt.Relation(df)
+            >>> relation = pt.duckdb.Relation(df)
             >>> relation.filter("number % 2 = 0").to_df()
             shape: (2, 2)
             ┌────────┬────────┐
             │ number ┆ string │
             │ ---    ┆ ---    │
             │ i64    ┆ str    │
             ╞════════╪════════╡
             │ 2      ┆ A      │
-            ├╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┤
             │ 4      ┆ B      │
             └────────┴────────┘
 
             >>> relation.filter(number=1, string="A").to_df()
             shape: (1, 2)
             ┌────────┬────────┐
             │ number ┆ string │
@@ -1139,16 +1129,16 @@
         *,
         on: str,
         how: Literal["inner", "left"] = "inner",
     ) -> RelationType:
         """
         Join relation with other relation source based on condition.
 
-        See :ref:`Relation.inner_join() <Relation.inner_join>` and
-        :ref:`Relation.left_join() <Relation.left_join>` for alternative method
+        See :ref:`duckdb.Relation.inner_join() <duckdb.Relation.inner_join>` and
+        :ref:`Relation.left_join() <duckdb.Relation.left_join>` for alternative method
         shortcuts instead of using ``how``.
 
         Args:
             other: A source which can be casted to a ``Relation`` object, and be used
                 as the right table in the join.
             on: Join condition following the ``INNER JOIN ... ON`` in the SQL query.
             how: Either ``"left"`` or ``"inner"`` for what type of SQL join operation to
@@ -1161,35 +1151,34 @@
             >>> import patito as pt
             >>> products_df = pt.DataFrame(
             ...     {
             ...         "product_name": ["apple", "banana", "oranges"],
             ...         "supplier_id": [2, 1, 3],
             ...     }
             ... )
-            >>> products = pt.Relation(products_df)
+            >>> products = pt.duckdb.Relation(products_df)
             >>> supplier_df = pt.DataFrame(
             ...     {
             ...         "id": [1, 2],
             ...         "supplier_name": ["Banana Republic", "Applies Inc."],
             ...     }
             ... )
-            >>> suppliers = pt.Relation(supplier_df)
+            >>> suppliers = pt.duckdb.Relation(supplier_df)
             >>> products.set_alias("p").join(
             ...     suppliers.set_alias("s"),
             ...     on="p.supplier_id = s.id",
             ...     how="inner",
             ... ).to_df()
             shape: (2, 4)
             ┌──────────────┬─────────────┬─────┬─────────────────┐
             │ product_name ┆ supplier_id ┆ id  ┆ supplier_name   │
             │ ---          ┆ ---         ┆ --- ┆ ---             │
             │ str          ┆ i64         ┆ i64 ┆ str             │
             ╞══════════════╪═════════════╪═════╪═════════════════╡
             │ apple        ┆ 2           ┆ 2   ┆ Applies Inc.    │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ banana       ┆ 1           ┆ 1   ┆ Banana Republic │
             └──────────────┴─────────────┴─────┴─────────────────┘
 
             >>> products.set_alias("p").join(
             ...     suppliers.set_alias("s"),
             ...     on="p.supplier_id = s.id",
             ...     how="left",
@@ -1197,17 +1186,15 @@
             shape: (3, 4)
             ┌──────────────┬─────────────┬──────┬─────────────────┐
             │ product_name ┆ supplier_id ┆ id   ┆ supplier_name   │
             │ ---          ┆ ---         ┆ ---  ┆ ---             │
             │ str          ┆ i64         ┆ i64  ┆ str             │
             ╞══════════════╪═════════════╪══════╪═════════════════╡
             │ apple        ┆ 2           ┆ 2    ┆ Applies Inc.    │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ banana       ┆ 1           ┆ 1    ┆ Banana Republic │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ oranges      ┆ 3           ┆ null ┆ null            │
             └──────────────┴─────────────┴──────┴─────────────────┘
         """
         return self._wrap(
             self._relation.join(
                 self.database.to_relation(other)._relation, condition=on, how=how
             ),
@@ -1230,34 +1217,33 @@
             >>> import patito as pt
             >>> products_df = pt.DataFrame(
             ...     {
             ...         "product_name": ["apple", "banana", "oranges"],
             ...         "supplier_id": [2, 1, 3],
             ...     }
             ... )
-            >>> products = pt.Relation(products_df)
+            >>> products = pt.duckdb.Relation(products_df)
             >>> supplier_df = pt.DataFrame(
             ...     {
             ...         "id": [1, 2],
             ...         "supplier_name": ["Banana Republic", "Applies Inc."],
             ...     }
             ... )
-            >>> suppliers = pt.Relation(supplier_df)
+            >>> suppliers = pt.duckdb.Relation(supplier_df)
             >>> products.set_alias("p").inner_join(
             ...     suppliers.set_alias("s"),
             ...     on="p.supplier_id = s.id",
             ... ).to_df()
             shape: (2, 4)
             ┌──────────────┬─────────────┬─────┬─────────────────┐
             │ product_name ┆ supplier_id ┆ id  ┆ supplier_name   │
             │ ---          ┆ ---         ┆ --- ┆ ---             │
             │ str          ┆ i64         ┆ i64 ┆ str             │
             ╞══════════════╪═════════════╪═════╪═════════════════╡
             │ apple        ┆ 2           ┆ 2   ┆ Applies Inc.    │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ banana       ┆ 1           ┆ 1   ┆ Banana Republic │
             └──────────────┴─────────────┴─────┴─────────────────┘
         """
         return self._wrap(
             self._relation.join(
                 other_rel=self.database.to_relation(other)._relation,
                 condition=on,
@@ -1282,36 +1268,34 @@
             >>> import patito as pt
             >>> products_df = pt.DataFrame(
             ...     {
             ...         "product_name": ["apple", "banana", "oranges"],
             ...         "supplier_id": [2, 1, 3],
             ...     }
             ... )
-            >>> products = pt.Relation(products_df)
+            >>> products = pt.duckdb.Relation(products_df)
             >>> supplier_df = pt.DataFrame(
             ...     {
             ...         "id": [1, 2],
             ...         "supplier_name": ["Banana Republic", "Applies Inc."],
             ...     }
             ... )
-            >>> suppliers = pt.Relation(supplier_df)
+            >>> suppliers = pt.duckdb.Relation(supplier_df)
             >>> products.set_alias("p").left_join(
             ...     suppliers.set_alias("s"),
             ...     on="p.supplier_id = s.id",
             ... ).to_df()
             shape: (3, 4)
             ┌──────────────┬─────────────┬──────┬─────────────────┐
             │ product_name ┆ supplier_id ┆ id   ┆ supplier_name   │
             │ ---          ┆ ---         ┆ ---  ┆ ---             │
             │ str          ┆ i64         ┆ i64  ┆ str             │
             ╞══════════════╪═════════════╪══════╪═════════════════╡
             │ apple        ┆ 2           ┆ 2    ┆ Applies Inc.    │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ banana       ┆ 1           ┆ 1    ┆ Banana Republic │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ oranges      ┆ 3           ┆ null ┆ null            │
             └──────────────┴─────────────┴──────┴─────────────────┘
         """
         return self._wrap(
             self._relation.join(
                 other_rel=self.database.to_relation(other)._relation,
                 condition=on,
@@ -1331,39 +1315,37 @@
 
         Returns:
             New relation with only n rows.
 
         Example:
             >>> import patito as pt
             >>> relation = (
-            ...     pt.Relation("select 1 as column")
-            ...     + pt.Relation("select 2 as column")
-            ...     + pt.Relation("select 3 as column")
-            ...     + pt.Relation("select 4 as column")
+            ...     pt.duckdb.Relation("select 1 as column")
+            ...     + pt.duckdb.Relation("select 2 as column")
+            ...     + pt.duckdb.Relation("select 3 as column")
+            ...     + pt.duckdb.Relation("select 4 as column")
             ... )
             >>> relation.limit(2).to_df()
             shape: (2, 1)
             ┌────────┐
             │ column │
             │ ---    │
             │ i64    │
             ╞════════╡
             │ 1      │
-            ├╌╌╌╌╌╌╌╌┤
             │ 2      │
             └────────┘
             >>> relation.limit(2, offset=2).to_df()
             shape: (2, 1)
             ┌────────┐
             │ column │
             │ ---    │
             │ i64    │
             ╞════════╡
             │ 3      │
-            ├╌╌╌╌╌╌╌╌┤
             │ 4      │
             └────────┘
         """
         return self._wrap(self._relation.limit(n=n, offset=offset), schema_change=False)
 
     def order(self: RelationType, by: Union[str, Iterable[str]]) -> RelationType:
         """
@@ -1388,50 +1370,41 @@
             shape: (4, 2)
             ┌─────────┬─────┐
             │ name    ┆ age │
             │ ---     ┆ --- │
             │ str     ┆ i64 │
             ╞═════════╪═════╡
             │ Alice   ┆ 20  │
-            ├╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┤
             │ Bob     ┆ 20  │
-            ├╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┤
             │ Charles ┆ 30  │
-            ├╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┤
             │ Diana   ┆ 35  │
             └─────────┴─────┘
-            >>> relation = pt.Relation(df)
+            >>> relation = pt.duckdb.Relation(df)
             >>> relation.order(by="age desc").to_df()
             shape: (4, 2)
             ┌─────────┬─────┐
             │ name    ┆ age │
             │ ---     ┆ --- │
             │ str     ┆ i64 │
             ╞═════════╪═════╡
             │ Diana   ┆ 35  │
-            ├╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┤
             │ Charles ┆ 30  │
-            ├╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┤
             │ Alice   ┆ 20  │
-            ├╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┤
             │ Bob     ┆ 20  │
             └─────────┴─────┘
             >>> relation.order(by=["age desc", "name desc"]).to_df()
             shape: (4, 2)
             ┌─────────┬─────┐
             │ name    ┆ age │
             │ ---     ┆ --- │
             │ str     ┆ i64 │
             ╞═════════╪═════╡
             │ Diana   ┆ 35  │
-            ├╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┤
             │ Charles ┆ 30  │
-            ├╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┤
             │ Bob     ┆ 20  │
-            ├╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌┤
             │ Alice   ┆ 20  │
             └─────────┴─────┘
         """
         order_expr = by if isinstance(by, str) else ", ".join(by)
         return self._wrap(
             self._relation.order(order_expr=order_expr),
             schema_change=False,
@@ -1452,15 +1425,15 @@
             table: Name of table for which to insert values into.
 
         Returns:
             Relation: The original relation, i.e. ``self``.
 
         Examples:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> db.to_relation("select 1 as a").create_table("my_table")
             >>> db.table("my_table").to_df()
             shape: (1, 1)
             ┌─────┐
             │ a   │
             │ --- │
             │ i64 │
@@ -1472,15 +1445,14 @@
             shape: (2, 1)
             ┌─────┐
             │ a   │
             │ --- │
             │ i64 │
             ╞═════╡
             │ 1   │
-            ├╌╌╌╌╌┤
             │ 2   │
             └─────┘
         """
         table_relation = self.database.table(table)
         missing_columns = set(table_relation.columns) - set(self.columns)
         if missing_columns:
             raise TypeError(
@@ -1505,15 +1477,15 @@
             Relation[Model]: A new relation with only those rows that are present in
             both relations.
 
         Example:
             >>> import patito as pt
             >>> df1 = pt.DataFrame({"a": [1, 1, 2], "b": [1, 1, 2]})
             >>> df2 = pt.DataFrame({"a": [1, 1, 3], "b": [1, 1, 3]})
-            >>> pt.Relation(df1).intersect(pt.Relation(df2)).to_df()
+            >>> pt.duckdb.Relation(df1).intersect(pt.duckdb.Relation(df2)).to_df()
             shape: (1, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
             │ 1   ┆ 1   │
@@ -1542,40 +1514,36 @@
             **named_projections: One ore more keyword arguments where the keyword
                 specifies the name of the new column and the value is an SQL statement
                 defining the content of the new column. For example
                 ``new_column="2 * another_column"``.
 
         Examples:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> relation = db.to_relation(pt.DataFrame({"original_column": [1, 2, 3]}))
             >>> relation.select("*").to_df()
             shape: (3, 1)
             ┌─────────────────┐
             │ original_column │
             │ ---             │
             │ i64             │
             ╞═════════════════╡
             │ 1               │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ 2               │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ 3               │
             └─────────────────┘
             >>> relation.select("*", multiplied_column="2 * original_column").to_df()
             shape: (3, 2)
             ┌─────────────────┬───────────────────┐
             │ original_column ┆ multiplied_column │
             │ ---             ┆ ---               │
             │ i64             ┆ i64               │
             ╞═════════════════╪═══════════════════╡
             │ 1               ┆ 2                 │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ 2               ┆ 4                 │
-            ├╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ 3               ┆ 6                 │
             └─────────────────┴───────────────────┘
         """
         # We expand '*' to an explicit list of columns in order to support redefining
         # columns within the star expressed columns.
         expanded_projections: list = list(projections)
         try:
@@ -1620,15 +1588,15 @@
 
         Raises:
             ValueError: If any of the given keywords do not exist as columns in the
                 relation.
 
         Examples:
             >>> import patito as pt
-            >>> relation = pt.Relation("select 1 as a, 2 as b")
+            >>> relation = pt.duckdb.Relation("select 1 as a, 2 as b")
             >>> relation.rename(b="c").to_df().select(["a", "c"])
             shape: (1, 2)
             ┌─────┬─────┐
             │ a   ┆ c   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
@@ -1662,16 +1630,16 @@
 
         Returns:
             Relation: A new relation containing the same query but addressable with the
             new alias.
 
         Example:
             >>> import patito as pt
-            >>> relation_1 = pt.Relation("select 1 as a, 2 as b")
-            >>> relation_2 = pt.Relation("select 1 as a, 3 as c")
+            >>> relation_1 = pt.duckdb.Relation("select 1 as a, 2 as b")
+            >>> relation_2 = pt.duckdb.Relation("select 1 as a, 3 as c")
             >>> relation_1.set_alias("x").inner_join(
             ...     relation_2.set_alias("y"),
             ...     on="x.a = y.a",
             ... ).select("x.a", "y.a", "b", "c").to_df()
             shape: (1, 4)
             ┌─────┬─────┬─────┬─────┐
             │ a   ┆ a:1 ┆ b   ┆ c   │
@@ -1687,41 +1655,43 @@
         )
 
     def set_model(self, model):  # type: ignore[no-untyped-def] # noqa: ANN
         """
         Associate a give Patito model with the relation.
 
         The returned relation has an associated ``.model`` attribute which can in turn
-        be used by several methods such as :ref:`Relation.get()<Relation.get>`,
-        :ref:`Relation.create_table()<Relation.create_table>`, and
-        :ref:`Relation.__iter__<Relation.__iter__>`.
+        be used by several methods such as :ref:`Relation.get()<duckdb.Relation.get>`,
+        :ref:`Relation.create_table()<duckdb.Relation.create_table>`, and
+        :ref:`Relation.__iter__<duckdb.Relation.__iter__>`.
 
         Args:
             model: A Patito Model class specifying the intended schema of the relation.
 
         Returns:
             Relation[model]: A new relation with the associated model.
 
         Example:
             >>> from typing import Literal
             >>> import patito as pt
             >>> class MySchema(pt.Model):
             ...     float_column: float
             ...     enum_column: Literal["A", "B", "C"]
             ...
-            >>> relation = pt.Relation("select 1 as float_column, 'A' as enum_column")
+            >>> relation = pt.duckdb.Relation(
+            ...     "select 1 as float_column, 'A' as enum_column"
+            ... )
             >>> relation.get()
             query_relation(float_column=1, enum_column='A')
             >>> relation.set_model(MySchema).get()
             MySchema(float_column=1.0, enum_column='A')
             >>> relation.create_table("unmodeled_table").types
-            {'float_column': 'INTEGER', 'enum_column': 'VARCHAR'}
+            {'float_column': INTEGER, 'enum_column': VARCHAR}
             >>> relation.set_model(MySchema).create_table("modeled_table").types
-            {'float_column': 'DOUBLE',
-             'enum_column': 'enum__7ba49365cc1b0fd57e61088b3bc9aa25'}
+            {'float_column': DOUBLE,
+             'enum_column': enum__7ba49365cc1b0fd57e61088b3bc9aa25}
         """
         # We are not able to annotate the generic instance of type(self)[type(model)]
         # due to the lack of higher-kinded generics in python as of this writing.
         # See: https://github.com/python/typing/issues/548
         # This cast() will be wrong for sub-classes of Relation...
         return cast(
             Relation[model],
@@ -1729,38 +1699,38 @@
                 derived_from=self._relation,
                 database=self.database,
                 model=model,
             ),
         )
 
     @property
-    def types(self) -> Dict[str, DuckDBSQLType]:
+    def types(self):  # type: ignore[no-untyped-def]  # noqa
         """
         Return the SQL types of all the columns of the given relation.
 
         Returns:
             dict[str, str]: A dictionary where the keys are the column names and the
             values are SQL types as strings.
 
         Examples:
             >>> import patito as pt
-            >>> pt.Relation("select 1 as a, 'my_value' as b").types
-            {'a': 'INTEGER', 'b': 'VARCHAR'}
+            >>> pt.duckdb.Relation("select 1 as a, 'my_value' as b").types
+            {'a': INTEGER, 'b': VARCHAR}
         """
         return dict(zip(self.columns, self._relation.types))
 
     def to_pandas(self) -> "pd.DataFrame":
         """
         Return a pandas DataFrame representation of relation object.
 
         Returns: A ``pandas.DataFrame`` object containing all the data of the relation.
 
         Example:
             >>> import patito as pt
-            >>> pt.Relation("select 1 as column union select 2 as column").order(
+            >>> pt.duckdb.Relation("select 1 as column union select 2 as column").order(
             ...     by="1"
             ... ).to_pandas()
                   column
                0       1
                1       2
         """
         return self._relation.to_df()
@@ -1769,66 +1739,65 @@
         """
         Return a polars DataFrame representation of relation object.
 
         Returns: A ``patito.DataFrame`` object which inherits from ``polars.DataFrame``.
 
         Example:
             >>> import patito as pt
-            >>> pt.Relation("select 1 as column union select 2 as column").order(
+            >>> pt.duckdb.Relation("select 1 as column union select 2 as column").order(
             ...     by="1"
             ... ).to_df()
             shape: (2, 1)
             ┌────────┐
             │ column │
             │ ---    │
             │ i64    │
             ╞════════╡
             │ 1      │
-            ├╌╌╌╌╌╌╌╌┤
             │ 2      │
             └────────┘
         """
         # Here we do a star-select to work around certain weird issues with DuckDB
         self._relation = self._relation.project("*")
         arrow_table = cast(pa.lib.Table, self._relation.to_arrow_table())
         try:
             # We cast `INTEGER`-typed columns to `pl.Int64` when converting to Polars
             # because polars is much more eager to store integer Series as 64-bit
             # integers. Otherwise there must be done a lot of manual casting whenever
             # you cross the boundary between DuckDB and polars.
-            return DataFrame._from_arrow(arrow_table).with_column(
+            return DataFrame._from_arrow(arrow_table).with_columns(
                 pl.col(pl.Int32).cast(pl.Int64)
             )
-        except pa.ArrowInvalid:  # pragma: no cover
+        except (pa.ArrowInvalid, pl.ArrowError):  # pragma: no cover
             # Empty relations with enum columns can sometimes produce errors.
             # As a last-ditch effort, we convert such columns to VARCHAR.
             casted_columns = [
                 f"{field.name}::VARCHAR as {field.name}"
                 if isinstance(field.type, pa.DictionaryType)
                 else field.name
                 for field in arrow_table.schema
             ]
             non_enum_relation = self._relation.project(", ".join(casted_columns))
             arrow_table = non_enum_relation.to_arrow_table()
-            return DataFrame._from_arrow(arrow_table).with_column(
+            return DataFrame._from_arrow(arrow_table).with_columns(
                 pl.col(pl.Int32).cast(pl.Int64)
             )
 
     def to_series(self) -> pl.Series:
         """
         Convert the given relation to a polars Series.
 
         Raises:
             TypeError: If the given relation does not contain exactly one column.
 
         Returns: A ``polars.Series`` object containing the data of the relation.
 
         Example:
             >>> import patito as pt
-            >>> relation = pt.Relation("select 1 as a union select 2 as a")
+            >>> relation = pt.duckdb.Relation("select 1 as a union select 2 as a")
             >>> relation.order(by="a").to_series()
             shape: (2,)
             Series: 'a' [i32]
             [
                         1
                         2
             ]
@@ -1850,48 +1819,47 @@
         The two relations must have the same column names, but not necessarily in the
         same order as reordering of columns is automatically performed, unlike regular
         SQL.
 
         Duplicates are `not` dropped.
 
         Args:
-            other: A ``patito.Relation`` object or something that can be `casted` to
-                ``patito.Relation``. See :ref:`Relation<Relation.__init__>`.
+            other: A ``patito.duckdb.Relation`` object or something that can be
+                *casted* to ``patito.duckdb.Relation``.
+                See :ref:`Relation<duckdb.Relation.__init__>`.
 
         Returns:
             New relation containing the rows of both ``self`` and ``other``.
 
         Raises:
             TypeError: If the two relations do not contain the same columns.
 
         Examples:
             >>> import patito as pt
-            >>> relation_1 = pt.Relation("select 1 as a")
-            >>> relation_2 = pt.Relation("select 2 as a")
+            >>> relation_1 = pt.duckdb.Relation("select 1 as a")
+            >>> relation_2 = pt.duckdb.Relation("select 2 as a")
             >>> relation_1.union(relation_2).to_df()
             shape: (2, 1)
             ┌─────┐
             │ a   │
             │ --- │
             │ i64 │
             ╞═════╡
             │ 1   │
-            ├╌╌╌╌╌┤
             │ 2   │
             └─────┘
 
             >>> (relation_1 + relation_2).to_df()
             shape: (2, 1)
             ┌─────┐
             │ a   │
             │ --- │
             │ i64 │
             ╞═════╡
             │ 1   │
-            ├╌╌╌╌╌┤
             │ 2   │
             └─────┘
         """
         other_relation = self.database.to_relation(other)
         if set(self.columns) != set(other_relation.columns):
             msg = "Union between relations with different column names is not allowed."
             additional_left = set(self.columns) - set(other_relation.columns)
@@ -1924,15 +1892,15 @@
                 expression.
 
         Returns:
             Relation with the given columns appended, or possibly overwritten.
 
         Examples:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> relation = db.to_relation("select 1 as a, 2 as b")
             >>> relation.with_columns(c="a + b").to_df()
             shape: (1, 3)
             ┌─────┬─────┬─────┐
             │ a   ┆ b   ┆ c   │
             │ --- ┆ --- ┆ --- │
             │ i64 ┆ i64 ┆ i64 │
@@ -1946,16 +1914,16 @@
         self: RelationType,
         include: Optional[Iterable[str]] = None,
         exclude: Optional[Iterable[str]] = None,
     ) -> RelationType:
         """
         Add missing defaultable columns filled with the default values of correct type.
 
-        Make sure to invoke :ref:`Relation.set_model()<Relation.set_model>` with the
-        correct model schema before executing
+        Make sure to invoke :ref:`Relation.set_model()<duckdb.Relation.set_model>` with
+        the correct model schema before executing
         ``Relation.with_missing_default_columns()``.
 
         Args:
             include: If provided, only fill in default values for missing columns part
                 of this collection of column names.
             exclude: If provided, do `not` fill in default values for missing columns
                 part of this collection of column names.
@@ -1968,15 +1936,15 @@
             >>> import patito as pt
             >>> class MyModel(pt.Model):
             ...     non_default_column: int
             ...     another_non_default_column: int
             ...     default_column: int = 42
             ...     another_default_column: int = 42
             ...
-            >>> relation = pt.Relation(
+            >>> relation = pt.duckdb.Relation(
             ...     "select 1 as non_default_column, 2 as default_column"
             ... )
             >>> relation.to_df()
             shape: (1, 2)
             ┌────────────────────┬────────────────┐
             │ non_default_column ┆ default_column │
             │ ---                ┆ ---            │
@@ -2036,16 +2004,16 @@
         self: RelationType,
         include: Optional[Iterable[str]] = None,
         exclude: Optional[Iterable[str]] = None,
     ) -> RelationType:
         """
         Add missing nullable columns filled with correctly typed nulls.
 
-        Make sure to invoke :ref:`Relation.set_model()<Relation.set_model>` with the
-        correct model schema before executing
+        Make sure to invoke :ref:`Relation.set_model()<duckdb.Relation.set_model>` with
+        the correct model schema before executing
         ``Relation.with_missing_nullable_columns()``.
 
         Args:
             include: If provided, only fill in null values for missing columns part of
                 this collection of column names.
             exclude: If provided, do `not` fill in null values for missing columns
                 part of this collection of column names.
@@ -2058,15 +2026,15 @@
             >>> from typing import Optional
             >>> import patito as pt
             >>> class MyModel(pt.Model):
             ...     non_nullable_column: int
             ...     nullable_column: Optional[int]
             ...     another_nullable_column: Optional[int]
             ...
-            >>> relation = pt.Relation("select 1 as nullable_column")
+            >>> relation = pt.duckdb.Relation("select 1 as nullable_column")
             >>> relation.to_df()
             shape: (1, 1)
             ┌─────────────────┐
             │ nullable_column │
             │ ---             │
             │ i64             │
             ╞═════════════════╡
@@ -2118,15 +2086,15 @@
                 raise exc
         return self._wrap(relation=relation, schema_change=False)
 
     def __add__(self: RelationType, other: RelationSource) -> RelationType:
         """
         Execute ``self.union(other)``.
 
-        See :ref:`Relation.union()<Relation.union>` for full documentation.
+        See :ref:`Relation.union()<duckdb.Relation.union>` for full documentation.
         """
         return self.union(other)
 
     def __eq__(self, other: object) -> bool:
         """Check if Relation is equal to a Relation-able data source."""
         other_relation = self.database.to_relation(other)  # type: ignore
         # Check if the number of rows are equal, and then check if each row is equal.
@@ -2135,29 +2103,29 @@
             row == other_row for row, other_row in zip(self, other_relation)
         )
 
     def __getitem__(self, key: Union[str, Iterable[str]]) -> Relation:
         """
         Return Relation with selected columns.
 
-        Uses :ref:`Relation.select()<Relation.select>` under-the-hood in order to
+        Uses :ref:`Relation.select()<duckdb.Relation.select>` under-the-hood in order to
         perform the selection. Can technically be used to rename columns,
         define derived columns, and so on, but prefer the use of Relation.select() for
         such use cases.
 
         Args:
             key: Columns to select, either a single column represented as a string, or
                 an iterable of strings.
 
         Returns:
             New relation only containing the column subset specified.
 
         Example:
             >>> import patito as pt
-            >>> relation = pt.Relation("select 1 as a, 2 as b, 3 as c")
+            >>> relation = pt.duckdb.Relation("select 1 as a, 2 as b, 3 as c")
             >>> relation.to_df()
             shape: (1, 3)
             ┌─────┬─────┬─────┐
             │ a   ┆ b   ┆ c   │
             │ --- ┆ --- ┆ --- │
             │ i64 ┆ i64 ┆ i64 │
             ╞═════╪═════╪═════╡
@@ -2188,26 +2156,26 @@
             schema_change=True,
         )
 
     def __iter__(self) -> Iterator[ModelType]:
         """
         Iterate over rows in relation.
 
-        If :ref:`Relation.set_model()<Relation.set_model>` has been invoked first, the
-        given model will be used to deserialize each row. Otherwise a Patito model
-        is dynamically constructed which fits the schema of the relation.
+        If :ref:`Relation.set_model()<duckdb.Relation.set_model>` has been invoked
+        first, the given model will be used to deserialize each row. Otherwise a Patito
+        model is dynamically constructed which fits the schema of the relation.
 
         Returns:
             Iterator[Model]: An iterator of patito Model objects representing each row.
 
         Example:
             >>> from typing import Literal
             >>> import patito as pt
             >>> df = pt.DataFrame({"float_column": [1, 2], "enum_column": ["A", "B"]})
-            >>> relation = pt.Relation(df).set_alias("my_relation")
+            >>> relation = pt.duckdb.Relation(df).set_alias("my_relation")
             >>> for row in relation:
             ...     print(row)
             ...
             float_column=1 enum_column='A'
             float_column=2 enum_column='B'
             >>> list(relation)
             [my_relation(float_column=1, enum_column='A'),
@@ -2235,27 +2203,27 @@
             else:
                 yield self._to_model(row_tuple)
 
     def __len__(self) -> int:
         """
         Return the number of rows in the relation.
 
-        See :ref:`Relation.count()<Relation.count>` for full documentation.
+        See :ref:`Relation.count()<duckdb.Relation.count>` for full documentation.
         """
         return self.count()
 
     def __str__(self) -> str:
         """
         Return string representation of Relation object.
 
         Includes an expression tree, the result columns, and a result preview.
 
         Example:
             >>> import patito as pt
-            >>> products = pt.Relation(
+            >>> products = pt.duckdb.Relation(
             ...     pt.DataFrame(
             ...         {
             ...             "product_name": ["apple", "red_apple", "banana", "oranges"],
             ...             "supplier_id": [2, 2, 1, 3],
             ...         }
             ...     )
             ... ).set_alias("products")
@@ -2278,15 +2246,15 @@
             VARCHAR BIGINT
             [ Rows: 4]
             apple   2
             red_apple       2
             banana  1
             oranges 3
 
-            >>> suppliers = pt.Relation(
+            >>> suppliers = pt.duckdb.Relation(
             ...     pt.DataFrame(
             ...         {
             ...             "id": [1, 2],
             ...             "supplier_name": ["Banana Republic", "Applies Inc."],
             ...         }
             ...     )
             ... ).set_alias("suppliers")
@@ -2366,15 +2334,15 @@
             path: Optional path to store all the data to. If ``None`` the data is
                 persisted in-memory only.
             read_only: If the database connection should be a read-only connection.
             **kwargs: Additional keywords forwarded to ``duckdb.connect()``.
 
         Examples:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> db.to_relation("select 1 as a, 2 as b").create_table("my_table")
             >>> db.query("select * from my_table").to_df()
             shape: (1, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
@@ -2394,20 +2362,20 @@
 
     @classmethod
     def default(cls) -> Database:
         """
         Return the default DuckDB database.
 
         Returns:
-            A patito :ref:`Database<Database>` object wrapping around the given
+            A patito :ref:`Database<duckdb.Database>` object wrapping around the given
             connection.
 
         Example:
             >>> import patito as pt
-            >>> db = pt.Database.default()
+            >>> db = pt.duckdb.Database.default()
             >>> db.query("select 1 as a, 2 as b").to_df()
             shape: (1, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
@@ -2424,21 +2392,22 @@
         Create database from native DuckDB connection object.
 
         Args:
             connection: A native DuckDB connection object created with
                 ``duckdb.connect()``.
 
         Returns:
-            A :ref:`Database<Database>` object wrapping around the given connection.
+            A :ref:`Database<duckdb.Database>` object wrapping around the given
+            connection.
 
         Example:
             >>> import duckdb
             >>> import patito as pt
             >>> connection = duckdb.connect()
-            >>> database = pt.Database.from_connection(connection)
+            >>> database = pt.duckdb.Database.from_connection(connection)
         """
         obj = cls.__new__(cls)
         obj.connection = connection
         obj.enum_types = set()
         return obj
 
     def to_relation(
@@ -2455,15 +2424,15 @@
         Args:
             derived_from (RelationSource): One of either a polars or pandas
                 ``DataFrame``, a ``pathlib.Path`` to a parquet or CSV file, a SQL query
                 string, or an existing relation.
 
         Example:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> db.to_relation("select 1 as a, 2 as b").to_df()
             shape: (1, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
@@ -2473,15 +2442,14 @@
             shape: (2, 2)
             ┌─────┬─────┐
             │ c   ┆ d   │
             │ --- ┆ --- │
             │ i64 ┆ str │
             ╞═════╪═════╡
             │ 3   ┆ 5   │
-            ├╌╌╌╌╌┼╌╌╌╌╌┤
             │ 4   ┆ 6   │
             └─────┴─────┘
         """
         return Relation(
             derived_from=derived_from,
             database=self,
         )
@@ -2499,43 +2467,40 @@
                 a semicolon (``;``).
             parameters: One or more sets of parameters to insert into prepared
                 statements. The values are replaced in place of the question marks
                 (``?``) in the prepared query.
 
         Example:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> db.execute("create table my_table (x bigint);")
             >>> db.execute("insert into my_table values (1), (2), (3)")
             >>> db.table("my_table").to_df()
             shape: (3, 1)
             ┌─────┐
             │ x   │
             │ --- │
             │ i64 │
             ╞═════╡
             │ 1   │
-            ├╌╌╌╌╌┤
             │ 2   │
-            ├╌╌╌╌╌┤
             │ 3   │
             └─────┘
 
             Parameters can be specified when executing prepared queries.
 
             >>> db.execute("delete from my_table where x = ?", (2,))
             >>> db.table("my_table").to_df()
             shape: (2, 1)
             ┌─────┐
             │ x   │
             │ --- │
             │ i64 │
             ╞═════╡
             │ 1   │
-            ├╌╌╌╌╌┤
             │ 3   │
             └─────┘
 
             Multiple parameter sets can be specified when executing multiple prepared
             queries.
 
             >>> db.execute(
@@ -2582,15 +2547,15 @@
             alias: The alias to assign to the resulting relation, to be used in further
                 queries.
 
         Returns: A relation representing the data produced by the given query.
 
         Example:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> relation = db.query("select 1 as a, 2 as b, 3 as c")
             >>> relation.to_df()
             shape: (1, 3)
             ┌─────┬─────┬─────┐
             │ a   ┆ b   ┆ c   │
             │ --- ┆ --- ┆ --- │
             │ i64 ┆ i64 ┆ i64 │
@@ -2624,15 +2589,15 @@
 
         Example:
             >>> import patito as pt
             >>> class Schema(pt.Model):
             ...     string_column: str
             ...     bool_column: bool
             ...
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> empty_relation = db.empty_relation(Schema)
             >>> empty_relation.to_df()
             shape: (0, 2)
             ┌───────────────┬─────────────┐
             │ string_column ┆ bool_column │
             │ ---           ┆ ---         │
             │ str           ┆ bool        │
@@ -2659,26 +2624,25 @@
 
         Args:
             name: The name of the table.
 
         Example:
             >>> import patito as pt
             >>> df = pt.DataFrame({"a": [1, 2], "b": [3, 4]})
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> relation = db.to_relation(df)
             >>> relation.create_table(name="my_table")
             >>> db.table("my_table").to_df()
             shape: (2, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
             │ 1   ┆ 3   │
-            ├╌╌╌╌╌┼╌╌╌╌╌┤
             │ 2   ┆ 4   │
             └─────┴─────┘
         """
         return Relation(
             self.connection.table(name),
             database=self.from_connection(self.connection),
         )
@@ -2689,26 +2653,25 @@
 
         Args:
             name: The name of the view.
 
         Example:
             >>> import patito as pt
             >>> df = pt.DataFrame({"a": [1, 2], "b": [3, 4]})
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> relation = db.to_relation(df)
             >>> relation.create_view(name="my_view")
             >>> db.view("my_view").to_df()
             shape: (2, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ i64 │
             ╞═════╪═════╡
             │ 1   ┆ 3   │
-            ├╌╌╌╌╌┼╌╌╌╌╌┤
             │ 2   ┆ 4   │
             └─────┴─────┘
         """
         return Relation(
             self.connection.view(name),
             database=self.from_connection(self.connection),
         )
@@ -2717,19 +2680,19 @@
         self,
         name: str,
         model: Type[ModelType],
     ) -> Relation[ModelType]:
         """
         Create table with schema matching the provided Patito model.
 
-        See :ref:`Relation.insert_into()<Relation.insert_into>` for how to insert data
-        into the table after creation.
-        The :ref:`Relation.create_table()<Relation.create_table>` method can also be
-        used to create a table from a given relation `and` insert the data at the same
-        time.
+        See :ref:`Relation.insert_into()<duckdb.Relation.insert_into>` for how to insert
+        data into the table after creation.
+        The :ref:`Relation.create_table()<duckdb.Relation.create_table>` method can also
+        be used to create a table from a given relation `and` insert the data at the
+        same time.
 
         Args:
             name: Name of new database table.
             model (Type[Model]): Patito model indicating names and types of table
                 columns.
         Returns:
             Relation[ModelType]: Relation pointing to the new table.
@@ -2737,18 +2700,18 @@
         Example:
             >>> from typing import Optional
             >>> import patito as pt
             >>> class MyModel(pt.Model):
             ...     str_column: str
             ...     nullable_string_column: Optional[str]
             ...
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> db.create_table(name="my_table", model=MyModel)
             >>> db.table("my_table").types
-            {'str_column': 'VARCHAR', 'nullable_string_column': 'VARCHAR'}
+            {'str_column': VARCHAR, 'nullable_string_column': VARCHAR}
         """
         self.create_enum_types(model=model)
         schema = model.schema()
         non_nullable = schema.get("required", [])
         columns = []
         for column_name, sql_type in model.sql_types.items():
             column = f"{column_name} {sql_type}"
@@ -2768,15 +2731,15 @@
                 will get respective DuckDB enum types.
 
         Example:
             >>> import patito as pt
             >>> class EnumModel(pt.Model):
             ...     enum_column: Literal["A", "B", "C"]
             ...
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> db.create_enum_types(EnumModel)
             >>> db.enum_types
             {'enum__7ba49365cc1b0fd57e61088b3bc9aa25'}
         """
         import duckdb
 
         for props in model._schema_properties().values():
@@ -2812,15 +2775,15 @@
         Return ``True`` if the database contains a table with the given name.
 
         Args:
             table: The name of the table to be checked for.
 
         Examples:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> "my_table" in db
             False
             >>> db.to_relation("select 1 as a, 2 as b").create_table(name="my_table")
             >>> "my_table" in db
             True
         """
         try:
```

### Comparing `patito-0.4.4/src/patito/exceptions.py` & `patito-0.5.0/src/patito/exceptions.py`

 * *Files identical despite different names*

### Comparing `patito-0.4.4/src/patito/polars.py` & `patito-0.5.0/src/patito/polars.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Logic related to the wrapping of the polars data frame library."""
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
+    Collection,
     Generic,
+    Iterable,
     Optional,
-    Sequence,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 import polars as pl
+from polars.type_aliases import IntoExpr
 from pydantic import create_model
 from typing_extensions import Literal
 
 from patito.exceptions import MultipleRowsReturned, RowDoesNotExist
 
 if TYPE_CHECKING:
     import numpy as np
-    from polars.internals import WhenThen, WhenThenThen
 
     from patito.pydantic import Model
 
 
 DF = TypeVar("DF", bound="DataFrame")
 LDF = TypeVar("LDF", bound="LazyFrame")
 ModelType = TypeVar("ModelType", bound="Model")
@@ -205,35 +206,29 @@
             shape: (4, 2)
             ┌──────┬────────┐
             │ year ┆ letter │
             │ ---  ┆ ---    │
             │ i64  ┆ str    │
             ╞══════╪════════╡
             │ 1    ┆ A      │
-            ├╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┤
             │ 1    ┆ B      │
-            ├╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┤
             │ 2    ┆ A      │
-            ├╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┤
             │ 2    ┆ B      │
             └──────┴────────┘
             >>> casted_classes = classes.cast()
             >>> casted_classes
             shape: (4, 2)
             ┌──────┬────────┐
             │ year ┆ letter │
             │ ---  ┆ ---    │
             │ u16  ┆ cat    │
             ╞══════╪════════╡
             │ 1    ┆ A      │
-            ├╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┤
             │ 1    ┆ B      │
-            ├╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┤
             │ 2    ┆ A      │
-            ├╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌┤
             │ 2    ┆ B      │
             └──────┴────────┘
             >>> casted_classes.validate()
         """
         cls = self._construct_dataframe_model_class(model=model)
         return cast(
             DataFrame[model],
@@ -288,26 +283,31 @@
                 columns.append(pl.col(column).cast(properties[column]["dtype"]))
             elif not strict and current_dtype in valid_dtypes[column]:
                 columns.append(pl.col(column))
             else:
                 columns.append(pl.col(column).cast(default_dtypes[column]))
         return self.with_columns(columns)
 
-    def drop(self: DF, columns: Optional[Union[str, Sequence[str]]] = None) -> DF:
+    def drop(
+        self: DF,
+        columns: Optional[Union[str, Collection[str]]] = None,
+        *more_columns: str,
+    ) -> DF:
         """
         Drop one or more columns from the dataframe.
 
         If ``name`` is not provided then all columns `not` specified by the associated
         patito model, for instance set with
         :ref:`DataFrame.set_model <DataFrame.set_model>`, are dropped.
 
         Args:
             columns: A single column string name, or list of strings, indicating
                 which columns to drop. If not specified, all columns *not*
                 specified by the associated dataframe model will be dropped.
+            more_columns: Additional named columns to drop.
 
         Returns:
             DataFrame[Model]: New dataframe without the specified columns.
 
         Examples:
             >>> import patito as pt
             >>> class Model(pt.Model):
@@ -317,21 +317,20 @@
             shape: (2, 1)
             ┌──────────┐
             │ column_1 │
             │ ---      │
             │ i64      │
             ╞══════════╡
             │ 1        │
-            ├╌╌╌╌╌╌╌╌╌╌┤
             │ 2        │
             └──────────┘
 
         """
         if columns is not None:
-            return super().drop(columns)
+            return self._from_pydf(super().drop(columns)._df)
         else:
             return self.drop(list(set(self.columns) - set(self.model.columns)))
 
     def validate(self: DF) -> DF:
         """
         Validate the schema and content of the dataframe.
 
@@ -414,29 +413,28 @@
             shape: (2, 3)
             ┌─────┬─────┬────────────┐
             │ foo ┆ bar ┆ double_bar │
             │ --- ┆ --- ┆ ---        │
             │ i64 ┆ i64 ┆ i64        │
             ╞═════╪═════╪════════════╡
             │ 1   ┆ 1   ┆ 2          │
-            ├╌╌╌╌╌┼╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ 2   ┆ 2   ┆ 4          │
             └─────┴─────┴────────────┘
         """
         df = self.lazy()
         for column_name, props in self.model._schema_properties().items():
             if "derived_from" in props:
                 derived_from = props["derived_from"]
                 dtype = self.model.dtypes[column_name]
                 if isinstance(derived_from, str):
-                    df = df.with_column(
+                    df = df.with_columns(
                         pl.col(derived_from).cast(dtype).alias(column_name)
                     )
                 elif isinstance(derived_from, pl.Expr):
-                    df = df.with_column(derived_from.cast(dtype).alias(column_name))
+                    df = df.with_columns(derived_from.cast(dtype).alias(column_name))
                 else:
                     raise TypeError(
                         "Can not derive dataframe column from type "
                         f"{type(derived_from)}."
                     )
         return cast(DF, df.collect())
 
@@ -484,20 +482,19 @@
             shape: (2, 2)
             ┌────────┬───────┐
             │ name   ┆ price │
             │ ---    ┆ ---   │
             │ str    ┆ i64   │
             ╞════════╪═══════╡
             │ apple  ┆ 10    │
-            ├╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌┤
             │ banana ┆ 19    │
             └────────┴───────┘
         """
         if strategy != "defaults":  # pragma: no cover
-            return cast(  # type: ignore[redundant-cast]
+            return cast(  # pyright: ignore[redundant-cast]
                 DF,
                 super().fill_null(
                     value=value,
                     strategy=strategy,
                     limit=limit,
                     matches_supertype=matches_supertype,
                 ),
@@ -603,15 +600,15 @@
 
         pydantic_annotations = {column: (Any, ...) for column in self.columns}
         return cast(
             Type[Model],
             create_model(  # type: ignore
                 "UntypedRow",
                 __base__=Model,
-                **pydantic_annotations,
+                **pydantic_annotations,  # pyright: ignore
             ),
         )
 
     @classmethod
     def read_csv(  # type: ignore[no-untyped-def]
         cls: Type[DF],
         *args,  # noqa: ANN002
@@ -658,54 +655,49 @@
             >>> import io
             >>> import patito as pt
             >>> class CSVModel(pt.Model):
             ...     a: float
             ...     b: str = pt.Field(derived_from="source_of_b")
             ...
             >>> csv_file = io.StringIO("a,source_of_b\n1,1")
-            >>> CSVModel.DataFrame.read_csv(csv_file).drop()
-            shape: (1, 2)
-            ┌─────┬─────┐
-            │ a   ┆ b   │
-            │ --- ┆ --- │
-            │ f64 ┆ str │
-            ╞═════╪═════╡
-            │ 1.0 ┆ 1   │
-            └─────┴─────┘
+
+
+            # >>> CSVModel.DataFrame.read_csv(csv_file).drop()
+            # shape: (1, 2)
+            # ┌─────┬─────┐
+            # │ a   ┆ b   │
+            # │ --- ┆ --- │
+            # │ f64 ┆ str │
+            # ╞═════╪═════╡
+            # │ 1.0 ┆ 1   │
+            # └─────┴─────┘
         """
         kwargs.setdefault("dtypes", cls.model.dtypes)
         if not kwargs.get("has_header", True) and "columns" not in kwargs:
             kwargs.setdefault("new_columns", cls.model.columns)
         df = cls.model.DataFrame._from_pydf(pl.read_csv(*args, **kwargs)._df)
         return df.derive()
 
     # --- Type annotation overrides ---
     def filter(  # noqa: D102
         self: DF,
-        predicate: Union[pl.Expr, str, pl.Series, list[bool], np.ndarray[Any, Any]],
+        predicate: Union[
+            pl.Expr, str, pl.Series, list[bool], np.ndarray[Any, Any], bool
+        ],
     ) -> DF:
         return cast(DF, super().filter(predicate=predicate))
 
     def select(  # noqa: D102
         self: DF,
-        exprs: Union[
-            pl.Expr,
-            pl.Series,
-            Sequence[Union[str, pl.Expr, pl.Series, "WhenThen", "WhenThenThen"]],
-        ],
+        *exprs: Union[IntoExpr, Iterable[IntoExpr]],
+        **named_exprs: IntoExpr,
     ) -> DF:
-        return cast(DF, super().select(exprs=exprs))  # type: ignore[redundant-cast]
-
-    def with_column(self: DF, column: Union[pl.Series, pl.Expr]) -> DF:  # noqa: D102
-        return cast(DF, super().with_column(column=column))
+        return cast(  # pyright: ignore[redundant-cast]
+            DF, super().select(*exprs, **named_exprs)
+        )
 
     def with_columns(  # noqa: D102
         self: DF,
-        exprs: Union[
-            pl.Expr,
-            pl.Series,
-            Sequence[Union[pl.Expr, pl.Series]],
-            None,
-        ] = None,
-        **named_exprs: Union[pl.Expr, pl.Series],
+        *exprs: Union[IntoExpr, Iterable[IntoExpr]],
+        **named_exprs: IntoExpr,
     ) -> DF:
-        return cast(DF, super().with_columns(exprs=exprs, **named_exprs))
+        return cast(DF, super().with_columns(*exprs, **named_exprs))
```

### Comparing `patito-0.4.4/src/patito/pydantic.py` & `patito-0.5.0/src/patito/pydantic.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 import polars as pl
+from polars.datatypes import PolarsDataType
 from pydantic import BaseConfig, BaseModel, Field, create_model  # noqa: F401
 from pydantic.main import ModelMetaclass as PydanticModelMetaclass
 from typing_extensions import Literal, get_args
 
 from patito.polars import DataFrame, LazyFrame
 from patito.validators import validate
 
@@ -106,15 +107,15 @@
             >>> Product.columns
             ['name', 'price']
         """
         return list(cls.schema()["properties"].keys())
 
     @property
     def dtypes(  # type: ignore
-        cls: Type[ModelType],
+        cls: Type[ModelType],  # pyright: ignore
     ) -> dict[str, Type[pl.DataType]]:
         """
         Return the polars dtypes of the dataframe.
 
         Unless Field(dtype=...) is specified, the highest signed column dtype
         is chosen for integer and float columns.
 
@@ -125,26 +126,24 @@
             >>> import patito as pt
             >>> class Product(pt.Model):
             ...     name: str
             ...     ideal_temperature: int
             ...     price: float
             ...
             >>> Product.dtypes
-            {'name': <class 'polars.datatypes.Utf8'>, \
-'ideal_temperature': <class 'polars.datatypes.Int64'>, \
-'price': <class 'polars.datatypes.Float64'>}
+            {'name': Utf8, 'ideal_temperature': Int64, 'price': Float64}
         """
         return {
             column: valid_dtypes[0] for column, valid_dtypes in cls.valid_dtypes.items()
         }
 
     @property
-    def valid_dtypes(  # type: ignore  # noqa: C901
-        cls: Type[ModelType],
-    ) -> dict[str, List[Type[pl.DataType]]]:
+    def valid_dtypes(  # type: ignore
+        cls: Type[ModelType],  # pyright: ignore
+    ) -> dict[str, List[Union[pl.PolarsDataType, pl.List]]]:
         """
         Return a list of polars dtypes which Patito considers valid for each field.
 
         The first item of each list is the default dtype chosen by Patito.
 
         Returns:
             A dictionary mapping each column string name to a list of valid dtypes.
@@ -160,90 +159,99 @@
             >>> class MyModel(pt.Model):
             ...     bool_column: bool
             ...     str_column: str
             ...     int_column: int
             ...     float_column: float
             ...
             >>> pprint(MyModel.valid_dtypes)
-            {'bool_column': [<class 'polars.datatypes.Boolean'>],
-             'float_column': [<class 'polars.datatypes.Float64'>,
-                              <class 'polars.datatypes.Float32'>],
-             'int_column': [<class 'polars.datatypes.Int64'>,
-                            <class 'polars.datatypes.Int32'>,
-                            <class 'polars.datatypes.Int16'>,
-                            <class 'polars.datatypes.Int8'>,
-                            <class 'polars.datatypes.UInt64'>,
-                            <class 'polars.datatypes.UInt32'>,
-                            <class 'polars.datatypes.UInt16'>,
-                            <class 'polars.datatypes.UInt8'>],
-             'str_column': [<class 'polars.datatypes.Utf8'>]}
+            {'bool_column': [Boolean],
+             'float_column': [Float64, Float32],
+             'int_column': [Int64, Int32, Int16, Int8, UInt64, UInt32, UInt16, UInt8],
+             'str_column': [Utf8]}
         """
         valid_dtypes = {}
         for column, props in cls._schema_properties().items():
-            if "dtype" in props:
-                valid_dtypes[column] = [
-                    props["dtype"],
-                ]
-            elif "enum" in props and props["type"] == "string":
-                valid_dtypes[column] = [pl.Categorical, pl.Utf8]
-            elif "type" not in props:
+            column_dtypes: List[Union[PolarsDataType, pl.List]]
+            if props.get("type") == "array":
+                array_props = props["items"]
+                item_dtypes = cls._valid_dtypes(props=array_props)
+                if item_dtypes is None:
+                    raise NotImplementedError(
+                        f"No valid dtype mapping found for column '{column}'."
+                    )
+                column_dtypes = [pl.List(dtype) for dtype in item_dtypes]
+            else:
+                column_dtypes = cls._valid_dtypes(props=props)  # pyright: ignore
+
+            if column_dtypes is None:
                 raise NotImplementedError(
                     f"No valid dtype mapping found for column '{column}'."
                 )
-            elif props["type"] == "integer":
-                valid_dtypes[column] = [
-                    pl.Int64,
-                    pl.Int32,
-                    pl.Int16,
-                    pl.Int8,
-                    pl.UInt64,
-                    pl.UInt32,
-                    pl.UInt16,
-                    pl.UInt8,
-                ]
-            elif props["type"] == "number":
-                if props.get("format") == "time-delta":
-                    valid_dtypes[column] = [
-                        pl.Duration,
-                    ]  # pyright: reportPrivateImportUsage=false
-                else:
-                    valid_dtypes[column] = [pl.Float64, pl.Float32]
-            elif props["type"] == "boolean":
-                valid_dtypes[column] = [
-                    pl.Boolean,
-                ]
-            elif props["type"] == "string":
-                string_format = props.get("format")
-                if string_format is None:
-                    valid_dtypes[column] = [
-                        pl.Utf8,
-                    ]
-                elif string_format == "date":
-                    valid_dtypes[column] = [
-                        pl.Date,
-                    ]
-                # TODO: Find out why this branch is not being hit
-                elif string_format == "date-time":  # pragma: no cover
-                    valid_dtypes[column] = [
-                        pl.Datetime,
-                    ]
-            elif props["type"] == "null":
-                valid_dtypes[column] = [
-                    pl.Null,
-                ]
-            else:  # pragma: no cover
-                raise NotImplementedError(
-                    f"No valid dtype mapping found for column '{column}'"
-                )
+            valid_dtypes[column] = column_dtypes
 
         return valid_dtypes
 
+    @staticmethod
+    def _valid_dtypes(  # noqa: C901
+        props: Dict,
+    ) -> Optional[List[pl.PolarsDataType]]:
+        """
+        Map schema property to list of valid polars data types.
+
+        Args:
+            props: Dictionary value retrieved from BaseModel._schema_properties().
+
+        Returns:
+            List of valid dtypes. None if no mapping exists.
+        """
+        if "dtype" in props:
+            return [
+                props["dtype"],
+            ]
+        elif "enum" in props and props["type"] == "string":
+            return [pl.Categorical, pl.Utf8]
+        elif "type" not in props:
+            return None
+        elif props["type"] == "integer":
+            return [
+                pl.Int64,
+                pl.Int32,
+                pl.Int16,
+                pl.Int8,
+                pl.UInt64,
+                pl.UInt32,
+                pl.UInt16,
+                pl.UInt8,
+            ]
+        elif props["type"] == "number":
+            if props.get("format") == "time-delta":
+                return [pl.Duration]
+            else:
+                return [pl.Float64, pl.Float32]
+        elif props["type"] == "boolean":
+            return [pl.Boolean]
+        elif props["type"] == "string":
+            string_format = props.get("format")
+            if string_format is None:
+                return [pl.Utf8]
+            elif string_format == "date":
+                return [pl.Date]
+            # TODO: Find out why this branch is not being hit
+            elif string_format == "date-time":  # pragma: no cover
+                return [pl.Datetime]
+            else:
+                return None  # pragma: no cover
+        elif props["type"] == "null":
+            return [pl.Null]
+        else:  # pragma: no cover
+            return None
+
     @property
     def valid_sql_types(  # type: ignore  # noqa: C901
-        cls: Type[ModelType],
+        cls: Type[ModelType],  # pyright: ignore
     ) -> dict[str, List["DuckDBSQLType"]]:
         """
         Return a list of DuckDB SQL types which Patito considers valid for each field.
 
         The first item of each list is the default dtype chosen by Patito.
 
         Returns:
@@ -298,15 +306,15 @@
                 valid_dtypes[column] = [
                     props["sql_type"],
                 ]
             elif "enum" in props and props["type"] == "string":
                 from patito.duckdb import _enum_type_name
 
                 # fmt: off
-                valid_dtypes[column] = [
+                valid_dtypes[column] = [  # pyright: ignore
                     _enum_type_name(field_properties=props),  # type: ignore
                     "VARCHAR", "CHAR", "BPCHAR", "TEXT", "STRING",
                 ]
                 # fmt: on
             elif "type" not in props:
                 raise NotImplementedError(
                     f"No valid sql_type mapping found for column '{column}'."
@@ -370,15 +378,15 @@
                     f"No valid sql_type mapping found for column '{column}'"
                 )
 
         return valid_dtypes
 
     @property
     def sql_types(  # type: ignore
-        cls: Type[ModelType],
+        cls: Type[ModelType],  # pyright: ignore
     ) -> dict[str, str]:
         """
         Return compatible DuckDB SQL types for all model fields.
 
         Returns:
             Dictionary with column name keys and SQL type identifier strings.
 
@@ -401,15 +409,15 @@
         return {
             column: valid_types[0]
             for column, valid_types in cls.valid_sql_types.items()
         }
 
     @property
     def defaults(  # type: ignore
-        cls: Type[ModelType],
+        cls: Type[ModelType],  # pyright: ignore
     ) -> dict[str, Any]:
         """
         Return default field values specified on the model.
 
         Returns:
             Dictionary containing fields with their respective default values.
 
@@ -428,15 +436,15 @@
             field_name: props["default"]
             for field_name, props in cls._schema_properties().items()
             if "default" in props
         }
 
     @property
     def non_nullable_columns(  # type: ignore
-        cls: Type[ModelType],  # pyright: reportGeneralTypeIssues=false
+        cls: Type[ModelType],  # pyright: ignore
     ) -> set[str]:
         """
         Return names of those columns that are non-nullable in the schema.
 
         Returns:
             Set of column name strings.
 
@@ -452,15 +460,15 @@
             >>> sorted(MyModel.non_nullable_columns)
             ['another_non_nullable_field', 'non_nullable_field']
         """
         return set(cls.schema().get("required", {}))
 
     @property
     def nullable_columns(  # type: ignore
-        cls: Type[ModelType],  # pyright: reportGeneralTypeIssues=false
+        cls: Type[ModelType],  # pyright: ignore
     ) -> set[str]:
         """
         Return names of those columns that are nullable in the schema.
 
         Returns:
             Set of column name strings.
 
@@ -476,15 +484,15 @@
             >>> sorted(MyModel.nullable_columns)
             ['inferred_nullable_field', 'nullable_field']
         """
         return set(cls.columns) - cls.non_nullable_columns
 
     @property
     def unique_columns(  # type: ignore
-        cls: Type[ModelType],
+        cls: Type[ModelType],  # pyright: ignore
     ) -> set[str]:
         """
         Return columns with uniqueness constraint.
 
         Returns:
             Set of column name strings.
 
@@ -527,20 +535,24 @@
     valid_dtypes: ClassVar[Dict[str, List[Type[pl.DataType]]]]
     valid_sql_types: ClassVar[Dict[str, List["DuckDBSQLType"]]]
 
     defaults: ClassVar[Dict[str, Any]]
 
     @classmethod  # type: ignore[misc]
     @property
-    def DataFrame(cls: Type[ModelType]) -> Type[DataFrame[ModelType]]:
+    def DataFrame(
+        cls: Type[ModelType],
+    ) -> Type[DataFrame[ModelType]]:  # pyright: ignore  # noqa
         """Return DataFrame class where DataFrame.set_model() is set to self."""
 
     @classmethod  # type: ignore[misc]
     @property
-    def LazyFrame(cls: Type[ModelType]) -> Type[LazyFrame[ModelType]]:
+    def LazyFrame(
+        cls: Type[ModelType],
+    ) -> Type[LazyFrame[ModelType]]:  # pyright: ignore
         """Return DataFrame class where DataFrame.set_model() is set to self."""
 
     @classmethod
     def from_row(
         cls: Type[ModelType],
         row: Union["pd.DataFrame", pl.DataFrame],
         validate: bool = True,
@@ -566,15 +578,15 @@
             ...     product_id: int
             ...     name: str
             ...     price: float
             ...
 
             >>> df = pl.DataFrame(
             ...     [["1", "product name", "1.22"]],
-            ...     columns=["product_id", "name", "price"],
+            ...     schema=["product_id", "name", "price"],
             ... )
             >>> Product.from_row(df)
             Product(product_id=1, name='product name', price=1.22)
             >>> Product.from_row(df, validate=False)
             Product(product_id='1', name='product name', price='1.22')
         """
         if isinstance(row, pl.DataFrame):
@@ -618,15 +630,15 @@
             ...     product_id: int
             ...     name: str
             ...     price: float
             ...
 
             >>> df = pl.DataFrame(
             ...     [["1", "product name", "1.22"]],
-            ...     columns=["product_id", "name", "price"],
+            ...     schema=["product_id", "name", "price"],
             ... )
             >>> Product._from_polars(df)
             Product(product_id=1, name='product name', price=1.22)
             >>> Product._from_polars(df, validate=False)
             Product(product_id='1', name='product name', price='1.22')
         """
         if not isinstance(dataframe, pl.DataFrame):
@@ -973,15 +985,14 @@
             shape: (2, 3)
             ┌───────────┬──────────────────┬────────────┐
             │ name      ┆ temperature_zone ┆ product_id │
             │ ---       ┆ ---              ┆ ---        │
             │ str       ┆ cat              ┆ i64        │
             ╞═══════════╪══════════════════╪════════════╡
             │ product A ┆ dry              ┆ 0          │
-            ├╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ product B ┆ dry              ┆ 1          │
             └───────────┴──────────────────┴────────────┘
         """
         if data is None:
             # We should create an empty dataframe, but with the correct dtypes
             kwargs = {}
         elif not isinstance(data, dict):
@@ -1457,15 +1468,15 @@
           ...
         patito.exceptions.ValidationError: 4 validation errors for Product
         name
           Missing column (type=type_error.missingcolumns)
         product_id
           2 rows with duplicated values. (type=value_error.rowvalue)
         price
-          Polars dtype <class 'polars.datatypes.Int64'> \
-          does not match model field type. (type=type_error.columndtype)
+          Polars dtype Int64 does not match model field type. \
+          (type=type_error.columndtype)
         brand_color
           2 rows with out of bound values. (type=value_error.rowvalue)
     """
 
 
 Field.__doc__ = FieldDoc.__doc__
```

### Comparing `patito-0.4.4/src/patito/sql.py` & `patito-0.5.0/src/patito/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             default: Default output value for inputs which have no provided mapping.
                 If set to None, SQL NULL will be inserted as the default value.
             as_column: Name of column to insert the mapped values into. If not provided
                 the SQL string expression will not end with "AS <as_column>".
 
         Examples:
             >>> import patito as pt
-            >>> db = pt.Database()
+            >>> db = pt.duckdb.Database()
             >>> relation = db.to_relation("select 1 as a union select 2 as a")
             >>> case_statement = pt.sql.Case(
             ...     on_column="a",
             ...     mapping={1: "one", 2: "two"},
             ...     default="three",
             ...     as_column="b",
             ... )
@@ -57,15 +57,14 @@
             shape: (2, 2)
             ┌─────┬─────┐
             │ a   ┆ b   │
             │ --- ┆ --- │
             │ i64 ┆ str │
             ╞═════╪═════╡
             │ 1   ┆ one │
-            ├╌╌╌╌╌┼╌╌╌╌╌┤
             │ 2   ┆ two │
             └─────┴─────┘
         """
         self.on_column = on_column
         self.as_column = as_column
         self.mapping = {
             sql_repr(key): sql_repr(value) for key, value in mapping.items()
```

### Comparing `patito-0.4.4/setup.py` & `patito-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,908 +1,911 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 7061 7469 746f 275d 0a0a 7061 636b  ['patito']..pack
-00000070: 6167 655f 6461 7461 203d 205c 0a7b 2727  age_data = \.{''
-00000080: 3a20 5b27 2a27 5d7d 0a0a 696e 7374 616c  : ['*']}..instal
-00000090: 6c5f 7265 7175 6972 6573 203d 205c 0a5b  l_requires = \.[
-000000a0: 2770 6f6c 6172 733e 3d30 2e31 352e 3227  'polars>=0.15.2'
-000000b0: 2c20 2770 7964 616e 7469 633e 3d31 2e37  , 'pydantic>=1.7
-000000c0: 2e30 272c 2027 7479 7069 6e67 2d65 7874  .0', 'typing-ext
-000000d0: 656e 7369 6f6e 7327 5d0a 0a65 7874 7261  ensions']..extra
-000000e0: 735f 7265 7175 6972 6520 3d20 5c0a 7b27  s_require = \.{'
-000000f0: 3a70 7974 686f 6e5f 7665 7273 696f 6e20  :python_version 
-00000100: 3c20 2233 2e38 2227 3a20 5b27 696d 706f  < "3.8"': ['impo
-00000110: 7274 6c69 622d 6d65 7461 6461 7461 275d  rtlib-metadata']
-00000120: 2c0a 2027 646f 6373 273a 205b 2753 7068  ,. 'docs': ['Sph
-00000130: 696e 7827 2c0a 2020 2020 2020 2020 2020  inx',.          
-00000140: 2773 7068 696e 782d 7274 642d 7468 656d  'sphinx-rtd-them
-00000150: 6527 2c0a 2020 2020 2020 2020 2020 2773  e',.          's
-00000160: 7068 696e 782d 6175 746f 6275 696c 6427  phinx-autobuild'
-00000170: 2c0a 2020 2020 2020 2020 2020 2773 7068  ,.          'sph
-00000180: 696e 782d 6175 746f 646f 632d 7479 7065  inx-autodoc-type
-00000190: 6869 6e74 7327 2c0a 2020 2020 2020 2020  hints',.        
-000001a0: 2020 2773 7068 696e 7863 6f6e 7472 6962    'sphinxcontrib
-000001b0: 2d6d 6572 6d61 6964 275d 2c0a 2027 6475  -mermaid'],. 'du
-000001c0: 636b 6462 3a70 7974 686f 6e5f 7665 7273  ckdb:python_vers
-000001d0: 696f 6e20 3e3d 2022 332e 3822 2061 6e64  ion >= "3.8" and
-000001e0: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
-000001f0: 3c20 2234 2e30 2227 3a20 5b27 6475 636b  < "4.0"': ['duck
-00000200: 6462 3e3d 302e 362e 3027 2c0a 2020 2020  db>=0.6.0',.    
-00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000240: 2020 2020 2020 2020 2020 2027 7079 6172             'pyar
-00000250: 726f 773e 3d35 2e30 2e30 275d 2c0a 2027  row>=5.0.0'],. '
-00000260: 7061 6e64 6173 3a70 7974 686f 6e5f 7665  pandas:python_ve
-00000270: 7273 696f 6e20 3e3d 2022 332e 3822 2061  rsion >= "3.8" a
-00000280: 6e64 2070 7974 686f 6e5f 7665 7273 696f  nd python_versio
-00000290: 6e20 3c20 2234 2e30 2227 3a20 5b27 7061  n < "4.0"': ['pa
-000002a0: 6e64 6173 275d 7d0a 0a73 6574 7570 5f6b  ndas']}..setup_k
-000002b0: 7761 7267 7320 3d20 7b0a 2020 2020 276e  wargs = {.    'n
-000002c0: 616d 6527 3a20 2770 6174 6974 6f27 2c0a  ame': 'patito',.
-000002d0: 2020 2020 2776 6572 7369 6f6e 273a 2027      'version': '
-000002e0: 302e 342e 3427 2c0a 2020 2020 2764 6573  0.4.4',.    'des
-000002f0: 6372 6970 7469 6f6e 273a 2027 4120 6461  cription': 'A da
-00000300: 7461 6672 616d 6520 6d6f 6465 6c6c 696e  taframe modellin
-00000310: 6720 6c69 6272 6172 7920 6275 696c 7420  g library built 
-00000320: 6f6e 2074 6f70 206f 6620 706f 6c61 7273  on top of polars
-00000330: 2061 6e64 2070 7964 616e 7469 632e 272c   and pydantic.',
-00000340: 0a20 2020 2027 6c6f 6e67 5f64 6573 6372  .    'long_descr
-00000350: 6970 7469 6f6e 273a 2027 2320 3c63 656e  iption': '# <cen
-00000360: 7465 723e 3c69 6d67 2068 6569 6768 743d  ter><img height=
-00000370: 2233 3070 7822 2073 7263 3d22 6874 7470  "30px" src="http
-00000380: 733a 2f2f 656d 6f6a 6970 6564 6961 2d75  s://emojipedia-u
-00000390: 732e 7333 2e64 7561 6c73 7461 636b 2e75  s.s3.dualstack.u
-000003a0: 732d 7765 7374 2d31 2e61 6d61 7a6f 6e61  s-west-1.amazona
-000003b0: 7773 2e63 6f6d 2f74 6875 6d62 732f 3132  ws.com/thumbs/12
-000003c0: 302f 7361 6d73 756e 672f 3738 2f64 7563  0/samsung/78/duc
-000003d0: 6b5f 3166 3938 362e 706e 6722 3e20 5061  k_1f986.png"> Pa
-000003e0: 7469 746f 3c63 656e 7465 723e 5c6e 5c6e  tito<center>\n\n
-000003f0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000400: 223e 5c6e 2020 2020 3c65 6d3e 5c6e 2020  ">\n    <em>\n  
-00000410: 2020 2020 2020 5061 7469 746f 2063 6f6d        Patito com
-00000420: 6269 6e65 7320 3c61 2068 7265 663d 2268  bines <a href="h
-00000430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000440: 6d2f 7361 6d75 656c 636f 6c76 696e 2f70  m/samuelcolvin/p
-00000450: 7964 616e 7469 6322 3e70 7964 616e 7469  ydantic">pydanti
-00000460: 633c 2f61 3e20 616e 6420 3c61 2068 7265  c</a> and <a hre
-00000470: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000480: 622e 636f 6d2f 706f 6c61 2d72 732f 706f  b.com/pola-rs/po
-00000490: 6c61 7273 223e 706f 6c61 7273 3c2f 613e  lars">polars</a>
-000004a0: 2069 6e20 6f72 6465 7220 746f 2077 7269   in order to wri
-000004b0: 7465 206d 6f64 6572 6e2c 2074 7970 652d  te modern, type-
-000004c0: 616e 6e6f 7461 7465 6420 6461 7461 2066  annotated data f
-000004d0: 7261 6d65 206c 6f67 6963 2e5c 6e20 2020  rame logic.\n   
-000004e0: 203c 2f65 6d3e 5c6e 2020 2020 3c62 723e   </em>\n    <br>
-000004f0: 5c6e 2020 2020 3c61 2068 7265 663d 2268  \n    <a href="h
-00000500: 7474 7073 3a2f 2f70 6174 6974 6f2e 7265  ttps://patito.re
-00000510: 6164 7468 6564 6f63 732e 696f 2f22 3e5c  adthedocs.io/">\
-00000520: 6e20 2020 2020 2020 203c 696d 6720 7372  n        <img sr
-00000530: 633d 2268 7474 7073 3a2f 2f72 6561 6474  c="https://readt
-00000540: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
-00000550: 6374 732f 7061 7469 746f 2f62 6164 6765  cts/patito/badge
-00000560: 2f22 2061 6c74 3d22 446f 6373 2073 7461  /" alt="Docs sta
-00000570: 7475 7322 3e5c 6e20 2020 203c 2f61 3e5c  tus">\n    </a>\
-00000580: 6e20 2020 203c 6120 6872 6566 3d22 6874  n    <a href="ht
-00000590: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000005a0: 2f6b 6f6c 6f6e 6961 6c6e 6f2f 7061 7469  /kolonialno/pati
-000005b0: 746f 2f61 6374 696f 6e73 3f77 6f72 6b66  to/actions?workf
-000005c0: 6c6f 773d 4349 223e 5c6e 2020 2020 2020  low=CI">\n      
-000005d0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-000005e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-000005f0: 6f6c 6f6e 6961 6c6e 6f2f 7061 7469 746f  olonialno/patito
-00000600: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000610: 7773 2f63 692e 796d 6c2f 6261 6467 652e  ws/ci.yml/badge.
-00000620: 7376 6722 2061 6c74 3d22 4349 2073 7461  svg" alt="CI sta
-00000630: 7475 7322 3e5c 6e20 2020 203c 2f61 3e5c  tus">\n    </a>\
-00000640: 6e20 2020 203c 6120 6872 6566 3d22 6874  n    <a href="ht
-00000650: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000660: 2f67 682f 6b6f 6c6f 6e69 616c 6e6f 2f70  /gh/kolonialno/p
-00000670: 6174 6974 6f22 3e5c 6e20 2020 2020 2020  atito">\n       
-00000680: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000690: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-000006a0: 2f6b 6f6c 6f6e 6961 6c6e 6f2f 7061 7469  /kolonialno/pati
-000006b0: 746f 2f62 7261 6e63 682f 6d61 696e 2f67  to/branch/main/g
-000006c0: 7261 7068 2f62 6164 6765 2e73 7667 3f74  raph/badge.svg?t
-000006d0: 6f6b 656e 3d37 3230 4c42 4459 4832 3522  oken=720LBDYH25"
-000006e0: 2f3e 5c6e 2020 2020 3c2f 613e 5c6e 2020  />\n    </a>\n  
-000006f0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000700: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
-00000710: 7267 2f70 7970 692f 7061 7469 746f 223e  rg/pypi/patito">
-00000720: 5c6e 2020 2020 2020 2020 3c69 6d67 2073  \n        <img s
-00000730: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000740: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000750: 762f 7061 7469 746f 2e73 7667 223e 5c6e  v/patito.svg">\n
-00000760: 2020 2020 3c2f 613e 5c6e 2020 2020 3c69      </a>\n    <i
-00000770: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000780: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000790: 7970 692f 7079 7665 7273 696f 6e73 2f70  ypi/pyversions/p
-000007a0: 6174 6974 6f22 3e5c 6e20 2020 203c 6120  atito">\n    <a 
-000007b0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-000007c0: 7468 7562 2e63 6f6d 2f6b 6f6c 6f6e 6961  thub.com/kolonia
-000007d0: 6c6e 6f2f 7061 7469 746f 2f62 6c6f 622f  lno/patito/blob/
-000007e0: 6d61 7374 6572 2f4c 4943 454e 5345 223e  master/LICENSE">
-000007f0: 5c6e 2020 2020 2020 2020 3c69 6d67 2073  \n        <img s
-00000800: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000810: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000820: 622f 6c69 6365 6e73 652f 6b6f 6c6f 6e69  b/license/koloni
-00000830: 616c 6e6f 2f70 6174 6974 6f2e 7376 6722  alno/patito.svg"
-00000840: 3e5c 6e20 2020 203c 2f61 3e5c 6e3c 2f70  >\n    </a>\n</p
-00000850: 3e5c 6e5c 6e50 6174 6974 6f20 6f66 6665  >\n\nPatito offe
-00000860: 7273 2061 2073 696d 706c 6520 7761 7920  rs a simple way 
-00000870: 746f 2064 6563 6c61 7265 2070 7964 616e  to declare pydan
-00000880: 7469 6320 6461 7461 206d 6f64 656c 7320  tic data models 
-00000890: 7768 6963 6820 646f 7562 6c65 2061 7320  which double as 
-000008a0: 7363 6865 6d61 2066 6f72 2079 6f75 7220  schema for your 
-000008b0: 706f 6c61 7273 2064 6174 6120 6672 616d  polars data fram
-000008c0: 6573 2e5c 6e54 6865 7365 2073 6368 656d  es.\nThese schem
-000008d0: 6120 6361 6e20 6265 2075 7365 6420 666f  a can be used fo
-000008e0: 723a 5c6e 5c6e f09f 91ae 2053 696d 706c  r:\n\n.... Simpl
-000008f0: 6520 616e 6420 7065 7266 6f72 6d61 6e74  e and performant
-00000900: 2064 6174 6120 6672 616d 6520 7661 6c69   data frame vali
-00000910: 6461 7469 6f6e 2e5c 5c5c 6ef0 9fa7 aa20  dation.\\\n.... 
-00000920: 4561 7379 2067 656e 6572 6174 696f 6e20  Easy generation 
-00000930: 6f66 2076 616c 6964 206d 6f63 6b20 6461  of valid mock da
-00000940: 7461 2066 7261 6d65 7320 666f 7220 7465  ta frames for te
-00000950: 7374 732e 5c5c 5c6e f09f 908d 2052 6574  sts.\\\n.... Ret
-00000960: 7269 6576 6520 616e 6420 7265 7072 6573  rieve and repres
-00000970: 656e 7420 7369 6e67 756c 6172 2072 6f77  ent singular row
-00000980: 7320 696e 2061 6e20 6f62 6a65 6374 2d6f  s in an object-o
-00000990: 7269 656e 7465 6420 6d61 6e6e 6572 2e5c  riented manner.\
-000009a0: 5c5c 6ef0 9fa7 a020 5072 6f76 6964 6520  \\n.... Provide 
-000009b0: 6120 7369 6e67 6c65 2073 6f75 7263 6520  a single source 
-000009c0: 6f66 2074 7275 7468 2066 6f72 2074 6865  of truth for the
-000009d0: 2063 6f72 6520 6461 7461 206d 6f64 656c   core data model
-000009e0: 7320 696e 2079 6f75 7220 636f 6465 2062  s in your code b
-000009f0: 6173 652e 205c 5c5c 6ef0 9fa6 8620 496e  ase. \\\n.... In
-00000a00: 7465 6772 6174 696f 6e20 7769 7468 2044  tegration with D
-00000a10: 7563 6b44 4220 666f 7220 7275 6e6e 696e  uckDB for runnin
-00000a20: 6720 666c 6578 6962 6c65 2053 514c 2071  g flexible SQL q
-00000a30: 7565 7269 6573 2e5c 6e5c 6e50 6174 6974  ueries.\n\nPatit
-00000a40: 6f20 6861 7320 6669 7273 742d 636c 6173  o has first-clas
-00000a50: 7320 7375 7070 6f72 7420 666f 7220 5b70  s support for [p
-00000a60: 6f6c 6172 735d 2822 6874 7470 733a 2f2f  olars]("https://
-00000a70: 6769 7468 7562 2e63 6f6d 2f70 6f6c 612d  github.com/pola-
-00000a80: 7273 2f70 6f6c 6172 7322 292c 2061 205f  rs/polars"), a _
-00000a90: 2262 6c61 7a69 6e67 6c79 2066 6173 7420  "blazingly fast 
-00000aa0: 4461 7461 4672 616d 6573 206c 6962 7261  DataFrames libra
-00000ab0: 7279 2077 7269 7474 656e 2069 6e20 5275  ry written in Ru
-00000ac0: 7374 225f 2e5c 6e5c 6e23 2320 496e 7374  st"_.\n\n## Inst
-00000ad0: 616c 6c61 7469 6f6e 5c6e 5c6e 6060 6073  allation\n\n```s
-00000ae0: 685c 6e70 6970 2069 6e73 7461 6c6c 2070  h\npip install p
-00000af0: 6174 6974 6f5c 6e60 6060 5c6e 5c6e 2323  atito\n```\n\n##
-00000b00: 2323 2044 7563 6b44 4220 496e 7465 6772  ## DuckDB Integr
-00000b10: 6174 696f 6e5c 6e5c 6e50 6174 6974 6f20  ation\n\nPatito 
-00000b20: 6361 6e20 616c 736f 2069 6e74 6567 7261  can also integra
-00000b30: 7465 2077 6974 6820 5b44 7563 6b44 425d  te with [DuckDB]
-00000b40: 2868 7474 7073 3a2f 2f64 7563 6b64 622e  (https://duckdb.
-00000b50: 6f72 672f 292e 5c6e 496e 206f 7264 6572  org/).\nIn order
-00000b60: 2074 6f20 656e 6162 6c65 2074 6869 7320   to enable this 
-00000b70: 696e 7465 6772 6174 696f 6e20 796f 7520  integration you 
-00000b80: 6d75 7374 2065 7870 6c69 6369 746c 7920  must explicitly 
-00000b90: 7370 6563 6966 7920 6974 2064 7572 696e  specify it durin
-00000ba0: 6720 696e 7374 616c 6c61 7469 6f6e 3a5c  g installation:\
-00000bb0: 6e5c 6e60 6060 7368 5c6e 7069 7020 696e  n\n```sh\npip in
-00000bc0: 7374 616c 6c20 5c27 7061 7469 746f 5b64  stall \'patito[d
-00000bd0: 7563 6b64 625d 5c27 5c6e 6060 605c 6e5c  uckdb]\'\n```\n\
-00000be0: 6e5c 6e23 2320 446f 6375 6d65 6e74 6174  n\n## Documentat
-00000bf0: 696f 6e5c 6e5c 6e54 6865 2066 756c 6c20  ion\n\nThe full 
-00000c00: 646f 6375 6d65 6e74 6174 696f 6e20 6f66  documentation of
-00000c10: 2050 6174 696f 2063 616e 2062 6520 666f   Patio can be fo
-00000c20: 756e 6420 5b68 6572 655d 2868 7474 7073  und [here](https
-00000c30: 3a2f 2f70 6174 6974 6f2e 7265 6164 7468  ://patito.readth
-00000c40: 6564 6f63 732e 696f 292e 5c6e 5c6e 2323  edocs.io).\n\n##
-00000c50: 20f0 9f91 ae20 4461 7461 2076 616c 6964   .... Data valid
-00000c60: 6174 696f 6e5c 6e5c 6e50 6174 6974 6f20  ation\n\nPatito 
-00000c70: 616c 6c6f 7773 2079 6f75 2074 6f20 7370  allows you to sp
-00000c80: 6563 6966 7920 7468 6520 7479 7065 206f  ecify the type o
-00000c90: 6620 6561 6368 2063 6f6c 756d 6e20 696e  f each column in
-00000ca0: 2079 6f75 7220 6461 7461 6672 616d 6520   your dataframe 
-00000cb0: 6279 2063 7265 6174 696e 6720 6120 7479  by creating a ty
-00000cc0: 7065 2d61 6e6e 6f74 6174 6564 2073 7562  pe-annotated sub
-00000cd0: 636c 6173 7320 6f66 2060 7061 7469 746f  class of `patito
-00000ce0: 2e4d 6f64 656c 603a 5c6e 5c6e 6060 6070  .Model`:\n\n```p
-00000cf0: 795c 6e23 206d 6f64 656c 732e 7079 5c6e  y\n# models.py\n
-00000d00: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000d10: 7274 204c 6974 6572 616c 2c20 4f70 7469  rt Literal, Opti
-00000d20: 6f6e 616c 5c6e 5c6e 696d 706f 7274 2070  onal\n\nimport p
-00000d30: 6174 6974 6f20 6173 2070 745c 6e5c 6e5c  atito as pt\n\n\
-00000d40: 6e63 6c61 7373 2050 726f 6475 6374 2870  nclass Product(p
-00000d50: 742e 4d6f 6465 6c29 3a5c 6e20 2020 2070  t.Model):\n    p
-00000d60: 726f 6475 6374 5f69 643a 2069 6e74 203d  roduct_id: int =
-00000d70: 2070 742e 4669 656c 6428 756e 6971 7565   pt.Field(unique
-00000d80: 3d54 7275 6529 5c6e 2020 2020 7465 6d70  =True)\n    temp
-00000d90: 6572 6174 7572 655f 7a6f 6e65 3a20 4c69  erature_zone: Li
-00000da0: 7465 7261 6c5b 2264 7279 222c 2022 636f  teral["dry", "co
-00000db0: 6c64 222c 2022 6672 6f7a 656e 225d 5c6e  ld", "frozen"]\n
-00000dc0: 2020 2020 6973 5f66 6f72 5f73 616c 653a      is_for_sale:
-00000dd0: 2062 6f6f 6c5c 6e60 6060 5c6e 5c6e 5468   bool\n```\n\nTh
-00000de0: 6520 2a2a 636c 6173 732a 2a20 6050 726f  e **class** `Pro
-00000df0: 6475 6374 6020 7265 7072 6573 656e 7473  duct` represents
-00000e00: 2074 6865 202a 2a73 6368 656d 612a 2a20   the **schema** 
-00000e10: 6f66 2074 6865 2064 6174 6120 6672 616d  of the data fram
-00000e20: 652c 2077 6869 6c65 202a 2a69 6e73 7461  e, while **insta
-00000e30: 6e63 6573 2a2a 206f 6620 6050 726f 6475  nces** of `Produ
-00000e40: 6374 6020 7265 7072 6573 656e 7420 7369  ct` represent si
-00000e50: 6e67 6c65 202a 2a72 6f77 732a 2a20 6f66  ngle **rows** of
-00000e60: 2074 6865 2064 6174 6166 7261 6d65 2e5c   the dataframe.\
-00000e70: 6e50 6174 6974 6f20 6361 6e20 6566 6669  nPatito can effi
-00000e80: 6369 656e 746c 7920 7661 6c69 6461 7465  ciently validate
-00000e90: 2074 6865 2063 6f6e 7465 6e74 206f 6620   the content of 
-00000ea0: 6172 6269 7472 6172 7920 6461 7461 2066  arbitrary data f
-00000eb0: 7261 6d65 7320 616e 6420 7072 6f76 6964  rames and provid
-00000ec0: 6520 6875 6d61 6e2d 7265 6164 6162 6c65  e human-readable
-00000ed0: 2065 7272 6f72 206d 6573 7361 6765 733a   error messages:
-00000ee0: 5c6e 5c6e 6060 6070 795c 6e69 6d70 6f72  \n\n```py\nimpor
-00000ef0: 7420 706f 6c61 7273 2061 7320 706c 5c6e  t polars as pl\n
-00000f00: 5c6e 6466 203d 2070 6c2e 4461 7461 4672  \ndf = pl.DataFr
-00000f10: 616d 6528 5c6e 2020 2020 7b5c 6e20 2020  ame(\n    {\n   
-00000f20: 2020 2020 2022 7072 6f64 7563 745f 6964       "product_id
-00000f30: 223a 205b 312c 2031 2c20 335d 2c5c 6e20  ": [1, 1, 3],\n 
-00000f40: 2020 2020 2020 2022 7465 6d70 6572 6174         "temperat
-00000f50: 7572 655f 7a6f 6e65 223a 205b 2264 7279  ure_zone": ["dry
-00000f60: 222c 2022 6472 7922 2c20 226f 7665 6e22  ", "dry", "oven"
-00000f70: 5d2c 5c6e 2020 2020 7d5c 6e29 5c6e 7472  ],\n    }\n)\ntr
-00000f80: 793a 5c6e 2020 2020 5072 6f64 7563 742e  y:\n    Product.
-00000f90: 7661 6c69 6461 7465 2864 6629 5c6e 6578  validate(df)\nex
-00000fa0: 6365 7074 2070 742e 5661 6c69 6461 7469  cept pt.Validati
-00000fb0: 6f6e 4572 726f 7220 6173 2065 7863 3a5c  onError as exc:\
-00000fc0: 6e20 2020 2070 7269 6e74 2865 7863 295c  n    print(exc)\
-00000fd0: 6e23 2033 2076 616c 6964 6174 696f 6e20  n# 3 validation 
-00000fe0: 6572 726f 7273 2066 6f72 2050 726f 6475  errors for Produ
-00000ff0: 6374 5c6e 2320 6973 5f66 6f72 5f73 616c  ct\n# is_for_sal
-00001000: 655c 6e23 2020 204d 6973 7369 6e67 2063  e\n#   Missing c
-00001010: 6f6c 756d 6e20 2874 7970 653d 7479 7065  olumn (type=type
-00001020: 5f65 7272 6f72 2e6d 6973 7369 6e67 636f  _error.missingco
-00001030: 6c75 6d6e 7329 5c6e 2320 7072 6f64 7563  lumns)\n# produc
-00001040: 745f 6964 5c6e 2320 2020 3220 726f 7773  t_id\n#   2 rows
-00001050: 2077 6974 6820 6475 706c 6963 6174 6564   with duplicated
-00001060: 2076 616c 7565 732e 2028 7479 7065 3d76   values. (type=v
-00001070: 616c 7565 5f65 7272 6f72 2e72 6f77 7661  alue_error.rowva
-00001080: 6c75 6529 5c6e 2320 7465 6d70 6572 6174  lue)\n# temperat
-00001090: 7572 655f 7a6f 6e65 5c6e 2320 2020 526f  ure_zone\n#   Ro
-000010a0: 7773 2077 6974 6820 696e 7661 6c69 6420  ws with invalid 
-000010b0: 7661 6c75 6573 3a20 7b5c 276f 7665 6e5c  values: {\'oven\
-000010c0: 277d 2e20 2874 7970 653d 7661 6c75 655f  '}. (type=value_
-000010d0: 6572 726f 722e 726f 7776 616c 7565 295c  error.rowvalue)\
-000010e0: 6e60 6060 5c6e 5c6e 3c64 6574 6169 6c73  n```\n\n<details
-000010f0: 3e5c 6e3c 7375 6d6d 6172 793e 3c62 3e43  >\n<summary><b>C
-00001100: 6c69 636b 2074 6f20 7365 6520 6120 7375  lick to see a su
-00001110: 6d6d 6172 7920 6f66 2064 6174 6166 7261  mmary of datafra
-00001120: 6d65 2d63 6f6d 7061 7469 626c 6520 7479  me-compatible ty
-00001130: 7065 2061 6e6e 6f74 6174 696f 6e73 2e3c  pe annotations.<
-00001140: 2f62 3e3c 2f73 756d 6d61 7279 3e5c 6e5c  /b></summary>\n\
-00001150: 6e2a 2052 6567 756c 6172 2070 7974 686f  n* Regular pytho
-00001160: 6e20 6461 7461 2074 7970 6573 2073 7563  n data types suc
-00001170: 6820 6173 2060 696e 7460 2c20 6066 6c6f  h as `int`, `flo
-00001180: 6174 602c 2060 626f 6f6c 602c 2060 7374  at`, `bool`, `st
-00001190: 7260 2c20 6064 6174 6560 2c20 7768 6963  r`, `date`, whic
-000011a0: 6820 6172 6520 7661 6c69 6461 7465 6420  h are validated 
-000011b0: 6167 6169 6e73 7420 636f 6d70 6174 6962  against compatib
-000011c0: 6c65 2070 6f6c 6172 7320 6461 7461 2074  le polars data t
-000011d0: 7970 6573 2e5c 6e2a 2057 7261 7070 696e  ypes.\n* Wrappin
-000011e0: 6720 796f 7572 2074 7970 6520 7769 7468  g your type with
-000011f0: 2060 7479 7069 6e67 2e4f 7074 696f 6e61   `typing.Optiona
-00001200: 6c60 2069 6e64 6963 6174 6573 2074 6861  l` indicates tha
-00001210: 7420 7468 6520 6769 7665 6e20 636f 6c75  t the given colu
-00001220: 6d6e 2061 6363 6570 7473 206d 6973 7369  mn accepts missi
-00001230: 6e67 2076 616c 7565 732e 5c6e 2a20 4d6f  ng values.\n* Mo
-00001240: 6465 6c20 6669 656c 6473 2061 6e6e 6f74  del fields annot
-00001250: 6174 6564 2077 6974 6820 6074 7970 696e  ated with `typin
-00001260: 672e 4c69 7465 7261 6c5b 2e2e 2e5d 6020  g.Literal[...]` 
-00001270: 6368 6563 6b20 6966 206f 6e6c 7920 6120  check if only a 
-00001280: 7265 7374 7269 6374 6564 2073 6574 206f  restricted set o
-00001290: 6620 7661 6c75 6573 2061 7265 2074 616b  f values are tak
-000012a0: 656e 2c20 6569 7468 6572 2061 7320 7468  en, either as th
-000012b0: 6520 6e61 7469 7665 2064 7479 7065 2028  e native dtype (
-000012c0: 652e 672e 2060 706c 2e55 7466 3860 2920  e.g. `pl.Utf8`) 
-000012d0: 6f72 2060 706c 2e43 6174 6567 6f72 6963  or `pl.Categoric
-000012e0: 616c 602e 5c6e 5c6e 4164 6469 746f 6e61  al`.\n\nAdditona
-000012f0: 6c6c 792c 2079 6f75 2063 616e 2061 7373  lly, you can ass
-00001300: 6967 6e20 6070 6174 6974 6f2e 4669 656c  ign `patito.Fiel
-00001310: 6460 2074 6f20 796f 7572 2063 6c61 7373  d` to your class
-00001320: 2076 6172 6961 626c 6573 2069 6e20 6f72   variables in or
-00001330: 6465 7220 746f 2073 7065 6369 6679 2061  der to specify a
-00001340: 6464 6974 696f 6e61 6c20 6368 6563 6b73  dditional checks
-00001350: 3a5c 6e5c 6e2a 2060 4669 656c 6428 6474  :\n\n* `Field(dt
-00001360: 7970 653d 2e2e 2e29 6020 656e 7375 7265  ype=...)` ensure
-00001370: 7320 7468 6174 2061 2073 7065 6369 6669  s that a specifi
-00001380: 6320 6474 7970 6520 6973 2075 7365 6420  c dtype is used 
-00001390: 696e 2074 686f 7365 2063 6173 6573 2077  in those cases w
-000013a0: 6865 7265 2073 6576 6572 616c 2064 6174  here several dat
-000013b0: 6120 7479 7065 7320 6172 6520 636f 6d70  a types are comp
-000013c0: 6c69 616e 7420 7769 7468 2074 6865 2061  liant with the a
-000013d0: 6e6e 6f74 6174 6564 2070 7974 686f 6e20  nnotated python 
-000013e0: 7479 7065 2c20 666f 7220 6578 616d 706c  type, for exampl
-000013f0: 6520 6070 726f 6475 6374 5f69 643a 2069  e `product_id: i
-00001400: 6e74 203d 2046 6965 6c64 2864 7479 7065  nt = Field(dtype
-00001410: 3d70 6c2e 5549 6e74 3332 2960 2e5c 6e2a  =pl.UInt32)`.\n*
-00001420: 2060 4669 656c 6428 756e 6971 7565 3d54   `Field(unique=T
-00001430: 7275 6529 6020 6368 6563 6b73 2069 6620  rue)` checks if 
-00001440: 6576 6572 7920 726f 7720 6861 7320 6120  every row has a 
-00001450: 756e 6971 7565 2076 616c 7565 2e5c 6e2a  unique value.\n*
-00001460: 2060 4669 656c 6428 6774 3d2e 2e2e 2c20   `Field(gt=..., 
-00001470: 6765 3d2e 2e2e 2c20 6c65 3d2e 2e2e 2c20  ge=..., le=..., 
-00001480: 6c74 3d2e 2e2e 2960 2061 6c6c 6f77 7320  lt=...)` allows 
-00001490: 796f 7520 746f 2073 7065 6369 6679 2062  you to specify b
-000014a0: 6f75 6e64 2063 6865 636b 7320 666f 7220  ound checks for 
-000014b0: 616e 7920 636f 6d62 696e 6174 696f 6e20  any combination 
-000014c0: 6f66 2060 3e20 6774 602c 2060 3e3d 2067  of `> gt`, `>= g
-000014d0: 6560 2c20 603c 3d20 6c65 6020 603c 206c  e`, `<= le` `< l
-000014e0: 7460 2c20 7265 7370 6563 7469 7665 6c79  t`, respectively
-000014f0: 2e5c 6e2a 2060 4669 656c 6428 6d75 6c74  .\n* `Field(mult
-00001500: 6970 6c65 5f6f 663d 6469 7669 736f 7229  iple_of=divisor)
-00001510: 6020 696e 206f 7264 6572 2074 6f20 6368  ` in order to ch
-00001520: 6563 6b20 6966 2061 2067 6976 656e 2063  eck if a given c
-00001530: 6f6c 756d 6e20 6f6e 6c79 2063 6f6e 7461  olumn only conta
-00001540: 696e 7320 7661 6c75 6573 2061 7320 6d75  ins values as mu
-00001550: 6c74 6970 6c65 7320 6f66 2074 6865 2067  ltiples of the g
-00001560: 6976 656e 2076 616c 7565 2e5c 6e2a 2060  iven value.\n* `
-00001570: 4669 656c 6428 6465 6661 756c 743d 6465  Field(default=de
-00001580: 6661 756c 745f 7661 6c75 652c 2063 6f6e  fault_value, con
-00001590: 7374 3d54 7275 6529 6020 696e 6469 6361  st=True)` indica
-000015a0: 7465 7320 7468 6174 2074 6865 2067 6976  tes that the giv
-000015b0: 656e 2063 6f6c 756d 6e20 6973 2072 6571  en column is req
-000015c0: 7569 7265 6420 616e 6420 5f6d 7573 745f  uired and _must_
-000015d0: 2074 616b 6520 7468 6520 6769 7665 6e20   take the given 
-000015e0: 6465 6661 756c 7420 7661 6c75 652e 5c6e  default value.\n
-000015f0: 2a20 5374 7269 6e67 2066 6965 6c64 7320  * String fields 
-00001600: 616e 6e6f 7461 7465 6420 7769 7468 2060  annotated with `
-00001610: 4669 656c 6428 7265 6765 783d 7222 3c72  Field(regex=r"<r
-00001620: 6567 6578 2d70 6174 7465 726e 3e22 2960  egex-pattern>")`
-00001630: 2c20 6046 6965 6c64 286d 6178 5f6c 656e  , `Field(max_len
-00001640: 6774 683d 626f 756e 6429 602c 2061 6e64  gth=bound)`, and
-00001650: 2f6f 7220 6046 6965 6c64 286d 696e 5f6c  /or `Field(min_l
-00001660: 656e 6774 6829 6020 7769 6c6c 2062 6520  ength)` will be 
-00001670: 7661 6c69 6461 7465 6420 7769 7468 205b  validated with [
-00001680: 706f 6c61 7273 5c27 2065 6666 6963 6965  polars\' efficie
-00001690: 6e74 2073 7472 696e 6720 7072 6f63 6573  nt string proces
-000016a0: 7369 6e67 2063 6170 6162 696c 6974 6965  sing capabilitie
-000016b0: 735d 2868 7474 7073 3a2f 2f70 6f6c 612d  s](https://pola-
-000016c0: 7273 2e67 6974 6875 622e 696f 2f70 6f6c  rs.github.io/pol
-000016d0: 6172 732d 626f 6f6b 2f75 7365 722d 6775  ars-book/user-gu
-000016e0: 6964 652f 686f 7763 616e 692f 6461 7461  ide/howcani/data
-000016f0: 2f73 7472 696e 6773 2e68 746d 6c29 2e5c  /strings.html).\
-00001700: 6e2a 2043 7573 746f 6d20 636f 6e73 7472  n* Custom constr
-00001710: 6169 6e74 7320 6361 6e20 6265 2073 7065  aints can be spe
-00001720: 6369 6669 6564 2077 6974 6820 7769 7468  cified with with
-00001730: 2060 4669 656c 6428 636f 6e73 7472 6169   `Field(constrai
-00001740: 6e74 733d 2e2e 2e29 602c 2065 6974 6865  nts=...)`, eithe
-00001750: 7220 6173 2061 2073 696e 676c 6520 706f  r as a single po
-00001760: 6c61 7273 2065 7870 7265 7373 696f 6e20  lars expression 
-00001770: 6f72 2061 206c 6973 7420 6f66 2065 7870  or a list of exp
-00001780: 7265 7373 696f 6e73 2e20 416c 6c20 7468  ressions. All th
-00001790: 6520 726f 7773 206f 6620 7468 6520 6461  e rows of the da
-000017a0: 7461 6672 616d 6520 6d75 7374 2073 6174  taframe must sat
-000017b0: 6973 6679 2074 6865 2067 6976 656e 2063  isfy the given c
-000017c0: 6f6e 7374 7261 696e 7428 7329 2069 6e20  onstraint(s) in 
-000017d0: 6f72 6465 7220 746f 2062 6520 636f 6e73  order to be cons
-000017e0: 6964 6572 6564 2076 616c 6964 2e20 4578  idered valid. Ex
-000017f0: 616d 706c 653a 2060 6576 656e 5f66 6965  ample: `even_fie
-00001800: 6c64 3a20 696e 7420 3d20 7074 2e46 6965  ld: int = pt.Fie
-00001810: 6c64 2863 6f6e 7374 7261 696e 7473 3d70  ld(constraints=p
-00001820: 6c2e 636f 6c28 2265 7665 6e5f 6669 656c  l.col("even_fiel
-00001830: 6422 2920 2520 3220 3d3d 2030 2960 2e5c  d") % 2 == 0)`.\
-00001840: 6e5c 6e41 6c74 686f 7567 6820 5061 7469  n\nAlthough Pati
-00001850: 746f 2073 7570 706f 7274 7320 5b70 616e  to supports [pan
-00001860: 6461 735d 2868 7474 7073 3a2f 2f67 6974  das](https://git
-00001870: 6875 622e 636f 6d2f 7061 6e64 6173 2d64  hub.com/pandas-d
-00001880: 6576 2f70 616e 6461 7329 2c20 6974 2069  ev/pandas), it i
-00001890: 7320 6869 6768 6c79 2072 6563 6f6d 6d65  s highly recomme
-000018a0: 6d65 6e64 6564 2074 6f20 6265 2075 7365  mended to be use
-000018b0: 6420 696e 2063 6f6d 6269 6e61 7469 6f6e  d in combination
-000018c0: 2077 6974 6820 5b70 6f6c 6172 735d 2822   with [polars]("
-000018d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000018e0: 6f6d 2f70 6f6c 612d 7273 2f70 6f6c 6172  om/pola-rs/polar
-000018f0: 7322 292e 5c6e 466f 7220 6120 6d75 6368  s").\nFor a much
-00001900: 206d 6f72 6520 6665 6174 7572 652d 636f   more feature-co
-00001910: 6d70 6c65 7465 2c20 7061 6e64 6173 2d66  mplete, pandas-f
-00001920: 6972 7374 206c 6962 7261 7279 2c20 7461  irst library, ta
-00001930: 6b65 2061 206c 6f6f 6b20 6174 205b 7061  ke a look at [pa
-00001940: 6e64 6572 615d 2868 7474 7073 3a2f 2f70  ndera](https://p
-00001950: 616e 6465 7261 2e72 6561 6474 6865 646f  andera.readthedo
-00001960: 6373 2e69 6f2f 292e 5c6e 3c2f 6465 7461  cs.io/).\n</deta
-00001970: 696c 733e 5c6e 5c6e 2323 20f0 9fa7 aa20  ils>\n\n## .... 
-00001980: 5379 6e74 6865 7369 7a65 2076 616c 6964  Synthesize valid
-00001990: 2074 6573 7420 6461 7461 5c6e 5c6e 5061   test data\n\nPa
-000019a0: 7469 746f 2065 6e63 6f75 7261 6765 7320  tito encourages 
-000019b0: 796f 7520 746f 2073 7472 6963 746c 7920  you to strictly 
-000019c0: 7661 6c69 6461 7465 2064 6174 6166 7261  validate datafra
-000019d0: 6d65 2069 6e70 7574 732c 2074 6875 7320  me inputs, thus 
-000019e0: 656e 7375 7269 6e67 2063 6f72 7265 6374  ensuring correct
-000019f0: 6e65 7373 2061 7420 7275 6e74 696d 652e  ness at runtime.
-00001a00: 5c6e 4275 7420 7769 7468 2066 6f72 6365  \nBut with force
-00001a10: 6420 636f 7272 6563 746e 6573 7320 636f  d correctness co
-00001a20: 6d65 7320 6672 6963 7469 6f6e 2c20 6573  mes friction, es
-00001a30: 7065 6369 616c 6c79 2064 7572 696e 6720  pecially during 
-00001a40: 7465 7374 696e 672e 5c6e 5461 6b65 2074  testing.\nTake t
-00001a50: 6865 2066 6f6c 6c6f 7769 6e67 2066 756e  he following fun
-00001a60: 6374 696f 6e20 6173 2061 6e20 6578 616d  ction as an exam
-00001a70: 706c 653a 5c6e 5c6e 6060 6070 795c 6e69  ple:\n\n```py\ni
-00001a80: 6d70 6f72 7420 706f 6c61 7273 2061 7320  mport polars as 
-00001a90: 706c 5c6e 5c6e 6465 6620 6e75 6d5f 7072  pl\n\ndef num_pr
-00001aa0: 6f64 7563 7473 5f66 6f72 5f73 616c 6528  oducts_for_sale(
-00001ab0: 7072 6f64 7563 7473 3a20 706c 2e44 6174  products: pl.Dat
-00001ac0: 6146 7261 6d65 2920 2d3e 2069 6e74 3a5c  aFrame) -> int:\
-00001ad0: 6e20 2020 2050 726f 6475 6374 2e76 616c  n    Product.val
-00001ae0: 6964 6174 6528 7072 6f64 7563 7473 295c  idate(products)\
-00001af0: 6e20 2020 2072 6574 7572 6e20 7072 6f64  n    return prod
-00001b00: 7563 7473 2e66 696c 7465 7228 706c 2e63  ucts.filter(pl.c
-00001b10: 6f6c 2822 6973 5f66 6f72 5f73 616c 6522  ol("is_for_sale"
-00001b20: 2929 2e68 6569 6768 745c 6e60 6060 5c6e  )).height\n```\n
-00001b30: 5c6e 5468 6520 666f 6c6c 6f77 696e 6720  \nThe following 
-00001b40: 7465 7374 2077 6f75 6c64 2066 6169 6c20  test would fail 
-00001b50: 7769 7468 2061 2060 7061 7469 746f 2e56  with a `patito.V
-00001b60: 616c 6964 6174 696f 6e45 7272 6f72 603a  alidationError`:
-00001b70: 5c6e 5c6e 6060 6070 795c 6e64 6566 2074  \n\n```py\ndef t
-00001b80: 6573 745f 6e75 6d5f 7072 6f64 7563 7473  est_num_products
-00001b90: 5f66 6f72 5f73 616c 6528 293a 5c6e 2020  _for_sale():\n  
-00001ba0: 2020 7072 6f64 7563 7473 203d 2070 6c2e    products = pl.
-00001bb0: 4461 7461 4672 616d 6528 7b22 6973 5f66  DataFrame({"is_f
-00001bc0: 6f72 5f73 616c 6522 3a20 5b54 7275 652c  or_sale": [True,
-00001bd0: 2054 7275 652c 2046 616c 7365 5d7d 295c   True, False]})\
-00001be0: 6e20 2020 2061 7373 6572 7420 6e75 6d5f  n    assert num_
-00001bf0: 7072 6f64 7563 7473 5f66 6f72 5f73 616c  products_for_sal
-00001c00: 6528 7072 6f64 7563 7473 2920 3d3d 2032  e(products) == 2
-00001c10: 5c6e 6060 605c 6e5c 6e49 6e20 6f72 6465  \n```\n\nIn orde
-00001c20: 7220 746f 206d 616b 6520 7468 6520 7465  r to make the te
-00001c30: 7374 2070 6173 7320 7765 2077 6f75 6c64  st pass we would
-00001c40: 2068 6176 6520 746f 2061 6464 2076 616c   have to add val
-00001c50: 6964 2064 756d 6d79 2064 6174 6120 666f  id dummy data fo
-00001c60: 7220 7468 6520 6074 656d 7065 7261 7475  r the `temperatu
-00001c70: 7265 5f7a 6f6e 6560 2061 6e64 2060 7072  re_zone` and `pr
-00001c80: 6f64 7563 745f 6964 6020 636f 6c75 6d6e  oduct_id` column
-00001c90: 732e 5c6e 5468 6973 2077 696c 6c20 7175  s.\nThis will qu
-00001ca0: 6963 6b6c 7920 696e 7472 6f64 7563 6520  ickly introduce 
-00001cb0: 6120 6c6f 7420 6f66 2062 6f69 6c65 7270  a lot of boilerp
-00001cc0: 6c61 7465 2074 6f20 616c 6c20 7465 7374  late to all test
-00001cd0: 7320 696e 766f 6c76 696e 6720 6461 7461  s involving data
-00001ce0: 2066 7261 6d65 732c 206f 6273 6375 7269   frames, obscuri
-00001cf0: 6e67 2077 6861 7420 6973 2061 6374 7561  ng what is actua
-00001d00: 6c6c 7920 6265 696e 6720 7465 7374 6564  lly being tested
-00001d10: 2069 6e20 6561 6368 2074 6573 742e 5c6e   in each test.\n
-00001d20: 466f 7220 7468 6973 2072 6561 736f 6e20  For this reason 
-00001d30: 5061 7469 746f 2070 726f 7669 6465 7320  Patito provides 
-00001d40: 7468 6520 6065 7861 6d70 6c65 7360 2063  the `examples` c
-00001d50: 6f6e 7374 7275 6374 6f72 2066 6f72 2067  onstructor for g
-00001d60: 656e 6572 6174 696e 6720 7465 7374 2064  enerating test d
-00001d70: 6174 6120 7468 6174 2069 7320 6675 6c6c  ata that is full
-00001d80: 7920 636f 6d70 6c69 616e 7420 7769 7468  y compliant with
-00001d90: 2074 6865 2067 6976 656e 206d 6f64 656c   the given model
-00001da0: 2073 6368 656d 612e 5c6e 5c6e 6060 6070   schema.\n\n```p
-00001db0: 795c 6e50 726f 6475 6374 2e65 7861 6d70  y\nProduct.examp
-00001dc0: 6c65 7328 7b22 6973 5f66 6f72 5f73 616c  les({"is_for_sal
-00001dd0: 6522 3a20 5b54 7275 652c 2054 7275 652c  e": [True, True,
-00001de0: 2046 616c 7365 5d7d 295c 6e23 2073 6861   False]})\n# sha
-00001df0: 7065 3a20 2833 2c20 3329 5c6e 2320 e294  pe: (3, 3)\n# ..
-00001e00: 8ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001e10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001e20: 9480 e294 80e2 9480 e294 ace2 9480 e294  ................
-00001e30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001e40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001e50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001e60: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-00001e70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001e80: 9480 e294 80e2 9480 e294 905c 6e23 20e2  ...........\n# .
-00001e90: 9482 2069 735f 666f 725f 7361 6c65 20e2  .. is_for_sale .
-00001ea0: 9486 2074 656d 7065 7261 7475 7265 5f7a  .. temperature_z
-00001eb0: 6f6e 6520 e294 8620 7072 6f64 7563 745f  one ... product_
-00001ec0: 6964 20e2 9482 5c6e 2320 e294 8220 2d2d  id ...\n# ... --
-00001ed0: 2d20 2020 2020 2020 2020 e294 8620 2d2d  -         ... --
-00001ee0: 2d20 2020 2020 2020 2020 2020 2020 20e2  -              .
-00001ef0: 9486 202d 2d2d 2020 2020 2020 2020 e294  .. ---        ..
-00001f00: 825c 6e23 20e2 9482 2062 6f6f 6c20 2020  .\n# ... bool   
-00001f10: 2020 2020 20e2 9486 2073 7472 2020 2020       ... str    
-00001f20: 2020 2020 2020 2020 2020 e294 8620 6936            ... i6
-00001f30: 3420 2020 2020 2020 20e2 9482 5c6e 2320  4        ...\n# 
-00001f40: e295 9ee2 9590 e295 90e2 9590 e295 90e2  ................
-00001f50: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
-00001f60: 90e2 9590 e295 90e2 9590 e295 aae2 9590  ................
-00001f70: e295 90e2 9590 e295 90e2 9590 e295 90e2  ................
-00001f80: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
-00001f90: 90e2 9590 e295 90e2 9590 e295 90e2 9590  ................
-00001fa0: e295 90e2 95aa e295 90e2 9590 e295 90e2  ................
-00001fb0: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
-00001fc0: 90e2 9590 e295 90e2 9590 e295 a15c 6e23  .............\n#
-00001fd0: 20e2 9482 2074 7275 6520 2020 2020 2020   ... true       
-00001fe0: 20e2 9486 2064 7279 2020 2020 2020 2020   ... dry        
-00001ff0: 2020 2020 2020 e294 8620 3020 2020 2020        ... 0     
-00002000: 2020 2020 20e2 9482 5c6e 2320 e294 9ce2       ...\n# ....
-00002010: 958c e295 8ce2 958c e295 8ce2 958c e295  ................
-00002020: 8ce2 958c e295 8ce2 958c e295 8ce2 958c  ................
-00002030: e295 8ce2 958c e294 bce2 958c e295 8ce2  ................
-00002040: 958c e295 8ce2 958c e295 8ce2 958c e295  ................
-00002050: 8ce2 958c e295 8ce2 958c e295 8ce2 958c  ................
-00002060: e295 8ce2 958c e295 8ce2 958c e295 8ce2  ................
-00002070: 94bc e295 8ce2 958c e295 8ce2 958c e295  ................
-00002080: 8ce2 958c e295 8ce2 958c e295 8ce2 958c  ................
-00002090: e295 8ce2 958c e294 a45c 6e23 20e2 9482  .........\n# ...
-000020a0: 2074 7275 6520 2020 2020 2020 20e2 9486   true        ...
-000020b0: 2064 7279 2020 2020 2020 2020 2020 2020   dry            
-000020c0: 2020 e294 8620 3120 2020 2020 2020 2020    ... 1         
-000020d0: 20e2 9482 5c6e 2320 e294 9ce2 958c e295   ...\n# ........
-000020e0: 8ce2 958c e295 8ce2 958c e295 8ce2 958c  ................
-000020f0: e295 8ce2 958c e295 8ce2 958c e295 8ce2  ................
-00002100: 958c e294 bce2 958c e295 8ce2 958c e295  ................
-00002110: 8ce2 958c e295 8ce2 958c e295 8ce2 958c  ................
-00002120: e295 8ce2 958c e295 8ce2 958c e295 8ce2  ................
-00002130: 958c e295 8ce2 958c e295 8ce2 94bc e295  ................
-00002140: 8ce2 958c e295 8ce2 958c e295 8ce2 958c  ................
-00002150: e295 8ce2 958c e295 8ce2 958c e295 8ce2  ................
-00002160: 958c e294 a45c 6e23 20e2 9482 2066 616c  .....\n# ... fal
-00002170: 7365 2020 2020 2020 20e2 9486 2064 7279  se       ... dry
-00002180: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-00002190: 8620 3220 2020 2020 2020 2020 20e2 9482  . 2          ...
-000021a0: 5c6e 2320 e294 94e2 9480 e294 80e2 9480  \n# ............
-000021b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000021c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000021d0: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000021e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000021f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002200: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
-00002210: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002220: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002230: 985c 6e60 6060 5c6e 5c6e 5468 6520 6065  .\n```\n\nThe `e
-00002240: 7861 6d70 6c65 7328 2960 206d 6574 686f  xamples()` metho
-00002250: 6420 6163 6365 7074 7320 7468 6520 7361  d accepts the sa
-00002260: 6d65 2061 7267 756d 656e 7473 2061 7320  me arguments as 
-00002270: 6120 7265 6775 6c61 7220 6461 7461 2066  a regular data f
-00002280: 7261 6d65 2063 6f6e 7374 7275 6374 6f72  rame constructor
-00002290: 2c20 7468 6520 6d61 696e 2064 6966 6665  , the main diffe
-000022a0: 7265 6e63 6520 6265 696e 6720 7468 6174  rence being that
-000022b0: 2069 7420 6669 6c6c 7320 696e 2076 616c   it fills in val
-000022c0: 6964 2064 756d 6d79 2064 6174 6120 666f  id dummy data fo
-000022d0: 7220 616e 7920 756e 7370 6563 6966 6965  r any unspecifie
-000022e0: 6420 636f 6c75 6d6e 732e 5c6e 5468 6520  d columns.\nThe 
-000022f0: 7465 7374 2063 616e 2074 6865 7265 666f  test can therefo
-00002300: 7265 2062 6520 7265 7772 6974 7465 6e20  re be rewritten 
-00002310: 6173 3a5c 6e5c 6e60 6060 7079 5c6e 6465  as:\n\n```py\nde
-00002320: 6620 7465 7374 5f6e 756d 5f70 726f 6475  f test_num_produ
-00002330: 6374 735f 666f 725f 7361 6c65 2829 3a5c  cts_for_sale():\
-00002340: 6e20 2020 2070 726f 6475 6374 7320 3d20  n    products = 
-00002350: 5072 6f64 7563 742e 6578 616d 706c 6573  Product.examples
-00002360: 287b 2269 735f 666f 725f 7361 6c65 223a  ({"is_for_sale":
-00002370: 205b 5472 7565 2c20 5472 7565 2c20 4661   [True, True, Fa
-00002380: 6c73 655d 7d29 5c6e 2020 2020 6173 7365  lse]})\n    asse
-00002390: 7274 206e 756d 5f70 726f 6475 6374 735f  rt num_products_
-000023a0: 666f 725f 7361 6c65 2870 726f 6475 6374  for_sale(product
-000023b0: 7329 203d 3d20 325c 6e60 6060 5c6e 5c6e  s) == 2\n```\n\n
-000023c0: 2323 20f0 9f96 bcef b88f 2041 206d 6f64  ## ....... A mod
-000023d0: 656c 2d61 7761 7265 2064 6174 6120 6672  el-aware data fr
-000023e0: 616d 6520 636c 6173 735c 6e50 6174 6974  ame class\nPatit
-000023f0: 6f20 6f66 6665 7273 2060 7061 7469 746f  o offers `patito
-00002400: 2e44 6174 6146 7261 6d65 602c 2061 2063  .DataFrame`, a c
-00002410: 6c61 7373 2074 6861 7420 6578 7465 6e64  lass that extend
-00002420: 7320 6070 6f6c 6172 732e 4461 7461 4672  s `polars.DataFr
-00002430: 616d 6560 2069 6e20 6f72 6465 7220 746f  ame` in order to
-00002440: 2070 726f 7669 6465 2075 7469 6c69 7479   provide utility
-00002450: 206d 6574 686f 6473 2072 656c 6174 6564   methods related
-00002460: 2074 6f20 6070 6174 6974 6f2e 4d6f 6465   to `patito.Mode
-00002470: 6c60 2e5c 6e54 6865 2073 6368 656d 6120  l`.\nThe schema 
-00002480: 6f66 2061 2064 6174 6120 6672 616d 6520  of a data frame 
-00002490: 6361 6e20 6265 2073 7065 6369 6669 6564  can be specified
-000024a0: 2061 7420 7275 6e74 696d 6520 6279 2069   at runtime by i
-000024b0: 6e76 6f6b 696e 6720 6070 6174 6974 6f2e  nvoking `patito.
-000024c0: 4461 7461 4672 616d 652e 7365 745f 6d6f  DataFrame.set_mo
-000024d0: 6465 6c28 6d6f 6465 6c29 602c 2061 6674  del(model)`, aft
-000024e0: 6572 2077 6869 6368 2061 2073 6574 206f  er which a set o
-000024f0: 6620 636f 6e74 6578 7475 616c 697a 6564  f contextualized
-00002500: 206d 6574 686f 6473 2062 6563 6f6d 6520   methods become 
-00002510: 6176 6169 6c61 626c 653a 5c6e 5c6e 2a20  available:\n\n* 
-00002520: 6044 6174 6146 7261 6d65 2e76 616c 6964  `DataFrame.valid
-00002530: 6174 6528 2960 202d 2056 616c 6964 6174  ate()` - Validat
-00002540: 6520 7468 6520 6769 7665 6e20 6461 7461  e the given data
-00002550: 2066 7261 6d65 2061 6e64 2072 6574 7572   frame and retur
-00002560: 6e20 6974 7365 6c66 2e5c 6e2a 2060 4461  n itself.\n* `Da
-00002570: 7461 4672 616d 652e 6472 6f70 2829 6020  taFrame.drop()` 
-00002580: 2d20 4472 6f70 2061 6c6c 2073 7570 6572  - Drop all super
-00002590: 666c 756f 7573 2063 6f6c 756d 6e73 205f  fluous columns _
-000025a0: 6e6f 745f 2073 7065 6369 6669 6564 2061  not_ specified a
-000025b0: 7320 6669 656c 6473 2069 6e20 7468 6520  s fields in the 
-000025c0: 6d6f 6465 6c2e 5c6e 2a20 6044 6174 6146  model.\n* `DataF
-000025d0: 7261 6d65 2e63 6173 7428 2960 202d 2043  rame.cast()` - C
-000025e0: 6173 7420 616e 7920 636f 6c75 6d6e 7320  ast any columns 
-000025f0: 7768 6963 6820 6172 6520 6e6f 7420 636f  which are not co
-00002600: 6d70 6174 6962 6c65 2077 6974 6820 7468  mpatible with th
-00002610: 6520 6769 7665 6e20 7479 7065 2061 6e6e  e given type ann
-00002620: 6f74 6174 696f 6e73 2e20 5768 656e 2060  otations. When `
-00002630: 4669 656c 6428 6474 7970 653d 2e2e 2e29  Field(dtype=...)
-00002640: 6020 6973 2073 7065 6369 6669 6564 2c20  ` is specified, 
-00002650: 7468 6520 6769 7665 6e20 6474 7970 6520  the given dtype 
-00002660: 7769 6c6c 2061 6c77 6179 7320 6265 2066  will always be f
-00002670: 6f72 6365 642c 2065 7665 6e20 696e 2063  orced, even in c
-00002680: 6f6d 7061 7469 626c 6520 6361 7365 732e  ompatible cases.
-00002690: 5c6e 2a20 6044 6174 6146 7261 6d65 2e67  \n* `DataFrame.g
-000026a0: 6574 2870 7265 6469 6361 7465 2960 202d  et(predicate)` -
-000026b0: 2052 6574 7269 6576 6520 6120 7369 6e67   Retrieve a sing
-000026c0: 6c65 2072 6f77 2066 726f 6d20 7468 6520  le row from the 
-000026d0: 6461 7461 2066 7261 6d65 2061 7320 616e  data frame as an
-000026e0: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
-000026f0: 206d 6f64 656c 2e20 416e 2065 7863 6570   model. An excep
-00002700: 7469 6f6e 2069 7320 7261 6973 6564 2069  tion is raised i
-00002710: 6620 6e6f 7420 6578 6163 746c 7920 6f6e  f not exactly on
-00002720: 6520 726f 7720 6973 2079 6965 6c64 6564  e row is yielded
-00002730: 2066 726f 6d20 7468 6520 6669 6c74 6572   from the filter
-00002740: 2070 7265 6469 6361 7465 2e5c 6e2a 2060   predicate.\n* `
-00002750: 4461 7461 4672 616d 652e 6669 6c6c 5f6e  DataFrame.fill_n
-00002760: 756c 6c28 7374 7261 7465 6779 3d22 6465  ull(strategy="de
-00002770: 6661 756c 7473 2229 6020 2d20 4669 6c6c  faults")` - Fill
-00002780: 2069 6e6e 206d 6973 7369 6e67 2076 616c   inn missing val
-00002790: 7565 7320 6163 636f 7264 696e 6720 746f  ues according to
-000027a0: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
-000027b0: 7565 7320 7365 7420 6f6e 2074 6865 206d  ues set on the m
-000027c0: 6f64 656c 2073 6368 656d 612e 5c6e 2a20  odel schema.\n* 
-000027d0: 6044 6174 6146 7261 6d65 2e64 6572 6976  `DataFrame.deriv
-000027e0: 6528 2960 202d 2041 206d 6f64 656c 2066  e()` - A model f
-000027f0: 6965 6c64 2061 6e6e 6f74 6174 6564 2077  ield annotated w
-00002800: 6974 6820 6046 6965 6c64 2864 6572 6976  ith `Field(deriv
-00002810: 6564 5f66 726f 6d3d 2e2e 2e29 6020 696e  ed_from=...)` in
-00002820: 6469 6361 7465 7320 7468 6174 2061 2063  dicates that a c
-00002830: 6f6c 756d 6e20 7368 6f75 6c64 2062 6520  olumn should be 
-00002840: 6465 6669 6e65 6420 6279 2073 6f6d 6520  defined by some 
-00002850: 6172 6269 7472 6172 7920 706f 6c61 7273  arbitrary polars
-00002860: 2065 7870 7265 7373 696f 6e2e 2049 6620   expression. If 
-00002870: 6064 6572 6976 6564 5f66 726f 6d60 2069  `derived_from` i
-00002880: 7320 7370 6563 6966 6965 6420 6173 2061  s specified as a
-00002890: 2073 7472 696e 672c 2074 6865 6e20 7468   string, then th
-000028a0: 6520 6769 7665 6e20 7661 6c75 6520 7769  e given value wi
-000028b0: 6c6c 2062 6520 696e 7465 7270 7265 7465  ll be interprete
-000028c0: 6420 6173 2061 2063 6f6c 756d 6e20 6e61  d as a column na
-000028d0: 6d65 2077 6974 6820 6070 6f6c 6172 732e  me with `polars.
-000028e0: 636f 6c28 2960 2e20 5468 6573 6520 636f  col()`. These co
-000028f0: 6c75 6d6e 7320 6172 6520 6372 6561 7465  lumns are create
-00002900: 6420 616e 6420 706f 7075 6c61 7465 6420  d and populated 
-00002910: 7769 7468 2064 6174 6120 6163 636f 7264  with data accord
-00002920: 696e 6720 746f 2074 6865 2060 6465 7269  ing to the `deri
-00002930: 7665 645f 6672 6f6d 6020 6578 7072 6573  ved_from` expres
-00002940: 7369 6f6e 7320 7768 656e 2079 6f75 2069  sions when you i
-00002950: 6e76 6f6b 6520 6044 6174 6146 7261 6d65  nvoke `DataFrame
-00002960: 2e64 6572 6976 6528 2960 2e5c 6e5c 6e54  .derive()`.\n\nT
-00002970: 6865 7365 206d 6574 686f 6473 2061 7265  hese methods are
-00002980: 2062 6573 7420 696c 6c75 7374 7261 7465   best illustrate
-00002990: 6420 7769 7468 2061 6e20 6578 616d 706c  d with an exampl
-000029a0: 653a 5c6e 5c6e 6060 6070 795c 6e66 726f  e:\n\n```py\nfro
-000029b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000029c0: 4c69 7465 7261 6c5c 6e5c 6e69 6d70 6f72  Literal\n\nimpor
-000029d0: 7420 7061 7469 746f 2061 7320 7074 5c6e  t patito as pt\n
-000029e0: 696d 706f 7274 2070 6f6c 6172 7320 6173  import polars as
-000029f0: 2070 6c5c 6e5c 6e5c 6e63 6c61 7373 2050   pl\n\n\nclass P
-00002a00: 726f 6475 6374 2870 742e 4d6f 6465 6c29  roduct(pt.Model)
-00002a10: 3a5c 6e20 2020 2070 726f 6475 6374 5f69  :\n    product_i
-00002a20: 643a 2069 6e74 203d 2070 742e 4669 656c  d: int = pt.Fiel
-00002a30: 6428 756e 6971 7565 3d54 7275 6529 5c6e  d(unique=True)\n
-00002a40: 2020 2020 2320 5370 6563 6966 7920 6120      # Specify a 
-00002a50: 7370 6563 6966 6963 2064 7479 7065 2074  specific dtype t
-00002a60: 6f20 6265 2075 7365 645c 6e20 2020 2070  o be used\n    p
-00002a70: 6f70 756c 6172 6974 795f 7261 6e6b 3a20  opularity_rank: 
-00002a80: 696e 7420 3d20 7074 2e46 6965 6c64 2864  int = pt.Field(d
-00002a90: 7479 7065 3d70 6c2e 5549 6e74 3136 295c  type=pl.UInt16)\
-00002aa0: 6e20 2020 2023 2046 6965 6c64 2077 6974  n    # Field wit
-00002ab0: 6820 6465 6661 756c 7420 7661 6c75 6520  h default value 
-00002ac0: 2266 6f72 2d73 616c 6522 5c6e 2020 2020  "for-sale"\n    
-00002ad0: 7374 6174 7573 3a20 4c69 7465 7261 6c5b  status: Literal[
-00002ae0: 2264 7261 6674 222c 2022 666f 722d 7361  "draft", "for-sa
-00002af0: 6c65 222c 2022 6469 7363 6f6e 7469 6e75  le", "discontinu
-00002b00: 6564 225d 203d 2022 666f 722d 7361 6c65  ed"] = "for-sale
-00002b10: 225c 6e20 2020 2023 2054 6865 2065 7572  "\n    # The eur
-00002b20: 6f63 656e 7420 636f 7374 2069 7320 6578  ocent cost is ex
-00002b30: 7472 6163 7465 6420 6672 6f6d 2074 6865  tracted from the
-00002b40: 2045 7572 6f20 636f 7374 2073 7472 696e   Euro cost strin
-00002b50: 6720 22e2 82ac 582e 5920 4555 5222 5c6e  g "...X.Y EUR"\n
-00002b60: 2020 2020 6575 726f 6365 6e74 5f63 6f73      eurocent_cos
-00002b70: 743a 2069 6e74 203d 2070 742e 4669 656c  t: int = pt.Fiel
-00002b80: 6428 5c6e 2020 2020 2020 2020 6465 7269  d(\n        deri
-00002b90: 7665 645f 6672 6f6d 3d31 3030 202a 2070  ved_from=100 * p
-00002ba0: 6c2e 636f 6c28 2263 6f73 7422 292e 7374  l.col("cost").st
-00002bb0: 722e 6578 7472 6163 7428 7222 e282 ac28  r.extract(r"...(
-00002bc0: 5c5c 642b 5c5c 2e2b 5c5c 642b 2922 292e  \\d+\\.+\\d+)").
-00002bd0: 6361 7374 2866 6c6f 6174 292e 726f 756e  cast(float).roun
-00002be0: 6428 3229 5c6e 2020 2020 295c 6e5c 6e5c  d(2)\n    )\n\n\
-00002bf0: 6e70 726f 6475 6374 7320 3d20 7074 2e44  nproducts = pt.D
-00002c00: 6174 6146 7261 6d65 285c 6e20 2020 207b  ataFrame(\n    {
-00002c10: 5c6e 2020 2020 2020 2020 2270 726f 6475  \n        "produ
-00002c20: 6374 5f69 6422 3a20 5b31 2c20 325d 2c5c  ct_id": [1, 2],\
-00002c30: 6e20 2020 2020 2020 2022 706f 7075 6c61  n        "popula
-00002c40: 7269 7479 5f72 616e 6b22 3a20 5b32 2c20  rity_rank": [2, 
-00002c50: 315d 2c5c 6e20 2020 2020 2020 2022 7374  1],\n        "st
-00002c60: 6174 7573 223a 205b 4e6f 6e65 2c20 2264  atus": [None, "d
-00002c70: 6973 636f 6e74 696e 7565 6422 5d2c 5c6e  iscontinued"],\n
-00002c80: 2020 2020 2020 2020 2263 6f73 7422 3a20          "cost": 
-00002c90: 5b22 e282 ac32 2e33 3020 4555 5222 2c20  ["...2.30 EUR", 
-00002ca0: 22e2 82ac 312e 3139 2045 5552 225d 2c5c  "...1.19 EUR"],\
-00002cb0: 6e20 2020 207d 5c6e 295c 6e70 726f 6475  n    }\n)\nprodu
-00002cc0: 6374 203d 2028 5c6e 2020 2020 7072 6f64  ct = (\n    prod
-00002cd0: 7563 7473 5c6e 2020 2020 2320 5370 6563  ucts\n    # Spec
-00002ce0: 6966 7920 7468 6520 7363 6865 6d61 206f  ify the schema o
-00002cf0: 6620 7468 6520 6769 7665 6e20 6461 7461  f the given data
-00002d00: 2066 7261 6d65 5c6e 2020 2020 2e73 6574   frame\n    .set
-00002d10: 5f6d 6f64 656c 2850 726f 6475 6374 295c  _model(Product)\
-00002d20: 6e20 2020 2023 2044 6572 6976 6520 7468  n    # Derive th
-00002d30: 6520 6065 7572 6f63 656e 745f 636f 7374  e `eurocent_cost
-00002d40: 6020 696e 7420 636f 6c75 6d6e 2066 726f  ` int column fro
-00002d50: 6d20 7468 6520 6063 6f73 7460 2073 7472  m the `cost` str
-00002d60: 696e 6720 636f 6c75 6d6e 2075 7369 6e67  ing column using
-00002d70: 2072 6567 6578 5c6e 2020 2020 2e64 6572   regex\n    .der
-00002d80: 6976 6528 295c 6e20 2020 2023 2044 726f  ive()\n    # Dro
-00002d90: 7020 7468 6520 6063 6f73 7460 2063 6f6c  p the `cost` col
-00002da0: 756d 6e20 6173 2069 7420 6973 206e 6f74  umn as it is not
-00002db0: 2070 6172 7420 6f66 2074 6865 206d 6f64   part of the mod
-00002dc0: 656c 5c6e 2020 2020 2e64 726f 7028 295c  el\n    .drop()\
-00002dd0: 6e20 2020 2023 2043 6173 7420 7468 6520  n    # Cast the 
-00002de0: 706f 7075 6c61 7269 7479 2072 616e 6b20  popularity rank 
-00002df0: 636f 6c75 6d6e 2074 6f20 616e 2075 6e73  column to an uns
-00002e00: 6967 6e65 6420 3136 2d62 6974 2069 6e74  igned 16-bit int
-00002e10: 6567 6572 2061 6e64 2063 656e 7473 2074  eger and cents t
-00002e20: 6f20 616e 2069 6e74 6567 6572 5c6e 2020  o an integer\n  
-00002e30: 2020 2e63 6173 7428 295c 6e20 2020 2023    .cast()\n    #
-00002e40: 2046 696c 6c20 6d69 7373 696e 6720 7661   Fill missing va
-00002e50: 6c75 6573 2077 6974 6820 7468 6520 6465  lues with the de
-00002e60: 6661 756c 7420 7661 6c75 6573 2073 7065  fault values spe
-00002e70: 6369 6669 6564 2069 6e20 7468 6520 7363  cified in the sc
-00002e80: 6865 6d61 5c6e 2020 2020 2e66 696c 6c5f  hema\n    .fill_
-00002e90: 6e75 6c6c 2873 7472 6174 6567 793d 2264  null(strategy="d
-00002ea0: 6566 6175 6c74 7322 295c 6e20 2020 2023  efaults")\n    #
-00002eb0: 2041 7373 6572 7420 7468 6174 2074 6865   Assert that the
-00002ec0: 2064 6174 6120 6672 616d 6520 6e6f 7720   data frame now 
-00002ed0: 636f 6d70 6c69 6573 2077 6974 6820 7468  complies with th
-00002ee0: 6520 7363 6865 6d61 5c6e 2020 2020 2e76  e schema\n    .v
-00002ef0: 616c 6964 6174 6528 295c 6e20 2020 2023  alidate()\n    #
-00002f00: 2052 6574 7269 6576 6520 6120 7369 6e67   Retrieve a sing
-00002f10: 6c65 2072 6f77 2061 6e64 2063 6173 7420  le row and cast 
-00002f20: 6974 2074 6f20 7468 6520 6d6f 6465 6c20  it to the model 
-00002f30: 636c 6173 735c 6e20 2020 202e 6765 7428  class\n    .get(
-00002f40: 706c 2e63 6f6c 2822 7072 6f64 7563 745f  pl.col("product_
-00002f50: 6964 2229 203d 3d20 3129 5c6e 295c 6e70  id") == 1)\n)\np
-00002f60: 7269 6e74 2872 6570 7228 7072 6f64 7563  rint(repr(produc
-00002f70: 7429 295c 6e23 2050 726f 6475 6374 2870  t))\n# Product(p
-00002f80: 726f 6475 6374 5f69 643d 312c 2070 6f70  roduct_id=1, pop
-00002f90: 756c 6172 6974 795f 7261 6e6b 3d32 2c20  ularity_rank=2, 
-00002fa0: 7374 6174 7573 3d5c 2766 6f72 2d73 616c  status=\'for-sal
-00002fb0: 655c 272c 2065 7572 6f63 656e 745f 636f  e\', eurocent_co
-00002fc0: 7374 3d32 3330 295c 6e60 6060 5c6e 5c6e  st=230)\n```\n\n
-00002fd0: 4576 6572 7920 5061 7469 746f 206d 6f64  Every Patito mod
-00002fe0: 656c 2061 7574 6f6d 6174 6963 616c 6c79  el automatically
-00002ff0: 2067 6574 7320 6120 602e 4461 7461 4672   gets a `.DataFr
-00003000: 616d 6560 2061 7474 7269 6275 7465 2c20  ame` attribute, 
-00003010: 6120 6375 7374 6f6d 2064 6174 6120 6672  a custom data fr
-00003020: 616d 6520 7375 6263 6c61 7373 2077 6865  ame subclass whe
-00003030: 7265 2060 2e73 6574 5f6d 6f64 656c 2829  re `.set_model()
-00003040: 6020 6973 2069 6e76 6f6b 6564 2061 7420  ` is invoked at 
-00003050: 696e 7374 616e 7469 6174 696f 6e2e 2057  instantiation. W
-00003060: 6974 6820 6f74 6865 7220 776f 7264 732c  ith other words,
-00003070: 2060 7074 2e44 6174 6146 7261 6d65 282e   `pt.DataFrame(.
-00003080: 2e2e 292e 7365 745f 6d6f 6465 6c28 5072  ..).set_model(Pr
-00003090: 6f64 7563 7429 6020 6973 2065 7175 6976  oduct)` is equiv
-000030a0: 616c 656e 7420 746f 2060 5072 6f64 7563  alent to `Produc
-000030b0: 742e 4461 7461 4672 616d 6528 2e2e 2e29  t.DataFrame(...)
-000030c0: 602e 5c6e 5c6e 2323 20f0 9f90 8d20 5265  `.\n\n## .... Re
-000030d0: 7072 6573 656e 7469 6e67 2072 6f77 7320  presenting rows 
-000030e0: 6173 2063 6c61 7373 6573 5c6e 5c6e 4461  as classes\n\nDa
-000030f0: 7461 2066 7261 6d65 7320 6172 6520 7461  ta frames are ta
-00003100: 696c 6f72 2d6d 6164 6520 666f 7220 7065  ilor-made for pe
-00003110: 7266 6f72 6d69 6e67 2076 6563 746f 7269  rforming vectori
-00003120: 7a65 6420 6f70 6572 6174 696f 6e73 206f  zed operations o
-00003130: 7665 7220 6120 5f73 6574 5f20 6f66 206f  ver a _set_ of o
-00003140: 626a 6563 7473 2e5c 6e42 7574 2077 6865  bjects.\nBut whe
-00003150: 6e20 7468 6520 7469 6d65 2063 6f6d 6573  n the time comes
-00003160: 2074 6f20 7265 7472 6965 7669 6e67 2061   to retrieving a
-00003170: 205f 7369 6e67 6c65 5f20 726f 7720 616e   _single_ row an
-00003180: 6420 6f70 6572 6174 6520 7570 6f6e 2069  d operate upon i
-00003190: 742c 2074 6865 2064 6174 6120 6672 616d  t, the data fram
-000031a0: 6520 636f 6e73 7472 7563 7420 6e61 7475  e construct natu
-000031b0: 7261 6c6c 7920 6661 6c6c 7320 7368 6f72  rally falls shor
-000031c0: 742e 5c6e 5061 7469 746f 2061 6c6c 6f77  t.\nPatito allow
-000031d0: 7320 796f 7520 746f 2065 6d62 6564 2072  s you to embed r
-000031e0: 6f77 2d6c 6576 656c 206c 6f67 6963 2069  ow-level logic i
-000031f0: 6e20 6d65 7468 6f64 7320 6465 6669 6e65  n methods define
-00003200: 6420 6f6e 2074 6865 206d 6f64 656c 2e5c  d on the model.\
-00003210: 6e5c 6e5c 6e60 6060 7079 5c6e 2320 6d6f  n\n\n```py\n# mo
-00003220: 6465 6c73 2e70 795c 6e69 6d70 6f72 7420  dels.py\nimport 
-00003230: 7061 7469 746f 2061 7320 7074 5c6e 5c6e  patito as pt\n\n
-00003240: 636c 6173 7320 5072 6f64 7563 7428 7074  class Product(pt
-00003250: 2e4d 6f64 656c 293a 5c6e 2020 2020 7072  .Model):\n    pr
-00003260: 6f64 7563 745f 6964 3a20 696e 7420 3d20  oduct_id: int = 
-00003270: 7074 2e46 6965 6c64 2875 6e69 7175 653d  pt.Field(unique=
-00003280: 5472 7565 295c 6e20 2020 206e 616d 653a  True)\n    name:
-00003290: 2073 7472 5c6e 5c6e 2020 2020 4070 726f   str\n\n    @pro
-000032a0: 7065 7274 795c 6e20 2020 2064 6566 2075  perty\n    def u
-000032b0: 726c 2873 656c 6629 202d 3e20 7374 723a  rl(self) -> str:
-000032c0: 5c6e 2020 2020 2020 2020 7265 7475 726e  \n        return
-000032d0: 2028 5c6e 2020 2020 2020 2020 2020 2020   (\n            
-000032e0: 2268 7474 7073 3a2f 2f6f 6461 2e63 6f6d  "https://oda.com
-000032f0: 2f6e 6f2f 7072 6f64 7563 7473 2f22 5c6e  /no/products/"\n
-00003300: 2020 2020 2020 2020 2020 2020 6622 7b73              f"{s
-00003310: 656c 662e 7072 6f64 7563 745f 6964 7d2d  elf.product_id}-
-00003320: 225c 6e20 2020 2020 2020 2020 2020 2066  "\n            f
-00003330: 227b 7365 6c66 2e6e 616d 652e 6c6f 7765  "{self.name.lowe
-00003340: 7228 292e 7265 706c 6163 6528 5c27 205c  r().replace(\' \
-00003350: 272c 205c 272d 5c27 297d 225c 6e20 2020  ', \'-\')}"\n   
-00003360: 2020 2020 2029 5c6e 6060 605c 6e5c 6e54       )\n```\n\nT
-00003370: 6865 2063 6c61 7373 2063 616e 2062 6520  he class can be 
-00003380: 696e 7374 616e 7469 6174 6564 2066 726f  instantiated fro
-00003390: 6d20 6120 7369 6e67 6c65 2072 6f77 206f  m a single row o
-000033a0: 6620 6120 6461 7461 2066 7261 6d65 2062  f a data frame b
-000033b0: 7920 7573 696e 6720 7468 6520 6066 726f  y using the `fro
-000033c0: 6d5f 726f 7728 2960 206d 6574 686f 643a  m_row()` method:
-000033d0: 5c6e 5c6e 6060 6070 795c 6e70 726f 6475  \n\n```py\nprodu
-000033e0: 6374 7320 3d20 706c 2e44 6174 6146 7261  cts = pl.DataFra
-000033f0: 6d65 285c 6e20 2020 207b 5c6e 2020 2020  me(\n    {\n    
-00003400: 2020 2020 2270 726f 6475 6374 5f69 6422      "product_id"
-00003410: 3a20 5b31 2c20 325d 2c5c 6e20 2020 2020  : [1, 2],\n     
-00003420: 2020 2022 6e61 6d65 223a 205b 2253 6b69     "name": ["Ski
-00003430: 6d6d 6564 206d 696c 6b22 2c20 2245 6767  mmed milk", "Egg
-00003440: 7322 5d2c 5c6e 2020 2020 7d5c 6e29 5c6e  s"],\n    }\n)\n
-00003450: 6d69 6c6b 5f72 6f77 203d 2070 726f 6475  milk_row = produ
-00003460: 6374 732e 6669 6c74 6572 2870 6c2e 636f  cts.filter(pl.co
-00003470: 6c28 2270 726f 6475 6374 5f69 6422 203d  l("product_id" =
-00003480: 3d20 3129 295c 6e6d 696c 6b20 3d20 5072  = 1))\nmilk = Pr
-00003490: 6f64 7563 742e 6672 6f6d 5f72 6f77 286d  oduct.from_row(m
-000034a0: 696c 6b5f 726f 7729 5c6e 7072 696e 7428  ilk_row)\nprint(
-000034b0: 6d69 6c6b 2e75 726c 295c 6e23 2068 7474  milk.url)\n# htt
-000034c0: 7073 3a2f 2f6f 6461 2e63 6f6d 2f6e 6f2f  ps://oda.com/no/
-000034d0: 7072 6f64 7563 7473 2f31 2d73 6b69 6d6d  products/1-skimm
-000034e0: 6564 2d6d 696c 6b5c 6e60 6060 5c6e 5c6e  ed-milk\n```\n\n
-000034f0: 4966 2079 6f75 2022 636f 6e6e 6563 7422  If you "connect"
-00003500: 2074 6865 2060 5072 6f64 7563 7460 206d   the `Product` m
-00003510: 6f64 656c 2077 6974 6820 7468 6520 6044  odel with the `D
-00003520: 6174 6146 7261 6d65 6020 6279 2074 6865  ataFrame` by the
-00003530: 2075 7365 206f 6620 6070 6174 6974 6f2e   use of `patito.
-00003540: 4461 7461 4672 616d 652e 7365 745f 6d6f  DataFrame.set_mo
-00003550: 6465 6c28 2960 2c20 6f72 2061 6c74 6572  del()`, or alter
-00003560: 6e61 7469 7665 6c79 2062 7920 7573 696e  natively by usin
-00003570: 6720 6050 726f 6475 6374 2e44 6174 6146  g `Product.DataF
-00003580: 7261 6d65 6020 6469 7265 6374 6c79 2c20  rame` directly, 
-00003590: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
-000035a0: 602e 6765 7428 2960 206d 6574 686f 6420  `.get()` method 
-000035b0: 696e 206f 7264 6572 2074 6f20 6669 6c74  in order to filt
-000035c0: 6572 2074 6865 2064 6174 6120 6672 616d  er the data fram
-000035d0: 6520 646f 776e 2074 6f20 6120 7369 6e67  e down to a sing
-000035e0: 6c65 2072 6f77 205f 616e 645f 2063 6173  le row _and_ cas
-000035f0: 7420 6974 2074 6f20 7468 6520 7265 7370  t it to the resp
-00003600: 6563 7469 7665 206d 6f64 656c 2063 6c61  ective model cla
-00003610: 7373 3a5c 6e5c 6e60 6060 7079 5c6e 5c6e  ss:\n\n```py\n\n
-00003620: 7072 6f64 7563 7473 203d 2050 726f 6475  products = Produ
-00003630: 6374 2e44 6174 6146 7261 6d65 285c 6e20  ct.DataFrame(\n 
-00003640: 2020 207b 5c6e 2020 2020 2020 2020 2270     {\n        "p
-00003650: 726f 6475 6374 5f69 6422 3a20 5b31 2c20  roduct_id": [1, 
-00003660: 325d 2c5c 6e20 2020 2020 2020 2022 6e61  2],\n        "na
-00003670: 6d65 223a 205b 2253 6b69 6d6d 6564 206d  me": ["Skimmed m
-00003680: 696c 6b22 2c20 2245 6767 7322 5d2c 5c6e  ilk", "Eggs"],\n
-00003690: 2020 2020 7d5c 6e29 5c6e 6d69 6c6b 203d      }\n)\nmilk =
-000036a0: 2070 726f 6475 6374 732e 6765 7428 706c   products.get(pl
-000036b0: 2e63 6f6c 2822 7072 6f64 7563 745f 6964  .col("product_id
-000036c0: 2229 203d 3d20 3129 5c6e 7072 696e 7428  ") == 1)\nprint(
-000036d0: 6d69 6c6b 2e75 726c 295c 6e23 2068 7474  milk.url)\n# htt
-000036e0: 7073 3a2f 2f6f 6461 2e63 6f6d 2f6e 6f2f  ps://oda.com/no/
-000036f0: 7072 6f64 7563 7473 2f31 2d73 6b69 6d6d  products/1-skimm
-00003700: 6564 2d6d 696c 6b5c 6e60 6060 5c6e 272c  ed-milk\n```\n',
-00003710: 0a20 2020 2027 6175 7468 6f72 273a 2027  .    'author': '
-00003720: 4a61 6b6f 6220 4765 7268 6172 6420 4d61  Jakob Gerhard Ma
-00003730: 7274 696e 7573 7365 6e27 2c0a 2020 2020  rtinussen',.    
-00003740: 2761 7574 686f 725f 656d 6169 6c27 3a20  'author_email': 
-00003750: 276a 616b 6f62 676d 4067 6d61 696c 2e63  'jakobgm@gmail.c
-00003760: 6f6d 272c 0a20 2020 2027 6d61 696e 7461  om',.    'mainta
-00003770: 696e 6572 273a 2027 4e6f 6e65 272c 0a20  iner': 'None',. 
-00003780: 2020 2027 6d61 696e 7461 696e 6572 5f65     'maintainer_e
-00003790: 6d61 696c 273a 2027 4e6f 6e65 272c 0a20  mail': 'None',. 
-000037a0: 2020 2027 7572 6c27 3a20 2768 7474 7073     'url': 'https
-000037b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b6f  ://github.com/ko
-000037c0: 6c6f 6e69 616c 6e6f 2f70 6174 6974 6f27  lonialno/patito'
-000037d0: 2c0a 2020 2020 2770 6163 6b61 6765 5f64  ,.    'package_d
-000037e0: 6972 273a 2070 6163 6b61 6765 5f64 6972  ir': package_dir
-000037f0: 2c0a 2020 2020 2770 6163 6b61 6765 7327  ,.    'packages'
-00003800: 3a20 7061 636b 6167 6573 2c0a 2020 2020  : packages,.    
-00003810: 2770 6163 6b61 6765 5f64 6174 6127 3a20  'package_data': 
-00003820: 7061 636b 6167 655f 6461 7461 2c0a 2020  package_data,.  
-00003830: 2020 2769 6e73 7461 6c6c 5f72 6571 7569    'install_requi
-00003840: 7265 7327 3a20 696e 7374 616c 6c5f 7265  res': install_re
-00003850: 7175 6972 6573 2c0a 2020 2020 2765 7874  quires,.    'ext
-00003860: 7261 735f 7265 7175 6972 6527 3a20 6578  ras_require': ex
-00003870: 7472 6173 5f72 6571 7569 7265 2c0a 2020  tras_require,.  
-00003880: 2020 2770 7974 686f 6e5f 7265 7175 6972    'python_requir
-00003890: 6573 273a 2027 3e3d 332e 372c 3c34 2e30  es': '>=3.7,<4.0
-000038a0: 272c 0a7d 0a0a 0a73 6574 7570 282a 2a73  ',.}...setup(**s
-000038b0: 6574 7570 5f6b 7761 7267 7329 0a         etup_kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7061 7469  : 2.1.Name: pati
+00000020: 746f 0a56 6572 7369 6f6e 3a20 302e 352e  to.Version: 0.5.
+00000030: 300a 5375 6d6d 6172 793a 2041 2064 6174  0.Summary: A dat
+00000040: 6166 7261 6d65 206d 6f64 656c 6c69 6e67  aframe modelling
+00000050: 206c 6962 7261 7279 2062 7569 6c74 206f   library built o
+00000060: 6e20 746f 7020 6f66 2070 6f6c 6172 7320  n top of polars 
+00000070: 616e 6420 7079 6461 6e74 6963 2e0a 486f  and pydantic..Ho
+00000080: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000090: 2f67 6974 6875 622e 636f 6d2f 6b6f 6c6f  /github.com/kolo
+000000a0: 6e69 616c 6e6f 2f70 6174 6974 6f0a 4c69  nialno/patito.Li
+000000b0: 6365 6e73 653a 204d 4954 0a4b 6579 776f  cense: MIT.Keywo
+000000c0: 7264 733a 2076 616c 6964 6174 696f 6e2c  rds: validation,
+000000d0: 6461 7461 6672 616d 650a 4175 7468 6f72  dataframe.Author
+000000e0: 3a20 4a61 6b6f 6220 4765 7268 6172 6420  : Jakob Gerhard 
+000000f0: 4d61 7274 696e 7573 7365 6e0a 4175 7468  Martinussen.Auth
+00000100: 6f72 2d65 6d61 696c 3a20 6a61 6b6f 6267  or-email: jakobg
+00000110: 6d40 676d 6169 6c2e 636f 6d0a 5265 7175  m@gmail.com.Requ
+00000120: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
+00000130: 2e38 2c3c 342e 300a 436c 6173 7369 6669  .8,<4.0.Classifi
+00000140: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
+00000150: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000160: 4954 204c 6963 656e 7365 0a43 6c61 7373  IT License.Class
+00000170: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000180: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000190: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
+000001a0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001c0: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
+000001d0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000001e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001f0: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
+00000200: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000210: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000220: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000230: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
+00000240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000250: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000260: 332e 3131 0a50 726f 7669 6465 732d 4578  3.11.Provides-Ex
+00000270: 7472 613a 2063 6163 6869 6e67 0a50 726f  tra: caching.Pro
+00000280: 7669 6465 732d 4578 7472 613a 2064 6f63  vides-Extra: doc
+00000290: 730a 5072 6f76 6964 6573 2d45 7874 7261  s.Provides-Extra
+000002a0: 3a20 6475 636b 6462 0a50 726f 7669 6465  : duckdb.Provide
+000002b0: 732d 4578 7472 613a 2070 616e 6461 730a  s-Extra: pandas.
+000002c0: 5265 7175 6972 6573 2d44 6973 743a 2053  Requires-Dist: S
+000002d0: 7068 696e 7820 283c 3729 203b 2065 7874  phinx (<7) ; ext
+000002e0: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
+000002f0: 7569 7265 732d 4469 7374 3a20 6475 636b  uires-Dist: duck
+00000300: 6462 2028 3e3d 302e 362e 3029 203b 2028  db (>=0.6.0) ; (
+00000310: 7079 7468 6f6e 5f76 6572 7369 6f6e 203e  python_version >
+00000320: 3d20 2233 2e38 2220 616e 6420 7079 7468  = "3.8" and pyth
+00000330: 6f6e 5f76 6572 7369 6f6e 203c 2022 342e  on_version < "4.
+00000340: 3022 2920 616e 6420 2865 7874 7261 203d  0") and (extra =
+00000350: 3d20 2264 7563 6b64 6222 290a 5265 7175  = "duckdb").Requ
+00000360: 6972 6573 2d44 6973 743a 2070 616e 6461  ires-Dist: panda
+00000370: 7320 3b20 2870 7974 686f 6e5f 7665 7273  s ; (python_vers
+00000380: 696f 6e20 3e3d 2022 332e 3822 2061 6e64  ion >= "3.8" and
+00000390: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
+000003a0: 3c20 2234 2e30 2229 2061 6e64 2028 6578  < "4.0") and (ex
+000003b0: 7472 6120 3d3d 2022 7061 6e64 6173 2229  tra == "pandas")
+000003c0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000003d0: 706f 6c61 7273 2028 3e3d 302e 3138 2e33  polars (>=0.18.3
+000003e0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+000003f0: 2070 7961 7272 6f77 2028 3e3d 352e 302e   pyarrow (>=5.0.
+00000400: 3029 203b 2028 7079 7468 6f6e 5f76 6572  0) ; (python_ver
+00000410: 7369 6f6e 203e 3d20 2233 2e38 2220 616e  sion >= "3.8" an
+00000420: 6420 7079 7468 6f6e 5f76 6572 7369 6f6e  d python_version
+00000430: 203c 2022 342e 3022 2920 616e 6420 2865   < "4.0") and (e
+00000440: 7874 7261 203d 3d20 2263 6163 6869 6e67  xtra == "caching
+00000450: 2220 6f72 2065 7874 7261 203d 3d20 2264  " or extra == "d
+00000460: 7563 6b64 6222 290a 5265 7175 6972 6573  uckdb").Requires
+00000470: 2d44 6973 743a 2070 7964 616e 7469 6320  -Dist: pydantic 
+00000480: 283e 3d31 2e37 2e30 290a 5265 7175 6972  (>=1.7.0).Requir
+00000490: 6573 2d44 6973 743a 2073 7068 696e 782d  es-Dist: sphinx-
+000004a0: 6175 746f 6275 696c 6420 3b20 6578 7472  autobuild ; extr
+000004b0: 6120 3d3d 2022 646f 6373 220a 5265 7175  a == "docs".Requ
+000004c0: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
+000004d0: 782d 6175 746f 646f 632d 7479 7065 6869  x-autodoc-typehi
+000004e0: 6e74 7320 3b20 6578 7472 6120 3d3d 2022  nts ; extra == "
+000004f0: 646f 6373 220a 5265 7175 6972 6573 2d44  docs".Requires-D
+00000500: 6973 743a 2073 7068 696e 782d 7274 642d  ist: sphinx-rtd-
+00000510: 7468 656d 6520 3b20 6578 7472 6120 3d3d  theme ; extra ==
+00000520: 2022 646f 6373 220a 5265 7175 6972 6573   "docs".Requires
+00000530: 2d44 6973 743a 2073 7068 696e 782d 746f  -Dist: sphinx-to
+00000540: 6f6c 626f 7820 3b20 6578 7472 6120 3d3d  olbox ; extra ==
+00000550: 2022 646f 6373 220a 5265 7175 6972 6573   "docs".Requires
+00000560: 2d44 6973 743a 2073 7068 696e 7863 6f6e  -Dist: sphinxcon
+00000570: 7472 6962 2d6d 6572 6d61 6964 203b 2065  trib-mermaid ; e
+00000580: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
+00000590: 6571 7569 7265 732d 4469 7374 3a20 7479  equires-Dist: ty
+000005a0: 7069 6e67 2d65 7874 656e 7369 6f6e 730a  ping-extensions.
+000005b0: 5072 6f6a 6563 742d 5552 4c3a 2044 6f63  Project-URL: Doc
+000005c0: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
+000005d0: 733a 2f2f 7061 7469 746f 2e72 6561 6474  s://patito.readt
+000005e0: 6865 646f 6373 2e69 6f0a 5072 6f6a 6563  hedocs.io.Projec
+000005f0: 742d 5552 4c3a 2052 6570 6f73 6974 6f72  t-URL: Repositor
+00000600: 792c 2068 7474 7073 3a2f 2f67 6974 6875  y, https://githu
+00000610: 622e 636f 6d2f 6b6f 6c6f 6e69 616c 6e6f  b.com/kolonialno
+00000620: 2f70 6174 6974 6f0a 4465 7363 7269 7074  /patito.Descript
+00000630: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+00000640: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+00000650: 0a23 203c 6365 6e74 6572 3e3c 696d 6720  .# <center><img 
+00000660: 6865 6967 6874 3d22 3330 7078 2220 7372  height="30px" sr
+00000670: 633d 2268 7474 7073 3a2f 2f65 6d6f 6a69  c="https://emoji
+00000680: 7065 6469 612d 7573 2e73 332e 6475 616c  pedia-us.s3.dual
+00000690: 7374 6163 6b2e 7573 2d77 6573 742d 312e  stack.us-west-1.
+000006a0: 616d 617a 6f6e 6177 732e 636f 6d2f 7468  amazonaws.com/th
+000006b0: 756d 6273 2f31 3230 2f73 616d 7375 6e67  umbs/120/samsung
+000006c0: 2f37 382f 6475 636b 5f31 6639 3836 2e70  /78/duck_1f986.p
+000006d0: 6e67 223e 2050 6174 6974 6f3c 6365 6e74  ng"> Patito<cent
+000006e0: 6572 3e0a 0a3c 7020 616c 6967 6e3d 2263  er>..<p align="c
+000006f0: 656e 7465 7222 3e0a 2020 2020 3c65 6d3e  enter">.    <em>
+00000700: 0a20 2020 2020 2020 2050 6174 6974 6f20  .        Patito 
+00000710: 636f 6d62 696e 6573 203c 6120 6872 6566  combines <a href
+00000720: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000730: 2e63 6f6d 2f73 616d 7565 6c63 6f6c 7669  .com/samuelcolvi
+00000740: 6e2f 7079 6461 6e74 6963 223e 7079 6461  n/pydantic">pyda
+00000750: 6e74 6963 3c2f 613e 2061 6e64 203c 6120  ntic</a> and <a 
+00000760: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000770: 7468 7562 2e63 6f6d 2f70 6f6c 612d 7273  thub.com/pola-rs
+00000780: 2f70 6f6c 6172 7322 3e70 6f6c 6172 733c  /polars">polars<
+00000790: 2f61 3e20 696e 206f 7264 6572 2074 6f20  /a> in order to 
+000007a0: 7772 6974 6520 6d6f 6465 726e 2c20 7479  write modern, ty
+000007b0: 7065 2d61 6e6e 6f74 6174 6564 2064 6174  pe-annotated dat
+000007c0: 6120 6672 616d 6520 6c6f 6769 632e 0a20  a frame logic.. 
+000007d0: 2020 203c 2f65 6d3e 0a20 2020 203c 6272     </em>.    <br
+000007e0: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+000007f0: 7474 7073 3a2f 2f70 6174 6974 6f2e 7265  ttps://patito.re
+00000800: 6164 7468 6564 6f63 732e 696f 2f22 3e0a  adthedocs.io/">.
+00000810: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000820: 3d22 6874 7470 733a 2f2f 7265 6164 7468  ="https://readth
+00000830: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
+00000840: 7473 2f70 6174 6974 6f2f 6261 6467 652f  ts/patito/badge/
+00000850: 2220 616c 743d 2244 6f63 7320 7374 6174  " alt="Docs stat
+00000860: 7573 223e 0a20 2020 203c 2f61 3e0a 2020  us">.    </a>.  
+00000870: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000880: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b6f  ://github.com/ko
+00000890: 6c6f 6e69 616c 6e6f 2f70 6174 6974 6f2f  lonialno/patito/
+000008a0: 6163 7469 6f6e 733f 776f 726b 666c 6f77  actions?workflow
+000008b0: 3d43 4922 3e0a 2020 2020 2020 2020 3c69  =CI">.        <i
+000008c0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000008d0: 6769 7468 7562 2e63 6f6d 2f6b 6f6c 6f6e  github.com/kolon
+000008e0: 6961 6c6e 6f2f 7061 7469 746f 2f61 6374  ialno/patito/act
+000008f0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f63  ions/workflows/c
+00000900: 692e 796d 6c2f 6261 6467 652e 7376 6722  i.yml/badge.svg"
+00000910: 2061 6c74 3d22 4349 2073 7461 7475 7322   alt="CI status"
+00000920: 3e0a 2020 2020 3c2f 613e 0a20 2020 203c  >.    </a>.    <
+00000930: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000940: 636f 6465 636f 762e 696f 2f67 682f 6b6f  codecov.io/gh/ko
+00000950: 6c6f 6e69 616c 6e6f 2f70 6174 6974 6f22  lonialno/patito"
+00000960: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
+00000970: 7263 3d22 6874 7470 733a 2f2f 636f 6465  rc="https://code
+00000980: 636f 762e 696f 2f67 682f 6b6f 6c6f 6e69  cov.io/gh/koloni
+00000990: 616c 6e6f 2f70 6174 6974 6f2f 6272 616e  alno/patito/bran
+000009a0: 6368 2f6d 6169 6e2f 6772 6170 682f 6261  ch/main/graph/ba
+000009b0: 6467 652e 7376 673f 746f 6b65 6e3d 3732  dge.svg?token=72
+000009c0: 304c 4244 5948 3235 222f 3e0a 2020 2020  0LBDYH25"/>.    
+000009d0: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+000009e0: 3d22 6874 7470 733a 2f2f 7079 7069 2e70  ="https://pypi.p
+000009f0: 7974 686f 6e2e 6f72 672f 7079 7069 2f70  ython.org/pypi/p
+00000a00: 6174 6974 6f22 3e0a 2020 2020 2020 2020  atito">.        
+00000a10: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000a20: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000a30: 2f70 7970 692f 762f 7061 7469 746f 2e73  /pypi/v/patito.s
+00000a40: 7667 223e 0a20 2020 203c 2f61 3e0a 2020  vg">.    </a>.  
+00000a50: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000a60: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000a70: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
+00000a80: 6e73 2f70 6174 6974 6f22 3e0a 2020 2020  ns/patito">.    
+00000a90: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000aa0: 2f67 6974 6875 622e 636f 6d2f 6b6f 6c6f  /github.com/kolo
+00000ab0: 6e69 616c 6e6f 2f70 6174 6974 6f2f 626c  nialno/patito/bl
+00000ac0: 6f62 2f6d 6173 7465 722f 4c49 4345 4e53  ob/master/LICENS
+00000ad0: 4522 3e0a 2020 2020 2020 2020 3c69 6d67  E">.        <img
+00000ae0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000af0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000b00: 6875 622f 6c69 6365 6e73 652f 6b6f 6c6f  hub/license/kolo
+00000b10: 6e69 616c 6e6f 2f70 6174 6974 6f2e 7376  nialno/patito.sv
+00000b20: 6722 3e0a 2020 2020 3c2f 613e 0a3c 2f70  g">.    </a>.</p
+00000b30: 3e0a 0a50 6174 6974 6f20 6f66 6665 7273  >..Patito offers
+00000b40: 2061 2073 696d 706c 6520 7761 7920 746f   a simple way to
+00000b50: 2064 6563 6c61 7265 2070 7964 616e 7469   declare pydanti
+00000b60: 6320 6461 7461 206d 6f64 656c 7320 7768  c data models wh
+00000b70: 6963 6820 646f 7562 6c65 2061 7320 7363  ich double as sc
+00000b80: 6865 6d61 2066 6f72 2079 6f75 7220 706f  hema for your po
+00000b90: 6c61 7273 2064 6174 6120 6672 616d 6573  lars data frames
+00000ba0: 2e0a 5468 6573 6520 7363 6865 6d61 2063  ..These schema c
+00000bb0: 616e 2062 6520 7573 6564 2066 6f72 3a0a  an be used for:.
+00000bc0: 0af0 9f91 ae20 5369 6d70 6c65 2061 6e64  ..... Simple and
+00000bd0: 2070 6572 666f 726d 616e 7420 6461 7461   performant data
+00000be0: 2066 7261 6d65 2076 616c 6964 6174 696f   frame validatio
+00000bf0: 6e2e 5c0a f09f a7aa 2045 6173 7920 6765  n.\..... Easy ge
+00000c00: 6e65 7261 7469 6f6e 206f 6620 7661 6c69  neration of vali
+00000c10: 6420 6d6f 636b 2064 6174 6120 6672 616d  d mock data fram
+00000c20: 6573 2066 6f72 2074 6573 7473 2e5c 0af0  es for tests.\..
+00000c30: 9f90 8d20 5265 7472 6965 7665 2061 6e64  ... Retrieve and
+00000c40: 2072 6570 7265 7365 6e74 2073 696e 6775   represent singu
+00000c50: 6c61 7220 726f 7773 2069 6e20 616e 206f  lar rows in an o
+00000c60: 626a 6563 742d 6f72 6965 6e74 6564 206d  bject-oriented m
+00000c70: 616e 6e65 722e 5c0a f09f a7a0 2050 726f  anner.\..... Pro
+00000c80: 7669 6465 2061 2073 696e 676c 6520 736f  vide a single so
+00000c90: 7572 6365 206f 6620 7472 7574 6820 666f  urce of truth fo
+00000ca0: 7220 7468 6520 636f 7265 2064 6174 6120  r the core data 
+00000cb0: 6d6f 6465 6c73 2069 6e20 796f 7572 2063  models in your c
+00000cc0: 6f64 6520 6261 7365 2e20 5c0a f09f a686  ode base. \.....
+00000cd0: 2049 6e74 6567 7261 7469 6f6e 2077 6974   Integration wit
+00000ce0: 6820 4475 636b 4442 2066 6f72 2072 756e  h DuckDB for run
+00000cf0: 6e69 6e67 2066 6c65 7869 626c 6520 5351  ning flexible SQ
+00000d00: 4c20 7175 6572 6965 732e 0a0a 5061 7469  L queries...Pati
+00000d10: 746f 2068 6173 2066 6972 7374 2d63 6c61  to has first-cla
+00000d20: 7373 2073 7570 706f 7274 2066 6f72 205b  ss support for [
+00000d30: 706f 6c61 7273 5d28 2268 7474 7073 3a2f  polars]("https:/
+00000d40: 2f67 6974 6875 622e 636f 6d2f 706f 6c61  /github.com/pola
+00000d50: 2d72 732f 706f 6c61 7273 2229 2c20 6120  -rs/polars"), a 
+00000d60: 5f22 626c 617a 696e 676c 7920 6661 7374  _"blazingly fast
+00000d70: 2044 6174 6146 7261 6d65 7320 6c69 6272   DataFrames libr
+00000d80: 6172 7920 7772 6974 7465 6e20 696e 2052  ary written in R
+00000d90: 7573 7422 5f2e 0a0a 2323 2049 6e73 7461  ust"_...## Insta
+00000da0: 6c6c 6174 696f 6e0a 0a60 6060 7368 0a70  llation..```sh.p
+00000db0: 6970 2069 6e73 7461 6c6c 2070 6174 6974  ip install patit
+00000dc0: 6f0a 6060 600a 0a23 2323 2320 4475 636b  o.```..#### Duck
+00000dd0: 4442 2049 6e74 6567 7261 7469 6f6e 0a0a  DB Integration..
+00000de0: 5061 7469 746f 2063 616e 2061 6c73 6f20  Patito can also 
+00000df0: 696e 7465 6772 6174 6520 7769 7468 205b  integrate with [
+00000e00: 4475 636b 4442 5d28 6874 7470 733a 2f2f  DuckDB](https://
+00000e10: 6475 636b 6462 2e6f 7267 2f29 2e0a 496e  duckdb.org/)..In
+00000e20: 206f 7264 6572 2074 6f20 656e 6162 6c65   order to enable
+00000e30: 2074 6869 7320 696e 7465 6772 6174 696f   this integratio
+00000e40: 6e20 796f 7520 6d75 7374 2065 7870 6c69  n you must expli
+00000e50: 6369 746c 7920 7370 6563 6966 7920 6974  citly specify it
+00000e60: 2064 7572 696e 6720 696e 7374 616c 6c61   during installa
+00000e70: 7469 6f6e 3a0a 0a60 6060 7368 0a70 6970  tion:..```sh.pip
+00000e80: 2069 6e73 7461 6c6c 2027 7061 7469 746f   install 'patito
+00000e90: 5b64 7563 6b64 625d 270a 6060 600a 0a0a  [duckdb]'.```...
+00000ea0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
+00000eb0: 0a0a 5468 6520 6675 6c6c 2064 6f63 756d  ..The full docum
+00000ec0: 656e 7461 7469 6f6e 206f 6620 5061 7469  entation of Pati
+00000ed0: 6f20 6361 6e20 6265 2066 6f75 6e64 205b  o can be found [
+00000ee0: 6865 7265 5d28 6874 7470 733a 2f2f 7061  here](https://pa
+00000ef0: 7469 746f 2e72 6561 6474 6865 646f 6373  tito.readthedocs
+00000f00: 2e69 6f29 2e0a 0a23 2320 f09f 91ae 2044  .io)...## .... D
+00000f10: 6174 6120 7661 6c69 6461 7469 6f6e 0a0a  ata validation..
+00000f20: 5061 7469 746f 2061 6c6c 6f77 7320 796f  Patito allows yo
+00000f30: 7520 746f 2073 7065 6369 6679 2074 6865  u to specify the
+00000f40: 2074 7970 6520 6f66 2065 6163 6820 636f   type of each co
+00000f50: 6c75 6d6e 2069 6e20 796f 7572 2064 6174  lumn in your dat
+00000f60: 6166 7261 6d65 2062 7920 6372 6561 7469  aframe by creati
+00000f70: 6e67 2061 2074 7970 652d 616e 6e6f 7461  ng a type-annota
+00000f80: 7465 6420 7375 6263 6c61 7373 206f 6620  ted subclass of 
+00000f90: 6070 6174 6974 6f2e 4d6f 6465 6c60 3a0a  `patito.Model`:.
+00000fa0: 0a60 6060 7079 0a23 206d 6f64 656c 732e  .```py.# models.
+00000fb0: 7079 0a66 726f 6d20 7479 7069 6e67 2069  py.from typing i
+00000fc0: 6d70 6f72 7420 4c69 7465 7261 6c2c 204f  mport Literal, O
+00000fd0: 7074 696f 6e61 6c0a 0a69 6d70 6f72 7420  ptional..import 
+00000fe0: 7061 7469 746f 2061 7320 7074 0a0a 0a63  patito as pt...c
+00000ff0: 6c61 7373 2050 726f 6475 6374 2870 742e  lass Product(pt.
+00001000: 4d6f 6465 6c29 3a0a 2020 2020 7072 6f64  Model):.    prod
+00001010: 7563 745f 6964 3a20 696e 7420 3d20 7074  uct_id: int = pt
+00001020: 2e46 6965 6c64 2875 6e69 7175 653d 5472  .Field(unique=Tr
+00001030: 7565 290a 2020 2020 7465 6d70 6572 6174  ue).    temperat
+00001040: 7572 655f 7a6f 6e65 3a20 4c69 7465 7261  ure_zone: Litera
+00001050: 6c5b 2264 7279 222c 2022 636f 6c64 222c  l["dry", "cold",
+00001060: 2022 6672 6f7a 656e 225d 0a20 2020 2069   "frozen"].    i
+00001070: 735f 666f 725f 7361 6c65 3a20 626f 6f6c  s_for_sale: bool
+00001080: 0a60 6060 0a0a 5468 6520 2a2a 636c 6173  .```..The **clas
+00001090: 732a 2a20 6050 726f 6475 6374 6020 7265  s** `Product` re
+000010a0: 7072 6573 656e 7473 2074 6865 202a 2a73  presents the **s
+000010b0: 6368 656d 612a 2a20 6f66 2074 6865 2064  chema** of the d
+000010c0: 6174 6120 6672 616d 652c 2077 6869 6c65  ata frame, while
+000010d0: 202a 2a69 6e73 7461 6e63 6573 2a2a 206f   **instances** o
+000010e0: 6620 6050 726f 6475 6374 6020 7265 7072  f `Product` repr
+000010f0: 6573 656e 7420 7369 6e67 6c65 202a 2a72  esent single **r
+00001100: 6f77 732a 2a20 6f66 2074 6865 2064 6174  ows** of the dat
+00001110: 6166 7261 6d65 2e0a 5061 7469 746f 2063  aframe..Patito c
+00001120: 616e 2065 6666 6963 6965 6e74 6c79 2076  an efficiently v
+00001130: 616c 6964 6174 6520 7468 6520 636f 6e74  alidate the cont
+00001140: 656e 7420 6f66 2061 7262 6974 7261 7279  ent of arbitrary
+00001150: 2064 6174 6120 6672 616d 6573 2061 6e64   data frames and
+00001160: 2070 726f 7669 6465 2068 756d 616e 2d72   provide human-r
+00001170: 6561 6461 626c 6520 6572 726f 7220 6d65  eadable error me
+00001180: 7373 6167 6573 3a0a 0a60 6060 7079 0a69  ssages:..```py.i
+00001190: 6d70 6f72 7420 706f 6c61 7273 2061 7320  mport polars as 
+000011a0: 706c 0a0a 6466 203d 2070 6c2e 4461 7461  pl..df = pl.Data
+000011b0: 4672 616d 6528 0a20 2020 207b 0a20 2020  Frame(.    {.   
+000011c0: 2020 2020 2022 7072 6f64 7563 745f 6964       "product_id
+000011d0: 223a 205b 312c 2031 2c20 335d 2c0a 2020  ": [1, 1, 3],.  
+000011e0: 2020 2020 2020 2274 656d 7065 7261 7475        "temperatu
+000011f0: 7265 5f7a 6f6e 6522 3a20 5b22 6472 7922  re_zone": ["dry"
+00001200: 2c20 2264 7279 222c 2022 6f76 656e 225d  , "dry", "oven"]
+00001210: 2c0a 2020 2020 7d0a 290a 7472 793a 0a20  ,.    }.).try:. 
+00001220: 2020 2050 726f 6475 6374 2e76 616c 6964     Product.valid
+00001230: 6174 6528 6466 290a 6578 6365 7074 2070  ate(df).except p
+00001240: 742e 5661 6c69 6461 7469 6f6e 4572 726f  t.ValidationErro
+00001250: 7220 6173 2065 7863 3a0a 2020 2020 7072  r as exc:.    pr
+00001260: 696e 7428 6578 6329 0a23 2033 2076 616c  int(exc).# 3 val
+00001270: 6964 6174 696f 6e20 6572 726f 7273 2066  idation errors f
+00001280: 6f72 2050 726f 6475 6374 0a23 2069 735f  or Product.# is_
+00001290: 666f 725f 7361 6c65 0a23 2020 204d 6973  for_sale.#   Mis
+000012a0: 7369 6e67 2063 6f6c 756d 6e20 2874 7970  sing column (typ
+000012b0: 653d 7479 7065 5f65 7272 6f72 2e6d 6973  e=type_error.mis
+000012c0: 7369 6e67 636f 6c75 6d6e 7329 0a23 2070  singcolumns).# p
+000012d0: 726f 6475 6374 5f69 640a 2320 2020 3220  roduct_id.#   2 
+000012e0: 726f 7773 2077 6974 6820 6475 706c 6963  rows with duplic
+000012f0: 6174 6564 2076 616c 7565 732e 2028 7479  ated values. (ty
+00001300: 7065 3d76 616c 7565 5f65 7272 6f72 2e72  pe=value_error.r
+00001310: 6f77 7661 6c75 6529 0a23 2074 656d 7065  owvalue).# tempe
+00001320: 7261 7475 7265 5f7a 6f6e 650a 2320 2020  rature_zone.#   
+00001330: 526f 7773 2077 6974 6820 696e 7661 6c69  Rows with invali
+00001340: 6420 7661 6c75 6573 3a20 7b27 6f76 656e  d values: {'oven
+00001350: 277d 2e20 2874 7970 653d 7661 6c75 655f  '}. (type=value_
+00001360: 6572 726f 722e 726f 7776 616c 7565 290a  error.rowvalue).
+00001370: 6060 600a 0a3c 6465 7461 696c 733e 0a3c  ```..<details>.<
+00001380: 7375 6d6d 6172 793e 3c62 3e43 6c69 636b  summary><b>Click
+00001390: 2074 6f20 7365 6520 6120 7375 6d6d 6172   to see a summar
+000013a0: 7920 6f66 2064 6174 6166 7261 6d65 2d63  y of dataframe-c
+000013b0: 6f6d 7061 7469 626c 6520 7479 7065 2061  ompatible type a
+000013c0: 6e6e 6f74 6174 696f 6e73 2e3c 2f62 3e3c  nnotations.</b><
+000013d0: 2f73 756d 6d61 7279 3e0a 0a2a 2052 6567  /summary>..* Reg
+000013e0: 756c 6172 2070 7974 686f 6e20 6461 7461  ular python data
+000013f0: 2074 7970 6573 2073 7563 6820 6173 2060   types such as `
+00001400: 696e 7460 2c20 6066 6c6f 6174 602c 2060  int`, `float`, `
+00001410: 626f 6f6c 602c 2060 7374 7260 2c20 6064  bool`, `str`, `d
+00001420: 6174 6560 2c20 7768 6963 6820 6172 6520  ate`, which are 
+00001430: 7661 6c69 6461 7465 6420 6167 6169 6e73  validated agains
+00001440: 7420 636f 6d70 6174 6962 6c65 2070 6f6c  t compatible pol
+00001450: 6172 7320 6461 7461 2074 7970 6573 2e0a  ars data types..
+00001460: 2a20 5772 6170 7069 6e67 2079 6f75 7220  * Wrapping your 
+00001470: 7479 7065 2077 6974 6820 6074 7970 696e  type with `typin
+00001480: 672e 4f70 7469 6f6e 616c 6020 696e 6469  g.Optional` indi
+00001490: 6361 7465 7320 7468 6174 2074 6865 2067  cates that the g
+000014a0: 6976 656e 2063 6f6c 756d 6e20 6163 6365  iven column acce
+000014b0: 7074 7320 6d69 7373 696e 6720 7661 6c75  pts missing valu
+000014c0: 6573 2e0a 2a20 4d6f 6465 6c20 6669 656c  es..* Model fiel
+000014d0: 6473 2061 6e6e 6f74 6174 6564 2077 6974  ds annotated wit
+000014e0: 6820 6074 7970 696e 672e 4c69 7465 7261  h `typing.Litera
+000014f0: 6c5b 2e2e 2e5d 6020 6368 6563 6b20 6966  l[...]` check if
+00001500: 206f 6e6c 7920 6120 7265 7374 7269 6374   only a restrict
+00001510: 6564 2073 6574 206f 6620 7661 6c75 6573  ed set of values
+00001520: 2061 7265 2074 616b 656e 2c20 6569 7468   are taken, eith
+00001530: 6572 2061 7320 7468 6520 6e61 7469 7665  er as the native
+00001540: 2064 7479 7065 2028 652e 672e 2060 706c   dtype (e.g. `pl
+00001550: 2e55 7466 3860 2920 6f72 2060 706c 2e43  .Utf8`) or `pl.C
+00001560: 6174 6567 6f72 6963 616c 602e 0a0a 4164  ategorical`...Ad
+00001570: 6469 746f 6e61 6c6c 792c 2079 6f75 2063  ditonally, you c
+00001580: 616e 2061 7373 6967 6e20 6070 6174 6974  an assign `patit
+00001590: 6f2e 4669 656c 6460 2074 6f20 796f 7572  o.Field` to your
+000015a0: 2063 6c61 7373 2076 6172 6961 626c 6573   class variables
+000015b0: 2069 6e20 6f72 6465 7220 746f 2073 7065   in order to spe
+000015c0: 6369 6679 2061 6464 6974 696f 6e61 6c20  cify additional 
+000015d0: 6368 6563 6b73 3a0a 0a2a 2060 4669 656c  checks:..* `Fiel
+000015e0: 6428 6474 7970 653d 2e2e 2e29 6020 656e  d(dtype=...)` en
+000015f0: 7375 7265 7320 7468 6174 2061 2073 7065  sures that a spe
+00001600: 6369 6669 6320 6474 7970 6520 6973 2075  cific dtype is u
+00001610: 7365 6420 696e 2074 686f 7365 2063 6173  sed in those cas
+00001620: 6573 2077 6865 7265 2073 6576 6572 616c  es where several
+00001630: 2064 6174 6120 7479 7065 7320 6172 6520   data types are 
+00001640: 636f 6d70 6c69 616e 7420 7769 7468 2074  compliant with t
+00001650: 6865 2061 6e6e 6f74 6174 6564 2070 7974  he annotated pyt
+00001660: 686f 6e20 7479 7065 2c20 666f 7220 6578  hon type, for ex
+00001670: 616d 706c 6520 6070 726f 6475 6374 5f69  ample `product_i
+00001680: 643a 2069 6e74 203d 2046 6965 6c64 2864  d: int = Field(d
+00001690: 7479 7065 3d70 6c2e 5549 6e74 3332 2960  type=pl.UInt32)`
+000016a0: 2e0a 2a20 6046 6965 6c64 2875 6e69 7175  ..* `Field(uniqu
+000016b0: 653d 5472 7565 2960 2063 6865 636b 7320  e=True)` checks 
+000016c0: 6966 2065 7665 7279 2072 6f77 2068 6173  if every row has
+000016d0: 2061 2075 6e69 7175 6520 7661 6c75 652e   a unique value.
+000016e0: 0a2a 2060 4669 656c 6428 6774 3d2e 2e2e  .* `Field(gt=...
+000016f0: 2c20 6765 3d2e 2e2e 2c20 6c65 3d2e 2e2e  , ge=..., le=...
+00001700: 2c20 6c74 3d2e 2e2e 2960 2061 6c6c 6f77  , lt=...)` allow
+00001710: 7320 796f 7520 746f 2073 7065 6369 6679  s you to specify
+00001720: 2062 6f75 6e64 2063 6865 636b 7320 666f   bound checks fo
+00001730: 7220 616e 7920 636f 6d62 696e 6174 696f  r any combinatio
+00001740: 6e20 6f66 2060 3e20 6774 602c 2060 3e3d  n of `> gt`, `>=
+00001750: 2067 6560 2c20 603c 3d20 6c65 6020 603c   ge`, `<= le` `<
+00001760: 206c 7460 2c20 7265 7370 6563 7469 7665   lt`, respective
+00001770: 6c79 2e0a 2a20 6046 6965 6c64 286d 756c  ly..* `Field(mul
+00001780: 7469 706c 655f 6f66 3d64 6976 6973 6f72  tiple_of=divisor
+00001790: 2960 2069 6e20 6f72 6465 7220 746f 2063  )` in order to c
+000017a0: 6865 636b 2069 6620 6120 6769 7665 6e20  heck if a given 
+000017b0: 636f 6c75 6d6e 206f 6e6c 7920 636f 6e74  column only cont
+000017c0: 6169 6e73 2076 616c 7565 7320 6173 206d  ains values as m
+000017d0: 756c 7469 706c 6573 206f 6620 7468 6520  ultiples of the 
+000017e0: 6769 7665 6e20 7661 6c75 652e 0a2a 2060  given value..* `
+000017f0: 4669 656c 6428 6465 6661 756c 743d 6465  Field(default=de
+00001800: 6661 756c 745f 7661 6c75 652c 2063 6f6e  fault_value, con
+00001810: 7374 3d54 7275 6529 6020 696e 6469 6361  st=True)` indica
+00001820: 7465 7320 7468 6174 2074 6865 2067 6976  tes that the giv
+00001830: 656e 2063 6f6c 756d 6e20 6973 2072 6571  en column is req
+00001840: 7569 7265 6420 616e 6420 5f6d 7573 745f  uired and _must_
+00001850: 2074 616b 6520 7468 6520 6769 7665 6e20   take the given 
+00001860: 6465 6661 756c 7420 7661 6c75 652e 0a2a  default value..*
+00001870: 2053 7472 696e 6720 6669 656c 6473 2061   String fields a
+00001880: 6e6e 6f74 6174 6564 2077 6974 6820 6046  nnotated with `F
+00001890: 6965 6c64 2872 6567 6578 3d72 223c 7265  ield(regex=r"<re
+000018a0: 6765 782d 7061 7474 6572 6e3e 2229 602c  gex-pattern>")`,
+000018b0: 2060 4669 656c 6428 6d61 785f 6c65 6e67   `Field(max_leng
+000018c0: 7468 3d62 6f75 6e64 2960 2c20 616e 642f  th=bound)`, and/
+000018d0: 6f72 2060 4669 656c 6428 6d69 6e5f 6c65  or `Field(min_le
+000018e0: 6e67 7468 2960 2077 696c 6c20 6265 2076  ngth)` will be v
+000018f0: 616c 6964 6174 6564 2077 6974 6820 5b70  alidated with [p
+00001900: 6f6c 6172 7327 2065 6666 6963 6965 6e74  olars' efficient
+00001910: 2073 7472 696e 6720 7072 6f63 6573 7369   string processi
+00001920: 6e67 2063 6170 6162 696c 6974 6965 735d  ng capabilities]
+00001930: 2868 7474 7073 3a2f 2f70 6f6c 612d 7273  (https://pola-rs
+00001940: 2e67 6974 6875 622e 696f 2f70 6f6c 6172  .github.io/polar
+00001950: 732d 626f 6f6b 2f75 7365 722d 6775 6964  s-book/user-guid
+00001960: 652f 686f 7763 616e 692f 6461 7461 2f73  e/howcani/data/s
+00001970: 7472 696e 6773 2e68 746d 6c29 2e0a 2a20  trings.html)..* 
+00001980: 4375 7374 6f6d 2063 6f6e 7374 7261 696e  Custom constrain
+00001990: 7473 2063 616e 2062 6520 7370 6563 6966  ts can be specif
+000019a0: 6965 6420 7769 7468 2077 6974 6820 6046  ied with with `F
+000019b0: 6965 6c64 2863 6f6e 7374 7261 696e 7473  ield(constraints
+000019c0: 3d2e 2e2e 2960 2c20 6569 7468 6572 2061  =...)`, either a
+000019d0: 7320 6120 7369 6e67 6c65 2070 6f6c 6172  s a single polar
+000019e0: 7320 6578 7072 6573 7369 6f6e 206f 7220  s expression or 
+000019f0: 6120 6c69 7374 206f 6620 6578 7072 6573  a list of expres
+00001a00: 7369 6f6e 732e 2041 6c6c 2074 6865 2072  sions. All the r
+00001a10: 6f77 7320 6f66 2074 6865 2064 6174 6166  ows of the dataf
+00001a20: 7261 6d65 206d 7573 7420 7361 7469 7366  rame must satisf
+00001a30: 7920 7468 6520 6769 7665 6e20 636f 6e73  y the given cons
+00001a40: 7472 6169 6e74 2873 2920 696e 206f 7264  traint(s) in ord
+00001a50: 6572 2074 6f20 6265 2063 6f6e 7369 6465  er to be conside
+00001a60: 7265 6420 7661 6c69 642e 2045 7861 6d70  red valid. Examp
+00001a70: 6c65 3a20 6065 7665 6e5f 6669 656c 643a  le: `even_field:
+00001a80: 2069 6e74 203d 2070 742e 4669 656c 6428   int = pt.Field(
+00001a90: 636f 6e73 7472 6169 6e74 733d 706c 2e63  constraints=pl.c
+00001aa0: 6f6c 2822 6576 656e 5f66 6965 6c64 2229  ol("even_field")
+00001ab0: 2025 2032 203d 3d20 3029 602e 0a0a 416c   % 2 == 0)`...Al
+00001ac0: 7468 6f75 6768 2050 6174 6974 6f20 7375  though Patito su
+00001ad0: 7070 6f72 7473 205b 7061 6e64 6173 5d28  pports [pandas](
+00001ae0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001af0: 6f6d 2f70 616e 6461 732d 6465 762f 7061  om/pandas-dev/pa
+00001b00: 6e64 6173 292c 2069 7420 6973 2068 6967  ndas), it is hig
+00001b10: 686c 7920 7265 636f 6d6d 656d 656e 6465  hly recommemende
+00001b20: 6420 746f 2062 6520 7573 6564 2069 6e20  d to be used in 
+00001b30: 636f 6d62 696e 6174 696f 6e20 7769 7468  combination with
+00001b40: 205b 706f 6c61 7273 5d28 2268 7474 7073   [polars]("https
+00001b50: 3a2f 2f67 6974 6875 622e 636f 6d2f 706f  ://github.com/po
+00001b60: 6c61 2d72 732f 706f 6c61 7273 2229 2e0a  la-rs/polars")..
+00001b70: 466f 7220 6120 6d75 6368 206d 6f72 6520  For a much more 
+00001b80: 6665 6174 7572 652d 636f 6d70 6c65 7465  feature-complete
+00001b90: 2c20 7061 6e64 6173 2d66 6972 7374 206c  , pandas-first l
+00001ba0: 6962 7261 7279 2c20 7461 6b65 2061 206c  ibrary, take a l
+00001bb0: 6f6f 6b20 6174 205b 7061 6e64 6572 615d  ook at [pandera]
+00001bc0: 2868 7474 7073 3a2f 2f70 616e 6465 7261  (https://pandera
+00001bd0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00001be0: 292e 0a3c 2f64 6574 6169 6c73 3e0a 0a23  )..</details>..#
+00001bf0: 2320 f09f a7aa 2053 796e 7468 6573 697a  # .... Synthesiz
+00001c00: 6520 7661 6c69 6420 7465 7374 2064 6174  e valid test dat
+00001c10: 610a 0a50 6174 6974 6f20 656e 636f 7572  a..Patito encour
+00001c20: 6167 6573 2079 6f75 2074 6f20 7374 7269  ages you to stri
+00001c30: 6374 6c79 2076 616c 6964 6174 6520 6461  ctly validate da
+00001c40: 7461 6672 616d 6520 696e 7075 7473 2c20  taframe inputs, 
+00001c50: 7468 7573 2065 6e73 7572 696e 6720 636f  thus ensuring co
+00001c60: 7272 6563 746e 6573 7320 6174 2072 756e  rrectness at run
+00001c70: 7469 6d65 2e0a 4275 7420 7769 7468 2066  time..But with f
+00001c80: 6f72 6365 6420 636f 7272 6563 746e 6573  orced correctnes
+00001c90: 7320 636f 6d65 7320 6672 6963 7469 6f6e  s comes friction
+00001ca0: 2c20 6573 7065 6369 616c 6c79 2064 7572  , especially dur
+00001cb0: 696e 6720 7465 7374 696e 672e 0a54 616b  ing testing..Tak
+00001cc0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00001cd0: 6675 6e63 7469 6f6e 2061 7320 616e 2065  function as an e
+00001ce0: 7861 6d70 6c65 3a0a 0a60 6060 7079 0a69  xample:..```py.i
+00001cf0: 6d70 6f72 7420 706f 6c61 7273 2061 7320  mport polars as 
+00001d00: 706c 0a0a 6465 6620 6e75 6d5f 7072 6f64  pl..def num_prod
+00001d10: 7563 7473 5f66 6f72 5f73 616c 6528 7072  ucts_for_sale(pr
+00001d20: 6f64 7563 7473 3a20 706c 2e44 6174 6146  oducts: pl.DataF
+00001d30: 7261 6d65 2920 2d3e 2069 6e74 3a0a 2020  rame) -> int:.  
+00001d40: 2020 5072 6f64 7563 742e 7661 6c69 6461    Product.valida
+00001d50: 7465 2870 726f 6475 6374 7329 0a20 2020  te(products).   
+00001d60: 2072 6574 7572 6e20 7072 6f64 7563 7473   return products
+00001d70: 2e66 696c 7465 7228 706c 2e63 6f6c 2822  .filter(pl.col("
+00001d80: 6973 5f66 6f72 5f73 616c 6522 2929 2e68  is_for_sale")).h
+00001d90: 6569 6768 740a 6060 600a 0a54 6865 2066  eight.```..The f
+00001da0: 6f6c 6c6f 7769 6e67 2074 6573 7420 776f  ollowing test wo
+00001db0: 756c 6420 6661 696c 2077 6974 6820 6120  uld fail with a 
+00001dc0: 6070 6174 6974 6f2e 5661 6c69 6461 7469  `patito.Validati
+00001dd0: 6f6e 4572 726f 7260 3a0a 0a60 6060 7079  onError`:..```py
+00001de0: 0a64 6566 2074 6573 745f 6e75 6d5f 7072  .def test_num_pr
+00001df0: 6f64 7563 7473 5f66 6f72 5f73 616c 6528  oducts_for_sale(
+00001e00: 293a 0a20 2020 2070 726f 6475 6374 7320  ):.    products 
+00001e10: 3d20 706c 2e44 6174 6146 7261 6d65 287b  = pl.DataFrame({
+00001e20: 2269 735f 666f 725f 7361 6c65 223a 205b  "is_for_sale": [
+00001e30: 5472 7565 2c20 5472 7565 2c20 4661 6c73  True, True, Fals
+00001e40: 655d 7d29 0a20 2020 2061 7373 6572 7420  e]}).    assert 
+00001e50: 6e75 6d5f 7072 6f64 7563 7473 5f66 6f72  num_products_for
+00001e60: 5f73 616c 6528 7072 6f64 7563 7473 2920  _sale(products) 
+00001e70: 3d3d 2032 0a60 6060 0a0a 496e 206f 7264  == 2.```..In ord
+00001e80: 6572 2074 6f20 6d61 6b65 2074 6865 2074  er to make the t
+00001e90: 6573 7420 7061 7373 2077 6520 776f 756c  est pass we woul
+00001ea0: 6420 6861 7665 2074 6f20 6164 6420 7661  d have to add va
+00001eb0: 6c69 6420 6475 6d6d 7920 6461 7461 2066  lid dummy data f
+00001ec0: 6f72 2074 6865 2060 7465 6d70 6572 6174  or the `temperat
+00001ed0: 7572 655f 7a6f 6e65 6020 616e 6420 6070  ure_zone` and `p
+00001ee0: 726f 6475 6374 5f69 6460 2063 6f6c 756d  roduct_id` colum
+00001ef0: 6e73 2e0a 5468 6973 2077 696c 6c20 7175  ns..This will qu
+00001f00: 6963 6b6c 7920 696e 7472 6f64 7563 6520  ickly introduce 
+00001f10: 6120 6c6f 7420 6f66 2062 6f69 6c65 7270  a lot of boilerp
+00001f20: 6c61 7465 2074 6f20 616c 6c20 7465 7374  late to all test
+00001f30: 7320 696e 766f 6c76 696e 6720 6461 7461  s involving data
+00001f40: 2066 7261 6d65 732c 206f 6273 6375 7269   frames, obscuri
+00001f50: 6e67 2077 6861 7420 6973 2061 6374 7561  ng what is actua
+00001f60: 6c6c 7920 6265 696e 6720 7465 7374 6564  lly being tested
+00001f70: 2069 6e20 6561 6368 2074 6573 742e 0a46   in each test..F
+00001f80: 6f72 2074 6869 7320 7265 6173 6f6e 2050  or this reason P
+00001f90: 6174 6974 6f20 7072 6f76 6964 6573 2074  atito provides t
+00001fa0: 6865 2060 6578 616d 706c 6573 6020 636f  he `examples` co
+00001fb0: 6e73 7472 7563 746f 7220 666f 7220 6765  nstructor for ge
+00001fc0: 6e65 7261 7469 6e67 2074 6573 7420 6461  nerating test da
+00001fd0: 7461 2074 6861 7420 6973 2066 756c 6c79  ta that is fully
+00001fe0: 2063 6f6d 706c 6961 6e74 2077 6974 6820   compliant with 
+00001ff0: 7468 6520 6769 7665 6e20 6d6f 6465 6c20  the given model 
+00002000: 7363 6865 6d61 2e0a 0a60 6060 7079 0a50  schema...```py.P
+00002010: 726f 6475 6374 2e65 7861 6d70 6c65 7328  roduct.examples(
+00002020: 7b22 6973 5f66 6f72 5f73 616c 6522 3a20  {"is_for_sale": 
+00002030: 5b54 7275 652c 2054 7275 652c 2046 616c  [True, True, Fal
+00002040: 7365 5d7d 290a 2320 7368 6170 653a 2028  se]}).# shape: (
+00002050: 332c 2033 290a 2320 e294 8ce2 9480 e294  3, 3).# ........
+00002060: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002070: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002080: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
+00002090: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000020a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000020b0: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
+000020c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000020d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000020e0: 9480 e294 900a 2320 e294 8220 6973 5f66  ......# ... is_f
+000020f0: 6f72 5f73 616c 6520 e294 8620 7465 6d70  or_sale ... temp
+00002100: 6572 6174 7572 655f 7a6f 6e65 20e2 9486  erature_zone ...
+00002110: 2070 726f 6475 6374 5f69 6420 e294 820a   product_id ....
+00002120: 2320 e294 8220 2d2d 2d20 2020 2020 2020  # ... ---       
+00002130: 2020 e294 8620 2d2d 2d20 2020 2020 2020    ... ---       
+00002140: 2020 2020 2020 20e2 9486 202d 2d2d 2020         ... ---  
+00002150: 2020 2020 2020 e294 820a 2320 e294 8220        ....# ... 
+00002160: 626f 6f6c 2020 2020 2020 2020 e294 8620  bool        ... 
+00002170: 7374 7220 2020 2020 2020 2020 2020 2020  str             
+00002180: 20e2 9486 2069 3634 2020 2020 2020 2020   ... i64        
+00002190: e294 820a 2320 e295 9ee2 9590 e295 90e2  ....# ..........
+000021a0: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
+000021b0: 90e2 9590 e295 90e2 9590 e295 90e2 9590  ................
+000021c0: e295 aae2 9590 e295 90e2 9590 e295 90e2  ................
+000021d0: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
+000021e0: 90e2 9590 e295 90e2 9590 e295 90e2 9590  ................
+000021f0: e295 90e2 9590 e295 90e2 95aa e295 90e2  ................
+00002200: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
+00002210: 90e2 9590 e295 90e2 9590 e295 90e2 9590  ................
+00002220: e295 a10a 2320 e294 8220 7472 7565 2020  ....# ... true  
+00002230: 2020 2020 2020 e294 8620 6472 7920 2020        ... dry   
+00002240: 2020 2020 2020 2020 2020 20e2 9486 2030             ... 0
+00002250: 2020 2020 2020 2020 2020 e294 820a 2320            ....# 
+00002260: e294 9ce2 958c e295 8ce2 958c e295 8ce2  ................
+00002270: 958c e295 8ce2 958c e295 8ce2 958c e295  ................
+00002280: 8ce2 958c e295 8ce2 958c e294 bce2 958c  ................
+00002290: e295 8ce2 958c e295 8ce2 958c e295 8ce2  ................
+000022a0: 958c e295 8ce2 958c e295 8ce2 958c e295  ................
+000022b0: 8ce2 958c e295 8ce2 958c e295 8ce2 958c  ................
+000022c0: e295 8ce2 94bc e295 8ce2 958c e295 8ce2  ................
+000022d0: 958c e295 8ce2 958c e295 8ce2 958c e295  ................
+000022e0: 8ce2 958c e295 8ce2 958c e294 a40a 2320  ..............# 
+000022f0: e294 8220 7472 7565 2020 2020 2020 2020  ... true        
+00002300: e294 8620 6472 7920 2020 2020 2020 2020  ... dry         
+00002310: 2020 2020 20e2 9486 2031 2020 2020 2020       ... 1      
+00002320: 2020 2020 e294 820a 2320 e294 9ce2 958c      ....# ......
+00002330: e295 8ce2 958c e295 8ce2 958c e295 8ce2  ................
+00002340: 958c e295 8ce2 958c e295 8ce2 958c e295  ................
+00002350: 8ce2 958c e294 bce2 958c e295 8ce2 958c  ................
+00002360: e295 8ce2 958c e295 8ce2 958c e295 8ce2  ................
+00002370: 958c e295 8ce2 958c e295 8ce2 958c e295  ................
+00002380: 8ce2 958c e295 8ce2 958c e295 8ce2 94bc  ................
+00002390: e295 8ce2 958c e295 8ce2 958c e295 8ce2  ................
+000023a0: 958c e295 8ce2 958c e295 8ce2 958c e295  ................
+000023b0: 8ce2 958c e294 a40a 2320 e294 8220 6661  ........# ... fa
+000023c0: 6c73 6520 2020 2020 2020 e294 8620 6472  lse       ... dr
+000023d0: 7920 2020 2020 2020 2020 2020 2020 20e2  y              .
+000023e0: 9486 2032 2020 2020 2020 2020 2020 e294  .. 2          ..
+000023f0: 820a 2320 e294 94e2 9480 e294 80e2 9480  ..# ............
+00002400: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002410: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002420: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002430: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002440: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002450: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+00002460: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002470: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002480: 980a 6060 600a 0a54 6865 2060 6578 616d  ..```..The `exam
+00002490: 706c 6573 2829 6020 6d65 7468 6f64 2061  ples()` method a
+000024a0: 6363 6570 7473 2074 6865 2073 616d 6520  ccepts the same 
+000024b0: 6172 6775 6d65 6e74 7320 6173 2061 2072  arguments as a r
+000024c0: 6567 756c 6172 2064 6174 6120 6672 616d  egular data fram
+000024d0: 6520 636f 6e73 7472 7563 746f 722c 2074  e constructor, t
+000024e0: 6865 206d 6169 6e20 6469 6666 6572 656e  he main differen
+000024f0: 6365 2062 6569 6e67 2074 6861 7420 6974  ce being that it
+00002500: 2066 696c 6c73 2069 6e20 7661 6c69 6420   fills in valid 
+00002510: 6475 6d6d 7920 6461 7461 2066 6f72 2061  dummy data for a
+00002520: 6e79 2075 6e73 7065 6369 6669 6564 2063  ny unspecified c
+00002530: 6f6c 756d 6e73 2e0a 5468 6520 7465 7374  olumns..The test
+00002540: 2063 616e 2074 6865 7265 666f 7265 2062   can therefore b
+00002550: 6520 7265 7772 6974 7465 6e20 6173 3a0a  e rewritten as:.
+00002560: 0a60 6060 7079 0a64 6566 2074 6573 745f  .```py.def test_
+00002570: 6e75 6d5f 7072 6f64 7563 7473 5f66 6f72  num_products_for
+00002580: 5f73 616c 6528 293a 0a20 2020 2070 726f  _sale():.    pro
+00002590: 6475 6374 7320 3d20 5072 6f64 7563 742e  ducts = Product.
+000025a0: 6578 616d 706c 6573 287b 2269 735f 666f  examples({"is_fo
+000025b0: 725f 7361 6c65 223a 205b 5472 7565 2c20  r_sale": [True, 
+000025c0: 5472 7565 2c20 4661 6c73 655d 7d29 0a20  True, False]}). 
+000025d0: 2020 2061 7373 6572 7420 6e75 6d5f 7072     assert num_pr
+000025e0: 6f64 7563 7473 5f66 6f72 5f73 616c 6528  oducts_for_sale(
+000025f0: 7072 6f64 7563 7473 2920 3d3d 2032 0a60  products) == 2.`
+00002600: 6060 0a0a 2323 20f0 9f96 bcef b88f 2041  ``..## ....... A
+00002610: 206d 6f64 656c 2d61 7761 7265 2064 6174   model-aware dat
+00002620: 6120 6672 616d 6520 636c 6173 730a 5061  a frame class.Pa
+00002630: 7469 746f 206f 6666 6572 7320 6070 6174  tito offers `pat
+00002640: 6974 6f2e 4461 7461 4672 616d 6560 2c20  ito.DataFrame`, 
+00002650: 6120 636c 6173 7320 7468 6174 2065 7874  a class that ext
+00002660: 656e 6473 2060 706f 6c61 7273 2e44 6174  ends `polars.Dat
+00002670: 6146 7261 6d65 6020 696e 206f 7264 6572  aFrame` in order
+00002680: 2074 6f20 7072 6f76 6964 6520 7574 696c   to provide util
+00002690: 6974 7920 6d65 7468 6f64 7320 7265 6c61  ity methods rela
+000026a0: 7465 6420 746f 2060 7061 7469 746f 2e4d  ted to `patito.M
+000026b0: 6f64 656c 602e 0a54 6865 2073 6368 656d  odel`..The schem
+000026c0: 6120 6f66 2061 2064 6174 6120 6672 616d  a of a data fram
+000026d0: 6520 6361 6e20 6265 2073 7065 6369 6669  e can be specifi
+000026e0: 6564 2061 7420 7275 6e74 696d 6520 6279  ed at runtime by
+000026f0: 2069 6e76 6f6b 696e 6720 6070 6174 6974   invoking `patit
+00002700: 6f2e 4461 7461 4672 616d 652e 7365 745f  o.DataFrame.set_
+00002710: 6d6f 6465 6c28 6d6f 6465 6c29 602c 2061  model(model)`, a
+00002720: 6674 6572 2077 6869 6368 2061 2073 6574  fter which a set
+00002730: 206f 6620 636f 6e74 6578 7475 616c 697a   of contextualiz
+00002740: 6564 206d 6574 686f 6473 2062 6563 6f6d  ed methods becom
+00002750: 6520 6176 6169 6c61 626c 653a 0a0a 2a20  e available:..* 
+00002760: 6044 6174 6146 7261 6d65 2e76 616c 6964  `DataFrame.valid
+00002770: 6174 6528 2960 202d 2056 616c 6964 6174  ate()` - Validat
+00002780: 6520 7468 6520 6769 7665 6e20 6461 7461  e the given data
+00002790: 2066 7261 6d65 2061 6e64 2072 6574 7572   frame and retur
+000027a0: 6e20 6974 7365 6c66 2e0a 2a20 6044 6174  n itself..* `Dat
+000027b0: 6146 7261 6d65 2e64 726f 7028 2960 202d  aFrame.drop()` -
+000027c0: 2044 726f 7020 616c 6c20 7375 7065 7266   Drop all superf
+000027d0: 6c75 6f75 7320 636f 6c75 6d6e 7320 5f6e  luous columns _n
+000027e0: 6f74 5f20 7370 6563 6966 6965 6420 6173  ot_ specified as
+000027f0: 2066 6965 6c64 7320 696e 2074 6865 206d   fields in the m
+00002800: 6f64 656c 2e0a 2a20 6044 6174 6146 7261  odel..* `DataFra
+00002810: 6d65 2e63 6173 7428 2960 202d 2043 6173  me.cast()` - Cas
+00002820: 7420 616e 7920 636f 6c75 6d6e 7320 7768  t any columns wh
+00002830: 6963 6820 6172 6520 6e6f 7420 636f 6d70  ich are not comp
+00002840: 6174 6962 6c65 2077 6974 6820 7468 6520  atible with the 
+00002850: 6769 7665 6e20 7479 7065 2061 6e6e 6f74  given type annot
+00002860: 6174 696f 6e73 2e20 5768 656e 2060 4669  ations. When `Fi
+00002870: 656c 6428 6474 7970 653d 2e2e 2e29 6020  eld(dtype=...)` 
+00002880: 6973 2073 7065 6369 6669 6564 2c20 7468  is specified, th
+00002890: 6520 6769 7665 6e20 6474 7970 6520 7769  e given dtype wi
+000028a0: 6c6c 2061 6c77 6179 7320 6265 2066 6f72  ll always be for
+000028b0: 6365 642c 2065 7665 6e20 696e 2063 6f6d  ced, even in com
+000028c0: 7061 7469 626c 6520 6361 7365 732e 0a2a  patible cases..*
+000028d0: 2060 4461 7461 4672 616d 652e 6765 7428   `DataFrame.get(
+000028e0: 7072 6564 6963 6174 6529 6020 2d20 5265  predicate)` - Re
+000028f0: 7472 6965 7665 2061 2073 696e 676c 6520  trieve a single 
+00002900: 726f 7720 6672 6f6d 2074 6865 2064 6174  row from the dat
+00002910: 6120 6672 616d 6520 6173 2061 6e20 696e  a frame as an in
+00002920: 7374 616e 6365 206f 6620 7468 6520 6d6f  stance of the mo
+00002930: 6465 6c2e 2041 6e20 6578 6365 7074 696f  del. An exceptio
+00002940: 6e20 6973 2072 6169 7365 6420 6966 206e  n is raised if n
+00002950: 6f74 2065 7861 6374 6c79 206f 6e65 2072  ot exactly one r
+00002960: 6f77 2069 7320 7969 656c 6465 6420 6672  ow is yielded fr
+00002970: 6f6d 2074 6865 2066 696c 7465 7220 7072  om the filter pr
+00002980: 6564 6963 6174 652e 0a2a 2060 4461 7461  edicate..* `Data
+00002990: 4672 616d 652e 6669 6c6c 5f6e 756c 6c28  Frame.fill_null(
+000029a0: 7374 7261 7465 6779 3d22 6465 6661 756c  strategy="defaul
+000029b0: 7473 2229 6020 2d20 4669 6c6c 2069 6e6e  ts")` - Fill inn
+000029c0: 206d 6973 7369 6e67 2076 616c 7565 7320   missing values 
+000029d0: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
+000029e0: 2064 6566 6175 6c74 2076 616c 7565 7320   default values 
+000029f0: 7365 7420 6f6e 2074 6865 206d 6f64 656c  set on the model
+00002a00: 2073 6368 656d 612e 0a2a 2060 4461 7461   schema..* `Data
+00002a10: 4672 616d 652e 6465 7269 7665 2829 6020  Frame.derive()` 
+00002a20: 2d20 4120 6d6f 6465 6c20 6669 656c 6420  - A model field 
+00002a30: 616e 6e6f 7461 7465 6420 7769 7468 2060  annotated with `
+00002a40: 4669 656c 6428 6465 7269 7665 645f 6672  Field(derived_fr
+00002a50: 6f6d 3d2e 2e2e 2960 2069 6e64 6963 6174  om=...)` indicat
+00002a60: 6573 2074 6861 7420 6120 636f 6c75 6d6e  es that a column
+00002a70: 2073 686f 756c 6420 6265 2064 6566 696e   should be defin
+00002a80: 6564 2062 7920 736f 6d65 2061 7262 6974  ed by some arbit
+00002a90: 7261 7279 2070 6f6c 6172 7320 6578 7072  rary polars expr
+00002aa0: 6573 7369 6f6e 2e20 4966 2060 6465 7269  ession. If `deri
+00002ab0: 7665 645f 6672 6f6d 6020 6973 2073 7065  ved_from` is spe
+00002ac0: 6369 6669 6564 2061 7320 6120 7374 7269  cified as a stri
+00002ad0: 6e67 2c20 7468 656e 2074 6865 2067 6976  ng, then the giv
+00002ae0: 656e 2076 616c 7565 2077 696c 6c20 6265  en value will be
+00002af0: 2069 6e74 6572 7072 6574 6564 2061 7320   interpreted as 
+00002b00: 6120 636f 6c75 6d6e 206e 616d 6520 7769  a column name wi
+00002b10: 7468 2060 706f 6c61 7273 2e63 6f6c 2829  th `polars.col()
+00002b20: 602e 2054 6865 7365 2063 6f6c 756d 6e73  `. These columns
+00002b30: 2061 7265 2063 7265 6174 6564 2061 6e64   are created and
+00002b40: 2070 6f70 756c 6174 6564 2077 6974 6820   populated with 
+00002b50: 6461 7461 2061 6363 6f72 6469 6e67 2074  data according t
+00002b60: 6f20 7468 6520 6064 6572 6976 6564 5f66  o the `derived_f
+00002b70: 726f 6d60 2065 7870 7265 7373 696f 6e73  rom` expressions
+00002b80: 2077 6865 6e20 796f 7520 696e 766f 6b65   when you invoke
+00002b90: 2060 4461 7461 4672 616d 652e 6465 7269   `DataFrame.deri
+00002ba0: 7665 2829 602e 0a0a 5468 6573 6520 6d65  ve()`...These me
+00002bb0: 7468 6f64 7320 6172 6520 6265 7374 2069  thods are best i
+00002bc0: 6c6c 7573 7472 6174 6564 2077 6974 6820  llustrated with 
+00002bd0: 616e 2065 7861 6d70 6c65 3a0a 0a60 6060  an example:..```
+00002be0: 7079 0a66 726f 6d20 7479 7069 6e67 2069  py.from typing i
+00002bf0: 6d70 6f72 7420 4c69 7465 7261 6c0a 0a69  mport Literal..i
+00002c00: 6d70 6f72 7420 7061 7469 746f 2061 7320  mport patito as 
+00002c10: 7074 0a69 6d70 6f72 7420 706f 6c61 7273  pt.import polars
+00002c20: 2061 7320 706c 0a0a 0a63 6c61 7373 2050   as pl...class P
+00002c30: 726f 6475 6374 2870 742e 4d6f 6465 6c29  roduct(pt.Model)
+00002c40: 3a0a 2020 2020 7072 6f64 7563 745f 6964  :.    product_id
+00002c50: 3a20 696e 7420 3d20 7074 2e46 6965 6c64  : int = pt.Field
+00002c60: 2875 6e69 7175 653d 5472 7565 290a 2020  (unique=True).  
+00002c70: 2020 2320 5370 6563 6966 7920 6120 7370    # Specify a sp
+00002c80: 6563 6966 6963 2064 7479 7065 2074 6f20  ecific dtype to 
+00002c90: 6265 2075 7365 640a 2020 2020 706f 7075  be used.    popu
+00002ca0: 6c61 7269 7479 5f72 616e 6b3a 2069 6e74  larity_rank: int
+00002cb0: 203d 2070 742e 4669 656c 6428 6474 7970   = pt.Field(dtyp
+00002cc0: 653d 706c 2e55 496e 7431 3629 0a20 2020  e=pl.UInt16).   
+00002cd0: 2023 2046 6965 6c64 2077 6974 6820 6465   # Field with de
+00002ce0: 6661 756c 7420 7661 6c75 6520 2266 6f72  fault value "for
+00002cf0: 2d73 616c 6522 0a20 2020 2073 7461 7475  -sale".    statu
+00002d00: 733a 204c 6974 6572 616c 5b22 6472 6166  s: Literal["draf
+00002d10: 7422 2c20 2266 6f72 2d73 616c 6522 2c20  t", "for-sale", 
+00002d20: 2264 6973 636f 6e74 696e 7565 6422 5d20  "discontinued"] 
+00002d30: 3d20 2266 6f72 2d73 616c 6522 0a20 2020  = "for-sale".   
+00002d40: 2023 2054 6865 2065 7572 6f63 656e 7420   # The eurocent 
+00002d50: 636f 7374 2069 7320 6578 7472 6163 7465  cost is extracte
+00002d60: 6420 6672 6f6d 2074 6865 2045 7572 6f20  d from the Euro 
+00002d70: 636f 7374 2073 7472 696e 6720 22e2 82ac  cost string "...
+00002d80: 582e 5920 4555 5222 0a20 2020 2065 7572  X.Y EUR".    eur
+00002d90: 6f63 656e 745f 636f 7374 3a20 696e 7420  ocent_cost: int 
+00002da0: 3d20 7074 2e46 6965 6c64 280a 2020 2020  = pt.Field(.    
+00002db0: 2020 2020 6465 7269 7665 645f 6672 6f6d      derived_from
+00002dc0: 3d31 3030 202a 2070 6c2e 636f 6c28 2263  =100 * pl.col("c
+00002dd0: 6f73 7422 292e 7374 722e 6578 7472 6163  ost").str.extrac
+00002de0: 7428 7222 e282 ac28 5c64 2b5c 2e2b 5c64  t(r"...(\d+\.+\d
+00002df0: 2b29 2229 2e63 6173 7428 666c 6f61 7429  +)").cast(float)
+00002e00: 2e72 6f75 6e64 2832 290a 2020 2020 290a  .round(2).    ).
+00002e10: 0a0a 7072 6f64 7563 7473 203d 2070 742e  ..products = pt.
+00002e20: 4461 7461 4672 616d 6528 0a20 2020 207b  DataFrame(.    {
+00002e30: 0a20 2020 2020 2020 2022 7072 6f64 7563  .        "produc
+00002e40: 745f 6964 223a 205b 312c 2032 5d2c 0a20  t_id": [1, 2],. 
+00002e50: 2020 2020 2020 2022 706f 7075 6c61 7269         "populari
+00002e60: 7479 5f72 616e 6b22 3a20 5b32 2c20 315d  ty_rank": [2, 1]
+00002e70: 2c0a 2020 2020 2020 2020 2273 7461 7475  ,.        "statu
+00002e80: 7322 3a20 5b4e 6f6e 652c 2022 6469 7363  s": [None, "disc
+00002e90: 6f6e 7469 6e75 6564 225d 2c0a 2020 2020  ontinued"],.    
+00002ea0: 2020 2020 2263 6f73 7422 3a20 5b22 e282      "cost": ["..
+00002eb0: ac32 2e33 3020 4555 5222 2c20 22e2 82ac  .2.30 EUR", "...
+00002ec0: 312e 3139 2045 5552 225d 2c0a 2020 2020  1.19 EUR"],.    
+00002ed0: 7d0a 290a 7072 6f64 7563 7420 3d20 280a  }.).product = (.
+00002ee0: 2020 2020 7072 6f64 7563 7473 0a20 2020      products.   
+00002ef0: 2023 2053 7065 6369 6679 2074 6865 2073   # Specify the s
+00002f00: 6368 656d 6120 6f66 2074 6865 2067 6976  chema of the giv
+00002f10: 656e 2064 6174 6120 6672 616d 650a 2020  en data frame.  
+00002f20: 2020 2e73 6574 5f6d 6f64 656c 2850 726f    .set_model(Pro
+00002f30: 6475 6374 290a 2020 2020 2320 4465 7269  duct).    # Deri
+00002f40: 7665 2074 6865 2060 6575 726f 6365 6e74  ve the `eurocent
+00002f50: 5f63 6f73 7460 2069 6e74 2063 6f6c 756d  _cost` int colum
+00002f60: 6e20 6672 6f6d 2074 6865 2060 636f 7374  n from the `cost
+00002f70: 6020 7374 7269 6e67 2063 6f6c 756d 6e20  ` string column 
+00002f80: 7573 696e 6720 7265 6765 780a 2020 2020  using regex.    
+00002f90: 2e64 6572 6976 6528 290a 2020 2020 2320  .derive().    # 
+00002fa0: 4472 6f70 2074 6865 2060 636f 7374 6020  Drop the `cost` 
+00002fb0: 636f 6c75 6d6e 2061 7320 6974 2069 7320  column as it is 
+00002fc0: 6e6f 7420 7061 7274 206f 6620 7468 6520  not part of the 
+00002fd0: 6d6f 6465 6c0a 2020 2020 2e64 726f 7028  model.    .drop(
+00002fe0: 290a 2020 2020 2320 4361 7374 2074 6865  ).    # Cast the
+00002ff0: 2070 6f70 756c 6172 6974 7920 7261 6e6b   popularity rank
+00003000: 2063 6f6c 756d 6e20 746f 2061 6e20 756e   column to an un
+00003010: 7369 676e 6564 2031 362d 6269 7420 696e  signed 16-bit in
+00003020: 7465 6765 7220 616e 6420 6365 6e74 7320  teger and cents 
+00003030: 746f 2061 6e20 696e 7465 6765 720a 2020  to an integer.  
+00003040: 2020 2e63 6173 7428 290a 2020 2020 2320    .cast().    # 
+00003050: 4669 6c6c 206d 6973 7369 6e67 2076 616c  Fill missing val
+00003060: 7565 7320 7769 7468 2074 6865 2064 6566  ues with the def
+00003070: 6175 6c74 2076 616c 7565 7320 7370 6563  ault values spec
+00003080: 6966 6965 6420 696e 2074 6865 2073 6368  ified in the sch
+00003090: 656d 610a 2020 2020 2e66 696c 6c5f 6e75  ema.    .fill_nu
+000030a0: 6c6c 2873 7472 6174 6567 793d 2264 6566  ll(strategy="def
+000030b0: 6175 6c74 7322 290a 2020 2020 2320 4173  aults").    # As
+000030c0: 7365 7274 2074 6861 7420 7468 6520 6461  sert that the da
+000030d0: 7461 2066 7261 6d65 206e 6f77 2063 6f6d  ta frame now com
+000030e0: 706c 6965 7320 7769 7468 2074 6865 2073  plies with the s
+000030f0: 6368 656d 610a 2020 2020 2e76 616c 6964  chema.    .valid
+00003100: 6174 6528 290a 2020 2020 2320 5265 7472  ate().    # Retr
+00003110: 6965 7665 2061 2073 696e 676c 6520 726f  ieve a single ro
+00003120: 7720 616e 6420 6361 7374 2069 7420 746f  w and cast it to
+00003130: 2074 6865 206d 6f64 656c 2063 6c61 7373   the model class
+00003140: 0a20 2020 202e 6765 7428 706c 2e63 6f6c  .    .get(pl.col
+00003150: 2822 7072 6f64 7563 745f 6964 2229 203d  ("product_id") =
+00003160: 3d20 3129 0a29 0a70 7269 6e74 2872 6570  = 1).).print(rep
+00003170: 7228 7072 6f64 7563 7429 290a 2320 5072  r(product)).# Pr
+00003180: 6f64 7563 7428 7072 6f64 7563 745f 6964  oduct(product_id
+00003190: 3d31 2c20 706f 7075 6c61 7269 7479 5f72  =1, popularity_r
+000031a0: 616e 6b3d 322c 2073 7461 7475 733d 2766  ank=2, status='f
+000031b0: 6f72 2d73 616c 6527 2c20 6575 726f 6365  or-sale', euroce
+000031c0: 6e74 5f63 6f73 743d 3233 3029 0a60 6060  nt_cost=230).```
+000031d0: 0a0a 4576 6572 7920 5061 7469 746f 206d  ..Every Patito m
+000031e0: 6f64 656c 2061 7574 6f6d 6174 6963 616c  odel automatical
+000031f0: 6c79 2067 6574 7320 6120 602e 4461 7461  ly gets a `.Data
+00003200: 4672 616d 6560 2061 7474 7269 6275 7465  Frame` attribute
+00003210: 2c20 6120 6375 7374 6f6d 2064 6174 6120  , a custom data 
+00003220: 6672 616d 6520 7375 6263 6c61 7373 2077  frame subclass w
+00003230: 6865 7265 2060 2e73 6574 5f6d 6f64 656c  here `.set_model
+00003240: 2829 6020 6973 2069 6e76 6f6b 6564 2061  ()` is invoked a
+00003250: 7420 696e 7374 616e 7469 6174 696f 6e2e  t instantiation.
+00003260: 2057 6974 6820 6f74 6865 7220 776f 7264   With other word
+00003270: 732c 2060 7074 2e44 6174 6146 7261 6d65  s, `pt.DataFrame
+00003280: 282e 2e2e 292e 7365 745f 6d6f 6465 6c28  (...).set_model(
+00003290: 5072 6f64 7563 7429 6020 6973 2065 7175  Product)` is equ
+000032a0: 6976 616c 656e 7420 746f 2060 5072 6f64  ivalent to `Prod
+000032b0: 7563 742e 4461 7461 4672 616d 6528 2e2e  uct.DataFrame(..
+000032c0: 2e29 602e 0a0a 2323 20f0 9f90 8d20 5265  .)`...## .... Re
+000032d0: 7072 6573 656e 7469 6e67 2072 6f77 7320  presenting rows 
+000032e0: 6173 2063 6c61 7373 6573 0a0a 4461 7461  as classes..Data
+000032f0: 2066 7261 6d65 7320 6172 6520 7461 696c   frames are tail
+00003300: 6f72 2d6d 6164 6520 666f 7220 7065 7266  or-made for perf
+00003310: 6f72 6d69 6e67 2076 6563 746f 7269 7a65  orming vectorize
+00003320: 6420 6f70 6572 6174 696f 6e73 206f 7665  d operations ove
+00003330: 7220 6120 5f73 6574 5f20 6f66 206f 626a  r a _set_ of obj
+00003340: 6563 7473 2e0a 4275 7420 7768 656e 2074  ects..But when t
+00003350: 6865 2074 696d 6520 636f 6d65 7320 746f  he time comes to
+00003360: 2072 6574 7269 6576 696e 6720 6120 5f73   retrieving a _s
+00003370: 696e 676c 655f 2072 6f77 2061 6e64 206f  ingle_ row and o
+00003380: 7065 7261 7465 2075 706f 6e20 6974 2c20  perate upon it, 
+00003390: 7468 6520 6461 7461 2066 7261 6d65 2063  the data frame c
+000033a0: 6f6e 7374 7275 6374 206e 6174 7572 616c  onstruct natural
+000033b0: 6c79 2066 616c 6c73 2073 686f 7274 2e0a  ly falls short..
+000033c0: 5061 7469 746f 2061 6c6c 6f77 7320 796f  Patito allows yo
+000033d0: 7520 746f 2065 6d62 6564 2072 6f77 2d6c  u to embed row-l
+000033e0: 6576 656c 206c 6f67 6963 2069 6e20 6d65  evel logic in me
+000033f0: 7468 6f64 7320 6465 6669 6e65 6420 6f6e  thods defined on
+00003400: 2074 6865 206d 6f64 656c 2e0a 0a0a 6060   the model....``
+00003410: 6070 790a 2320 6d6f 6465 6c73 2e70 790a  `py.# models.py.
+00003420: 696d 706f 7274 2070 6174 6974 6f20 6173  import patito as
+00003430: 2070 740a 0a63 6c61 7373 2050 726f 6475   pt..class Produ
+00003440: 6374 2870 742e 4d6f 6465 6c29 3a0a 2020  ct(pt.Model):.  
+00003450: 2020 7072 6f64 7563 745f 6964 3a20 696e    product_id: in
+00003460: 7420 3d20 7074 2e46 6965 6c64 2875 6e69  t = pt.Field(uni
+00003470: 7175 653d 5472 7565 290a 2020 2020 6e61  que=True).    na
+00003480: 6d65 3a20 7374 720a 0a20 2020 2040 7072  me: str..    @pr
+00003490: 6f70 6572 7479 0a20 2020 2064 6566 2075  operty.    def u
+000034a0: 726c 2873 656c 6629 202d 3e20 7374 723a  rl(self) -> str:
+000034b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000034c0: 280a 2020 2020 2020 2020 2020 2020 2268  (.            "h
+000034d0: 7474 7073 3a2f 2f65 7861 6d70 6c65 2e63  ttps://example.c
+000034e0: 6f6d 2f6e 6f2f 7072 6f64 7563 7473 2f22  om/no/products/"
+000034f0: 0a20 2020 2020 2020 2020 2020 2066 227b  .            f"{
+00003500: 7365 6c66 2e70 726f 6475 6374 5f69 647d  self.product_id}
+00003510: 2d22 0a20 2020 2020 2020 2020 2020 2066  -".            f
+00003520: 227b 7365 6c66 2e6e 616d 652e 6c6f 7765  "{self.name.lowe
+00003530: 7228 292e 7265 706c 6163 6528 2720 272c  r().replace(' ',
+00003540: 2027 2d27 297d 220a 2020 2020 2020 2020   '-')}".        
+00003550: 290a 6060 600a 0a54 6865 2063 6c61 7373  ).```..The class
+00003560: 2063 616e 2062 6520 696e 7374 616e 7469   can be instanti
+00003570: 6174 6564 2066 726f 6d20 6120 7369 6e67  ated from a sing
+00003580: 6c65 2072 6f77 206f 6620 6120 6461 7461  le row of a data
+00003590: 2066 7261 6d65 2062 7920 7573 696e 6720   frame by using 
+000035a0: 7468 6520 6066 726f 6d5f 726f 7728 2960  the `from_row()`
+000035b0: 206d 6574 686f 643a 0a0a 6060 6070 790a   method:..```py.
+000035c0: 7072 6f64 7563 7473 203d 2070 6c2e 4461  products = pl.Da
+000035d0: 7461 4672 616d 6528 0a20 2020 207b 0a20  taFrame(.    {. 
+000035e0: 2020 2020 2020 2022 7072 6f64 7563 745f         "product_
+000035f0: 6964 223a 205b 312c 2032 5d2c 0a20 2020  id": [1, 2],.   
+00003600: 2020 2020 2022 6e61 6d65 223a 205b 2253       "name": ["S
+00003610: 6b69 6d6d 6564 206d 696c 6b22 2c20 2245  kimmed milk", "E
+00003620: 6767 7322 5d2c 0a20 2020 207d 0a29 0a6d  ggs"],.    }.).m
+00003630: 696c 6b5f 726f 7720 3d20 7072 6f64 7563  ilk_row = produc
+00003640: 7473 2e66 696c 7465 7228 706c 2e63 6f6c  ts.filter(pl.col
+00003650: 2822 7072 6f64 7563 745f 6964 2220 3d3d  ("product_id" ==
+00003660: 2031 2929 0a6d 696c 6b20 3d20 5072 6f64   1)).milk = Prod
+00003670: 7563 742e 6672 6f6d 5f72 6f77 286d 696c  uct.from_row(mil
+00003680: 6b5f 726f 7729 0a70 7269 6e74 286d 696c  k_row).print(mil
+00003690: 6b2e 7572 6c29 0a23 2068 7474 7073 3a2f  k.url).# https:/
+000036a0: 2f65 7861 6d70 6c65 2e63 6f6d 2f6e 6f2f  /example.com/no/
+000036b0: 7072 6f64 7563 7473 2f31 2d73 6b69 6d6d  products/1-skimm
+000036c0: 6564 2d6d 696c 6b0a 6060 600a 0a49 6620  ed-milk.```..If 
+000036d0: 796f 7520 2263 6f6e 6e65 6374 2220 7468  you "connect" th
+000036e0: 6520 6050 726f 6475 6374 6020 6d6f 6465  e `Product` mode
+000036f0: 6c20 7769 7468 2074 6865 2060 4461 7461  l with the `Data
+00003700: 4672 616d 6560 2062 7920 7468 6520 7573  Frame` by the us
+00003710: 6520 6f66 2060 7061 7469 746f 2e44 6174  e of `patito.Dat
+00003720: 6146 7261 6d65 2e73 6574 5f6d 6f64 656c  aFrame.set_model
+00003730: 2829 602c 206f 7220 616c 7465 726e 6174  ()`, or alternat
+00003740: 6976 656c 7920 6279 2075 7369 6e67 2060  ively by using `
+00003750: 5072 6f64 7563 742e 4461 7461 4672 616d  Product.DataFram
+00003760: 6560 2064 6972 6563 746c 792c 2079 6f75  e` directly, you
+00003770: 2063 616e 2075 7365 2074 6865 2060 2e67   can use the `.g
+00003780: 6574 2829 6020 6d65 7468 6f64 2069 6e20  et()` method in 
+00003790: 6f72 6465 7220 746f 2066 696c 7465 7220  order to filter 
+000037a0: 7468 6520 6461 7461 2066 7261 6d65 2064  the data frame d
+000037b0: 6f77 6e20 746f 2061 2073 696e 676c 6520  own to a single 
+000037c0: 726f 7720 5f61 6e64 5f20 6361 7374 2069  row _and_ cast i
+000037d0: 7420 746f 2074 6865 2072 6573 7065 6374  t to the respect
+000037e0: 6976 6520 6d6f 6465 6c20 636c 6173 733a  ive model class:
+000037f0: 0a0a 6060 6070 790a 0a70 726f 6475 6374  ..```py..product
+00003800: 7320 3d20 5072 6f64 7563 742e 4461 7461  s = Product.Data
+00003810: 4672 616d 6528 0a20 2020 207b 0a20 2020  Frame(.    {.   
+00003820: 2020 2020 2022 7072 6f64 7563 745f 6964       "product_id
+00003830: 223a 205b 312c 2032 5d2c 0a20 2020 2020  ": [1, 2],.     
+00003840: 2020 2022 6e61 6d65 223a 205b 2253 6b69     "name": ["Ski
+00003850: 6d6d 6564 206d 696c 6b22 2c20 2245 6767  mmed milk", "Egg
+00003860: 7322 5d2c 0a20 2020 207d 0a29 0a6d 696c  s"],.    }.).mil
+00003870: 6b20 3d20 7072 6f64 7563 7473 2e67 6574  k = products.get
+00003880: 2870 6c2e 636f 6c28 2270 726f 6475 6374  (pl.col("product
+00003890: 5f69 6422 2920 3d3d 2031 290a 7072 696e  _id") == 1).prin
+000038a0: 7428 6d69 6c6b 2e75 726c 290a 2320 6874  t(milk.url).# ht
+000038b0: 7470 733a 2f2f 6578 616d 706c 652e 636f  tps://example.co
+000038c0: 6d2f 6e6f 2f70 726f 6475 6374 732f 312d  m/no/products/1-
+000038d0: 736b 696d 6d65 642d 6d69 6c6b 0a60 6060  skimmed-milk.```
+000038e0: 0a0a                                     ..
```

