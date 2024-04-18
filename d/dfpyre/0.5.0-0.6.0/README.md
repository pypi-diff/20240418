# Comparing `tmp/dfpyre-0.5.0.tar.gz` & `tmp/dfpyre-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfpyre-0.5.0.tar", max compression
+gzip compressed data, was "dfpyre-0.6.0.tar", max compression
```

## Comparing `dfpyre-0.5.0.tar` & `dfpyre-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1060 2024-02-25 02:05:19.117008 dfpyre-0.5.0/LICENSE
--rw-r--r--   0        0        0     9463 2024-03-22 02:43:18.730959 dfpyre-0.5.0/README.md
--rw-r--r--   0        0        0       25 2024-02-25 02:05:19.117008 dfpyre-0.5.0/dfpyre/__init__.py
--rw-r--r--   0        0        0    30347 2024-02-25 02:05:19.117008 dfpyre-0.5.0/dfpyre/data/data.json
--rw-r--r--   0        0        0     7688 2024-03-22 02:26:03.719216 dfpyre-0.5.0/dfpyre/items.py
--rw-r--r--   0        0        0    13805 2024-03-22 02:33:23.064565 dfpyre-0.5.0/dfpyre/pyre.py
--rw-r--r--   0        0        0      980 2024-03-22 02:24:32.576925 dfpyre-0.5.0/dfpyre/style.py
--rw-r--r--   0        0        0      488 2024-03-22 03:14:36.399992 dfpyre-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    10142 1970-01-01 00:00:00.000000 dfpyre-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-17 21:20:51.864329 dfpyre-0.6.0/LICENSE
+-rw-r--r--   0        0        0    10665 2024-04-18 01:13:01.761353 dfpyre-0.6.0/README.md
+-rw-r--r--   0        0        0       25 2024-02-25 02:05:19.117008 dfpyre-0.6.0/dfpyre/__init__.py
+-rw-r--r--   0        0        0    30347 2024-02-25 02:05:19.117008 dfpyre-0.6.0/dfpyre/data/data.json
+-rw-r--r--   0        0        0     9215 2024-04-17 20:33:13.377155 dfpyre-0.6.0/dfpyre/items.py
+-rw-r--r--   0        0        0    16970 2024-04-17 20:38:50.169866 dfpyre-0.6.0/dfpyre/pyre.py
+-rw-r--r--   0        0        0     5450 2024-04-17 20:34:34.634288 dfpyre-0.6.0/dfpyre/scriptgen.py
+-rw-r--r--   0        0        0      980 2024-03-22 02:24:32.576925 dfpyre-0.6.0/dfpyre/style.py
+-rw-r--r--   0        0        0      488 2024-04-18 00:35:46.594471 dfpyre-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    11344 1970-01-01 00:00:00.000000 dfpyre-0.6.0/PKG-INFO
```

### Comparing `dfpyre-0.5.0/LICENSE` & `dfpyre-0.6.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Amp
+Copyright (c) 2024 Amp
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dfpyre-0.5.0/README.md` & `dfpyre-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 ## Functions and Procedures
 
 - [Creating Functions and Processes](#creating-functions-and-processes)
 - [Calling Functions and Processes](#calling-functions-and-processes)
 
 ## Extras
 
+- [Importing from Code](#importing-from-code)
+- [Script Generation](#script-generation)
 - [Method List](#method-list)
 
 ___
 
 ### Setup
 
 To start creating in pyre, you have to create a DFTemplate object like so:
@@ -257,25 +259,26 @@
 ```
 
 ### Particle
 
 Represents a diamondfire particle item:
 
 ```py
-particle(name='Cloud', amount=10, horizontal=1.0, vertical=0.5, x=1.0, y=0.0, z=0.0, motionVariation=100)
+particle({'particle':'Cloud','cluster':{'amount':1,'horizontal':0.0,'vertical':0.0},'data':{'x':1.0,'y':0.0,'z':0.0,'motionVariation':100}})
 ```
 
 Example:
 
 ```py
 # plays a white cloud particle effect at 5, 50, 5
 from dfpyre import *
 t = DFTemplate()
 t.player_event('Join')
-t.player_action('Particle', particle('Cloud'), loc(5, 50, 5))
+part = particle({'particle':'Cloud','cluster':{'amount':1,'horizontal':0.0,'vertical':0.0},'data':{'x':1.0,'y':0.0,'z':0.0,'motionVariation':100}})
+t.player_action('Particle', part, loc(5, 50, 5))
 ```
 
 Currently, the particle object does not support colors.
 
 ### Potion
 
 Represents a diamondfire potion item:
@@ -419,14 +422,39 @@
 
 ```py
 from dfpyre import *
 t = DFTemplate()
 t.player_event('Join')
 t.call_function('doStuff')
 ```
+ 
+### Importing from Code
+
+You can import existing templates from their built code using the `from_code` method:
+
+```py
+from dfpyre import *
+template_code = 'H4sIAGVyIGYC/3WOMQ7CMAxFz4LnDsw5AhITI6qQSaw2IrGrxkJCVe5eh3boAJP9n/Kfs8AziX8VcPcFYgC3Zej26YDexGoZvUZhAxeJ3PI8WMtKSrnV+1q7P4op4Yfmx244qG7E4Uql4EA/jNv2Jc3qJU/2KqBiY4yZjI6UkpzAjkNJouDO1X7S1xUDaGUl2QAAAA=='
+
+t = DFTemplate.from_code(template_code)
+# add onto the template from here
+```
+
+
+### Script Generation
+
+You can also generate an equivalent python script for a template from a template object:
+
+```py
+from dfpyre import *
+template_code = 'H4sIAGVyIGYC/3WOMQ7CMAxFz4LnDsw5AhITI6qQSaw2IrGrxkJCVe5eh3boAJP9n/Kfs8AziX8VcPcFYgC3Zej26YDexGoZvUZhAxeJ3PI8WMtKSrnV+1q7P4op4Yfmx244qG7E4Uql4EA/jNv2Jc3qJU/2KqBiY4yZjI6UkpzAjkNJouDO1X7S1xUDaGUl2QAAAA=='
+
+t = DFTemplate.from_code(template_code)
+t.generate_script('my_template.py')    # generated python script will be written to my_template.py
+```
 
 ### Method List
 
 - Events / Function / Process
   - player_event
   - entity_event
   - function
```

### Comparing `dfpyre-0.5.0/dfpyre/data/data.json` & `dfpyre-0.6.0/dfpyre/data/data.json`

 * *Files identical despite different names*

### Comparing `dfpyre-0.5.0/dfpyre/pyre.py` & `dfpyre-0.6.0/dfpyre/pyre.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """
 A package for externally creating code templates for the DiamondFire Minecraft server.
 
 By Amp
-2/24/2024
 """
 
 import base64
 import gzip
 import json
 import os
 from difflib import get_close_matches
 import datetime
 from typing import Tuple, List, Dict
 from enum import Enum
+import socket
 from mcitemlib.itemlib import Item as NbtItem
 from dfpyre.items import *
+from dfpyre.scriptgen import generate_script, GeneratorFlags
 
 COL_WARN = '\x1b[33m'
 COL_RESET = '\x1b[0m'
 COL_SUCCESS = '\x1b[32m'
 COL_ERROR = '\x1b[31m'
 
 CODEBLOCK_DATA_PATH = os.path.join(os.path.dirname(__file__), 'data/data.json')
 
 VARIABLE_TYPES = {'txt', 'comp', 'num', 'item', 'loc', 'var', 'snd', 'part', 'pot', 'g_val', 'vec', 'pn_el'}
 TEMPLATE_STARTERS = {'event', 'entity_event', 'func', 'process'}
+SINGLE_NAME_CODEBLOCKS = {'func', 'process', 'call_func', 'start_process', 'else'}
 
 TARGETS = ['Selection', 'Default', 'Killer', 'Damager', 'Shooter', 'Victim', 'AllPlayers', 'Projectile', 'AllEntities', 'AllMobs', 'LastEntity']
 TARGET_CODEBLOCKS = {'player_action', 'entity_action', 'if_player', 'if_entity'}
 
 VAR_SHORTHAND_CHAR = '$'
 VAR_SCOPES = {'g': 'unsaved', 's': 'saved', 'l': 'local', 'i': 'line'}
 
@@ -56,14 +58,23 @@
 
 class CodeBlock:
     def __init__(self, name: str, args: Tuple=(), target: Target=DEFAULT_TARGET, data: Dict={}):
         self.name = name
         self.args = args
         self.target = target
         self.data = data
+    
+    def __repr__(self) -> str:
+        if self.name in SINGLE_NAME_CODEBLOCKS:
+            if self.name == 'else':
+                return 'CodeBlock(else)'
+            return f'CodeBlock({self.name}, {self.data["data"]})'
+        elif 'block' in self.data:
+            return f'CodeBlock({self.data["block"]}, {self.name})'
+        return f'CodeBlock(bracket, {self.data["type"]}, {self.data["direct"]})'
 
 
 def _warn(message):
     print(f'{COL_WARN}! WARNING ! {message}{COL_RESET}')
 
 
 def _warn_unrecognized_name(codeblock_type: str, codeblock_name: str):
@@ -104,15 +115,15 @@
 
 def _convert_data_types(args):
     converted_args = []
     for value in args:
         if type(value) in {int, float}:
             converted_args.append(num(value))
         elif type(value) is str:
-            if value[0] == VAR_SHORTHAND_CHAR and value[1] in VAR_SCOPES:
+            if len(value) > 2 and value[0] == VAR_SHORTHAND_CHAR and value[1] in VAR_SCOPES:
                 var_object = var(value[2:], VAR_SCOPES[value[1]])
                 converted_args.append(var_object)
             else:
                 converted_args.append(text(value))
         else:
             converted_args.append(value)
     return tuple(converted_args)
@@ -153,44 +164,48 @@
     return _reformat_codeblock_tags(tags, codeblock_type, codeblock_name)
 
 
 def _build_block(codeblock: CodeBlock, include_tags: bool):
     """
     Builds a properly formatted block from a CodeBlock object.
     """
-    final_block = codeblock.data.copy()
+    built_block = codeblock.data.copy()
     codeblock_type = codeblock.data.get('block')
     
     # add target if necessary ('Selection' is the default when 'target' is blank)
     if codeblock_type in TARGET_CODEBLOCKS and codeblock.target != DEFAULT_TARGET:
-        final_block['target'] = codeblock.target.get_string_value()
+        built_block['target'] = codeblock.target.get_string_value()
     
     # add items into args
     final_args = [arg.format(slot) for slot, arg in enumerate(codeblock.args) if arg.type in VARIABLE_TYPES]
     
     # check for unrecognized name, add tags
     if codeblock_type is not None:  # for brackets
         if codeblock_type not in TAGDATA_EXTRAS_KEYS and codeblock.name not in ALL_CODEBLOCK_NAMES:
             _warn_unrecognized_name(codeblock_type, codeblock.name)
         elif include_tags:
             tags = _get_codeblock_tags(codeblock_type, codeblock.name)
             if len(final_args) + len(tags) > 27:
                 final_args = final_args[:(27-len(tags))]  # trim list if over 27 elements
             final_args.extend(tags)  # add tags to end
     
-    final_block['args'] = {'items': final_args}
-    return final_block
+    built_block['args'] = {'items': final_args}
+    return built_block
 
 
-def _df_encode(jsonString: str) -> str:
+def _df_encode(json_string: str) -> str:
     """
     Encodes a stringified json.
     """
-    encodedString = gzip.compress(jsonString.encode('utf-8'))
-    return base64.b64encode(encodedString).decode('utf-8')
+    encoded_string = gzip.compress(json_string.encode('utf-8'))
+    return base64.b64encode(encoded_string).decode('utf-8')
+
+
+def _df_decode(encoded_string: str) -> str:
+    return gzip.decompress(base64.b64decode(encoded_string)).decode('utf-8')
 
 
 def _get_template_item(template_code: str, name: str, author: str) -> NbtItem:
     now = datetime.datetime.now()
 
     template_item = NbtItem('yellow_shulker_box')
     template_item.set_name(f'&x&f&f&5&c&0&0>> &x&f&f&c&7&0&0{name}')
@@ -207,23 +222,66 @@
         'hypercube:pyre_creation_timestamp': now.timestamp()
     }
     template_item.set_tag('PublicBukkitValues', pbv_tag, raw=True)
 
     return template_item
 
 
+# TODO: 
+# - add inserting codeblocks at any index
 class DFTemplate:
     """
     Represents a DiamondFire code template.
     """
     def __init__(self, name: str=None, author: str='pyre'):
         self.codeblocks: List[CodeBlock] = []
-        self.closebracket = None
+        self.bracket_stack: list[str] = []
         self.name = name
         self.author = author
+    
+
+    def __repr__(self) -> str:
+        return f'DFTemplate(name: {self.name}, author: {self.author}, codeblocks: {len(self.codeblocks)})'
+
+
+    @staticmethod
+    def from_code(template_code: str):
+        """
+        Create a template object from an existing template code.
+        """
+        template_dict = json.loads(_df_decode(template_code))
+        template = DFTemplate()
+        for block_dict in template_dict['blocks']:
+            if 'args' in block_dict:
+                args = []
+                for item_dict in block_dict['args']['items']:
+                    parsed_item = item_from_dict(item_dict['item'])
+                    if parsed_item is not None:
+                        args.append(parsed_item)
+            target = Target(TARGETS.index(block_dict['target'])) if 'target' in block_dict else DEFAULT_TARGET
+
+            codeblock_name = 'bracket'
+            if 'block' in block_dict and block_dict['block'] in SINGLE_NAME_CODEBLOCKS:
+                codeblock_name = block_dict['block']
+            elif 'action' in block_dict:
+                codeblock_name = block_dict['action']
+            codeblock = CodeBlock(codeblock_name, args, target, block_dict)
+            template.codeblocks.append(codeblock)
+        
+        return template
+
+
+    @staticmethod
+    def receive_from_recode():
+        print('Waiting for item to be sent...')
+        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        s.connect(('localhost', 31372))
+        received = s.recv(8192)
+        print(received)
+        s.close()
 
 
     def _set_template_name(self, first_block):
         if self.name is not None:
             return
         if 'data' in first_block:
             self.name = first_block['data']
@@ -233,15 +291,15 @@
             self.name = first_block['block'] + '_' + first_block['action']
 
 
     def build(self, include_tags: bool=True) -> str:
         """
         Build this template.
 
-        :param bool includeTags: If True, include item tags in code blocks. Otherwise omit them.
+        :param bool include_tags: If True, include item tags in code blocks. Otherwise omit them.
         :return: String containing encoded template data.
         """
         template_dict_blocks = [_build_block(codeblock, include_tags) for codeblock in self.codeblocks]
         template_dict = {'blocks': template_dict_blocks}
         first_block = template_dict_blocks[0]
         if first_block['block'] not in TEMPLATE_STARTERS:
             _warn('Template does not start with an event, function, or process.')
@@ -258,28 +316,28 @@
         """
         Builds this template and sends it to DiamondFire automatically.
         
         :param bool includeTags: If True, include item tags in code blocks. Otherwise omit them.
         """
         templateCode = self.build(includeTags)
         templateItem = _get_template_item(templateCode, self.name, self.author)
-        return templateItem.send_to_minecraft(method)
+        return templateItem.send_to_minecraft(method, 'pyre')
     
 
     def clear(self):
         """
         Clears this template's data.
         """
         self.__init__()
     
 
     def _openbracket(self, btype: Literal['norm', 'repeat']='norm'):
-        bracket = CodeBlock('Bracket', data={'id': 'bracket', 'direct': 'open', 'type': btype})
+        bracket = CodeBlock('bracket', data={'id': 'bracket', 'direct': 'open', 'type': btype})
         self.codeblocks.append(bracket)
-        self.closebracket = btype
+        self.bracket_stack.append(btype)
     
 
     # command methods
     def player_event(self, name: str):
         cmd = CodeBlock(name, data={'id': 'block', 'block': 'event', 'action': name})
         self.codeblocks.append(cmd)
     
@@ -287,20 +345,21 @@
     def entity_event(self, name: str):
         cmd = CodeBlock(name, data={'id': 'block', 'block': 'entity_event', 'action': name})
         self.codeblocks.append(cmd)
     
 
     def function(self, name: str, *args):
         args = _convert_data_types(args)
-        cmd = CodeBlock('function', args, data={'id': 'block', 'block': 'func', 'data': name})
+        cmd = CodeBlock('func', args, data={'id': 'block', 'block': 'func', 'data': name})
         self.codeblocks.append(cmd)
     
 
-    def process(self, name: str):
-        cmd = CodeBlock('process', data={'id': 'block', 'block': 'process', 'data': name})
+    def process(self, name: str, *args):
+        args = _convert_data_types(args)
+        cmd = CodeBlock('process', args, data={'id': 'block', 'block': 'process', 'data': name})
         self.codeblocks.append(cmd)
     
 
     def call_function(self, name: str, *args):
         args = _convert_data_types(args)
         cmd = CodeBlock('call_func', args, data={'id': 'block', 'block': 'call_func', 'data': name})
         self.codeblocks.append(cmd)
@@ -379,15 +438,15 @@
         cmd = CodeBlock(name, args, data=data)
         self.codeblocks.append(cmd)
         self._openbracket('repeat')
 
 
     def bracket(self, *args):
         args = _convert_data_types(args)
-        cmd = CodeBlock('Bracket', data={'id': 'bracket', 'direct': 'close', 'type': self.closebracket})
+        cmd = CodeBlock('bracket', data={'id': 'bracket', 'direct': 'close', 'type': self.bracket_stack.pop()})
         self.codeblocks.append(cmd)
     
 
     def control(self, name: str, *args):
         args = _convert_data_types(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'control', 'action': name})
         self.codeblocks.append(cmd)
@@ -398,8 +457,23 @@
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'select_obj', 'action': name})
         self.codeblocks.append(cmd)
     
 
     def set_variable(self, name: str, *args):
         args = _convert_data_types(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'set_var', 'action': name})
-        self.codeblocks.append(cmd)
+        self.codeblocks.append(cmd)
+    
+    
+    def generate_script(self, output_path: str, indent_size: int=4, literal_shorthand: bool=True, var_shorthand: bool=False):
+        """
+        Generate an equivalent python script for this template.
+
+        :param str output_path: The file path to write the script to.
+        :param int indent_size: The multiple of spaces to add when indenting lines.
+        :param bool literal_shorthand: If True, `text` and `num` items will be written as strings and ints respectively.
+        :param bool var_shorthand: If True, all variables will be written using variable shorthand.
+        """
+        flags = GeneratorFlags(indent_size, literal_shorthand, var_shorthand)
+        with open(output_path, 'w') as f:
+            f.write(generate_script(self, flags))
+
```

### Comparing `dfpyre-0.5.0/dfpyre/style.py` & `dfpyre-0.6.0/dfpyre/style.py`

 * *Files identical despite different names*

### Comparing `dfpyre-0.5.0/PKG-INFO` & `dfpyre-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dfpyre
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package for external creation of code templates for the DiamondFire Minecraft server.
 Home-page: https://github.com/Amp63/pyre
 License: MIT
 Keywords: diamondfire,minecraft,template,item
 Author: Amp
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: mcitemlib (>=0.1.2,<0.2.0)
+Requires-Dist: mcitemlib (>=0.2.4,<0.3.0)
 Project-URL: Repository, https://github.com/Amp63/pyre
 Description-Content-Type: text/markdown
 
 # pyre
 
 A package for external creation of code templates for the DiamondFire Minecraft server (mcdiamondfire.com).
 
@@ -66,14 +66,16 @@
 ## Functions and Procedures
 
 - [Creating Functions and Processes](#creating-functions-and-processes)
 - [Calling Functions and Processes](#calling-functions-and-processes)
 
 ## Extras
 
+- [Importing from Code](#importing-from-code)
+- [Script Generation](#script-generation)
 - [Method List](#method-list)
 
 ___
 
 ### Setup
 
 To start creating in pyre, you have to create a DFTemplate object like so:
@@ -275,25 +277,26 @@
 ```
 
 ### Particle
 
 Represents a diamondfire particle item:
 
 ```py
-particle(name='Cloud', amount=10, horizontal=1.0, vertical=0.5, x=1.0, y=0.0, z=0.0, motionVariation=100)
+particle({'particle':'Cloud','cluster':{'amount':1,'horizontal':0.0,'vertical':0.0},'data':{'x':1.0,'y':0.0,'z':0.0,'motionVariation':100}})
 ```
 
 Example:
 
 ```py
 # plays a white cloud particle effect at 5, 50, 5
 from dfpyre import *
 t = DFTemplate()
 t.player_event('Join')
-t.player_action('Particle', particle('Cloud'), loc(5, 50, 5))
+part = particle({'particle':'Cloud','cluster':{'amount':1,'horizontal':0.0,'vertical':0.0},'data':{'x':1.0,'y':0.0,'z':0.0,'motionVariation':100}})
+t.player_action('Particle', part, loc(5, 50, 5))
 ```
 
 Currently, the particle object does not support colors.
 
 ### Potion
 
 Represents a diamondfire potion item:
@@ -437,14 +440,39 @@
 
 ```py
 from dfpyre import *
 t = DFTemplate()
 t.player_event('Join')
 t.call_function('doStuff')
 ```
+ 
+### Importing from Code
+
+You can import existing templates from their built code using the `from_code` method:
+
+```py
+from dfpyre import *
+template_code = 'H4sIAGVyIGYC/3WOMQ7CMAxFz4LnDsw5AhITI6qQSaw2IrGrxkJCVe5eh3boAJP9n/Kfs8AziX8VcPcFYgC3Zej26YDexGoZvUZhAxeJ3PI8WMtKSrnV+1q7P4op4Yfmx244qG7E4Uql4EA/jNv2Jc3qJU/2KqBiY4yZjI6UkpzAjkNJouDO1X7S1xUDaGUl2QAAAA=='
+
+t = DFTemplate.from_code(template_code)
+# add onto the template from here
+```
+
+
+### Script Generation
+
+You can also generate an equivalent python script for a template from a template object:
+
+```py
+from dfpyre import *
+template_code = 'H4sIAGVyIGYC/3WOMQ7CMAxFz4LnDsw5AhITI6qQSaw2IrGrxkJCVe5eh3boAJP9n/Kfs8AziX8VcPcFYgC3Zej26YDexGoZvUZhAxeJ3PI8WMtKSrnV+1q7P4op4Yfmx244qG7E4Uql4EA/jNv2Jc3qJU/2KqBiY4yZjI6UkpzAjkNJouDO1X7S1xUDaGUl2QAAAA=='
+
+t = DFTemplate.from_code(template_code)
+t.generate_script('my_template.py')    # generated python script will be written to my_template.py
+```
 
 ### Method List
 
 - Events / Function / Process
   - player_event
   - entity_event
   - function
```

