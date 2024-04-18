# Comparing `tmp/gifnoc-0.3.0.tar.gz` & `tmp/gifnoc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gifnoc-0.3.0.tar", max compression
+gzip compressed data, was "gifnoc-0.3.1.tar", max compression
```

## Comparing `gifnoc-0.3.0.tar` & `gifnoc-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2268 2024-03-13 17:48:39.575307 gifnoc-0.3.0/README.md
--rw-r--r--   0        0        0      431 2024-04-04 05:32:30.662546 gifnoc-0.3.0/gifnoc/__init__.py
--rw-r--r--   0        0        0     3289 2024-03-22 19:29:13.603238 gifnoc-0.3.0/gifnoc/__main__.py
--rw-r--r--   0        0        0     3227 2024-04-04 03:48:00.163881 gifnoc-0.3.0/gifnoc/acquire.py
--rw-r--r--   0        0        0     6539 2024-04-04 03:48:14.365182 gifnoc-0.3.0/gifnoc/arg.py
--rw-r--r--   0        0        0      126 2024-04-04 03:48:14.345716 gifnoc-0.3.0/gifnoc/config.py
--rw-r--r--   0        0        0     4420 2024-03-14 18:27:32.891465 gifnoc-0.3.0/gifnoc/docstrings.py
--rw-r--r--   0        0        0     6588 2024-04-04 03:48:14.376041 gifnoc-0.3.0/gifnoc/interface.py
--rw-r--r--   0        0        0     1348 2024-03-04 20:00:45.907307 gifnoc-0.3.0/gifnoc/merge.py
--rw-r--r--   0        0        0     3782 2024-04-03 21:43:10.065094 gifnoc-0.3.0/gifnoc/parse.py
--rw-r--r--   0        0        0     1392 2024-04-04 03:48:14.376295 gifnoc-0.3.0/gifnoc/proxy.py
--rw-r--r--   0        0        0     6863 2024-04-04 03:48:14.395375 gifnoc-0.3.0/gifnoc/registry.py
--rw-r--r--   0        0        0     1617 2024-04-04 03:48:14.390506 gifnoc-0.3.0/gifnoc/schema.py
--rw-r--r--   0        0        0      247 2024-03-08 22:39:08.607547 gifnoc-0.3.0/gifnoc/std/__init__.py
--rw-r--r--   0        0        0      822 2024-04-04 03:48:14.346765 gifnoc-0.3.0/gifnoc/std/_time.py
--rw-r--r--   0        0        0     4006 2024-04-04 05:34:58.949225 gifnoc-0.3.0/gifnoc/type_wrappers.py
--rw-r--r--   0        0        0     4273 2024-03-20 22:11:06.107781 gifnoc-0.3.0/gifnoc/utils.py
--rw-r--r--   0        0        0       18 2024-04-04 15:42:38.322839 gifnoc-0.3.0/gifnoc/version.py
--rw-r--r--   0        0        0      622 2024-04-04 15:42:38.300894 gifnoc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 gifnoc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2268 2024-03-13 17:48:39.575307 gifnoc-0.3.1/README.md
+-rw-r--r--   0        0        0      431 2024-04-04 05:32:30.662546 gifnoc-0.3.1/gifnoc/__init__.py
+-rw-r--r--   0        0        0     3261 2024-04-17 20:19:50.897932 gifnoc-0.3.1/gifnoc/__main__.py
+-rw-r--r--   0        0        0     3542 2024-04-17 20:52:37.030911 gifnoc-0.3.1/gifnoc/acquire.py
+-rw-r--r--   0        0        0     6497 2024-04-17 20:43:59.542425 gifnoc-0.3.1/gifnoc/arg.py
+-rw-r--r--   0        0        0      126 2024-04-04 03:48:14.345716 gifnoc-0.3.1/gifnoc/config.py
+-rw-r--r--   0        0        0     4420 2024-03-14 18:27:32.891465 gifnoc-0.3.1/gifnoc/docstrings.py
+-rw-r--r--   0        0        0     6544 2024-04-17 20:19:50.897927 gifnoc-0.3.1/gifnoc/interface.py
+-rw-r--r--   0        0        0     1347 2024-04-17 20:19:50.897737 gifnoc-0.3.1/gifnoc/merge.py
+-rw-r--r--   0        0        0     3835 2024-04-17 20:16:50.868285 gifnoc-0.3.1/gifnoc/parse.py
+-rw-r--r--   0        0        0     1362 2024-04-17 20:19:50.896918 gifnoc-0.3.1/gifnoc/proxy.py
+-rw-r--r--   0        0        0     6717 2024-04-17 20:19:50.898068 gifnoc-0.3.1/gifnoc/registry.py
+-rw-r--r--   0        0        0     1617 2024-04-04 03:48:14.390506 gifnoc-0.3.1/gifnoc/schema.py
+-rw-r--r--   0        0        0      247 2024-03-08 22:39:08.607547 gifnoc-0.3.1/gifnoc/std/__init__.py
+-rw-r--r--   0        0        0      822 2024-04-04 03:48:14.346765 gifnoc-0.3.1/gifnoc/std/_time.py
+-rw-r--r--   0        0        0     3976 2024-04-17 20:19:50.897814 gifnoc-0.3.1/gifnoc/type_wrappers.py
+-rw-r--r--   0        0        0     4259 2024-04-17 21:31:33.848158 gifnoc-0.3.1/gifnoc/utils.py
+-rw-r--r--   0        0        0       18 2024-04-17 21:39:53.520816 gifnoc-0.3.1/gifnoc/version.py
+-rw-r--r--   0        0        0      671 2024-04-17 21:39:53.497651 gifnoc-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 gifnoc-0.3.1/PKG-INFO
```

### Comparing `gifnoc-0.3.0/README.md` & `gifnoc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.0/gifnoc/__main__.py` & `gifnoc-0.3.1/gifnoc/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,15 @@
         if options.SUBPATH:
             cfg_type, _ = type_at_path(cfg_type, options.SUBPATH.split("."))
         schema = deserialization_schema(cfg_type)
         print(json.dumps(schema, indent=4))
 
 
 def main():
