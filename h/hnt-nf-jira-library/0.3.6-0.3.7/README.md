# Comparing `tmp/hnt_nf_jira_library-0.3.6.tar.gz` & `tmp/hnt_nf_jira_library-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.3.6.tar", last modified: Wed Apr 17 20:36:59 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.3.7.tar", last modified: Thu Apr 18 12:42:07 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.3.6.tar` & `hnt_nf_jira_library-0.3.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.120420 hnt_nf_jira_library-0.3.6/
--rw-rw-rw-   0        0        0      286 2024-04-17 20:36:59.117424 hnt_nf_jira_library-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.115162 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.052539 hnt_nf_jira_library-0.3.6/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.6/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.099283 hnt_nf_jira_library-0.3.6/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.112404 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-15 12:56:23.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     4200 2024-04-17 19:50:51.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     5454 2024-04-15 14:35:02.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     3250 2024-04-17 17:10:21.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      234 2024-04-15 13:00:20.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      448 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      354 2024-04-15 13:00:14.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    14826 2024-04-17 17:51:01.000000 hnt_nf_jira_library-0.3.6/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-17 20:36:59.120420 hnt_nf_jira_library-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-17 20:35:51.000000 hnt_nf_jira_library-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:42:07.812063 hnt_nf_jira_library-0.3.7/
+-rw-rw-rw-   0        0        0      286 2024-04-18 12:42:07.810064 hnt_nf_jira_library-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 12:42:07.805941 hnt_nf_jira_library-0.3.7/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-18 12:42:07.000000 hnt_nf_jira_library-0.3.7/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2024-04-18 12:42:07.000000 hnt_nf_jira_library-0.3.7/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 12:42:07.000000 hnt_nf_jira_library-0.3.7/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-18 12:42:07.000000 hnt_nf_jira_library-0.3.7/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 12:42:07.000000 hnt_nf_jira_library-0.3.7/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 12:42:07.569586 hnt_nf_jira_library-0.3.7/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.7/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:42:07.750919 hnt_nf_jira_library-0.3.7/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:42:07.800991 hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4893 2024-04-15 12:56:23.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     4284 2024-04-18 12:40:33.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     5454 2024-04-15 14:35:02.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     3354 2024-04-18 12:41:15.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      234 2024-04-15 13:00:20.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      448 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      354 2024-04-15 13:00:14.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.7/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    14826 2024-04-17 17:51:01.000000 hnt_nf_jira_library-0.3.7/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 12:42:07.813063 hnt_nf_jira_library-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-18 12:41:49.000000 hnt_nf_jira_library-0.3.7/setup.py
```

### Comparing `hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.3.7/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,9 +95,10 @@
         def _check_fatura_form(self, form_data):
             if 'nro_fatura' not in form_data: raise KeyError(f"ERRO - O Campo {'nro_fatura'} não foi enviado.")
             if form_data['nro_fatura'] is None or form_data['nro_fatura'] == "": raise KeyError(f"ERRO - O Campo {'nro_fatura'} está vazio.")
             pass
 
         def _check_required_form(self, form_data):
             for field in form_data:
-                if form_data[field] is None or form_data[field] == "":raise KeyError(f"ERRO - O Campo {field} está vazio")
+                if field not in OPTIONAL_FIELDS and field not in SEFAZ_FIELDS:
+                    if form_data[field] is None or form_data[field] == "":raise KeyError(f"ERRO - O Campo {field} está vazio")
             pass
```

### Comparing `hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.3.7/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.6/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.3.7/nf_jira/entities/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 # Constants Jira
 JIRA_AUTH = (os.getenv("USER"), os.getenv("ACCESS_TOKEN"))
 API_ISSUE_URL = os.getenv("ISSUE_URL")
 API_FORM_URL = os.getenv("FORM_URL")
 CLOUD_ID = os.getenv("CLOUD_ID")
 
 #Constantes de Validação
+OPTIONAL_FIELDS = [
+    "nro_fatura",
+    "nro_nota_fiscal",
+    "valor_liquido",
+    "juros"
+]
+
 SEFAZ_FIELDS = [
     "data_autorizacao",
     "hora_autorizacao",
     "protocolo_autorizacao",
     "chave_acesso"
 ]
```

### Comparing `hnt_nf_jira_library-0.3.6/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.3.7/nf_jira/wrapper_nf_jira.py`

 * *Files identical despite different names*

