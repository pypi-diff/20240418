# Comparing `tmp/dlg_paletteGen-0.3.5.tar.gz` & `tmp/dlg_palettegen-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlg_paletteGen-0.3.5.tar", last modified: Mon Mar 25 11:26:57 2024, max compression
+gzip compressed data, was "dlg_palettegen-0.3.6.tar", last modified: Thu Apr 18 09:41:25 2024, max compression
```

## Comparing `dlg_paletteGen-0.3.5.tar` & `dlg_palettegen-0.3.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:26:57.986204 dlg_paletteGen-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-25 11:26:57.986204 dlg_paletteGen-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:26:57.978204 dlg_paletteGen-0.3.5/dlg_paletteGen/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/dlg_paletteGen/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/dlg_paletteGen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/dlg_paletteGen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33046 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/dlg_paletteGen/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/dlg_paletteGen/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/dlg_paletteGen/module_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/dlg_paletteGen/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    32315 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/dlg_paletteGen/source_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23498 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/dlg_paletteGen/support_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:26:57.982204 dlg_paletteGen-0.3.5/dlg_paletteGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-25 11:26:57.000000 dlg_paletteGen-0.3.5/dlg_paletteGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-25 11:26:57.000000 dlg_paletteGen-0.3.5/dlg_paletteGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:26:57.000000 dlg_paletteGen-0.3.5/dlg_paletteGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-25 11:26:57.000000 dlg_paletteGen-0.3.5/dlg_paletteGen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-25 11:26:57.000000 dlg_paletteGen-0.3.5/dlg_paletteGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 11:26:57.000000 dlg_paletteGen-0.3.5/dlg_paletteGen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:26:57.986204 dlg_paletteGen-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:26:57.982204 dlg_paletteGen-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:26:57.982204 dlg_paletteGen-0.3.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/PickOne.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_casatask.py
--rw-r--r--   0 runner    (1001) docker     (127)    38003 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_eagle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_oskar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_rascil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/data/example_tabascal.py
--rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-03-25 11:26:49.000000 dlg_paletteGen-0.3.5/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.553818 dlg_palettegen-0.3.6/dlg_paletteGen/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33046 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/module_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32315 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/source_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23817 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/dlg_paletteGen/support_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 09:41:25.000000 dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.553818 dlg_palettegen-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:41:25.557818 dlg_palettegen-0.3.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/PickOne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_casatask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38003 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_eagle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_oskar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_rascil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/data/example_tabascal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21745 2024-04-18 09:41:17.000000 dlg_palettegen-0.3.6/tests/test_base.py
```

### Comparing `dlg_paletteGen-0.3.5/HISTORY.md` & `dlg_palettegen-0.3.6/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Fixed value of complex types. [Andreas Wicenec]
+
+
+0.3.5 (2024-03-25)
+------------------
+- Release: version 0.3.5 🚀 [Andreas Wicenec]
 - Release: version 0.3.4 🚀 [Andreas Wicenec]
 - Updated gituhub actions. [Andreas Wicenec]
 
 
 0.3.4 (2024-03-25)
 ------------------
 - Release: version 0.3.4 🚀 [Andreas Wicenec]
```

### Comparing `dlg_paletteGen-0.3.5/LICENSE` & `dlg_palettegen-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/PKG-INFO` & `dlg_palettegen-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlg_paletteGen
-Version: 0.3.5
+Version: 0.3.6
 Summary: DALiuGE palette generator tool
 Home-page: https://github.com/ICRAR/dlg_paletteGen/
 Author: ICRAR
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-benedict
 Requires-Dist: numpy
```

### Comparing `dlg_paletteGen-0.3.5/README.md` & `dlg_palettegen-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/dlg_paletteGen/classes.py` & `dlg_palettegen-0.3.6/dlg_paletteGen/classes.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/dlg_paletteGen/cli.py` & `dlg_palettegen-0.3.6/dlg_paletteGen/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,15 +101,17 @@
         "-q",
         "--quiet",
         help="Only critical logging",
         action="store_true",
     )
     if not args:
         if len(sys.argv) == 1:
-            print("\x1b[31;20mInsufficient number of " + "arguments provided!!!\n\x1b[0m")
+            print(
+                "\x1b[31;20mInsufficient number of " + "arguments provided!!!\n\x1b[0m"
+            )
             parser.print_help(sys.stderr)
             sys.exit(1)
         args = parser.parse_args()
     logger.setLevel(logging.INFO)
     if args.quiet:
         logger.setLevel(logging.CRITICAL)
     elif args.verbose:
