# Comparing `tmp/hnt_nf_jira_library-0.3.5.tar.gz` & `tmp/hnt_nf_jira_library-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.3.5.tar", last modified: Mon Apr 15 18:56:06 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.3.6.tar", last modified: Wed Apr 17 20:36:59 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.3.5.tar` & `hnt_nf_jira_library-0.3.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 18:56:06.467845 hnt_nf_jira_library-0.3.5/
--rw-rw-rw-   0        0        0      286 2024-04-15 18:56:06.463844 hnt_nf_jira_library-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 18:56:06.459845 hnt_nf_jira_library-0.3.5/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-15 18:56:06.000000 hnt_nf_jira_library-0.3.5/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2024-04-15 18:56:06.000000 hnt_nf_jira_library-0.3.5/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 18:56:06.000000 hnt_nf_jira_library-0.3.5/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-15 18:56:06.000000 hnt_nf_jira_library-0.3.5/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 18:56:06.000000 hnt_nf_jira_library-0.3.5/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 18:56:06.384063 hnt_nf_jira_library-0.3.5/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.5/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:56:06.437842 hnt_nf_jira_library-0.3.5/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:56:06.455844 hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4893 2024-04-15 12:56:23.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     2162 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     5454 2024-04-15 14:35:02.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     2956 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      234 2024-04-15 13:00:20.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      448 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      354 2024-04-15 13:00:14.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.5/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    14540 2024-04-15 18:46:38.000000 hnt_nf_jira_library-0.3.5/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-15 18:56:06.468847 hnt_nf_jira_library-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-15 18:55:10.000000 hnt_nf_jira_library-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.120420 hnt_nf_jira_library-0.3.6/
+-rw-rw-rw-   0        0        0      286 2024-04-17 20:36:59.117424 hnt_nf_jira_library-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.115162 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 20:36:58.000000 hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.052539 hnt_nf_jira_library-0.3.6/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.6/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.099283 hnt_nf_jira_library-0.3.6/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:36:59.112404 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4893 2024-04-15 12:56:23.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     4200 2024-04-17 19:50:51.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     5454 2024-04-15 14:35:02.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     3250 2024-04-17 17:10:21.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      234 2024-04-15 13:00:20.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      448 2024-04-15 12:56:24.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      354 2024-04-15 13:00:14.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-04-13 16:16:55.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.6/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    14826 2024-04-17 17:51:01.000000 hnt_nf_jira_library-0.3.6/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-17 20:36:59.120420 hnt_nf_jira_library-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-17 20:35:51.000000 hnt_nf_jira_library-0.3.6/setup.py
```

### Comparing `hnt_nf_jira_library-0.3.5/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.3.6/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.5/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_library-0.3.6/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.3.5/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.3.6/nf_jira/entities/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,30 @@
 
 # Constants Jira
 JIRA_AUTH = (os.getenv("USER"), os.getenv("ACCESS_TOKEN"))
 API_ISSUE_URL = os.getenv("ISSUE_URL")
 API_FORM_URL = os.getenv("FORM_URL")
 CLOUD_ID = os.getenv("CLOUD_ID")
 
+#Constantes de Validação
+SEFAZ_FIELDS = [
+    "data_autorizacao",
+    "hora_autorizacao",
+    "protocolo_autorizacao",
+    "chave_acesso"
+]
+
+FISCAL_FIELDS = [
+    "InvoiceNumber"
+]
+
+FATURA_FIELDS = [
+    "SupplierInvoiceNumber"
+]
+
 API_HEADERS = {
                 "Accept": "application/json",
                 "Content-Type": "application/json",
               }
 API_ATTACHMENT_HEADERS = {
                             "Accept": "*/*",
                          }
@@ -74,8 +90,9 @@
 SERVIÇOS_DA_FATURA = "InvoiceServices"
 IMPOSTOS = "Taxes"
 CAMPOS_CUSTOMIZADOS = "CustomFields"
 ALOCAÇÕES_DE_CUSTO = "CostAllocations"
 ARQUIVOS_DA_FATURA = "InvoiceFiles"
 COMPLEMENTO_DE_ÁGUA = "WaterComplement"
 COMPLEMENTO_DE_ENERGIA = "EnergyComplement"
-COMPLEMENTO_DE_GÁS = "GasComplement"
+COMPLEMENTO_DE_GÁS = "GasComplement"
+POSSUI_CHAVE_ACESSO = "possui_chave_acesso"
```

### Comparing `hnt_nf_jira_library-0.3.5/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.3.6/nf_jira/wrapper_nf_jira.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
         return fatura_model
 
     def _get_nf_jira(self, issue_id):
         try:
 
             issue_data = self.IssueJira.get_issue(issue_id)
             complement_form = self._get_issue_fields_by_keys( issue_id, FORM_TEMPLATE_COMPLEMENTO )
+            self.GuiandoHelper.check_guiando_form(complement_form)
 
             issue_data["fields"] = self.JiraFieldsHelper.remove_null_fields(issue_data.get("fields"))
             attachment = self.AttachmentJira.get_attachment(issue_data)
 
             nf_type_id = complement_form["tipo_conta"]
 
             if nf_type_id == "ÁGUA":
@@ -287,16 +288,20 @@
             attachment[DATA_DE_EMISSÃO] = complement_form['data_emissao']
             attachment[DATA_DE_VENCIMENTO] = complement_form['data_vencimento']
             attachment[CHAVE_DE_ACESSO_DA_FATURA] = complement_form['chave_acesso']
             attachment[DATA_DE_REFERÊNCIA] = complement_form['periodo_referencia']
             attachment["numero_log"] = complement_form['protocolo_autorizacao']
             attachment["data_procmto"] = complement_form['data_autorizacao']
             attachment["hora_procmto"] = complement_form['hora_autorizacao']
-            attachment[nf_type]["DataLeituraAnterior"] = complement_form['data_leitura_anterior']
-            attachment[nf_type]["DataLeituraAtual"] = complement_form['data_leitura_atual']
+            attachment[nf_type] = {
+                "DataLeituraAnterior" : complement_form['data_leitura_anterior'],
+                "DataLeituraAtual"    : complement_form['data_leitura_atual']
+            }
+            # attachment[nf_type]["DataLeituraAnterior"] = complement_form['data_leitura_anterior']
+            # attachment[nf_type]["DataLeituraAtual"] = complement_form['data_leitura_atual']
             attachment["grupo_compradores"] = complement_form['grupo_compradores']
 
             #Validação de Valor Liquido da Fatura
             if complement_form['valor_liquido'] != "" and complement_form['valor_liquido'] != None:
                 attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_liquido']
             elif complement_form['valor_nota'] != None and complement_form['valor_nota'] != "":
                 attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_nota']
```

