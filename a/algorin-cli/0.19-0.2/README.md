# Comparing `tmp/algorin_cli-0.19.tar.gz` & `tmp/algorin-cli-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algorin_cli-0.19.tar", last modified: Thu Apr 18 01:31:01 2024, max compression
+gzip compressed data, was "algorin-cli-0.2.tar", last modified: Wed Apr 17 21:55:16 2024, max compression
```

## Comparing `algorin_cli-0.19.tar` & `algorin-cli-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-18 01:31:01.038347 algorin_cli-0.19/
--rw-r--r--   0 1064331    (502) staff       (20)     7951 2024-04-18 01:31:01.037247 algorin_cli-0.19/PKG-INFO
--rw-r--r--   0 1064331    (502) staff       (20)       33 2024-04-17 19:58:47.000000 algorin_cli-0.19/README.md
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-18 01:31:01.009619 algorin_cli-0.19/algorin/
--rw-r--r--   0 1064331    (502) staff       (20)      515 2024-04-18 01:24:21.000000 algorin_cli-0.19/algorin/__init__.py
--rw-r--r--   0 1064331    (502) staff       (20)     1284 2024-04-18 01:06:50.000000 algorin_cli-0.19/algorin/chatbot.py
--rw-r--r--   0 1064331    (502) staff       (20)     1021 2024-04-17 22:04:49.000000 algorin_cli-0.19/algorin/file_extractor.py
--rw-r--r--   0 1064331    (502) staff       (20)     2230 2024-04-18 01:28:03.000000 algorin_cli-0.19/algorin/main.py
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-18 01:31:01.027278 algorin_cli-0.19/algorin_cli.egg-info/
--rw-r--r--   0 1064331    (502) staff       (20)     7951 2024-04-18 01:31:00.000000 algorin_cli-0.19/algorin_cli.egg-info/PKG-INFO
--rw-r--r--   0 1064331    (502) staff       (20)      399 2024-04-18 01:31:00.000000 algorin_cli-0.19/algorin_cli.egg-info/SOURCES.txt
--rw-r--r--   0 1064331    (502) staff       (20)        1 2024-04-18 01:31:00.000000 algorin_cli-0.19/algorin_cli.egg-info/dependency_links.txt
--rw-r--r--   0 1064331    (502) staff       (20)       55 2024-04-18 01:31:00.000000 algorin_cli-0.19/algorin_cli.egg-info/entry_points.txt
--rw-r--r--   0 1064331    (502) staff       (20)     4100 2024-04-18 01:31:00.000000 algorin_cli-0.19/algorin_cli.egg-info/requires.txt
--rw-r--r--   0 1064331    (502) staff       (20)       14 2024-04-18 01:31:00.000000 algorin_cli-0.19/algorin_cli.egg-info/top_level.txt
--rw-r--r--   0 1064331    (502) staff       (20)       38 2024-04-18 01:31:01.038464 algorin_cli-0.19/setup.cfg
--rw-r--r--   0 1064331    (502) staff       (20)      879 2024-04-18 01:30:50.000000 algorin_cli-0.19/setup.py
-drwxr-xr-x   0 1064331    (502) staff       (20)        0 2024-04-18 01:31:01.023870 algorin_cli-0.19/tests/
--rw-r--r--   0 1064331    (502) staff       (20)      178 2024-04-17 20:21:38.000000 algorin_cli-0.19/tests/__init__.py
--rw-r--r--   0 1064331    (502) staff       (20)      546 2024-04-17 20:22:40.000000 algorin_cli-0.19/tests/test_chatbot.py
--rw-r--r--   0 1064331    (502) staff       (20)      769 2024-04-17 20:22:47.000000 algorin_cli-0.19/tests/test_file_extractor.py
--rw-r--r--   0 1064331    (502) staff       (20)      631 2024-04-17 20:22:52.000000 algorin_cli-0.19/tests/test_main.py
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

