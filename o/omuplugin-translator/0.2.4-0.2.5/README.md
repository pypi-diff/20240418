# Comparing `tmp/omuplugin_translator-0.2.4.tar.gz` & `tmp/omuplugin_translator-0.2.5.tar.gz`

## Comparing `omuplugin_translator-0.2.4.tar` & `omuplugin_translator-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/src/omuplugin_translator/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/src/omuplugin_translator/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/src/omuplugin_translator/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/src/omuplugin_translator/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.5/PKG-INFO
```

### Comparing `omuplugin_translator-0.2.4/src/omuplugin_translator/plugin.py` & `omuplugin_translator-0.2.5/src/omuplugin_translator/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,69 @@
 from __future__ import annotations
 
-from edgetrans import EdgeTranslator, Translator
+from typing import TypedDict
+
+from edgetrans import EdgeTranslator, Language, Translator
+from loguru import logger
 from omu.identifier import Identifier
 from omuchat import App, Client, content, model
 from omuchat.event.event_types import events
 
+IDENTIFIER = Identifier("cc.omuchat", "plugin-translator")
 APP = App(
-    Identifier("cc.omuchat", "plugin-translator"),
+    IDENTIFIER,
     version="0.1.0",
 )
 client = Client(APP)
+
 translator: Translator | None = None
 
 
+class TrasnlatorConfig(TypedDict):
+    active: bool
+    language: Language
+
+
+config = TrasnlatorConfig(active=False, language="ja")
+CONFIG_REGISTRY_TYPE = client.registry.create("config", config)
+
+
+@CONFIG_REGISTRY_TYPE.listen
+async def on_config_change(new_config: TrasnlatorConfig):
+    global config
+    config = new_config
+    logger.info(f"translator config updated: {config}")
+
+
 async def translate(component: content.Component) -> content.Component:
     if not translator:
         return component
     texts = [
         sibling for sibling in component.iter() if isinstance(sibling, content.Text)
     ]
     translated = await translator.translate(
-        [text.text for text in texts if text.text], "ar"
+        [text.text for text in texts if text.text], config["language"]
     )
     for text, (translation, _) in zip(texts, translated):
         text.text = translation
     return component
 
 
 @client.chat.messages.proxy
 async def on_message_add(message: model.Message) -> model.Message:
+    if not config["active"]:
+        return message
     if not message.content:
         return message
     message.content = await translate(message.content)
     return message
 
 
 @client.on(events.ready)
 async def on_ready():
-    global translator
+    global translator, config
+    config = await CONFIG_REGISTRY_TYPE.get()
     translator = await EdgeTranslator.create()
 
 
 if __name__ == "__main__":
     client.run()
```

### Comparing `omuplugin_translator-0.2.4/pyproject.toml` & `omuplugin_translator-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_translator"
-version = "0.2.4"
+version = "0.2.5"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["edgetrans>=0.2.3", "omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

