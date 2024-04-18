# Comparing `tmp/imy-0.2.3.tar.gz` & `tmp/imy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.2.3.tar", max compression
+gzip compressed data, was "imy-0.2.4.tar", max compression
```

## Comparing `imy-0.2.3.tar` & `imy-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.3/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.3/README.md
--rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.3/imy/__init__.py
--rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.3/imy/assets.py
--rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.3/imy/async_utils.py
--rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.3/imy/config.py
--rw-r--r--   0        0        0       66 2024-04-07 17:07:49.466586 imy-0.2.3/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-01 10:37:37.589305 imy-0.2.3/imy/docstrings/models.py
--rw-r--r--   0        0        0    14281 2024-04-01 10:37:37.592638 imy-0.2.3/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8572 2024-04-10 14:07:52.133967 imy-0.2.3/imy/inject.py
--rw-r--r--   0        0        0    13613 2024-04-10 14:10:43.230681 imy-0.2.3/imy/logs.py
--rw-r--r--   0        0        0     2167 2024-04-11 21:48:52.558560 imy-0.2.3/imy/package_metadata.py
--rw-r--r--   0        0        0      754 2024-04-12 07:06:15.658576 imy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.4/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.4/imy/__init__.py
+-rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.4/imy/assets.py
+-rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.4/imy/async_utils.py
+-rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.4/imy/config.py
+-rw-r--r--   0        0        0       71 2024-04-18 06:50:34.243007 imy-0.2.4/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     5072 2024-04-18 07:34:38.648724 imy-0.2.4/imy/docstrings/data_models.py
+-rw-r--r--   0        0        0    16728 2024-04-18 07:37:22.300844 imy-0.2.4/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8572 2024-04-10 14:07:52.133967 imy-0.2.4/imy/inject.py
+-rw-r--r--   0        0        0    13613 2024-04-10 14:10:43.230681 imy-0.2.4/imy/logs.py
+-rw-r--r--   0        0        0     2167 2024-04-11 21:48:52.558560 imy-0.2.4/imy/package_metadata.py
+-rw-r--r--   0        0        0      754 2024-04-18 18:57:24.091110 imy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.4/PKG-INFO
```

### Comparing `imy-0.2.3/LICENSE` & `imy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.2.3/imy/assets.py` & `imy-0.2.4/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.3/imy/async_utils.py` & `imy-0.2.4/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.3/imy/config.py` & `imy-0.2.4/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.3/imy/docstrings/parsers.py` & `imy-0.2.4/imy/docstrings/parsers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import collections
+import copy
 import dataclasses
+import functools
 import inspect
 import textwrap
 import typing
 import warnings
 from dataclasses import is_dataclass
 from typing import *  # type: ignore
 
 import introspection
+import introspection.types
 import introspection.typing
 from uniserde import Jsonable
 
-from . import models
+from . import data_models
 
 
 def split_docstring_into_sections(docstring: str) -> tuple[str, dict[str, str]]:
     """
     Splits the given docstring into sections separated by markdown headings. The
     result is the part of the string before the first heading, and a dictionary
     mapping the heading names to the text of the sections ("the summary").
@@ -163,15 +166,15 @@
     return summary, details, sections
 
 
 def parse_docstring(
     docstring: str,
     *,
     key_sections: Iterable[str],
-) -> models.Docstring:
+) -> data_models.Docstring:
     """
     Parses a docstring into
 
     - summary
     - details
     - sections
 
@@ -214,28 +217,28 @@
     # Make sure all requested sections are present
     missing_sections = key_sections - key_value_sections.keys()
 
     for missing_section in missing_sections:
         key_value_sections[missing_section] = {}
 
     # Done
-    return models.Docstring(
+    return data_models.Docstring(
         summary=summary,
         details=details,
         key_sections=key_value_sections,
     )
 
 
-def parse_function(func: Callable[..., Any]) -> models.FunctionDocs:
+def parse_function(func: Callable[..., Any]) -> data_models.FunctionDocs:
     """
-    Given a function, parse its signature an docstring into a `FunctionDocs`
+    Given a function, parse its signature and docstring into a `FunctionDocs`
     object.
     """
 
-    def parse_annotation(annotation: object) -> str | None:
+    def parse_annotation(annotation: object) -> introspection.types.TypeAnnotation:
         if annotation is inspect.Parameter.empty:
             return None
 
         # Recursive types can cause issues. In particular, we have `Jsonable`,
         # which is a recursive type, and `JsonDoc`, which references `Jsonable`.
         # So if a module imports `JsonDoc` but doesn't import `Jsonable`, it's
         # impossible to evaluate the forward reference `"Jsonable"` in that
@@ -257,79 +260,124 @@
             func.__module__,
             extra_globals=extra_globals,
             mode="ast",
             treat_name_errors_as_imports=True,
             strict=True,
         )
 