### Comparing `algorin_cli-0.19/PKG-INFO` & `algorin-cli-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: algorin-cli
-Version: 0.19
+Version: 0.2
 Summary: Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.
 Home-page: https://github.com/Jorge-Polanco-Roque/bot_cli
 Author: JP
 Author-email: jorge.polanco@itesm.mx
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
-Requires-Dist: algorin-cli==0.18
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.2.0
 Requires-Dist: appdirs==1.4.4
-Requires-Dist: appnope==0.1.4
-Requires-Dist: asttokens==2.4.1
+Requires-Dist: appnope
+Requires-Dist: asttokens
 Requires-Dist: attrs==23.2.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: backports.tarfile==1.1.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: bitarray==2.9.2
 Requires-Dist: blinker==1.7.0
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: chardet==5.2.0
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: chroma-hnswlib==0.7.2
 Requires-Dist: chromadb==0.4.6
 Requires-Dist: click==8.1.7
 Requires-Dist: coloredlogs==15.0.1
-Requires-Dist: comm==0.2.2
+Requires-Dist: comm
 Requires-Dist: dataclasses-json==0.6.4
 Requires-Dist: dataclasses-json-speakeasy==0.5.11
 Requires-Dist: datasets==2.18.0
-Requires-Dist: debugpy==1.8.1
+Requires-Dist: debugpy
 Requires-Dist: decorator==4.4.2
 Requires-Dist: decouple==0.0.7
 Requires-Dist: dill==0.3.8
 Requires-Dist: diskcache==5.6.3
 Requires-Dist: distro==1.9.0
 Requires-Dist: docker==7.0.0
 Requires-Dist: docstring_parser==0.16
 Requires-Dist: docutils==0.21.1
 Requires-Dist: emoji==2.10.1
-Requires-Dist: exceptiongroup==1.2.0
-Requires-Dist: executing==2.0.1
+Requires-Dist: exceptiongroup
+Requires-Dist: executing
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: fastapi==0.99.1
 Requires-Dist: filelock==3.13.1
 Requires-Dist: filetype==1.2.0
 Requires-Dist: FLAML==2.1.1
 Requires-Dist: Flask==2.3.3
 Requires-Dist: flatbuffers==23.5.26
@@ -76,164 +75,163 @@
 Requires-Dist: httptools==0.6.1
 Requires-Dist: httpx==0.26.0
 Requires-Dist: huggingface-hub==0.21.3
 Requires-Dist: humanfriendly==10.0
 Requires-Dist: idna==3.6
 Requires-Dist: imageio==2.34.0
 Requires-Dist: imageio-ffmpeg==0.4.9
-Requires-Dist: importlib_metadata==7.1.0
+Requires-Dist: importlib-metadata
 Requires-Dist: importlib_resources==6.1.2
 Requires-Dist: iniconfig==2.0.0
-Requires-Dist: ipykernel==6.29.4
-Requires-Dist: ipython==8.23.0
+Requires-Dist: ipykernel
+Requires-Dist: ipython
 Requires-Dist: itsdangerous==2.1.2
 Requires-Dist: jaraco.classes==3.4.0
 Requires-Dist: jaraco.context==5.3.0
 Requires-Dist: jaraco.functools==4.0.0
-Requires-Dist: jedi==0.19.1
+Requires-Dist: jedi
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: joblib==1.3.2
 Requires-Dist: jsonpatch==1.33
 Requires-Dist: jsonpath-python==1.0.6
 Requires-Dist: jsonpointer==2.4
-Requires-Dist: jupyter_client==8.6.1
-Requires-Dist: jupyter_core==5.7.2
+Requires-Dist: jupyter_client
+Requires-Dist: jupyter_core
 Requires-Dist: keyring==25.1.0
 Requires-Dist: langchain==0.1.9
 Requires-Dist: langchain-community==0.0.27
 Requires-Dist: langchain-core==0.1.30
 Requires-Dist: langchain-openai==0.0.8
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: langgraph==0.0.29
 Requires-Dist: langsmith==0.1.10
 Requires-Dist: llvmlite==0.42.0
 Requires-Dist: lxml==5.1.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: marshmallow==3.20.2
