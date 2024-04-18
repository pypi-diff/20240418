# Comparing `tmp/cycquery-0.1.6.tar.gz` & `tmp/cycquery-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycquery-0.1.6.tar", max compression
+gzip compressed data, was "cycquery-0.1.7.tar", max compression
```

## Comparing `cycquery-0.1.6.tar` & `cycquery-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11347 2024-03-04 17:21:16.956846 cycquery-0.1.6/LICENSE.md
--rw-r--r--   0        0        0     4038 2024-03-04 17:21:16.956846 cycquery-0.1.6/README.md
--rw-r--r--   0        0        0      528 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/__init__.py
--rw-r--r--   0        0        0     8097 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/base.py
--rw-r--r--   0        0        0      330 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/eicu.py
--rw-r--r--   0        0        0     6680 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/gemini.py
--rw-r--r--   0        0        0     7527 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/interface.py
--rw-r--r--   0        0        0     2123 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/mimiciii.py
--rw-r--r--   0        0        0     5034 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/mimiciv.py
--rw-r--r--   0        0        0     7847 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/omop.py
--rw-r--r--   0        0        0    91642 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/ops.py
--rw-r--r--   0        0        0    15678 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/orm.py
--rw-r--r--   0        0        0       49 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/post_process/__init__.py
--rw-r--r--   0        0        0     1258 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/post_process/gemini.py
--rw-r--r--   0        0        0     4632 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/post_process/mimiciv.py
--rw-r--r--   0        0        0     3725 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/post_process/util.py
--rw-r--r--   0        0        0    33784 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/util.py
--rw-r--r--   0        0        0       23 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/utils/__init__.py
--rw-r--r--   0        0        0     4962 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/utils/common.py
--rw-r--r--   0        0        0    10208 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/utils/file.py
--rw-r--r--   0        0        0     3610 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/utils/log.py
--rw-r--r--   0        0        0      875 2024-03-04 17:21:16.956846 cycquery-0.1.6/cycquery/utils/profile.py
--rw-r--r--   0        0        0     3326 2024-03-04 17:21:16.960846 cycquery-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4930 1970-01-01 00:00:00.000000 cycquery-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-04-18 16:18:51.522804 cycquery-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0     3239 2024-04-18 16:18:51.522804 cycquery-0.1.7/README.md
+-rw-r--r--   0        0        0      315 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/base.py
+-rw-r--r--   0        0        0      330 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/eicu.py
+-rw-r--r--   0        0        0     6680 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/gemini.py
+-rw-r--r--   0        0        0     7527 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/interface.py
+-rw-r--r--   0        0        0     2123 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/mimiciii.py
+-rw-r--r--   0        0        0     5034 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/mimiciv.py
+-rw-r--r--   0        0        0     7847 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/omop.py
+-rw-r--r--   0        0        0    91618 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/ops.py
+-rw-r--r--   0        0        0    16206 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/orm.py
+-rw-r--r--   0        0        0       49 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/post_process/__init__.py
+-rw-r--r--   0        0        0     1258 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/post_process/gemini.py
+-rw-r--r--   0        0        0     4632 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/post_process/mimiciv.py
+-rw-r--r--   0        0        0     3725 2024-04-18 16:18:51.522804 cycquery-0.1.7/cycquery/post_process/util.py
+-rw-r--r--   0        0        0    33704 2024-04-18 16:18:51.526804 cycquery-0.1.7/cycquery/util.py
+-rw-r--r--   0        0        0       23 2024-04-18 16:18:51.526804 cycquery-0.1.7/cycquery/utils/__init__.py
+-rw-r--r--   0        0        0     4963 2024-04-18 16:18:51.526804 cycquery-0.1.7/cycquery/utils/common.py
+-rw-r--r--   0        0        0    10208 2024-04-18 16:18:51.526804 cycquery-0.1.7/cycquery/utils/file.py
+-rw-r--r--   0        0        0     3610 2024-04-18 16:18:51.526804 cycquery-0.1.7/cycquery/utils/log.py
+-rw-r--r--   0        0        0      875 2024-04-18 16:18:51.526804 cycquery-0.1.7/cycquery/utils/profile.py
+-rw-r--r--   0        0        0     3334 2024-04-18 16:18:51.530804 cycquery-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4116 1970-01-01 00:00:00.000000 cycquery-0.1.7/PKG-INFO
```

### Comparing `cycquery-0.1.6/LICENSE.md` & `cycquery-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/README.md` & `cycquery-0.1.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-cyclops-query
+cycquery
 --------------------------------------------------------------------------------
 
 [![PyPI](https://img.shields.io/pypi/v/cycquery)](https://pypi.org/project/cycquery)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cycquery)
-[![code checks](https://github.com/VectorInstitute/cyclops-query/actions/workflows/code_checks.yml/badge.svg)](https://github.com/VectorInstitute/cyclops-query/actions/workflows/code_checks.yml)
-[![integration tests](https://github.com/VectorInstitute/cyclops-query/actions/workflows/integration_tests.yml/badge.svg)](https://github.com/VectorInstitute/cyclops-query/actions/workflows/integration_tests.yml)
-[![docs](https://github.com/VectorInstitute/cyclops-query/actions/workflows/docs_deploy.yml/badge.svg)](https://github.com/VectorInstitute/cyclops-query/actions/workflows/docs_deploy.yml)
-[![codecov](https://codecov.io/gh/VectorInstitute/cyclops-query/branch/main/graph/badge.svg)](https://codecov.io/gh/VectorInstitute/cyclops-query)
-[![license](https://img.shields.io/github/license/VectorInstitute/cyclops-query.svg)](https://github.com/VectorInstitute/cyclops-query/blob/main/LICENSE)
+[![code checks](https://github.com/VectorInstitute/cycquery/actions/workflows/code_checks.yml/badge.svg)](https://github.com/VectorInstitute/cycquery/actions/workflows/code_checks.yml)
+[![integration tests](https://github.com/VectorInstitute/cycquery/actions/workflows/integration_tests.yml/badge.svg)](https://github.com/VectorInstitute/cycquery/actions/workflows/integration_tests.yml)
+[![docs](https://github.com/VectorInstitute/cycquery/actions/workflows/docs_deploy.yml/badge.svg)](https://github.com/VectorInstitute/cycquery/actions/workflows/docs_deploy.yml)
+[![codecov](https://codecov.io/gh/VectorInstitute/cycquery/branch/main/graph/badge.svg)](https://codecov.io/gh/VectorInstitute/cycquery)
+[![license](https://img.shields.io/github/license/VectorInstitute/cycquery.svg)](https://github.com/VectorInstitute/cycquery/blob/main/LICENSE)
 
-``cyclops-query`` is a tool for querying relational databases using a simple Python API. It is specifically developed to query
+``cycquery`` is a tool for querying relational databases using a simple Python API. It is specifically developed to query
 Electronic Health Record (EHR) databases. The tool is a wrapper around [SQLAlchemy](https://www.sqlalchemy.org/) and can be used
 to write SQL-like queries in Python, including joins, conditions, groupby aggregation and many more.
 
 ## 🐣 Getting Started
 
-### Installing cyclops-query using pip
+### Installing cycquery using pip
 
 ```bash
 python3 -m pip install cycquery
 ```
 
 ### Query postgresql database
 
@@ -85,31 +85,13 @@
 python3 -m poetry install --with docs
 cd docs
 make html SPHINXOPTS="-D nbsphinx_allow_errors=True"
 ```
 
 ### Contributing
 
-Contributing to ``cyclops-query`` is welcomed.
-See [Contributing](https://vectorinstitute.github.io/cyclops-query/api/contributing.html) for
+Contributing to ``cycquery`` is welcomed.
+See [Contributing](https://vectorinstitute.github.io/cycquery/api/contributing.html) for
 guidelines.
 
 
-## 📚 [Documentation](https://vectorinstitute.github.io/cyclops-query/)
-
-
-## 🎓 Citation
-
-Reference to cite when you use ``cyclops-query`` in a project or a research paper:
-
-```
-@article {Krishnan2022.12.02.22283021,
-	author = {Krishnan, Amrit and Subasri, Vallijah and McKeen, Kaden and Kore, Ali and Ogidi, Franklin and Alinoori, Mahshid and Lalani, Nadim and Dhalla, Azra and Verma, Amol and Razak, Fahad and Pandya, Deval and Dolatabadi, Elham},
-	title = {CyclOps: Cyclical development towards operationalizing ML models for health},
-	elocation-id = {2022.12.02.22283021},
-	year = {2022},
-	doi = {10.1101/2022.12.02.22283021},
-	publisher = {Cold Spring Harbor Laboratory Press},
-	URL = {https://www.medrxiv.org/content/early/2022/12/08/2022.12.02.22283021},
-	journal = {medRxiv}
-}
-```
+## 📚 [Documentation](https://vectorinstitute.github.io/cycquery/)
```

### Comparing `cycquery-0.1.6/cycquery/base.py` & `cycquery-0.1.7/cycquery/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,16 @@
     host : str, optional
         The host address of the database, by default empty. Not used for SQLite.
     port : int, optional
         The port number for the database, by default None. Not used for SQLite.
     database : str, optional
         The name of the database or the path to the database file (for SQLite),
         by default empty.
+    schemas : Union[str, List[str]], optional
+        The schema(s) to query, by default None.
 
     Notes
     -----
     This class is intended to be subclassed to provide methods for querying tables in
     the database. This class automatically creates methods for querying tables in the
     database. The methods are named after the schema and table name, i.e.
     `self.schema_name.table_name()`. The methods are created when the class is
@@ -105,22 +107,24 @@
         self,
         dbms: str,
         user: str = "",
         password: str = "",
         host: str = "",
         port: Optional[int] = None,
         database: str = "",
+        schemas: Optional[List[str]] = None,
     ) -> None:
         config = DatasetQuerierConfig(
             database=database,
             user=user,
             password=password,
             dbms=dbms,
             host=host,
             port=port,
+            schemas=schemas,
         )
         self.db = Database(config)
         if not self.db.is_connected:
             LOGGER.error("Database is not connected, cannot run queries.")
             return
         self._setup_table_methods()
 
@@ -129,15 +133,23 @@
 
         Returns
         -------
         List[str]
             List of schema names.
 
         """
-        return list(self.db.inspector.get_schema_names())
+        all_schemas = list(self.db.inspector.get_schema_names())
+        if self.db.config.schemas is None:
+            return all_schemas
+        if isinstance(self.db.config.schemas, str):
+            schemas_to_use = [self.db.config.schemas]
+        else:
+            schemas_to_use = self.db.config.schemas
+
+        return [schema for schema in all_schemas if schema in schemas_to_use]
 
     def list_tables(self, schema_name: Optional[str] = None) -> List[str]:
         """List table methods that can be queried using the database.
 
         Parameters
         ----------
         schema_name
```

### Comparing `cycquery-0.1.6/cycquery/gemini.py` & `cycquery-0.1.7/cycquery/gemini.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/interface.py` & `cycquery-0.1.7/cycquery/interface.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/mimiciii.py` & `cycquery-0.1.7/cycquery/mimiciii.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/mimiciv.py` & `cycquery-0.1.7/cycquery/mimiciv.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/omop.py` & `cycquery-0.1.7/cycquery/omop.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/ops.py` & `cycquery-0.1.7/cycquery/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,24 +269,21 @@
     --------
     >>> Sequential(Drop(["col1", "col2"]), ...)
     >>> Sequential([Drop(["col1", "col2"]), ...])
 
     """
 
     @typing.overload
-    def __init__(self, *ops: QueryOp) -> None:
-        ...
+    def __init__(self, *ops: QueryOp) -> None: ...
 
     @typing.overload
-    def __init__(self, ops: typing.List[QueryOp]) -> None:
-        ...
+    def __init__(self, ops: typing.List[QueryOp]) -> None: ...
 
     @typing.overload
-    def __init__(self, op: OrderedDict[str, QueryOp]) -> None:
-        ...
+    def __init__(self, op: OrderedDict[str, QueryOp]) -> None: ...
 
     def __init__(self, *args: QueryOp) -> None:  # type: ignore
         """Initialize the class.
 
         Parameters
         ----------
         args
```

### Comparing `cycquery-0.1.6/cycquery/orm.py` & `cycquery-0.1.7/cycquery/orm.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,23 +113,26 @@
     host : str, optional
         The host address of the database, by default empty. Not used for SQLite.
     port : int, optional
         The port number for the database, by default None. Not used for SQLite.
     database : str, optional
         The name of the database or the path to the database file (for SQLite),
         by default empty.
+    schemas : Union[str, List[str]], optional
+        The schema(s) to be used for querying, by default None.
 
     """
 
     dbms: str
     user: str = ""
     password: str = ""
     host: str = ""
     port: Optional[int] = None
     database: str = ""
+    schemas: Optional[Union[str, List[str]]] = None
 
 
 class Database:
     """Database class.
 
     Attributes
     ----------
@@ -234,28 +237,35 @@
         """
         return self._tables
 
     def _setup(self) -> None:
         """Prepare ORM DB."""
         meta: Dict[str, MetaData] = {}
         schemas = self.inspector.get_schema_names()
+        if self.config.schemas is None:
+            schemas_to_use = schemas
+        elif isinstance(self.config.schemas, str):
+            schemas_to_use = [self.config.schemas]
+        else:
+            schemas_to_use = self.config.schemas
         for schema_name in schemas:
-            metadata = MetaData(schema=schema_name)
-            metadata.reflect(bind=self.engine)
-            meta[schema_name] = metadata
-            schema = DBSchema(schema_name, meta[schema_name])
-            for table_name in meta[schema_name].tables:
-                table = DBTable(table_name, meta[schema_name].tables[table_name])
-                for column in meta[schema_name].tables[table_name].columns:
-                    setattr(table, column.name, column)
-                if not isinstance(table.name_, str):
-                    table.name_ = str(table.name_)
-                self._tables.append(table.name_)
-                setattr(schema, get_attr_name(table.name_), table)
-            setattr(self, schema_name, schema)
+            if schemas_to_use is None or schema_name in schemas_to_use:
+                metadata = MetaData(schema=schema_name)
+                metadata.reflect(bind=self.engine)
+                meta[schema_name] = metadata
+                schema = DBSchema(schema_name, meta[schema_name])
+                for table_name in meta[schema_name].tables:
+                    table = DBTable(table_name, meta[schema_name].tables[table_name])
+                    for column in meta[schema_name].tables[table_name].columns:
+                        setattr(table, column.name, column)
+                    if not isinstance(table.name_, str):
+                        table.name_ = str(table.name_)
+                    self._tables.append(table.name_)
+                    setattr(schema, get_attr_name(table.name_), table)
+                setattr(self, schema_name, schema)
 
     @time_function
     @table_params_to_type(Select)
     def run_query(
         self,
         query: Union[TableTypes, str],
         dtype_backend: str = "pyarrow",
```

### Comparing `cycquery-0.1.6/cycquery/post_process/gemini.py` & `cycquery-0.1.7/cycquery/post_process/gemini.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/post_process/mimiciv.py` & `cycquery-0.1.7/cycquery/post_process/mimiciv.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/post_process/util.py` & `cycquery-0.1.7/cycquery/post_process/util.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/util.py` & `cycquery-0.1.7/cycquery/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 
 def _to_subquery(table: TableTypes) -> Subquery:
     """Convert a table from a table type object to the Subquery type.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         Table to convert.
 
     Returns
     -------
     sqlalchemy.sql.selectable.Subquery
         The converted table.
 
@@ -100,15 +100,15 @@
 
 
 def _to_select(table: TableTypes) -> Select:
     """Convert a table from a table type object to the Select type.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         Table to convert.
 
     Returns
     -------
     sqlalchemy.sql.selectable.Select
         The converted table.
 
@@ -180,15 +180,15 @@
 
 
 def table_params_to_type(to_type: TableTypes) -> Callable[..., Any]:
     """Decorate to convert TableTypes params to a specified type.
 
     Parameters
     ----------
-    to_type: cyclops.query.util.TableTypes
+    to_type: cycquery.util.TableTypes
         The type to which to convert.
 
     Returns
     -------
     Callable
         The processed function.
 
@@ -213,15 +213,15 @@
     table: TableTypes,
     col: str,
 ) -> Column:
     """Extract a column object from a table by name.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table with the column.
     col: str
         Name of column to extract.
 
     Returns
     -------
     sqlalchemy.sql.schema.Column
@@ -240,15 +240,15 @@
     table: TableTypes,
     cols: Union[str, List[str]],
 ) -> Subquery:
     """Filter a table, keeping only the specified columns.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table with the column.
     cols: str or list of str
         Name of columns to keep.
 
     Returns
     -------
     sqlalchemy.sql.selectable.Subquery
@@ -271,15 +271,15 @@
     table: TableTypes,
     cols: Union[str, List[str]],
 ) -> List[Column]:
     """Extract a number of columns from the table.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table.
     cols: str or list of str
         Names of columns to extract.
 
     Returns
     -------
     list of sqlalchemy.sql.schema.Column
@@ -291,15 +291,15 @@
 
 @table_params_to_type(Subquery)
 def get_column_names(table: TableTypes) -> List[str]:
     """Extract column names from a table.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table.
 
     Returns
     -------
     list of str
         The table column names.
 
@@ -313,15 +313,15 @@
     cols: Union[str, List[str]],
     raise_error: bool = False,
 ) -> bool:
     """Check whether a table has all of the specified columns.
 
     Parameters
     ----------
-    table : cyclops.query.util.TableTypes
+    table : cycquery.util.TableTypes
         Table to check.
     cols: str or list of str
         Required columns.
     raise_error: bool
         Whether to raise an error if the required columns are not found.
 
     Returns
@@ -409,15 +409,15 @@
     table: TableTypes,
     drop_cols: Union[str, List[str]],
 ) -> Subquery:
     """Drop, or remove, some columns from a table.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table.
     col : str or list of str
         Names of columns to drop.
     drop_cols: str or list of str
         Names of columns to drop.
 
     Returns
@@ -436,15 +436,15 @@
     """Rename a table's columns.
 
     Rename the table's columns according to a dictionary of strings,
     where the key is the current name, and the value is the replacement.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table.
     rename_map : dict
         Dictionary mapping current column names (key) to new ones (value).
 
     Returns
     -------
     sqlalchemy.sql.selectable.Subquery
@@ -461,15 +461,15 @@
 
 @table_params_to_type(Subquery)
 def reorder_columns(table: TableTypes, cols: List[str]) -> Subquery:
     """Reorder a table's columns.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table to reorder.
     cols : list of str
         New order of columns, which must include all existing columns.
 
     Returns
     -------
     sqlalchemy.sql.selectable.Subquery
@@ -510,15 +510,15 @@
     """Apply a function to some columns.
 
     This function can change existing columns or create new
     columns depending on whether new_col_labels is specified.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table.
     col_names: str or list of str
         Columns to which to apply the function.
     funcs: callable or list of callable
         Function(s) to apply to the columns, where the function takes an column
         as its only parameter and returns another column object.
     new_col_labels: str or list of str, optional
@@ -571,15 +571,15 @@
 ) -> Subquery:
     """Trim, or strip, specified columns.
 
     Trimming refers to the removal of leading/trailing whitespace.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table.
     cols: str or list of str
         Names of columns to trim.
     new_col_labels: str or list of str, optional
         If specified, create new columns with these labels. Otherwise,
         apply the function to the existing columns.
 
@@ -1096,15 +1096,15 @@
     types: Union[Any, List[Any]],
     raise_error: bool = False,
 ) -> bool:
     """Check whether some columns are each one of a number of types.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table.
     cols: str or list of str
         Column names to check.
     types: any
         The allowed types for each column.
     raise_error: bool
         Whether to raise an error if one of the columns are none of the types.
@@ -1140,15 +1140,15 @@
     cols: Union[str, List[str]],
     raise_error: bool = False,
 ) -> bool:
     """Check whether some columns are Date or DateTime columns.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table.
     cols: str or list of str
         Column names to check.
     raise_error: bool
         Whether to raise an error if one of the columns are none of the types.
 
     Returns
@@ -1173,15 +1173,15 @@
     Create a time delta (interval) column from a number of
     numeric timestamp columns.
 
     Warning: Null values in each specified numeric time column are coalesced to 0.
 
     Parameters
     ----------
-    table: cyclops.query.util.TableTypes
+    table: cycquery.util.TableTypes
         The table.
     years: None or str
         Years column.
     months: None or str
         Months column.
     days: None or str
         Days column.
```

### Comparing `cycquery-0.1.6/cycquery/utils/common.py` & `cycquery-0.1.7/cycquery/utils/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Common utility functions that can be used across multiple cyclops packages."""
+"""Common utility functions that can be used across multiple cycquery packages."""
 
 import warnings
 from datetime import datetime
 from typing import Any, List, Optional, Union
 
 import numpy as np
 import numpy.typing as npt
```

### Comparing `cycquery-0.1.6/cycquery/utils/file.py` & `cycquery-0.1.7/cycquery/utils/file.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/utils/log.py` & `cycquery-0.1.7/cycquery/utils/log.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/cycquery/utils/profile.py` & `cycquery-0.1.7/cycquery/utils/profile.py`

 * *Files identical despite different names*

### Comparing `cycquery-0.1.6/pyproject.toml` & `cycquery-0.1.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "cycquery"
-version = "0.1.6"
+version = "0.1.7"
 description = "A tool to query EHR databases"
 authors = ["Vector AI Engineering <cyclops@vectorinstitute.ai>"]
 license = "Apache-2.0"
-repository = "https://github.com/VectorInstitute/cyclops-query"
-documentation = "https://vectorinstitute.github.io/cyclops-query/"
+repository = "https://github.com/VectorInstitute/cycquery"
+documentation = "https://vectorinstitute.github.io/cycquery/"
 packages = [
     { include = "cycquery" },
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
@@ -20,37 +20,38 @@
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.1"
 pre-commit = "^2.17.0"
-black = "^22.1.0"
 pytest-cov = "^3.0.0"
 codecov = "^2.1.13"
 nbstripout = "^0.6.1"
 mypy = "^1.0.0"
-ruff = "^0.2.0"
+ruff = "^0.3.0"
 nbqa = { version = "^1.7.0", extras = ["toolchain"] }
+pip-audit = "^2.7.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 numpydoc = "^1.2"
 sphinx = "^7.2.5"
-sphinx-rtd-theme = "^2.0.0rc2"
 sphinxcontrib-apidoc = "^0.4.0"
 sphinx-autodoc-typehints = "^1.24.0"
 myst-parser = "^2.0.0"
+sphinx-design = "^0.5.0"
 sphinx-copybutton = "^0.5.0"
 sphinx-autoapi = "^2.0.0"
 nbsphinx = "^0.8.11"
 ipython = "^8.8.0"
 ipykernel = "^6.23.0"
+furo = "^2024.01.29"
 
 [tool.mypy]
 ignore_missing_imports = true
 install_types = true
 pretty = true
 namespace_packages = true
 explicit_package_bases = true
```

### Comparing `cycquery-0.1.6/PKG-INFO` & `cycquery-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: cycquery
-Version: 0.1.6
+Version: 0.1.7
 Summary: A tool to query EHR databases
-Home-page: https://github.com/VectorInstitute/cyclops-query
+Home-page: https://github.com/VectorInstitute/cycquery
 License: Apache-2.0
 Author: Vector AI Engineering
 Author-email: cyclops@vectorinstitute.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=1.4.32,<2.0.0)
 Requires-Dist: pandas (>2.0.0,<2.2.0)
 Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Requires-Dist: pyarrow (>=14.0.0,<15.0.0)
-Project-URL: Documentation, https://vectorinstitute.github.io/cyclops-query/
-Project-URL: Repository, https://github.com/VectorInstitute/cyclops-query
+Project-URL: Documentation, https://vectorinstitute.github.io/cycquery/
+Project-URL: Repository, https://github.com/VectorInstitute/cycquery
 Description-Content-Type: text/markdown
 
-cyclops-query
+cycquery
 --------------------------------------------------------------------------------
 
 [![PyPI](https://img.shields.io/pypi/v/cycquery)](https://pypi.org/project/cycquery)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cycquery)
-[![code checks](https://github.com/VectorInstitute/cyclops-query/actions/workflows/code_checks.yml/badge.svg)](https://github.com/VectorInstitute/cyclops-query/actions/workflows/code_checks.yml)
-[![integration tests](https://github.com/VectorInstitute/cyclops-query/actions/workflows/integration_tests.yml/badge.svg)](https://github.com/VectorInstitute/cyclops-query/actions/workflows/integration_tests.yml)
-[![docs](https://github.com/VectorInstitute/cyclops-query/actions/workflows/docs_deploy.yml/badge.svg)](https://github.com/VectorInstitute/cyclops-query/actions/workflows/docs_deploy.yml)
-[![codecov](https://codecov.io/gh/VectorInstitute/cyclops-query/branch/main/graph/badge.svg)](https://codecov.io/gh/VectorInstitute/cyclops-query)
-[![license](https://img.shields.io/github/license/VectorInstitute/cyclops-query.svg)](https://github.com/VectorInstitute/cyclops-query/blob/main/LICENSE)
+[![code checks](https://github.com/VectorInstitute/cycquery/actions/workflows/code_checks.yml/badge.svg)](https://github.com/VectorInstitute/cycquery/actions/workflows/code_checks.yml)
+[![integration tests](https://github.com/VectorInstitute/cycquery/actions/workflows/integration_tests.yml/badge.svg)](https://github.com/VectorInstitute/cycquery/actions/workflows/integration_tests.yml)
+[![docs](https://github.com/VectorInstitute/cycquery/actions/workflows/docs_deploy.yml/badge.svg)](https://github.com/VectorInstitute/cycquery/actions/workflows/docs_deploy.yml)
+[![codecov](https://codecov.io/gh/VectorInstitute/cycquery/branch/main/graph/badge.svg)](https://codecov.io/gh/VectorInstitute/cycquery)
+[![license](https://img.shields.io/github/license/VectorInstitute/cycquery.svg)](https://github.com/VectorInstitute/cycquery/blob/main/LICENSE)
 
-``cyclops-query`` is a tool for querying relational databases using a simple Python API. It is specifically developed to query
+``cycquery`` is a tool for querying relational databases using a simple Python API. It is specifically developed to query
 Electronic Health Record (EHR) databases. The tool is a wrapper around [SQLAlchemy](https://www.sqlalchemy.org/) and can be used
 to write SQL-like queries in Python, including joins, conditions, groupby aggregation and many more.
 
 ## 🐣 Getting Started
 
-### Installing cyclops-query using pip
+### Installing cycquery using pip
 
 ```bash
 python3 -m pip install cycquery
 ```
 
 ### Query postgresql database
 
@@ -107,32 +107,14 @@
 python3 -m poetry install --with docs
 cd docs
 make html SPHINXOPTS="-D nbsphinx_allow_errors=True"
 ```
 
 ### Contributing
 
-Contributing to ``cyclops-query`` is welcomed.
-See [Contributing](https://vectorinstitute.github.io/cyclops-query/api/contributing.html) for
+Contributing to ``cycquery`` is welcomed.
+See [Contributing](https://vectorinstitute.github.io/cycquery/api/contributing.html) for
 guidelines.
 
 
-## 📚 [Documentation](https://vectorinstitute.github.io/cyclops-query/)
-
-
-## 🎓 Citation
-
-Reference to cite when you use ``cyclops-query`` in a project or a research paper:
-
-```
-@article {Krishnan2022.12.02.22283021,
-	author = {Krishnan, Amrit and Subasri, Vallijah and McKeen, Kaden and Kore, Ali and Ogidi, Franklin and Alinoori, Mahshid and Lalani, Nadim and Dhalla, Azra and Verma, Amol and Razak, Fahad and Pandya, Deval and Dolatabadi, Elham},
-	title = {CyclOps: Cyclical development towards operationalizing ML models for health},
-	elocation-id = {2022.12.02.22283021},
-	year = {2022},
-	doi = {10.1101/2022.12.02.22283021},
-	publisher = {Cold Spring Harbor Laboratory Press},
-	URL = {https://www.medrxiv.org/content/early/2022/12/08/2022.12.02.22283021},
-	journal = {medRxiv}
-}
-```
+## 📚 [Documentation](https://vectorinstitute.github.io/cycquery/)
```