-        return str_type_hint(annotation)  # type: ignore
+        return introspection.typing.annotation_to_string(annotation)  # type: ignore
 
     # Parse the parameters
     signature = inspect.signature(func)
-    parameters: dict[str, models.FunctionParameter] = {}
+    parameters: dict[str, data_models.FunctionParameter] = {}
 
     for param_name, param in signature.parameters.items():
         if param.default == inspect.Parameter.empty:
             param_default = None
         else:
             param_default = repr(param.default)
 
-        parameters[param_name] = models.FunctionParameter(
+        parameters[param_name] = data_models.FunctionParameter(
             name=param_name,
             type=parse_annotation(param.annotation),
             default=param_default,
             kw_only=param.kind == inspect.Parameter.KEYWORD_ONLY,
             collect_positional=param.kind == inspect.Parameter.VAR_POSITIONAL,
             collect_keyword=param.kind == inspect.Parameter.VAR_KEYWORD,
             description=None,
         )
 
+    # All our components are dataclasses, and all default values are
+    # converted into default factories. This results in the default
+    # values of `__init__` parameters being displayed as `<factory>`.
+    if any(param.default == "<factory>" for param in parameters.values()):
+        # This is super hacky, but since the actual default value isn't
+        # accessible from the `__init__` function, we somehow have to
+        # get a hold of the class, then the field, the default factory,
+        # and finally the default value.
+        cls = func.__globals__[func.__qualname__.split(".")[0]]
+        fields = {field.name: field for field in dataclasses.fields(cls)}
+
+        for param in parameters.values():
+            if param.default != "<factory>":
+                continue
+
+            default_factory = fields[param.name].default_factory
+
+            if not isinstance(default_factory, functools.partial):
+                continue
+
+            if default_factory.func not in (copy.copy, copy.deepcopy):
+                continue
+
+            default_value = default_factory.args[0]
+            if default_value is None or type(default_value) in (
+                bool,
+                int,
+                float,
+                bytes,
+                str,
+            ):
+                param.default = repr(default_value)
+
     # Parse the docstring
     docstring = inspect.getdoc(func)
 
     if docstring is None:
-        parsed = models.Docstring(summary=None, details=None, key_sections={})
+        parsed = data_models.Docstring(summary=None, details=None, key_sections={})
+        raises = []
+        metadata = data_models.FunctionMetadata.from_dictionary({})
     else:
-        parsed = parse_docstring(docstring, key_sections=["args", "raises"])
-
-        raw_params = parsed.key_sections["args"]
-        raw_raises = parsed.key_sections["raises"]
+        parsed = parse_docstring(
+            docstring,
+            key_sections=[
+                "args",
+                "raises",
+                "metadata",
+            ],
+        )
 
         # Add any information learned about parameters from the docstring
-        for param_name, param_details in raw_params.items():
+        for param_name, param_details in parsed.key_sections["args"].items():
             try:
                 result_param = parameters[param_name]
             except KeyError:
                 warnings.warn(
                     f"The docstring for function `{func.__name__}` mentions a parameter `{param_name}` that does not exist in the function signature."
                 )
                 continue
 
             result_param.description = param_details
 
         # Add information about raised exceptions
-        raises = list(raw_raises.items())
+        raises = list(parsed.key_sections["raises"].items())
+
+        # Parse the metadata
+        metadata = data_models.FunctionMetadata.from_dictionary(
+            parsed.key_sections["metadata"]
+        )
 
     # Build the result
-    return models.FunctionDocs(
+    return data_models.FunctionDocs(
         name=func.__name__,
         parameters=list(parameters.values()),
         return_type=parse_annotation(signature.return_annotation),
         synchronous=not inspect.iscoroutinefunction(func),
         summary=parsed.summary,
         details=parsed.details,
         raises=raises,
+        metadata=metadata,
     )
 
 
 def _parse_class_docstring_with_inheritance(
     cls: type,
     *,
     key_sections: Iterable[str],
-) -> models.Docstring:
+) -> data_models.Docstring:
     """
     Parses the docstring of a class in the same format as `parse_docstring`, but
     accounts for inheritance: Key-Value sections of all classes are merged, in a
     way that preserves child docs over parent docs.
     """
 
     # Parse the docstring for this class
@@ -338,15 +386,15 @@
     key_sections = set(key_sections)
     parsed_docs = parse_docstring(
         "" if raw_docs is None else raw_docs,
         key_sections=key_sections,
     )
 
     # Get the docstrings for the base classes
-    base_docs: list[models.Docstring] = []
+    base_docs: list[data_models.Docstring] = []
 
     for base in cls.__bases__:
         base_docs.append(
             _parse_class_docstring_with_inheritance(
                 base,
                 key_sections=key_sections,
             )
@@ -361,96 +409,109 @@
             result_section = result_sections.setdefault(section_name, {})
             result_section.update(section)
 
     # Done
     return parsed_docs
 
 
-def parse_class(cls: type) -> models.ClassDocs:
+def parse_class(cls: type) -> data_models.ClassDocs:
     """
     Given a class, parse its signature an docstring into a `ClassDocs` object.
     """
 
     # Parse the functions
     #
     # Make sure to add functions from base classes as well
-    functions_by_name: dict[str, models.FunctionDocs] = {}
+    functions_by_name: dict[str, data_models.FunctionDocs] = {}
 
     def add_functions(cls: type) -> None:
         # Chain to the base classes
         for base in cls.__bases__:
             add_functions(base)
 
-        # Then process this class. This way they override inherited functions.
+        # Then process this class. This way locals functions override inherited
+        # ones.
         for name, func in inspect.getmembers(cls, inspect.isfunction):
             func_docs = parse_function(func)
             functions_by_name[name] = func_docs
 
     add_functions(cls)
-    functions = list(functions_by_name.values())
 
-    # Parse the fields
-    fields_by_name: dict[str, models.ClassField] = {}
+    # Do the same for fields
+    fields_by_name: dict[str, data_models.ClassField] = {}
 
-    for name, typ in inspection.get_resolved_type_annotations(cls).items():
-        if typ is dataclasses.KW_ONLY:
-            continue
+    def add_fields(cls: type) -> None:
+        # Chain to the base classes
+        for base in cls.__bases__:
+            add_fields(base)
 
-        fields_by_name[name] = models.ClassField(
-            name=name,
-            type=str_type_hint(typ),
-            default=None,
-            description=None,
-        )
+        # Then process this class. This way locals fields override inherited
+        # ones.
+        for attribute_name, annotation in vars(cls).get("__annotations__", {}).items():
+            attribute_type = introspection.typing.resolve_forward_refs(
+                annotation=annotation,
+                context=cls.__module__,
+                mode="ast",
+                strict=True,
+                treat_name_errors_as_imports=True,
+            )
+
+            fields_by_name[attribute_name] = data_models.ClassField(
+                name=attribute_name,
+                type=attribute_type,  # type: ignore
+                default=None,
+                description=None,
+            )
+
+    add_fields(cls)
 
     # Properties are also fields
     for name, _ in inspect.getmembers(cls, inspect.isdatadescriptor):
         if name in fields_by_name:
             continue
 
+        # TODO
+
     # Is this a dataclass? If so, get the fields from there
     if is_dataclass(cls):
         for dataclass_field in dataclasses.fields(cls):
             doc_field = fields_by_name[dataclass_field.name]
 
             # Default value?
             if dataclass_field.default is not dataclasses.MISSING:
                 doc_field.default = repr(dataclass_field.default)
 
             # Default factory?
             elif dataclass_field.default_factory is not dataclasses.MISSING:
                 doc_field.default = repr(dataclass_field.default_factory())
 
     # Parse the docstring
-    (
-        short_description,
-        long_description,
-        sections,
-    ) = _parse_class_docstring_with_inheritance(
+    docs = _parse_class_docstring_with_inheritance(
         cls,
-        key_sections=["attributes"],
+        key_sections=[
+            "attributes",
+            "metadata",
+        ],
     )
 
     # Add any information learned about fields from the docstring
-    raw_attributes = sections["attributes"]
-
-    for field_name, field_details in raw_attributes.items():
+    for field_name, field_details in docs.key_sections["attributes"].items():
         try:
             result_field = fields_by_name[field_name]
         except KeyError:
             warnings.warn(
                 f"The docstring for class `{cls.__name__}` mentions a field `{field_name}` that does not exist in the class."
             )
             continue
 
         result_field.description = field_details
 
     # If `__init__` is missing documentation for any parameters, try to copy the
     # values from matching fields.
-    for func_docs in functions:
+    for func_docs in functions_by_name.values():
         if func_docs.name != "__init__":
             continue
 
         for param in func_docs.parameters:
             if param.description is not None:
                 continue
 
@@ -460,14 +521,17 @@
                 continue
 
             param.description = field.description
 
         break
 
     # Build the result
-    return models.ClassDocs(
+    return data_models.ClassDocs(
         name=cls.__name__,
         attributes=list(fields_by_name.values()),
-        functions=functions,
-        summary=short_description,
-        details=long_description,
+        functions=list(functions_by_name.values()),
+        summary=docs.summary,
+        details=docs.details,
+        metadata=data_models.ClassMetadata.from_dictionary(
+            docs.key_sections["metadata"]
+        ),
     )
```

### Comparing `imy-0.2.3/imy/inject.py` & `imy-0.2.4/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.3/imy/logs.py` & `imy-0.2.4/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.3/imy/package_metadata.py` & `imy-0.2.4/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.3/pyproject.toml` & `imy-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.2.3"
+version = "0.2.4"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.2.3/PKG-INFO` & `imy-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