-Requires-Dist: matplotlib-inline==0.1.7
+Requires-Dist: matplotlib-inline
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: monotonic==1.6
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: moviepy==1.0.3
 Requires-Dist: mpmath==1.3.0
 Requires-Dist: multidict==6.0.5
 Requires-Dist: multiprocess==0.70.16
 Requires-Dist: mypy-extensions==1.0.0
-Requires-Dist: nest-asyncio==1.6.0
+Requires-Dist: nest_asyncio
 Requires-Dist: networkx==3.2.1
 Requires-Dist: nh3==0.2.17
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numba==0.59.0
 Requires-Dist: numpy==1.26.4
 Requires-Dist: onnxruntime==1.17.1
-Requires-Dist: openai==1.21.2
+Requires-Dist: openai
 Requires-Dist: openai-whisper==20231117
 Requires-Dist: opencv-python-headless==4.9.0.80
 Requires-Dist: orjson==3.9.15
 Requires-Dist: overrides==7.7.0
-Requires-Dist: packaging==23.2
+Requires-Dist: packaging
 Requires-Dist: pandas==2.2.1
-Requires-Dist: parso==0.8.4
+Requires-Dist: parso
 Requires-Dist: pdfreader==0.1.12
-Requires-Dist: pexpect==4.9.0
-Requires-Dist: pickleshare==0.7.5
+Requires-Dist: pexpect
+Requires-Dist: pickleshare
 Requires-Dist: pillow==10.2.0
 Requires-Dist: pkginfo==1.10.0
-Requires-Dist: platformdirs==4.2.0
+Requires-Dist: platformdirs
 Requires-Dist: pluggy==1.4.0
 Requires-Dist: posthog==3.4.2
 Requires-Dist: proglog==0.1.10
-Requires-Dist: prompt-toolkit==3.0.43
+Requires-Dist: prompt-toolkit
 Requires-Dist: proto-plus==1.23.0
 Requires-Dist: protobuf==4.25.3
-Requires-Dist: psutil==5.9.8
-Requires-Dist: ptyprocess==0.7.0
+Requires-Dist: psutil
+Requires-Dist: ptyprocess
 Requires-Dist: pulsar-client==3.4.0
-Requires-Dist: pure-eval==0.2.2
+Requires-Dist: pure-eval
 Requires-Dist: pyarrow==15.0.2
 Requires-Dist: pyarrow-hotfix==0.6
 Requires-Dist: pyasn1==0.6.0
 Requires-Dist: pyasn1_modules==0.4.0
 Requires-Dist: pyautogen==0.2.13
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: pydantic==1.10.0
 Requires-Dist: pydantic_core==2.16.2
 Requires-Dist: pyee==11.1.0
-Requires-Dist: Pygments==2.17.2
+Requires-Dist: Pygments
 Requires-Dist: PyMuPDF==1.23.26
 Requires-Dist: PyMuPDFb==1.23.22
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: PyPika==0.48.9
 Requires-Dist: pysbd==0.3.4
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: pytest==8.1.1
 Requires-Dist: pytest-mock==3.14.0
-Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: python-dateutil
 Requires-Dist: python-decouple==3.8
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: python-iso639==2024.2.7
 Requires-Dist: python-magic==0.4.27
 Requires-Dist: python-pptx==0.6.23
 Requires-Dist: pytube==15.0.0
 Requires-Dist: pytz==2024.1
 Requires-Dist: PyYAML==6.0.1
-Requires-Dist: pyzmq==26.0.0
+Requires-Dist: pyzmq
 Requires-Dist: ragas==0.1.6
 Requires-Dist: rapidfuzz==3.6.1
 Requires-Dist: readme_renderer==43.0
 Requires-Dist: regex==2023.12.25
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: rsa==4.9
 Requires-Dist: safetensors==0.4.2
 Requires-Dist: scikit-learn==1.4.1.post1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: sentence-transformers==2.5.0
 Requires-Dist: shapely==2.0.4
