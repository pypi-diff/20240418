# Comparing `tmp/nsj_sql_utils_lib-1.1.3.tar.gz` & `tmp/nsj_sql_utils_lib-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_sql_utils_lib-1.1.3.tar", last modified: Wed Mar 27 19:49:39 2024, max compression
+gzip compressed data, was "nsj_sql_utils_lib-1.1.4.tar", last modified: Thu Apr 18 17:45:24 2024, max compression
```

## Comparing `nsj_sql_utils_lib-1.1.3.tar` & `nsj_sql_utils_lib-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2024-03-27 19:49:39.203519 nsj_sql_utils_lib-1.1.3/
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)     5094 2024-03-27 19:49:39.203519 nsj_sql_utils_lib-1.1.3/PKG-INFO
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)     4368 2024-03-14 17:04:52.000000 nsj_sql_utils_lib-1.1.3/README.md
-drwxr-xr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2024-03-27 19:49:39.203519 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2024-03-14 17:04:52.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/__init__.py
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)      925 2024-03-14 17:04:52.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/dao_util.py
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)     6130 2024-03-14 17:04:52.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/dbadapter3.py
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)      869 2024-03-14 17:04:52.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/dbconection_psycopg2.py
-drwxr-xr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2024-03-27 19:49:39.203519 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/updater/
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2024-03-14 17:04:52.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/updater/__init__.py
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)     1040 2024-03-19 18:52:49.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/updater/create_script.py
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)     1809 2024-03-14 17:04:52.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/updater/db_updater.py
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)     9738 2024-03-27 19:46:32.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/updater/erp_database_updater.py
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)      341 2024-03-14 17:04:52.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/updater/vars.py
-drwxr-xr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2024-03-27 19:49:39.203519 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib.egg-info/
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)     5094 2024-03-27 19:49:39.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib.egg-info/PKG-INFO
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)      605 2024-03-27 19:49:39.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib.egg-info/SOURCES.txt
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)        1 2024-03-27 19:49:39.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib.egg-info/dependency_links.txt
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)       59 2024-03-27 19:49:39.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib.egg-info/requires.txt
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)       18 2024-03-27 19:49:39.000000 nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib.egg-info/top_level.txt
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)      103 2024-03-14 17:04:52.000000 nsj_sql_utils_lib-1.1.3/pyproject.toml
--rw-r--r--   0 wallacepinho  (1000) wallacepinho  (1000)      837 2024-03-27 19:49:39.203519 nsj_sql_utils_lib-1.1.3/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4366 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.1.4/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:45:24.308136 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-22 21:56:47.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      925 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dao_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6246 2024-04-18 17:44:35.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dbadapter3.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      869 2023-07-22 22:02:23.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dbconection_psycopg2.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1040 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/create_script.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1809 2024-01-12 20:44:34.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/db_updater.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9738 2024-04-18 17:44:27.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/erp_database_updater.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      341 2024-01-02 22:09:17.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/vars.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     5091 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      605 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       59 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       18 2024-04-18 17:45:24.000000 nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-22 22:03:17.000000 nsj_sql_utils_lib-1.1.4/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      837 2024-04-18 17:45:24.312136 nsj_sql_utils_lib-1.1.4/setup.cfg
```

### Comparing `nsj_sql_utils_lib-1.1.3/PKG-INFO` & `nsj_sql_utils_lib-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_sql_utils_lib
-Version: 1.1.3
+Version: 1.1.4
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,16 @@
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Requires-Dist: psycopg2_binary>=2.9.6
 Requires-Dist: SQLAlchemy>=1.4.32
 Requires-Dist: sqlparams>=3.0.0
 
 # nsj-sql-utils-lib
-    Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
+
+Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
         
 ## Principais utilitários:
     
 * **dao_util:** Módulo com utilitátios para implementação de classes DAO (exemplo: facilitar a criação da lista de fileds de um select, ou fields e values de um insert).
     * **dbadapter3:** Classe adapter para utilizar conexões de banco de dados (útil para conexões psycopg2).
     * **dbconection_psycopg2:** Classe para abertura de conexão com postgres, utilizando o drive psycopg2 (sem pool de conexões, nem uso do SQL Alchemy).
     * **db-updater:** Modulo para atualização de bancos pensado para ser em um formato parecido com o erp-3
