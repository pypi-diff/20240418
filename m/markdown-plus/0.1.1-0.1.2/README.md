# Comparing `tmp/markdown_plus-0.1.1.tar.gz` & `tmp/markdown_plus-0.1.2.tar.gz`

## Comparing `markdown_plus-0.1.1.tar` & `markdown_plus-0.1.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/CODEOWNERS
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/READMEold.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/docs/DevelopNewGenerators.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/docs/DevelopNewTemplates.md
--rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/docs/Generators.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/docs/README.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/docs/Templates.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/_version.py
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/cli.py
--rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/cli_old.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/config.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core_old.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core/__init__.py
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core/generator.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core/importer.py
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core/documents/block.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core/documents/definitions.py
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core/documents/document.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core/documents/structure.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core/environments/base.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/core/environments/ros2.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/flags.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/generate/__init__.py
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/generate/content.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/generate/installation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/generate/getting_started/__init__.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/generate/getting_started/pakk.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/include/__init__.py
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/include/example.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/include/examples.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/include/md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/ros/__init__.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/ros/interfaces.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/ros/launchs.py
--rw-r--r--   0        0        0     7976 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/generators/ros/nodes.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/Hooks.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/MDP_IGNORE
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/default/DOCS.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/default/README.md
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/init/_README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/init/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/init/docs/AUTHORS.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/init/docs/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/init/examples/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/init/examples/example1.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/templates/init/examples/mdplus.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/util/__init__.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/util/file_utils.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/util/hooks.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/util/markdown.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/util/regex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/util/parser/__init__.py
--rw-r--r--   0        0        0    15397 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/util/parser/py_parser.py
--rw-r--r--   0        0        0    20733 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/mdplus/util/parser/ros2_parser.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/.gitignore
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/LICENSE
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/README.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 markdown_plus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/CODEOWNERS
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/READMEold.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/DevelopNewGenerators.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/DevelopNewTemplates.md
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/Generators.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/README.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/docs/Templates.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/_version.py
+-rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/cli.py
+-rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/cli_old.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/config.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core_old.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/__init__.py
+-rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/generator.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/importer.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/documents/block.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/documents/definitions.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/documents/document.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/documents/structure.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/environments/base.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/core/environments/ros2.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/flags.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/__init__.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/content.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/installation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/getting_started/__init__.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/generate/getting_started/pakk.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/include/__init__.py
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/include/example.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/include/examples.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/include/md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/ros/__init__.py
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/ros/interfaces.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/ros/launchs.py
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/generators/ros/nodes.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/Hooks.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/MDP_IGNORE
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/default/DOCS.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/default/README.md
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/_README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/docs/AUTHORS.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/docs/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/examples/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/examples/example1.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/templates/init/examples/mdplus.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/__init__.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/file_utils.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/hooks.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/markdown.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/parser/__init__.py
+-rw-r--r--   0        0        0    15397 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/parser/py_parser.py
+-rw-r--r--   0        0        0    20733 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/mdplus/util/parser/ros2_parser.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/.gitignore
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 markdown_plus-0.1.2/PKG-INFO
```

### Comparing `markdown_plus-0.1.1/READMEold.md` & `markdown_plus-0.1.2/READMEold.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/.github/workflows/python-publish.yml` & `markdown_plus-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/docs/Generators.md` & `markdown_plus-0.1.2/docs/Generators.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/docs/README.md` & `markdown_plus-0.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/cli.py` & `markdown_plus-0.1.2/mdplus/cli.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/cli_old.py` & `markdown_plus-0.1.2/mdplus/cli_old.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/config.py` & `markdown_plus-0.1.2/mdplus/config.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/core_old.py` & `markdown_plus-0.1.2/mdplus/core_old.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/logger.py` & `markdown_plus-0.1.2/mdplus/logger.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/core/generator.py` & `markdown_plus-0.1.2/mdplus/core/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,18 @@
         """Get the entry of the module, containing the start and end tag.
 
         Returns
         -------
         str
             The entry of the module.
         """
+        if not self.is_applicable():
+            logger.info("Module %s not applicable", self.command)
+            return self.origin_text
+
         logger.info("Generating entry for %s", self.command)
 
         # Adapt the header level
         content = self.get_content()
         content = adapt_header_level(content, self.arg_level - 1)
 
         return "\n".join([self.start_tag, content, self.end_tag])
```

### Comparing `markdown_plus-0.1.1/mdplus/core/importer.py` & `markdown_plus-0.1.2/mdplus/core/importer.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,18 @@
     def get_module(command: str) -> MdpGenerator | None:
         """Get a module for a given command."""
 
         from mdplus.core.generator import MdpGenerator
 
         if command not in ModuleImporter.modules:
             module_name = f"{GENERATORS_PREFIX}.{command}"
-            spec = importlib.util.find_spec(module_name)
+            try:
+                spec = importlib.util.find_spec(module_name)
+            except ModuleNotFoundError:
+                spec = None
             if spec is not None:
                 logger.debug("Importing generator %s", module_name)
                 ModuleImporter.modules[command] = importlib.import_module(module_name)
 
             else:
                 logger.warning("Generator %s not found", module_name)
                 ModuleImporter.modules[command] = None