-Requires-Dist: six==1.16.0
+Requires-Dist: six
 Requires-Dist: slack_sdk==3.27.1
 Requires-Dist: slackclient==2.9.4
 Requires-Dist: slackeventsapi==3.0.1
 Requires-Dist: sniffio==1.3.0
 Requires-Dist: soupsieve==2.5
 Requires-Dist: SQLAlchemy==2.0.27
-Requires-Dist: stack-data==0.6.3
+Requires-Dist: stack-data
 Requires-Dist: starlette==0.27.0
 Requires-Dist: sympy==1.12
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: tenacity==8.2.3
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: threadpoolctl==3.3.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: tokenizers==0.15.2
 Requires-Dist: torch==2.1.2
-Requires-Dist: tornado==6.4
+Requires-Dist: tornado
 Requires-Dist: tqdm==4.66.2
-Requires-Dist: traitlets==5.14.2
+Requires-Dist: traitlets
 Requires-Dist: transformers==4.38.1
 Requires-Dist: twine==5.0.0
 Requires-Dist: typing-inspect==0.9.0
 Requires-Dist: typing_extensions==4.9.0
 Requires-Dist: tzdata==2024.1
 Requires-Dist: unstructured==0.13.0
 Requires-Dist: unstructured-client==0.18.0
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: uvicorn==0.27.1
 Requires-Dist: uvloop==0.19.0
 Requires-Dist: vision-agent==0.0.46
 Requires-Dist: watchfiles==0.21.0
-Requires-Dist: wcwidth==0.2.13
+Requires-Dist: wcwidth
 Requires-Dist: websockets==12.0
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: wrapt==1.16.0
 Requires-Dist: XlsxWriter==3.2.0
 Requires-Dist: xxhash==3.4.1
 Requires-Dist: yarl==1.9.4
-Requires-Dist: yolk3k==0.9
 Requires-Dist: youtube-dl==2021.12.17
-Requires-Dist: zipp==3.18.1
+Requires-Dist: zipp
 
 Dar API Key de OpenAI al inicio.
```

### Comparing `algorin_cli-0.19/algorin/chatbot.py` & `algorin-cli-0.2/algorin-cli/main.py`

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

### Comparing `algorin_cli-0.19/algorin/file_extractor.py` & `algorin-cli-0.2/algorin-cli/file_extractor.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.19/algorin_cli.egg-info/PKG-INFO` & `algorin-cli-0.2/algorin_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: algorin-cli
-Version: 0.19
+Version: 0.2
 Summary: Acceso a GPT-3 y procesamiento de documentos desde la línea de comandos.
 Home-page: https://github.com/Jorge-Polanco-Roque/bot_cli
 Author: JP
 Author-email: jorge.polanco@itesm.mx
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
-Requires-Dist: algorin-cli==0.18
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.2.0
 Requires-Dist: appdirs==1.4.4
-Requires-Dist: appnope==0.1.4
-Requires-Dist: asttokens==2.4.1
+Requires-Dist: appnope
+Requires-Dist: asttokens
 Requires-Dist: attrs==23.2.0
 Requires-Dist: backoff==2.2.1
 Requires-Dist: backports.tarfile==1.1.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: bitarray==2.9.2
 Requires-Dist: blinker==1.7.0
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: chardet==5.2.0
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: chroma-hnswlib==0.7.2
 Requires-Dist: chromadb==0.4.6
 Requires-Dist: click==8.1.7
 Requires-Dist: coloredlogs==15.0.1
-Requires-Dist: comm==0.2.2
+Requires-Dist: comm
 Requires-Dist: dataclasses-json==0.6.4
 Requires-Dist: dataclasses-json-speakeasy==0.5.11
 Requires-Dist: datasets==2.18.0
-Requires-Dist: debugpy==1.8.1
+Requires-Dist: debugpy
 Requires-Dist: decorator==4.4.2
 Requires-Dist: decouple==0.0.7
 Requires-Dist: dill==0.3.8
 Requires-Dist: diskcache==5.6.3
 Requires-Dist: distro==1.9.0
 Requires-Dist: docker==7.0.0
 Requires-Dist: docstring_parser==0.16
 Requires-Dist: docutils==0.21.1
 Requires-Dist: emoji==2.10.1
