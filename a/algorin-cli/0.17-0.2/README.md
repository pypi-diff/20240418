# Comparing `tmp/algorin_cli-0.17.tar.gz` & `tmp/algorin-cli-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algorin_cli-0.17.tar", last modified: Thu Apr 18 01:21:21 2024, max compression
+gzip compressed data, was "algorin-cli-0.2.tar", last modified: Wed Apr 17 21:55:16 2024, max compression
```

## Comparing `algorin_cli-0.17.tar` & `algorin-cli-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-18 01:21:21.970917 algorin_cli-0.17/
--rw-r--r--   0 1064331    (502) staff       (20)     7652 2024-04-18 01:21:21.969893 algorin_cli-0.17/PKG-INFO
--rw-r--r--   0 1064331    (502) staff       (20)       33 2024-04-17 19:58:47.000000 algorin_cli-0.17/README.md
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-18 01:21:21.940833 algorin_cli-0.17/algorin/
--rw-r--r--   0 1064331    (502) staff       (20)      473 2024-04-17 22:08:13.000000 algorin_cli-0.17/algorin/__init__.py
--rw-r--r--   0 1064331    (502) staff       (20)     1284 2024-04-18 01:06:50.000000 algorin_cli-0.17/algorin/chatbot.py
--rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 22:04:49.000000 algorin_cli-0.17/algorin/file_extractor.py
--rw-r--r--   0 1064331    (502) staff       (20)     2230 2024-04-18 01:20:13.000000 algorin_cli-0.17/algorin/main.py
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-18 01:21:21.961165 algorin_cli-0.17/algorin_cli.egg-info/
--rw-r--r--   0 1064331    (502) staff       (20)     7652 2024-04-18 01:21:21.000000 algorin_cli-0.17/algorin_cli.egg-info/PKG-INFO
--rw-r--r--   0 1064331    (502) staff       (20)      399 2024-04-18 01:21:21.000000 algorin_cli-0.17/algorin_cli.egg-info/SOURCES.txt
--rw-r--r--   0 1064331    (502) staff       (20)        1 2024-04-18 01:21:21.000000 algorin_cli-0.17/algorin_cli.egg-info/dependency_links.txt
--rw-r--r--   0 1064331    (502) staff       (20)       55 2024-04-18 01:21:21.000000 algorin_cli-0.17/algorin_cli.egg-info/entry_points.txt
--rw-r--r--   0 1064331    (502) staff       (20)     3831 2024-04-18 01:21:21.000000 algorin_cli-0.17/algorin_cli.egg-info/requires.txt
--rw-r--r--   0 1064331    (502) staff       (20)       14 2024-04-18 01:21:21.000000 algorin_cli-0.17/algorin_cli.egg-info/top_level.txt
--rw-r--r--   0 1064331    (502) staff       (20)       38 2024-04-18 01:21:21.971019 algorin_cli-0.17/setup.cfg
--rw-r--r--   0 1064331    (502) staff       (20)      879 2024-04-18 01:21:13.000000 algorin_cli-0.17/setup.py
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-18 01:21:21.952640 algorin_cli-0.17/tests/
--rw-r--r--   0 1064331    (502) staff       (20)      178 2024-04-17 20:21:38.000000 algorin_cli-0.17/tests/__init__.py
--rw-r--r--   0 1064331    (502) staff       (20)      546 2024-04-17 20:22:40.000000 algorin_cli-0.17/tests/test_chatbot.py
--rw-r--r--   0 1064331    (502) staff       (20)      769 2024-04-17 20:22:47.000000 algorin_cli-0.17/tests/test_file_extractor.py
--rw-r--r--   0 1064331    (502) staff       (20)      631 2024-04-17 20:22:52.000000 algorin_cli-0.17/tests/test_main.py
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:55:16.686299 algorin-cli-0.2/
+-rw-r--r--   0 1064331    (502) staff       (20)     7651 2024-04-17 21:55:16.684052 algorin-cli-0.2/PKG-INFO
+-rw-r--r--   0 1064331    (502) staff       (20)       33 2024-04-17 19:58:47.000000 algorin-cli-0.2/README.md
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:55:16.662564 algorin-cli-0.2/algorin-cli/
+-rw-r--r--   0 1064331    (502) staff       (20)      425 2024-04-17 20:22:58.000000 algorin-cli-0.2/algorin-cli/__init__.py
+-rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:07.000000 algorin-cli-0.2/algorin-cli/chatbot.py
+-rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 18:41:17.000000 algorin-cli-0.2/algorin-cli/file_extractor.py
+-rw-r--r--   0 1064331    (502) staff       (20)     1834 2024-04-17 18:41:13.000000 algorin-cli-0.2/algorin-cli/main.py
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:55:16.669851 algorin-cli-0.2/algorin_cli.egg-info/
+-rw-r--r--   0 1064331    (502) staff       (20)     7651 2024-04-17 21:55:16.000000 algorin-cli-0.2/algorin_cli.egg-info/PKG-INFO
+-rw-r--r--   0 1064331    (502) staff       (20)      415 2024-04-17 21:55:16.000000 algorin-cli-0.2/algorin_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 1064331    (502) staff       (20)        1 2024-04-17 21:55:16.000000 algorin-cli-0.2/algorin_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 1064331    (502) staff       (20)       58 2024-04-17 21:55:16.000000 algorin-cli-0.2/algorin_cli.egg-info/entry_points.txt
+-rw-r--r--   0 1064331    (502) staff       (20)     3831 2024-04-17 21:55:16.000000 algorin-cli-0.2/algorin_cli.egg-info/requires.txt
+-rw-r--r--   0 1064331    (502) staff       (20)       18 2024-04-17 21:55:16.000000 algorin-cli-0.2/algorin_cli.egg-info/top_level.txt
+-rw-r--r--   0 1064331    (502) staff       (20)       38 2024-04-17 21:55:16.686416 algorin-cli-0.2/setup.cfg
+-rw-r--r--   0 1064331    (502) staff       (20)      881 2024-04-17 21:55:05.000000 algorin-cli-0.2/setup.py
+drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-17 21:55:16.673756 algorin-cli-0.2/tests/
+-rw-r--r--   0 1064331    (502) staff       (20)      178 2024-04-17 20:21:38.000000 algorin-cli-0.2/tests/__init__.py
+-rw-r--r--   0 1064331    (502) staff       (20)      546 2024-04-17 20:22:40.000000 algorin-cli-0.2/tests/test_chatbot.py
+-rw-r--r--   0 1064331    (502) staff       (20)      769 2024-04-17 20:22:47.000000 algorin-cli-0.2/tests/test_file_extractor.py
+-rw-r--r--   0 1064331    (502) staff       (20)      631 2024-04-17 20:22:52.000000 algorin-cli-0.2/tests/test_main.py
```

### Comparing `algorin_cli-0.17/PKG-INFO` & `algorin-cli-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorin-cli
-Version: 0.17
+Version: 0.2
 Summary: Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.
 Home-page: https://github.com/Jorge-Polanco-Roque/bot_cli
 Author: JP
 Author-email: jorge.polanco@itesm.mx
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `algorin_cli-0.17/algorin/chatbot.py` & `algorin-cli-0.2/algorin-cli/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,54 @@
-from openai import OpenAI
-
-client = None
-
-def setup_api_key(key):
-    global client
-    # Inicializa el cliente de OpenAI una vez que la API key está configurada
-    client = OpenAI(api_key=key)
-
-def chat_with_gpt(initial_context):
-    global client
-    if client is None:
-        print("Cliente de OpenAI no inicializado. Por favor, ejecute setup_api_key primero.")
-        return
-
-    chat_log = [{"role": "system", "content": "You are a helpful assistant."}]
-    if initial_context:
-        chat_log.append({"role": "user", "content": initial_context})
-
-    while True:
-        user_input = input("Tú: ")
-        if user_input.lower() == "exit":
-            print("Terminando chat...")
-            break
-
-        chat_log.append({"role": "user", "content": user_input})
-
+#!/usr/bin/venv python3
+import os
+from file_extractor import extract_text
+from chatbot import setup_api_key, chat_with_gpt, chat_without_context
+
+def execute_transcript(path):
+    if not os.path.exists(path):
+        print("La ruta especificada no existe.")
+        return ""
+    
+    files = [f for f in os.listdir(path) if f.endswith(('.txt', '.pdf', '.docx', '.pptx'))]
+    texts = []
+    for f in files:
+        file_path = os.path.join(path, f)
         try:
-            response = client.chat.completions.create(
-                model="gpt-3.5-turbo",
-                messages=chat_log
-            )
-            bot_response = response.choices[0].message.content
-            print("ChatGPT: ", bot_response)
-
-            chat_log.append({"role": "assistant", "content": bot_response})
+            text = extract_text(file_path)
+            texts.append(text)
         except Exception as e:
-            print(f"Error al generar la respuesta del chat: {e}")
+            print(f"No se pudo procesar el archivo {f} debido a un error: {e}")
+    
+    combined_text = "\n\n".join(texts)
+    return combined_text
+
+def main_menu():
+    print("Bienvenido al CLI de Documentos y ChatGPT")
+    api_key = input("Por favor, ingrese su API key de OpenAI: ")
+    setup_api_key(api_key)
+    
+    while True:
+        print("\nMenú:")
+        print("1. Extraer texto y chat con contexto")
+        print("2. Chat directo sin contexto")
+        print("3. Salir")
+        choice = input("Ingrese su elección (1-3): ")
+        
+        if choice == '1':
+            path = input("Por favor, ingrese la ruta donde están los archivos: ")
+            context = execute_transcript(path)
+            if context:
+                print("Iniciando chat con contexto...")
+                chat_with_gpt(context)
+            else:
+                print("No se encontró texto válido para usar como contexto.")
+        elif choice == '2':
+            print("Iniciando chat directo sin contexto...")
+            chat_without_context()
+        elif choice == '3':
+            print("Saliendo del programa...")
             break
+        else:
+            print("Opción no válida, por favor intente de nuevo.")
 
-def chat_without_context():
-    chat_with_gpt(None)
+if __name__ == "__main__":
+    main_menu()
```