-    parser = argparse.ArgumentParser(
-        description="Do things with gifnoc configurations."
-    )
+    parser = argparse.ArgumentParser(description="Do things with gifnoc configurations.")
     parser.add_argument(
         "--module",
         "-m",
         action="append",
         help="Module(s) with the configuration definition(s)",
         default=[],
     )
@@ -65,17 +63,15 @@
     subparsers = parser.add_subparsers(dest="command", required=True)
 
     dump = subparsers.add_parser("dump", help="Dump configuration.")
     dump.add_argument("SUBPATH", help="Subpath to dump", nargs="?", default=None)
     dump.add_argument("--format", "-f", help="Dump format", default="raw")
 
     schema = subparsers.add_parser("schema", help="Dump JSON schema.")
-    schema.add_argument(
-        "SUBPATH", help="Subpath to get a schema for", nargs="?", default=None
-    )
+    schema.add_argument("SUBPATH", help="Subpath to get a schema for", nargs="?", default=None)
 
     options = parser.parse_args()
 
     from_env = os.environ.get("GIFNOC_MODULE", None)
     from_env = from_env.split(",") if from_env else []
 
     modules = [*from_env, *options.module]
```

### Comparing `gifnoc-0.3.0/gifnoc/acquire.py` & `gifnoc-0.3.1/gifnoc/acquire.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,68 @@
-from dataclasses import fields, is_dataclass
+from dataclasses import fields
 from pathlib import Path
+from typing import Protocol, Union, runtime_checkable
 
-from ovld import meta, ovld
+from ovld import Dataclass, ovld
 
 from .merge import merge
 from .parse import Context, EnvContext, FileContext, parse_file, parse_source
 from .utils import UnionTypes, convertible_from_string
 
 