-Requires-Dist: exceptiongroup==1.2.0
-Requires-Dist: executing==2.0.1
+Requires-Dist: exceptiongroup
+Requires-Dist: executing
 Requires-Dist: faiss-cpu==1.8.0
 Requires-Dist: fastapi==0.99.1
 Requires-Dist: filelock==3.13.1
 Requires-Dist: filetype==1.2.0
 Requires-Dist: FLAML==2.1.1
 Requires-Dist: Flask==2.3.3
 Requires-Dist: flatbuffers==23.5.26
@@ -76,164 +75,163 @@
 Requires-Dist: httptools==0.6.1
 Requires-Dist: httpx==0.26.0
 Requires-Dist: huggingface-hub==0.21.3
 Requires-Dist: humanfriendly==10.0
 Requires-Dist: idna==3.6
 Requires-Dist: imageio==2.34.0
 Requires-Dist: imageio-ffmpeg==0.4.9
-Requires-Dist: importlib_metadata==7.1.0
+Requires-Dist: importlib-metadata
 Requires-Dist: importlib_resources==6.1.2
 Requires-Dist: iniconfig==2.0.0
-Requires-Dist: ipykernel==6.29.4
-Requires-Dist: ipython==8.23.0
+Requires-Dist: ipykernel
+Requires-Dist: ipython
 Requires-Dist: itsdangerous==2.1.2
 Requires-Dist: jaraco.classes==3.4.0
 Requires-Dist: jaraco.context==5.3.0
 Requires-Dist: jaraco.functools==4.0.0
-Requires-Dist: jedi==0.19.1
+Requires-Dist: jedi
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: joblib==1.3.2
 Requires-Dist: jsonpatch==1.33
 Requires-Dist: jsonpath-python==1.0.6
 Requires-Dist: jsonpointer==2.4
-Requires-Dist: jupyter_client==8.6.1
-Requires-Dist: jupyter_core==5.7.2
+Requires-Dist: jupyter_client
+Requires-Dist: jupyter_core
 Requires-Dist: keyring==25.1.0
 Requires-Dist: langchain==0.1.9
 Requires-Dist: langchain-community==0.0.27
 Requires-Dist: langchain-core==0.1.30
 Requires-Dist: langchain-openai==0.0.8
 Requires-Dist: langdetect==1.0.9
 Requires-Dist: langgraph==0.0.29
 Requires-Dist: langsmith==0.1.10
 Requires-Dist: llvmlite==0.42.0
 Requires-Dist: lxml==5.1.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: marshmallow==3.20.2
-Requires-Dist: matplotlib-inline==0.1.7
+Requires-Dist: matplotlib-inline
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: monotonic==1.6
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: moviepy==1.0.3
 Requires-Dist: mpmath==1.3.0
 Requires-Dist: multidict==6.0.5
 Requires-Dist: multiprocess==0.70.16
 Requires-Dist: mypy-extensions==1.0.0
-Requires-Dist: nest-asyncio==1.6.0
+Requires-Dist: nest_asyncio
 Requires-Dist: networkx==3.2.1
 Requires-Dist: nh3==0.2.17
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numba==0.59.0
 Requires-Dist: numpy==1.26.4
 Requires-Dist: onnxruntime==1.17.1
-Requires-Dist: openai==1.21.2
+Requires-Dist: openai
 Requires-Dist: openai-whisper==20231117
 Requires-Dist: opencv-python-headless==4.9.0.80
 Requires-Dist: orjson==3.9.15
 Requires-Dist: overrides==7.7.0
-Requires-Dist: packaging==23.2
+Requires-Dist: packaging
 Requires-Dist: pandas==2.2.1
-Requires-Dist: parso==0.8.4
+Requires-Dist: parso
 Requires-Dist: pdfreader==0.1.12
-Requires-Dist: pexpect==4.9.0
-Requires-Dist: pickleshare==0.7.5
+Requires-Dist: pexpect
+Requires-Dist: pickleshare
 Requires-Dist: pillow==10.2.0
 Requires-Dist: pkginfo==1.10.0
