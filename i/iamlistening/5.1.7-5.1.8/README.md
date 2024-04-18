# Comparing `tmp/iamlistening-5.1.7.tar.gz` & `tmp/iamlistening-5.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-5.1.7.tar", max compression
+gzip compressed data, was "iamlistening-5.1.8.tar", max compression
```

## Comparing `iamlistening-5.1.7.tar` & `iamlistening-5.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2024-04-08 10:29:00.100565 iamlistening-5.1.7/LICENSE
--rw-r--r--   0        0        0     2467 2024-04-08 10:29:00.100565 iamlistening-5.1.7/README.md
--rw-r--r--   0        0        0      113 2024-04-08 10:29:36.036539 iamlistening-5.1.7/iamlistening/__init__.py
--rw-r--r--   0        0        0      443 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/config.py
--rw-r--r--   0        0        0     1824 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/default_settings.toml
--rw-r--r--   0        0        0      548 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/__init__.py
--rw-r--r--   0        0        0     3441 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/client.py
--rw-r--r--   0        0        0      790 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/discord.py
--rw-r--r--   0        0        0      668 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/guilded.py
--rw-r--r--   0        0        0      834 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/lemmy.py
--rw-r--r--   0        0        0     1281 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/mastodon.py
--rw-r--r--   0        0        0     1413 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/matrix.py
--rw-r--r--   0        0        0      698 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/revolt.py
--rw-r--r--   0        0        0      899 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/telegram.py
--rw-r--r--   0        0        0      761 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/handler/twitch.py
--rw-r--r--   0        0        0     6600 2024-04-08 10:29:00.104565 iamlistening-5.1.7/iamlistening/main.py
--rw-r--r--   0        0        0     4025 2024-04-08 10:29:36.036539 iamlistening-5.1.7/pyproject.toml
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 iamlistening-5.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-18 05:16:31.547231 iamlistening-5.1.8/LICENSE
+-rw-r--r--   0        0        0     2467 2024-04-18 05:16:31.547231 iamlistening-5.1.8/README.md
+-rw-r--r--   0        0        0      113 2024-04-18 05:17:05.695458 iamlistening-5.1.8/iamlistening/__init__.py
+-rw-r--r--   0        0        0      443 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/config.py
+-rw-r--r--   0        0        0     1824 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0      548 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/__init__.py
+-rw-r--r--   0        0        0     3441 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/client.py
+-rw-r--r--   0        0        0      790 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/discord.py
+-rw-r--r--   0        0        0      668 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/guilded.py
+-rw-r--r--   0        0        0      834 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/lemmy.py
+-rw-r--r--   0        0        0     1281 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/mastodon.py
+-rw-r--r--   0        0        0     1413 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/matrix.py
+-rw-r--r--   0        0        0      698 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/revolt.py
+-rw-r--r--   0        0        0      899 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/telegram.py
+-rw-r--r--   0        0        0      761 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/handler/twitch.py
+-rw-r--r--   0        0        0     6600 2024-04-18 05:16:31.555231 iamlistening-5.1.8/iamlistening/main.py
+-rw-r--r--   0        0        0     4027 2024-04-18 05:17:05.695458 iamlistening-5.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 iamlistening-5.1.8/PKG-INFO
```

### Comparing `iamlistening-5.1.7/LICENSE` & `iamlistening-5.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/README.md` & `iamlistening-5.1.8/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/default_settings.toml` & `iamlistening-5.1.8/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/__init__.py` & `iamlistening-5.1.8/iamlistening/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/client.py` & `iamlistening-5.1.8/iamlistening/handler/client.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/discord.py` & `iamlistening-5.1.8/iamlistening/handler/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/guilded.py` & `iamlistening-5.1.8/iamlistening/handler/guilded.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/lemmy.py` & `iamlistening-5.1.8/iamlistening/handler/lemmy.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/mastodon.py` & `iamlistening-5.1.8/iamlistening/handler/mastodon.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/matrix.py` & `iamlistening-5.1.8/iamlistening/handler/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/revolt.py` & `iamlistening-5.1.8/iamlistening/handler/revolt.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/telegram.py` & `iamlistening-5.1.8/iamlistening/handler/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/handler/twitch.py` & `iamlistening-5.1.8/iamlistening/handler/twitch.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/iamlistening/main.py` & `iamlistening-5.1.8/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-5.1.7/pyproject.toml` & `iamlistening-5.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "5.1.7"
+version = "5.1.8"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix",
@@ -32,15 +32,15 @@
 py-cord= "2.5.0"
 simplematrixbotlib= "2.10.3"
 rocketchat-API= "1.32.0"
 "Mastodon.py" = "1.8.1"
 beautifulsoup4 = "4.12.3"
 "guilded.py" = "1.13.0"
 "revolt.py" = "0.2.0"
-pythorhead = {version ="0.23.1", python = ">=3.10,<3.12"}
+pythorhead = {version ="0.24.0", python = ">=3.10,<3.12"}
 twitchio = "2.9.1"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = ">=8.0.8"
 ruff = "^0.3.0"
 black = "^24.0.0"
 pre-commit = "^3.3.1"
@@ -133,14 +133,15 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
@@ -202,19 +203,20 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "7.2.6"
+sphinx = "7.3.6"
 pydata-sphinx-theme = "^0.15.0"
 sphinx-hoverxref = "^1.3.0"
 sphinx_copybutton = "0.5.2"
 myst_parser = "^2.0.0"
 sphinx_design = "^0.5.0"
```

### Comparing `iamlistening-5.1.7/PKG-INFO` & `iamlistening-5.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 5.1.7
+Version: 5.1.8
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Mastodon.py (==1.8.1)
 Requires-Dist: beautifulsoup4 (==4.12.3)
 Requires-Dist: dynaconf (>=3.1.12)
 Requires-Dist: guilded.py (==1.13.0)
 Requires-Dist: loguru (>=0.6.0)
 Requires-Dist: py-cord (==2.5.0)
-Requires-Dist: pythorhead (==0.23.1) ; python_version >= "3.10" and python_version < "3.12"
+Requires-Dist: pythorhead (==0.24.0) ; python_version >= "3.10" and python_version < "3.12"
 Requires-Dist: revolt.py (==0.2.0)
 Requires-Dist: rocketchat-API (==1.32.0)
 Requires-Dist: simplematrixbotlib (==2.10.3)
 Requires-Dist: telethon (==1.34.0)
 Requires-Dist: twitchio (==2.9.1)
 Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/iamlistening/issues
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 5.1.7 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 5.1.8 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: Mastodon.py (==1.8.1) Requires-Dist:
 beautifulsoup4 (==4.12.3) Requires-Dist: dynaconf (>=3.1.12) Requires-Dist:
 guilded.py (==1.13.0) Requires-Dist: loguru (>=0.6.0) Requires-Dist: py-cord
-(==2.5.0) Requires-Dist: pythorhead (==0.23.1) ; python_version >= "3.10" and
+(==2.5.0) Requires-Dist: pythorhead (==0.24.0) ; python_version >= "3.10" and
 python_version < "3.12" Requires-Dist: revolt.py (==0.2.0) Requires-Dist:
 rocketchat-API (==1.32.0) Requires-Dist: simplematrixbotlib (==2.10.3)
 Requires-Dist: telethon (==1.34.0) Requires-Dist: twitchio (==2.9.1) Project-
 URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/iamlistening/issues Project-
 URL: Support, https://github.com/mraniki/iamlistening/discussions Description-
 Content-Type: text/markdown
```

