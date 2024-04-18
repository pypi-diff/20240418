# Comparing `tmp/cefi-4.6.2.tar.gz` & `tmp/cefi-4.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.6.2.tar", max compression
+gzip compressed data, was "cefi-4.6.3.tar", max compression
```

## Comparing `cefi-4.6.2.tar` & `cefi-4.6.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-17 04:28:00.614209 cefi-4.6.2/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-17 04:28:00.614209 cefi-4.6.2/README.md
--rw-r--r--   0        0        0       87 2024-04-17 04:28:38.910304 cefi-4.6.2/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-17 04:28:00.614209 cefi-4.6.2/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-17 04:28:00.614209 cefi-4.6.2/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-17 04:28:00.614209 cefi-4.6.2/cefi/handler/__init__.py
--rw-r--r--   0        0        0    11042 2024-04-17 04:28:00.614209 cefi-4.6.2/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     5517 2024-04-17 04:28:00.614209 cefi-4.6.2/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     9015 2024-04-17 04:28:00.614209 cefi-4.6.2/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-17 04:28:00.614209 cefi-4.6.2/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-17 04:28:00.614209 cefi-4.6.2/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8160 2024-04-17 04:28:00.614209 cefi-4.6.2/cefi/main.py
--rw-r--r--   0        0        0     3764 2024-04-17 04:28:38.910304 cefi-4.6.2/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-18 05:14:43.872266 cefi-4.6.3/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-18 05:14:43.872266 cefi-4.6.3/README.md
+-rw-r--r--   0        0        0       87 2024-04-18 05:15:21.676507 cefi-4.6.3/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-18 05:14:43.872266 cefi-4.6.3/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-18 05:14:43.872266 cefi-4.6.3/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-18 05:14:43.872266 cefi-4.6.3/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    11042 2024-04-18 05:14:43.872266 cefi-4.6.3/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-04-18 05:14:43.872266 cefi-4.6.3/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     9015 2024-04-18 05:14:43.872266 cefi-4.6.3/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-18 05:14:43.872266 cefi-4.6.3/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-18 05:14:43.872266 cefi-4.6.3/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8160 2024-04-18 05:14:43.872266 cefi-4.6.3/cefi/main.py
+-rw-r--r--   0        0        0     3766 2024-04-18 05:15:21.676507 cefi-4.6.3/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.6.3/PKG-INFO
```

### Comparing `cefi-4.6.2/LICENSE` & `cefi-4.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.6.2/README.md` & `cefi-4.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.6.2/cefi/default_settings.toml` & `cefi-4.6.3/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.6.2/cefi/handler/capitalcom.py` & `cefi-4.6.3/cefi/handler/capitalcom.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.2/cefi/handler/ccxt.py` & `cefi-4.6.3/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.2/cefi/handler/client.py` & `cefi-4.6.3/cefi/handler/client.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.2/cefi/handler/ctrader.py` & `cefi-4.6.3/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.2/cefi/handler/ib_sync.py` & `cefi-4.6.3/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.2/cefi/main.py` & `cefi-4.6.3/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.6.2/pyproject.toml` & `cefi-4.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.6.2"
+version = "4.6.3"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -161,14 +161,15 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
@@ -269,19 +270,20 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "7.3.1"
+sphinx = "7.3.6"
 pydata-sphinx-theme = "^0.15.0"
 sphinx-hoverxref = "^1.3.0"
 sphinx_copybutton = "0.5.2"
 myst_parser = "^2.0.0"
 sphinx_design = "^0.5.0"
```

### Comparing `cefi-4.6.2/PKG-INFO` & `cefi-4.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.6.2
+Version: 4.6.3
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.6.2 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.6.3 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