-Requires-Dist: platformdirs==4.2.0
+Requires-Dist: platformdirs
 Requires-Dist: pluggy==1.4.0
 Requires-Dist: posthog==3.4.2
 Requires-Dist: proglog==0.1.10
-Requires-Dist: prompt-toolkit==3.0.43
+Requires-Dist: prompt-toolkit
 Requires-Dist: proto-plus==1.23.0
 Requires-Dist: protobuf==4.25.3
-Requires-Dist: psutil==5.9.8
-Requires-Dist: ptyprocess==0.7.0
+Requires-Dist: psutil
+Requires-Dist: ptyprocess
 Requires-Dist: pulsar-client==3.4.0
-Requires-Dist: pure-eval==0.2.2
+Requires-Dist: pure-eval
 Requires-Dist: pyarrow==15.0.2
 Requires-Dist: pyarrow-hotfix==0.6
 Requires-Dist: pyasn1==0.6.0
 Requires-Dist: pyasn1_modules==0.4.0
 Requires-Dist: pyautogen==0.2.13
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: pydantic==1.10.0
 Requires-Dist: pydantic_core==2.16.2
 Requires-Dist: pyee==11.1.0
-Requires-Dist: Pygments==2.17.2
+Requires-Dist: Pygments
 Requires-Dist: PyMuPDF==1.23.26
 Requires-Dist: PyMuPDFb==1.23.22
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: PyPika==0.48.9
 Requires-Dist: pysbd==0.3.4
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: pytest==8.1.1
 Requires-Dist: pytest-mock==3.14.0
-Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: python-dateutil
 Requires-Dist: python-decouple==3.8
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: python-iso639==2024.2.7
 Requires-Dist: python-magic==0.4.27
 Requires-Dist: python-pptx==0.6.23
 Requires-Dist: pytube==15.0.0
 Requires-Dist: pytz==2024.1
 Requires-Dist: PyYAML==6.0.1
-Requires-Dist: pyzmq==26.0.0
+Requires-Dist: pyzmq
 Requires-Dist: ragas==0.1.6
 Requires-Dist: rapidfuzz==3.6.1
 Requires-Dist: readme_renderer==43.0
 Requires-Dist: regex==2023.12.25
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: rsa==4.9
 Requires-Dist: safetensors==0.4.2
 Requires-Dist: scikit-learn==1.4.1.post1
 Requires-Dist: scipy==1.12.0
 Requires-Dist: sentence-transformers==2.5.0
 Requires-Dist: shapely==2.0.4
-Requires-Dist: six==1.16.0
+Requires-Dist: six
 Requires-Dist: slack_sdk==3.27.1
 Requires-Dist: slackclient==2.9.4
 Requires-Dist: slackeventsapi==3.0.1
 Requires-Dist: sniffio==1.3.0
 Requires-Dist: soupsieve==2.5
 Requires-Dist: SQLAlchemy==2.0.27
-Requires-Dist: stack-data==0.6.3
+Requires-Dist: stack-data
 Requires-Dist: starlette==0.27.0
 Requires-Dist: sympy==1.12
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: tenacity==8.2.3
 Requires-Dist: termcolor==2.4.0
 Requires-Dist: threadpoolctl==3.3.0
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: tokenizers==0.15.2
 Requires-Dist: torch==2.1.2
-Requires-Dist: tornado==6.4
+Requires-Dist: tornado
 Requires-Dist: tqdm==4.66.2
-Requires-Dist: traitlets==5.14.2
+Requires-Dist: traitlets
 Requires-Dist: transformers==4.38.1
 Requires-Dist: twine==5.0.0
 Requires-Dist: typing-inspect==0.9.0
 Requires-Dist: typing_extensions==4.9.0
 Requires-Dist: tzdata==2024.1
 Requires-Dist: unstructured==0.13.0
 Requires-Dist: unstructured-client==0.18.0
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: uvicorn==0.27.1
 Requires-Dist: uvloop==0.19.0
 Requires-Dist: vision-agent==0.0.46
 Requires-Dist: watchfiles==0.21.0
