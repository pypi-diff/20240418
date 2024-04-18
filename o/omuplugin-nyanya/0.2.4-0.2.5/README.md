# Comparing `tmp/omuplugin_nyanya-0.2.4.tar.gz` & `tmp/omuplugin_nyanya-0.2.5.tar.gz`

## Comparing `omuplugin_nyanya-0.2.4.tar` & `omuplugin_nyanya-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.4/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.4/src/omuplugin_nyanya/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.4/src/omuplugin_nyanya/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.4/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.4/README.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/src/omuplugin_nyanya/__init__.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/src/omuplugin_nyanya/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/README.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 omuplugin_nyanya-0.2.5/PKG-INFO
```

### Comparing `omuplugin_nyanya-0.2.4/src/omuplugin_nyanya/plugin.py` & `omuplugin_nyanya-0.2.5/src/omuplugin_nyanya/plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 }
 
 
 async def translate(component: content.Component) -> content.Component:
     for child in component.iter():
         if not isinstance(child, content.Text):
             continue
-        child.text = "".join(replaces.get(char, char) for char in child.text)
+        child.text = child.text.translate(str.maketrans(replaces))
     return component
 
 
 @client.chat.messages.proxy
 async def on_message_add(message: model.Message) -> model.Message:
     if not message.content:
         return message
```

### Comparing `omuplugin_nyanya-0.2.4/pyproject.toml` & `omuplugin_nyanya-0.2.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_nyanya"
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