```

### Comparing `markdown_plus-0.1.1/mdplus/core/documents/block.py` & `markdown_plus-0.1.2/mdplus/core/documents/block.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/core/documents/definitions.py` & `markdown_plus-0.1.2/mdplus/core/documents/definitions.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/core/documents/document.py` & `markdown_plus-0.1.2/mdplus/core/documents/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,18 +145,28 @@
         workspace: Workspace,
         comment_definition: CommentDefinition = CommentDefinition.get_python_style(),
     ):
         super().__init__(file_path, workspace, comment_definition)
 
         self.origin_text = None
 
+    @property
+    def skip_generating(self):
+        flags = ["skip_generating", "skip", "ignore"]
+
+        for flag in flags:
+            if flag in self.args:
+                return self.args[flag]
+
+        return False
+
     def process(self):
 
         # If skip_generating is set, we do not generate the document
-        if self.args.get("skip_generating", False):
+        if self.skip_generating:
             logger.info(f"Skipping document: {self.full_path}")
             return
 
         logger.info(f"Processing document: {self.full_path}")
 
         text = ""
         with open(self.full_path, "r", encoding="utf-8") as f:
```

### Comparing `markdown_plus-0.1.1/mdplus/core/documents/structure.py` & `markdown_plus-0.1.2/mdplus/core/documents/structure.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/core/environments/base.py` & `markdown_plus-0.1.2/mdplus/core/environments/base.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/generators/generate/content.py` & `markdown_plus-0.1.2/mdplus/generators/generate/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import os
 import logging
 
 from mdplus.core.generator import MdpGenerator
 
-from markdownTable import markdownTable
+from markdownTable import markdown_table
 
 import pandas as pd
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -118,10 +118,10 @@
 
 
             # Convert entries to a dataframe
             df = pd.DataFrame(entries.items(), columns=["Dir", "Content"])
 
             # Create a Markdown table out of the dataframe
             mkdict = df.to_dict(orient="records")
-            content.append(markdownTable(mkdict).setParams(row_sep="markdown", quote=False).getMarkdown())
+            content.append(markdown_table(mkdict).set_params(row_sep="markdown", quote=False, padding_weight="right").get_markdown())
 
             return "\n\n".join(content)
```

### Comparing `markdown_plus-0.1.1/mdplus/generators/generate/installation.py` & `markdown_plus-0.1.2/mdplus/generators/generate/installation.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/generators/generate/getting_started/pakk.py` & `markdown_plus-0.1.2/mdplus/generators/generate/getting_started/pakk.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/generators/include/example.py` & `markdown_plus-0.1.2/mdplus/generators/include/example.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/generators/include/examples.py` & `markdown_plus-0.1.2/mdplus/generators/include/examples.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/generators/include/md.py` & `markdown_plus-0.1.2/mdplus/generators/include/md.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/generators/ros/interfaces.py` & `markdown_plus-0.1.2/mdplus/generators/ros/interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, Dict, List
 
-from markdownTable import markdownTable
+from markdownTable import markdown_table
 
 from mdplus.core.environments.ros2 import Ros2Environment
 from mdplus.util.markdown import get_anchor_from_header
 from mdplus.util.parser.ros2_parser import Package, PackageType
 from overrides import overrides
 
 if TYPE_CHECKING:
@@ -85,8 +85,8 @@
                         "Package": package.name,
                     }
                 )
 
         msg_data.sort(key=lambda x: x["Name"])
         srv_data.sort(key=lambda x: x["Name"])
 
-        return markdownTable(msg_data + srv_data).setParams(row_sep="markdown", quote=False).getMarkdown()
+        return markdown_table(msg_data + srv_data).set_params(row_sep="markdown", quote=False, padding_weight="right").get_markdown()
```

### Comparing `markdown_plus-0.1.1/mdplus/generators/ros/launchs.py` & `markdown_plus-0.1.2/mdplus/generators/ros/launchs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
-from markdownTable import markdownTable
+from markdownTable import markdown_table
 
 import mdplus.util.file_utils as file_utils
 from mdplus.core.environments.ros2 import Ros2Environment
 from mdplus.core.generator import MdpGenerator
 from mdplus.util.markdown import adapt_string_for_table, get_link
 from mdplus.util.parser.ros2_parser import Package, PackageType
 from overrides import overrides
@@ -55,12 +55,12 @@
                                 ),
                             }
                         )
 
         scripts.sort(key=lambda x: x["Name"])
 
         if len(scripts) > 0:
-            content.append(markdownTable(scripts).setParams(row_sep="markdown", quote=False).getMarkdown())
+            content.append(markdown_table(scripts).set_params(row_sep="markdown", quote=False, padding_weight="right").get_markdown())
         else:
             content.append("This package has no launch scripts")
 
         return "\n\n".join(content)