-Requires-Dist: wcwidth==0.2.13
+Requires-Dist: wcwidth
 Requires-Dist: websockets==12.0
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: wrapt==1.16.0
 Requires-Dist: XlsxWriter==3.2.0
 Requires-Dist: xxhash==3.4.1
 Requires-Dist: yarl==1.9.4
-Requires-Dist: yolk3k==0.9
 Requires-Dist: youtube-dl==2021.12.17
-Requires-Dist: zipp==3.18.1
+Requires-Dist: zipp
 
 Dar API Key de OpenAI al inicio.
```

### Comparing `algorin_cli-0.19/algorin_cli.egg-info/requires.txt` & `algorin-cli-0.2/algorin_cli.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 aiohttp==3.9.3
 aiosignal==1.3.1
-algorin-cli==0.18
 annotated-types==0.6.0
 anyio==4.2.0
 appdirs==1.4.4
-appnope==0.1.4
-asttokens==2.4.1
+appnope
+asttokens
 attrs==23.2.0
 backoff==2.2.1
 backports.tarfile==1.1.0
 beautifulsoup4==4.12.3
 bitarray==2.9.2
 blinker==1.7.0
 cachetools==5.3.3
 certifi==2024.2.2
 chardet==5.2.0
 charset-normalizer==3.3.2
 chroma-hnswlib==0.7.2
 chromadb==0.4.6
 click==8.1.7
 coloredlogs==15.0.1
-comm==0.2.2
+comm
 dataclasses-json==0.6.4
 dataclasses-json-speakeasy==0.5.11
 datasets==2.18.0
-debugpy==1.8.1
+debugpy
 decorator==4.4.2
 decouple==0.0.7
 dill==0.3.8
 diskcache==5.6.3
 distro==1.9.0
 docker==7.0.0
 docstring_parser==0.16
 docutils==0.21.1
 emoji==2.10.1
-exceptiongroup==1.2.0
-executing==2.0.1
+exceptiongroup
+executing
 faiss-cpu==1.8.0
 fastapi==0.99.1
 filelock==3.13.1
 filetype==1.2.0
 FLAML==2.1.1
 Flask==2.3.3
 flatbuffers==23.5.26
@@ -64,162 +63,161 @@
 httptools==0.6.1
 httpx==0.26.0
 huggingface-hub==0.21.3
 humanfriendly==10.0
 idna==3.6
 imageio==2.34.0
 imageio-ffmpeg==0.4.9
-importlib_metadata==7.1.0
+importlib-metadata
 importlib_resources==6.1.2
 iniconfig==2.0.0
-ipykernel==6.29.4
-ipython==8.23.0
+ipykernel
+ipython
 itsdangerous==2.1.2
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
 jaraco.functools==4.0.0
-jedi==0.19.1
+jedi
 Jinja2==3.1.3
 joblib==1.3.2
 jsonpatch==1.33
 jsonpath-python==1.0.6
 jsonpointer==2.4
-jupyter_client==8.6.1
-jupyter_core==5.7.2
+jupyter_client
+jupyter_core
 keyring==25.1.0
 langchain==0.1.9
 langchain-community==0.0.27
 langchain-core==0.1.30
 langchain-openai==0.0.8
 langdetect==1.0.9
 langgraph==0.0.29
 langsmith==0.1.10
 llvmlite==0.42.0
 lxml==5.1.0
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 marshmallow==3.20.2
-matplotlib-inline==0.1.7
+matplotlib-inline
 mdurl==0.1.2
 monotonic==1.6
 more-itertools==10.2.0
 moviepy==1.0.3
 mpmath==1.3.0
 multidict==6.0.5
 multiprocess==0.70.16
 mypy-extensions==1.0.0
-nest-asyncio==1.6.0
+nest_asyncio
 networkx==3.2.1
 nh3==0.2.17
 nltk==3.8.1
 numba==0.59.0
 numpy==1.26.4
 onnxruntime==1.17.1
