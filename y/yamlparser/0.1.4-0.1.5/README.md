# Comparing `tmp/yamlparser-0.1.4.tar.gz` & `tmp/yamlparser-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Source/github/yamlparse/dist/.tmp-emvn4ske/yamlparser-0.1.4.tar", last modified: Wed Mar 27 07:56:59 2024, max compression
+gzip compressed data, was "/mnt/d/Source/github/yamlparse/dist/.tmp-rwxjsa0i/yamlparser-0.1.5.tar", last modified: Wed Apr 17 17:23:46 2024, max compression
```

## Comparing `yamlparser-0.1.4.tar` & `yamlparser-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-03-27 07:56:59.123920 yamlparser-0.1.4/
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)     1559 2023-11-09 10:17:41.000000 yamlparser-0.1.4/LICENSE
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)    13094 2024-03-27 07:56:59.121918 yamlparser-0.1.4/PKG-INFO
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)    12499 2024-03-27 07:51:12.000000 yamlparser-0.1.4/README.md
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)      826 2024-03-27 07:12:50.000000 yamlparser-0.1.4/pyproject.toml
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       16 2023-12-06 12:16:15.000000 yamlparser-0.1.4/requirements.txt
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       38 2024-03-27 07:56:59.123920 yamlparser-0.1.4/setup.cfg
-drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-03-27 07:56:59.107936 yamlparser-0.1.4/yamlparser/
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       98 2024-03-26 16:19:18.000000 yamlparser-0.1.4/yamlparser/__init__.py
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)    11945 2024-03-27 07:55:43.000000 yamlparser-0.1.4/yamlparser/namespace.py
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)     5722 2024-03-26 17:09:56.000000 yamlparser-0.1.4/yamlparser/parser.py
-drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-03-27 07:56:59.119927 yamlparser-0.1.4/yamlparser.egg-info/
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)    13094 2024-03-27 07:56:59.000000 yamlparser-0.1.4/yamlparser.egg-info/PKG-INFO
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)      286 2024-03-27 07:56:59.000000 yamlparser-0.1.4/yamlparser.egg-info/SOURCES.txt
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)        1 2024-03-27 07:56:59.000000 yamlparser-0.1.4/yamlparser.egg-info/dependency_links.txt
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       16 2024-03-27 07:56:59.000000 yamlparser-0.1.4/yamlparser.egg-info/requires.txt
--rwxrwxrwx   0 guenther  (1000) guenther  (1000)       11 2024-03-27 07:56:59.000000 yamlparser-0.1.4/yamlparser.egg-info/top_level.txt
+drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-04-17 17:23:46.260460 yamlparser-0.1.5/
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)     1559 2023-11-09 10:17:41.000000 yamlparser-0.1.5/LICENSE
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)    13094 2024-04-17 17:23:46.259461 yamlparser-0.1.5/PKG-INFO
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)    12499 2024-03-27 07:51:12.000000 yamlparser-0.1.5/README.md
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)      819 2024-04-17 17:11:30.000000 yamlparser-0.1.5/pyproject.toml
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       16 2023-12-06 12:16:15.000000 yamlparser-0.1.5/requirements.txt
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       38 2024-04-17 17:23:46.260460 yamlparser-0.1.5/setup.cfg
+drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-04-17 17:23:46.248458 yamlparser-0.1.5/yamlparser/
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       98 2024-03-26 16:19:18.000000 yamlparser-0.1.5/yamlparser/__init__.py
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)    13188 2024-04-17 17:12:09.000000 yamlparser-0.1.5/yamlparser/namespace.py
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)     6353 2024-04-17 17:09:30.000000 yamlparser-0.1.5/yamlparser/parser.py
+drwxrwxrwx   0 guenther  (1000) guenther  (1000)        0 2024-04-17 17:23:46.257461 yamlparser-0.1.5/yamlparser.egg-info/
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)    13094 2024-04-17 17:23:46.000000 yamlparser-0.1.5/yamlparser.egg-info/PKG-INFO
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)      286 2024-04-17 17:23:46.000000 yamlparser-0.1.5/yamlparser.egg-info/SOURCES.txt
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)        1 2024-04-17 17:23:46.000000 yamlparser-0.1.5/yamlparser.egg-info/dependency_links.txt
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       16 2024-04-17 17:23:46.000000 yamlparser-0.1.5/yamlparser.egg-info/requires.txt
+-rwxrwxrwx   0 guenther  (1000) guenther  (1000)       11 2024-04-17 17:23:46.000000 yamlparser-0.1.5/yamlparser.egg-info/top_level.txt
```

### Comparing `yamlparser-0.1.4/LICENSE` & `yamlparser-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yamlparser-0.1.4/PKG-INFO` & `yamlparser-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlparser
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Package to combine YAML configurations and argument parsing
 Author-email: Manuel Guenther <siebenkopf@googlemail.com>
 Project-URL: Homepage, https://github.com/AIML-IfI/yamlparser
 Project-URL: Bug Tracker, https://github.com/AIML-IfI/yamlparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yamlparser-0.1.4/README.md` & `yamlparser-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `yamlparser-0.1.4/pyproject.toml` & `yamlparser-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yamlparser"
