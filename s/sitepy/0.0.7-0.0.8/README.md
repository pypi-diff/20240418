# Comparing `tmp/sitepy-0.0.7.tar.gz` & `tmp/sitepy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.0.7.tar", last modified: Wed Apr 17 18:32:14 2024, max compression
+gzip compressed data, was "sitepy-0.0.8.tar", last modified: Thu Apr 18 18:40:48 2024, max compression
```

## Comparing `sitepy-0.0.7.tar` & `sitepy-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:32:14.627603 sitepy-0.0.7/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 18:32:14.626933 sitepy-0.0.7/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-17 18:32:14.627730 sitepy-0.0.7/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)     1028 2024-04-17 18:32:03.000000 sitepy-0.0.7/setup.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:32:14.624078 sitepy-0.0.7/sitepy/
--rw-r--r--   0 lewis-family   (501) staff       (20)       24 2024-04-17 18:27:23.000000 sitepy-0.0.7/sitepy/__init__.py
--rw-r--r--   0 lewis-family   (501) staff       (20)     2781 2024-04-17 18:31:56.000000 sitepy-0.0.7/sitepy/core.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:32:14.626396 sitepy-0.0.7/sitepy.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 18:32:14.000000 sitepy-0.0.7/sitepy.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      162 2024-04-17 18:32:14.000000 sitepy-0.0.7/sitepy.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-17 18:32:14.000000 sitepy-0.0.7/sitepy.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-17 18:32:14.000000 sitepy-0.0.7/sitepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 18:40:48.064246 sitepy-0.0.8/
+-rw-rw-rw-   0        0        0     1766 2024-04-18 18:40:48.063246 sitepy-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2024-04-17 20:28:24.000000 sitepy-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 18:40:48.065248 sitepy-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2024-04-17 20:39:38.000000 sitepy-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:40:48.046242 sitepy-0.0.8/sitepy/
+-rw-rw-rw-   0        0        0      112 2024-04-18 18:39:00.000000 sitepy-0.0.8/sitepy/__init__.py
+-rw-rw-rw-   0        0        0     3274 2024-04-18 01:58:35.000000 sitepy-0.0.8/sitepy/sitepy.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:40:48.060245 sitepy-0.0.8/sitepy.egg-info/
+-rw-rw-rw-   0        0        0     1766 2024-04-18 18:40:47.000000 sitepy-0.0.8/sitepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-04-18 18:40:47.000000 sitepy-0.0.8/sitepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 18:40:47.000000 sitepy-0.0.8/sitepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 18:40:47.000000 sitepy-0.0.8/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.0.7/PKG-INFO` & `sitepy-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
-Name: sitepy
-Version: 0.0.7
-Summary: A simple web framework.
-Home-page: https://github.com/WolfTheDeveloper/sitepy
-Author: WolfTheDev
-Author-email: wolfthedev@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# sitepy
-
-A simple web framework for Python.
-
-## Installation
-
-You can install sitepy with pip:
-
-```sh
-pip install sitepy
-```
-
-## Usage
-
-Here's a basic example of a sitepy application:
-
-```python
-from sitepy import sitepy
-
-app = sitepy()
-
-@app.route("/", methods=['GET', 'POST'])
-def index():
-    return "Hello, world!"
-
-if __name__ == "__main__":
-    app.run()
-```
-
-This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
-
-## Features
-
-- Simple routing: Use the @app.route decorator to define routes.
-
-- Middleware support: Use app.use to add middleware functions.
-
-- Static file serving: Files in the static directory are served at /static.
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[Apache](LICENSE)
+Metadata-Version: 2.1
+Name: sitepy
+Version: 0.0.8
+Summary: A simple web framework.
+Home-page: https://github.com/WolfTheDeveloper/sitepy
+Author: WolfTheDev
+Author-email: wolfthedev@gmail.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# sitepy
+
+A simple web framework for Python.
+
+## Installation
+
+You can install sitepy with pip:
+
+```sh
+pip install sitepy
+```
+
+## Usage
+
+Here's a basic example of a sitepy application:
+
+```python
+from sitepy import sitepy
+
+app = sitepy()
+
+@app.route("/", methods=['GET', 'POST'])
+def index():
+    return "Hello, world!"
+
+if __name__ == "__main__":
+    app.run()
+```
+
+This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
+
+## Features
+
+- Simple routing: Use the @app.route decorator to define routes.
+
+- Middleware support: Use app.use to add middleware functions.
+
+- Static file serving: Files in the static directory are served at /static.
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[Apache](LICENSE)
```

### Comparing `sitepy-0.0.7/setup.py` & `sitepy-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='sitepy',
-    version='0.0.7',
-    description='A simple web framework.',
-    author='WolfTheDev',
-    author_email='wolfthedev@gmail.com',
-    url='https://github.com/WolfTheDeveloper/sitepy',
-    packages=find_packages(),
-    long_description=open('sitepy/README.md').read(),
-    long_description_content_type='text/markdown',  # Add this line
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-    ],
-    python_requires='>=3.6',
+from setuptools import setup, find_packages
+
+setup(
+    name='sitepy',
+    version='0.0.8',
+    description='A simple web framework.',
+    author='WolfTheDev',
+    author_email='wolfthedev@gmail.com',
+    url='https://github.com/WolfTheDeveloper/sitepy',
+    packages=find_packages(),
+    long_description=open('sitepy/README.md').read(),
+    long_description_content_type='text/markdown',  # Add this line
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: Apache Software License',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+    ],
+    python_requires='>=3.6',
 )