-def is_structure(cls):
-    return issubclass(cls, dict) or issubclass(cls, list) or is_dataclass(cls)
+@runtime_checkable
+class PassthroughProtocol(Protocol):
+    __passthrough__: object
 
+    @classmethod
+    def __subclasshook__(cls, subclass):
+        return hasattr(cls, "__passthrough__")
 
-def is_passthrough(cls):
-    return hasattr(cls, "__passthrough__")
+
+StructureType = Union[type[list], type[dict], type[Dataclass]]
 
 
 @ovld
-def _acquire(model: meta(is_dataclass), d: dict, context: Context):
+def acquire(model: type[Dataclass], d: dict, context: Context):
     d = dict(d)
     for field in fields(model):
         if field.name in d:
             v = d[field.name]
             d[field.name] = acquire(field.type, v, context)
     return d
 
 
 @ovld
-def _acquire(model: str, s: str, context: FileContext):
+def acquire(model: type[str], s: str, context: FileContext):  # noqa: F811
     return s
 
 
 @ovld
-def _acquire(model: int, x: int, context: Context):
+def acquire(model: type[int], x: int, context: Context):  # noqa: F811
     return x
 
 
 @ovld
-def _acquire(model: float, x: float, context: Context):
+def acquire(model: type[float], x: float, context: Context):  # noqa: F811
     return x
 
 
 @ovld
-def _acquire(model: bool, x: bool, context: Context):
+def acquire(model: type[bool], x: bool, context: Context):  # noqa: F811
     return x
 
 
 @ovld
-def _acquire(model: list, xs: list, context: Context):
+def acquire(model: type[list], xs: list, context: Context):  # noqa: F811
     (element_model,) = model.__args__
     return [acquire(element_model, x, context) for x in xs]
 
 
 @ovld
-def _acquire(model: dict, xs: dict, context: Context):
+def acquire(model: type[dict], xs: dict, context: Context):  # noqa: F811
     if hasattr(model, "__annotations__"):
         return {
             k: acquire(v_model, xs[k], context)
             for k, v_model in model.__annotations__.items()
             if k in xs
         }
 
@@ -69,70 +74,71 @@
         }
 
     else:
         return xs
 
 
 @ovld
-def _acquire(model: meta(is_structure), p: Path, context: FileContext):
+def acquire(model: StructureType, p: Path, context: FileContext):  # noqa: F811
     p = (context.path or ".") / Path(p)
     return acquire(model, parse_file(p), FileContext(path=p.parent))
 
 
 @ovld
-def _acquire(model: meta(is_structure), s: str, context: FileContext):
+def acquire(model: StructureType, s: str, context: FileContext):  # noqa: F811
     if convertible_from_string(model):
         return s
     else:
         return acquire(model, Path(s), context)
 
 
 @ovld
-def _acquire(model: meta(is_passthrough), x: object, context: Context):
+def acquire(  # noqa: F811
+    model: type[PassthroughProtocol], x: object, context: Context
+):
     return acquire(model.__passthrough__, x, context)
 
 
 @ovld
-def _acquire(model: bool, s: str, context: EnvContext):
+def acquire(model: type[bool], s: str, context: EnvContext):  # noqa: F811
     if s.strip().lower() in ("", "0", "false"):
         return False
     else:
         return True
 
 
 @ovld
-def _acquire(model: int, s: str, context: EnvContext):
+def acquire(model: type[int], s: str, context: EnvContext):  # noqa: F811
     return int(s)
 
 
 @ovld
-def _acquire(model: float, s: str, context: EnvContext):
+def acquire(model: type[float], s: str, context: EnvContext):  # noqa: F811
     return float(s)
 
 
 @ovld
-def _acquire(model: str, s: str, context: EnvContext):
+def acquire(model: type[str], s: str, context: EnvContext):  # noqa: F811
     return s
 
 
 @ovld
-def _acquire(model: Path, s: str, context: FileContext):
+def acquire(model: type[Path], s: str, context: FileContext):  # noqa: F811
     return str(((context.path or ".") / s).resolve())
 
 
 @ovld
