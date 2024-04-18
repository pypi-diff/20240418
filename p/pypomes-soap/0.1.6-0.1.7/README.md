# Comparing `tmp/pypomes_soap-0.1.6.tar.gz` & `tmp/pypomes_soap-0.1.7.tar.gz`

## Comparing `pypomes_soap-0.1.6.tar` & `pypomes_soap-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pypomes_soap-0.1.6/src/pypomes_soap/__init__.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 pypomes_soap-0.1.6/src/pypomes_soap/soap_pomes.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_soap-0.1.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_soap-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_soap-0.1.6/README.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pypomes_soap-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pypomes_soap-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/src/pypomes_soap/__init__.py
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/src/pypomes_soap/soap_pomes.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/README.md
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pypomes_soap-0.1.7/PKG-INFO
```

### Comparing `pypomes_soap-0.1.6/src/pypomes_soap/soap_pomes.py` & `pypomes_soap-0.1.7/src/pypomes_soap/soap_pomes.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,49 +4,55 @@
 from lxml import etree
 from pathlib import Path
 from pypomes_core import json_normalize_dict, xml_to_dict
 from pypomes_http import HTTP_POST_TIMEOUT
 from zeep import Client
 
 
-def soap_build_envelope(ws_url: str, service: str, payload: dict, file_path: Path = None) -> bytes:
+def soap_build_envelope(ws_url: str,
+                        service: str,
+                        payload: dict,
+                        filepath: Path = None) -> bytes:
     """
     Constrói e retorna o envelope SOAP para um dado serviço. Esse envelope não contem os *headers*.
 
     :param ws_url: a URL da solicitação
     :param payload: os dados a serem enviados
     :param service: o nome do serviço
-    :param file_path: Path to store the soap envelope.
+    :param filepath: Path to store the soap envelope.
     :return: o envelope para a requisição SOAP, sem os headers
     """
     # obtem o cliente
     zeep_client: Client = Client(wsdl=ws_url)
     # obtem o envelope XML
     root = zeep_client.create_message(zeep_client.service, service, **payload)
     result: bytes = etree.tostring(element_or_tree=root,
                                    pretty_print=True)
 
     # salva o envelope em arquivo ?
-    if file_path:
+    if filepath:
         # sim
-        with Path.open(file_path, "wb") as f:
+        with filepath.open("wb") as f:
             f.write(result)
 
     return result
 
 
-def soap_post(ws_url: str, soap_envelope: bytes, extra_headers: dict = None,
-              file_path: Path = None, timeout: int = HTTP_POST_TIMEOUT) -> bytes:
+def soap_post(ws_url: str,
+              soap_envelope: bytes,
+              extra_headers: dict = None,
+              filepath: Path = None,
+              timeout: int | None = HTTP_POST_TIMEOUT) -> bytes:
     """
     Encaminha a solicitação SOAP, e retorna a resposta recebida.
 
     :param ws_url: a URL da solicitação
     :param soap_envelope: o envelope SOAP
     :param extra_headers: cabeçalho adicional
-    :param file_path: Path to store the response to the request.
+    :param filepath: Path to store the response to the request.
     :param timeout: timeout, in seconds (defaults to HTTP_POST_TIMEOUT - use None to omit)
     :return: a resposta à solicitação
     """
     # constrói o cabeçalho do envelope SOAP
     headers: dict = {"SOAPAction": '""',
                      "content-type": "application/soap+xml; charset=utf-8"}
 
@@ -59,49 +65,53 @@
     response: requests.Response = requests.post(url=ws_url,
                                                 data=soap_envelope,
                                                 headers=headers,
                                                 timeout=timeout)
     result: bytes = response.content
 
     # salva o response em arquivo ?
-    if file_path:
+    if filepath:
         # sim
-        with Path.open(file_path, "wb") as f:
+        with filepath.open("wb") as f:
             f.write(result)
 
     return result
 
 
-def soap_post_zeep(zeep_service: callable, payload: dict, file_path: Path = None) -> dict:
+def soap_post_zeep(zeep_service: callable,
+                   payload: dict,
+                   filepath: Path = None) -> dict:
     """
     Encaminha a solicitação SOAP utilizando o pacote *zeep*, e retorna a resposta recebida.
 
     :param zeep_service: o serviço de referência
     :param payload: os dados a serem enviados
-    :param file_path: Path to store the JSON corresponding to the returned response.
+    :param filepath: Path to store the JSON corresponding to the returned response.
     :return: a resposta à solicitação
     """
     # invoca o servico
     # ('response' é uma subclasse de dict - definida como retorno do 'zeep_service' no wsdl)
     response: any = zeep_service(**payload)
 
     # converte o conteúdo retornado em dict e o prepara para descarga em JSON
     result: dict = ast.literal_eval(str(response))
     json_normalize_dict(result)
 
     # salva o retorno em arquivo ?