```

### Comparing `markdown_plus-0.1.1/mdplus/generators/ros/nodes.py` & `markdown_plus-0.1.2/mdplus/generators/ros/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, List
 
-from markdownTable import markdownTable
+from markdownTable import markdown_table
 
 import mdplus.util.file_utils as file_utils
 from mdplus.core.environments.ros2 import Ros2Environment
 from mdplus.core.generator import MdpGenerator
 from mdplus.util.markdown import adapt_header_level, get_anchor_from_header, get_link
 from mdplus.util.parser.ros2_parser import Node, Package, PackageType
 
@@ -48,15 +48,15 @@
                             }
                         )
 
         nodes.sort(key=lambda x: x["Name"])
         if len(nodes) == 0:
             return ""
 
-        return markdownTable(nodes).setParams(row_sep="markdown", quote=False).getMarkdown()
+        return markdown_table(nodes).set_params(row_sep="markdown", quote=False, padding_weight="right").get_markdown()
 
     def get_content(self) -> str:
         """Creates a table of nodes found in the ROS-packages"""
 
         dir_path = self.workspace.root_path
         logger.info(f"Create ROS node information for {dir_path}")
 
@@ -169,15 +169,15 @@
         if not has_other_topics_than_not_found:
             for topic in topics:
                 del topic["Info"]
 
         if len(topics) > 0:
             topics.sort(key=lambda x: x["Topic"])
             table = (
-                markdownTable(topics).setParams(row_sep="markdown", quote=False, padding_weight="right").getMarkdown()
+                markdown_table(topics).set_params(row_sep="markdown", quote=False, padding_weight="right").get_markdown()
             )
             content.insert(2, "**Publisher, Subscriber and Services of this node**")
             content.insert(3, table)
 
         #################################################################################
         ### Parameter stuff
 
@@ -193,15 +193,15 @@
                         "Default": parameter.value,
                         "Info": parameter.comment,
                     }
                 )
             if len(parameters) > 0:
                 parameters.sort(key=lambda x: x["Name"])
                 table = (
-                    markdownTable(parameters)
-                    .setParams(row_sep="markdown", quote=False, padding_weight="right")
-                    .getMarkdown()
+                    markdown_table(parameters)
+                    .set_params(row_sep="markdown", quote=False, padding_weight="right")
+                    .get_markdown()
                 )
                 content.insert(2, "**Parameters of this node**")
                 content.insert(3, table)
 
         return "\n\n".join(content)
```

### Comparing `markdown_plus-0.1.1/mdplus/templates/default/README.md` & `markdown_plus-0.1.2/mdplus/templates/default/README.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/util/file_utils.py` & `markdown_plus-0.1.2/mdplus/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/util/hooks.py` & `markdown_plus-0.1.2/mdplus/util/hooks.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/util/markdown.py` & `markdown_plus-0.1.2/mdplus/util/markdown.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/util/regex.py` & `markdown_plus-0.1.2/mdplus/util/regex.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/util/parser/py_parser.py` & `markdown_plus-0.1.2/mdplus/util/parser/py_parser.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/mdplus/util/parser/ros2_parser.py` & `markdown_plus-0.1.2/mdplus/util/parser/ros2_parser.py`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/.gitignore` & `markdown_plus-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/LICENSE` & `markdown_plus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/README.md` & `markdown_plus-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `markdown_plus-0.1.1/pyproject.toml` & `markdown_plus-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "markdown-plus"
-version = "0.1.1"
-authors = [
-  { name="Valentin Schröter", email="vasc9380@th-wildau.de" },
-]
+version = "0.1.2"
+authors = [{ name = "Valentin Schröter", email = "vasc9380@th-wildau.de" }]
 description = "Generator for markdown files."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-    "click-aliases",
-    "click",
-    "GitPython",
-    "inquirerpy",
-    "mistletoe",
-    "overrides",
-    "pandas",
-    "py-markdown-table",
-    "rich",
-]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "click-aliases",
+  "click",
+  "GitPython",
+  "inquirerpy",
+  "mistletoe",
+  "overrides",
+  "pandas",
+  "py-markdown-table",
+  "rich",
 ]
+classifiers = ["Programming Language :: Python :: 3"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["mdplus"]
 
 [project.urls]
 Homepage = "https://github.com/iCampus-Wildau/markdown-plus"
 Issues = "https://github.com/iCampus-Wildau/markdown-plus/issues"
```

### Comparing `markdown_plus-0.1.1/PKG-INFO` & `markdown_plus-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.3
 Name: markdown-plus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generator for markdown files.
 Project-URL: Homepage, https://github.com/iCampus-Wildau/markdown-plus
 Project-URL: Issues, https://github.com/iCampus-Wildau/markdown-plus/issues
 Author-email: Valentin Schröter <vasc9380@th-wildau.de>
 License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: click
 Requires-Dist: click-aliases
 Requires-Dist: gitpython
 Requires-Dist: inquirerpy
 Requires-Dist: mistletoe
```

