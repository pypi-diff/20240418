# Comparing `tmp/flatpack-3.3.0.tar.gz` & `tmp/flatpack-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.3.0.tar", last modified: Tue Apr 16 19:54:57 2024, max compression
+gzip compressed data, was "flatpack-3.3.1.tar", last modified: Thu Apr 18 10:05:02 2024, max compression
```

## Comparing `flatpack-3.3.0.tar` & `flatpack-3.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-16 19:54:57.546888 flatpack-3.3.0/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.0/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-16 19:54:57.546555 flatpack-3.3.0/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     4456 2024-04-16 19:54:33.000000 flatpack-3.3.0/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-16 19:54:57.543959 flatpack-3.3.0/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.0/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.0/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.0/flatpack/datasets.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.0/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    26035 2024-04-16 19:03:58.000000 flatpack-3.3.0/flatpack/main.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.0/flatpack/models.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-16 19:54:57.545864 flatpack-3.3.0/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.0/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.0/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.0/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.0/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.0/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     3952 2024-04-16 19:15:27.000000 flatpack-3.3.0/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-16 19:54:57.546175 flatpack-3.3.0/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-16 19:54:57.000000 flatpack-3.3.0/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-16 19:54:57.000000 flatpack-3.3.0/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-16 19:54:57.000000 flatpack-3.3.0/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-16 19:54:57.000000 flatpack-3.3.0/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      206 2024-04-16 19:54:57.000000 flatpack-3.3.0/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-16 19:54:57.000000 flatpack-3.3.0/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-16 19:54:57.547118 flatpack-3.3.0/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)      916 2024-04-16 19:50:51.000000 flatpack-3.3.0/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-18 10:05:02.500169 flatpack-3.3.1/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.3.1/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-18 10:05:02.499764 flatpack-3.3.1/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4456 2024-04-16 19:54:33.000000 flatpack-3.3.1/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-18 10:05:02.496545 flatpack-3.3.1/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      132 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/datasets.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1057 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    26139 2024-04-18 10:04:30.000000 flatpack-3.3.1/flatpack/main.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       59 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/models.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-18 10:05:02.498917 flatpack-3.3.1/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6972 2024-04-06 18:22:51.000000 flatpack-3.3.1/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.3.1/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     3952 2024-04-16 19:15:27.000000 flatpack-3.3.1/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-04-18 10:05:02.499296 flatpack-3.3.1/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5089 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      485 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      206 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-04-18 10:05:02.000000 flatpack-3.3.1/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-04-18 10:05:02.500378 flatpack-3.3.1/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      916 2024-04-18 10:03:35.000000 flatpack-3.3.1/setup.py
```

### Comparing `flatpack-3.3.0/LICENSE` & `flatpack-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.0/PKG-INFO` & `flatpack-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.0
+Version: 3.3.1
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.3.0/README.md` & `flatpack-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.0/flatpack/datasets.py` & `flatpack-3.3.1/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.0/flatpack/instructions.py` & `flatpack-3.3.1/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.0/flatpack/main.py` & `flatpack-3.3.1/flatpack/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,36 +547,37 @@
                                                  help='Build a model using the building script from the last unboxed flatpack.')
             parser_build.add_argument('directory', nargs='?', default=None,
                                       help='The directory of the flatpack to build.')
 
             subparsers.add_parser('version', help='Display the version of flatpack.')
 
             # Adding subparsers for 'add-text' and 'search-text' commands specifically because they need additional arguments
-            parser_add_text = subparsers.add_parser('add-text',
+            parser_add_text = subparsers.add_parser('vector-add-texts',
                                                     help='Add new texts to generate embeddings and store them.')
             parser_add_text.add_argument('texts', nargs='+', help='Texts to add.')
 
-            parser_search_text = subparsers.add_parser('search-text',
+            parser_search_text = subparsers.add_parser('vector-search-text',
                                                        help='Search for texts similar to the given query.')
             parser_search_text.add_argument('query', help='Text query to search for.')
 
-            parser_add_pdf = subparsers.add_parser('add-pdf', help='Add text from a PDF file to the vector database.')
+            parser_add_pdf = subparsers.add_parser('vector-add-pdf',
+                                                   help='Add text from a PDF file to the vector database.')
             parser_add_pdf.add_argument('pdf_path', help='Path to the PDF file to add.')
 
-            parser_add_url = subparsers.add_parser('add-url', help='Add text from a URL to the vector database.')
+            parser_add_url = subparsers.add_parser('vector-add-url', help='Add text from a URL to the vector database.')
             parser_add_url.add_argument('url', help='URL to add.')
 
             args = parser.parse_args()
 
             fpk_get_api_key()
 
-            if args.command == 'add-text':
+            if args.command == 'vector-add-texts':
                 vm.add_texts(args.texts)
                 print(f"Added {len(args.texts)} texts to the database.")
-            elif args.command == 'search-text':
+            elif args.command == 'vector-search':
                 try:
                     results = vm.search_vectors(args.query)
                     if results:
                         print("Search results:")
                         for result in results:
                             id = result["id"]
                             rank = result["rank"]
@@ -584,22 +585,22 @@
                             print(f"({rank}) {id}: {text}\n")
                     else:
                         print("No results found.")
                 except ValueError as e:
                     print(f"Error: {e}")
                 except Exception as e:
                     print(f"❌ An unexpected error occurred.")
-            elif args.command == 'add-pdf':
+            elif args.command == 'vector-add-pdf':
                 pdf_path = args.pdf_path
                 if not os.path.exists(pdf_path):
                     print(f"❌ PDF file does not exist: '{pdf_path}'.")
                     return
                 vm.add_pdf(pdf_path)
                 print(f"✅ Added text from PDF: '{pdf_path}' to the vector database.")
-            elif args.command == 'add-url':
+            elif args.command == 'vector-add-url':
                 url = args.url
                 try:
                     response = requests.head(url, allow_redirects=True, timeout=5)
                     if response.status_code >= 200 and response.status_code < 400:
                         vm.add_url(url)
                         print(f"✅ Added text from URL: '{url}' to the vector database.")
                     else:
```

### Comparing `flatpack-3.3.0/flatpack/modules/lstm.py` & `flatpack-3.3.1/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.0/flatpack/modules/rnn.py` & `flatpack-3.3.1/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.0/flatpack/parsers.py` & `flatpack-3.3.1/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.0/flatpack/vector_manager.py` & `flatpack-3.3.1/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.3.0/flatpack.egg-info/PKG-INFO` & `flatpack-3.3.1/flatpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.3.0
+Version: 3.3.1
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `flatpack-3.3.0/setup.py` & `flatpack-3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.3.0",
+    version="3.3.1",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "cryptography==42.0.5",
         "faiss-cpu==1.8.0",
         "fastapi==0.110.1",
```