```

### Comparing `nsj_sql_utils_lib-1.1.3/README.md` & `nsj_sql_utils_lib-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # nsj-sql-utils-lib
-    Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
+
+Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
         
 ## Principais utilitários:
     
 * **dao_util:** Módulo com utilitátios para implementação de classes DAO (exemplo: facilitar a criação da lista de fileds de um select, ou fields e values de um insert).
     * **dbadapter3:** Classe adapter para utilizar conexões de banco de dados (útil para conexões psycopg2).
     * **dbconection_psycopg2:** Classe para abertura de conexão com postgres, utilizando o drive psycopg2 (sem pool de conexões, nem uso do SQL Alchemy).
     * **db-updater:** Modulo para atualização de bancos pensado para ser em um formato parecido com o erp-3 
@@ -72,8 +73,8 @@
      |--scriptspath   SCRIPTSPATH  |'./database/scripts/' | Caminho da pasta de scripts  
 
  > python -m nsj_sql_utils_lib.updater.create_script[-h] [--filename FILENAME] [--scriptspath SCRIPTSPATH]
  
  
  
  * Pode ser usado a forma como imagem docker:
- *   > docker run -v "$PWD/database:/src/database" db-updater python -m nsj_sql_utils_lib.updater.create_script [-h] [--filename FILENAME] [--scriptspath SCRIPTSPATH]
+ *   > docker run -v "$PWD/database:/src/database" db-updater python -m nsj_sql_utils_lib.updater.create_script [-h] [--filename FILENAME] [--scriptspath SCRIPTSPATH]
```

### Comparing `nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/dao_util.py` & `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dao_util.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/dbadapter3.py` & `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dbadapter3.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
                 lista.append(obj)
                 item = cur.fetchone()
 
             return (cur.rowcount, lista)
         else:
             return (cur.rowcount, [])
-        
-    def simple_execute(self, sql): 
+
+    def simple_execute(self, sql):
         # Verificando se a query está no padrão do DBAdapter2
         if self.adapter2_matcher.match(sql.replace("\n", " ####### ")):
             sql = self._ajustar_query_adapter2_to3(sql)
 
         with self.conn.cursor() as cur:
             cur.execute(sql)
 
@@ -78,15 +78,19 @@
 
         Os parâmetros do comando sql devem ser passados com a sintaxe %(nome)s, no SQL,
         e seus valores devem ser passados como kwargs.
         """
 
         if not isinstance(self.conn, AlchemyConnection):
             # Verificando se a query está no padrão do DBAdapter2
-            if self.adapter2_matcher.match(sql.replace("\n", " ####### ")):
+            if self.adapter2_matcher.match(
+                sql.replace("\n", " ####### ")
+                .replace("http:", " ###2### ")
+                .replace("https:", " ###3### ")
+            ):
                 sql = self._ajustar_query_adapter2_to3(sql)
 
             with self.conn.cursor() as cur:
                 cur.execute(sql, kwargs)
 
                 return self._handle_result(cur)
         else:
```

### Comparing `nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/dbconection_psycopg2.py` & `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/dbconection_psycopg2.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/updater/create_script.py` & `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/create_script.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/updater/db_updater.py` & `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/db_updater.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib/updater/erp_database_updater.py` & `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib/updater/erp_database_updater.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib.egg-info/PKG-INFO` & `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_sql_utils_lib
-Version: 1.1.3
+Version: 1.1.4
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,16 @@
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Requires-Dist: psycopg2_binary>=2.9.6
 Requires-Dist: SQLAlchemy>=1.4.32
 Requires-Dist: sqlparams>=3.0.0
 
 # nsj-sql-utils-lib
-    Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
+
+Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
         
 ## Principais utilitários:
     
 * **dao_util:** Módulo com utilitátios para implementação de classes DAO (exemplo: facilitar a criação da lista de fileds de um select, ou fields e values de um insert).
     * **dbadapter3:** Classe adapter para utilizar conexões de banco de dados (útil para conexões psycopg2).
     * **dbconection_psycopg2:** Classe para abertura de conexão com postgres, utilizando o drive psycopg2 (sem pool de conexões, nem uso do SQL Alchemy).
     * **db-updater:** Modulo para atualização de bancos pensado para ser em um formato parecido com o erp-3
```

### Comparing `nsj_sql_utils_lib-1.1.3/nsj_sql_utils_lib.egg-info/SOURCES.txt` & `nsj_sql_utils_lib-1.1.4/nsj_sql_utils_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-1.1.3/setup.cfg` & `nsj_sql_utils_lib-1.1.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_sql_utils_lib
-version = 1.1.3
+version = 1.1.4
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-sql-utils-lib
 project_urls =
```

