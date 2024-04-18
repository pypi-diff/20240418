# Comparing `tmp/nsj_sql_utils_lib-1.1.4.tar.gz` & `tmp/nsj_sql_utils_lib-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_sql_utils_lib-1.1.4.tar", last modified: Thu Apr 18 17:45:24 2024, max compression
+gzip compressed data, was "nsj_sql_utils_lib-1.1.5.tar", last modified: Thu Apr 18 17:51:27 2024, max compression
```

## Comparing `nsj_sql_utils_lib-1.1.4.tar` & `nsj_sql_utils_lib-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4366 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.1.4/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:45:24.308136 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-22 21:56:47.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      925 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dao_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     6246 2024-04-18 17:44:35.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dbadapter3.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      869 2023-07-22 22:02:23.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dbconection_psycopg2.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1040 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/create_script.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1809 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/db_updater.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9738 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/erp_database_updater.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      341 2024-01-02 22:09:17.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/vars.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      605 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       59 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       18 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-22 22:03:17.000000 nsj_sql_utils_lib-1.1.4/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      837 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:51:27.827620 nsj_sql_utils_lib-1.1.5/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-18 17:51:27.827620 nsj_sql_utils_lib-1.1.5/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4366 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.1.5/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:51:27.827620 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-22 21:56:47.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      925 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/dao_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6535 2024-04-18 17:51:13.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/dbadapter3.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      869 2023-07-22 22:02:23.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/dbconection_psycopg2.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:51:27.827620 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/updater/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/updater/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1040 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/updater/create_script.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1809 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/updater/db_updater.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9738 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/updater/erp_database_updater.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      341 2024-01-02 22:09:17.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/updater/vars.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:51:27.827620 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib.egg-info/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-18 17:51:27.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      605 2024-04-18 17:51:27.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-18 17:51:27.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       59 2024-04-18 17:51:27.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       18 2024-04-18 17:51:27.000000 nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-22 22:03:17.000000 nsj_sql_utils_lib-1.1.5/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      837 2024-04-18 17:51:27.827620 nsj_sql_utils_lib-1.1.5/setup.cfg
```

### Comparing `nsj_sql_utils_lib-1.1.4/PKG-INFO` & `nsj_sql_utils_lib-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_sql_utils_lib
-Version: 1.1.4
+Version: 1.1.5
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_sql_utils_lib-1.1.4/README.md` & `nsj_sql_utils_lib-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dao_util.py` & `nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/dao_util.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dbadapter3.py` & `nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/dbadapter3.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Obs.: Esse adapter é simplificado, com relação ao DBAdapter2 e o DBAdapter, mas,
     contém função para execução de instruções SQL multivaloradas.
     """
 
     def __init__(self, conn):
         self.conn = conn
         self._transaction = None
-        self.adapter2_matcher = re.compile(r".*:([^ ]+)")
+        self.adapter2_matcher = re.compile(r".*:([^ \"]+)")
 
     def begin(self):
         if self._transaction is None:
             self.execute("begin")
             self._transaction = True
 
     def commit(self):
@@ -56,15 +56,19 @@
 
             return (cur.rowcount, lista)
         else:
             return (cur.rowcount, [])
 
     def simple_execute(self, sql):
         # Verificando se a query está no padrão do DBAdapter2
-        if self.adapter2_matcher.match(sql.replace("\n", " ####### ")):
+        if self.adapter2_matcher.match(
+            sql.replace("\n", " ####### ")
+            .replace("http:", "###2###")
+            .replace("https:", "###3###")
+        ):
             sql = self._ajustar_query_adapter2_to3(sql)
 
         with self.conn.cursor() as cur:
             cur.execute(sql)
 
             return self._handle_result(cur)
 
@@ -80,16 +84,16 @@
         e seus valores devem ser passados como kwargs.
         """
 
         if not isinstance(self.conn, AlchemyConnection):
             # Verificando se a query está no padrão do DBAdapter2
             if self.adapter2_matcher.match(
                 sql.replace("\n", " ####### ")
-                .replace("http:", " ###2### ")
-                .replace("https:", " ###3### ")
+                .replace("http:", "###2###")
+                .replace("https:", "###3###")
             ):
                 sql = self._ajustar_query_adapter2_to3(sql)
 
             with self.conn.cursor() as cur:
                 cur.execute(sql, kwargs)
 
                 return self._handle_result(cur)
@@ -141,15 +145,19 @@
             return self._handle_result(cur)
 
     def _ajustar_query_sqlalchemy(self, sql: str, pars: dict[str, any]):
         sql = re.sub(r"%\(([^\(\)]+)\)s", r":\1", sql)
         return SQLParams("named", "format").format(sql, pars)
 
     def _ajustar_query_adapter2_to3(self, sql: str):
+        sql = sql.replace("http:", "###2###")
+        sql = sql.replace("https:", "###3###")
         sql = re.sub(r":([^ \n,\)]+)", r"%(\1)s", sql)
+        sql = sql.replace("###2###", "http:")
+        sql = sql.replace("###3###", "https:")
         return sql
 
     def execute_query_to_model(self, sql: str, model_class: object, **kwargs) -> list:
         """
         Executando uma instrução sql com retorno.
 
         O retorno é feito em forma de uma lista (list), com elementos do tipo passado pelo parâmetro
```

### Comparing `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dbconection_psycopg2.py` & `nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/dbconection_psycopg2.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/create_script.py` & `nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/updater/create_script.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/db_updater.py` & `nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/updater/db_updater.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/erp_database_updater.py` & `nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib/updater/erp_database_updater.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/PKG-INFO` & `nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_sql_utils_lib
-Version: 1.1.4
+Version: 1.1.5
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/SOURCES.txt` & `nsj_sql_utils_lib-1.1.5/nsj_sql_utils_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.4/setup.cfg` & `nsj_sql_utils_lib-1.1.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_sql_utils_lib
-version = 1.1.4
+version = 1.1.5
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-sql-utils-lib
 project_urls =
```