### Comparing `algorin_cli-0.17/algorin/file_extractor.py` & `algorin-cli-0.2/algorin-cli/file_extractor.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.17/algorin_cli.egg-info/PKG-INFO` & `algorin-cli-0.2/algorin_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorin-cli
-Version: 0.17
+Version: 0.2
 Summary: Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.
 Home-page: https://github.com/Jorge-Polanco-Roque/bot_cli
 Author: JP
 Author-email: jorge.polanco@itesm.mx
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `algorin_cli-0.17/algorin_cli.egg-info/requires.txt` & `algorin-cli-0.2/algorin_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.17/setup.py` & `algorin-cli-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='algorin-cli',
-    version='0.17',
+    version='0.2',
     author='JP',
     author_email='jorge.polanco@itesm.mx',
     packages=find_packages(),
     install_requires=[line.strip() for line in open("requirements.txt", "r").readlines()],
     description='Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown', 
@@ -15,11 +15,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
-            'algorin-cli=algorin.main:main_menu',  # Asegúrate de que el path aquí es correcto
+            'algorin-cli=algorincli.main:main_menu',  # Asegúrate de que el path aquí es correcto
         ],
     },
 )
```

### Comparing `algorin_cli-0.17/tests/test_chatbot.py` & `algorin-cli-0.2/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.17/tests/test_file_extractor.py` & `algorin-cli-0.2/tests/test_file_extractor.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.17/tests/test_main.py` & `algorin-cli-0.2/tests/test_main.py`

 * *Files identical despite different names*