-    if file_path:
+    if filepath:
         # sim
-        with Path.open(file_path, "w") as f:
+        with filepath.open("w") as f:
             f.write(json.dumps(result, ensure_ascii=False))
 
     return result
 
 
-def soap_get_dict(soap_response: bytes, xml_path: Path = None, json_path: Path = None) -> dict:
+def soap_get_dict(soap_response: bytes,
+                  xml_path: Path = None,
+                  json_path: Path = None) -> dict:
     """
     Recupera o objeto *dict* contendo os dados retornados pela solicitação SOAP.
 
     Esse objeto é retornado em condições de ser descarregado em formato JSON.
 
     :param soap_response: o conteúdo retornado pela solicitação SOAP
     :param xml_path: Path to store the XML correspondinge to the returned response.
@@ -112,25 +122,25 @@
     pos_1: int = soap_response.find(b"<soap:Body>") + 11
     pos_2: int = soap_response.find(b"</soap:Body>", pos_1)
     content: bytes = soap_response[pos_1:pos_2]
 
     # salva o conteúdo XML retornado em arquivo ?
     if xml_path:
         # sim
-        with Path.open(xml_path, "wb") as f:
+        with xml_path.open("wb") as f:
             f.write(content)
 
     # converte o conteúdo XML em dict e o prepara para descarga em JSON
     result: dict = xml_to_dict(content)
     json_normalize_dict(result)
 
     # salva o retorno em arquivo ?
     if json_path:
         # sim
-        with Path.open(json_path, "w") as f:
+        with json_path.open("w") as f:
             f.write(json.dumps(result, ensure_ascii=False))
 
     return result
 
 
 def soap_get_cids(soap_response: bytes) -> list[bytes]:
     """
@@ -160,23 +170,25 @@
         pos_2: int = soap_response.find(b'"', pos_1)
         result.append(soap_response[pos_1:pos_2])
         pos_1 = soap_response.find(prefix, pos_1)
 
     return result
 
 
-def soap_get_attachment(soap_response: bytes, cid: bytes, file_path: Path = None) -> bytes:
+def soap_get_attachment(soap_response: bytes,
+                        cid: bytes,
+                        filepath: Path = None) -> bytes:
     """
     Obtem e retorna o anexo contido no *response* da solicitação *SOAP*, no padrão *MTOM*.
 
     Nesse padrão (*Message Transmission Optimization Mechanism*), o anexo é identificado pelo *cid* (Content-ID).
 
     :param soap_response: o conteúdo retornado pela solicitação SOAP
     :param cid: a identificação do anexo
-    :param file_path: Path to store the JSON corresponding to the returned attachment.
+    :param filepath: Path to store the JSON corresponding to the returned attachment.
     :return: o anexo em referência, ou None se não for encontrado
     """
     # inicializa a variável de retorno
     result: bytes | None = None
 
     # localiza o início do anexo
     mark: bytes = b"Content-ID: <" + cid + b">"
@@ -199,13 +211,13 @@
         # localiza o final do anexo
         pos_2 = soap_response.find(separator, pos_1)
 
         # obtem o anexo
         result: bytes = soap_response[pos_1:pos_2]
 
         # salva o attachment em arquivo ?
-        if file_path:
+        if filepath:
             # sim
-            with Path.open(file_path, "wb") as f:
+            with filepath.open("wb") as f:
                 f.write(result)
 
     return result
```

### Comparing `pypomes_soap-0.1.6/LICENSE` & `pypomes_soap-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_soap-0.1.6/pyproject.toml` & `pypomes_soap-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [build-system]
 requires = [
-    "hatchling"
+    "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_soap"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (SOAP module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "lxml>=4.9.3",
     "pip>=24.0",
-    "pypomes_core>=0.6.8",
-    "pypomes_http>=0.0.6",
+    "pypomes_core>=0.8.7",
+    "pypomes_http>=0.1.3",
     "requests>=2.31.0",
     "setuptools>=68.0.0",
     "wheel>=0.42.0",
     "zeep>=4.2.1"
 ]
 
 [project.urls]
```

### Comparing `pypomes_soap-0.1.6/PKG-INFO` & `pypomes_soap-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pypomes_soap
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of Python pomes, pennyeach (SOAP module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-SOAP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-SOAP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: lxml>=4.9.3
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.6.8
-Requires-Dist: pypomes-http>=0.0.6
+Requires-Dist: pypomes-core>=0.8.7
+Requires-Dist: pypomes-http>=0.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
 Requires-Dist: zeep>=4.2.1
```