-def _acquire(model: object, obj: object, context: Context):
+def acquire(model: type[object], obj: object, context: Context):  # noqa: F811
     return obj
 
 
-def acquire(model, obj, context):
-    if isinstance(model, UnionTypes):
-        model, *_ = model.__args__
-    method = _acquire[getattr(model, "__origin__", model), type(obj), type(context)]
-    return method(model, obj, context)
+@ovld
+def acquire(model: UnionTypes, obj: object, context: Context):  # noqa: F811
+    model, *_ = model.__args__
+    return acquire(model, obj, context)
 
 
 def parse_sources(model, *sources):
     result = {}
     for src in sources:
         for ctx, dct in parse_source(src):
             result = merge(result, acquire(model, dct, ctx))
```

### Comparing `gifnoc-0.3.0/gifnoc/arg.py` & `gifnoc-0.3.1/gifnoc/arg.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,43 +27,49 @@
     help: str = None
     command_field: str = "command"
     commands: dict[str, Union[str, "Command"]] = field(default_factory=dict)
     options: dict[str, Union[str, Option]] = field(default_factory=dict)
 
 
 @ovld
-def compile_option(model: bool, path: str, option: Option):
+def compile_option(model: type[bool], path: str, option: Option):
     if option.action is None:
         option.action = argparse.BooleanOptionalAction
     return option
 
 
 @ovld
-def compile_option(model: (int, float), path: str, option: Option):  # noqa: F811
+def compile_option(  # noqa: F811
+    model: Union[type[int], type[float]], path: str, option: Option
+):
     if option.type is None:
         option.type = model
     return option
 
 
 @ovld
-def compile_option(model: object, path: str, option: Option):  # noqa: F811
+def compile_option(model: type[list], path: str, option: Option):  # noqa: F811
+    assert isinstance(model, GenericAlias)
+    option = compile_option(model.__args__[0], path, option)
+    option.action = "append"
+    return option
+
+
+@ovld
+def compile_option(model: type[object], path: str, option: Option):  # noqa: F811
     if isinstance(model, GenericAlias):
-        if model.__origin__ is list:
-            option = compile_option(model.__args__[0], path, option)
-            option.action = "append"
-        else:
-            return None
+        return None
     elif option.type is None:
         option.type = str
     return option
 
 
 @ovld
-def compile_option(model: object, path: str, option: str):  # noqa: F811
-    return compile_option[model, str, Option](model, path, Option(option=option))
+def compile_option(model: type[object], path: str, option: str):  # noqa: F811
+    return compile_option(model, path, Option(option=option))
 
 
 def abspath(path, mount):
     if mount.startswith("."):
         return f"{path}{mount}"
     else:
         return mount
@@ -91,63 +97,54 @@
     else:
         model = global_model
         doc = ""
 
     def _compile_option(p, v):
         ap = abspath(mount, p)
         typ, doc = type_at_path(global_model, ap.split("."), allow_union=False)
-        opt = compile_option[typ, str, type(v)](typ, mount, v)
+        opt = compile_option(typ, mount, v)
         if not opt:
             return None
         if opt.help is None:
             opt.help = doc
         return ap, opt
 
     def _merge(opts1, opts2):
         results = {abspath(mount, p): v for p, v in opts1.items()}
         opts2 = {abspath(mount, p): v for p, v in opts2.items()}
         for k, v in opts2.items():
             if k in results:
                 v = replace(
                     results[k],
-                    **{
-                        key: value
-                        for key, value in vars(v).items()
-                        if value is not None
-                    },
+                    **{key: value for key, value in vars(v).items() if value is not None},
                 )
             results[k] = v
         return results
 
     options = {}
     if command.auto:
         options.update(auto(model, mount))
     options = _merge(options, command.options)