-version = "0.1.4"
-authors = [
-  { name="Manuel Guenther", email="siebenkopf@googlemail.com" },
-]
+version = "0.1.5"
+authors = [{name="Manuel Guenther", email="siebenkopf@googlemail.com"}]
 description = "A Package to combine YAML configurations and argument parsing"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `yamlparser-0.1.4/yamlparser/namespace.py` & `yamlparser-0.1.5/yamlparser/namespace.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,23 @@
         sub_config_key: str
         When the configuration files contain this key, this is interpreted as an additional linked config file.
         """
         self._sub_config_key = sub_config_key
         self.update(config)
         self._modifiable = modifiable
 
+    def clone(self):
+        """Returns a copy of this namespace"""
+        return NameSpace(self.dict())
+
+    def keys(self):
+        """Returns the current list of keys in this namespace"""
+        return self.dict().keys()
+
+
     def add(self, key, config):
         """Adds the given configuration as a sub-namespace.
         This is identical to `self.key = NameSpace(config)`"""
         # adds a different config file into a sub-namespace
         self[key] = NameSpace(config)
 
     def set(self, key, value):
@@ -98,38 +107,60 @@
             raise AttributeError(f"You are trying to overwrite key {key} in a frozen namespace")
         keys = key.split(".")
         if len(keys) > 1:
             getattr(self,keys[0]).set(".".join(keys[1:]), value)
         else:
             self[key] = value
 
+    def delete(self, key):
+        """Removes the given key from this namespace. The key can contain periods, which are parsed into sub-namespaces"""
+        if not self._modifiable:
+            raise AttributeError(f"You are trying to delete key {key} from a frozen namespace")
+
+        keys = key.split(".")
+        if len(keys) > 1:
+            self[keys[0]].delete(".".join(keys[1:]))
+        else:
+            delattr(self, key)
+
     def update(self, config):
         """Updates this namespace with the given configuration. Sub-namespaces will be entirely overwritten, not updated."""
         # Updates this namespace with the given config
         # read from yaml file, if it is a file
         loaded_config = self.load(config)
         # recurse through configuration dictionary to build nested namespaces
         config = {}
         for name, value in loaded_config.items():
-            if isinstance(value, dict):
-                # create sub-config
-                config[name] = NameSpace(value, self._sub_config_key)
-                # check if there is a sub-config file listed
-                if self._sub_config_key in config[name].dict():
-                    # load config file
-                    sub_config = NameSpace(config[name][self._sub_config_key])
-                    if name not in sub_config.dict().keys():
-                        raise ValueError(f"The sub configuration file {sub_config_file_name} does not contain key {name}")
-                    # set this as the config
-                    config[name] = sub_config[name]
-                    # apply any overwrites from this config file
-                    config[name].update({key:value for key,value in loaded_config[name].items() if key != self._sub_config_key})
+            # if the name contains at least one period, we have a nested namespace
+            if "." in name:
+                # split the name into the first part and the rest
+                first, rest = name.split(".", 1)
+                # create a new namespace if not existing
+                if first not in config.keys():
+                    config[first] = NameSpace({})
+                # update the sub-namespace
+                config[first].update({rest:value})
             else:
-                config[name] = value
-        # recurse through namespace and load sub-configurations
+
+                if isinstance(value, dict):
+                    # create sub-config
+                    config[name] = NameSpace(value, self._sub_config_key)
+                    # check if there is a sub-config file listed
+                    if self._sub_config_key in config[name].dict().keys():
+                        # load config file
+                        sub_config = NameSpace(config[name][self._sub_config_key])
+                        if name not in sub_config.dict().keys():
+                            raise ValueError(f"The sub configuration file {config[name][self._sub_config_key]} does not contain key '{name}'")
+                        # set this as the config
+                        config[name] = sub_config[name]
+                        # apply any overwrites from this config file
+                        config[name].update({key:value for key,value in loaded_config[name].items() if key != self._sub_config_key})
+                else:
+                    config[name] = value
+            # recurse through namespace and load sub-configurations
         self.__dict__.update(config)
 
     def freeze(self):
         """Freezes this namespace recursively."""
         # recursively freeze all sub-namespaces
         for value in vars(self).values():
             if isinstance (value, NameSpace):
```