-openai==1.21.2
+openai
 openai-whisper==20231117
 opencv-python-headless==4.9.0.80
 orjson==3.9.15
 overrides==7.7.0
-packaging==23.2
+packaging
 pandas==2.2.1
-parso==0.8.4
+parso
 pdfreader==0.1.12
-pexpect==4.9.0
-pickleshare==0.7.5
+pexpect
+pickleshare
 pillow==10.2.0
 pkginfo==1.10.0
-platformdirs==4.2.0
+platformdirs
 pluggy==1.4.0
 posthog==3.4.2
 proglog==0.1.10
-prompt-toolkit==3.0.43
+prompt-toolkit
 proto-plus==1.23.0
 protobuf==4.25.3
-psutil==5.9.8
-ptyprocess==0.7.0
+psutil
+ptyprocess
 pulsar-client==3.4.0
-pure-eval==0.2.2
+pure-eval
 pyarrow==15.0.2
 pyarrow-hotfix==0.6
 pyasn1==0.6.0
 pyasn1_modules==0.4.0
 pyautogen==0.2.13
 pycryptodome==3.20.0
 pydantic==1.10.0
 pydantic_core==2.16.2
 pyee==11.1.0
-Pygments==2.17.2
+Pygments
 PyMuPDF==1.23.26
 PyMuPDFb==1.23.22
 PyPDF2==3.0.1
 PyPika==0.48.9
 pysbd==0.3.4
 pytesseract==0.3.10
 pytest==8.1.1
 pytest-mock==3.14.0
-python-dateutil==2.8.2
+python-dateutil
 python-decouple==3.8
 python-docx==1.1.0
 python-dotenv==1.0.1
 python-iso639==2024.2.7
 python-magic==0.4.27
 python-pptx==0.6.23
 pytube==15.0.0
 pytz==2024.1
 PyYAML==6.0.1
-pyzmq==26.0.0
+pyzmq
 ragas==0.1.6
 rapidfuzz==3.6.1
 readme_renderer==43.0
 regex==2023.12.25
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 rsa==4.9
 safetensors==0.4.2
 scikit-learn==1.4.1.post1
 scipy==1.12.0
 sentence-transformers==2.5.0
 shapely==2.0.4
-six==1.16.0
+six
 slack_sdk==3.27.1
 slackclient==2.9.4
 slackeventsapi==3.0.1
 sniffio==1.3.0
 soupsieve==2.5
 SQLAlchemy==2.0.27
-stack-data==0.6.3
+stack-data
 starlette==0.27.0
 sympy==1.12
 tabulate==0.9.0
 tenacity==8.2.3
 termcolor==2.4.0
 threadpoolctl==3.3.0
 tiktoken==0.6.0
 tokenizers==0.15.2
 torch==2.1.2
-tornado==6.4
+tornado
 tqdm==4.66.2
-traitlets==5.14.2
+traitlets
 transformers==4.38.1
 twine==5.0.0
 typing-inspect==0.9.0
 typing_extensions==4.9.0
 tzdata==2024.1
 unstructured==0.13.0
 unstructured-client==0.18.0
 urllib3==1.26.18
 uvicorn==0.27.1
 uvloop==0.19.0
 vision-agent==0.0.46
 watchfiles==0.21.0
-wcwidth==0.2.13
+wcwidth
 websockets==12.0
 Werkzeug==3.0.1
 wrapt==1.16.0
 XlsxWriter==3.2.0
 xxhash==3.4.1
 yarl==1.9.4
-yolk3k==0.9
 youtube-dl==2021.12.17
-zipp==3.18.1
+zipp
```

### Comparing `algorin_cli-0.19/setup.py` & `algorin-cli-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='algorin-cli',
-    version='0.19',
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

### Comparing `algorin_cli-0.19/tests/test_chatbot.py` & `algorin-cli-0.2/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.19/tests/test_file_extractor.py` & `algorin-cli-0.2/tests/test_file_extractor.py`

 * *Files identical despite different names*

### Comparing `algorin_cli-0.19/tests/test_main.py` & `algorin-cli-0.2/tests/test_main.py`

 * *Files identical despite different names*

