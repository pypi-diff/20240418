# Comparing `tmp/omuplugin_chat-0.2.4.tar.gz` & `tmp/omuplugin_chat-0.2.5.tar.gz`

## Comparing `omuplugin_chat-0.2.4.tar` & `omuplugin_chat-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/src/omuplugin_chat/__init__.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/src/omuplugin_chat/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/src/omuplugin_chat/__init__.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/src/omuplugin_chat/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 omuplugin_chat-0.2.5/PKG-INFO
```

### Comparing `omuplugin_chat-0.2.4/src/omuplugin_chat/plugin.py` & `omuplugin_chat-0.2.5/src/omuplugin_chat/plugin.py`

 * *Files identical despite different names*

### Comparing `omuplugin_chat-0.2.4/pyproject.toml` & `omuplugin_chat-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_chat"
-version = "0.2.4"
+version = "0.2.5"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