### Comparing `yamlparser-0.1.4/yamlparser/parser.py` & `yamlparser-0.1.5/yamlparser/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 global _config
 _config = None
 
 def config_parser(
         parser=None,
         default_config_files=None,
         infer_types=True,
-        ingnore_keys=[],
+        ignore_keys=[],
         add_config_files=False,
         command_line_options=None,
         store_config=True,
+        auto_format=True,
         sub_config_key="yaml"
     ):
     """Creates or updates an `argparse.ArgumentParser` with the option to load configuration files (YAML).
     These files will be automatically parsed and each configuration will be added as a separate option to the command line.
     After calling this function, the global :py:func:`get_config` will return the loaded configuration.
 
     Arguments:
@@ -37,21 +38,25 @@
     These keys will not be put on the command line as options.
 
     add_config_files: bool
     If selected, the list of configuration files is added to the final configuration under the `configuration_files` list.
 
     command_line_options: list or None
     For debugging purposes, a list of command line options is accepted. This is mainly a debug and test feature.
-    If not present, `sys.agrv[1:]` is selected, as usual.
+    If not present, `sys.argv[1:]` is selected, as usual.
 
     store_config: bool
     If selected (the default), the configuration will be stored in a global object that can be accessed via py:func:`get_config()`.
     Note that, in this case, the configuration is frozen and can no longer be updated (unless unfreeze is called).
     Note further that all string variables are automatically evaluated.
 
+    auto_format: bool
+    If selected (the default), the configuration will be formatted such that {key} values are replaced with the actual values in the configuration.
+    You can later call namespace.format_self() in order to format it.
+
     sub_config_key: str
     When the configuration files contain this key, this is interpreted as an additional linked config file.
 
     Returns:
     namespace: NameSpace
     A namespace object containing all options taken from configuration file and command line.
     """
@@ -81,40 +86,49 @@
 
     # compute the types of the nested configurations
     attributes = namespace.attributes()
 
     # create a parser entry for these types
     if parser is None:
         parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter, usage='%(prog)s configuration_files [options]')
+
+    existing_options = list(parser._option_string_actions.keys())
+
     parser.add_argument("configuration_files", nargs="*", default=default_config_files, help="The configuration files to parse. From the second config onward, it be key=value pairs to create sub-configurations")
 
     for k,v in attributes.items():
-        if k in ingnore_keys: continue
+        if k in ignore_keys: continue
         metavar = k.split(".")[-1].upper()
         option = "--"+k
-        if isinstance(v, list):
+        if option in existing_options:
+            # option was requested in the parser, but we already have this option
+            # in this case, we update the default value with the one read from the config
+            parser._option_string_actions[option].default = v
+        elif isinstance(v, list):
             parser.add_argument(option, metavar=metavar, nargs="+", type=type(v[0]) if infer_types else None, help=f"Overwrite list of values for {k}, default={v}")
         else:
             parser.add_argument(option, metavar=metavar, type=type(v) if infer_types else None, help=f"Overwrite value for {k}, content of configuration file: `{v}`")
 
     # parse arguments again
     args = parser.parse_args(command_line_options)
 
     # overwrite values in config
     for k,v in vars(args).items():
         if add_config_files or k != "configuration_files":
             if v is not None:
                 namespace.set(k,v)
 
+    if auto_format:
+        namespace.format_self()
+
     if store_config:
         global _config
         if _config is not None:
             warnings.warn("The configuration has already been set, overwriting it.")
         _config = namespace
-        _config.format_self()
         _config.freeze()
 
     return namespace
 
 
 def get_config():
     """Returns the global configuration object, which is the result of (the latest call to) py:func:`config_parser`.
```

### Comparing `yamlparser-0.1.4/yamlparser.egg-info/PKG-INFO` & `yamlparser-0.1.5/yamlparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlparser
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Package to combine YAML configurations and argument parsing
 Author-email: Manuel Guenther <siebenkopf@googlemail.com>
 Project-URL: Homepage, https://github.com/AIML-IfI/yamlparser
 Project-URL: Bug Tracker, https://github.com/AIML-IfI/yamlparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