```

### Comparing `sitepy-0.0.7/sitepy/core.py` & `sitepy-0.0.8/sitepy/sitepy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,82 @@
-import os
-from urllib.parse import parse_qs
-from wsgiref.simple_server import make_server
-import inspect
-
-class SitePy:
-    def __init__(self, static_dir='static'):
-        self.routes = {}
-        self.middleware = [self.logger_middleware]
-        self.static_dir = static_dir
-
-    def route(self, path, methods=['GET']):
-        def wrapper(handler):
-            self.routes[(path, tuple(methods))] = handler
-            return handler
-        return wrapper
-
-    def use(self, middleware):
-        self.middleware.append(middleware)
-
-    def logger_middleware(self, environ):
-        print(f"Request received for {environ['PATH_INFO']}")
-
-    def __call__(self, environ, start_response):
-        path = environ['PATH_INFO']
-        method = environ['REQUEST_METHOD']
-        for middleware in self.middleware:
-            middleware(environ)
-        handler = None
-        for route, methods in self.routes.keys():
-            if path == route and method in methods:
-                handler = self.routes[(route, methods)]
-                break
-        if handler:
-            try:
-                request_body_size = int(environ.get('CONTENT_LENGTH', 0))
-            except ValueError:
-                request_body_size = 0
-            request_body = environ['wsgi.input'].read(request_body_size)
-            params = parse_qs(request_body) if request_body else {}
-            handler_args = inspect.signature(handler).parameters
-            response_body = handler(params) if handler_args else handler()
-            status = '200 OK'
-            headers = [('Content-type', 'text/html')]
-            start_response(status, headers)
-            return [response_body.encode()]
-        elif path.startswith('/' + self.static_dir):
-            try:
-                with open(path[1:], 'rb') as f:
-                    response_body = f.read()
-                status = '200 OK'
-                headers = [('Content-type', 'application/octet-stream')]
-                start_response(status, headers)
-                return [response_body]
-            except FileNotFoundError:
-                status = '404 NOT FOUND'
-                headers = [('Content-type', 'text/html')]
-                start_response(status, headers)
-                return ['File not found'.encode()]
-        else:
-            status = '404 NOT FOUND'
-            headers = [('Content-type', 'text/html')]
-            start_response(status, headers)
-            return ['Route not found'.encode()]
-
-    def run(self, port=8080, host='localhost'):
-        try:
-            server = make_server(host, port, self)
-            print(f'Serving on {host}:{port}')
-            server.serve_forever()
-        except KeyboardInterrupt:
-            print('\nServer shutting down...')
-            server.server_close()
+import os
+from urllib.parse import parse_qs
+from wsgiref.simple_server import make_server
+import inspect
+
+class SitePy:
+    def __init__(self, static_dir='static', templates_dir='templates'):
+        self.routes = {}
+        self.middleware = [self.logger_middleware]
+        self.static_dir = static_dir
+        self.templates_dir = templates_dir
+
+    def render_template(self, template_name, context={}):
+        template_path = os.path.join(self.templates_dir, template_name)
+        with open(template_path, 'r') as f:
+            template = f.read()
+        for key, value in context.items():
+            template = template.replace(f'{{{{ {key} }}}}', value)
+        return template
+
+    def route(self, path, methods=['GET']):
+        def wrapper(handler):
+            self.routes[(path, tuple(methods))] = handler
+            return handler
+        return wrapper
+
+    def use(self, middleware):
+        self.middleware.append(middleware)
+
+    def logger_middleware(self, environ):
+        print(f"Request received for {environ['PATH_INFO']}")
+
+    def __call__(self, environ, start_response):
+        path = environ['PATH_INFO']
+        method = environ['REQUEST_METHOD']
+        for middleware in self.middleware:
+            middleware(environ)
+        handler = None
+        for route, methods in self.routes.keys():
+            if path == route and method in methods:
+                handler = self.routes[(route, methods)]
+                break
+        if handler:
+            try:
+                request_body_size = int(environ.get('CONTENT_LENGTH', 0))
+            except ValueError:
+                request_body_size = 0
+            request_body = environ['wsgi.input'].read(request_body_size)
+            params = parse_qs(request_body) if request_body else {}
+            handler_args = inspect.signature(handler).parameters
+            response_body = handler(params) if handler_args else handler()
+            status = '200 OK'
+            headers = [('Content-type', 'text/html')]
+            start_response(status, headers)
+            return [response_body.encode()]
+        elif path.startswith('/' + self.static_dir):
+            try:
+                with open(path[1:], 'rb') as f:
+                    response_body = f.read()
+                status = '200 OK'
+                headers = [('Content-type', 'application/octet-stream')]
+                start_response(status, headers)
+                return [response_body]
+            except FileNotFoundError:
+                status = '404 NOT FOUND'
+                headers = [('Content-type', 'text/html')]
+                start_response(status, headers)
+                return ['File not found'.encode()]
+        else:
+            status = '404 NOT FOUND'
+            headers = [('Content-type', 'text/html')]
+            start_response(status, headers)
+            return ['Route not found'.encode()]
+
+    def run(self, host='localhost', port=8080):
+        try:
+            server = make_server(host, port, self)
+            print(f'Serving on {host}:{port}')
+            server.serve_forever()
+        except KeyboardInterrupt:
+            print('\nServer shutting down...')
+            server.server_close()
```

### Comparing `sitepy-0.0.7/sitepy.egg-info/PKG-INFO` & `sitepy-0.0.8/sitepy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-Metadata-Version: 2.1
-Name: sitepy
-Version: 0.0.7
-Summary: A simple web framework.
-Home-page: https://github.com/WolfTheDeveloper/sitepy
-Author: WolfTheDev
-Author-email: wolfthedev@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# sitepy
-
-A simple web framework for Python.
-
-## Installation
-
-You can install sitepy with pip:
-
-```sh
-pip install sitepy
-```
-
-## Usage
-
-Here's a basic example of a sitepy application:
-
-```python
-from sitepy import sitepy
-
-app = sitepy()
-
-@app.route("/", methods=['GET', 'POST'])
-def index():
-    return "Hello, world!"
-
-if __name__ == "__main__":
-    app.run()
-```
-
-This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
-
-## Features
-
-- Simple routing: Use the @app.route decorator to define routes.
-
-- Middleware support: Use app.use to add middleware functions.
-
-- Static file serving: Files in the static directory are served at /static.
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[Apache](LICENSE)
+Metadata-Version: 2.1
+Name: sitepy
+Version: 0.0.8
+Summary: A simple web framework.
+Home-page: https://github.com/WolfTheDeveloper/sitepy
+Author: WolfTheDev
+Author-email: wolfthedev@gmail.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# sitepy
+
+A simple web framework for Python.
+
+## Installation
+
+You can install sitepy with pip:
+
+```sh
+pip install sitepy
+```
+
+## Usage
+
+Here's a basic example of a sitepy application:
+
+```python
+from sitepy import sitepy
+
+app = sitepy()
+
+@app.route("/", methods=['GET', 'POST'])
+def index():
+    return "Hello, world!"
+
+if __name__ == "__main__":
+    app.run()
+```
+
+This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
+
+## Features
+
+- Simple routing: Use the @app.route decorator to define routes.
+
+- Middleware support: Use app.use to add middleware functions.
+
+- Static file serving: Files in the static directory are served at /static.
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[Apache](LICENSE)
```