@@ -233,25 +235,26 @@
             nodes, module_doc = nodes_from_module(m, recursive=top_recursive)
         else:
             nodes, module_doc = nodes_from_module(m, recursive=recursive)
         if len(nodes) == 0:
             continue
         filename = outfile if not split else f"{outfile}{m.replace('.','_')}.palette"
         files[filename] = len(nodes)
-        prepare_and_write_palette(nodes, filename, module_doc=module_doc)
+        palette = prepare_and_write_palette(nodes, filename, module_doc=module_doc)
         logger.info(
             "%s palette file written with %s components\n%s",
             filename,
             len(nodes),
             m,
         )
     logger.info(
         "\n\n>>>>>>> Extraction summary <<<<<<<<\n%s\n",
         "\n".join([f"Wrote {k} with {v} components" for k, v in files.items()]),
     )
+    return palette
 
 
 def main():  # pragma: no cover
     """
     The main function executes on commands:
     `python -m dlg_paletteGen` and `$ dlg_paletteGen `.
     """
@@ -279,15 +282,15 @@
     logger.info("Module Path: %s", module_path)
 
     # create a temp directory for the output of doxygen
     output_directory = tempfile.TemporaryDirectory()
 
     if len(module_path) > 0:
         outputfile = "" if outputfile == "." else outputfile
