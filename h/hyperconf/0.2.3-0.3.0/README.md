# Comparing `tmp/hyperconf-0.2.3.tar.gz` & `tmp/hyperconf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperconf-0.2.3.tar", max compression
+gzip compressed data, was "hyperconf-0.3.0.tar", max compression
```

## Comparing `hyperconf-0.2.3.tar` & `hyperconf-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-11-02 08:29:27.135950 hyperconf-0.2.3/LICENSE
--rw-r--r--   0        0        0     2027 2024-01-15 14:47:22.059295 hyperconf-0.2.3/README.md
--rw-r--r--   0        0        0      143 2023-11-28 14:18:28.420747 hyperconf-0.2.3/hyperconf/__init__.py
--rw-r--r--   0        0        0     7305 2024-01-15 10:06:45.998565 hyperconf-0.2.3/hyperconf/_lan.g
--rw-r--r--   0        0        0      578 2024-01-15 13:58:57.764742 hyperconf-0.2.3/hyperconf/builtins.yaml
--rw-r--r--   0        0        0     8754 2024-01-25 12:22:46.520444 hyperconf-0.2.3/hyperconf/config.py
--rw-r--r--   0        0        0    17036 2024-01-25 12:22:46.520696 hyperconf-0.2.3/hyperconf/dsl.py
--rw-r--r--   0        0        0     3973 2023-11-28 14:18:28.422137 hyperconf-0.2.3/hyperconf/errors.py
--rw-r--r--   0        0        0      523 2024-01-25 12:22:46.520918 hyperconf-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 hyperconf-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-11-02 08:29:27.135950 hyperconf-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2020 2024-04-18 15:03:29.068311 hyperconf-0.3.0/README.md
+-rw-r--r--   0        0        0      216 2024-04-18 14:55:12.306209 hyperconf-0.3.0/hyperconf/__init__.py
+-rw-r--r--   0        0        0      633 2024-04-18 14:55:12.306464 hyperconf-0.3.0/hyperconf/builtins.yaml
+-rw-r--r--   0        0        0     8494 2024-04-18 14:55:12.306755 hyperconf-0.3.0/hyperconf/config.py
+-rw-r--r--   0        0        0    18841 2024-04-18 14:55:12.307055 hyperconf-0.3.0/hyperconf/dsl.py
+-rw-r--r--   0        0        0     4218 2024-04-18 14:55:12.307489 hyperconf-0.3.0/hyperconf/errors.py
+-rw-r--r--   0        0        0     2093 2024-04-18 14:55:12.307815 hyperconf-0.3.0/hyperconf/mapping.py
+-rw-r--r--   0        0        0      523 2024-04-18 15:07:17.280565 hyperconf-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 hyperconf-0.3.0/PKG-INFO
```

### Comparing `hyperconf-0.2.3/LICENSE` & `hyperconf-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperconf-0.2.3/README.md` & `hyperconf-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,68 +2,66 @@
 
 [![Build Status](https://travis-ci.org/your-username/hyperconfig.svg?branch=main)](https://travis-ci.org/rchindris/hyperconfig)
 [![PyPI version](https://badge.fury.io/py/hyperconfig.svg)](https://badge.fury.io/py/hyperconfig)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 ## Overview
 
-HyperConfig is a Python library for creating schema-based configuration. 
-It allows zero code configuration definition where both the structure and the 
-configuration values are validated using YAML based schema definition files.
+HyperConfig is a Python library for creating schema-based configuration files.
+It automatically parses parses, validates and converts configuration objects 
+according to a predefined configuration schema.
 
 
 Advantages:
 
 - less code: define the structure in YAML, validate and load configs using a one-liner.
 - shared schemas: define once, use in multiple projects.
 - extensibility: add configuration types and validation rules without coding.
 
 ## Installation
 
 ```bash
-pip install hyperconfig
+pip install hyperconf
 
 ```
 
 ## Usage
 
 Define your schema in a definition file, `ships.yaml`:
 
 ``` yaml
-# Spaceship Configuration Schema
-
-ship_type:
-  type: str
-  validator: hval.isalpha()
-  required: true
-
-shipcolor:
-  type: str
-  validator: hval.lower() in ['red', 'blue', 'green', 'yellow', 'gray']
-  required: true
-
-enginepower:
-  type: int
-  validator: 100 <= hval <= 1000
-  required: true
-
-shieldlevel:
-  type: float
-  validator:  0.0 <= hval <= 1.0
-  required: true
-
-ship:
-  captain: str
-  crew:
-   type: int
-   validator: hval > 0
-  class: shiptype
-  color: shipcolor
-  shields: shieldlevel
-  engines: enginepower
+  # Spaceship Configuration Schema
+  ship_type:
+    type: str
+    validator: hval.isalpha()
+    required: true
+
+  shipcolor:
+    type: str
+    validator: hval.lower() in ['red', 'blue', 'green', 'yellow', 'gray']
+    required: true
+
+  enginepower:
+    type: int
+    validator: 100 <= hval <= 1000
+    required: true
+
+  shieldlevel:
+    type: percent
+    required: true
+
+  ship:
+    captain: str
+    crew:
+      type: int
+      validator: hval > 0
+    class: shiptype
+    color: shipcolor
+    shields: shieldlevel
+    engines: enginepower
 ```
 
 Then use the schema to create configuration values, `gameconfig.yaml`:
 
 ``` yaml
 use: ships
```

### Comparing `hyperconf-0.2.3/hyperconf/config.py` & `hyperconf-0.3.0/hyperconf/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,62 +163,60 @@
         self.__def__ = hdef
 
         # Scan the entire file for use directives and
         # load referred definitions.
         objs = []
         for decl_name, val in config_values.items():
             if decl_name == dsl.Keywords.use:
-                dsl.ConfigDefs.parse_yaml(val, 0, fname)
+                dsl.ConfigDefs.parse_yaml(val, ref_file=fname)
             else:
                 objs.append((decl_name, val))
 
         # Parse objects
         for decl_name, val in objs:
             ident, htype = dsl.HyperDef.infer_type(decl_name, val, hdef)
+
             if htype is None:
                 raise err.UndefinedTagError(ident, self._line)
 
+            # handle dict, list or atomic options
             if isinstance(val, dict):
+                # set default option values.
+                htype.set_defaults(val)
+
                 htype.validate(val, self._line, self._file)
                 self.update({
                     ident: HyperConfig(ident, val, htype,
                                        strict=strict,
                                        line=self._line,
                                        fname=self._file)
                 })
             elif isinstance(val, list):
-                # Require that all list elements are of type
-                # dict or other lists.
-                # if any(type(_) != dict and type(_) != list for _ in val):
-                #     raise err.ConfigurationError(
-                #         "List options must contain elements of type dict or list "
-                #         f"(in list for option {decl_name})",
-                #         line=self._line,
-                #         fname=self._file)
-
                 elems = []
 
                 for elem in val:
                     if isinstance(elem, dict):
                         elem_id, elem_decl = next(iter(elem.items()))
 
                         htype.validate(elem_decl, self._line, self._file)
+
                         elems.append(HyperConfig(
                             elem_id, elem_decl, htype,
                             strict=strict,
                             line=self._line,
                             fname=self._file
                         ))
                     else:
                         htype.validate(elem, self._line, self._file)
                         elems.append(elem)
                 self.update({
                     ident: elems
                 })
             else:
+                htype.validate(val, self._line, self._file)
                 self.update({ident: htype.convert(val)})
 
     def __getattr__(self, attr: str):
         """Return attribute value."""
         if attr is None:
             raise ValueError("attr is None")
         if attr not in self:
```

### Comparing `hyperconf-0.2.3/hyperconf/dsl.py` & `hyperconf-0.3.0/hyperconf/dsl.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,18 +37,19 @@
 class Keywords:
     """Define reserved keys."""
 
     validator = "validator"
     converter = "converter"
     typename = "type"
     required = "required"
+    default = "default"
     allow_multiple = "allow_many"
     line = "__line__"
     use = "use"
-    HDef = [validator, converter, typename, required, allow_multiple]
+    HDef = [validator, converter, typename, required, allow_multiple, default]
 
 
 class HyperDef:
     """Provide type attributes."""
 
     @staticmethod
     def parse(tname: str, tdef: dict, fname: str = None):
@@ -68,15 +69,15 @@
         :class:`Keywords.typename` and infers that the configuration object type
         name is the found value if it exists, or the specified argument `tname`
         if not. It also checks that :class:`Keywords.required` and
         :class:`Keywords.validator` exist and t
         The method then treats the rest of the dictionary keys as option specifiers.
         Each option must be of a previously defined type.
         Nesting definitions is not allowed.
-        
+
         Example(s):
         >>> hyper_def.parse('nat', {
         ...     'validator': "hval >= 0"
         ... })
         >>> hyper_def.parse('mongo_db', {
         ...     "hostname": {
         ...         "_typename": "str",
@@ -101,14 +102,15 @@
         if _tdef is None or not isinstance(_tdef, dict):
             raise ValueError("tdef must be a dictionary")
 
         type_name = _tdef.get(Keywords.typename, tname)
         is_required = _tdef.get(Keywords.required, False)
         validator = _tdef.get(Keywords.validator, None)
         converter = _tdef.get(Keywords.converter, None)
+        default = _tdef.get(Keywords.default, None)
 
         for k in Keywords.HDef:
             if k in _tdef:
                 del _tdef[k]
 
         # Parse options.
         opts = []
@@ -135,37 +137,39 @@
                             message="Invalid option definition: "
                             f"found unexpected key '{akey}'. "
                             "Please note that nesting definitions is "
                             "not allowed.")
                 opts.append(HyperDef(
                     name=aname,
                     typename=aval.get(Keywords.typename, str),
-                    required=aval.get(Keywords.required, True),
+                    required=aval.get(Keywords.required, False),
                     validator=aval.get(Keywords.validator, None),
                     converter=aval.get(Keywords.converter, None),
+                    default=aval.get(Keywords.default, None),
                     line=opt_line,
                     fpath=fname))
             else:
                 opts.append(HyperDef(name=aname, typename=aval))
 
         return HyperDef(name=tname,
                         typename=type_name,
                         required=is_required,
                         validator=validator,
                         converter=converter,
+                        default=default,
                         options=opts)
 
     @staticmethod
     def infer_type(decl_tag: str, decl: str = None, hdef = None):
         """Determine the definition for the given tag.
 
         A declaration has the syntax
-        
+
          decl_name[=def_name]: ...
-           
+
         If def_name is specified then the decl_name can be any valid
         identifier, otherwise decl_name designates the definition to use,
         e.g.:
 
         database_config:
         ...
         database_config1=database_config:
@@ -196,24 +200,25 @@
             opt = [o for o_name, o in hdef.options.items() if o.name == ident]
             if opt:
                 htype = opt[0].typename
 
         if not htype:
             # Default to the actual datatype.
             htype = decl.__class__.__name__
-            
+
         return ident, ConfigDefs.get(htype) if htype else None
 
     def __init__(self, name,
                  typename=None,
                  line: int = -1,
                  fpath: str = None,
                  required: bool = False,
                  validator: str = None,
                  converter: str = None,
+                 default: str = None,
                  allow_multiple_values: bool = False,
                  options: t.List = []):
         """ Initialize a configuration object definition.
 
         :param name:
          the object name. Must start with a letter or '_' and
          cannot contain whitespace and special characters.
@@ -225,73 +230,100 @@
         :param file:
          the path to the file containing this definition.
         :param line:
          the line at which the definition is specified.
         """
         self.name = name
         self.typename = typename
-        self.requiredred = required
+        self.required = required
         self.def_file = fpath
         self.line = line
-        self._validator = validator
-        self._converter = converter
+        self.validator = validator
+        self.converter = converter
+        self.default = default
         self.options = {o.name: o for o in options}
         self.allow_multiple_values = allow_multiple_values
 
     def __repr__(self):
         """Debug str representation."""
         return f"({self.name} "\
             f"{list(self.options.keys())})"
 
-    def validate(self, decl: dict, line: int=0, filename: str = None):
-        """Validate the structure and values from declaration."""
-        if not self._validator:
-            return True
+    def set_defaults(self, decl: dict, in_place: bool = True):
+        """Set default values for unspecified options.
+
+        This function only adds options and their default values
+        if the option is not 'required'.
+        Args:
+        decl (dict): the configuation object declaration.
+        in_place (bool): if True add the missing options to the
+         decl dict, if False return a new dictionary.
+        """
+        if decl is None:
+            raise ValueError("decl is None")
+        if not isinstance(decl, dict):
+            raise ValueError("expecting a dict instance for decl")
+
+        opts = decl if in_place else decl.copy()
+        for opt_name, opt in self.options.items():
+            if opt.required:
+                continue
+            if opt_name not in opts:
+                opts[opt_name] = opt.default
 
+        return opts
+
+
+    def validate(self, decl: dict, line: int=0, filename: str=None):
+        """Validate the structure and values from declaration."""
         # validate structure
         if type(decl) is dict:
             decl_opts = list(decl.keys())
-            
+            if Keywords.line in decl_opts:
+                decl_opts.remove(Keywords.line)
+
             # any required opt not specified => error
             for opt_name, opt in self.options.items():
-                if not opt_name in decl_opts and opt.is_required:
+                if opt_name in decl_opts:
+                    decl_opts.remove(opt_name)
+                elif opt.required:
                     raise err.ConfigurationError(
                         f"Missing required option {opt}",
-                        line=decl.line, fname=filename
-                    )
-                decl_opts.remove(opt_name)
+                        line=line, fname=filename)
+
 
             # check if remaining are valid opt names
             if any([opt not in self.options.keys()
                     for opt in decl_opts]):
                 opt_names = [o for o in decl_opts
                              if not o in self.options]
                 raise err.ConfigurationError(
                     f"Unkown options {opt_names} for definition {self}.",
                     line=line,
-                    filename=filename
+                    fname=filename
                 )
 
         is_valid = True
         err_msg = None
+
         try:
             context = _eval_imports.copy()
             context.update({
                 "htype": self,
                 "hval": decl,
             })
             val_result = eval(
-                self._validator,
+                self.validator,
                 context
             )
             if isinstance(val_result, tuple):
                 is_valid, err_msg = val_result
             else:
                 is_valid = val_result
-                
+
             # Consider only bool values for False.
             if not is_valid and\
                not isinstance(is_valid, bool):
                 is_valid = True
         except Exception as e:
             err_msg = e
 
@@ -299,29 +331,29 @@
             raise err.ConfigurationError(
                 f"Invalid configuration value '{decl}' "
                 f"for type {self} "
                 f"{': ' + (str(err_msg) if err_msg else '')}",
                 line=line,
                 fname=filename
             )
-        
+
     def convert(self, decl, line: int=0, filename: str = None):
         """Convert option value."""
         if decl is None:
             raise ValueError("decl is None")
-        if not self._converter:
+        if not self.converter:
             return decl
         try:
             context = _eval_imports.copy()
             context.update({
                 "htype": self,
                 "hval": decl,
             })
             res = eval(
-                self._converter,
+                self.converter,
                 context
             )
             return res
         except Exception as e:
             raise err.ConfigurationError(
                 f"Could not convert value '{decl}' "
                 f"for type {self}: {e}",
@@ -330,28 +362,30 @@
             )
 
 
 class ConfigDefs:
     """Template definition parser and type registry."""
 
     _typedefs = {}
+    _loaded_files = []
+    _search_packages = [__name__.split(".")[0]]
 
     @staticmethod
     def add(hdefs):
         """Register a definition or list of definitions.
 
         :param hdefs:
           definition or a collection of definitions.
         """
         if hdefs is None:
             raise ValueError("hdefs is None")
         if not isinstance(hdefs, list):
             hdefs = [hdefs]
 
-        for hdef in hdefs:            
+        for hdef in hdefs:
             if hdef.name in ConfigDefs._typedefs:
                 raise err.DuplicateDefError(
                     ConfigDefs._typedefs[hdef.name], hdef
                 )
             ConfigDefs._typedefs[hdef.name] = hdef
 
     @staticmethod
@@ -375,14 +409,26 @@
     @staticmethod
     def clear():
         """Remove all known type bindings."""
         ConfigDefs._typedefs.clear()
         ConfigDefs._loaded_files.clear()
 
     @staticmethod
+    def add_package(package_name: str):
+        """Add a package to the def search path.
+
+        Args:
+        package_name (str): a Python package name.
+        """
+        if package_name is None:
+            raise ValueError("package_name is None")
+        if not package_name in ConfigDefs._search_packages:
+            ConfigDefs._search_packages.append(package_name)
+
+    @staticmethod
     def parse_dict(defs: t.Dict, fname: str = None):
         """Parse type definitions.
 
         :param defs: a dictionary containing type structure
         information (as nested dictionaries).
 
         :return: a list of :class:TypeDef definitions.
@@ -432,50 +478,59 @@
         return typedefs
 
     @staticmethod
     def load_builtins():
         """Load built-in types."""
         ConfigDefs.parse_yaml("builtins")
 
-    _loaded_files = []
+
     @staticmethod
-    def parse_yaml(template_path: str, line: int = 0, ref_file: str = None):
+    def parse_yaml(template_path: str,
+                   line: int = 0, ref_file: str = None):
         """Load definitions from path.
 
         :param template_path:
         the path to the template file. It can be an absolute path,
         a relative path to the current working directory or a
         package resource.
         :param line:
         the line at which the use directive occurs.
         :param ref_file:
         the file that contains the use directive.
         """
+        if template_path is None:
+            raise ValueError("template_path is None")
         if not template_path.endswith(".yaml"):
             template_path = template_path + ".yaml"
 
-        template_path = Path(template_path) if \
-            isinstance(template_path, str) else template_path
+        template_path = Path(template_path)
 
         if not template_path.exists():
-            # Search for a packaged resource
-            # having the same name (predefined template).
-            pkg_files = resources.files("hyperconf")
-            template_path = pkg_files / template_path.name
+            # File not found. Search for a package resource
+            # in one of the packages listed in _search_path.
+            found_in_package = False
+
+            for package_name in ConfigDefs._search_packages:
+                pkg_files = resources.files(package_name)
+
+                package_path = pkg_files / template_path.name
+                if package_path.exists():
+                    found_in_package = True
+                    template_path = package_path
 
-            if not template_path.exists():
+            if not found_in_package:
                 raise err.TemplateDefinitionError(
                     name=Keywords.use,
                     message=f"Failed to load template '{template_path}'. "
                     "Could not find a file or a resource with that name.",
                     line=line,
                     config_path=ref_file)
 
-        if template_path not in ConfigDefs._loaded_files:
-            ConfigDefs._loaded_files.append(template_path)
+        if not template_path.as_posix() in ConfigDefs._loaded_files:
+            ConfigDefs._loaded_files.append(template_path.as_posix())
             with open(template_path) as tfile:
                 try:
                     return ConfigDefs.parse_dict(
                         yaml.load(tfile, Loader=_LineInfoLoader),
                         fname=template_path.as_posix()
                     )
                 except yaml.scanner.ScannerError as e:
```

### Comparing `hyperconf-0.2.3/hyperconf/errors.py` & `hyperconf-0.3.0/hyperconf/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Define custom hyperconf exceptions."""
-
+from typing import Type
 
 class HyperConfError(Exception):
     """Base exception class for HyperConf package."""
 
     def __init__(self, message: str,
                  line: int = None, config_path: str = None):
         """Initialize a Hyperconf exception.
@@ -121,7 +121,14 @@
                  fname: str = None):
         """Initialize an InvalidYamlError.
 
         Args:
         message (str): the error message.
         """
         super().__init__(message, line, fname)
+
+
+class DuplicateMappingError(HyperConfError):
+    """Signals that a tag is already mapped to a class."""
+
+    def __init__(self, tag: str, cls: Type):
+        super().__init__(f"the tag {tag} is already mapped to {cls}")
```

### Comparing `hyperconf-0.2.3/pyproject.toml` & `hyperconf-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperconf"
-version = "0.2.3"
+version = "0.3.0"
 description = "YAML-based configuration library, featuring zero-code validation and parsing."
 authors = ["Radu Chindris <radu.chindris@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `hyperconf-0.2.3/PKG-INFO` & `hyperconf-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperconf
-Version: 0.2.3
+Version: 0.3.0
 Summary: YAML-based configuration library, featuring zero-code validation and parsing.
 License: MIT
 Author: Radu Chindris
 Author-email: radu.chindris@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,68 +18,66 @@
 
 [![Build Status](https://travis-ci.org/your-username/hyperconfig.svg?branch=main)](https://travis-ci.org/rchindris/hyperconfig)
 [![PyPI version](https://badge.fury.io/py/hyperconfig.svg)](https://badge.fury.io/py/hyperconfig)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 ## Overview
 
-HyperConfig is a Python library for creating schema-based configuration. 
-It allows zero code configuration definition where both the structure and the 
-configuration values are validated using YAML based schema definition files.
+HyperConfig is a Python library for creating schema-based configuration files.
+It automatically parses parses, validates and converts configuration objects 
+according to a predefined configuration schema.
 
 
 Advantages:
 
 - less code: define the structure in YAML, validate and load configs using a one-liner.
 - shared schemas: define once, use in multiple projects.
 - extensibility: add configuration types and validation rules without coding.
 
 ## Installation
 
 ```bash
-pip install hyperconfig
+pip install hyperconf
 
 ```
 
 ## Usage
 
 Define your schema in a definition file, `ships.yaml`:
 
 ``` yaml
-# Spaceship Configuration Schema
-
-ship_type:
-  type: str
-  validator: hval.isalpha()
-  required: true
-
-shipcolor:
-  type: str
-  validator: hval.lower() in ['red', 'blue', 'green', 'yellow', 'gray']
-  required: true
-
-enginepower:
-  type: int
-  validator: 100 <= hval <= 1000
-  required: true
-
-shieldlevel:
-  type: float
-  validator:  0.0 <= hval <= 1.0
-  required: true
-
-ship:
-  captain: str
-  crew:
-   type: int
-   validator: hval > 0
-  class: shiptype
-  color: shipcolor
-  shields: shieldlevel
-  engines: enginepower
+  # Spaceship Configuration Schema
+  ship_type:
+    type: str
+    validator: hval.isalpha()
+    required: true
+
+  shipcolor:
+    type: str
+    validator: hval.lower() in ['red', 'blue', 'green', 'yellow', 'gray']
+    required: true
+
+  enginepower:
+    type: int
+    validator: 100 <= hval <= 1000
+    required: true
+
+  shieldlevel:
+    type: percent
+    required: true
+
+  ship:
+    captain: str
+    crew:
+      type: int
+      validator: hval > 0
+    class: shiptype
+    color: shipcolor
+    shields: shieldlevel
+    engines: enginepower
 ```
 
 Then use the schema to create configuration values, `gameconfig.yaml`:
 
 ``` yaml
 use: ships
```