-    options = dict(
-        compiled for p, v in options.items() if (compiled := _compile_option(p, v))
-    )
+    options = dict(compiled for p, v in options.items() if (compiled := _compile_option(p, v)))
 
     commands = {
-        cmd: compile_command(global_model, mount, v)
-        for cmd, v in command.commands.items()
+        cmd: compile_command(global_model, mount, v) for cmd, v in command.commands.items()
     }
     return replace(
         command,
         help=command.help or doc,
         mount=mount,
         auto=False,
         commands=commands,
         options=options,
     )
 
 
 @ovld
-def add_arguments_to_parser(
-    parser: argparse.ArgumentParser, command: Command, registry: Registry
-):
+def add_arguments_to_parser(parser: argparse.ArgumentParser, command: Command, registry: Registry):
     for dest, option in command.options.items():
         option.dest = f"&{dest}"
         add_arguments_to_parser(parser, option, registry)
     if command.commands:
         global_model = registry.model()
         dest = f"&{command.mount}.{command.command_field}"
         path = dest[1:].split(".")
```

### Comparing `gifnoc-0.3.0/gifnoc/docstrings.py` & `gifnoc-0.3.1/gifnoc/docstrings.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.0/gifnoc/interface.py` & `gifnoc-0.3.1/gifnoc/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from . import registry as registry_module
 from .arg import Command, add_arguments_to_parser, compile_command
 from .parse import EnvironMap, OptionsMap
 from .registry import Configuration, Registry, active_configuration
 from .utils import ConfigurationError, get_at_path
 
 global_registry = Registry()
-registry_module.global_configuration = Configuration(
-    sources=[], registry=global_registry
-)
+registry_module.global_configuration = Configuration(sources=[], registry=global_registry)
 
 register = global_registry.register
 map_environment_variables = global_registry.map_environment_variables
 define = global_registry.define
 use = global_registry.use
 load = global_registry.load
 load_global = global_registry.load_global
@@ -111,17 +109,15 @@
 
             model = registry.model()
             if isinstance(options, dict) or options is None:
                 command = Command(mount="", options=options)
             elif isinstance(options, str):
                 command = Command(mount=options, auto=True)
             elif not isinstance(options, Command):
-                raise TypeError(
-                    "options argument to cli() should be a dict or a Command"
-                )
+                raise TypeError("options argument to cli() should be a dict or a Command")
             else:
                 command = options
 
             command = compile_command(model, "", command)
             add_arguments_to_parser(argparser, command, registry)
 
             parsed = argparser.parse_args(sys.argv[1:] if argv is None else argv)