-        palettes_from_module(
+        palette = palettes_from_module(
             module_path, outfile=outputfile, recursive=recursive, split=split
         )
     else:
         # add extra doxygen setting for input and output locations
         DOXYGEN_SETTINGS.update({"PROJECT_NAME": os.environ.get("PROJECT_NAME")})
         DOXYGEN_SETTINGS.update({"INPUT": inputdir})
         DOXYGEN_SETTINGS.update({"OUTPUT_DIRECTORY": output_directory.name})
@@ -298,11 +301,12 @@
         # get environment variables
         # gitrepo = os.environ.get("GIT_REPO")
         # version = os.environ.get("PROJECT_VERSION")
 
         nodes = process_compounddefs(
             output_xml_filename, tag, allow_missing_eagle_start, language
         )
-        prepare_and_write_palette(nodes, outputfile)
+        palette = prepare_and_write_palette(nodes, outputfile)
         return
     # cleanup the output directory
     output_directory.cleanup()
+    return palette
```

### Comparing `dlg_paletteGen-0.3.5/dlg_paletteGen/module_base.py` & `dlg_palettegen-0.3.6/dlg_paletteGen/module_base.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/dlg_paletteGen/settings.py` & `dlg_palettegen-0.3.6/dlg_paletteGen/settings.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/dlg_paletteGen/source_base.py` & `dlg_palettegen-0.3.6/dlg_paletteGen/source_base.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/dlg_paletteGen/support_functions.py` & `dlg_palettegen-0.3.6/dlg_paletteGen/support_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,20 @@
     palette["modelData"]["numLGNodes"] = len(nodes)
 
     palette["nodeDataArray"] = nodes
 
     # write palette to file
     # logger.debug(">>> palette: %s", palette)
     with open(output_filename, "w", encoding="utf-8") as outfile:
-        json.dump(palette, outfile, indent=4)
+        try:
+            json.dump(palette, outfile, indent=4)
+            return palette
+        except TypeError:
+            logger.error("Problem serializing palette! Bailing out!!")
+            return palette
 
 
 def get_field_by_name(name: str, node, value_key: str = "") -> dict:
     """
     Get field dictionary from node providing a name.
 
     :param name: the name of the field to retrieve
@@ -243,23 +248,24 @@
         elif not func_name:
             v_ind += 1
             f_nodes.append(nodes[i])
             vertices[v_ind] = nodes[i]
     block_dag = build_block_dag(vertices, [], data_fields=BLOCKDAG_DATA_FIELDS)
 
     # write the output json file
-    write_palette_json(
+    palette = write_palette_json(
         output_filename,
         module_doc,
         f_nodes,
         GITREPO,
         VERSION,
         block_dag,
     )
     logger.debug("Wrote %s components to %s", len(nodes), output_filename)
+    return palette
 
 
 def get_submodules(module):
     """
     Retrieve names of sub-modules using iter_modules.
     This will also return sub-packages. Third tuple
     item is a flag ispkg indicating that.
@@ -374,15 +380,17 @@
                             logger.debug(
                                 "Trying to load backwards: %s",
                                 ".".join(parts[:-1]),
                             )
                             mod = importlib.import_module(".".join(parts[:-1]))
                             break
                         except Exception as e:
-                            raise ValueError("Problem importing module %s, %s" % (mod, e))
+                            raise ValueError(
+                                "Problem importing module %s, %s" % (mod, e)
+                            )
                 logger.debug("Loaded module: %s", mod_name)
             else:
                 logger.debug("Recursive import failed! %s", parts[0] in sys.modules)
                 return None
     return mod
 
 
@@ -460,15 +468,15 @@
         if isinstance(value, type):
             value = None
         try:
             json.dumps(value)
         except TypeError:
             # this is a complex type
             logger.debug("Object not JSON serializable: %s", value)
-            ptype = type(value).__name__
+            ptype = value = type(value).__name__
         if not isinstance(value, (str, bool)) and (
             ptype in ["Json"]
         ):  # we want to carry these as strings
             value = value.__name__()
     param_desc["value"] = value
     param_desc["type"] = typeFix(ptype)
     return param_desc
@@ -540,15 +548,17 @@
             dtype = param_desc["desc"].split(",", maxsplit=1)[0]
             if dtype in SVALUE_TYPES:
                 param_desc["type"] = SVALUE_TYPES[dtype]
         if param_desc["type"] and field[p]["type"] in [None, "UNSPECIFIED"]:
             field[p]["type"] = param_desc["type"]
         if isinstance(field[p]["value"], numpy.ndarray):
             try:
-                field[p]["value"] = field[p]["defaultValue"] = field[p]["value"].tolist()
+                field[p]["value"] = field[p]["defaultValue"] = field[p][
+                    "value"
+                ].tolist()
             except NotImplementedError:
                 field[p]["value"] = []
         fields.update(field)
 
     logger.debug("Parameters %s", fields)
     if descr_miss:
         logger.warning(
@@ -609,15 +619,17 @@
 
     n = "execution_time"
     et = initializeField(n)
     et[n]["name"] = n
     et[n]["value"] = 2
     et[n]["defaultValue"] = 2
     et[n]["type"] = "Integer"
-    et[n]["description"] = "Estimate of execution time (in seconds) for this application."
+    et[n][
+        "description"
+    ] = "Estimate of execution time (in seconds) for this application."
     et[n]["parameterType"] = "ConstraintParameter"
     Node["fields"].update(et)
 
     n = "num_cpus"
     ncpus = initializeField(n)
     ncpus[n]["name"] = n
     ncpus[n]["value"] = 1
```

### Comparing `dlg_paletteGen-0.3.5/dlg_paletteGen.egg-info/PKG-INFO` & `dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlg_paletteGen
-Version: 0.3.5
+Version: 0.3.6
 Summary: DALiuGE palette generator tool
 Home-page: https://github.com/ICRAR/dlg_paletteGen/
 Author: ICRAR
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-benedict
 Requires-Dist: numpy
```

### Comparing `dlg_paletteGen-0.3.5/dlg_paletteGen.egg-info/SOURCES.txt` & `dlg_palettegen-0.3.6/dlg_paletteGen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/setup.py` & `dlg_palettegen-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/PickOne.py` & `dlg_palettegen-0.3.6/tests/data/PickOne.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_casatask.py` & `dlg_palettegen-0.3.6/tests/data/example_casatask.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_eagle.py` & `dlg_palettegen-0.3.6/tests/data/example_eagle.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_functions.py` & `dlg_palettegen-0.3.6/tests/data/example_functions.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_google.py` & `dlg_palettegen-0.3.6/tests/data/example_google.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_numpy.py` & `dlg_palettegen-0.3.6/tests/data/example_numpy.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_options.py` & `dlg_palettegen-0.3.6/tests/data/example_options.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_oskar.py` & `dlg_palettegen-0.3.6/tests/data/example_oskar.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_rascil.py` & `dlg_palettegen-0.3.6/tests/data/example_rascil.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_rest.py` & `dlg_palettegen-0.3.6/tests/data/example_rest.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/data/example_tabascal.py` & `dlg_palettegen-0.3.6/tests/data/example_tabascal.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.3.5/tests/test_base.py` & `dlg_palettegen-0.3.6/tests/test_base.py`

 * *Files identical despite different names*