```

### Comparing `gifnoc-0.3.0/gifnoc/merge.py` & `gifnoc-0.3.1/gifnoc/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Utilities to merge dictionaries and other data structures."""
 
-
 from typing import Union
 
 from ovld import ovld
 
 from .utils import DELETE
 
 ###########
```

### Comparing `gifnoc-0.3.0/gifnoc/parse.py` & `gifnoc-0.3.1/gifnoc/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,15 +92,16 @@
         )
     if parser is None:
         sfx = file.suffix
         parser = extensions.get(sfx, None)
         if parser is None:
             raise NoParserError(f"No parser found for the {sfx} format")
     text = file.read_text()
-    return parser.load(text)
+    results = parser.load(text)
+    return results if results is not None else {}
 
 
 @ovld
 def parse_source(source: (str, Path)):  # noqa: F811
     """Parse a source from the filesystem."""
     source = Path(source).expanduser()
     if source.is_dir():
```

### Comparing `gifnoc-0.3.0/gifnoc/proxy.py` & `gifnoc-0.3.1/gifnoc/proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,17 +27,15 @@
                 else:
                     cfg = getattr(cfg, k)
             self._cached_data = root
             self._cached = cfg
             return cfg
         except (KeyError, AttributeError):
             key = ".".join(self._pth)
-            raise MissingConfigurationError(
-                f"No configuration was loaded for key '{key}'."
-            )
+            raise MissingConfigurationError(f"No configuration was loaded for key '{key}'.")
 
     def __str__(self):
         return f"Proxy for {self._obj()}"
 
     def __repr__(self):
         return f"Proxy({self._obj()!r})"
```

### Comparing `gifnoc-0.3.0/gifnoc/registry.py` & `gifnoc-0.3.1/gifnoc/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,19 +117,15 @@
             dc = make_dataclass(
                 cls_name=self.path,
                 bases=(self.cls,),
                 fields=[
                     (
                         name,
                         built := cfg.build(),
-                        field(
-                            default_factory=get_default_factory(
-                                built, cfg.default_factory
-                            )
-                        ),
+                        field(default_factory=get_default_factory(built, cfg.default_factory)),
                     )
                     for name, cfg in self.extras.items()
                 ],
             )
         if self.wrapper:
             dc = self.wrapper[dc]
         return dc
@@ -213,11 +209,9 @@
     ) -> _T:
         from .config import _Proxy
 
         # The typing is a little bit of a lie since we're returning a _Proxy object,
         # but it works just the same.
         self.register(field, model, default_factory=default_factory)
         if environ:
-            self.map_environment_variables(
-                **{k: f"{field}.{v}" for k, v in environ.items()}
-            )
+            self.map_environment_variables(**{k: f"{field}.{v}" for k, v in environ.items()})
         return _Proxy(*field.split("."))
```

### Comparing `gifnoc-0.3.0/gifnoc/schema.py` & `gifnoc-0.3.1/gifnoc/schema.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.0/gifnoc/std/_time.py` & `gifnoc-0.3.1/gifnoc/std/_time.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.3.0/gifnoc/type_wrappers.py` & `gifnoc-0.3.1/gifnoc/type_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,15 @@
         if key not in wrapper_cache:
             typ = type(
                 f"{name}[{item.__name__}]",
                 (cls,),
                 {"__passthrough__": item, "__wrapper__": cls},
             )
             wrapper_cache[key] = typ
-            deserializer(
-                Conversion(typ._deserialize, source=dict[str, Any], target=typ)
-            )
+            deserializer(Conversion(typ._deserialize, source=dict[str, Any], target=typ))
 
         return wrapper_cache[key]
 
 
 class _TaggedSubclass(_WrapperBase):
     @classmethod
     def register_schemas(cls):
```

### Comparing `gifnoc-0.3.0/gifnoc/utils.py` & `gifnoc-0.3.1/gifnoc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,10 +132,8 @@
             curr = curr[int(p)]
         else:
             curr = getattr(curr, p)
     return curr
 
 
 def convertible_from_string(typ):
-    return any(
-        converter_types(ds, target=typ)[0] is str for ds in default_deserialization(typ)
-    )
+    return any(converter_types(ds, target=typ)[0] is str for ds in default_deserialization(typ))
```

### Comparing `gifnoc-0.3.0/pyproject.toml` & `gifnoc-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 [tool.poetry]
 name = "gifnoc"
-version = "0.3.0"
+version = "0.3.1"
 description = "Handle configuration for multiple libraries"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-ovld = "^0.3.2"
+ovld = "^0.3.5"
 apischema = "^0.18.1"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.12.1"
-ruff = "^0.1.9"
+ruff = "^0.3.7"
 pytest-cov = "^5.0.0"
 pytest-regressions = "^2.5.0"
 pytest-timeout = "^2.3.1"
 
 [tool.poetry.scripts]
 gifnoc = "gifnoc.__main__:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 99
+
+[tool.ruff.lint]
 extend-select = ["I"]
+
+[tool.ruff.lint.isort]
+combine-as-imports = true
```

### Comparing `gifnoc-0.3.0/PKG-INFO` & `gifnoc-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gifnoc
-Version: 0.3.0
+Version: 0.3.1
 Summary: Handle configuration for multiple libraries
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: apischema (>=0.18.1,<0.19.0)
-Requires-Dist: ovld (>=0.3.2,<0.4.0)
+Requires-Dist: ovld (>=0.3.5,<0.4.0)
 Description-Content-Type: text/markdown
 
 
 # Gifnoc
 
 Gifnoc is a unified configuration system for Python modules.
```

