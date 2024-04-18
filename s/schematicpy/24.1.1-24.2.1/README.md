# Comparing `tmp/schematicpy-24.1.1.tar.gz` & `tmp/schematicpy-24.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematicpy-24.1.1.tar", max compression
+gzip compressed data, was "schematicpy-24.2.1.tar", max compression
```

## Comparing `schematicpy-24.1.1.tar` & `schematicpy-24.2.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1073 2024-01-22 17:45:00.153852 schematicpy-24.1.1/LICENSE
--rw-r--r--   0        0        0    17127 2024-01-22 17:45:00.153852 schematicpy-24.1.1/README.md
--rw-r--r--   0        0        0     3748 2024-01-22 17:45:27.229763 schematicpy-24.1.1/pyproject.toml
--rw-r--r--   0        0        0     1424 2024-01-22 17:45:00.157852 schematicpy-24.1.1/schematic/__init__.py
--rw-r--r--   0        0        0     1421 2024-01-22 17:45:00.157852 schematicpy-24.1.1/schematic/__main__.py
--rw-r--r--   0        0        0        0 2024-01-22 17:45:00.157852 schematicpy-24.1.1/schematic/configuration/__init__.py
--rw-r--r--   0        0        0     6996 2024-01-22 17:45:00.157852 schematicpy-24.1.1/schematic/configuration/configuration.py
--rw-r--r--   0        0        0     5034 2024-01-22 17:45:00.157852 schematicpy-24.1.1/schematic/configuration/dataclasses.py
--rw-r--r--   0        0        0      663 2024-01-22 17:45:00.157852 schematicpy-24.1.1/schematic/etc/README.md
--rw-r--r--   0        0        0    76063 2024-01-22 17:45:00.157852 schematicpy-24.1.1/schematic/etc/data_models/biothings.model.jsonld
--rw-r--r--   0        0        0  1387510 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/etc/data_models/schema_org.model.jsonld
--rw-r--r--   0        0        0     4414 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/etc/validation_schemas/class.schema.json
--rw-r--r--   0        0        0     9914 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/etc/validation_schemas/model.schema.json
--rw-r--r--   0        0        0     5021 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/etc/validation_schemas/property.schema.json
--rw-r--r--   0        0        0     3193 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/exceptions.py
--rw-r--r--   0        0        0    10451 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/help.py
--rw-r--r--   0        0        0     3415 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/loader.py
--rw-r--r--   0        0        0       59 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/manifest/__init__.py
--rw-r--r--   0        0        0    10076 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/manifest/commands.py
--rw-r--r--   0        0        0    86406 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/manifest/generator.py
--rw-r--r--   0        0        0    22904 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/models/GE_Helpers.py
--rw-r--r--   0        0        0       52 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/models/__init__.py
--rw-r--r--   0        0        0     6616 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/models/commands.py
--rw-r--r--   0        0        0    17870 2024-01-22 17:45:00.161852 schematicpy-24.1.1/schematic/models/metadata.py
--rw-r--r--   0        0        0    46040 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/models/validate_attribute.py
--rw-r--r--   0        0        0    12074 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/models/validate_manifest.py
--rw-r--r--   0        0        0      495 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/__init__.py
--rw-r--r--   0        0        0     4379 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/commands.py
--rw-r--r--   0        0        0     4291 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/curie.py
--rw-r--r--   0        0        0     5829 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/data_model_edges.py
--rw-r--r--   0        0        0    29457 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/data_model_graph.py
--rw-r--r--   0        0        0    17905 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/data_model_json_schema.py
--rw-r--r--   0        0        0    22070 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/data_model_jsonld.py
--rw-r--r--   0        0        0    12130 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/data_model_nodes.py
--rw-r--r--   0        0        0    21884 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/data_model_parser.py
--rw-r--r--   0        0        0     9561 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/data_model_relationships.py
--rw-r--r--   0        0        0     6896 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/data_model_validator.py
--rw-r--r--   0        0        0     7070 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/schemas/json_schema_validator.py
--rw-r--r--   0        0        0       96 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/store/__init__.py
--rw-r--r--   0        0        0      218 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/store/base.py
--rw-r--r--   0        0        0   115079 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/store/synapse.py
--rw-r--r--   0        0        0        0 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/__init__.py
--rw-r--r--   0        0        0     2524 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/cli_utils.py
--rw-r--r--   0        0        0     2785 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/curie_utils.py
--rw-r--r--   0        0        0     8182 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/df_utils.py
--rw-r--r--   0        0        0     8686 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/general.py
--rw-r--r--   0        0        0     7338 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/google_api_utils.py
--rw-r--r--   0        0        0     1140 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/io_utils.py
--rw-r--r--   0        0        0     5369 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/schema_utils.py
--rw-r--r--   0        0        0     9565 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/validate_rules_utils.py
--rw-r--r--   0        0        0     3086 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/validate_utils.py
--rw-r--r--   0        0        0      236 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/utils/viz_utils.py
--rw-r--r--   0        0        0      119 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/version.py
--rw-r--r--   0        0        0      135 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/visualization/__init__.py
--rw-r--r--   0        0        0    10868 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/visualization/attributes_explorer.py
--rw-r--r--   0        0        0     3548 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/visualization/commands.py
--rw-r--r--   0        0        0    37679 2024-01-22 17:45:00.165852 schematicpy-24.1.1/schematic/visualization/tangled_tree.py
--rw-r--r--   0        0        0    19684 1970-01-01 00:00:00.000000 schematicpy-24.1.1/setup.py
--rw-r--r--   0        0        0    19602 1970-01-01 00:00:00.000000 schematicpy-24.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-22 22:30:26.223071 schematicpy-24.2.1/LICENSE
+-rw-r--r--   0        0        0    17325 2024-02-22 22:30:26.223071 schematicpy-24.2.1/README.md
+-rw-r--r--   0        0        0     4064 2024-02-22 22:31:39.504377 schematicpy-24.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1424 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/__init__.py
+-rw-r--r--   0        0        0     1421 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/__main__.py
+-rw-r--r--   0        0        0        0 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/configuration/__init__.py
+-rw-r--r--   0        0        0     7438 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/configuration/configuration.py
+-rw-r--r--   0        0        0     5034 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/configuration/dataclasses.py
+-rw-r--r--   0        0        0      663 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/etc/README.md
+-rw-r--r--   0        0        0    76063 2024-02-22 22:30:26.227072 schematicpy-24.2.1/schematic/etc/data_models/biothings.model.jsonld
+-rw-r--r--   0        0        0  1387510 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/etc/data_models/schema_org.model.jsonld
+-rw-r--r--   0        0        0     4414 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/etc/validation_schemas/class.schema.json
+-rw-r--r--   0        0        0     9914 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/etc/validation_schemas/model.schema.json
+-rw-r--r--   0        0        0     5021 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/etc/validation_schemas/property.schema.json
+-rw-r--r--   0        0        0     3193 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/exceptions.py
+-rw-r--r--   0        0        0    13233 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/help.py
+-rw-r--r--   0        0        0     3415 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/loader.py
+-rw-r--r--   0        0        0       59 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/manifest/__init__.py
+-rw-r--r--   0        0        0    10466 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/manifest/commands.py
+-rw-r--r--   0        0        0    89190 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/manifest/generator.py
+-rw-r--r--   0        0        0    22966 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/GE_Helpers.py
+-rw-r--r--   0        0        0       52 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/__init__.py
+-rw-r--r--   0        0        0     7693 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/commands.py
+-rw-r--r--   0        0        0    18010 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/metadata.py
+-rw-r--r--   0        0        0    45258 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/validate_attribute.py
+-rw-r--r--   0        0        0    12730 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/models/validate_manifest.py
+-rw-r--r--   0        0        0      495 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/__init__.py
+-rw-r--r--   0        0        0     4660 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/commands.py
+-rw-r--r--   0        0        0     4291 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/curie.py
+-rw-r--r--   0        0        0     6081 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/data_model_edges.py
+-rw-r--r--   0        0        0    30011 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/data_model_graph.py
+-rw-r--r--   0        0        0    17905 2024-02-22 22:30:26.231072 schematicpy-24.2.1/schematic/schemas/data_model_json_schema.py
+-rw-r--r--   0        0        0    22193 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_jsonld.py
+-rw-r--r--   0        0        0    12819 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_nodes.py
+-rw-r--r--   0        0        0    22874 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_parser.py
+-rw-r--r--   0        0        0     9561 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_relationships.py
+-rw-r--r--   0        0        0     6924 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/data_model_validator.py
+-rw-r--r--   0        0        0     7070 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/schemas/json_schema_validator.py
+-rw-r--r--   0        0        0       96 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/store/__init__.py
+-rw-r--r--   0        0        0      218 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/store/base.py
+-rw-r--r--   0        0        0   120688 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/store/synapse.py
+-rw-r--r--   0        0        0        0 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/__init__.py
+-rw-r--r--   0        0        0     2920 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/cli_utils.py
+-rw-r--r--   0        0        0     2870 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/curie_utils.py
+-rw-r--r--   0        0        0     9915 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/df_utils.py
+-rw-r--r--   0        0        0    10386 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/general.py
+-rw-r--r--   0        0        0     5769 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/google_api_utils.py
+-rw-r--r--   0        0        0     1221 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/io_utils.py
+-rw-r--r--   0        0        0    17546 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/schema_utils.py
+-rw-r--r--   0        0        0    10288 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/validate_rules_utils.py
+-rw-r--r--   0        0        0     3334 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/validate_utils.py
+-rw-r--r--   0        0        0      563 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/utils/viz_utils.py
+-rw-r--r--   0        0        0      119 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/version.py
+-rw-r--r--   0        0        0      164 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/visualization/__init__.py
+-rw-r--r--   0        0        0    12312 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/visualization/attributes_explorer.py
+-rw-r--r--   0        0        0     4928 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/visualization/commands.py
+-rw-r--r--   0        0        0    40250 2024-02-22 22:30:26.235072 schematicpy-24.2.1/schematic/visualization/tangled_tree.py
+-rw-r--r--   0        0        0    19958 1970-01-01 00:00:00.000000 schematicpy-24.2.1/setup.py
+-rw-r--r--   0        0        0    19961 1970-01-01 00:00:00.000000 schematicpy-24.2.1/PKG-INFO
```

### Comparing `schematicpy-24.1.1/LICENSE` & `schematicpy-24.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/README.md` & `schematicpy-24.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,26 @@
 ```
 4. Install the dependencies by doing: 
 ```
 poetry install
 ```
 This command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)
 
+If you want to install the API you will need to install those dependencies as well:
+
+```
+poetry install --extras "api"
+```
+
+If you want to install the uwsgi:
+
+```
+poetry install --extras "api"
+```
+
 5. Fill in credential files: 
 *Note*: If you won't interact with Synapse, please ignore this section.
 
 There are two main configuration files that need to be edited:
 config.yml
 and [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)
```

### Comparing `schematicpy-24.1.1/pyproject.toml` & `schematicpy-24.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "schematicpy"
-version = "v24.1.1"
+version = "v24.2.1"
 description = "Package for biomedical data model and metadata ingress management"
 authors = [ "Milen Nikolov <milen.nikolov@sagebase.org>", "Lingling Peng <lingling.peng@sagebase.org>", "Mialy Defelice <mialy.defelice@sagebase.org>", "Gianna Jordan <gianna.jordan@sagebase.org>", "Bruno Grande <bruno.grande@sagebase.org>", "Robert Allaway <robert.allaway@sagebionetworks.org>",]
 readme = "README.md"
 homepage = "https://github.com/Sage-Bionetworks/schematic"
 repository = "https://github.com/Sage-Bionetworks/schematic"
 documentation = "https://github.com/Sage-Bionetworks/schematic"
 keywords = [ "schema", "metadata", "validation", "data model", "linked data",]
@@ -33,56 +33,74 @@
 google-auth-oauthlib = "^0.8.0"
 graphviz = "^0.20.0"
 inflection = "^0.5.1"
 jsonschema = "^4.0.0"
 networkx = ">=2.2.8"
 numpy = "^1.21.1"
 oauth2client = "^4.1.0"
-pandas = "^1.3.1"
+pandas = "^2.0.0"
 pygsheets = "^2.0.4"
 PyYAML = "^6.0.0"
 rdflib = "^6.0.0"
 setuptools = "^66.0.0"
-synapseclient = "^3.1.1"
+synapseclient = "^3.2.0"
 tenacity = "^8.0.1"
 toml = "^0.10.2"
-Flask = "^2.0.0"
 great-expectations = "^0.15.0"
 sphinx-click = "^4.0.0"
 MarkupSafe = "2.1.0"
 itsdangerous = "^2.0.0"
-Jinja2 = ">2.11.3"
 openpyxl = "^3.0.9"
-Flask-Cors = "^3.0.10"
 pdoc = "^12.2.0"
 dateparser = "^1.1.4"
 pandarallel = "^1.6.4"
 pyopenssl = "^23.0.0"
 typing-extensions = "<4.6.0"
 dataclasses-json = "^0.6.1"
 
+[tool.poetry.extras]
+api = [ "connexion", "Flask", "Flask-Cors", "Jinja2",]
+aws = [ "uWSGI",]
+
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--verbose"
 testpaths = [ "tests",]
 filterwarnings = [ "ignore::DeprecationWarning",]
 markers = [ "google_credentials_needed: marks tests requiring Google credentials (skipped on GitHub CI) ", "submission: tests that involve submitting manifests\n    ", "not_windows: tests that don't work on on windows machine\n    ", "schematic_api: marks tests covering API functionality (skipped on regular GitHub CI test suite)\n    ", "rule_combos: marks tests covering combinations of rules that aren't always necessary and can add significantly to CI runtime (skipped on GitHub CI unless prompted to run in commit message)\n    ", "table_operations: marks tests covering table operations that pass locally but fail on CI due to interactions with Synapse (skipped on GitHub CI)\n    ", "rule_benchmark: marks tests covering validation rule benchmarking\n    ", "synapse_credentials_needed: marks api tests that require synapse credentials to run\n    ", "empty_token: marks api tests that send empty credentials in the request\n    ",]
 
-[tool.poetry.dependencies.connexion]
-extras = [ "swagger-ui",]
-version = "^2.8.0"
-
 [tool.poetry.dependencies."backports.zoneinfo"]
 markers = "python_version < \"3.9\""
 version = "^0.2.1"
 
 [tool.poetry.dependencies.schematic-db]
-version = "0.0.dev33"
+version = "0.0.34"
 extras = [ "synapse",]
 
+[tool.poetry.dependencies.connexion]
+extras = [ "swagger-ui",]
+version = "^2.8.0"
+optional = true
+
+[tool.poetry.dependencies.Flask]
+version = "^2.0.0"
+optional = true
+
+[tool.poetry.dependencies.Flask-Cors]
+version = "^3.0.10"
+optional = true
+
+[tool.poetry.dependencies.uWSGI]
+version = "^2.0.21"
+optional = true
+
+[tool.poetry.dependencies.Jinja2]
+version = ">2.11.3"
+optional = true
+
 [tool.poetry.group.aws]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.5.1"
@@ -91,8 +109,7 @@
 python-dotenv = "^0.21.0"
 black = "^23.7.0"
 mypy = "^1.4.1"
 pylint = "^2.16.1"
 pytest-xdist = "^3.5.0"
 
 [tool.poetry.group.aws.dependencies]
-uWSGI = "^2.0.21"
```

### Comparing `schematicpy-24.1.1/schematic/__init__.py` & `schematicpy-24.2.1/schematic/__init__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/__main__.py` & `schematicpy-24.2.1/schematic/__main__.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 logger = logging.getLogger()
 click_log.basic_config(logger)
 
 # dict() -> new empty dictionary
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
+
 # invoke_without_command=True -> forces the application not to show aids before losing them with a --h
 @click.group(context_settings=CONTEXT_SETTINGS, invoke_without_command=True)
 @click_log.simple_verbosity_option(logger)
 def main():
     """
     Command line interface to the `schematic` backend services.
     """
@@ -36,10 +37,9 @@
 main.add_command(init_cli)  # add init commands
 main.add_command(manifest_cli)  # add manifest commands
 main.add_command(model_cli)  # add model commands
 main.add_command(schema_cli)  # add schema commands
 main.add_command(viz_cli)  # add viz commands
 
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `schematicpy-24.1.1/schematic/configuration/configuration.py` & `schematicpy-24.2.1/schematic/configuration/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,21 +79,22 @@
             )
 
         self._manifest_config = ManifestConfig(**config.get("manifest", {}))
         self._model_config = ModelConfig(**config.get("model", {}))
         self._google_sheets_config = GoogleSheetsConfig(
             **config.get("google_sheets", {})
         )
-        self._set_asset_store(config.get("asset_store", {}))
+        asset_store_config = config.get("asset_store", None)
+        if asset_store_config:
+            self._set_asset_store(asset_store_config)
 
     def _set_asset_store(self, config: dict[str, Any]) -> None:
         allowed_config_fields = {"synapse"}
-        if not config:
-            pass
-        if not set(config.keys()).issubset(allowed_config_fields):
+        all_fields_are_valid = set(config.keys()).issubset(allowed_config_fields)
+        if not all_fields_are_valid:
             raise ConfigNonAllowedFieldError(
                 "Non allowed fields in asset_store of configuration file.",
                 list(config.keys()),
                 list(allowed_config_fields),
             )
         self._synapse_config = SynapseConfig(**config["synapse"])
 
@@ -177,14 +178,23 @@
         Returns:
             str: The path of the Google service account credentials.
         """
         return normalize_path(
             self._google_sheets_config.service_acct_creds, self._parent_directory
         )
 
+    @service_account_credentials_path.setter
+    def service_account_credentials_path(self, path: str) -> None:
+        """Sets the path of the Google service account credentials.
+
+        Args:
+            path (str): The path of the Google service account credentials.
+        """
+        self._google_sheets_config.service_acct_creds = path
+
     @property
     def google_sheets_master_template_id(self) -> str:
         """
         Returns:
             str: The template id of the google sheet.
         """
         return "1LYS5qE4nV9jzcYw5sXwCza25slDfRA1CIg3cs-hCdpU"
```

### Comparing `schematicpy-24.1.1/schematic/configuration/dataclasses.py` & `schematicpy-24.2.1/schematic/configuration/dataclasses.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/etc/README.md` & `schematicpy-24.2.1/schematic/etc/README.md`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/etc/data_models/biothings.model.jsonld` & `schematicpy-24.2.1/schematic/etc/data_models/biothings.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/etc/data_models/schema_org.model.jsonld` & `schematicpy-24.2.1/schematic/etc/data_models/schema_org.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/etc/validation_schemas/class.schema.json` & `schematicpy-24.2.1/schematic/etc/validation_schemas/class.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/etc/validation_schemas/model.schema.json` & `schematicpy-24.2.1/schematic/etc/validation_schemas/model.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/etc/validation_schemas/property.schema.json` & `schematicpy-24.2.1/schematic/etc/validation_schemas/property.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/exceptions.py` & `schematicpy-24.2.1/schematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/help.py` & `schematicpy-24.2.1/schematic/help.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,14 +50,20 @@
                 "You can either explicitly pass the `.json` file here or provide it in the `config.yml` file "
                 "as a value for the `(model > location)` key."
             ),
             "alphabetize_valid_values": (
                 "Specify to alphabetize valid attribute values either ascending (a) or descending (d)."
                 "Optional"
             ),
+            "data_model_labels": (
+                "Choose how to set the label in the data model. "
+                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
+                "class_label, default, use standard class or property label. "
+                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
+            ),
         },
         "migrate": {
             "short_help": (
                 "Specify the path to the `config.yml` using this option. "
                 "This is a required argument."
             ),
             "project_scope": (
@@ -97,19 +103,14 @@
                 "Specify the synID of the dataset folder on Synapse to which you intend to submit "
                 "the metadata manifest file. This is a required argument."
             ),
             "validate_component": (
                 "The component or data type from the data model which you can use to validate the "
                 "data filled in your manifest template."
             ),
-            "use_schema_label": (
-                "Store attributes using the schema label (--use_schema_label, default) or store attributes using the display label "
-                "(--use_display_label). Attribute display names in the schema must not only include characters that are "
-                "not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'"
-            ),
             "hide_blanks": (
                 "This is a boolean flag. If flag is provided when command line utility is executed, annotations with blank values will be hidden from a dataset's annotation list in Synaspe."
                 "If not, annotations with blank values will be displayed."
             ),
             "manifest_record_type": (
                 "Specify the way the manifest should be store as on Synapse. Options are 'file_only', 'file_and_entities', 'table_and_file' and "
                 "'table_file_and_entities'. 'file_and_entities' will store the manifest as a csv and create Synapse files for each row in the manifest. "
@@ -123,15 +124,30 @@
                 "'replace' will remove the rows and columns from the existing table and store the new rows and columns, preserving the name and synID. "
                 "'upsert' will add the new rows to the table and preserve the exisitng rows and columns in the existing table. "
                 "Default value is 'replace'. "
                 "Upsert specific requirements: {\n}"
                 "'upsert' should be used for initial table uploads if users intend to upsert into them at a later time."
                 "Using 'upsert' at creation will generate the metadata necessary for upsert functionality."
                 "Upsert functionality requires primary keys to be specified in the data model and manfiest as <component>_id."
-                "Currently it is required to use -dl/--use_display_label with table upserts."
+                "Currently it is required to use --table_column_names = display_name with table upserts."
+            ),
+            "annotation_keys": (
+                "Store attributes using the class label (default) or store attributes using the display label. "
+                "Attribute display names in the schema must not only include characters that are "
+                "not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'"
+            ),
+            "table_column_names": (
+                "class_label, display_label, display_name, default, class_label. When true annotations and table columns will be uploaded with the display name formatting with blacklisted characters removed. "
+                "To use for tables, use in conjunction with the use_schema_label flag."
+            ),
+            "data_model_labels": (
+                "Choose how to set the label in the data model. "
+                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
+                "class_label, default, use standard class or property label. "
+                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
             ),
         },
         "validate": {
             "short_help": ("Validation of manifest files."),
             "manifest_path": (
                 "Specify the path to the metadata manifest file that you want to submit to a dataset on Synapse. "
                 "This is a required argument."
@@ -150,14 +166,20 @@
                 "This is a boolean flag. If flag is provided when command line utility is executed, validation suite will only run with in-house validation rules, "
                 "and Great Expectations rules and suite will not be utilized."
                 "If not, the Great Expectations suite will be utilized and all rules will be available."
             ),
             "project_scope": (
                 "Specify a comma-separated list of projects to search through for cross manifest validation."
             ),
+            "data_model_labels": (
+                "Choose how to set the label in the data model. "
+                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
+                "class_label, default, use standard class or property label. "
+                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
+            ),
         },
     }
 }
 
 
 # `schematic schema` related sub-commands description
 schema_commands = {
@@ -165,14 +187,20 @@
         "convert": {
             "short_help": (
                 "Convert specification from CSV data model to JSON-LD data model."
             ),
             "output_jsonld": (
                 "Path to where the generated JSON-LD file needs to be outputted."
             ),
+            "data_model_labels": (
+                "Choose how to set the label in the data model. "
+                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
+                "class_label, default, use standard class or property label. "
+                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
+            ),
         }
     }
 }
 
 
 # `schematic init` command description
 init_command = {
@@ -192,10 +220,16 @@
         "tangled_tree": {
             "figure_type": (
                 "Specify the type of schema visualization to make. Either 'dependency' or 'component'."
             ),
             "text_format": (
                 "Specify the type of text to gather for tangled tree visualization, either 'plain' or 'highlighted'."
             ),
+            "data_model_labels": (
+                "Choose how to set the label in the data model. "
+                "display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to class_label. "
+                "class_label, default, use standard class or property label. "
+                "Do not change from default unless there is a real need, using 'display_label' can have consequences if not used properly."
+            ),
         },
     }
 }
```

### Comparing `schematicpy-24.1.1/schematic/loader.py` & `schematicpy-24.2.1/schematic/loader.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/manifest/commands.py` & `schematicpy-24.2.1/schematic/manifest/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 import click
 import click_log
 
 from schematic.schemas.data_model_parser import DataModelParser
 from schematic.schemas.data_model_graph import DataModelGraph, DataModelGraphExplorer
 from schematic.manifest.generator import ManifestGenerator
 
-from schematic.utils.cli_utils import log_value_from_config, query_dict, parse_synIDs
+from schematic.utils.cli_utils import log_value_from_config, query_dict, parse_syn_ids
 from schematic.utils.google_api_utils import export_manifest_csv
 from schematic.help import manifest_commands
 
 from schematic.store.synapse import SynapseStorage
 from schematic.configuration.configuration import CONFIG
 
-logger = logging.getLogger('schematic')
+logger = logging.getLogger("schematic")
 click_log.basic_config(logger)
 
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
+
 # invoke_without_command=True -> forces the application not to show aids before losing them with a --h
 @click.group(context_settings=CONTEXT_SETTINGS, invoke_without_command=True)
 @click_log.simple_verbosity_option(logger)
 @click.option(
     "-c",
     "--config",
     envvar="SCHEMATIC_CONFIG",
@@ -58,15 +59,17 @@
 )
 @click.option(
     "-dt",
     "--data_type",
     help=query_dict(manifest_commands, ("manifest", "get", "data_type")),
 )
 @click.option(
-    "-p", "--path_to_data_model", help=query_dict(manifest_commands, ("manifest", "get", "path_to_data_model"))
+    "-p",
+    "--path_to_data_model",
+    help=query_dict(manifest_commands, ("manifest", "get", "path_to_data_model")),
 )
 @click.option(
     "-d",
     "--dataset_id",
     help=query_dict(manifest_commands, ("manifest", "get", "dataset_id")),
 )
 @click.option(
@@ -95,158 +98,174 @@
     "-js",
     "--json_schema",
     help=query_dict(manifest_commands, ("manifest", "get", "json_schema")),
 )
 @click.option(
     "-av",
     "--alphabetize_valid_values",
-    default = 'ascending',
+    default="ascending",
     help=query_dict(manifest_commands, ("manifest", "get", "alphabetize_valid_values")),
 )
+@click.option(
+    "--data_model_labels",
+    "-dml",
+    default="class_label",
+    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    help=query_dict(manifest_commands, ("manifest", "get", "data_model_labels")),
+)
 @click.pass_obj
 def get_manifest(
     ctx,
     title,
     data_type,
     path_to_data_model,
     dataset_id,
     sheet_url,
     output_csv,
     use_annotations,
     json_schema,
     output_xlsx,
     alphabetize_valid_values,
+    data_model_labels,
 ):
     """
     Running CLI with manifest generation options.
     """
     # Optional parameters that need to be passed to ManifestGenerator()
     # If CLI parameters are None they are gotten from the CONFIG object and logged
     if data_type is None:
-        data_type =  CONFIG.manifest_data_type
+        data_type = CONFIG.manifest_data_type
         log_value_from_config("data_type", data_type)
     if path_to_data_model is None:
-        path_to_data_model =  CONFIG.model_location
+        path_to_data_model = CONFIG.model_location
         log_value_from_config("path_to_data_model", path_to_data_model)
     if title is None:
-        title =  CONFIG.manifest_title
+        title = CONFIG.manifest_title
         log_value_from_config("title", title)
 
-    data_model_parser = DataModelParser(path_to_data_model = path_to_data_model)
+    data_model_parser = DataModelParser(path_to_data_model=path_to_data_model)
 
-    #Parse Model
+    # Parse Model
     logger.info("Parsing data model.")
     parsed_data_model = data_model_parser.parse_model()
 
     # Instantiate DataModelGraph
-    data_model_grapher = DataModelGraph(parsed_data_model)
+    data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
     # Generate graph
     logger.info("Generating data model graph.")
     graph_data_model = data_model_grapher.generate_data_model_graph()
 
     def create_single_manifest(data_type, output_csv=None, output_xlsx=None):
         # create object of type ManifestGenerator
         manifest_generator = ManifestGenerator(
             path_to_data_model=path_to_data_model,
-            graph = graph_data_model,
+            graph=graph_data_model,
             title=t,
             root=data_type,
             use_annotations=use_annotations,
             alphabetize_valid_values=alphabetize_valid_values,
         )
 
         # call get_manifest() on manifest_generator
         # if output_xlsx gets specified, output_format = "excel"
-        if output_xlsx: 
+        if output_xlsx:
             output_format = "excel"
             # if file name is in the path, and that file does not exist
             if not os.path.exists(output_xlsx):
                 if ".xlsx" or ".xls" in output_xlsx:
                     path = Path(output_xlsx)
                     output_path = path.parent.absolute()
                     if not os.path.exists(output_path):
                         raise ValueError(
                             f"{output_path} does not exists. Please try a valid file path"
                         )
                 else:
                     raise ValueError(
-                            f"{output_xlsx} does not exists. Please try a valid file path"
-                        )
+                        f"{output_xlsx} does not exists. Please try a valid file path"
+                    )
             else:
                 # Check if base path itself exists.
                 if not os.path.exists(os.path.dirname(output_xlsx)):
                     raise ValueError(
-                    f"{output_xlsx} does not exists. Please try a valid file path"
+                        f"{output_xlsx} does not exists. Please try a valid file path"
                     )
                 output_path = output_xlsx
-        else: 
+        else:
             output_format = None
             output_path = None
 
         result = manifest_generator.get_manifest(
-            dataset_id=dataset_id, sheet_url=sheet_url, json_schema=json_schema, output_format = output_format, output_path = output_path
+            dataset_id=dataset_id,
+            sheet_url=sheet_url,
+            json_schema=json_schema,
+            output_format=output_format,
+            output_path=output_path,
         )
 
         if sheet_url:
             logger.info("Find the manifest template using this Google Sheet URL:")
             click.echo(result)
-        if output_csv is None and output_xlsx is None: 
+        if output_csv is None and output_xlsx is None:
             prefix, _ = os.path.splitext(path_to_data_model)
             prefix_root, prefix_ext = os.path.splitext(prefix)
             if prefix_ext == ".model":
                 prefix = prefix_root
             output_csv = f"{prefix}.{data_type}.manifest.csv"
 
         elif output_xlsx:
             logger.info(
                 f"Find the manifest template using this Excel file path: {output_xlsx}"
             )
             return result
         export_manifest_csv(file_path=output_csv, manifest=result)
         logger.info(
-                f"Find the manifest template using this CSV file path: {output_csv}"
-            )
+            f"Find the manifest template using this CSV file path: {output_csv}"
+        )
         return result
 
     if type(data_type) is str:
         data_type = [data_type]
 
-    if data_type[0] == 'all manifests':      
+    if data_type[0] == "all manifests":
         # Feed graph into the data model graph explorer
         dmge = DataModelGraphExplorer(graph_data_model)
-        component_digraph = dmge.get_digraph_by_edge_type('requiresComponent')
+        component_digraph = dmge.get_digraph_by_edge_type("requiresComponent")
         components = component_digraph.nodes()
         for component in components:
-            t = f'{title}.{component}.manifest'
-            result = create_single_manifest(data_type = component)
+            t = f"{title}.{component}.manifest"
+            result = create_single_manifest(data_type=component)
     else:
         for dt in data_type:
             if len(data_type) > 1 and not output_xlsx:
-                t = f'{title}.{dt}.manifest'
-            elif output_xlsx: 
+                t = f"{title}.{dt}.manifest"
+            elif output_xlsx:
                 if ".xlsx" or ".xls" in output_xlsx:
                     title_with_extension = os.path.basename(output_xlsx)
-                    t = title_with_extension.split('.')[0]
+                    t = title_with_extension.split(".")[0]
             else:
                 t = title
-            result = create_single_manifest(data_type = dt, output_csv=output_csv, output_xlsx=output_xlsx)
+            result = create_single_manifest(
+                data_type=dt, output_csv=output_csv, output_xlsx=output_xlsx
+            )
 
     return result
 
+
 @manifest.command(
-    "migrate", short_help=query_dict(manifest_commands, ("manifest", "migrate", "short_help"))
+    "migrate",
+    short_help=query_dict(manifest_commands, ("manifest", "migrate", "short_help")),
 )
 @click_log.simple_verbosity_option(logger)
 # define the optional arguments
 @click.option(
     "-ps",
     "--project_scope",
     default=None,
-    callback=parse_synIDs,
+    callback=parse_syn_ids,
     help=query_dict(manifest_commands, ("manifest", "migrate", "project_scope")),
 )
 @click.option(
     "-ap",
     "--archive_project",
     default=None,
     help=query_dict(manifest_commands, ("manifest", "migrate", "archive_project")),
@@ -277,22 +296,26 @@
     return_entities: bool,
     dry_run: bool,
 ):
     """
     Running CLI with manifest migration options.
     """
     if jsonld is None:
-        jsonld =  CONFIG.model_location
+        jsonld = CONFIG.model_location
         log_value_from_config("jsonld", jsonld)
 
     full_scope = project_scope + [archive_project]
-    synStore = SynapseStorage(project_scope = full_scope)  
+    synStore = SynapseStorage(project_scope=full_scope)
 
     for project in project_scope:
         if not return_entities:
             logging.info("Re-uploading manifests as tables")
-            synStore.upload_annotated_project_manifests_to_synapse(project, jsonld, dry_run)
+            synStore.upload_annotated_project_manifests_to_synapse(
+                project, jsonld, dry_run
+            )
         if archive_project:
             logging.info("Migrating entitites")
-            synStore.move_entities_to_new_project(project, archive_project, return_entities, dry_run)
-        
-    return 
+            synStore.move_entities_to_new_project(
+                project, archive_project, return_entities, dry_run
+            )
+
+    return
```

### Comparing `schematicpy-24.1.1/schematic/manifest/generator.py` & `schematicpy-24.2.1/schematic/manifest/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,46 +6,46 @@
 from openpyxl import load_workbook
 from openpyxl.utils.dataframe import dataframe_to_rows
 import os
 import pandas as pd
 from pathlib import Path
 import pygsheets as ps
 from tempfile import NamedTemporaryFile
-from typing import Dict, List, Optional, Tuple, Union, BinaryIO, Literal
-from flask import send_from_directory
+from typing import Any, Dict, List, Optional, Tuple, Union, BinaryIO, Literal
 
 from schematic.schemas.data_model_graph import DataModelGraph, DataModelGraphExplorer
 from schematic.schemas.data_model_parser import DataModelParser
 from schematic.schemas.data_model_json_schema import DataModelJSONSchema
 
 from schematic.utils.google_api_utils import (
     execute_google_api_requests,
     build_service_account_creds,
 )
 from schematic.utils.df_utils import update_df, load_df
+from schematic.utils.schema_utils import extract_component_validation_rules
 from schematic.utils.validate_utils import rule_in_rule_list
+from schematic.utils.schema_utils import DisplayLabelType
 
-#TODO: This module should only be aware of the store interface
+# TODO: This module should only be aware of the store interface
 # we shouldn't need to expose Synapse functionality explicitly
 from schematic.store.synapse import SynapseStorage
 
 from schematic.configuration.configuration import CONFIG
 from schematic.utils.google_api_utils import export_manifest_drive_service
 
 
 logger = logging.getLogger(__name__)
 
 
-
 class ManifestGenerator(object):
     def __init__(
         self,
         path_to_data_model: str,  # JSON-LD file to be used for generating the manifest
-        graph: nx.MultiDiGraph, # At this point, the graph is fully formed.
-        alphabetize_valid_values: str = 'ascending',
+        graph: nx.MultiDiGraph,  # At this point, the graph is fully formed.
+        alphabetize_valid_values: str = "ascending",
         title: str = None,  # manifest sheet title
         root: str = None,
         additional_metadata: Dict = None,
         use_annotations: bool = False,
     ) -> None:
         # use service account creds
         services_creds = build_service_account_creds()
@@ -91,23 +91,25 @@
             )
 
         # Instantiate Data Model Explorer object
         self.dmge = DataModelGraphExplorer(self.graph)
 
         # additional metadata to add to manifest
         self.additional_metadata = additional_metadata
-   
+
         # Check if the class is in the schema
         root_in_schema = self.dmge.is_class_in_schema(self.root)
-        
+
         # If the class could not be found, give a notification
         if not root_in_schema:
-            exception_message = f"The DataType entered ({self.root}) could not be found in the data model schema. " + \
-                                "Please confirm that the datatype is in the data model and that the spelling matches the class label in the .jsonld file."
-            raise LookupError(exception_message) 
+            exception_message = (
+                f"The DataType entered ({self.root}) could not be found in the data model schema. "
+                + "Please confirm that the datatype is in the data model and that the spelling matches the class label in the .jsonld file."
+            )
+            raise LookupError(exception_message)
 
         # Determine whether current data type is file-based
         self.is_file_based = "Filename" in self.dmge.get_node_dependencies(self.root)
 
     def _attribute_to_letter(self, attribute, manifest_fields):
         """Map attribute to column letter in a google sheet"""
 
@@ -188,15 +190,15 @@
         # return new copy sheet ID
         return (
             self.drive_service.files()
             .copy(fileId=origin_file_id, body=copied_file)
             .execute()["id"]
         )
 
-    def _create_empty_manifest_spreadsheet(self, title:str) -> str:
+    def _create_empty_manifest_spreadsheet(self, title: str) -> str:
         """
         Creates an empty google spreadsheet returning the id.
         If the configuration has a template id it will be used
 
         Args:
             title (str): The title of the spreadsheet
 
@@ -205,29 +207,26 @@
         """
         template_id = CONFIG.google_sheets_master_template_id
 
         if template_id:
             spreadsheet_id = self._gdrive_copy_file(template_id, title)
 
         else:
-            spreadsheet_body = {
-                'properties': {
-                    'title': title
-                }
-            }
+            spreadsheet_body = {"properties": {"title": title}}
 
-            spreadsheet_id = self.sheet_service.spreadsheets().create(
-                body=spreadsheet_body,
-                fields="spreadsheetId").execute().get("spreadsheetId"
+            spreadsheet_id = (
+                self.sheet_service.spreadsheets()
+                .create(body=spreadsheet_body, fields="spreadsheetId")
+                .execute()
+                .get("spreadsheetId")
             )
 
         return spreadsheet_id
 
     def _get_cell_borders(self, cell_range):
-
         # set border style request
         color = {
             "red": 226.0 / 255.0,
             "green": 227.0 / 255.0,
             "blue": 227.0 / 255.0,
         }
 
@@ -255,34 +254,38 @@
 
         batch = self.drive_service.new_batch_http_request(callback=callback)
 
         worldPermission = {"type": "anyone", "role": "writer"}
 
         batch.add(
             self.drive_service.permissions().create(
-                fileId=fileId, body=worldPermission, fields="id",
+                fileId=fileId,
+                body=worldPermission,
+                fields="id",
             )
         )
         batch.execute()
 
-    def _store_valid_values_as_data_dictionary(self, column_id:int, valid_values:list, spreadsheet_id:str) -> list:
-        '''store valid values in google sheet (sheet 2). This step is required for "ONE OF RANGE" validation
+    def _store_valid_values_as_data_dictionary(
+        self, column_id: int, valid_values: list, spreadsheet_id: str
+    ) -> list:
+        """store valid values in google sheet (sheet 2). This step is required for "ONE OF RANGE" validation
         Args:
             column_id: id of column
             valid_values: a list of valid values for a given attribute (i.e. for diagnosis, this looks like: [{'userEnteredValue': 'Cancer'}, {'userEnteredValue': 'Healthy'}])
             spreadsheet_id: google spreadsheet id
-        
+
         return: range of valid values (i.e. for diagnosis, [{'userEnteredValue': '=Sheet2!D2:D3'}])
-        '''
+        """
         # get valid values w/o google sheet header
         values = [valid_value["userEnteredValue"] for valid_value in valid_values]
-        
-        if self.alphabetize and self.alphabetize.lower().startswith('a'):
+
+        if self.alphabetize and self.alphabetize.lower().startswith("a"):
             values.sort(reverse=False, key=str.lower)
-        elif self.alphabetize and self.alphabetize.lower().startswith('d'):
+        elif self.alphabetize and self.alphabetize.lower().startswith("d"):
             values.sort(reverse=True, key=str.lower)
 
         # store valid values explicitly in workbook at the provided range to use as validation values
         target_col_letter = self._column_to_letter(column_id)
         body = {"majorDimension": "COLUMNS", "values": [values]}
         target_range = (
             "Sheet2!"
@@ -306,26 +309,27 @@
         return valid_values
 
     def _get_column_data_validation_values(
         self,
         spreadsheet_id,
         valid_values,
         column_id,
-        strict:Optional[bool],
+        strict: Optional[bool],
         validation_type="ONE_OF_LIST",
         custom_ui=True,
         input_message="Choose one from dropdown",
     ):
-
         # set validation strictness to config file default if None indicated.
         if strict == None:
             strict = CONFIG.google_sheets_strict_validation
-        #store valid values explicitly in workbook at the provided range to use as validation values
+        # store valid values explicitly in workbook at the provided range to use as validation values
         if validation_type == "ONE_OF_RANGE":
-            valid_values=self._store_valid_values_as_data_dictionary(column_id, valid_values, spreadsheet_id)
+            valid_values = self._store_valid_values_as_data_dictionary(
+                column_id, valid_values, spreadsheet_id
+            )
 
         # setup validation data request body
         validation_body = {
             "requests": [
                 {
                     "setDataValidation": {
                         "range": {
@@ -363,27 +367,30 @@
         if "enum" in prop:
             return prop["enum"]
         elif "items" in prop:
             return prop["items"]["enum"]
         else:
             return []
 
-
     def _get_json_schema(self, json_schema_filepath: str) -> Dict:
         """Open json schema as a dictionary.
         Args:
             json_schema_filepath(str): path to json schema file
         Returns:
             Dictionary, containing portions of the json schema
         TODO: Do we even allow people to provide a json_schema_filepath anyore?
         """
         if not json_schema_filepath:
             # TODO Catch error if no JSONLD or JSON path provided.
-            data_model_js = DataModelJSONSchema(jsonld_path=self.model_path, graph=self.graph)
-            json_schema = data_model_js.get_json_validation_schema(source_node=self.root, schema_name=self.title)
+            data_model_js = DataModelJSONSchema(
+                jsonld_path=self.model_path, graph=self.graph
+            )
+            json_schema = data_model_js.get_json_validation_schema(
+                source_node=self.root, schema_name=self.title
+            )
         else:
             with open(json_schema_filepath) as jsonfile:
                 json_schema = json.load(jsonfile)
         return json_schema
 
     def _get_required_metadata_fields(self, json_schema, fields):
         """For the root node gather dependency requirements (all attributes linked to this node)
@@ -473,15 +480,15 @@
             contain {'Component': [self.root]}
         """
         if "Component" in required_metadata_fields.keys():
             # check if additional metadata has actually been instantiated in the
             # constructor (it's optional) if not, instantiate it
             if not self.additional_metadata:
                 self.additional_metadata = {}
-            if self.is_file_based and 'Filename' in self.additional_metadata:
+            if self.is_file_based and "Filename" in self.additional_metadata:
                 self.additional_metadata["Component"] = [self.root] * max(
                     1, len(self.additional_metadata["Filename"])
                 )
             else:
                 self.additional_metadata["Component"] = [self.root]
         return
 
@@ -687,15 +694,15 @@
                         "fields": "userEnteredFormat(textFormat)",
                     }
                 }
             ]
         }
         return vr_format_body
 
-    def _request_regex_vr(self, gs_formula, i:int, text_color={"red": 1}):
+    def _request_regex_vr(self, gs_formula, i: int, text_color={"red": 1}):
         """
         Generate request to change font color to black upon corretly formatted
         user entry.
         """
         requests_vr = {
             "requests": [
                 {
@@ -708,30 +715,33 @@
                             },
                             "booleanRule": {
                                 "condition": {
                                     "type": "CUSTOM_FORMULA",
                                     "values": gs_formula,
                                 },
                                 "format": {
-                                    "textFormat": {
-                                        "foregroundColor": text_color
-                                    }
+                                    "textFormat": {"foregroundColor": text_color}
                                 },
                             },
                         },
                         "index": 0,
                     }
                 }
             ]
         }
         return requests_vr
 
-    def _request_regex_match_vr_formatting(self, validation_rules: List[str], i: int,
-        spreadsheet_id: str, requests_body: dict, strict: Optional[bool],
-        ):
+    def _request_regex_match_vr_formatting(
+        self,
+        validation_rules: List[str],
+        i: int,
+        spreadsheet_id: str,
+        requests_body: dict,
+        strict: Optional[bool],
+    ):
         """
         Purpose:
             - Apply regular expression validaiton rules to google sheets.
             - Will only be run if the regex module specified in the validation
             rules is 'match'.
                 - This is because of the limitations of google sheets regex.
                 - Users can additionally add 'strict' to the end of their validation
@@ -781,15 +791,15 @@
             ## Change request to change the text color of the column we are validating to red.
             requests_vr_format_body = self._request_update_base_color(
                 i,
                 color={
                     "red": 232.0 / 255.0,
                     "green": 80.0 / 255.0,
                     "blue": 70.0 / 255.0,
-                }
+                },
             )
 
             ## Create request to for conditionally formatting user input.
             requests_vr = self._request_regex_vr(gs_formula, i, text_color)
 
             ## Create request to generate data validator.
             requests_data_validation_vr = self._get_column_data_validation_values(
@@ -798,37 +808,32 @@
                 column_id=i,
                 strict=strict,
                 custom_ui=False,
                 input_message=input_message,
                 validation_type="CUSTOM_FORMULA",
             )
 
-            requests_body["requests"].append(
-                requests_vr_format_body["requests"]
-            )
+            requests_body["requests"].append(requests_vr_format_body["requests"])
             requests_body["requests"].append(requests_vr["requests"])
-            requests_body["requests"].append(
-                requests_data_validation_vr["requests"]
-            )
+            requests_body["requests"].append(requests_data_validation_vr["requests"])
         return requests_body
 
-
     def _request_row_format(self, i, req):
         """Adding description to headers, this is not executed if
         only JSON schema is defined. Also formatting required columns.
         Args:
             i (int): column index
             req (str): column name
         Returns:
             notes_body["requests"] (dict): with information on note
                 to add to the column header. This notes body will be added to a request.
         """
         if self.dmge:
             # get node definition
-            note = self.dmge.get_node_comment(node_display_name = req)
+            note = self.dmge.get_node_comment(node_display_name=req)
 
             notes_body = {
                 "requests": [
                     {
                         "updateCells": {
                             "range": {
                                 "startRowIndex": 0,
@@ -862,15 +867,15 @@
             valid_values(list[str]): containing all valid values defined in the
                 data model for this node/column
 
         Returns:
             notes_body["requests"] (dict): with information on note
                 to add to the column header, about using multiselect.
                 This notes body will be added to a request.
-        """            
+        """
         if rule_in_rule_list("list", validation_rules) and valid_values:
             note = "Please enter applicable comma-separated items selected from the set of allowable terms for this attribute. See our data standards for allowable terms"
             notes_body = {
                 "requests": [
                     {
                         "repeatCell": {
                             "range": {
@@ -882,15 +887,17 @@
                             "fields": "note",
                         }
                     }
                 ]
             }
             return notes_body["requests"]
         elif rule_in_rule_list("list", validation_rules) and not valid_values:
-            note = "Please enter values as a comma separated list. For example: XX, YY, ZZ"
+            note = (
+                "Please enter values as a comma separated list. For example: XX, YY, ZZ"
+            )
             notes_body = {
                 "requests": [
                     {
                         "repeatCell": {
                             "range": {
                                 "startRowIndex": 1,
                                 "startColumnIndex": i,
@@ -985,16 +992,20 @@
         else:
             validation_body = self._get_column_data_validation_values(
                 spreadsheet_id, req_vals, i, strict=None
             )
         return validation_body["requests"]
 
     def _dependency_formatting(
-        self, i, req_val, ordered_metadata_fields, val_dependencies,
-        dependency_formatting_body
+        self,
+        i,
+        req_val,
+        ordered_metadata_fields,
+        val_dependencies,
+        dependency_formatting_body,
     ):
         """If there are additional attribute dependencies find the corresponding
         fields that need to be filled in and construct conditional formatting rules
         indicating the dependencies need to be filled in.
 
         set target ranges for this rule
         i.e. dependency attribute columns that will be formatted
@@ -1039,17 +1050,15 @@
                     "rule": {
                         "ranges": rule_ranges[j],
                         "booleanRule": formatting_rule,
                     },
                     "index": 0,
                 }
             }
-            dependency_formatting_body["requests"].append(
-                            conditional_format_rule
-                        )
+            dependency_formatting_body["requests"].append(conditional_format_rule)
         return dependency_formatting_body["requests"]
 
     def _request_dependency_formatting(
         self, i, req_vals, ordered_metadata_fields, requests_body
     ):
         """Gather all the formattng for node dependencies.
         Args:
@@ -1078,22 +1087,23 @@
 
             # prepare request calls
             dependency_formatting_body = {"requests": []}
 
             # set conditiaon formatting for dependencies.
             if val_dependencies:
                 dependency_formatting_body["requests"] = self._dependency_formatting(
-                    i, req_val, ordered_metadata_fields, val_dependencies,
-                    dependency_formatting_body
+                    i,
+                    req_val,
+                    ordered_metadata_fields,
+                    val_dependencies,
+                    dependency_formatting_body,
                 )
 
             if dependency_formatting_body["requests"]:
-                requests_body["requests"].append(
-                    dependency_formatting_body["requests"]
-                )
+                requests_body["requests"].append(dependency_formatting_body["requests"])
         return requests_body
 
     def _create_requests_body(
         self,
         required_metadata_fields,
         ordered_metadata_fields,
         json_schema,
@@ -1121,36 +1131,44 @@
                 containing all the update requests to add to the gs
         """
         # store all requests to execute at once
         requests_body = {}
         requests_body["requests"] = []
         for i, req in enumerate(ordered_metadata_fields[0]):
             # Gather validation rules and valid values for attribute.
-            validation_rules = self.dmge.get_node_validation_rules(node_display_name=req)
-            
+            validation_rules = self.dmge.get_node_validation_rules(
+                node_display_name=req
+            )
+            if isinstance(validation_rules, dict):
+                validation_rules = extract_component_validation_rules(
+                    validation_rules=validation_rules, manifest_component=self.root
+                )
+
             # Add regex match validaiton rule to Google Sheets.
             if validation_rules and sheet_url:
-                requests_body =self._request_regex_match_vr_formatting(
-                        validation_rules, i, spreadsheet_id, requests_body, strict
-                        )
+                requests_body = self._request_regex_match_vr_formatting(
+                    validation_rules, i, spreadsheet_id, requests_body, strict
+                )
 
             if req in json_schema["properties"].keys():
                 valid_values = self._get_valid_values_from_jsonschema_property(
                     json_schema["properties"][req]
                 )
             else:
                 valid_values = []
 
             # Set row formatting
             get_row_formatting = self._request_row_format(i, req)
             if get_row_formatting:
                 requests_body["requests"].append(get_row_formatting)
 
             # set color of required columns to blue
-            required_columns_color = self._set_required_columns_color(i, req, json_schema)
+            required_columns_color = self._set_required_columns_color(
+                i, req, json_schema
+            )
             if required_columns_color:
                 requests_body["requests"].append(required_columns_color)
             # Add note on how to use multi-select, when appropriate
             note_vv = self._request_note_valid_values(
                 i, req, validation_rules, valid_values
             )
             if note_vv:
@@ -1161,36 +1179,45 @@
             req_vals = [{"userEnteredValue": value} for value in values if value]
             if not req_vals:
                 continue
 
             # for attributes that don't require "list", create dropdown options and set up data validation rules
             if not rule_in_rule_list("list", validation_rules):
                 create_dropdown = self._request_dropdown(
-                i, req_vals, spreadsheet_id, validation_rules, valid_values
-            )
+                    i, req_vals, spreadsheet_id, validation_rules, valid_values
+                )
                 if create_dropdown:
                     requests_body["requests"].append(create_dropdown)
 
             # for attributes that require "list", simply store valid values (if any) in second sheet
-            elif len(req_vals)>0 and rule_in_rule_list("list", validation_rules):
+            elif len(req_vals) > 0 and rule_in_rule_list("list", validation_rules):
                 self._store_valid_values_as_data_dictionary(i, req_vals, spreadsheet_id)
 
             # generate a conditional format rule for each required value (i.e. valid value)
             # for this field (i.e. if this field is set to a valid value that may require additional
             # fields to be filled in, these additional fields will be formatted in a custom style (e.g. red background)
 
-            requests_body = self._request_dependency_formatting(i, req_vals, ordered_metadata_fields, requests_body)
-           
+            requests_body = self._request_dependency_formatting(
+                i, req_vals, ordered_metadata_fields, requests_body
+            )
+
         # Set borders formatting
         borders_formatting = self._request_cell_borders()
         if borders_formatting:
             requests_body["requests"].append(borders_formatting)
         return requests_body
 
-    def _create_empty_gs(self, required_metadata_fields, json_schema, spreadsheet_id, sheet_url, strict: Optional[bool]):
+    def _create_empty_gs(
+        self,
+        required_metadata_fields,
+        json_schema,
+        spreadsheet_id,
+        sheet_url,
+        strict: Optional[bool],
+    ):
         """Generate requests to add columns and format the google sheet.
         Args:
             required_metadata_fields(dict):
                 keys: of all the fields/attributes that need to be added
                     to the manifest
                 values(list[str]): valid values
             json_schema: dict, representing a handful of values
@@ -1258,15 +1285,20 @@
 
         # Add additional metadata as entries to columns
         required_metadata_fields = self._get_additional_metadata(
             required_metadata_fields
         )
         return required_metadata_fields
 
-    def get_empty_manifest(self, strict: Optional[bool], json_schema_filepath: str=None, sheet_url: Optional[bool]=None):
+    def get_empty_manifest(
+        self,
+        strict: Optional[bool],
+        json_schema_filepath: str = None,
+        sheet_url: Optional[bool] = None,
+    ):
         """Create an empty manifest using specifications from the
         json schema.
         Args:
             strict (bool): strictness with which to apply validation rules to google sheets. If true, blocks incorrect entries; if false, raises a warning
             json_schema_filepath (str): path to json schema file
             sheet_url (Will be deprecated): a boolean ; determine if a pandas dataframe or a google sheet url gets return
             strict (Optional Bool): strictness with which to apply validation rules to google sheets. True, blocks incorrect entries, False, raises a warning
@@ -1279,31 +1311,38 @@
         json_schema = self._get_json_schema(json_schema_filepath=json_schema_filepath)
 
         required_metadata_fields = self._gather_all_fields(
             json_schema["properties"].keys(), json_schema
         )
 
         manifest_url = self._create_empty_gs(
-            required_metadata_fields, json_schema, spreadsheet_id, sheet_url=sheet_url, strict=strict,
+            required_metadata_fields,
+            json_schema,
+            spreadsheet_id,
+            sheet_url=sheet_url,
+            strict=strict,
         )
         return manifest_url
 
-    def _get_missing_columns(self, headers_1:list , headers_2:list) -> list:
+    def _get_missing_columns(self, headers_1: list, headers_2: list) -> list:
         """Compare two colunm sets and get cols that are in headers_1, but not headers_2
         Args:
             headers_1 (list): list of column headers
             headers_2 (list): list of column headers
-        Returns: 
+        Returns:
             list: column headers in headers_1 but not headers_2
 
         """
         return set(headers_1) - set(headers_2)
 
     def set_dataframe_by_url(
-        self, manifest_url: str, manifest_df: pd.DataFrame, out_of_schema_columns: set =None,
+        self,
+        manifest_url: str,
+        manifest_df: pd.DataFrame,
+        out_of_schema_columns: set = None,
     ) -> ps.Spreadsheet:
         """Update Google Sheets using given pandas DataFrame.
         Args:
             manifest_url (str): Google Sheets URL.
             manifest_df (pd.DataFrame): Data frame to "upload".
             out_of_schema_columns (set): Columns that are in downloaded manifest, but not in current schema.
         Returns:
@@ -1320,18 +1359,21 @@
 
         wb.set_dataframe(manifest_df, (1, 1), fit=True)
 
         # update validation rules (i.e. no validation rules) for out of schema columns, if any
         # TODO: similarly clear formatting for out of schema columns, if any
         if out_of_schema_columns:
             num_out_of_schema_columns = len(out_of_schema_columns)
-            start_col = self._column_to_letter(len(manifest_df.columns) - num_out_of_schema_columns) # find start of out of schema columns
-            end_col = self._column_to_letter(len(manifest_df.columns) + 1) # find end of out of schema columns
-            wb.set_data_validation(start = start_col, end = end_col, condition_type = None)
-        
+            start_col = self._column_to_letter(
+                len(manifest_df.columns) - num_out_of_schema_columns
+            )  # find start of out of schema columns
+            end_col = self._column_to_letter(
+                len(manifest_df.columns) + 1
+            )  # find end of out of schema columns
+            wb.set_data_validation(start=start_col, end=end_col, condition_type=None)
 
         # set permissions so that anyone with the link can edit
         sh.share("", role="writer", type="anyone")
 
         return sh
 
     def get_dataframe_by_url(self, manifest_url: str) -> pd.DataFrame:
@@ -1380,15 +1422,15 @@
         # Generate a dictionary mapping labels to display names
         label_map = {l: model_nodes[l]["displayName"] for l in labels}
 
         # Use the above dictionary to rename columns in question
         return annotations.rename(columns=label_map)
 
     def get_manifest_with_annotations(
-        self, annotations: pd.DataFrame, strict: Optional[bool]=None
+        self, annotations: pd.DataFrame, strict: Optional[bool] = None
     ) -> Tuple[ps.Spreadsheet, pd.DataFrame]:
         """Generate manifest, optionally with annotations (if requested).
         Args:
             annotations (pd.DataFrame): Annotations table (can be empty).
             strict (Optional Bool): strictness with which to apply validation rules to google sheets. True, blocks incorrect entries, False, raises a warning
         Returns:
             Tuple[ps.Spreadsheet, pd.DataFrame]: Both the Google Sheet
@@ -1419,335 +1461,464 @@
         # a data frame whose columns are in the same order
         manifest_df = update_df(manifest_df, annotations)
         manifest_sh = self.set_dataframe_by_url(manifest_url, manifest_df)
         manifest_url = manifest_sh.url
 
         return manifest_url, manifest_df
 
-    def export_sheet_to_excel(self, title: str = None, manifest_url : str = None, output_location: str = None) -> str:
+    def export_sheet_to_excel(
+        self, title: str = None, manifest_url: str = None, output_location: str = None
+    ) -> str:
         """
         export manifest as an Excel spreadsheet and return local file path
         Args:
             title: title of the exported excel spreadsheet
-            manifest_url: manifest google sheet url 
+            manifest_url: manifest google sheet url
             output_location: the location where the exported excel file would live
-        return: 
-            Export manifest to a desired location. 
+        return:
+            Export manifest to a desired location.
         """
         # construct file name
         file_name = title + ".xlsx"
-        #if file path exists and it contains a file name: 
-        if output_location: 
+        # if file path exists and it contains a file name:
+        if output_location:
             if os.path.exists(output_location):
-                if Path(output_location).suffix == '.xlsx' or Path(output_location).suffix == '.xls':
+                if (
+                    Path(output_location).suffix == ".xlsx"
+                    or Path(output_location).suffix == ".xls"
+                ):
                     output_excel_file_path = output_location
                 # if users define the location but it doesn't contain a file name, we should add the file name:
                 else:
                     output_excel_file_path = os.path.join(output_location, file_name)
-    
+
         # trigger a warning if file path is provided but does not exist
         elif output_location and not os.path.exists(output_location):
-            output_excel_file_path = os.path.abspath(os.path.join(os.getcwd(), file_name))
-            logger.warning(f'{output_location} does not exist. Using current working directory {output_excel_file_path}')
+            output_excel_file_path = os.path.abspath(
+                os.path.join(os.getcwd(), file_name)
+            )
+            logger.warning(
+                f"{output_location} does not exist. Using current working directory {output_excel_file_path}"
+            )
         # otherwise, use the default location
         else:
-            output_excel_file_path = os.path.abspath(os.path.join(os.getcwd(), file_name))
-        
+            output_excel_file_path = os.path.abspath(
+                os.path.join(os.getcwd(), file_name)
+            )
+
         # export the manifest to excel
-        export_manifest_drive_service(manifest_url, file_path=output_excel_file_path, mimeType = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
-        
+        export_manifest_drive_service(
+            manifest_url,
+            file_path=output_excel_file_path,
+            mime_type="application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
+        )
+
         return output_excel_file_path
 
-    def _handle_output_format_logic(self, output_format: str = None, output_path: str = None, sheet_url: bool = None, empty_manifest_url: str = None, dataframe: pd.DataFrame = None, out_of_schema_columns: set =None):
+    def _handle_output_format_logic(
+        self,
+        output_format: str = None,
+        output_path: str = None,
+        sheet_url: bool = None,
+        empty_manifest_url: str = None,
+        dataframe: pd.DataFrame = None,
+        out_of_schema_columns: set = None,
+    ):
         """
         Handle the logic between sheet_url parameter and output_format parameter to determine the type of output to return
-        Args: 
+        Args:
             output_format: Determines if Google sheet URL, pandas dataframe, or Excel spreadsheet gets returned.
             sheet_url (Will be deprecated): a boolean ; determine if a pandas dataframe or a google sheet url gets return
-            empty_manifest_url: Google sheet URL that leads to an empty manifest 
+            empty_manifest_url: Google sheet URL that leads to an empty manifest
             dataframe: the pandas dataframe that contains the metadata that needs to be populated to an empty manifest
             output_path: Determines the output path of the exported manifest (only relevant if returning an excel spreadsheet)
             out_of_schema_columns (set): Columns that are in downloaded manifest, but not in current schema.
-        Return: 
-            a pandas dataframe, file path of an excel spreadsheet, or a google sheet URL 
+        Return:
+            a pandas dataframe, file path of an excel spreadsheet, or a google sheet URL
         TODO:
             Depreciate sheet URL and add google_sheet as an output_format choice.
         """
 
-        # if the output type gets set to "dataframe", return a data frame 
+        # if the output type gets set to "dataframe", return a data frame
         if output_format == "dataframe":
             return dataframe
-        
+
         # if the output type gets set to "excel", return an excel spreadsheet
-        elif output_format == "excel":              
+        elif output_format == "excel":
             # export manifest url that only contains column headers to Excel
-            output_file_path = self.export_sheet_to_excel(title = self.title,
-                                                          manifest_url = empty_manifest_url,
-                                                          output_location = output_path,
-                                                          )
+            output_file_path = self.export_sheet_to_excel(
+                title=self.title,
+                manifest_url=empty_manifest_url,
+                output_location=output_path,
+            )
 
             # populate an excel spreadsheet with the existing dataframe
             self.populate_existing_excel_spreadsheet(output_file_path, dataframe)
 
             return output_file_path
-        
+
         # Return google sheet if sheet_url flag is raised.
         elif sheet_url:
-            manifest_sh = self.set_dataframe_by_url(manifest_url=empty_manifest_url, manifest_df=dataframe, out_of_schema_columns=out_of_schema_columns)
+            manifest_sh = self.set_dataframe_by_url(
+                manifest_url=empty_manifest_url,
+                manifest_df=dataframe,
+                out_of_schema_columns=out_of_schema_columns,
+            )
             return manifest_sh.url
-        
+
         # Default return a DataFrame
         else:
             return dataframe
-    
+
     @staticmethod
-    def create_single_manifest(path_to_data_model: str, graph_data_model: nx.MultiDiGraph, data_type: str, access_token:Optional[str]=None, dataset_id:Optional[str]=None, strict:Optional[bool]=True, title:Optional[str]=None, output_format:Literal["google_sheet", "excel", "dataframe"]="google_sheet", use_annotations:Optional[bool]=False) -> Union[str, pd.DataFrame, BinaryIO]:
+    def create_single_manifest(
+        path_to_data_model: str,
+        graph_data_model: nx.MultiDiGraph,
+        data_type: str,
+        access_token: Optional[str] = None,
+        dataset_id: Optional[str] = None,
+        strict: Optional[bool] = True,
+        title: Optional[str] = None,
+        output_format: Literal["google_sheet", "excel", "dataframe"] = "google_sheet",
+        use_annotations: Optional[bool] = False,
+    ) -> Union[str, pd.DataFrame]:
         """Create a single manifest
 
         Args:
-            jsonld (str): jsonld schema 
+            path_to_data_model (str): data model schema
+            graph_data_model (nx.MultiDiGraph): graph data model
             data_type (str): data type of a manifest
-            access_token (str, optional): synapse access token. Required when getting an existing manifest. Defaults to None.
-            dataset_id (str, optional): dataset id when generating an existing manifest. Defaults to None.
-            strict (bool, optional): strictness with which to apply validation rules to google sheets. Defaults to True.
-            title (str, optional): title of a given manifest. Defaults to None.
-            output_format (str, optional): format of manifest. It has three options: google sheet, excel or dataframe. Defaults to None.
-            use_annotations (bool, optional): whether to use annotations. Defaults to False.
+            access_token (Optional[str], optional): synapse access token. Required when getting an existing manifest. Defaults to None.
+            dataset_id (Optional[str], optional):dataset id when generating an existing manifest. Defaults to None. Defaults to None.
+            strict (Optional[bool], optional): strictness with which to apply validation rules to google sheets. Defaults to True.
+            title (Optional[str], optional):title of a given manifest. Defaults to None.
+            output_format (Literal['google_sheet', 'excel', 'dataframe'], optional): format of manifest. Defaults to "google_sheet".
+            use_annotations (Optional[bool], optional):whether to use annotations. Defaults to False.
 
         Returns:
-            Union[str, pd.DataFrame, BinaryIO]: Googlesheet URL or pandas dataframe or Excel.
+            Union[str, pd.DataFrame]: Googlesheet URL or pandas dataframe or an excel file path
         """
         # create object of type ManifestGenerator
         manifest_generator = ManifestGenerator(
             path_to_data_model=path_to_data_model,
             graph=graph_data_model,
             title=title,
             root=data_type,
             use_annotations=use_annotations,
-            alphabetize_valid_values = 'ascending',
+            alphabetize_valid_values="ascending",
         )
 
         # if returning a dataframe
         if output_format:
             if "dataframe" in output_format:
                 output_format = "dataframe"
 
         result = manifest_generator.get_manifest(
-            dataset_id=dataset_id, sheet_url=True, output_format=output_format, access_token=access_token, strict=strict,
+            dataset_id=dataset_id,
+            sheet_url=True,
+            output_format=output_format,
+            access_token=access_token,
+            strict=strict,
         )
 
-        # return an excel file if output_format is set to "excel"
-        if output_format == "excel":
-            dir_name = os.path.dirname(result)
-            file_name = os.path.basename(result)
-            mimetype='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
-            return send_from_directory(directory=dir_name, path=file_name, as_attachment=True, mimetype=mimetype, max_age=0)
-               
         return result
-    
+
     @staticmethod
-    def create_manifests(path_to_data_model:str, data_types:list, access_token:Optional[str]=None, dataset_ids:Optional[list]=None, output_format:Literal["google_sheet", "excel", "dataframe"]="google_sheet", title:Optional[str]=None, strict:Optional[bool]=True, use_annotations:Optional[bool]=False) -> Union[List[str], List[pd.DataFrame], BinaryIO]:
+    def create_manifests(
+        path_to_data_model: str,
+        data_types: list,
+        data_model_labels: DisplayLabelType = "class_label",
+        access_token: Optional[str] = None,
+        dataset_ids: Optional[list] = None,
+        output_format: Literal["google_sheet", "excel", "dataframe"] = "google_sheet",
+        title: Optional[str] = None,
+        strict: Optional[bool] = True,
+        use_annotations: Optional[bool] = False,
+    ) -> Union[List[str], List[pd.DataFrame]]:
         """Create multiple manifests
 
         Args:
             path_to_data_model (str): str path to data model
-            data_type (list): a list of data types 
+            data_types (list): a list of data types
             access_token (str, optional): synapse access token. Required when getting an existing manifest. Defaults to None.
-            dataset_id (list, optional): a list of dataset ids when generating an existing manifest. Defaults to None.
+            dataset_ids (list, optional): a list of dataset ids when generating an existing manifest. Defaults to None.
             output_format (str, optional):format of manifest. It has three options: google sheet, excel or dataframe. Defaults to None.
             title (str, optional): title of a given manifest. Defaults to None.
             strict (bool, optional): strictness with which to apply validation rules to google sheets. Defaults to None.
             use_annotations (bool, optional): whether to use annotations. Defaults to False.
 
         Returns:
-            Union[List[str], List[pd.DataFrame], BinaryIO]: a list of Googlesheet URLs, a list of pandas dataframes or an Excel file.
+            Union[List[str], List[pd.DataFrame]]: a list of Googlesheet URLs, a list of pandas dataframes or excel file paths
         """
-        data_model_parser = DataModelParser(path_to_data_model = path_to_data_model)
+        if dataset_ids:
+            # Check that the number of submitted data_types matches
+            # the number of dataset_ids (if applicable)
+            len_data_types = len(data_types)
+            len_dataset_ids = len(dataset_ids)
+
+            if len_data_types != len_dataset_ids:
+                raise ValueError(
+                    f"There is a mismatch in the number of data_types and dataset_id's that "
+                    f"submitted. Please check your submission and try again."
+                )
 
-        #Parse Model
+            # Raise an error if used in conjunction with datatype = 'all_manifests'
+            if data_types[0] == "all manifests":
+                raise ValueError(
+                    "When submitting 'all manifests' as the data_type cannot also submit dataset_id. "
+                    "Please check your submission and try again."
+                )
+
+        data_model_parser = DataModelParser(path_to_data_model=path_to_data_model)
+
+        # Parse Model
         parsed_data_model = data_model_parser.parse_model()
 
         # Instantiate DataModelGraph
-        data_model_grapher = DataModelGraph(parsed_data_model)
+        data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
         # Generate graph
         graph_data_model = data_model_grapher.generate_data_model_graph()
 
         # Gather all returned result urls
         all_results = []
-        if data_types[0] == 'all manifests':
+        if data_types[0] == "all manifests":
             dmge = DataModelGraphExplorer(graph_data_model)
-            component_digraph = dmge.get_digraph_by_edge_type('requiresComponent')
+            component_digraph = dmge.get_digraph_by_edge_type("requiresComponent")
             components = component_digraph.nodes()
             for component in components:
                 if title:
-                    t = f'{title}.{component}.manifest'
-                else: 
-                    t = f'Example.{component}.manifest'
+                    t = f"{title}.{component}.manifest"
+                else:
+                    t = f"Example.{component}.manifest"
                 if output_format != "excel":
-                    result = ManifestGenerator.create_single_manifest(path_to_data_model=path_to_data_model, data_type=component, graph_data_model=graph_data_model, output_format=output_format, title=t, access_token=access_token)
+                    result = ManifestGenerator.create_single_manifest(
+                        path_to_data_model=path_to_data_model,
+                        data_type=component,
+                        graph_data_model=graph_data_model,
+                        output_format=output_format,
+                        title=t,
+                        strict=strict,
+                        access_token=access_token,
+                    )
                     all_results.append(result)
-                else: 
-                    logger.error('Currently we do not support returning multiple files as Excel format at once. Please choose a different output format. ')
+                else:
+                    logger.error(
+                        "Currently we do not support returning multiple files as Excel format at once. Please choose a different output format. "
+                    )
         else:
             for i, dt in enumerate(data_types):
-                if not title: 
-                    t = f'Example.{dt}.manifest'
-                else: 
+                if not title:
+                    t = f"Example.{dt}.manifest"
+                else:
                     if len(data_types) > 1:
-                        t = f'{title}.{dt}.manifest'
-                    else: 
+                        t = f"{title}.{dt}.manifest"
+                    else:
                         t = title
                 if dataset_ids:
                     # if a dataset_id is provided add this to the function call.
-                    result = ManifestGenerator.create_single_manifest(path_to_data_model=path_to_data_model, data_type=dt, graph_data_model=graph_data_model, dataset_id=dataset_ids[i], output_format=output_format, title=t, access_token=access_token, use_annotations=use_annotations)
+                    result = ManifestGenerator.create_single_manifest(
+                        path_to_data_model=path_to_data_model,
+                        data_type=dt,
+                        graph_data_model=graph_data_model,
+                        dataset_id=dataset_ids[i],
+                        output_format=output_format,
+                        title=t,
+                        strict=strict,
+                        access_token=access_token,
+                        use_annotations=use_annotations,
+                    )
                 else:
-                    result = ManifestGenerator.create_single_manifest(path_to_data_model=path_to_data_model, data_type=dt, graph_data_model=graph_data_model, output_format=output_format, title=t, access_token=access_token, use_annotations=use_annotations)
+                    result = ManifestGenerator.create_single_manifest(
+                        path_to_data_model=path_to_data_model,
+                        data_type=dt,
+                        graph_data_model=graph_data_model,
+                        output_format=output_format,
+                        title=t,
+                        strict=strict,
+                        access_token=access_token,
+                        use_annotations=use_annotations,
+                    )
 
                 # if output is pandas dataframe or google sheet url
                 if isinstance(result, str) or isinstance(result, pd.DataFrame):
                     all_results.append(result)
-                else: 
+                else:
                     if len(data_types) > 1:
-                        logger.warning(f'Currently we do not support returning multiple files as Excel format at once. Only {t} would get returned. ')
+                        logger.warning(
+                            f"Currently we do not support returning multiple files as Excel format at once. Only {t} would get returned. "
+                        )
                     return result
 
         return all_results
-        
 
     def get_manifest(
-        self, dataset_id: str = None, sheet_url: bool = None, json_schema: str = None, output_format: str = None, output_path: str = None, access_token: str = None, strict: Optional[bool]=None,
+        self,
+        dataset_id: str = None,
+        sheet_url: bool = None,
+        json_schema: str = None,
+        output_format: str = None,
+        output_path: str = None,
+        access_token: str = None,
+        strict: Optional[bool] = None,
     ) -> Union[str, pd.DataFrame]:
         """Gets manifest for a given dataset on Synapse.
            TODO: move this function to class MetadatModel (after MetadataModel is refactored)
 
         Args:
             dataset_id: Synapse ID of the "dataset" entity on Synapse (for a given center/project).
             sheet_url (Will be deprecated): a boolean ; determine if a pandas dataframe or a google sheet url gets return
             output_format: Determines if Google sheet URL, pandas dataframe, or Excel spreadsheet gets returned.
             output_path: Determines the output path of the exported manifest
-            access_token: Token in .synapseConfig. Since we could not pre-load access_token as an environment variable on AWS, we have to add this variable. 
+            access_token: Token in .synapseConfig. Since we could not pre-load access_token as an environment variable on AWS, we have to add this variable.
 
         Returns:
-            Googlesheet URL, pandas dataframe, or an Excel spreadsheet 
+            Googlesheet URL, pandas dataframe, or an Excel spreadsheet
         """
         # Handle case when no dataset ID is provided
         if not dataset_id:
-            manifest_url = self.get_empty_manifest(json_schema_filepath=json_schema, strict=strict, sheet_url=sheet_url)
+            manifest_url = self.get_empty_manifest(
+                json_schema_filepath=json_schema, strict=strict, sheet_url=sheet_url
+            )
 
             # if output_form parameter is set to "excel", return an excel spreadsheet
-            if output_format == "excel": 
-                output_file_path = self.export_sheet_to_excel(title = self.title, manifest_url = manifest_url, output_location = output_path)
+            if output_format == "excel":
+                output_file_path = self.export_sheet_to_excel(
+                    title=self.title,
+                    manifest_url=manifest_url,
+                    output_location=output_path,
+                )
                 return output_file_path
             # since we are not going to return an empty dataframe for an empty manifest, here we will just return a google sheet url for all other cases
-            else: 
+            else:
                 return manifest_url
 
         # Otherwise, create manifest using the given dataset
-        #TODO: avoid explicitly exposing Synapse store functionality
+        # TODO: avoid explicitly exposing Synapse store functionality
         # just instantiate a Store class and let it decide at runtime/config
         # the store type
-        if access_token: 
+        if access_token:
             # for getting an existing manifest on AWS
             store = SynapseStorage(access_token=access_token)
-        else: 
+        else:
             store = SynapseStorage()
 
         # Get manifest file associated with given dataset (if applicable)
         # populate manifest with set of new files (if applicable)
-        manifest_record = store.updateDatasetManifestFiles(self.dmge, datasetId = dataset_id, store = False)
+        manifest_record = store.updateDatasetManifestFiles(
+            self.dmge, datasetId=dataset_id, store=False
+        )
 
         # get URL of an empty manifest file created based on schema component
         empty_manifest_url = self.get_empty_manifest(strict=strict, sheet_url=True)
 
         # Populate empty template with existing manifest
         if manifest_record:
             # TODO: Update or remove the warning in self.__init__() if
             # you change the behavior here based on self.use_annotations
             # Update df with existing manifest. Agnostic to output format
-            updated_df, out_of_schema_columns = self._update_dataframe_with_existing_df(empty_manifest_url=empty_manifest_url, existing_df=manifest_record[1])
+            updated_df, out_of_schema_columns = self._update_dataframe_with_existing_df(
+                empty_manifest_url=empty_manifest_url, existing_df=manifest_record[1]
+            )
 
             # determine the format of manifest
-            result = self._handle_output_format_logic(output_format = output_format,
-                                                      output_path = output_path,
-                                                      sheet_url = sheet_url,
-                                                      empty_manifest_url=empty_manifest_url,
-                                                      dataframe = updated_df,
-                                                      out_of_schema_columns=out_of_schema_columns,
-                                                      )
+            result = self._handle_output_format_logic(
+                output_format=output_format,
+                output_path=output_path,
+                sheet_url=sheet_url,
+                empty_manifest_url=empty_manifest_url,
+                dataframe=updated_df,
+                out_of_schema_columns=out_of_schema_columns,
+            )
             return result
 
         # Generate empty template and optionally fill in with annotations
-        # if there is no existing manifest and use annotations is set to True, 
+        # if there is no existing manifest and use annotations is set to True,
         # pull annotations (in reality, annotations should be empty when there is no existing manifest)
         else:
             # Using getDatasetAnnotations() to retrieve file names and subset
             # entities to files and folders (ignoring tables/views)
             annotations = pd.DataFrame()
             if self.use_annotations:
                 if self.is_file_based:
                     annotations = store.getDatasetAnnotations(dataset_id)
                     # Update `additional_metadata` and generate manifest
-                    manifest_url, manifest_df = self.get_manifest_with_annotations(annotations,strict=strict)
-                
-                # If the annotations are empty, 
-                # ie if there are no annotations to pull or annotations were unable to be pulled because the metadata is not file based, 
+                    manifest_url, manifest_df = self.get_manifest_with_annotations(
+                        annotations, strict=strict
+                    )
+
+                # If the annotations are empty,
+                # ie if there are no annotations to pull or annotations were unable to be pulled because the metadata is not file based,
                 # then create manifest from an empty manifest
                 if annotations.empty:
                     empty_manifest_df = self.get_dataframe_by_url(empty_manifest_url)
                     manifest_df = empty_manifest_df
 
-                    logger.warning(f"Annotations were not able to be gathered for the given parameters. This manifest will be generated from an empty manifest.")
-                    
+                    logger.warning(
+                        f"Annotations were not able to be gathered for the given parameters. This manifest will be generated from an empty manifest."
+                    )
+
             else:
                 empty_manifest_df = self.get_dataframe_by_url(empty_manifest_url)
                 if self.is_file_based:
                     # for file-based manifest, make sure that entityId column and Filename column still gets filled even though use_annotations gets set to False
-                    manifest_df = store.add_entity_id_and_filename(dataset_id,empty_manifest_df)
+                    manifest_df = store.add_entity_id_and_filename(
+                        dataset_id, empty_manifest_df
+                    )
                 else:
                     manifest_df = empty_manifest_df
 
             # Update df with existing manifest. Agnostic to output format
-            updated_df, out_of_schema_columns = self._update_dataframe_with_existing_df(empty_manifest_url=empty_manifest_url, existing_df=manifest_df)
+            updated_df, out_of_schema_columns = self._update_dataframe_with_existing_df(
+                empty_manifest_url=empty_manifest_url, existing_df=manifest_df
+            )
 
-            # determine the format of manifest that gets return 
-            result = self._handle_output_format_logic(output_format = output_format,
-                                                      output_path = output_path,
-                                                      sheet_url = sheet_url,
-                                                      empty_manifest_url=empty_manifest_url,
-                                                      dataframe = updated_df,
-                                                      out_of_schema_columns = out_of_schema_columns,
-                                                      )
+            # determine the format of manifest that gets return
+            result = self._handle_output_format_logic(
+                output_format=output_format,
+                output_path=output_path,
+                sheet_url=sheet_url,
+                empty_manifest_url=empty_manifest_url,
+                dataframe=updated_df,
+                out_of_schema_columns=out_of_schema_columns,
+            )
             return result
 
-    def _get_end_columns(self, current_schema_headers, existing_manifest_headers, out_of_schema_columns):
+    def _get_end_columns(
+        self, current_schema_headers, existing_manifest_headers, out_of_schema_columns
+    ):
         """
         Gather columns to be added to the end of the manifest, and ensure entityId is at the end.
         Args:
             current_schema_headers: list, columns in the current manifest schema
             existing_manifest_headers: list, columns in the existing manifest
             out_of_schema_columns: set, columns that are in the existing manifest, but not the current schema
         Returns:
             end_columns: list of columns to be added to the end of the manifest.
         """
         # Identify columns to add to the end of the manifest
         end_columns = list(out_of_schema_columns)
-        
+
         # Make sure want Ids are placed at end of manifest, in given order.
-        for id_name in ['Uuid', 'Id', 'entityId']:
+        for id_name in ["Uuid", "Id", "entityId"]:
             if id_name in end_columns:
                 end_columns.remove(id_name)
                 end_columns.append(id_name)
-        
+
         # Add entity_id to the end columns if it should be there but isn't
-        if 'entityId' in (current_schema_headers or existing_manifest_headers) and 'entityId' not in end_columns:
-            end_columns.append('entityId')
+        if (
+            "entityId" in (current_schema_headers or existing_manifest_headers)
+            and "entityId" not in end_columns
+        ):
+            end_columns.append("entityId")
         return end_columns
 
-    def _update_dataframe_with_existing_df(self, empty_manifest_url: str, existing_df: pd.DataFrame) -> pd.DataFrame:
+    def _update_dataframe_with_existing_df(
+        self, empty_manifest_url: str, existing_df: pd.DataFrame
+    ) -> pd.DataFrame:
         """
         Handle scenario when existing manifest does not match new manifest template due to changes in the data model:
             the sheet column header reflect the latest schema the existing manifest column-set may be outdated
             ensure that, if missing, attributes from the latest schema are added to the column-set of the existing manifest so that the user can modify their data if needed
             to comply with the latest schema.
         Args:
             empty_manifest_url (str): Google Sheet URL with an empty manifest with headers.
@@ -1755,131 +1926,169 @@
 
         Returns:
             updated_df (Pd.DataFrame): existing_df with new_columns added.
             out_of_schema_columns (set): Columns that are in downloaded manifest, but not in current schema.
         """
 
         # Get headers for the current schema and existing manifest df.
-        current_schema_headers = list(self.get_dataframe_by_url(manifest_url=empty_manifest_url).columns)
+        current_schema_headers = list(
+            self.get_dataframe_by_url(manifest_url=empty_manifest_url).columns
+        )
         existing_manifest_headers = list(existing_df.columns)
 
         # Find columns that exist in the current schema, but are not in the manifest being downloaded.
-        new_columns = self._get_missing_columns(current_schema_headers, existing_manifest_headers)
+        new_columns = self._get_missing_columns(
+            current_schema_headers, existing_manifest_headers
+        )
 
         # Find columns that exist in the manifest being downloaded, but not in the current schema.
-        out_of_schema_columns = self._get_missing_columns(existing_manifest_headers, current_schema_headers)
+        out_of_schema_columns = self._get_missing_columns(
+            existing_manifest_headers, current_schema_headers
+        )
 
         # clean empty columns if any are present (there should be none)
         # TODO: Remove this line once we start preventing empty column names
-        if '' in new_columns:
-            new_columns = new_columns.remove('')
+        if "" in new_columns:
+            new_columns = new_columns.remove("")
 
         # Copy the df for updating.
         updated_df = existing_df.copy(deep=True)
-        
+
         # update existing manifest w/ missing columns, if any
         if new_columns:
             updated_df = updated_df.assign(
                 **dict(zip(new_columns, len(new_columns) * [""]))
             )
 
-        end_columns = self._get_end_columns(current_schema_headers=current_schema_headers,
-                                           existing_manifest_headers=existing_manifest_headers,
-                                           out_of_schema_columns=out_of_schema_columns)
-        
+        end_columns = self._get_end_columns(
+            current_schema_headers=current_schema_headers,
+            existing_manifest_headers=existing_manifest_headers,
+            out_of_schema_columns=out_of_schema_columns,
+        )
+
         # sort columns in the updated manifest:
         # match latest schema order
         # move obsolete columns at the end
         updated_df = updated_df[self.sort_manifest_fields(updated_df.columns)]
 
         # move obsolete columns at the end with entityId at the very end
-        updated_df = updated_df[[c for c in updated_df if c not in end_columns] + list(end_columns)]
+        updated_df = updated_df[
+            [c for c in updated_df if c not in end_columns] + list(end_columns)
+        ]
         return updated_df, out_of_schema_columns
 
     def _format_new_excel_column(self, worksheet, new_column_index: int, col: str):
         """Add new column to an openpyxl worksheet and format header.
         Args:
             worksheet: openpyxl worksheet
             new_column_index, int: index to add new column
         Return:
             modified worksheet
         """
         # Add column header
-        worksheet.cell(row=1, column=new_column_index+1).value = col
-        # Format new column header 
-        worksheet.cell(row=1, column=new_column_index+1).font = Font(size=8, bold=True, color="FF000000")
-        worksheet.cell(row=1, column=new_column_index+1).alignment = Alignment(horizontal="center", vertical="bottom")
-        worksheet.cell(row=1, column=new_column_index+1).fill = PatternFill(start_color='FFE0E0E0', end_color='FFE0E0E0', fill_type='solid')
+        worksheet.cell(row=1, column=new_column_index + 1).value = col
+        # Format new column header
+        worksheet.cell(row=1, column=new_column_index + 1).font = Font(
+            size=8, bold=True, color="FF000000"
+        )
+        worksheet.cell(row=1, column=new_column_index + 1).alignment = Alignment(
+            horizontal="center", vertical="bottom"
+        )
+        worksheet.cell(row=1, column=new_column_index + 1).fill = PatternFill(
+            start_color="FFE0E0E0", end_color="FFE0E0E0", fill_type="solid"
+        )
         return worksheet
 
-    def populate_existing_excel_spreadsheet(self, existing_excel_path: str = None, additional_df: pd.DataFrame = None):
-        '''Populate an existing excel spreadsheet by using an additional dataframe (to avoid sending metadata directly to Google APIs)
+    def populate_existing_excel_spreadsheet(
+        self, existing_excel_path: str = None, additional_df: pd.DataFrame = None
+    ):
+        """Populate an existing excel spreadsheet by using an additional dataframe (to avoid sending metadata directly to Google APIs)
         New columns will be placed at the end of the spreadsheet.
         Args:
             existing_excel_path: path of an existing excel spreadsheet
             additional_df: additional dataframe
-        Return: 
+        Return:
             added new dataframe to the existing excel path.
         Note:
-            - Done by rows and column as a way to preserve formatting. 
+            - Done by rows and column as a way to preserve formatting.
             Doing a complete replacement will remove all conditional formatting and dropdowns.
-        '''
+        """
         # load workbook
         workbook = load_workbook(existing_excel_path)
         worksheet = workbook.active
 
         # Add new data to existing excel
         if not additional_df.empty:
-            existing_excel_headers = [cell.value for cell in worksheet[1] if cell.value != None]
+            existing_excel_headers = [
+                cell.value for cell in worksheet[1] if cell.value != None
+            ]
 
             new_column_index = len(existing_excel_headers)
             df_columns = additional_df.columns
 
             # Iteratively fill workbook with contents of additional_df
-            for row_num, row_contents in enumerate(dataframe_to_rows(additional_df, index=False, header=False), 2):
+            for row_num, row_contents in enumerate(
+                dataframe_to_rows(additional_df, index=False, header=False), 2
+            ):
                 for index, col in enumerate(df_columns):
                     if col in existing_excel_headers:
                         # Get index of column header in existing excel to ensure no values are placed in incorrect spot.
                         existing_column_index = existing_excel_headers.index(col)
-                        worksheet.cell(row=row_num, column=existing_column_index+1).value = row_contents[index]
+                        worksheet.cell(
+                            row=row_num, column=existing_column_index + 1
+                        ).value = row_contents[index]
                     else:
                         # Add new col to excel worksheet and format.
-                        worksheet = self._format_new_excel_column(worksheet=worksheet, new_column_index=new_column_index, col=col)
+                        worksheet = self._format_new_excel_column(
+                            worksheet=worksheet,
+                            new_column_index=new_column_index,
+                            col=col,
+                        )
                         # Add data to column
-                        worksheet.cell(row=row_num, column=new_column_index+1).value = row_contents[index]
+                        worksheet.cell(
+                            row=row_num, column=new_column_index + 1
+                        ).value = row_contents[index]
                         # Add new column to headers so it can be accounted for.
                         existing_excel_headers.append(col)
                         # Update index for adding new columns.
-                        new_column_index+=1                   
+                        new_column_index += 1
         workbook.save(existing_excel_path)
 
-    def populate_manifest_spreadsheet(self, existing_manifest_path: str = None, empty_manifest_url: str = None, return_excel: bool = False, title: str = None):
+    def populate_manifest_spreadsheet(
+        self,
+        existing_manifest_path: str = None,
+        empty_manifest_url: str = None,
+        return_excel: bool = False,
+        title: str = None,
+    ):
         """Creates a google sheet manifest based on existing manifest.
         Args:
             existing_manifest_path: the location of the manifest containing metadata presently stored
             empty_manifest_url: the path to a manifest template to be prepopulated with existing's manifest metadata
             return_excel: if true, return an Excel spreadsheet instead of Google sheet
-            title: title of output manifest 
+            title: title of output manifest
         """
 
         # read existing manifest
         manifest = load_df(existing_manifest_path)
-        
-        if return_excel: 
-            '''if we are returning an Excel spreadsheet, do not populate dataframe to google'''
-            # get an empty manifest 
+
+        if return_excel:
+            """if we are returning an Excel spreadsheet, do not populate dataframe to google"""
+            # get an empty manifest
             manifest_url = empty_manifest_url
 
             # export the manifest to excel
-            output_excel_file_path = self.export_sheet_to_excel(manifest_url = manifest_url, title=title)
-            
-            # populate exported sheet 
+            output_excel_file_path = self.export_sheet_to_excel(
+                manifest_url=manifest_url, title=title
+            )
+
+            # populate exported sheet
             self.populate_existing_excel_spreadsheet(output_excel_file_path, manifest)
             return output_excel_file_path
-        else: 
+        else:
             manifest_sh = self.set_dataframe_by_url(empty_manifest_url, manifest)
             return manifest_sh.url
 
     def sort_manifest_fields(self, manifest_fields, order="schema"):
         # order manifest fields alphabetically (base order)
         manifest_fields = sorted(manifest_fields)
```

### Comparing `schematicpy-24.1.1/schematic/models/GE_Helpers.py` & `schematicpy-24.2.1/schematic/models/GE_Helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from statistics import mode
 from tabnanny import check
 import logging
 import os
 import re
 import numpy as np
 
@@ -15,68 +14,77 @@
 from attr import attr
 
 from ruamel import yaml
 
 import great_expectations as ge
 from great_expectations.core.expectation_configuration import ExpectationConfiguration
 from great_expectations.data_context import BaseDataContext
-from great_expectations.data_context.types.base import DataContextConfig, DatasourceConfig, FilesystemStoreBackendDefaults
-from great_expectations.data_context.types.resource_identifiers import ExpectationSuiteIdentifier
+from great_expectations.data_context.types.base import (
+    DataContextConfig,
+    DatasourceConfig,
+    FilesystemStoreBackendDefaults,
+)
+from great_expectations.data_context.types.resource_identifiers import (
+    ExpectationSuiteIdentifier,
+)
 from great_expectations.exceptions.exceptions import GreatExpectationsError
 
 
 from schematic.models.validate_attribute import GenerateError
 from schematic.schemas.data_model_graph import DataModelGraphExplorer
 
-from schematic.utils.validate_utils import rule_in_rule_list, np_array_to_str_list, iterable_to_str_list
+from schematic.utils.schema_utils import extract_component_validation_rules
+
+from schematic.utils.validate_utils import (
+    rule_in_rule_list,
+    np_array_to_str_list,
+    iterable_to_str_list,
+)
 
 logger = logging.getLogger(__name__)
 
+
 class GreatExpectationsHelpers(object):
     """
-        Great Expectations helper class
+    Great Expectations helper class
 
-        Provides basic utilities to:
-            1) Create GE workflow specific to manifest according to validation rules
-            2) Parse results dict to generate appropriate errors
+    Provides basic utilities to:
+        1) Create GE workflow specific to manifest according to validation rules
+        2) Parse results dict to generate appropriate errors
     """
-    def __init__(self,
-        dmge,
-        unimplemented_expectations,
-        manifest,
-        manifestPath
-        ):
-        """
-            Purpose:
-                Instantiate a great expectations helpers object
-            Args:
-                dmge: 
-                    DataModelGraphExplorer Object
-                unimplemented_expectations:
-                    dictionary of validation rules that currently do not have expectations developed
-                manifest:
-                    manifest being validated
-                manifestPath:
-                    path to manifest being validated            
+
+    def __init__(self, dmge, unimplemented_expectations, manifest, manifestPath):
+        """
+        Purpose:
+            Instantiate a great expectations helpers object
+        Args:
+            dmge:
+                DataModelGraphExplorer Object
+            unimplemented_expectations:
+                dictionary of validation rules that currently do not have expectations developed
+            manifest:
+                manifest being validated
+            manifestPath:
+                path to manifest being validated
         """
         self.unimplemented_expectations = unimplemented_expectations
         self.dmge = dmge
         self.manifest = manifest
         self.manifestPath = manifestPath
 
-    def  build_context(self):
+    def build_context(self):
         """
-            Purpose:
-                Create a dataContext and datasource and add to object 
-            Returns:
-                saves dataContext and datasource to self
+        Purpose:
+            Create a dataContext and datasource and add to object
+        Returns:
+            saves dataContext and datasource to self
         """
-        self.context=ge.get_context()
+        self.context = ge.get_context()
 
-        #create datasource configuration
+        # create datasource configuration
         datasource_config = {
             "name": "example_datasource",
             "class_name": "Datasource",
             "module_name": "great_expectations.datasource",
             "execution_engine": {
                 "module_name": "great_expectations.execution_engine",
                 "class_name": "PandasExecutionEngine",
@@ -85,285 +93,304 @@
                 "default_runtime_data_connector_name": {
                     "class_name": "RuntimeDataConnector",
                     "batch_identifiers": ["default_identifier_name"],
                 },
             },
         }
 
-        #create data context configuration
+        # create data context configuration
         data_context_config = DataContextConfig(
             datasources={
                 "pandas": DatasourceConfig(
                     class_name="Datasource",
-                    execution_engine={
-                        "class_name": "PandasExecutionEngine"
-                    },
+                    execution_engine={"class_name": "PandasExecutionEngine"},
                     data_connectors={
                         "default_runtime_data_connector_name": {
                             "class_name": "RuntimeDataConnector",
                             "batch_identifiers": ["default_identifier_name"],
                         }
                     },
                 )
             },
-            store_backend_defaults=FilesystemStoreBackendDefaults(root_directory=os.path.join(os.getcwd(),'great_expectations')),
+            store_backend_defaults=FilesystemStoreBackendDefaults(
+                root_directory=os.path.join(os.getcwd(), "great_expectations")
+            ),
         )
 
-        #build context and add data source
-        self.context=BaseDataContext(project_config=data_context_config)
-        #self.context.test_yaml_config(yaml.dump(datasource_config))
+        # build context and add data source
+        self.context = BaseDataContext(project_config=data_context_config)
+        # self.context.test_yaml_config(yaml.dump(datasource_config))
         self.context.add_datasource(**datasource_config)
 
-        
-    def build_expectation_suite(self,):
+    def build_expectation_suite(
+        self,
+    ):
         """
-            Purpose:
-                Construct an expectation suite to validate columns with rules that have expectations
-                Add suite to object
-            Input:
-                
-            Returns:
-                saves expectation suite and identifier to self
-            
+        Purpose:
+            Construct an expectation suite to validate columns with rules that have expectations
+            Add suite to object
+        Input:
+
+        Returns:
+            saves expectation suite and identifier to self
+
         """
         validation_expectation = {
             "int": "expect_column_values_to_be_in_type_list",
             "float": "expect_column_values_to_be_in_type_list",
             "str": "expect_column_values_to_be_of_type",
             "num": "expect_column_values_to_be_in_type_list",
             "date": "expect_column_values_to_be_dateutil_parseable",
             "recommended": "expect_column_values_to_not_match_regex_list",
             "protectAges": "expect_column_values_to_be_between",
             "unique": "expect_column_values_to_be_unique",
             "inRange": "expect_column_values_to_be_between",
             "IsNA": "expect_column_values_to_match_regex_list",
-
             # To be implemented rules with possible expectations
-            #"list": "expect_column_values_to_not_match_regex_list",
-            #"regex": "expect_column_values_to_match_regex",
-            #"url": "expect_column_values_to_be_valid_urls",
-            #"matchAtLeastOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
-            #"matchExactlyOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
+            # "list": "expect_column_values_to_not_match_regex_list",
+            # "regex": "expect_column_values_to_match_regex",
+            # "url": "expect_column_values_to_be_valid_urls",
+            # "matchAtLeastOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
+            # "matchExactlyOne": "expect_foreign_keys_in_column_a_to_exist_in_column_b",
         }
-        
-        #create blank expectation suite
-        self.expectation_suite_name = "Manifest_test_suite"       
+
+        # create blank expectation suite
+        self.expectation_suite_name = "Manifest_test_suite"
         self.suite = self.context.add_expectation_suite(
             expectation_suite_name=self.expectation_suite_name,
-        )    
+        )
 
-        #build expectation configurations for each expectation
+        # build expectation configurations for each expectation
         for col in self.manifest.columns:
-            args={}
-            meta={}
-            
+            args = {}
+            meta = {}
+
             # remove trailing/leading whitespaces from manifest
-            self.manifest.applymap(lambda x: x.strip() if isinstance(x, str) else x)
-            validation_rules = self.dmge.get_node_validation_rules(node_display_name=col)
+            self.manifest.map(lambda x: x.strip() if isinstance(x, str) else x)
 
-            #check if attribute has any rules associated with it
+            validation_rules = self.dmge.get_node_validation_rules(
+                node_display_name=col
+            )
+
+            # check if attribute has any rules associated with it
             if validation_rules:
-                #iterate through all validation rules for an attribute
+                # Check if the validation rule applies to this manifest
+                if isinstance(validation_rules, dict):
+                    validation_rules = extract_component_validation_rules(
+                        manifest_component=self.manifest["Component"][0],
+                        validation_rules=validation_rules,
+                    )
+                # iterate through all validation rules for an attribute
                 for rule in validation_rules:
                     base_rule = rule.split(" ")[0]
-            
-                    #check if rule has an implemented expectation
-                    if rule_in_rule_list(rule,self.unimplemented_expectations):
+
+                    # check if rule has an implemented expectation
+                    if rule_in_rule_list(rule, self.unimplemented_expectations):
                         continue
 
-                
                     args["column"] = col
                     args["result_format"] = "COMPLETE"
 
-
-                    #Validate num
-                    if base_rule=='num':
-                        args["mostly"]=1.0
-                        args["type_list"]=['int','int64', 'float', 'float64']
-                        meta={
+                    # Validate num
+                    if base_rule == "num":
+                        args["mostly"] = 1.0
+                        args["type_list"] = ["int", "int64", "float", "float64"]
+                        meta = {
                             "notes": {
                                 "format": "markdown",
-                                "content": "Expect column values to be of int or float type. **Markdown** `Supported`"
+                                "content": "Expect column values to be of int or float type. **Markdown** `Supported`",
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
-                
-                    #Validate float
-                    elif base_rule=='float':
-                        args["mostly"]=1.0
-                        args["type_list"]=['float', 'float64']
-                        meta={
+
+                    # Validate float
+                    elif base_rule == "float":
+                        args["mostly"] = 1.0
+                        args["type_list"] = ["float", "float64"]
+                        meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column values to be of float type. **Markdown** `Supported`",
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
-                
-                    #Validate int
-                    elif base_rule=='int':
-                        args["mostly"]=1.0
-                        args["type_list"]=['int','int64']
-                        meta={
+
+                    # Validate int
+                    elif base_rule == "int":
+                        args["mostly"] = 1.0
+                        args["type_list"] = ["int", "int64"]
+                        meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column values to be of int type. **Markdown** `Supported`",
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
-                
-                    #Validate string
-                    elif base_rule=='str':
-                        args["mostly"]=1.0
-                        args["type_"]='str'
-                        meta={
+
+                    # Validate string
+                    elif base_rule == "str":
+                        args["mostly"] = 1.0
+                        args["type_"] = "str"
+                        meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column values to be of string type. **Markdown** `Supported`",
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
 
-                    #Validate date
-                    elif base_rule=='date':
-                        args["mostly"]=1.0
-                        meta={
+                    # Validate date
+                    elif base_rule == "date":
+                        args["mostly"] = 1.0
+                        meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": (
                                     "Expect column values to be parsable by dateutils. "
                                     "**Markdown** `Supported`"
                                 ),
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
 
-                    elif base_rule==("recommended"):
-                        args["mostly"]=0.0000000001
-                        args["regex_list"]=['^$']
-                        meta={
+                    elif base_rule == ("recommended"):
+                        args["mostly"] = 0.0000000001
+                        args["regex_list"] = ["^$"]
+                        meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column to not be empty. **Markdown** `Supported`",
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
 
-                    elif base_rule==("protectAges"):
-                        #Function to convert to different age limit formats
+                    elif base_rule == ("protectAges"):
+                        # Function to convert to different age limit formats
                         min_age, max_age = self.get_age_limits()
 
-                        args["mostly"]=1.0
-                        args["min_value"]=min_age
-                        args["max_value"]=max_age
-                        #args['allow_cross_type_comparisons']=True # TODO Can allow after issue #980 is completed
-                        meta={
+                        args["mostly"] = 1.0
+                        args["min_value"] = min_age
+                        args["max_value"] = max_age
+                        # args['allow_cross_type_comparisons']=True # TODO Can allow after issue #980 is completed
+                        meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect ages to be between 18 years (6,570 days) and 90 years (32,850 days) of age. **Markdown** `Supported`",
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
 
-                    elif base_rule==("unique"):
-                        args["mostly"]=1.0
-                        meta={
+                    elif base_rule == ("unique"):
+                        args["mostly"] = 1.0
+                        meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column values to be Unique. **Markdown** `Supported`",
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
-                    
-                    elif base_rule==("inRange"):
-                        args["mostly"]=1.0
-                        args["min_value"]=float(rule.split(" ")[1]) if rule.split(" ")[1].lower() != 'none' else None
-                        args["max_value"]=float(rule.split(" ")[2]) if rule.split(" ")[2].lower() != 'none' else None
-                        args['allow_cross_type_comparisons']=True # TODO Should follow up with issue #980
-                        meta={
+
+                    elif base_rule == ("inRange"):
+                        args["mostly"] = 1.0
+                        args["min_value"] = (
+                            float(rule.split(" ")[1])
+                            if rule.split(" ")[1].lower() != "none"
+                            else None
+                        )
+                        args["max_value"] = (
+                            float(rule.split(" ")[2])
+                            if rule.split(" ")[2].lower() != "none"
+                            else None
+                        )
+                        args[
+                            "allow_cross_type_comparisons"
+                        ] = True  # TODO Should follow up with issue #980
+                        meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column values to be within a specified range. **Markdown** `Supported`",
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
-                        
-                    elif base_rule==("IsNA"):
-                        args["mostly"]=1.0
-                        args["regex_list"]=['Not Applicable']
-                        meta={
+
+                    elif base_rule == ("IsNA"):
+                        args["mostly"] = 1.0
+                        args["regex_list"] = ["Not Applicable"]
+                        meta = {
                             "notes": {
                                 "format": "markdown",
                                 "content": "Expect column values to be marked Not Applicable. **Markdown** `Supported`",
                             },
-                            "validation_rule": rule
+                            "validation_rule": rule,
                         }
-                                        
-                    #add expectation for attribute to suite        
+
+                    # add expectation for attribute to suite
                     self.add_expectation(
                         rule=rule,
                         args=args,
                         meta=meta,
                         validation_expectation=validation_expectation,
                     )
-        
-            
-        self.context.update_expectation_suite(expectation_suite=self.suite,)
 
-        suite_identifier = ExpectationSuiteIdentifier(expectation_suite_name=self.expectation_suite_name)
+        self.context.update_expectation_suite(
+            expectation_suite=self.suite,
+        )
+
+        suite_identifier = ExpectationSuiteIdentifier(
+            expectation_suite_name=self.expectation_suite_name
+        )
         self.context.build_data_docs(resource_identifiers=[suite_identifier])
         ##Webpage DataDocs opened here:
-        #self.context.open_data_docs(resource_identifier=suite_identifier) 
+        # self.context.open_data_docs(resource_identifier=suite_identifier)
 
     def add_expectation(
         self,
         rule: str,
         args: Dict,
         meta: Dict,
         validation_expectation: Dict,
-        ):
+    ):
         """
-            Purpose:
-                Add individual expectation for a rule to the suite
-            Input:
-                rule: 
-                    validation rule
-                args: 
-                    dict of arguments specifying expectation behavior
-                meta:
-                    dict of additional information for each expectation
-                validation_expectation:
-                    dictionary to map between rules and expectations
-            Returns:
-                adds expectation to self.suite
-            
+        Purpose:
+            Add individual expectation for a rule to the suite
+        Input:
+            rule:
+                validation rule
+            args:
+                dict of arguments specifying expectation behavior
+            meta:
+                dict of additional information for each expectation
+            validation_expectation:
+                dictionary to map between rules and expectations
+        Returns:
+            adds expectation to self.suite
+
         """
         # Create an Expectation
         expectation_configuration = ExpectationConfiguration(
             # Name of expectation type being added
             expectation_type=validation_expectation[rule.split(" ")[0]],
-
-            #add arguments and meta message
+            # add arguments and meta message
             kwargs={**args},
-            meta={**meta}
+            meta={**meta},
         )
         # Add the Expectation to the suite
         self.suite.add_expectation(expectation_configuration=expectation_configuration)
 
     def build_checkpoint(self):
         """
-            Purpose:
-                Build checkpoint to validate manifest
-            Input:
-            Returns:
-                adds checkpoint to self 
-        """
-        #create manifest checkpoint
-        self.checkpoint_name = "manifest_checkpoint"  
-        checkpoint_config={
+        Purpose:
+            Build checkpoint to validate manifest
+        Input:
+        Returns:
+            adds checkpoint to self
+        """
+        # create manifest checkpoint
+        self.checkpoint_name = "manifest_checkpoint"
+        checkpoint_config = {
             "name": self.checkpoint_name,
             "config_version": 1,
             "class_name": "SimpleCheckpoint",
             "validations": [
                 {
                     "batch_request": {
                         "datasource_name": "example_datasource",
@@ -371,173 +398,182 @@
                         "data_asset_name": "Manifest",
                     },
                     "expectation_suite_name": self.expectation_suite_name,
                 }
             ],
         }
 
-        #self.context.test_yaml_config(yaml.dump(checkpoint_config),return_mode="report_object")        
+        # self.context.test_yaml_config(yaml.dump(checkpoint_config),return_mode="report_object")
         self.context.add_checkpoint(**checkpoint_config)
-    
+
     def generate_errors(
         self,
         validation_results: Dict,
         validation_types: Dict,
         errors: List,
         warnings: List,
         dmge: DataModelGraphExplorer,
-        ):
+    ):
         """
-            Purpose:
-                Parse results dictionary and generate errors for expectations
-            Input:
-                validation_results:
-                    dictionary of results for each expectation
-                validation_types:
-                    dict of types of errors to generate for each validation rule
-                errors:
-                    list of errors
-                warnings:
-                    list of warnings    
-            Returns:
-                errors:
-                    list of errors
-                warnings:
-                    list of warnings
-                self.manifest:
-                    manifest, possibly updated (censored ages)
+        Purpose:
+            Parse results dictionary and generate errors for expectations
+        Input:
+            validation_results:
+                dictionary of results for each expectation
+            validation_types:
+                dict of types of errors to generate for each validation rule
+            errors:
+                list of errors
+            warnings:
+                list of warnings
+        Returns:
+            errors:
+                list of errors
+            warnings:
+                list of warnings
+            self.manifest:
+                manifest, possibly updated (censored ages)
         """
 
-        type_dict={
+        type_dict = {
             "float64": float,
             "int64": int,
             "str": str,
         }
-        for result_dict in validation_results[0]['results']:
-
-            
+        for result_dict in validation_results[0]["results"]:
             indices = []
             values = []
-            
-            #if the expectaion failed, get infromation to generate error message
-            if not result_dict['success']:
-                errColumn   = result_dict['expectation_config']['kwargs']['column']               
-                rule        = result_dict['expectation_config']['meta']['validation_rule']
 
+            # if the expectaion failed, get infromation to generate error message
+            if not result_dict["success"]:
+                errColumn = result_dict["expectation_config"]["kwargs"]["column"]
+                rule = result_dict["expectation_config"]["meta"]["validation_rule"]
+
+                if (
+                    "exception_info" in result_dict.keys()
+                    and result_dict["exception_info"]["exception_message"]
+                ):
+                    raise GreatExpectationsError(
+                        result_dict["exception_info"]["exception_traceback"]
+                    )
 
-                if 'exception_info' in result_dict.keys() and result_dict['exception_info']['exception_message']:
-                    raise GreatExpectationsError(result_dict['exception_info']['exception_traceback'])
-                
-                #only some expectations explicitly list unexpected values and indices, read or find if not present
-                elif 'unexpected_index_list' in result_dict['result']:
-                    indices = result_dict['result']['unexpected_index_list']
-                    values  = result_dict['result']['unexpected_list']
+                # only some expectations explicitly list unexpected values and indices, read or find if not present
+                elif "unexpected_index_list" in result_dict["result"]:
+                    indices = result_dict["result"]["unexpected_index_list"]
+                    values = result_dict["result"]["unexpected_list"]
 
                 # Technically, this shouldn't ever happen, but will keep as a failsafe in case many things go wrong
-                # because type validation is column aggregate expectation and not column map expectation when columns are not of object type, 
+                # because type validation is column aggregate expectation and not column map expectation when columns are not of object type,
                 # indices and values cannot be returned
                 else:
                     for i, item in enumerate(self.manifest[errColumn]):
-                        observed_type=result_dict['result']['observed_value']
-                        indices.append(i)   if isinstance(item,type_dict[observed_type]) else indices
-                        values.append(item) if isinstance(item,type_dict[observed_type]) else values
-
-                #call functions to generate error messages and add to error list
-                if validation_types[rule.split(" ")[0]]['type']=='type_validation':
-                    for row, value in zip(indices,values):
+                        observed_type = result_dict["result"]["observed_value"]
+                        indices.append(i) if isinstance(
+                            item, type_dict[observed_type]
+                        ) else indices
+                        values.append(item) if isinstance(
+                            item, type_dict[observed_type]
+                        ) else values
+
+                # call functions to generate error messages and add to error list
+                if validation_types[rule.split(" ")[0]]["type"] == "type_validation":
+                    for row, value in zip(indices, values):
                         vr_errors, vr_warnings = GenerateError.generate_type_error(
-                                val_rule = rule,
-                                row_num = str(row+2),
-                                attribute_name = errColumn,
-                                invalid_entry = str(value),
-                                dmge = dmge,
-                            )
+                            val_rule=rule,
+                            row_num=str(row + 2),
+                            attribute_name=errColumn,
+                            invalid_entry=str(value),
+                            dmge=dmge,
+                        )
                         if vr_errors:
-                            errors.append(vr_errors)  
+                            errors.append(vr_errors)
                         if vr_warnings:
-                            warnings.append(vr_warnings) 
-                elif validation_types[rule.split(" ")[0]]['type']=='regex_validation':
-                    expression=result_dict['expectation_config']['kwargs']['regex']
-                    for row, value in zip(indices,values):   
+                            warnings.append(vr_warnings)
+                elif validation_types[rule.split(" ")[0]]["type"] == "regex_validation":
+                    expression = result_dict["expectation_config"]["kwargs"]["regex"]
+                    for row, value in zip(indices, values):
                         vr_errors, vr_warnings = GenerateError.generate_regex_error(
-                                val_rule= rule,
-                                reg_expression = expression,
-                                row_num = str(row+2),
-                                module_to_call = 'match',
-                                attribute_name = errColumn,
-                                invalid_entry = value,
-                                dmge = dmge,
-                            )
+                            val_rule=rule,
+                            reg_expression=expression,
+                            row_num=str(row + 2),
+                            module_to_call="match",
+                            attribute_name=errColumn,
+                            invalid_entry=value,
+                            dmge=dmge,
+                        )
                         if vr_errors:
-                            errors.append(vr_errors)  
+                            errors.append(vr_errors)
                         if vr_warnings:
-                            warnings.append(vr_warnings)                          
-                elif validation_types[rule.split(" ")[0]]['type']=='content_validation':     
+                            warnings.append(vr_warnings)
+                elif (
+                    validation_types[rule.split(" ")[0]]["type"] == "content_validation"
+                ):
                     vr_errors, vr_warnings = GenerateError.generate_content_error(
-                                                            val_rule = rule, 
-                                                            attribute_name = errColumn,
-                                                            row_num = np_array_to_str_list(np.array(indices)+2),
-                                                            error_val = iterable_to_str_list(values),  
-                                                            dmge = self.dmge
-                                                        )       
+                        val_rule=rule,
+                        attribute_name=errColumn,
+                        row_num=np_array_to_str_list(np.array(indices) + 2),
+                        error_val=iterable_to_str_list(values),
+                        dmge=self.dmge,
+                    )
                     if vr_errors:
-                        errors.append(vr_errors)  
-                        if rule.startswith('protectAges'):
-                            self.censor_ages(vr_errors,errColumn)
-                            
+                        errors.append(vr_errors)
+                        if rule.startswith("protectAges"):
+                            self.censor_ages(vr_errors, errColumn)
+
                     if vr_warnings:
-                        warnings.append(vr_warnings)  
-                        if rule.startswith('protectAges'):
-                            self.censor_ages(vr_warnings,errColumn)
-                            
+                        warnings.append(vr_warnings)
+                        if rule.startswith("protectAges"):
+                            self.censor_ages(vr_warnings, errColumn)
 
         return errors, warnings
 
     def get_age_limits(
         self,
-        ):
+    ):
         """
-            Purpose:
-                Get boundaries of ages that need to be censored for different age formats
-            Input:
-            Returns:
-                min_age:
-                    minimum age that will not be censored
-                max age:
-                    maximum age that will not be censored
-            
-        """        
+        Purpose:
+            Get boundaries of ages that need to be censored for different age formats
+        Input:
+        Returns:
+            min_age:
+                minimum age that will not be censored
+            max age:
+                maximum age that will not be censored
 
-        min_age = 6550      #days
-        max_age = 32849     #days
+        """
+
+        min_age = 6550  # days
+        max_age = 32849  # days
 
         return min_age, max_age
 
     def censor_ages(
         self,
         message: List,
         col: str,
-        ):
+    ):
         """
-            Purpose:
-                Censor ages in manifest as appropriate
-            Input:
-                message: 
-                    error or warning message for age validation rule
-                col:
-                    name of column containing ages
-            Returns:
-                updates self.manifest with censored ages
-            TODO: Speed up conversion from str list to int list
+        Purpose:
+            Censor ages in manifest as appropriate
+        Input:
+            message:
+                error or warning message for age validation rule
+            col:
+                name of column containing ages
+        Returns:
+            updates self.manifest with censored ages
+        TODO: Speed up conversion from str list to int list
         """
         censor_rows = []
-        
+
         for row in message[0]:
             censor_rows.append(int(row) - 2)
 
-        self.manifest.loc[censor_rows,(col)] = 'age censored'
+        self.manifest.loc[censor_rows, (col)] = "age censored"
 
         # update the manifest file, so that ages are censored
-        self.manifest.to_csv(self.manifestPath.replace('.csv','_censored.csv'), index=False)
+        self.manifest.to_csv(
+            self.manifestPath.replace(".csv", "_censored.csv"), index=False
+        )
         logging.info("Sensitive ages have been censored.")
 
         return
```

### Comparing `schematicpy-24.1.1/schematic/models/metadata.py` & `schematicpy-24.2.1/schematic/models/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import logging
 import networkx as nx
+from os.path import exists
 from jsonschema import ValidationError
 
 # allows specifying explicit variable types
 from typing import Any, Dict, Optional, Text, List
 
 from schematic.manifest.generator import ManifestGenerator
 from schematic.schemas.data_model_graph import DataModelGraph, DataModelGraphExplorer
 from schematic.schemas.data_model_parser import DataModelParser
 from schematic.schemas.data_model_json_schema import DataModelJSONSchema
 
-
-#TODO: This module should only be aware of the store interface
+# TODO: This module should only be aware of the store interface
 # we shouldn't need to expose Synapse functionality explicitly
 from schematic.store.synapse import SynapseStorage
 
 from schematic.utils.df_utils import load_df
 
 from schematic.models.validate_manifest import validate_all
 
@@ -30,16 +30,20 @@
 
     1) manipulate the metadata model
     2) generate metadata model views:
         - generate manifest view of the metadata model
         - generate validation schema view of the metadata model
     """
 
-    def __init__(self, inputMModelLocation: str, inputMModelLocationType: str,) -> None:
-
+    def __init__(
+        self,
+        inputMModelLocation: str,
+        inputMModelLocationType: str,
+        data_model_labels: str,
+    ) -> None:
         """Instantiates a MetadataModel object.
 
         Args:
             inputMModelLocation: local path, uri, synapse entity id (e.g. gs://, syn123, /User/x/…); present location
             inputMModelLocationType: specifier to indicate where the metadata model resource can be found (e.g. 'local' if file/JSON-LD is on local machine)
         """
         # extract extension of 'inputMModelLocation'
@@ -47,20 +51,20 @@
 
         logger.debug(
             f"Initializing DataModelGraphExplorer object from {inputMModelLocation} schema."
         )
 
         self.inputMModelLocation = inputMModelLocation
 
-        data_model_parser = DataModelParser(path_to_data_model = self.inputMModelLocation)
-        #Parse Model
+        data_model_parser = DataModelParser(path_to_data_model=self.inputMModelLocation)
+        # Parse Model
         parsed_data_model = data_model_parser.parse_model()
 
         # Instantiate DataModelGraph
-        data_model_grapher = DataModelGraph(parsed_data_model)
+        data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
         # Generate graph
         self.graph_data_model = data_model_grapher.generate_data_model_graph()
 
         self.dmge = DataModelGraphExplorer(self.graph_data_model)
 
         # check if the type of MModel file is "local"
@@ -134,15 +138,15 @@
         """
         additionalMetadata = {}
         if filenames:
             additionalMetadata["Filename"] = filenames
 
         mg = ManifestGenerator(
             path_to_json_ld=self.inputMModelLocation,
-            graph = self.graph_data_model,
+            graph=self.graph_data_model,
             title=title,
             root=rootNode,
             additional_metadata=additionalMetadata,
             use_annotations=useAnnotations,
         )
 
         if datasetId:
@@ -204,33 +208,36 @@
             A validation status message; if there is an error the message.
             contains the manifest annotation record (i.e. row) that is invalid, along with the validation error associated with this record.
 
         Raises:
             ValueError: rootNode not found in metadata model.
         """
         # get validation schema for a given node in the data model, if the user has not provided input validation schema
-        
+
         if not jsonSchema:
-            
             # Instantiate Data Model Json Schema
-            self.data_model_js = DataModelJSONSchema(jsonld_path=self.inputMModelLocation, graph=self.graph_data_model)
-            
+            self.data_model_js = DataModelJSONSchema(
+                jsonld_path=self.inputMModelLocation, graph=self.graph_data_model
+            )
+
             jsonSchema = self.data_model_js.get_json_validation_schema(
                 rootNode, rootNode + "_validation"
             )
 
         errors = []
         warnings = []
 
-        load_args={
-            "dtype":"string",
-            }
+        load_args = {
+            "dtype": "string",
+        }
         # get annotations from manifest (array of json annotations corresponding to manifest rows)
         manifest = load_df(
-            manifestPath, preserve_raw_input=False, **load_args,
+            manifestPath,
+            preserve_raw_input=False,
+            **load_args,
         )  # read manifest csv file as is from manifest path
 
         # handler for mismatched components/data types
         # throw TypeError if the value(s) in the "Component" column differ from the selected template type
         if ("Component" in manifest.columns) and (
             (len(manifest["Component"].unique()) > 1)
             or (manifest["Component"].unique()[0] != rootNode)
@@ -255,165 +262,184 @@
                         # tuple of the component in the manifest and selected template type
                         # check: R/Reticulate cannnot handle dicts? So returning tuple
                         (component, rootNode),
                     ]
                 )
 
             return errors, warnings
-        
+
         # check if suite has been created. If so, delete it
         if os.path.exists("great_expectations/expectations/Manifest_test_suite.json"):
             os.remove("great_expectations/expectations/Manifest_test_suite.json")
-            
-        errors, warnings, manifest = validate_all(self, 
-                                                  errors=errors,
-                                                  warnings=warnings,
-                                                  manifest=manifest,
-                                                  manifestPath=manifestPath,
-                                                  dmge=self.dmge,
-                                                  jsonSchema=jsonSchema,
-                                                  restrict_rules=restrict_rules,
-                                                  project_scope=project_scope,
-                                                  access_token=access_token)
+
+        errors, warnings, manifest = validate_all(
+            self,
+            errors=errors,
+            warnings=warnings,
+            manifest=manifest,
+            manifestPath=manifestPath,
+            dmge=self.dmge,
+            jsonSchema=jsonSchema,
+            restrict_rules=restrict_rules,
+            project_scope=project_scope,
+            access_token=access_token,
+        )
         return errors, warnings
 
-    def populateModelManifest(self, title, manifestPath: str, rootNode: str, return_excel = False) -> str:
+    def populateModelManifest(
+        self, title, manifestPath: str, rootNode: str, return_excel=False
+    ) -> str:
         """Populate an existing annotations manifest based on a dataframe.
             TODO: Remove this method; always use getModelManifest instead
 
         Args:
             rootNode: a schema node label (i.e. term).
             manifestPath: a path to the manifest csv file containing annotations.
 
         Returns:
             A link to the filled in model manifest (e.g. google sheet).
 
         Raises:
             ValueError: rootNode not found in metadata model.
         """
         mg = ManifestGenerator(
-            path_to_data_model=self.inputMModelLocation, graph = self.graph_data_model, title=title, root=rootNode
+            path_to_data_model=self.inputMModelLocation,
+            graph=self.graph_data_model,
+            title=title,
+            root=rootNode,
         )
 
         emptyManifestURL = mg.get_manifest()
 
-        return mg.populate_manifest_spreadsheet(manifestPath, emptyManifestURL, return_excel = return_excel, title=title)
+        return mg.populate_manifest_spreadsheet(
+            manifestPath, emptyManifestURL, return_excel=return_excel, title=title
+        )
 
     def submit_metadata_manifest(
         self,
         manifest_path: str,
         path_to_json_ld: str,
         dataset_id: str,
         manifest_record_type: str,
         restrict_rules: bool,
         access_token: Optional[str] = None,
         validate_component: Optional[str] = None,
-        use_schema_label: bool = True,
         hide_blanks: bool = False,
         project_scope: List = None,
-        table_manipulation: str = 'replace'
+        table_manipulation: str = "replace",
+        table_column_names: str = "class_label",
+        annotation_keys: str = "class_label",
     ) -> str:
         """Wrap methods that are responsible for validation of manifests for a given component, and association of the
         same manifest file with a specified dataset.
         Args:
             manifest_path: Path to the manifest file, which contains the metadata.
             dataset_id: Synapse ID of the dataset on Synapse containing the metadata manifest file.
             validate_component: Component from the schema.org schema based on which the manifest template has been generated.
         Returns:
             Manifest ID: If both validation and association were successful.
         Exceptions:
             ValueError: When validate_component is provided, but it cannot be found in the schema.
             ValidationError: If validation against data model was not successful.
         """
 
-        #TODO: avoid explicitly exposing Synapse store functionality
+        # TODO: avoid explicitly exposing Synapse store functionality
         # just instantiate a Store class and let it decide at runtime/config
         # the store type
-        syn_store = SynapseStorage(access_token = access_token, project_scope = project_scope)
-        manifest_id=None
-        censored_manifest_id=None
-        restrict_maniest=False
-        censored_manifest_path=manifest_path.replace('.csv','_censored.csv')
+        syn_store = SynapseStorage(
+            access_token=access_token, project_scope=project_scope
+        )
+        manifest_id = None
+        censored_manifest_id = None
+        restrict_maniest = False
+        censored_manifest_path = manifest_path.replace(".csv", "_censored.csv")
         # check if user wants to perform validation or not
         if validate_component is not None:
-
             try:
                 # check if the component ("class" in schema) passed as argument is valid (present in schema) or not
                 self.dmge.is_class_in_schema(validate_component)
             except:
                 # a KeyError exception is raised when validate_component fails in the try-block above
                 # here, we are suppressing the KeyError exception and replacing it with a more
                 # descriptive ValueError exception
                 raise ValueError(
                     f"The component '{validate_component}' could not be found "
                     f"in the schema here '{path_to_json_ld}'"
                 )
 
             # automatic JSON schema generation and validation with that JSON schema
             val_errors, val_warnings = self.validateModelManifest(
-                manifestPath=manifest_path, rootNode=validate_component, restrict_rules=restrict_rules, project_scope=project_scope, access_token=access_token
+                manifestPath=manifest_path,
+                rootNode=validate_component,
+                restrict_rules=restrict_rules,
+                project_scope=project_scope,
+                access_token=access_token,
             )
 
             # if there are no errors in validation process
-            if val_errors == []:                
+            if val_errors == []:
                 # upload manifest file from `manifest_path` path to entity with Syn ID `dataset_id`
                 if os.path.exists(censored_manifest_path):
                     censored_manifest_id = syn_store.associateMetadataWithFiles(
-                        dmge = self.dmge,
-                        metadataManifestPath = censored_manifest_path,
-                        datasetId = dataset_id, 
-                        manifest_record_type = manifest_record_type,
-                        useSchemaLabel = use_schema_label,
-                        hideBlanks = hide_blanks,
+                        dmge=self.dmge,
+                        metadataManifestPath=censored_manifest_path,
+                        datasetId=dataset_id,
+                        manifest_record_type=manifest_record_type,
+                        hideBlanks=hide_blanks,
                         table_manipulation=table_manipulation,
+                        table_column_names=table_column_names,
+                        annotation_keys=annotation_keys,
                     )
                     restrict_maniest = True
-                
+
                 manifest_id = syn_store.associateMetadataWithFiles(
-                    dmge = self.dmge,
-                    metadataManifestPath = manifest_path, 
-                    datasetId = dataset_id, 
-                    manifest_record_type = manifest_record_type,
-                    useSchemaLabel = use_schema_label, 
-                    hideBlanks = hide_blanks,
+                    dmge=self.dmge,
+                    metadataManifestPath=manifest_path,
+                    datasetId=dataset_id,
+                    manifest_record_type=manifest_record_type,
+                    hideBlanks=hide_blanks,
                     restrict_manifest=restrict_maniest,
                     table_manipulation=table_manipulation,
+                    table_column_names=table_column_names,
+                    annotation_keys=annotation_keys,
                 )
 
                 logger.info(f"No validation errors occured during validation.")
                 return manifest_id
-                
+
             else:
                 raise ValidationError(
                     "Manifest could not be validated under provided data model. "
                     f"Validation failed with the following errors: {val_errors}"
                 )
 
         # no need to perform validation, just submit/associate the metadata manifest file
         if os.path.exists(censored_manifest_path):
             censored_manifest_id = syn_store.associateMetadataWithFiles(
-                dmge = self.dmge,
+                dmge=self.dmge,
                 metadataManifestPath=censored_manifest_path,
                 datasetId=dataset_id,
                 manifest_record_type=manifest_record_type,
-                useSchemaLabel=use_schema_label,
                 hideBlanks=hide_blanks,
                 table_manipulation=table_manipulation,
+                table_column_names=table_column_names,
+                annotation_keys=annotation_keys,
             )
             restrict_maniest = True
-        
+
         manifest_id = syn_store.associateMetadataWithFiles(
-            dmge = self.dmge,
+            dmge=self.dmge,
             metadataManifestPath=manifest_path,
             datasetId=dataset_id,
             manifest_record_type=manifest_record_type,
-            useSchemaLabel=use_schema_label,
             hideBlanks=hide_blanks,
             restrict_manifest=restrict_maniest,
             table_manipulation=table_manipulation,
+            table_column_names=table_column_names,
+            annotation_keys=annotation_keys,
         )
 
         logger.debug(
             "Optional validation was not performed on manifest before association."
         )
 
         return manifest_id
```

### Comparing `schematicpy-24.1.1/schematic/models/validate_attribute.py` & `schematicpy-24.2.1/schematic/models/validate_attribute.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,309 +1,330 @@
 import builtins
 import logging
 import re
 import sys
 import time
 from time import perf_counter
 from os import getenv
+
 # allows specifying explicit variable types
 from typing import Any, Dict, List, Optional, Text
 from urllib import error
 from urllib.parse import urlparse
-from urllib.request import (HTTPDefaultErrorHandler, OpenerDirector, Request,
-                            urlopen)
+from urllib.request import HTTPDefaultErrorHandler, OpenerDirector, Request, urlopen
 
 import numpy as np
 import pandas as pd
 from jsonschema import ValidationError
 
 from schematic.schemas.data_model_graph import DataModelGraphExplorer
 
 from schematic.store.base import BaseStorage
 from schematic.store.synapse import SynapseStorage
 from schematic.utils.validate_rules_utils import validation_rule_info
-from schematic.utils.validate_utils import (comma_separated_list_regex,
-                                            parse_str_series_to_list,
-                                            np_array_to_str_list,
-                                            iterable_to_str_list,
-                                            rule_in_rule_list,
-                                            )
+from schematic.utils.validate_utils import (
+    comma_separated_list_regex,
+    parse_str_series_to_list,
+    np_array_to_str_list,
+    iterable_to_str_list,
+    rule_in_rule_list,
+)
 
 from synapseclient.core.exceptions import SynapseNoCredentialsError
 
 logger = logging.getLogger(__name__)
 
+
 class GenerateError:
-    def generate_schema_error(row_num: str, attribute_name: str, error_msg: str, invalid_entry: str, dmge: DataModelGraphExplorer,)-> List[str]:
-        '''
+    def generate_schema_error(
+        row_num: str,
+        attribute_name: str,
+        error_msg: str,
+        invalid_entry: str,
+        dmge: DataModelGraphExplorer,
+    ) -> List[str]:
+        """
         Purpose: Process error messages generated from schema
         Input:
             - row_num: the row the error occurred on.
             - attribute_name: the attribute the error occurred on.
             - error_msg: Error message
-        '''
+        """
         error_list = []
         warning_list = []
-        
-        #Determine which, if any, message to raise
-        if attribute_name.lower() == 'wrong schema':
-            raises = 'error'
-        else:    
+
+        # Determine which, if any, message to raise
+        if attribute_name.lower() == "wrong schema":
+            raises = "error"
+        else:
             raises = GenerateError.get_message_level(
-                val_rule = 'schema',
-                attribute_name = attribute_name,
-                dmge = dmge,
-                )
+                val_rule="schema",
+                attribute_name=attribute_name,
+                dmge=dmge,
+            )
 
-        #if a message needs to be raised, get the approrpiate function to do so
+        # if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logger,raises)  
+            logLevel = getattr(logger, raises)
         else:
             return error_list, warning_list
 
-
         error_col = attribute_name  # Attribute name
         error_row = row_num  # index row of the manifest where the error presented.
         error_message = error_msg
 
         arg_error_string = (
-                f"For the attribute '{error_col}', on row {error_row}, {error_message}."
+            f"For the attribute '{error_col}', on row {error_row}, {error_message}."
         )
         logLevel(arg_error_string)
 
-        if raises == 'error':
+        if raises == "error":
             error_list = [error_row, error_col, error_message, invalid_entry]
-        elif raises == 'warning':
+        elif raises == "warning":
             warning_list = [error_row, error_col, error_message, invalid_entry]
 
-        return error_list, warning_list 
+        return error_list, warning_list
 
     def generate_list_error(
-        list_string: str, row_num: str, attribute_name: str, list_error: str,
-        invalid_entry:str, dmge: DataModelGraphExplorer, val_rule: str,
+        list_string: str,
+        row_num: str,
+        attribute_name: str,
+        list_error: str,
+        invalid_entry: str,
+        dmge: DataModelGraphExplorer,
+        val_rule: str,
     ) -> List[str]:
         """
-            Purpose:
-                If an error is found in the string formatting, detect and record
-                an error message.
-            Input:
-                - list_string: the user input list, that is represented as a string.
-                - row_num: the row the error occurred on.
-                - attribute_name: the attribute the error occurred on.
-            Returns:
-            logger.error or logger.warning.
-            Errors: List[str] Error details for further storage.
-            warnings: List[str] Warning details for further storage.
-            """
+        Purpose:
+            If an error is found in the string formatting, detect and record
+            an error message.
+        Input:
+            - list_string: the user input list, that is represented as a string.
+            - row_num: the row the error occurred on.
+            - attribute_name: the attribute the error occurred on.
+        Returns:
+        logger.error or logger.warning.
+        Errors: List[str] Error details for further storage.
+        warnings: List[str] Warning details for further storage.
+        """
 
         error_list = []
         warning_list = []
-        
-        #Determine which, if any, message to raise
+
+        # Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
-            val_rule = val_rule,
-            attribute_name = attribute_name,
-            dmge = dmge,
-            )
+            val_rule=val_rule,
+            attribute_name=attribute_name,
+            dmge=dmge,
+        )
 
-        #if a message needs to be raised, get the approrpiate function to do so
+        # if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logger,raises)  
+            logLevel = getattr(logger, raises)
         else:
             return error_list, warning_list
 
         if list_error == "not_comma_delimited":
             error_str = (
                 f"For attribute {attribute_name} in row {row_num} it does not "
                 f"appear as if you provided a comma delimited string. Please check "
                 f"your entry ('{list_string}'') and try again."
             )
             logLevel(error_str)
             error_row = row_num  # index row of the manifest where the error presented.
             error_col = attribute_name  # Attribute name
             error_message = error_str
             error_val = invalid_entry
-                #return error and empty list for warnings
-        
-        if raises == 'error':
+            # return error and empty list for warnings
+
+        if raises == "error":
             error_list = [error_row, error_col, error_message, error_val]
-        #return warning and empty list for errors
-        elif raises == 'warning':
+        # return warning and empty list for errors
+        elif raises == "warning":
             warning_list = [error_row, error_col, error_message, error_val]
-        
-        return error_list, warning_list 
+
+        return error_list, warning_list
 
     def generate_regex_error(
         val_rule: str,
         reg_expression: str,
         row_num: str,
         module_to_call: str,
         attribute_name: str,
         invalid_entry: str,
         dmge: DataModelGraphExplorer,
     ) -> List[str]:
         """
-            Purpose:
-                Generate an logging error as well as a stored error message, when
-                a regex error is encountered.
-            Input:
-                val_rule: str, defined in the schema.
-                reg_expression: str, defined in the schema
-                row_num: str, row where the error was detected
-                module_to_call: re module specified in the schema
-                attribute_name: str, attribute being validated
-            Returns:
-            logger.error or logger.warning.
-            Errors: List[str] Error details for further storage.
-            warnings: List[str] Warning details for further storage.
-            """
+        Purpose:
+            Generate an logging error as well as a stored error message, when
+            a regex error is encountered.
+        Input:
+            val_rule: str, defined in the schema.
+            reg_expression: str, defined in the schema
+            row_num: str, row where the error was detected
+            module_to_call: re module specified in the schema
+            attribute_name: str, attribute being validated
+        Returns:
+        logger.error or logger.warning.
+        Errors: List[str] Error details for further storage.
+        warnings: List[str] Warning details for further storage.
+        """
         error_list = []
         warning_list = []
-        
-        #Determine which, if any, message to raise
+
+        # Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
-            val_rule = val_rule,
-            attribute_name = attribute_name,
-            dmge = dmge,
-            )
+            val_rule=val_rule,
+            attribute_name=attribute_name,
+            dmge=dmge,
+        )
 
-        #if a message needs to be raised, get the approrpiate function to do so
+        # if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logger,raises)  
+            logLevel = getattr(logger, raises)
         else:
             return error_list, warning_list
 
         regex_error_string = (
             f"For the attribute {attribute_name}, on row {row_num}, the string is not properly formatted. "
             f'It should follow the following re.{module_to_call} pattern "{reg_expression}".'
         )
         logLevel(regex_error_string)
         error_row = row_num  # index row of the manifest where the error presented.
         error_col = attribute_name  # Attribute name
         error_message = regex_error_string
         error_val = invalid_entry
 
-        #return error and empty list for warnings
-        if raises == 'error':
+        # return error and empty list for warnings
+        if raises == "error":
             error_list = [error_row, error_col, error_message, error_val]
-        #return warning and empty list for errors
-        elif raises == 'warning':
+        # return warning and empty list for errors
+        elif raises == "warning":
             warning_list = [error_row, error_col, error_message, error_val]
-        
-        return error_list, warning_list       
+
+        return error_list, warning_list
 
     def generate_type_error(
-        val_rule: str, row_num: str, attribute_name: str, invalid_entry:str, dmge: DataModelGraphExplorer,
+        val_rule: str,
+        row_num: str,
+        attribute_name: str,
+        invalid_entry: str,
+        dmge: DataModelGraphExplorer,
     ) -> List[str]:
         """
-            Purpose:
-                Generate an logging error as well as a stored error message, when
-                a type error is encountered.
-            Input:
-                val_rule: str, defined in the schema.
-                row_num: str, row where the error was detected
-                attribute_name: str, attribute being validated
-            Returns:
-            logger.error or logger.warning.
-            Errors: List[str] Error details for further storage.
-            warnings: List[str] Warning details for further storage.
-            """
+        Purpose:
+            Generate an logging error as well as a stored error message, when
+            a type error is encountered.
+        Input:
+            val_rule: str, defined in the schema.
+            row_num: str, row where the error was detected
+            attribute_name: str, attribute being validated
+        Returns:
+        logger.error or logger.warning.
+        Errors: List[str] Error details for further storage.
+        warnings: List[str] Warning details for further storage.
+        """
 
         error_list = []
         warning_list = []
 
-        #Determine which, if any, message to raise
+        # Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
-            dmge = dmge,
-            attribute_name = attribute_name,
-            val_rule = val_rule,
-            )
+            dmge=dmge,
+            attribute_name=attribute_name,
+            val_rule=val_rule,
+        )
 
-        #if a message needs to be raised, get the approrpiate function to do so
+        # if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logger,raises)  
+            logLevel = getattr(logger, raises)
         else:
             return error_list, warning_list
 
         type_error_str = (
             f"On row {row_num} the attribute {attribute_name} "
             f"does not contain the proper value type {val_rule}."
         )
         error_row = row_num  # index row of the manifest where the error presented.
         error_col = attribute_name  # Attribute name
         error_message = type_error_str
         error_val = invalid_entry
 
-        #TODO: not sure if this i needed (to split)
-        validation_rules=dmge.get_node_validation_rules(node_display_name=attribute_name)
-
-        #TODO: Can remove when handling updated so split within graph
-        if validation_rules and '::' in validation_rules[0]:
-                validation_rules = validation_rules[0].split("::")
+        # TODO: not sure if this i needed (to split)
+        validation_rules = dmge.get_node_validation_rules(
+            node_display_name=attribute_name
+        )
 
         # If IsNA rule is being used to allow `Not Applicable` entries, do not log a message
-        if error_val.lower() == 'not applicable' and rule_in_rule_list('IsNA', validation_rules):
-          pass  
+        if error_val.lower() == "not applicable" and rule_in_rule_list(
+            "IsNA", validation_rules
+        ):
+            pass
         else:
             logLevel(type_error_str)
-            #return error and empty list for warnings
-            if raises == 'error':
+            # return error and empty list for warnings
+            if raises == "error":
                 error_list = [error_row, error_col, error_message, error_val]
-            #return warning and empty list for errors
-            elif raises == 'warning':
+            # return warning and empty list for errors
+            elif raises == "warning":
                 warning_list = [error_row, error_col, error_message, error_val]
-        
-        return error_list, warning_list              
+
+        return error_list, warning_list
 
     def generate_url_error(
-        url: str, url_error: str, row_num: str, attribute_name: str, argument: str,
-        invalid_entry:str, dmge: DataModelGraphExplorer, val_rule: str,
+        url: str,
+        url_error: str,
+        row_num: str,
+        attribute_name: str,
+        argument: str,
+        invalid_entry: str,
+        dmge: DataModelGraphExplorer,
+        val_rule: str,
     ) -> List[str]:
         """
-            Purpose:
-                Generate an logging error as well as a stored error message, when
-                a URL error is encountered.
-
-                Types of errors included:
-                    - Invalid URL: Refers to a URL that brings up an error when 
-                        attempted to be accessed such as a HTTPError 404 Webpage Not Found.
-                    - Argument Error: this refers to a valid URL that does not 
-                        contain within it the arguments specified by the schema,
-                        such as 'protocols.io' or 'dox.doi.org'
-                    - Random Entry: this refers to an entry try that is not 
-                        validated to be a URL.
-                        e.g. 'lkejrlei', '0', 'not applicable'
-            Input:
-                url: str, that was input by the user.
-                url_error: str, error detected in url_validation()
-                attribute_name: str, attribute being validated
-                argument: str, argument being validated.
-            Returns:
-            logger.error or logger.warning.
-            Errors: List[str] Error details for further storage.
-            warnings: List[str] Warning details for further storage.
-            """
+        Purpose:
+            Generate an logging error as well as a stored error message, when
+            a URL error is encountered.
+
+            Types of errors included:
+                - Invalid URL: Refers to a URL that brings up an error when
+                    attempted to be accessed such as a HTTPError 404 Webpage Not Found.
+                - Argument Error: this refers to a valid URL that does not
+                    contain within it the arguments specified by the schema,
+                    such as 'protocols.io' or 'dox.doi.org'
+                - Random Entry: this refers to an entry try that is not
+                    validated to be a URL.
+                    e.g. 'lkejrlei', '0', 'not applicable'
+        Input:
+            url: str, that was input by the user.
+            url_error: str, error detected in url_validation()
+            attribute_name: str, attribute being validated
+            argument: str, argument being validated.
+        Returns:
+        logger.error or logger.warning.
+        Errors: List[str] Error details for further storage.
+        warnings: List[str] Warning details for further storage.
+        """
 
         error_list = []
         warning_list = []
-        
-        #Determine which, if any, message to raise
+
+        # Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
-            val_rule = val_rule,
-            attribute_name = attribute_name,
-            dmge = dmge,
-            )
+            val_rule=val_rule,
+            attribute_name=attribute_name,
+            dmge=dmge,
+        )
 
-        #if a message needs to be raised, get the approrpiate function to do so
+        # if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logger,raises)  
+            logLevel = getattr(logger, raises)
         else:
             return error_list, warning_list
 
-
         error_row = row_num  # index row of the manifest where the error presented.
         error_col = attribute_name  # Attribute name
         if url_error == "invalid_url":
             invalid_url_error_string = (
                 f"For the attribute '{attribute_name}', on row {row_num}, the URL provided ({url}) does not "
                 f"conform to the standards of a URL. Please make sure you are entering a real, working URL "
                 f"as required by the Schema."
@@ -324,107 +345,107 @@
                 f"For the attribute '{attribute_name}', on row {row_num}, the input provided ('{url}'') does not "
                 f"look like a URL, please check input and try again."
             )
             logLevel(random_entry_error_str)
             error_message = random_entry_error_str
             error_val = f"URL Error: Random Entry"
 
-        #return error and empty list for warnings
-        if raises == 'error':
+        # return error and empty list for warnings
+        if raises == "error":
             error_list = [error_row, error_col, error_message, error_val]
-        #return warning and empty list for errors
-        elif raises == 'warning':
+        # return warning and empty list for errors
+        elif raises == "warning":
             warning_list = [error_row, error_col, error_message, error_val]
-        
-        return error_list, warning_list        
+
+        return error_list, warning_list
 
     def generate_cross_warning(
         val_rule: str,
         attribute_name: str,
         dmge: DataModelGraphExplorer,
-        matching_manifests = [],
-        missing_manifest_ID = None,
-        invalid_entry = None,
-        row_num = None,
-        
+        matching_manifests=[],
+        missing_manifest_ID=None,
+        invalid_entry=None,
+        row_num=None,
     ) -> List[str]:
         """
-            Purpose:
-                Generate an logging error as well as a stored error message, when
-                a cross validation error is encountered.
-            Input:
-                val_rule: str, defined in the schema.
-                matching_manifests: list of manifests with all values in the target attribute present
-                manifest_ID: str, synID of the target manifest missing the source value
-                attribute_name: str, attribute being validated
-                invalid_entry: str, value present in source manifest that is missing in the target
-                row_num: row in source manifest with value missing in target manifests             
-            Returns:
-            logger.error or logger.warning.
-            Errors: List[str] Error details for further storage.
-            warnings: List[str] Warning details for further storage.
-            """
+        Purpose:
+            Generate an logging error as well as a stored error message, when
+            a cross validation error is encountered.
+        Input:
+            val_rule: str, defined in the schema.
+            matching_manifests: list of manifests with all values in the target attribute present
+            manifest_ID: str, synID of the target manifest missing the source value
+            attribute_name: str, attribute being validated
+            invalid_entry: str, value present in source manifest that is missing in the target
+            row_num: row in source manifest with value missing in target manifests
+        Returns:
+        logger.error or logger.warning.
+        Errors: List[str] Error details for further storage.
+        warnings: List[str] Warning details for further storage.
+        """
         error_list = []
         warning_list = []
-        
-        #Determine which, if any, message to raise
+
+        # Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
-            val_rule = val_rule,
-            attribute_name = attribute_name,
-            dmge = dmge,
-            )
+            val_rule=val_rule,
+            attribute_name=attribute_name,
+            dmge=dmge,
+        )
 
-        #if a message needs to be raised, get the approrpiate function to do so
+        # if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logger,raises)  
+            logLevel = getattr(logger, raises)
         else:
             return error_list, warning_list
 
-        if val_rule.__contains__('matchAtLeast'):
-            cross_error_str = (
-                f"Value(s) {invalid_entry} from row(s) {row_num} of the attribute {attribute_name} in the source manifest are missing." )
-            cross_error_str += f" Manifest(s) {missing_manifest_ID} are missing the value(s)." if missing_manifest_ID else ""
-            
-        elif val_rule.__contains__('matchExactly'):
+        if val_rule.__contains__("matchAtLeast"):
+            cross_error_str = f"Value(s) {invalid_entry} from row(s) {row_num} of the attribute {attribute_name} in the source manifest are missing."
+            cross_error_str += (
+                f" Manifest(s) {missing_manifest_ID} are missing the value(s)."
+                if missing_manifest_ID
+                else ""
+            )
+
+        elif val_rule.__contains__("matchExactly"):
             if matching_manifests != []:
-                cross_error_str = (
-                    f"All values from attribute {attribute_name} in the source manifest are present in {len(matching_manifests)} manifests instead of only 1.")
-                cross_error_str += f" Manifests {matching_manifests} match the values in the source attribute." if matching_manifests else ""
-                    
-            elif val_rule.__contains__('set'):
-                cross_error_str = (
-                    f"No matches for the values from attribute {attribute_name} in the source manifest are present in any other manifests instead of being present in exactly 1. "
+                cross_error_str = f"All values from attribute {attribute_name} in the source manifest are present in {len(matching_manifests)} manifests instead of only 1."
+                cross_error_str += (
+                    f" Manifests {matching_manifests} match the values in the source attribute."
+                    if matching_manifests
+                    else ""
                 )
-            elif val_rule.__contains__('value'):
-                cross_error_str = (
-                    f"Value(s) {invalid_entry} from row(s) {row_num} of the attribute {attribute_name} in the source manifest are not present in only one other manifest. " 
-                )            
+
+            elif val_rule.__contains__("set"):
+                cross_error_str = f"No matches for the values from attribute {attribute_name} in the source manifest are present in any other manifests instead of being present in exactly 1. "
+            elif val_rule.__contains__("value"):
+                cross_error_str = f"Value(s) {invalid_entry} from row(s) {row_num} of the attribute {attribute_name} in the source manifest are not present in only one other manifest. "
 
         logLevel(cross_error_str)
         error_row = row_num  # index row of the manifest where the error presented.
         error_col = attribute_name  # Attribute name
         error_message = cross_error_str
-        error_val = invalid_entry #Value from source manifest missing from targets
-        
-        #return error and empty list for warnings
-        if raises == 'error':
+        error_val = invalid_entry  # Value from source manifest missing from targets
+
+        # return error and empty list for warnings
+        if raises == "error":
             error_list = [error_row, error_col, error_message, error_val]
-        #return warning and empty list for errors
-        elif raises == 'warning':
+        # return warning and empty list for errors
+        elif raises == "warning":
             warning_list = [error_row, error_col, error_message, error_val]
-        
-        return error_list, warning_list        
 
+        return error_list, warning_list
 
     def generate_content_error(
         val_rule: str,
         attribute_name: str,
         dmge: DataModelGraphExplorer,
-        row_num = None,
-        error_val = None,    
+        row_num=None,
+        error_val=None,
     ) -> (List[str], List[str]):
         """
         Purpose:
             Generate an logging error or warning as well as a stored error/warning message when validating the content of a manifest attribute.
 
             Types of error/warning included:
                 - recommended - Raised when an attribute is empty and recommended but not required.
@@ -444,92 +465,82 @@
         """
         error_list = []
         warning_list = []
         error_col = attribute_name  # Attribute name
         if error_val:
             error_val = iterable_to_str_list(set(error_val))
 
-        #Determine which, if any, message to raise
+        # Determine which, if any, message to raise
         raises = GenerateError.get_message_level(
             val_rule=val_rule,
-            attribute_name = attribute_name,
-            dmge = dmge,
-            )
+            attribute_name=attribute_name,
+            dmge=dmge,
+        )
 
-        #if a message needs to be raised, get the approrpiate function to do so
+        # if a message needs to be raised, get the approrpiate function to do so
         if raises:
-            logLevel = getattr(logger,raises)  
+            logLevel = getattr(logger, raises)
         else:
             return error_list, warning_list
-        
-        #log warning or error message
-        if val_rule.startswith('recommended'):
-            content_error_str = (
-                f"Column {attribute_name} is recommended but empty."
-            )
+
+        # log warning or error message
+        if val_rule.startswith("recommended"):
+            content_error_str = f"Column {attribute_name} is recommended but empty."
             logLevel(content_error_str)
             error_message = content_error_str
 
-            if raises == 'error':
+            if raises == "error":
                 error_list = [error_col, error_message]
-            #return warning and empty list for errors
-            elif raises == 'warning':
+            # return warning and empty list for errors
+            elif raises == "warning":
                 warning_list = [error_col, error_message]
 
             return error_list, warning_list
 
-        elif val_rule.startswith('unique'):    
-            content_error_str = (
-                f"Column {attribute_name} has the duplicate value(s) {error_val} in rows: {row_num}."
-            )
+        elif val_rule.startswith("unique"):
+            content_error_str = f"Column {attribute_name} has the duplicate value(s) {error_val} in rows: {row_num}."
 
-        elif val_rule.startswith('protectAges'):
-            content_error_str = (
-                f"Column {attribute_name} contains ages that should be censored in rows: {row_num}."
-            )           
+        elif val_rule.startswith("protectAges"):
+            content_error_str = f"Column {attribute_name} contains ages that should be censored in rows: {row_num}."
 
-        elif val_rule.startswith('inRange'):
-            content_error_str = (
-                f"{attribute_name} values in rows {row_num} are out of the specified range."
-            )
-        elif val_rule.startswith('date'):
+        elif val_rule.startswith("inRange"):
+            content_error_str = f"{attribute_name} values in rows {row_num} are out of the specified range."
+        elif val_rule.startswith("date"):
             content_error_str = (
                 f"{attribute_name} values in rows {row_num} are not parsable as dates."
-            )  
-        elif val_rule.startswith('IsNA'):
-            content_error_str = (
-                f"{attribute_name} values in rows {row_num} are not marked as 'Not Applicable'."
-            )  
+            )
+        elif val_rule.startswith("IsNA"):
+            content_error_str = f"{attribute_name} values in rows {row_num} are not marked as 'Not Applicable'."
 
         if val_rule != "IsNA":
             logLevel(content_error_str)
-            error_row = row_num 
+            error_row = row_num
             error_message = content_error_str
-            #return error and empty list for warnings
-            if raises == 'error':
+            # return error and empty list for warnings
+            if raises == "error":
                 error_list = [error_row, error_col, error_message, error_val]
-            #return warning and empty list for errors
-            elif raises == 'warning':
+            # return warning and empty list for errors
+            elif raises == "warning":
                 warning_list = [error_row, error_col, error_message, error_val]
-        
+
         return error_list, warning_list
 
     def get_message_level(
         dmge: DataModelGraphExplorer,
         attribute_name: str,
         val_rule: str,
-        ) -> str:
+    ) -> str:
         """
         Purpose:
             Determine whether an error or warning message should be logged and displayed
-            
-            if node is not required, 
+
+            if node is not required,
                 return warning
-            if node is recommended and requried, 
-                return None    
+            if node is recommended and requried,
+                return None
             for other rules, parse possible, if not use default specified in validation_rule_info
 
         Input:
                 val_rule: str, defined in the schema.
                 dmge: DataModelGraphExplorer object
                 attribute_name: str, attribute being validated
         Returns:
@@ -537,30 +548,34 @@
         # TODO: recommended and other rules
         """
 
         level = None
         rule_parts = val_rule.split(" ")
         rule_info = validation_rule_info()
 
-        #set message level to default and change after
-        if rule_parts[0] != 'schema':
-            level = rule_info[rule_parts[0]]['default_message_level']
+        # set message level to default and change after
+        if rule_parts[0] != "schema":
+            level = rule_info[rule_parts[0]]["default_message_level"]
         # Parse rule for level, set to default if not specified
-        if rule_parts[-1].lower() == 'error' or rule_parts[0] == 'schema':
-            level = 'error'
-        elif rule_parts[-1].lower() == 'warning':
-            level = 'warning'        
+        if rule_parts[-1].lower() == "error" or rule_parts[0] == "schema":
+            level = "error"
+        elif rule_parts[-1].lower() == "warning":
+            level = "warning"
         elif not dmge.get_node_required(node_display_name=attribute_name):
             # If not required raise warnings to notify
-            level = 'warning' 
-        elif dmge.get_node_required(node_display_name=attribute_name) and 'recommended' in val_rule:
+            level = "warning"
+        elif (
+            dmge.get_node_required(node_display_name=attribute_name)
+            and "recommended" in val_rule
+        ):
             level = None
-            
+
         return level
 
+
 class ValidateAttribute(object):
     """
     A collection of functions to validate manifest attributes.
         list_validation
         regex_validation
         type_validation
         url_validation
@@ -568,45 +583,56 @@
         get_target_manifests - helper function
     See functions for more details.
     TODO:
         - Add year validator
         - Add string length validator
     """
 
-    def get_target_manifests(target_component, project_scope: List, access_token: str = None):
+    def get_target_manifests(
+        target_component, project_scope: List, access_token: str = None
+    ):
         t_manifest_search = perf_counter()
-        target_manifest_IDs=[]
-        target_dataset_IDs=[]
-        
-        #login
+        target_manifest_IDs = []
+        target_dataset_IDs = []
+
+        # login
         try:
-            synStore = SynapseStorage(access_token=access_token, project_scope=project_scope)        
+            synStore = SynapseStorage(
+                access_token=access_token, project_scope=project_scope
+            )
         except SynapseNoCredentialsError as e:
             raise ValueError(
                 "No Synapse credentials were provided. Credentials must be provided to utilize cross-manfiest validation functionality."
-                ) from e
+            ) from e
 
-        #Get list of all projects user has access to
+        # Get list of all projects user has access to
         projects = synStore.getStorageProjects(project_scope=project_scope)
         for project in projects:
-            
-            #get all manifests associated with datasets in the projects
-            target_datasets=synStore.getProjectManifests(projectId=project[0])
+            # get all manifests associated with datasets in the projects
+            target_datasets = synStore.getProjectManifests(projectId=project[0])
 
-            #If the manifest includes the target component, include synID in list
+            # If the manifest includes the target component, include synID in list
             for target_dataset in target_datasets:
-                if target_component == target_dataset[-1][0].replace(" ","").lower() and target_dataset[1][0] != "":
+                if (
+                    target_component == target_dataset[-1][0].replace(" ", "").lower()
+                    and target_dataset[1][0] != ""
+                ):
                     target_manifest_IDs.append(target_dataset[1][0])
                     target_dataset_IDs.append(target_dataset[0][0])
 
-        logger.debug(f"Cross manifest gathering elapsed time {perf_counter()-t_manifest_search}")
-        return synStore, target_manifest_IDs, target_dataset_IDs    
+        logger.debug(
+            f"Cross manifest gathering elapsed time {perf_counter()-t_manifest_search}"
+        )
+        return synStore, target_manifest_IDs, target_dataset_IDs
 
     def list_validation(
-        self, val_rule: str, manifest_col: pd.core.series.Series, dmge: DataModelGraphExplorer,
+        self,
+        val_rule: str,
+        manifest_col: pd.core.series.Series,
+        dmge: DataModelGraphExplorer,
     ) -> (List[List[str]], List[List[str]], pd.core.series.Series):
         """
         Purpose:
             Determine if values for a particular attribute are comma separated.
         Input:
             - val_rule: str, Validation rule
             - manifest_col: pd.core.series.Series, column for a given attribute
@@ -621,72 +647,73 @@
         # convert to a real list of strings, with leading and trailing
         # white spaces removed.
         errors = []
         warnings = []
         manifest_col = manifest_col.astype(str)
         csv_re = comma_separated_list_regex()
 
-        rule_parts=val_rule.lower().split(" ")
+        rule_parts = val_rule.lower().split(" ")
         if len(rule_parts) > 1:
-            list_robustness=rule_parts[1]
+            list_robustness = rule_parts[1]
         else:
-            list_robustness = 'strict'
+            list_robustness = "strict"
 
-
-        if list_robustness == 'strict':
-        # This will capture any if an entry is not formatted properly. Only for strict lists
+        if list_robustness == "strict":
+            # This will capture any if an entry is not formatted properly. Only for strict lists
             for i, list_string in enumerate(manifest_col):
-                if not re.fullmatch(csv_re,list_string):
+                if not re.fullmatch(csv_re, list_string):
                     list_error = "not_comma_delimited"
                     vr_errors, vr_warnings = GenerateError.generate_list_error(
-                            list_string,
-                            row_num=str(i + 2),
-                            attribute_name=manifest_col.name,
-                            list_error=list_error,
-                            invalid_entry=manifest_col[i],
-                            dmge = dmge,
-                            val_rule = val_rule, 
-                        )
+                        list_string,
+                        row_num=str(i + 2),
+                        attribute_name=manifest_col.name,
+                        list_error=list_error,
+                        invalid_entry=manifest_col[i],
+                        dmge=dmge,
+                        val_rule=val_rule,
+                    )
                     if vr_errors:
                         errors.append(vr_errors)
                     if vr_warnings:
                         warnings.append(vr_warnings)
-                
 
         # Convert string to list.
         manifest_col = parse_str_series_to_list(manifest_col)
 
         return errors, warnings, manifest_col
 
     def regex_validation(
-        self, val_rule: str, manifest_col: pd.core.series.Series, dmge: DataModelGraphExplorer,
+        self,
+        val_rule: str,
+        manifest_col: pd.core.series.Series,
+        dmge: DataModelGraphExplorer,
     ) -> (List[List[str]], List[List[str]]):
         """
         Purpose:
             Check if values for a given manifest attribue conform to the reguar expression,
             provided in val_rule.
         Input:
             - val_rule: str, Validation rule
             - manifest_col: pd.core.series.Series, column for a given
                 attribute in the manifest
             - dmge: DataModelGraphExplorer Object
             Using this module requres validation rules written in the following manner:
                 'regex module regular expression'
-                - regex: is an exact string specifying that the input is to be validated as a 
+                - regex: is an exact string specifying that the input is to be validated as a
                 regular expression.
-                - module: is the name of the module within re to run ie. search. 
+                - module: is the name of the module within re to run ie. search.
                 - regular_expression: is the regular expression with which to validate
                 the user input.
         Returns:
             - This function will return errors when the user input value
             does not match schema specifications.
             logger.error or logger.warning.
             Errors: List[str] Error details for further storage.
             warnings: List[str] Warning details for further storage.
-        TODO: 
+        TODO:
             move validation to convert step.
         """
 
         reg_exp_rules = val_rule.split(" ")
 
         try:
             module_to_call = getattr(re, reg_exp_rules[1])
@@ -696,68 +723,73 @@
                 f"The regex rules were not provided properly for attribute {manifest_col.name}."
                 f" They should be provided as follows ['regex', 'module name', 'regular expression']"
             )
 
         errors = []
         warnings = []
 
-        validation_rules = dmge.get_node_validation_rules(node_display_name=manifest_col.name)
-        if validation_rules and '::' in validation_rules[0]:
-                validation_rules = validation_rules[0].split("::")
+        validation_rules = dmge.get_node_validation_rules(
+            node_display_name=manifest_col.name
+        )
+        if validation_rules and "::" in validation_rules[0]:
+            validation_rules = validation_rules[0].split("::")
         # Handle case where validating re's within a list.
-        if re.search('list',"|".join(validation_rules)):
+        if re.search("list", "|".join(validation_rules)):
             if type(manifest_col[0]) == str:
                 # Convert string to list.
                 manifest_col = parse_str_series_to_list(manifest_col)
 
             for i, row_values in enumerate(manifest_col):
                 for j, re_to_check in enumerate(row_values):
                     re_to_check = str(re_to_check)
                     if not bool(module_to_call(reg_expression, re_to_check)) and bool(
                         re_to_check
                     ):
                         vr_errors, vr_warnings = GenerateError.generate_regex_error(
-                                val_rule = val_rule,
-                                reg_expression = reg_expression,
-                                row_num=str(i + 2),
-                                module_to_call=reg_exp_rules[1],
-                                attribute_name=manifest_col.name,
-                                invalid_entry=manifest_col[i],
-                                dmge = dmge,
-                            )
+                            val_rule=val_rule,
+                            reg_expression=reg_expression,
+                            row_num=str(i + 2),
+                            module_to_call=reg_exp_rules[1],
+                            attribute_name=manifest_col.name,
+                            invalid_entry=manifest_col[i],
+                            dmge=dmge,
+                        )
                         if vr_errors:
                             errors.append(vr_errors)
                         if vr_warnings:
                             warnings.append(vr_warnings)
 
         # Validating single re's
         else:
             manifest_col = manifest_col.astype(str)
             for i, re_to_check in enumerate(manifest_col):
                 if not bool(module_to_call(reg_expression, re_to_check)) and bool(
                     re_to_check
                 ):
                     vr_errors, vr_warnings = GenerateError.generate_regex_error(
-                            val_rule = val_rule,
-                            reg_expression = reg_expression,
-                            row_num=str(i + 2),
-                            module_to_call=reg_exp_rules[1],
-                            attribute_name=manifest_col.name,
-                            invalid_entry=manifest_col[i],
-                            dmge = dmge,
-                        )
+                        val_rule=val_rule,
+                        reg_expression=reg_expression,
+                        row_num=str(i + 2),
+                        module_to_call=reg_exp_rules[1],
+                        attribute_name=manifest_col.name,
+                        invalid_entry=manifest_col[i],
+                        dmge=dmge,
+                    )
                     if vr_errors:
                         errors.append(vr_errors)
                     if vr_warnings:
                         warnings.append(vr_warnings)
 
         return errors, warnings
 
     def type_validation(
-        self, val_rule: str, manifest_col: pd.core.series.Series, dmge: DataModelGraphExplorer,
+        self,
+        val_rule: str,
+        manifest_col: pd.core.series.Series,
+        dmge: DataModelGraphExplorer,
     ) -> (List[List[str]], List[List[str]]):
         """
         Purpose:
             Check if values for a given manifest attribue are the same type
             specified in val_rule.
         Input:
             - val_rule: str, Validation rule, specifying input type, either
@@ -771,54 +803,56 @@
             logger.error or logger.warning.
             Errors: List[str] Error details for further storage.
             warnings: List[str] Warning details for further storage.
         TODO:
             Convert all inputs to .lower() just to prevent any entry errors.
         """
         specified_type = {
-            'num': (int, np.int64, float),
-            'int': (int, np.int64),
-            'float': (float),
-            'str': (str),
+            "num": (int, np.int64, float),
+            "int": (int, np.int64),
+            "float": (float),
+            "str": (str),
         }
 
         errors = []
         warnings = []
         # num indicates either a float or int.
         if val_rule == "num":
             for i, value in enumerate(manifest_col):
                 if bool(value) and not isinstance(value, specified_type[val_rule]):
                     vr_errors, vr_warnings = GenerateError.generate_type_error(
-                            val_rule = val_rule ,
-                            row_num=str(i + 2),
-                            attribute_name=manifest_col.name,
-                            invalid_entry=str(manifest_col[i]),
-                            dmge = dmge,
-                        )
+                        val_rule=val_rule,
+                        row_num=str(i + 2),
+                        attribute_name=manifest_col.name,
+                        invalid_entry=str(manifest_col[i]),
+                        dmge=dmge,
+                    )
                     if vr_errors:
                         errors.append(vr_errors)
                     if vr_warnings:
                         warnings.append(vr_warnings)
         elif val_rule in ["int", "float", "str"]:
             for i, value in enumerate(manifest_col):
                 if bool(value) and not isinstance(value, specified_type[val_rule]):
                     vr_errors, vr_warnings = GenerateError.generate_type_error(
-                            val_rule = val_rule,
-                            row_num=str(i + 2),
-                            attribute_name=manifest_col.name,
-                            invalid_entry=str(manifest_col[i]),
-                            dmge = dmge,
-                        )
+                        val_rule=val_rule,
+                        row_num=str(i + 2),
+                        attribute_name=manifest_col.name,
+                        invalid_entry=str(manifest_col[i]),
+                        dmge=dmge,
+                    )
                     if vr_errors:
                         errors.append(vr_errors)
                     if vr_warnings:
                         warnings.append(vr_warnings)
         return errors, warnings
 
-    def url_validation(self, val_rule: str, manifest_col: str, dmge: DataModelGraphExplorer) -> (List[List[str]], List[List[str]]):
+    def url_validation(
+        self, val_rule: str, manifest_col: str, dmge: DataModelGraphExplorer
+    ) -> (List[List[str]], List[List[str]]):
         """
         Purpose:
             Validate URL's submitted for a particular attribute in a manifest.
             Determine if the URL is valid and contains attributes specified in the
             schema.
         Input:
             - val_rule: str, Validation rule
@@ -833,34 +867,34 @@
         url_args = val_rule.split(" ")[1:]
         errors = []
         warnings = []
 
         for i, url in enumerate(manifest_col):
             # Check if a random phrase, string or number was added and
             # log the appropriate error.
-            if not isinstance(url,str) or not (
+            if not isinstance(url, str) or not (
                 urlparse(url).scheme
                 + urlparse(url).netloc
                 + urlparse(url).params
                 + urlparse(url).query
                 + urlparse(url).fragment
             ):
                 #
                 url_error = "random_entry"
                 valid_url = False
                 vr_errors, vr_warnings = GenerateError.generate_url_error(
-                        url,
-                        url_error=url_error,
-                        row_num=str(i + 2),
-                        attribute_name=manifest_col.name,
-                        argument=url_args,
-                        invalid_entry=manifest_col[i],
-                        dmge = dmge,
-                        val_rule = val_rule,
-                    )
+                    url,
+                    url_error=url_error,
+                    row_num=str(i + 2),
+                    attribute_name=manifest_col.name,
+                    argument=url_args,
+                    invalid_entry=manifest_col[i],
+                    dmge=dmge,
+                    val_rule=val_rule,
+                )
                 if vr_errors:
                     errors.append(vr_errors)
                 if vr_warnings:
                     warnings.append(vr_warnings)
             else:
                 # add scheme to the URL if not currently added.
                 if not urlparse(url).scheme:
@@ -872,196 +906,225 @@
                     response = urlopen(request)
                     valid_url = True
                     response_code = response.getcode()
                 except:
                     valid_url = False
                     url_error = "invalid_url"
                     vr_errors, vr_warnings = GenerateError.generate_url_error(
-                            url,
-                            url_error=url_error,
-                            row_num=str(i + 2),
-                            attribute_name=manifest_col.name,
-                            argument=url_args,
-                            invalid_entry=manifest_col[i],
-                            dmge = dmge,
-                            val_rule = val_rule,
-                        )
+                        url,
+                        url_error=url_error,
+                        row_num=str(i + 2),
+                        attribute_name=manifest_col.name,
+                        argument=url_args,
+                        invalid_entry=manifest_col[i],
+                        dmge=dmge,
+                        val_rule=val_rule,
+                    )
                     if vr_errors:
                         errors.append(vr_errors)
                     if vr_warnings:
                         warnings.append(vr_warnings)
                 if valid_url == True:
                     # If the URL works, check to see if it contains the proper arguments
                     # as specified in the schema.
                     for arg in url_args:
                         if arg not in url:
                             url_error = "arg_error"
                             vr_errors, vr_warnings = GenerateError.generate_url_error(
-                                    url,
-                                    url_error=url_error,
-                                    row_num=str(i + 2),
-                                    attribute_name=manifest_col.name,
-                                    argument=arg,
-                                    invalid_entry=manifest_col[i],
-                                    dmge = dmge,
-                                    val_rule = val_rule,
-                                )
+                                url,
+                                url_error=url_error,
+                                row_num=str(i + 2),
+                                attribute_name=manifest_col.name,
+                                argument=arg,
+                                invalid_entry=manifest_col[i],
+                                dmge=dmge,
+                                val_rule=val_rule,
+                            )
                             if vr_errors:
                                 errors.append(vr_errors)
                             if vr_warnings:
                                 warnings.append(vr_warnings)
         return errors, warnings
 
     def cross_validation(
-        self, val_rule: str, manifest_col: pd.core.series.Series, project_scope: List, dmge: DataModelGraphExplorer, access_token: str,
+        self,
+        val_rule: str,
+        manifest_col: pd.core.series.Series,
+        project_scope: List,
+        dmge: DataModelGraphExplorer,
+        access_token: str,
     ) -> List[List[str]]:
         """
         Purpose:
             Do cross validation between the current manifest and all other manifests a user has access to on Synapse.
             Check if values in this manifest are present fully in others.
         Input:
             - val_rule: str, Validation rule
             - manifest_col: pd.core.series.Series, column for a given
                 attribute in the manifest
             - dmge: DataModelGraphExplorer Object
         Output:
-            This function will return errors when values in the current manifest's attribute 
+            This function will return errors when values in the current manifest's attribute
             are not fully present in the correct amount of other manifests.
         """
         errors = []
         warnings = []
         missing_values = {}
-        missing_manifest_log={}
-        present_manifest_log=[]
+        missing_manifest_log = {}
+        present_manifest_log = []
         target_column = pd.Series(dtype=object)
-        #parse sources and targets
-        source_attribute=manifest_col.name
+        # parse sources and targets
+        source_attribute = manifest_col.name
         [target_component, target_attribute] = val_rule.lower().split(" ")[1].split(".")
-        scope=val_rule.lower().split(" ")[2]
-        target_column.name=target_attribute
+        scope = val_rule.lower().split(" ")[2]
+        target_column.name = target_attribute
 
-        
-        #Get IDs of manifests with target component
-        synStore, target_manifest_IDs, target_dataset_IDs = ValidateAttribute.get_target_manifests(target_component, project_scope, access_token)
+        # Get IDs of manifests with target component
+        (
+            synStore,
+            target_manifest_IDs,
+            target_dataset_IDs,
+        ) = ValidateAttribute.get_target_manifests(
+            target_component, project_scope, access_token
+        )
 
         t_cross_manifest = perf_counter()
-        #Read each manifest
-        for target_manifest_ID, target_dataset_ID in zip(target_manifest_IDs,target_dataset_IDs):
+        # Read each manifest
+        for target_manifest_ID, target_dataset_ID in zip(
+            target_manifest_IDs, target_dataset_IDs
+        ):
             entity = synStore.getDatasetManifest(
-                datasetId = target_dataset_ID,
-                downloadFile = True
-                )
-            target_manifest=pd.read_csv(entity.path)
+                datasetId=target_dataset_ID, downloadFile=True
+            )
+            target_manifest = pd.read_csv(entity.path)
 
-            #convert manifest column names into validation rule input format - 
-            column_names={}
+            # convert manifest column names into validation rule input format -
+            column_names = {}
             for name in target_manifest.columns:
-                column_names[name.replace(" ","").lower()]=name
+                column_names[name.replace(" ", "").lower()] = name
 
-            if scope.__contains__('set'):
-                #If the manifest has the target attribute for the component do the cross validation
-                if target_attribute in column_names:                    
+            if scope.__contains__("set"):
+                # If the manifest has the target attribute for the component do the cross validation
+                if target_attribute in column_names:
                     target_column = target_manifest[column_names[target_attribute]]
 
-                    #Do the validation on both columns
+                    # Do the validation on both columns
                     missing_values = manifest_col[~manifest_col.isin(target_column)]
 
                     if missing_values.empty:
                         present_manifest_log.append(target_manifest_ID)
                     else:
                         missing_manifest_log[target_manifest_ID] = missing_values
 
-            elif scope.__contains__('value'):
+            elif scope.__contains__("value"):
                 if target_attribute in column_names:
-                    target_manifest.rename(columns={column_names[target_attribute]: target_attribute}, inplace=True)
-                    
+                    target_manifest.rename(
+                        columns={column_names[target_attribute]: target_attribute},
+                        inplace=True,
+                    )
+
                     target_column = pd.concat(
-                        objs = [target_column, target_manifest[target_attribute]],
-                        join = 'outer',
-                        ignore_index= True,
-                    )                
-                    target_column = target_column.astype('object')
-                    #print(target_column)
-                    
-        
-        
-        missing_rows=[]
-        missing_values=[]  
+                        objs=[target_column, target_manifest[target_attribute]],
+                        join="outer",
+                        ignore_index=True,
+                    )
+                    target_column = target_column.astype("object")
+                    # print(target_column)
 
+        missing_rows = []
+        missing_values = []
 
-        if scope.__contains__('value'):
+        if scope.__contains__("value"):
             missing_values = manifest_col[~manifest_col.isin(target_column)]
-            duplicated_values = manifest_col[manifest_col.isin(target_column[target_column.duplicated()])]
-            
-            if val_rule.__contains__('matchAtLeastOne') and not missing_values.empty:
+            duplicated_values = manifest_col[
+                manifest_col.isin(target_column[target_column.duplicated()])
+            ]
+
+            if val_rule.__contains__("matchAtLeastOne") and not missing_values.empty:
                 missing_rows = missing_values.index.to_numpy() + 2
                 missing_rows = np_array_to_str_list(missing_rows)
                 vr_errors, vr_warnings = GenerateError.generate_cross_warning(
-                        val_rule = val_rule,
-                        row_num = missing_rows,
-                        attribute_name = source_attribute,
-                        invalid_entry = iterable_to_str_list(missing_values),
-                        dmge = dmge,
-                    )
+                    val_rule=val_rule,
+                    row_num=missing_rows,
+                    attribute_name=source_attribute,
+                    invalid_entry=iterable_to_str_list(missing_values),
+                    dmge=dmge,
+                )
                 if vr_errors:
                     errors.append(vr_errors)
                 if vr_warnings:
                     warnings.append(vr_warnings)
-            elif val_rule.__contains__('matchExactlyOne') and (duplicated_values.any() or missing_values.any()):
-                invalid_values  = pd.merge(duplicated_values,missing_values,how='outer')
-                invalid_rows    = pd.merge(duplicated_values,missing_values,how='outer',left_index=True,right_index=True).index.to_numpy() + 2
-                invalid_rows    = np_array_to_str_list(invalid_rows)
+            elif val_rule.__contains__("matchExactlyOne") and (
+                duplicated_values.any() or missing_values.any()
+            ):
+                invalid_values = pd.merge(
+                    duplicated_values, missing_values, how="outer"
+                )
+                invalid_rows = (
+                    pd.merge(
+                        duplicated_values,
+                        missing_values,
+                        how="outer",
+                        left_index=True,
+                        right_index=True,
+                    ).index.to_numpy()
+                    + 2
+                )
+                invalid_rows = np_array_to_str_list(invalid_rows)
                 vr_errors, vr_warnings = GenerateError.generate_cross_warning(
-                        val_rule = val_rule,
-                        row_num = invalid_rows,
-                        attribute_name = source_attribute, 
-                        invalid_entry = iterable_to_str_list(invalid_values.squeeze()),
-                        dmge = dmge,
-                    )
+                    val_rule=val_rule,
+                    row_num=invalid_rows,
+                    attribute_name=source_attribute,
+                    invalid_entry=iterable_to_str_list(invalid_values.squeeze()),
+                    dmge=dmge,
+                )
                 if vr_errors:
                     errors.append(vr_errors)
                 if vr_warnings:
                     warnings.append(vr_warnings)
-            
 
-            
-        #generate warnings if necessary
-        elif scope.__contains__('set'):
-            if val_rule.__contains__('matchAtLeastOne') and len(present_manifest_log) < 1:     
-                missing_entries = list(missing_manifest_log.values()) 
-                missing_manifest_IDs = list(missing_manifest_log.keys()) 
+        # generate warnings if necessary
+        elif scope.__contains__("set"):
+            if (
+                val_rule.__contains__("matchAtLeastOne")
+                and len(present_manifest_log) < 1
+            ):
+                missing_entries = list(missing_manifest_log.values())
+                missing_manifest_IDs = list(missing_manifest_log.keys())
                 for missing_entry in missing_entries:
-                    missing_rows.append(missing_entry.index[0]+2)
+                    missing_rows.append(missing_entry.index[0] + 2)
                     missing_values.append(missing_entry.values[0])
-                    
-                missing_rows=iterable_to_str_list(set(missing_rows))
-                missing_values=iterable_to_str_list(set(missing_values))
-                
+
+                missing_rows = iterable_to_str_list(set(missing_rows))
+                missing_values = iterable_to_str_list(set(missing_values))
+
                 vr_errors, vr_warnings = GenerateError.generate_cross_warning(
-                        val_rule = val_rule,
-                        row_num = missing_rows,
-                        attribute_name = source_attribute,
-                        invalid_entry = missing_values,
-                        missing_manifest_ID = missing_manifest_IDs,
-                        dmge = dmge,
-                    )
+                    val_rule=val_rule,
+                    row_num=missing_rows,
+                    attribute_name=source_attribute,
+                    invalid_entry=missing_values,
+                    missing_manifest_ID=missing_manifest_IDs,
+                    dmge=dmge,
+                )
                 if vr_errors:
                     errors.append(vr_errors)
                 if vr_warnings:
                     warnings.append(vr_warnings)
-            elif val_rule.__contains__('matchExactlyOne') and len(present_manifest_log) != 1:
+            elif (
+                val_rule.__contains__("matchExactlyOne")
+                and len(present_manifest_log) != 1
+            ):
                 vr_errors, vr_warnings = GenerateError.generate_cross_warning(
-                        val_rule = val_rule,
-                        attribute_name = source_attribute,
-                        matching_manifests = present_manifest_log,
-                        dmge = dmge,
-                    )
+                    val_rule=val_rule,
+                    attribute_name=source_attribute,
+                    matching_manifests=present_manifest_log,
+                    dmge=dmge,
+                )
                 if vr_errors:
                     errors.append(vr_errors)
                 if vr_warnings:
                     warnings.append(vr_warnings)
-                
 
-        logger.debug(f"cross manifest validation time {perf_counter()-t_cross_manifest}")
+        logger.debug(
+            f"cross manifest validation time {perf_counter()-t_cross_manifest}"
+        )
         return errors, warnings
-
-
```

### Comparing `schematicpy-24.1.1/schematic/models/validate_manifest.py` & `schematicpy-24.2.1/schematic/models/validate_manifest.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,46 +6,50 @@
 
 import numpy as np
 import os
 import pandas as pd
 import re
 import sys
 from time import perf_counter
+from numbers import Number
 
 # allows specifying explicit variable types
 from typing import Any, Dict, Optional, Text, List
 from urllib.parse import urlparse
 from urllib.request import urlopen, OpenerDirector, HTTPDefaultErrorHandler
 from urllib.request import Request
 from urllib import error
 
 from schematic.models.validate_attribute import ValidateAttribute, GenerateError
+
 from schematic.schemas.data_model_graph import DataModelGraphExplorer
 from schematic.store.synapse import SynapseStorage
 from schematic.models.GE_Helpers import GreatExpectationsHelpers
 from schematic.utils.validate_rules_utils import validation_rule_info
 from schematic.utils.validate_utils import rule_in_rule_list
+from schematic.utils.schema_utils import extract_component_validation_rules
 
 logger = logging.getLogger(__name__)
 
+
 class ValidateManifest(object):
     def __init__(self, errors, manifest, manifestPath, dmge, jsonSchema):
         self.errors = errors
         self.manifest = manifest
         self.manifestPath = manifestPath
         self.dmge = dmge
-        self.jsonSchema = jsonSchema       
+        self.jsonSchema = jsonSchema
 
     def get_multiple_types_error(
         self, validation_rules: list, attribute_name: str, error_type: str
     ) -> List[str]:
         """
-            Generate error message for errors when trying to specify 
-            multiple validation rules.
-            """
+        Generate error message for errors when trying to specify
+        multiple validation rules.
+        """
         error_col = attribute_name  # Attribute name
         if error_type == "too_many_rules":
             error_str = (
                 f"For attribute {attribute_name}, the provided validation rules ({validation_rules}) ."
                 f"have too many entries. We currently only specify two rules ('list :: another_rule')."
             )
             logger.error(error_str)
@@ -58,215 +62,263 @@
             )
             logger.error(error_str)
             error_message = error_str
             error_val = f"Multiple Rules: list not first"
         return ["NA", error_col, error_message, error_val]
 
     def validate_manifest_rules(
-        self, manifest: pd.core.frame.DataFrame, dmge: DataModelGraphExplorer, restrict_rules: bool, project_scope: List, access_token: Optional[str] = None,
+        self,
+        manifest: pd.core.frame.DataFrame,
+        dmge: DataModelGraphExplorer,
+        restrict_rules: bool,
+        project_scope: List,
+        access_token: Optional[str] = None,
     ) -> (pd.core.frame.DataFrame, List[List[str]]):
         """
         Purpose:
             Take validation rules set for a particular attribute
             and validate manifest entries based on these rules.
         Input:
             manifest: pd.core.frame.DataFrame
                 imported from models/metadata.py
                 contains metadata input from user for each attribute.
             dmge: DataModelGraphExplorer
                 initialized within models/metadata.py
         Returns:
             manifest: pd.core.frame.DataFrame
-                If a 'list' validatior is run, the manifest needs to be 
+                If a 'list' validatior is run, the manifest needs to be
                 updated to change the attribute column values to a list.
                 In this case the manifest will be updated then exported.
             errors: List[List[str]]
                 If any errors are generated they will be added to an errors
                 list log recording the following information:
                 [error_row, error_col, error_message, error_val]
-        TODO: 
+        TODO:
             -Investigate why a :: delimiter is breaking up the
                 validation rules without me having to do anything...
-            - Move the rules formatting validation to the JSONLD 
+            - Move the rules formatting validation to the JSONLD
                 generation script.
         """
 
         # for each type of rule that can be spefified (key) point
         # to the type of validation that will be run.
 
         validation_types = validation_rule_info()
 
-        type_dict={
+        type_dict = {
             "float64": float,
             "int64": int,
             "str": str,
         }
 
-        unimplemented_expectations=[
+        unimplemented_expectations = [
             "url",
             "list",
             "regex.*",
             "matchAtLeastOne.*",
             "matchExactlyOne.*",
-            ]
+        ]
 
         in_house_rules = [
             "int",
             "float",
             "num",
             "str",
             "regex.*",
             "url",
             "list",
             "matchAtLeastOne.*",
             "matchExactlyOne.*",
         ]
 
         # initialize error and warning handling lists.
-        errors = []   
-        warnings = [] 
+        errors = []
+        warnings = []
 
         if not restrict_rules:
             t_GE = perf_counter()
-            #operations necessary to set up and run ge suite validation
-            ge_helpers=GreatExpectationsHelpers(
+            # operations necessary to set up and run ge suite validation
+            ge_helpers = GreatExpectationsHelpers(
                 dmge=dmge,
                 unimplemented_expectations=unimplemented_expectations,
-                manifest = manifest,
-                manifestPath = self.manifestPath,
-                )
+                manifest=manifest,
+                manifestPath=self.manifestPath,
+            )
 
             ge_helpers.build_context()
             ge_helpers.build_expectation_suite()
             ge_helpers.build_checkpoint()
 
             try:
-                #run GE validation
+                # run GE validation
                 results = ge_helpers.context.run_checkpoint(
                     checkpoint_name=ge_helpers.checkpoint_name,
                     batch_request={
                         "runtime_parameters": {"batch_data": manifest},
-                        "batch_identifiers": {
-                            "default_identifier_name": "manifestID"
-                        },
+                        "batch_identifiers": {"default_identifier_name": "manifestID"},
                     },
-                    result_format={'result_format': 'COMPLETE'},
-                )       
+                    result_format={"result_format": "COMPLETE"},
+                )
             finally:
-                ge_helpers.context.delete_checkpoint(ge_helpers.checkpoint_name) 
-                ge_helpers.context.delete_expectation_suite(ge_helpers.expectation_suite_name)
-        
-            validation_results = results.list_validation_results()            
+                ge_helpers.context.delete_checkpoint(ge_helpers.checkpoint_name)
+                ge_helpers.context.delete_expectation_suite(
+                    ge_helpers.expectation_suite_name
+                )
 
-            #parse validation results dict and generate errors
+            validation_results = results.list_validation_results()
+
+            # parse validation results dict and generate errors
             errors, warnings = ge_helpers.generate_errors(
-                errors = errors,
-                warnings = warnings,
-                validation_results = validation_results,
-                validation_types = validation_types,
-                dmge = dmge,
-                )        
-            logger.debug(f"GE elapsed time {perf_counter()-t_GE}")       
-        else:             
-            logger.info("Great Expetations suite will not be utilized.")  
+                errors=errors,
+                warnings=warnings,
+                validation_results=validation_results,
+                validation_types=validation_types,
+                dmge=dmge,
+            )
+            logger.debug(f"GE elapsed time {perf_counter()-t_GE}")
+        else:
+            logger.info("Great Expetations suite will not be utilized.")
 
-        t_err=perf_counter()
-        regex_re=re.compile('regex.*')
+        t_err = perf_counter()
+        regex_re = re.compile("regex.*")
         for col in manifest.columns:
-            
             # remove trailing/leading whitespaces from manifest
-            manifest.applymap(lambda x: x.strip() if isinstance(x, str) else x)
+            manifest.map(lambda x: x.strip() if isinstance(x, str) else x)
             validation_rules = dmge.get_node_validation_rules(node_display_name=col)
 
-            #TODO: Can remove when handling updated so split within graph
-            if validation_rules and '::' in validation_rules[0]:
-                validation_rules = validation_rules[0].split("::")
+            # Parse the validation rules
+            if validation_rules and isinstance(validation_rules, dict):
+                validation_rules = extract_component_validation_rules(
+                    manifest_component=manifest["Component"][0],
+                    validation_rules=validation_rules,
+                )
 
             # Check that attribute rules conform to limits:
-            # no more than two rules for an attribute. 
+            # no more than two rules for an attribute.
             # As more combinations get added, may want to bring out into its own function / or use validate_rules_utils?
             if len(validation_rules) > 2:
                 errors.append(
                     self.get_multiple_types_error(
                         validation_rules, col, error_type="too_many_rules"
                     )
                 )
 
             # Given a validation rule, run validation. Skip validations already performed by GE
             for rule in validation_rules:
                 validation_type = rule.split(" ")[0]
-                if rule_in_rule_list(rule,unimplemented_expectations) or (rule_in_rule_list(rule,in_house_rules) and restrict_rules):
-                    if not rule_in_rule_list(rule,in_house_rules):
-                        logger.warning(f"Validation rule {rule.split(' ')[0]} has not been implemented in house and cannnot be validated without Great Expectations.")
-                        continue  
+                if rule_in_rule_list(rule, unimplemented_expectations) or (
+                    rule_in_rule_list(rule, in_house_rules) and restrict_rules
+                ):
+                    if not rule_in_rule_list(rule, in_house_rules):
+                        logger.warning(
+                            f"Validation rule {rule.split(' ')[0]} has not been implemented in house and cannnot be validated without Great Expectations."
+                        )
+                        continue
 
-                    t_indiv_rule=perf_counter()
-                    #Validate for each individual validation rule.
+                    t_indiv_rule = perf_counter()
+                    # Validate for each individual validation rule.
                     validation_method = getattr(
-                            ValidateAttribute, validation_types[validation_type]['type']
-                        )
+                        ValidateAttribute, validation_types[validation_type]["type"]
+                    )
 
                     if validation_type == "list":
                         vr_errors, vr_warnings, manifest_col = validation_method(
-                            self, rule, manifest[col], dmge,
+                            self,
+                            rule,
+                            manifest[col],
+                            dmge,
                         )
                         manifest[col] = manifest_col
                     elif validation_type.lower().startswith("match"):
                         vr_errors, vr_warnings = validation_method(
                             self, rule, manifest[col], project_scope, dmge, access_token
                         )
                     else:
                         vr_errors, vr_warnings = validation_method(
-                            self, rule, manifest[col], dmge,
+                            self,
+                            rule,
+                            manifest[col],
+                            dmge,
                         )
                     # Check for validation rule errors and add them to other errors.
                     if vr_errors:
                         errors.extend(vr_errors)
                     if vr_warnings:
                         warnings.extend(vr_warnings)
-                    logger.debug(f"Rule {rule} elapsed time: {perf_counter()-t_indiv_rule}")
+                    logger.debug(
+                        f"Rule {rule} elapsed time: {perf_counter()-t_indiv_rule}"
+                    )
         logger.debug(f"In House validation elapsed time {perf_counter()-t_err}")
         return manifest, errors, warnings
 
-    def validate_manifest_values(self, manifest, jsonSchema, dmge,
+    def validate_manifest_values(
+        self,
+        manifest,
+        jsonSchema,
+        dmge,
     ) -> (List[List[str]], List[List[str]]):
         t_json_schema = perf_counter()
 
         errors = []
         warnings = []
-        col_attr = {} # save the mapping between column index and attribute name
-        
+        col_attr = {}  # save the mapping between column index and attribute name
+
         # numerical values need to be type string for the jsonValidator
-        for col in manifest.select_dtypes(include=[int, np.int64, float, np.float64]).columns:
-            manifest[col]=manifest[col].astype('string')
-        manifest = manifest.applymap(lambda x: str(x) if isinstance(x, (int, np.int64, float, np.float64)) else x, na_action='ignore')
+        for col in manifest.select_dtypes(
+            include=[int, np.int64, float, np.float64]
+        ).columns:
+            manifest[col] = manifest[col].astype("string")
+        manifest = manifest.map(
+            lambda x: str(x) if isinstance(x, Number) else x, na_action="ignore"
+        )
 
         annotations = json.loads(manifest.to_json(orient="records"))
         for i, annotation in enumerate(annotations):
             v = Draft7Validator(jsonSchema)
             for error in sorted(v.iter_errors(annotation), key=exceptions.relevance):
                 errorRow = str(i + 2)
                 errorCol = error.path[-1] if len(error.path) > 0 else "Wrong schema"
                 errorColName = error.path[0] if len(error.path) > 0 else "Wrong schema"
                 errorMsg = error.message[0:500]
                 errorVal = error.instance if len(error.path) > 0 else "Wrong schema"
 
-                val_errors, val_warnings =  GenerateError.generate_schema_error(row_num = errorRow, attribute_name = errorColName, error_msg = errorMsg, invalid_entry = errorVal, dmge = dmge)
+                val_errors, val_warnings = GenerateError.generate_schema_error(
+                    row_num=errorRow,
+                    attribute_name=errorColName,
+                    error_msg=errorMsg,
+                    invalid_entry=errorVal,
+                    dmge=dmge,
+                )
 
                 if val_errors:
                     errors.append(val_errors)
                 if val_warnings:
                     warnings.append(val_warnings)
-        logger.debug(f"JSON Schema validation elapsed time {perf_counter()-t_json_schema}")
+        logger.debug(
+            f"JSON Schema validation elapsed time {perf_counter()-t_json_schema}"
+        )
         return errors, warnings
 
 
-def validate_all(self, errors, warnings, manifest, manifestPath, dmge, jsonSchema, restrict_rules, project_scope: List, access_token: str):
+def validate_all(
+    self,
+    errors,
+    warnings,
+    manifest,
+    manifestPath,
+    dmge,
+    jsonSchema,
+    restrict_rules,
+    project_scope: List,
+    access_token: str,
+):
     vm = ValidateManifest(errors, manifest, manifestPath, dmge, jsonSchema)
-    manifest, vmr_errors, vmr_warnings = vm.validate_manifest_rules(manifest, dmge, restrict_rules, project_scope, access_token)
+    manifest, vmr_errors, vmr_warnings = vm.validate_manifest_rules(
+        manifest, dmge, restrict_rules, project_scope, access_token
+    )
     if vmr_errors:
         errors.extend(vmr_errors)
     if vmr_warnings:
         warnings.extend(vmr_warnings)
 
     vmv_errors, vmv_warnings = vm.validate_manifest_values(manifest, jsonSchema, dmge)
     if vmv_errors:
```

### Comparing `schematicpy-24.1.1/schematic/schemas/commands.py` & `schematicpy-24.2.1/schematic/schemas/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,20 +38,27 @@
     short_help=query_dict(schema_commands, ("schema", "convert", "short_help")),
 )
 @click_log.simple_verbosity_option(logger)
 @click.argument(
     "schema", type=click.Path(exists=True), metavar="<DATA_MODEL_CSV>", nargs=1
 )
 @click.option(
+    "--data_model_labels",
+    "-dml",
+    default="class_label",
+    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    help=query_dict(schema_commands, ("schema", "convert", "data_model_labels")),
+)
+@click.option(
     "--output_jsonld",
     "-o",
     metavar="<OUTPUT_PATH>",
     help=query_dict(schema_commands, ("schema", "convert", "output_jsonld")),
 )
-def convert(schema, output_jsonld):
+def convert(schema, data_model_labels, output_jsonld):
     """
     Running CLI to convert data model specification in CSV format to
     data model in JSON-LD format.
 
     Note: Currently, not configured to build off of base model, so removing --base_schema argument for now
     """
 
@@ -63,15 +70,15 @@
 
     # Parse Model
     logger.info("Parsing data model.")
     parsed_data_model = data_model_parser.parse_model()
 
     # Convert parsed model to graph
     # Instantiate DataModelGraph
-    data_model_grapher = DataModelGraph(parsed_data_model)
+    data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
     # Generate graph
     logger.info("Generating data model graph.")
     graph_data_model = data_model_grapher.generate_data_model_graph()
 
     # Validate generated data model.
     logger.info("Validating the data model internally.")
@@ -97,15 +104,15 @@
                     logger.warning(w)
 
     logger.info("Converting data model to JSON-LD")
     jsonld_data_model = convert_graph_to_jsonld(Graph=graph_data_model)
 
     # output JSON-LD file alongside CSV file by default, get path.
     if output_jsonld is None:
-        if not '.jsonld' in schema:
+        if not ".jsonld" in schema:
             csv_no_ext = re.sub("[.]csv$", "", schema)
             output_jsonld = csv_no_ext + ".jsonld"
         else:
             output_jsonld = schema
 
         logger.info(
             "By default, the JSON-LD output will be stored alongside the first "
```

### Comparing `schematicpy-24.1.1/schematic/schemas/curie.py` & `schematicpy-24.2.1/schematic/schemas/curie.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/schemas/data_model_edges.py` & `schematicpy-24.2.1/schematic/schemas/data_model_edges.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def generate_edge(
         self,
         node: str,
         all_node_dict: dict,
         attr_rel_dict: dict,
         edge_relationships: dict,
-        edge_list:list,
+        edge_list: list,
     ) -> list[tuple[str, str, dict[str:str, str:int]]]:
         """Generate an edge between a target node and relevant other nodes the data model. In short, does this current node belong to a recorded relationship in the attribute, relationshps dictionary. Go through each attribute and relationship to find where the node may be.
         Args:
             G, nx.MultiDiGraph: networkx graph representation of the data model, that is in the process of being fully built. At this point, all the nodes would have been added, and edges are being added per target node.
             node, str: target node to look for connecting edges
             all_node_dict, dict: a dictionary containing information about all nodes in the model
                 key: node display name
@@ -63,29 +63,35 @@
                             # For single (non list) entries, add weight of 0
                             weight = 0
                         # Get the edge_key for the edge relationship we are adding at this step
                         edge_key = self.data_model_relationships[rel_key]["edge_key"]
                         # Add edges, in a manner that preserves directionality
                         # TODO: rewrite to use edge_dir
                         if rel_key in ["subClassOf", "domainIncludes"]:
-                            edge_list.append((
-                                all_node_dict[node]["label"],
-                                all_node_dict[attribute_display_name]["label"],
-                                {'key':edge_key,
-                                'weight':weight,})
+                            edge_list.append(
+                                (
+                                    all_node_dict[node]["label"],
+                                    all_node_dict[attribute_display_name]["label"],
+                                    {
+                                        "key": edge_key,
+                                        "weight": weight,
+                                    },
                                 )
+                            )
                         else:
-                            edge_list.append((
-                                all_node_dict[attribute_display_name]["label"],
-                                all_node_dict[node]["label"],
-                                {'key':edge_key,
-                                'weight':weight},)
+                            edge_list.append(
+                                (
+                                    all_node_dict[attribute_display_name]["label"],
+                                    all_node_dict[node]["label"],
+                                    {"key": edge_key, "weight": weight},
                                 )
+                            )
                         # Add add rangeIncludes/valid value relationships in reverse as well, making the attribute the parent of the valid value.
                         if rel_key == "rangeIncludes":
-                            edge_list.append((
-                                all_node_dict[attribute_display_name]["label"],
-                                all_node_dict[node]["label"],
-                                {'key':"parentOf",
-                                'weight':weight},)
+                            edge_list.append(
+                                (
+                                    all_node_dict[attribute_display_name]["label"],
+                                    all_node_dict[node]["label"],
+                                    {"key": "parentOf", "weight": weight},
                                 )
+                            )
         return edge_list
```

### Comparing `schematicpy-24.1.1/schematic/schemas/data_model_graph.py` & `schematicpy-24.2.1/schematic/schemas/data_model_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from schematic.schemas.data_model_edges import DataModelEdges
 from schematic.schemas.data_model_nodes import DataModelNodes
 from schematic.schemas.data_model_relationships import DataModelRelationships
 
 from schematic.utils.schema_utils import (
     get_property_label_from_display_name,
     get_class_label_from_display_name,
+    DisplayLabelType,
 )
 from schematic.utils.general import unlist
 from schematic.utils.viz_utils import visualize
 
 logger = logging.getLogger(__name__)
 
 
@@ -39,28 +40,35 @@
     from the data model parser.
 
     Create a singleton.
     """
 
     __metaclass__ = DataModelGraphMeta
 
-    def __init__(self, attribute_relationships_dict: dict) -> None:
+    def __init__(
+        self,
+        attribute_relationships_dict: dict,
+        data_model_labels: DisplayLabelType = "class_label",
+    ) -> None:
         """Load parsed data model.
         Args:
             attributes_relationship_dict, dict: generated in data_model_parser
                 {Attribute Display Name: {
                         Relationships: {
                                     CSV Header: Value}}}
-        Raises:
+            data_model_labels: str, display_label or class_label.
+                display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to schema_label.
+                class_label, default, use standard class or property label.         Raises:
             ValueError, attribute_relationship_dict not loaded.
         """
         self.attribute_relationships_dict = attribute_relationships_dict
         self.dmn = DataModelNodes(self.attribute_relationships_dict)
         self.dme = DataModelEdges()
         self.dmr = DataModelRelationships()
+        self.data_model_labels = data_model_labels
 
         if not self.attribute_relationships_dict:
             raise ValueError(
                 "Something has gone wrong, a data model was not loaded into the DataModelGraph Class. Please check that your paths are correct"
             )
         self.graph = self.generate_data_model_graph()
 
@@ -82,15 +90,17 @@
 
         all_node_dict = {}
 
         ## Fill in MultiDigraph with nodes
         for node in all_nodes:
             # Gather information for each node
             node_dict = self.dmn.generate_node_dict(
-                node, self.attribute_relationships_dict
+                node_display_name=node,
+                attr_rel_dict=self.attribute_relationships_dict,
+                data_model_labels=self.data_model_labels,
             )
 
             # Add each node to the all_node_dict to be used for generating edges
             all_node_dict[node] = node_dict
 
             # Generate node and attach information (attributes) to each node
             G = self.dmn.generate_node(G, node_dict)
@@ -106,15 +116,15 @@
                 edge_relationships,
                 edge_list,
             )
             edge_list = edge_list_2.copy()
 
         # Add edges to the Graph
         for node_1, node_2, edge_dict in edge_list:
-            G.add_edge(node_1, node_2, key=edge_dict['key'], weight=edge_dict['weight'])
+            G.add_edge(node_1, node_2, key=edge_dict["key"], weight=edge_dict["weight"])
         return G
 
 
 class DataModelGraphExplorer:
     def __init__(
         self,
         G,
@@ -360,15 +370,15 @@
         # Check if node is in the graph, if not throw an error.
         if not self.is_class_in_schema(node_label=source_node_label):
             raise KeyError(
                 f"Cannot find node: {source_node_label} in the graph, please check entry."
             )
 
         edge_key = self.rel_dict[key]["edge_key"]
-        
+
         # Handle out edges
         if self.rel_dict[key]["jsonld_direction"] == "out":
             # use outedges
 
             original_edge_weights_dict = {
                 attached_node: self.graph[source_node][attached_node][edge_key][
                     "weight"
```

### Comparing `schematicpy-24.1.1/schematic/schemas/data_model_json_schema.py` & `schematicpy-24.2.1/schematic/schemas/data_model_json_schema.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/schemas/data_model_jsonld.py` & `schematicpy-24.2.1/schematic/schemas/data_model_jsonld.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,24 +131,24 @@
             node_edges, list: List of Tuples of edges associated with the given node, tuple contains the two nodes, plus the weight dict associated with the edge connection.
         """
         node_edges = list(self.graph.in_edges(node, data=True))
         node_edges.extend(list(self.graph.out_edges(node, data=True)))
         return node_edges
 
     def get_edges_associated_with_property_nodes(
-        self, node:str
+        self, node: str
     ) -> List[tuple[str, str, dict[str, int]]]:
         """Get edges associated with property nodes to make sure we add that relationship.
         Args:
             node, str: Label of node property in the graph to look for assiciated edges
         Returns:
             node_edges, list: List of Tuples of edges associated with the given node, tuple contains the two nodes, plus the weight dict associated with the edge connection.
         """
         # Get edge keys for domainIncludes and subclassOf
-        domainIncludes_edge_key = self.rel_dict['domainIncludes']['edge_key']        
+        domainIncludes_edge_key = self.rel_dict["domainIncludes"]["edge_key"]
         node_edges = []
         # Get dict of edges for the current property node
         node_edges_dict = self.graph[node]
         for node_2, edge_dict in node_edges_dict.items():
             # Look through relationships in the edge dictionary
             for edge_key in edge_dict:
                 # If the edge is a property or subclass then add the edges to the list
@@ -163,18 +163,19 @@
             rel_vals, dict: sub relationship dict for a given relationship (contains informtion like, 'edge_rel', 'jsonld_key' etc..)
             node, str: node whose edge information is presently being added to the JSONLD
         Returns:
         """
         # Get all edges associated with the current node
         node_edges = self.get_edges_associated_with_node(node=node)
 
-
         # For properties look for reverse relationships too
         if node in self.dmge.find_properties():
-            property_node_edges = self.get_edges_associated_with_property_nodes(node=node)
+            property_node_edges = self.get_edges_associated_with_property_nodes(
+                node=node
+            )
             node_edges.extend(property_node_edges)
 
         # Get node pairs and weights for each edge
         for node_1, node_2, weight in node_edges:
             # Retrieve the relationship(s) and related info between the two nodes
             node_edge_relationships = self.graph[node_1][node_2]
 
@@ -184,16 +185,18 @@
             # Check if edge_key is even one of the relationships for this node pair.
             if edge_key in node_edge_relationships:
                 # for each relationship between the given nodes
                 for relationship, weight_dict in node_edge_relationships.items():
                     # If the relationship defined and edge_key
                     if relationship == edge_key:
                         # TODO: rewrite to use edge_dir
-                        domainIncludes_edge_key = self.rel_dict['domainIncludes']['edge_key']
-                        subclassOf_edge_key = self.rel_dict['subClassOf']['edge_key']
+                        domainIncludes_edge_key = self.rel_dict["domainIncludes"][
+                            "edge_key"
+                        ]
+                        subclassOf_edge_key = self.rel_dict["subClassOf"]["edge_key"]
                         if edge_key in [subclassOf_edge_key]:
                             if node_2 == node:
                                 # Make sure the key is in the template (differs between properties and classes)
                                 if rel_vals["jsonld_key"] in template.keys():
                                     node_1_id = {"@id": "bts:" + node_1}
                                     # TODO Move this to a helper function to clear up.
                                     if (
@@ -299,14 +302,15 @@
             data_model_relationships=data_model_relationships,
         )
 
         # Reorder lists based on weights:
         template = self.reorder_template_entries(
             template=template,
         )
+
         # Add contexts to certain values
         template = self.add_contexts_to_entries(
             template=template,
         )
 
         return template
 
@@ -410,15 +414,17 @@
                 ][0]
 
                 # Order edges
                 sorted_edges = self.dmge.get_ordered_entry(
                     key=key, source_node_label=template_label
                 )
                 if not len(entry) == len(sorted_edges):
-                    logger.error("There is an error with sorting values in the JSONLD, please issue a bug report.")
+                    logger.error(
+                        "There is an error with sorting values in the JSONLD, please issue a bug report."
+                    )
 
                 edge_weights_dict = {edge: i for i, edge in enumerate(sorted_edges)}
                 ordered_edges = [0] * len(edge_weights_dict.keys())
                 for edge, normalized_weight in edge_weights_dict.items():
                     ordered_edges[normalized_weight] = {"@id": "bts:" + edge}
 
                 # Throw an error if ordered_edges does not get fully filled as expected.
```

### Comparing `schematicpy-24.1.1/schematic/schemas/data_model_nodes.py` & `schematicpy-24.2.1/schematic/schemas/data_model_nodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from inspect import isfunction
 import networkx as nx
 from rdflib import Namespace
-from typing import Any, Dict, Optional, Text, List, Callable
+from typing import Any, Dict, Optional, Text, List, Literal, Callable
 
 from schematic.schemas.data_model_parser import DataModelJSONLDParser
 from schematic.schemas.data_model_relationships import DataModelRelationships
 
 from schematic.utils.schema_utils import (
     get_label_from_display_name,
     get_attribute_display_name_from_label,
     convert_bool_to_str,
     parse_validation_rules,
+    DisplayLabelType,
 )
 from schematic.utils.validate_rules_utils import validate_schema_rules
 from schematic.schemas.curie import uri2curie, curie2uri
 
 
 class DataModelNodes:
     def __init__(self, attribute_relationships_dict):
@@ -126,14 +127,15 @@
         self,
         rel_func: callable,
         node_display_name: str = "",
         key: str = "",
         attr_relationships={},
         csv_header="",
         entry_type="",
+        data_model_labels: DisplayLabelType = "class_label",
     ):
         """This function exists to centralzie handling of functions for filling out node information, makes sure all the proper parameters are passed to each function.
         Args:
             rel_func, callable: Function to call to get information to attach to the node
             node_display_name, str: node display name
             key, str: relationship key
             attr_relationships, dict: relationships portion of attributes_relationships dictionary
@@ -153,15 +155,17 @@
             )
 
         elif rel_func == parse_validation_rules:
             return parse_validation_rules(attr_relationships[csv_header])
 
         elif rel_func == get_label_from_display_name:
             return get_label_from_display_name(
-                display_name=node_display_name, entry_type=entry_type
+                display_name=node_display_name,
+                entry_type=entry_type,
+                data_model_labels=data_model_labels,
             )
 
         elif rel_func == convert_bool_to_str:
             if type(attr_relationships[csv_header]) == str:
                 if attr_relationships[csv_header].lower() == "true":
                     return True
                 elif attr_relationships[csv_header].lower() == "false":
@@ -172,23 +176,30 @@
 
         else:
             # Raise Error if the rel_func provided is not captured.
             raise ValueError(
                 f"The function provided ({rel_func}) to define the relationship {key} is not captured in the function run_rel_functions, please update."
             )
 
-    def generate_node_dict(self, node_display_name: str, attr_rel_dict: dict) -> dict:
+    def generate_node_dict(
+        self,
+        node_display_name: str,
+        attr_rel_dict: dict,
+        data_model_labels: DisplayLabelType = "class_label",
+    ) -> dict:
         """Gather information to be attached to each node.
         Args:
             node_display_name, str: display name for current node
             attr_rel_dict, dict: generated in data_model_parser
                 {Attribute Display Name: {
                         Relationships: {
                                     CSV Header: Value}}}
-
+            data_model_labels: str, display_label or class_label.
+                display_label, use the display name as a label, if it is valid (contains no blacklisted characters) otherwise will default to schema_label.
+                class_label, default, use standard class or property label.
         Returns:
             node_dict, dict: dictionary of relationship information about the current node
                 {'displayName': '', 'label': '', 'comment': 'TBD', 'required': None, 'validationRules': [], 'isPartOf': '', 'uri': ''}
         Note:
             If the default calls function, call that function for the default or alternate implementation.
             May need to update this logic for varying function calls. (for example the current function takes in the node display name
             would need to update if new function took in something else.)
@@ -224,14 +235,15 @@
                             rel_key: self.run_rel_functions(
                                 rel_node_dict["standard"],
                                 node_display_name=node_display_name,
                                 key=key,
                                 attr_relationships=attr_relationships,
                                 csv_header=csv_header,
                                 entry_type=entry_type,
+                                data_model_labels=data_model_labels,
                             )
                         }
                     )
                 else:
                     # For standard entries, get information from attr_relationship dictionary
                     node_dict.update({rel_key: attr_relationships[csv_header]})
             # else, add default values
@@ -245,14 +257,15 @@
                             rel_key: self.run_rel_functions(
                                 rel_node_dict["default"],
                                 node_display_name=node_display_name,
                                 key=key,
                                 attr_relationships=attr_relationships,
                                 csv_header=csv_header,
                                 entry_type=entry_type,
+                                data_model_labels=data_model_labels,
                             )
                         }
                     )
                 else:
                     # Set value to defaults.
                     node_dict.update({rel_key: rel_node_dict["default"]})
```

### Comparing `schematicpy-24.1.1/schematic/schemas/data_model_parser.py` & `schematicpy-24.2.1/schematic/schemas/data_model_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import pandas as pd
 import pathlib
+
 from typing import Any, Dict, Optional, Text, List, Union
 
 from schematic.utils.df_utils import load_df
 from schematic.utils.io_utils import load_json
 from schematic.utils.schema_utils import attr_dict_template
 
 from schematic.schemas.data_model_relationships import DataModelRelationships
@@ -239,76 +240,91 @@
         self,
     ):
         # Instantiate DataModelRelationships
         self.dmr = DataModelRelationships()
         # Load relationships dictionary.
         self.rel_dict = self.dmr.define_data_model_relationships()
 
-    def parse_entry(self, rel_entry: any, id_jsonld_key: str, dn_label_dict:dict[str:str], model_jsonld:dict) -> Any:
+    def parse_entry(
+        self,
+        rel_entry: any,
+        id_jsonld_key: str,
+        dn_label_dict: dict[str:str],
+        model_jsonld: dict,
+    ) -> Any:
         """Parse an input entry based on certain attributes
         Args:
             rel_entry: Given a single entry and relationship in a JSONLD data model, the recorded value
             id_jsonld_key, str: the jsonld key for id
         Returns:
             parsed_rel_entry: an entry that has been parsed base on its input type and characteristics.
         """
         # Retrieve ID from single value dictionary
         if type(rel_entry) == dict and len(rel_entry.keys()) == 1:
             parsed_rel_entry = rel_entry["@id"]
         # Parse list of dictionaries to make a list of entries with context stripped (will update this section when contexts added.)
         elif type(rel_entry) == list and type(rel_entry[0]) == dict:
-            parsed_rel_entry = self.convert_entry_to_dn_label([r[id_jsonld_key].split(":")[1] for r in rel_entry], model_jsonld)
+            parsed_rel_entry = self.convert_entry_to_dn_label(
+                [r[id_jsonld_key].split(":")[1] for r in rel_entry], model_jsonld
+            )
         # Strip context from string and convert true/false to bool
         elif type(rel_entry) == str:
             # Remove contexts and treat strings as appropriate.
             if ":" in rel_entry and "http:" not in rel_entry:
                 parsed_rel_entry = rel_entry.split(":")[1]
                 # Convert true/false strings to boolean
                 if parsed_rel_entry.lower() == "true":
                     parsed_rel_entry = True
                 elif parsed_rel_entry.lower == "false":
                     parsed_rel_entry = False
             else:
-                parsed_rel_entry=self.convert_entry_to_dn_label(rel_entry, model_jsonld)
+                parsed_rel_entry = self.convert_entry_to_dn_label(
+                    rel_entry, model_jsonld
+                )
 
         # For anything else get that
         else:
-            parsed_rel_entry=self.convert_entry_to_dn_label(rel_entry, model_jsonld)
+            parsed_rel_entry = self.convert_entry_to_dn_label(rel_entry, model_jsonld)
 
         return parsed_rel_entry
 
     def label_to_dn_dict(self, model_jsonld: list[dict]):
-        """ Generate a dictionary of labels to display name, so can easily look up display names using the label.
+        """Generate a dictionary of labels to display name, so can easily look up display names using the label.
         Args:
             model_jsonld: list of dictionaries, each dictionary is an entry in the jsonld data model
         Returns:
             dn_label_dict: dict of model labels to display names
         """
         jsonld_keys_to_extract = ["label", "displayName"]
         label_jsonld_key, dn_jsonld_key = [
             self.rel_dict[key]["jsonld_key"] for key in jsonld_keys_to_extract
         ]
         dn_label_dict = {}
         for entry in model_jsonld:
-            dn_label_dict[entry[label_jsonld_key]]=entry[dn_jsonld_key]
+            dn_label_dict[entry[label_jsonld_key]] = entry[dn_jsonld_key]
         return dn_label_dict
 
-    def convert_entry_to_dn_label(self, parsed_rel_entry:Union[str,list], model_jsonld:list[dict]) -> Union[str,list]:
+    def convert_entry_to_dn_label(
+        self, parsed_rel_entry: Union[str, list], model_jsonld: list[dict]
+    ) -> Union[str, list]:
         """Convert a parsed entry to display name, taking into account the entry type
         Args:
             parsed_rel_entry: an entry that has been parsed base on its input type and characteristics.
             model_jsonld: list of dictionaries, each dictionary is an entry in the jsonld data model
         Returns:
             parsed_rel_entry: an entry that has been parsed based on its input type and characteristics, and converted to display names.
         """
         # Get a dictionary of display_names mapped to labels
         dn_label_dict = self.label_to_dn_dict(model_jsonld=model_jsonld)
         # Handle if using the display name as the label
         if type(parsed_rel_entry) == list:
-            parsed_rel_entry = [dn_label_dict.get(entry) if dn_label_dict.get(entry) else entry for entry in parsed_rel_entry ]
+            parsed_rel_entry = [
+                dn_label_dict.get(entry) if dn_label_dict.get(entry) else entry
+                for entry in parsed_rel_entry
+            ]
         elif type(parsed_rel_entry) == str:
             converted_label = dn_label_dict.get(parsed_rel_entry)
             if converted_label:
                 parsed_rel_entry = dn_label_dict.get(parsed_rel_entry)
         return parsed_rel_entry
 
     def gather_jsonld_attributes_relationships(self, model_jsonld: List[dict]) -> Dict:
@@ -358,68 +374,90 @@
                 attr_rel_dictionary.update(attr_dict_template(attr_key))
 
             # Add relationships for each entry
             # Go through each defined relationship type (rel_key) and its attributes (rel_vals)
             for rel_key, rel_vals in self.rel_dict.items():
                 # Determine if current entry in the for loop, can be described by the current relationship that is being cycled through.
                 # used to also check "csv_header" in rel_vals.keys() which allows all JSONLD values through even if it does not have a CSV counterpart, will allow other values thorough in the else statement now
-                if (
-                    rel_vals["jsonld_key"] in entry.keys()
-                    and rel_vals["csv_header"]
-                ):
+                if rel_vals["jsonld_key"] in entry.keys() and rel_vals["csv_header"]:
                     # Retrieve entry value associated with the given relationship
                     rel_entry = entry[rel_vals["jsonld_key"]]
                     # If there is an entry parse it by type and add to the attr:relationships dictionary.
                     if rel_entry:
                         parsed_rel_entry = self.parse_entry(
-                            rel_entry=rel_entry, id_jsonld_key=id_jsonld_key, dn_label_dict=dn_label_dict, model_jsonld=model_jsonld,
+                            rel_entry=rel_entry,
+                            id_jsonld_key=id_jsonld_key,
+                            dn_label_dict=dn_label_dict,
+                            model_jsonld=model_jsonld,
                         )
                         rel_csv_header = self.rel_dict[rel_key]["csv_header"]
-                        if rel_key == 'domainIncludes':
+                        if rel_key == "domainIncludes":
                             # In the JSONLD the domain includes field contains the ids of attributes that the current attribute is the property/parent of.
                             # Because of this we need to handle these values differently.
                             # We will get the values in the field (parsed_val), then add the current attribute as to the property key in the attr_rel_dictionary[p_attr_key].
                             for parsed_val in parsed_rel_entry:
                                 attr_in_dict = False
-                                #Get propert/parent key (displayName)
-                                p_attr_key=''
+                                # Get propert/parent key (displayName)
+                                p_attr_key = ""
                                 # Check if the parsed value is already a part of the attr_rel_dictionary
                                 for attr_dn, rels in attr_rel_dictionary.items():
                                     if parsed_val == attr_dn:
                                         p_attr_key = attr_dn
                                         attr_in_dict = True
                                 # If it is part of the dictionary update add current attribute as a property of the parsed value
                                 if attr_in_dict == True:
-                                    if not rel_csv_header in attr_rel_dictionary[p_attr_key]["Relationships"]:
-                                        attr_rel_dictionary[p_attr_key]["Relationships"].update({rel_csv_header:[entry[dn_jsonld_key]]})
+                                    if (
+                                        not rel_csv_header
+                                        in attr_rel_dictionary[p_attr_key][
+                                            "Relationships"
+                                        ]
+                                    ):
+                                        attr_rel_dictionary[p_attr_key][
+                                            "Relationships"
+                                        ].update(
+                                            {rel_csv_header: [entry[dn_jsonld_key]]}
+                                        )
                                     else:
-                                        attr_rel_dictionary[p_attr_key]["Relationships"].update({rel_csv_header:[entry[dn_jsonld_key]]})
+                                        attr_rel_dictionary[p_attr_key][
+                                            "Relationships"
+                                        ][rel_csv_header].extend([entry[dn_jsonld_key]])
                                 # If the parsed_val is not already recorded in the dictionary, add it
                                 elif attr_in_dict == False:
                                     # Get the display name for the parsed value
-                                    p_attr_key = self.convert_entry_to_dn_label(parsed_val, model_jsonld)
-                                    
-                                    attr_rel_dictionary.update(attr_dict_template(p_attr_key))
-                                    attr_rel_dictionary[p_attr_key]["Relationships"].update({rel_csv_header:[entry[label_jsonld_key]]})
-                        
+                                    p_attr_key = self.convert_entry_to_dn_label(
+                                        parsed_val, model_jsonld
+                                    )
+
+                                    attr_rel_dictionary.update(
+                                        attr_dict_template(p_attr_key)
+                                    )
+                                    attr_rel_dictionary[p_attr_key][
+                                        "Relationships"
+                                    ].update(
+                                        {rel_csv_header: [entry[label_jsonld_key]]}
+                                    )
+
                         else:
                             attr_rel_dictionary[attr_key]["Relationships"].update(
                                 {rel_csv_header: parsed_rel_entry}
                             )
-                        
+
                 elif (
                     rel_vals["jsonld_key"] in entry.keys()
                     and not rel_vals["csv_header"]
                 ):
                     # Retrieve entry value associated with the given relationship
                     rel_entry = entry[rel_vals["jsonld_key"]]
                     # If there is an entry parset it by type and add to the attr:relationships dictionary.
                     if rel_entry:
                         parsed_rel_entry = self.parse_entry(
-                            rel_entry=rel_entry, id_jsonld_key=id_jsonld_key, dn_label_dict=dn_label_dict, model_jsonld=model_jsonld,
+                            rel_entry=rel_entry,
+                            id_jsonld_key=id_jsonld_key,
+                            dn_label_dict=dn_label_dict,
+                            model_jsonld=model_jsonld,
                         )
                         # Add relationships for each attribute and relationship to the dictionary
                         attr_rel_dictionary[attr_key]["Relationships"].update(
                             {rel_key: parsed_rel_entry}
                         )
         return attr_rel_dictionary
```

### Comparing `schematicpy-24.1.1/schematic/schemas/data_model_relationships.py` & `schematicpy-24.2.1/schematic/schemas/data_model_relationships.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/schemas/data_model_validator.py` & `schematicpy-24.2.1/schematic/schemas/data_model_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 import multiprocessing
 import networkx as nx
 import time
 from typing import Any, Dict, Optional, Text, List, Tuple
 
 from schematic.schemas.data_model_relationships import DataModelRelationships
+
 logger = logging.getLogger(__name__)
 
+
 class DataModelValidator:
     """
     Check for consistency within data model.
     """
 
     def __init__(
         self,
@@ -83,30 +85,32 @@
     def check_is_dag(self) -> List[str]:
         """Check that generated graph is a directed acyclic graph
         Returns:
                 error, list: List of error messages if graph is not a DAG. List will include a message for each cycle found, if not there is a more generic message for the graph as a whole.
         """
         error = []
         if not nx.is_directed_acyclic_graph(self.graph):
-            cycles = multiprocessing.Process(target=self.run_cycles, name="Get Cycles", args=(self.graph,))
+            cycles = multiprocessing.Process(
+                target=self.run_cycles, name="Get Cycles", args=(self.graph,)
+            )
             cycles.start()
 
             # Give up to 5 seconds to find cycles, if not exit and issue standard error
             time.sleep(5)
 
             # If thread is active
             if cycles.is_alive():
                 # Terminate foo
                 cycles.terminate()
                 # Cleanup
                 cycles.join()
 
             error.append(
                 f"Schematic requires models be a directed acyclic graph (DAG). Please inspect your model."
-                )
+            )
 
         return error
 
     def check_blacklisted_characters(self) -> List[str]:
         """We strip these characters in store, so not sure if it matter if we have them now, maybe add warning
         Returns:
                 warning, list: list of warnings for each node in the graph, that has a Display name that contains blacklisted characters.
```

### Comparing `schematicpy-24.1.1/schematic/schemas/json_schema_validator.py` & `schematicpy-24.2.1/schematic/schemas/json_schema_validator.py`

 * *Files identical despite different names*

### Comparing `schematicpy-24.1.1/schematic/store/synapse.py` & `schematicpy-24.2.1/schematic/store/synapse.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,23 @@
 import os
 import re
 import secrets
 import shutil
 import synapseclient
 import uuid  # used to generate unique names for entities
 
-from tenacity import retry, stop_after_attempt, wait_chain, wait_fixed, retry_if_exception_type
+from tenacity import (
+    retry,
+    stop_after_attempt,
+    wait_chain,
+    wait_fixed,
+    retry_if_exception_type,
+)
 from time import sleep
+
 # allows specifying explicit variable types
 from typing import Dict, List, Tuple, Sequence, Union, Optional
 
 
 from synapseclient import (
     Synapse,
     File,
@@ -30,50 +37,60 @@
     EntityViewType,
     Column,
     as_table_columns,
 )
 from synapseclient.entity import File
 from synapseclient.table import CsvFileTable, build_table, Schema
 from synapseclient.annotations import from_synapse_annotations
-from synapseclient.core.exceptions import SynapseHTTPError, SynapseAuthenticationError, SynapseUnmetAccessRestrictions
+from synapseclient.core.exceptions import (
+    SynapseHTTPError,
+    SynapseAuthenticationError,
+    SynapseUnmetAccessRestrictions,
+)
 import synapseutils
 from synapseutils.copy_functions import changeFileMetaData
 
 import uuid
 
 from schematic_db.rdb.synapse_database import SynapseDatabase
 
 from schematic.schemas.data_model_graph import DataModelGraphExplorer
 
 from schematic.utils.df_utils import update_df, load_df, col_in_dataframe
 from schematic.utils.validate_utils import comma_separated_list_regex, rule_in_rule_list
+
 # entity_type_mapping, get_dir_size, create_temp_folder, check_synapse_cache_size, and clear_synapse_cache functions are used for AWS deployment
 # Please do not remove these import statements
-from schematic.utils.general import (entity_type_mapping,
-                                     get_dir_size,
-                                     convert_gb_to_bytes,
-                                     create_temp_folder,
-                                     check_synapse_cache_size,
-                                     clear_synapse_cache,
-                                     profile,
-                                     calculate_datetime)
+from schematic.utils.general import (
+    entity_type_mapping,
+    get_dir_size,
+    convert_gb_to_bytes,
+    create_temp_folder,
+    check_synapse_cache_size,
+    clear_synapse_cache,
+    profile,
+    calculate_datetime,
+)
+
 from schematic.utils.schema_utils import get_class_label_from_display_name
 
 from schematic.store.base import BaseStorage
 from schematic.exceptions import MissingConfigValueError, AccessCredentialsError
 from schematic.configuration.configuration import CONFIG
 
 logger = logging.getLogger("Synapse storage")
 
+
 @dataclass
 class ManifestDownload(object):
     """
     syn: an object of type synapseclient.
-    manifest_id: id of a manifest  
+    manifest_id: id of a manifest
     """
+
     syn: synapseclient.Synapse
     manifest_id: str
 
     def _download_manifest_to_folder(self) -> File:
         """
         try downloading a manifest to local cache or a given folder
         manifest
@@ -87,84 +104,96 @@
                 shutil.rmtree(temporary_manifest_storage)
             # create a new directory to store manifest
             if not os.path.exists(temporary_manifest_storage):
                 os.mkdir(temporary_manifest_storage)
             # create temporary folders for storing manifests
             download_location = create_temp_folder(temporary_manifest_storage)
         else:
-            download_location=CONFIG.manifest_folder
+            download_location = CONFIG.manifest_folder
         manifest_data = self.syn.get(
-                self.manifest_id,
-                downloadLocation=download_location,
-                ifcollision="overwrite.local",
-            )
+            self.manifest_id,
+            downloadLocation=download_location,
+            ifcollision="overwrite.local",
+        )
         return manifest_data
 
     def _entity_type_checking(self) -> str:
         """
         check the entity type of the id that needs to be downloaded
-        Return: 
+        Return:
              if the entity type is wrong, raise an error
         """
         # check the type of entity
         entity_type = entity_type_mapping(self.syn, self.manifest_id)
-        if entity_type  != "file":
-            logger.error(f'You are using entity type: {entity_type}. Please provide a file ID')
+        if entity_type != "file":
+            logger.error(
+                f"You are using entity type: {entity_type}. Please provide a file ID"
+            )
 
     @staticmethod
-    def download_manifest(self, newManifestName: str="", manifest_df: pd.DataFrame=pd.DataFrame()) -> Union[str,File]:
+    def download_manifest(
+        self, newManifestName: str = "", manifest_df: pd.DataFrame = pd.DataFrame()
+    ) -> Union[str, File]:
         """
-        Download a manifest based on a given manifest id. 
+        Download a manifest based on a given manifest id.
         Args:
             newManifestName(optional): new name of a manifest that gets downloaded.
             manifest_df(optional): a dataframe containing name and id of manifests in a given asset view
-        Return: 
+        Return:
             manifest_data: synapse entity file object
         """
 
         # enables retrying if user does not have access to uncensored manifest
         # pass synID to synapseclient.Synapse.get() method to download (and overwrite) file to a location
         manifest_data = ""
 
         # check entity type
         self._entity_type_checking()
 
         # download a manifest
         try:
             manifest_data = self._download_manifest_to_folder()
-        except(SynapseUnmetAccessRestrictions, SynapseAuthenticationError):
+        except (SynapseUnmetAccessRestrictions, SynapseAuthenticationError):
             # if there's an error getting an uncensored manifest, try getting the censored manifest
             if not manifest_df.empty:
-                censored_regex=re.compile('.*censored.*')
-                censored = manifest_df['name'].str.contains(censored_regex)
-                new_manifest_id=manifest_df[censored]["id"][0]
+                censored_regex = re.compile(".*censored.*")
+                censored = manifest_df["name"].str.contains(censored_regex)
+                new_manifest_id = manifest_df[censored]["id"][0]
                 self.manifest_id = new_manifest_id
-                try: 
+                try:
                     manifest_data = self._download_manifest_to_folder()
-                except (SynapseUnmetAccessRestrictions, SynapseAuthenticationError) as e:
-                    raise PermissionError("You don't have access to censored and uncensored manifests in this dataset.") from e
+                except (
+                    SynapseUnmetAccessRestrictions,
+                    SynapseAuthenticationError,
+                ) as e:
+                    raise PermissionError(
+                        "You don't have access to censored and uncensored manifests in this dataset."
+                    ) from e
             else:
-                logger.error(f"You don't have access to the requested resource: {self.manifest_id}")
+                logger.error(
+                    f"You don't have access to the requested resource: {self.manifest_id}"
+                )
 
-        if newManifestName and os.path.exists(manifest_data.get('path')):
+        if newManifestName and os.path.exists(manifest_data.get("path")):
             # Rename the file we just made to the new name
-            new_manifest_filename = newManifestName + '.csv'
+            new_manifest_filename = newManifestName + ".csv"
 
             # get location of existing manifest. The manifest that will be renamed should live in the same folder as existing manifest.
-            parent_folder = os.path.dirname(manifest_data.get('path'))
+            parent_folder = os.path.dirname(manifest_data.get("path"))
 
             new_manifest_path_name = os.path.join(parent_folder, new_manifest_filename)
-            os.rename(manifest_data['path'], new_manifest_path_name)
+            os.rename(manifest_data["path"], new_manifest_path_name)
 
             # Update file names/paths in manifest_data
-            manifest_data['name'] = new_manifest_filename
-            manifest_data['filename'] = new_manifest_filename
-            manifest_data['path'] = new_manifest_path_name
+            manifest_data["name"] = new_manifest_filename
+            manifest_data["filename"] = new_manifest_filename
+            manifest_data["path"] = new_manifest_path_name
         return manifest_data
 
+
 class SynapseStorage(BaseStorage):
     """Implementation of Storage interface for datasets/files stored on Synapse.
     Provides utilities to list files in a specific project; update files annotations, create fileviews, etc.
 
     TODO: Need to define the interface and rename and/or refactor some of the methods below.
     """
 
@@ -194,49 +223,53 @@
         self.storageFileview = CONFIG.synapse_master_fileview_id
         self.manifest = CONFIG.synapse_manifest_basename
         self.root_synapse_cache = "/root/.synapseCache"
         self._query_fileview()
 
     def _purge_synapse_cache(self, maximum_storage_allowed_cache_gb=1):
         """
-        Purge synapse cache if it exceeds a certain size. Default to 1GB. 
+        Purge synapse cache if it exceeds a certain size. Default to 1GB.
         Args:
-            maximum_storage_allowed_cache_gb: the maximum storage allowed before purging cache. Default is 1 GB. 
+            maximum_storage_allowed_cache_gb: the maximum storage allowed before purging cache. Default is 1 GB.
         """
         # try clearing the cache
         # scan a directory and check size of files
         if os.path.exists(self.root_synapse_cache):
-            maximum_storage_allowed_cache_bytes = convert_gb_to_bytes(maximum_storage_allowed_cache_gb)
+            maximum_storage_allowed_cache_bytes = convert_gb_to_bytes(
+                maximum_storage_allowed_cache_gb
+            )
             nbytes = get_dir_size(self.root_synapse_cache)
             dir_size_bytes = check_synapse_cache_size(directory=self.root_synapse_cache)
             # if 1 GB has already been taken, purge cache before 15 min
             if dir_size_bytes >= maximum_storage_allowed_cache_bytes:
                 num_of_deleted_files = clear_synapse_cache(self.syn.cache, minutes=15)
-                logger.info(f'{num_of_deleted_files}  files have been deleted from {self.root_synapse_cache}')
+                logger.info(
+                    f"{num_of_deleted_files}  files have been deleted from {self.root_synapse_cache}"
+                )
             else:
                 # on AWS, OS takes around 14-17% of our ephemeral storage (20GiB)
                 # instead of guessing how much space that we left, print out .synapseCache here
-                logger.info(f'the total size of .synapseCache is: {nbytes} bytes')
+                logger.info(f"the total size of .synapseCache is: {nbytes} bytes")
 
     def _query_fileview(self):
         self._purge_synapse_cache()
         try:
             self.storageFileview = CONFIG.synapse_master_fileview_id
             self.manifest = CONFIG.synapse_manifest_basename
             if self.project_scope:
                 self.storageFileviewTable = self.syn.tableQuery(
                     f"SELECT * FROM {self.storageFileview} WHERE projectId IN {tuple(self.project_scope + [''])}"
-                    ).asDataFrame()
+                ).asDataFrame()
             else:
                 # get data in administrative fileview for this pipeline
                 self.storageFileviewTable = self.syn.tableQuery(
                     "SELECT * FROM " + self.storageFileview
                 ).asDataFrame()
         except SynapseHTTPError:
-            raise AccessCredentialsError(self.storageFileview)    
+            raise AccessCredentialsError(self.storageFileview)
 
     @staticmethod
     def login(token=None, access_token=None):
         # If no token is provided, try retrieving access token from environment
         if not token and not access_token:
             access_token = os.getenv("SYNAPSE_ACCESS_TOKEN")
 
@@ -249,37 +282,39 @@
             except synapseclient.core.exceptions.SynapseHTTPError:
                 raise ValueError("Please make sure you are logged into synapse.org.")
         elif access_token:
             try:
                 syn = synapseclient.Synapse()
                 syn.default_headers["Authorization"] = f"Bearer {access_token}"
             except synapseclient.core.exceptions.SynapseHTTPError:
-                raise ValueError("No access to resources. Please make sure that your token is correct")
+                raise ValueError(
+                    "No access to resources. Please make sure that your token is correct"
+                )
         else:
             # login using synapse credentials provided by user in .synapseConfig (default) file
             syn = synapseclient.Synapse(configPath=CONFIG.synapse_configuration_path)
             syn.login(silent=True)
         return syn
 
     def missing_entity_handler(method):
         def wrapper(*args, **kwargs):
             try:
                 return method(*args, **kwargs)
-            except(SynapseHTTPError) as ex:
-                str_message = str(ex).replace("\n","")
-                if 'trash' in str_message or 'does not exist' in str_message:
+            except SynapseHTTPError as ex:
+                str_message = str(ex).replace("\n", "")
+                if "trash" in str_message or "does not exist" in str_message:
                     logging.warning(str_message)
                     return None
                 else:
                     raise ex
+
         return wrapper
 
     def getStorageFileviewTable(self):
-        """ Returns the storageFileviewTable obtained during initialization.
-        """
+        """Returns the storageFileviewTable obtained during initialization."""
         return self.storageFileviewTable
 
     def getPaginatedRestResults(self, currentUserId: str) -> Dict[str, str]:
         """Gets the paginated results of the REST call to Synapse to check what projects the current user has access to.
 
         Args:
             currentUserId: synapse id for the user whose projects we want to get.
@@ -333,24 +368,24 @@
         currentUserProjects = [
             currentUserProject.get("id")
             for currentUserProject in currentUserProjects["results"]
         ]
 
         # find set of user projects that are also in this pipeline's storage projects set
         storageProjects = list(set(storageProjects) & set(currentUserProjects))
-        
+
         # Limit projects to scope if specified
         if project_scope:
             storageProjects = list(set(storageProjects) & set(project_scope))
 
             if not storageProjects:
                 raise Warning(
                     f"There are no projects that the user has access to that match the criteria of the specified project scope: {project_scope}"
                 )
-        
+
         # prepare a return list of project IDs and names
         projects = []
         for projectId in storageProjects:
             projectName = self.syn.get(projectId, downloadFile=False).name
             projects.append((projectId, projectName))
 
         sorted_projects_list = sorted(projects, key=lambda tup: tup[0])
@@ -414,200 +449,220 @@
 
         Returns:
             A list of files; the list consists of tuples (fileId, fileName).
 
         Raises:
             ValueError: Dataset ID not found.
         """
-
         # select all files within a given storage dataset folder (top level folder in a Synapse storage project or folder marked with contentType = 'dataset')
-        walked_path = synapseutils.walk(self.syn, datasetId, includeTypes=["folder", "file"])
+        walked_path = synapseutils.walk(
+            self.syn, datasetId, includeTypes=["folder", "file"]
+        )
 
         file_list = []
 
         # iterate over all results
         for dirpath, dirname, filenames in walked_path:
-
             # iterate over all files in a folder
             for filename in filenames:
-
                 if (not "manifest" in filename[0] and not fileNames) or (
                     fileNames and filename[0] in fileNames
                 ):
-
                     # don't add manifest to list of files unless it is specified in the list of specified fileNames; return all found files
                     # except the manifest if no fileNames have been specified
                     # TODO: refactor for clarity/maintainability
 
                     if fullpath:
                         # append directory path to filename
                         filename = (dirpath[0] + "/" + filename[0], filename[1])
 
                     # add file name file id tuple, rearranged so that id is first and name follows
                     file_list.append(filename[::-1])
 
         return file_list
 
     def _get_manifest_id(self, manifest: pd.DataFrame) -> str:
-        """If both censored and uncensored manifests are present, return uncensored manifest; if only one manifest is present, return manifest id of that manifest; if more than two manifests are present, return the manifest id of the first one. 
+        """If both censored and uncensored manifests are present, return uncensored manifest; if only one manifest is present, return manifest id of that manifest; if more than two manifests are present, return the manifest id of the first one.
         Args:
         manifest: a dataframe contains name and id of manifests in a given asset view
 
-        Return: 
+        Return:
         manifest_syn_id: id of a given censored or uncensored manifest
-        """ 
-        censored_regex=re.compile('.*censored.*')
-        censored = manifest['name'].str.contains(censored_regex)
+        """
+        censored_regex = re.compile(".*censored.*")
+        censored = manifest["name"].str.contains(censored_regex)
         if any(censored):
             # Try to use uncensored manifest first
-            not_censored=~censored
+            not_censored = ~censored
             if any(not_censored):
-                manifest_syn_id=manifest[not_censored]["id"][0]
+                manifest_syn_id = manifest[not_censored]["id"].iloc[0]
             # if only censored manifests are available, just use the first censored manifest
-            else: 
-                manifest_syn_id = manifest["id"][0]
+            else:
+                manifest_syn_id = manifest["id"].iloc[0]
 
-        #otherwise, use the first (implied only) version that exists
+        # otherwise, use the first (implied only) version that exists
         else:
-            manifest_syn_id = manifest["id"][0]
-        
+            manifest_syn_id = manifest["id"].iloc[0]
+
         return manifest_syn_id
 
     def getDatasetManifest(
-        self, datasetId: str, downloadFile: bool = False, newManifestName: str='',
+        self,
+        datasetId: str,
+        downloadFile: bool = False,
+        newManifestName: str = "",
     ) -> Union[str, File]:
         """Gets the manifest associated with a given dataset.
 
         Args:
             datasetId: synapse ID of a storage dataset.
             downloadFile: boolean argument indicating if manifest file in dataset should be downloaded or not.
-            newManifestName: new name of a manifest that gets downloaded 
+            newManifestName: new name of a manifest that gets downloaded
 
         Returns:
             manifest_syn_id (String): Synapse ID of exisiting manifest file.
             manifest_data (synapseclient.entity.File): Synapse entity if downloadFile is True.
             "" (String): No pre-exisiting manifest in dataset.
         """
         manifest_data = ""
 
         # get a list of files containing the manifest for this dataset (if any)
         all_files = self.storageFileviewTable
 
-        # construct regex based on manifest basename in the config 
-        manifest_re=re.compile(os.path.basename(self.manifest)+".*.[tc]sv")
+        # construct regex based on manifest basename in the config
+        manifest_re = re.compile(os.path.basename(self.manifest) + ".*.[tc]sv")
 
         # search manifest based on given manifest basename regex above
         # and return a dataframe containing name and id of manifests in a given asset view
         manifest = all_files[
-            (all_files['name'].str.contains(manifest_re,regex=True))
+            (all_files["name"].str.contains(manifest_re, regex=True))
             & (all_files["parentId"] == datasetId)
         ]
 
         manifest = manifest[["id", "name"]]
-        
+
         # if there is no pre-exisiting manifest in the specified dataset
         if manifest.empty:
-            logger.warning(f"Could not find a manifest that fits basename {self.manifest} in asset view and dataset {datasetId}")
+            logger.warning(
+                f"Could not find a manifest that fits basename {self.manifest} in asset view and dataset {datasetId}"
+            )
             return ""
 
         # if there is an exisiting manifest
         else:
             manifest_syn_id = self._get_manifest_id(manifest)
-            if downloadFile: 
+            if downloadFile:
                 md = ManifestDownload(self.syn, manifest_id=manifest_syn_id)
-                manifest_data = ManifestDownload.download_manifest(md, newManifestName=newManifestName, manifest_df=manifest)
-                ## TO DO: revisit how downstream code handle manifest_data. If the downstream code would break when manifest_data is an empty string, 
-                ## then we should catch the error here without returning an empty string. 
+                manifest_data = ManifestDownload.download_manifest(
+                    md, newManifestName=newManifestName, manifest_df=manifest
+                )
+                ## TO DO: revisit how downstream code handle manifest_data. If the downstream code would break when manifest_data is an empty string,
+                ## then we should catch the error here without returning an empty string.
                 if not manifest_data:
-                    logger.debug(f"No manifest data returned. Please check if you have successfully downloaded manifest: {manifest_syn_id}")
+                    logger.debug(
+                        f"No manifest data returned. Please check if you have successfully downloaded manifest: {manifest_syn_id}"
+                    )
                 return manifest_data
             return manifest_syn_id
 
-    def getDataTypeFromManifest(self, manifestId:str):
+    def getDataTypeFromManifest(self, manifestId: str):
         """Fetch a manifest and return data types of all columns
-        Args: 
+        Args:
             manifestId: synapse ID of a manifest
         """
-        # get manifest file path 
+        # get manifest file path
         manifest_filepath = self.syn.get(manifestId).path
 
-        # load manifest dataframe 
-        manifest = load_df(manifest_filepath, preserve_raw_input=False, data_model=False)
+        # load manifest dataframe
+        manifest = load_df(
+            manifest_filepath, preserve_raw_input=False, data_model=False
+        )
 
         # convert the dataFrame to use best possible dtypes.
         manifest_new = manifest.convert_dtypes()
 
         # get data types of columns
-        result = manifest_new.dtypes.to_frame('dtypes').reset_index()
-
-        # return the result as a dictionary 
-        result_dict = result.set_index('index')['dtypes'].astype(str).to_dict()
+        result = manifest_new.dtypes.to_frame("dtypes").reset_index()
 
+        # return the result as a dictionary
+        result_dict = result.set_index("index")["dtypes"].astype(str).to_dict()
 
         return result_dict
 
-    def _get_files_metadata_from_dataset(self, datasetId: str, only_new_files: bool, manifest:pd.DataFrame=None) -> Optional[dict]:
+    def _get_files_metadata_from_dataset(
+        self, datasetId: str, only_new_files: bool, manifest: pd.DataFrame = None
+    ) -> Optional[dict]:
         """retrieve file ids under a particular datasetId
 
         Args:
-            datasetId (str): a dataset id 
-            only_new_files (bool): if only adding new files that are not already exist 
-            manifest (pd.DataFrame): metadata manifest dataframe. Default to None. 
+            datasetId (str): a dataset id
+            only_new_files (bool): if only adding new files that are not already exist
+            manifest (pd.DataFrame): metadata manifest dataframe. Default to None.
 
         Returns:
             a dictionary that contains filename and entityid under a given datasetId or None if there is nothing under a given dataset id are not available
         """
         dataset_files = self.getFilesInStorageDataset(datasetId)
         if dataset_files:
-            dataset_file_names_id_dict = self._get_file_entityIds(dataset_files, only_new_files=only_new_files, manifest=manifest)
+            dataset_file_names_id_dict = self._get_file_entityIds(
+                dataset_files, only_new_files=only_new_files, manifest=manifest
+            )
             return dataset_file_names_id_dict
         else:
             return None
 
-    def add_entity_id_and_filename(self,  datasetId: str, manifest: pd.DataFrame) -> pd.DataFrame:
+    def add_entity_id_and_filename(
+        self, datasetId: str, manifest: pd.DataFrame
+    ) -> pd.DataFrame:
         """add entityid and filename column to an existing manifest assuming entityId column is not already present
 
         Args:
             datasetId (str): dataset syn id
-            manifest (pd.DataFrame): existing manifest dataframe, assuming this dataframe does not have an entityId column and Filename column is present but completely empty 
+            manifest (pd.DataFrame): existing manifest dataframe, assuming this dataframe does not have an entityId column and Filename column is present but completely empty
 
         Returns:
-            pd.DataFrame: returns a pandas dataframe 
+            pd.DataFrame: returns a pandas dataframe
         """
-        # get file names and entity ids of a given dataset 
-        dataset_files_dict = self._get_files_metadata_from_dataset(datasetId, only_new_files=False)
+        # get file names and entity ids of a given dataset
+        dataset_files_dict = self._get_files_metadata_from_dataset(
+            datasetId, only_new_files=False
+        )
 
-        if dataset_files_dict: 
-            # turn manifest dataframe back to a dictionary for operation 
-            manifest_dict = manifest.to_dict('list')
+        if dataset_files_dict:
+            # turn manifest dataframe back to a dictionary for operation
+            manifest_dict = manifest.to_dict("list")
 
             # update Filename column
             # add entityId column to the end
             manifest_dict.update(dataset_files_dict)
-            
-            # if the component column exists in existing manifest, fill up that column 
+
+            # if the component column exists in existing manifest, fill up that column
             if "Component" in manifest_dict.keys():
-                manifest_dict["Component"] = manifest_dict["Component"] * max(1, len(manifest_dict["Filename"]))
-            
+                manifest_dict["Component"] = manifest_dict["Component"] * max(
+                    1, len(manifest_dict["Filename"])
+                )
+
             # turn dictionary back to a dataframe
-            manifest_df_index = pd.DataFrame.from_dict(manifest_dict, orient='index')
+            manifest_df_index = pd.DataFrame.from_dict(manifest_dict, orient="index")
             manifest_df_updated = manifest_df_index.transpose()
 
             # fill na with empty string
             manifest_df_updated = manifest_df_updated.fillna("")
 
             # drop index
             manifest_df_updated = manifest_df_updated.reset_index(drop=True)
 
             return manifest_df_updated
         else:
             return manifest
 
-    def fill_in_entity_id_filename(self, datasetId: str, manifest: pd.DataFrame) -> Tuple[List, pd.DataFrame]:
-        """fill in Filename column and EntityId column. EntityId column and Filename column will be created if not already present. 
+    def fill_in_entity_id_filename(
+        self, datasetId: str, manifest: pd.DataFrame
+    ) -> Tuple[List, pd.DataFrame]:
+        """fill in Filename column and EntityId column. EntityId column and Filename column will be created if not already present.
 
         Args:
             datasetId (str): dataset syn id
             manifest (pd.DataFrame): existing manifest dataframe.
 
         Returns:
             Tuple[List, pd.DataFrame]: a list of synIds that are under a given datasetId folder and updated manifest dataframe
@@ -616,39 +671,43 @@
         dataset_files = self.getFilesInStorageDataset(datasetId)
 
         # update manifest with additional filenames, if any
         # note that if there is an existing manifest and there are files in the dataset
         # the columns Filename and entityId are assumed to be present in manifest schema
         # TODO: use idiomatic panda syntax
         if dataset_files:
-            new_files = self._get_file_entityIds(dataset_files=dataset_files, only_new_files=True, manifest=manifest)
+            new_files = self._get_file_entityIds(
+                dataset_files=dataset_files, only_new_files=True, manifest=manifest
+            )
 
             # update manifest so that it contains new dataset files
             new_files = pd.DataFrame(new_files)
             manifest = (
-                    pd.concat([manifest, new_files], sort=False)
-                    .reset_index()
-                    .drop("index", axis=1)
+                pd.concat([manifest, new_files], sort=False)
+                .reset_index()
+                .drop("index", axis=1)
             )
 
-        manifest = manifest.fillna("") 
+        manifest = manifest.fillna("")
         return dataset_files, manifest
-        
-    def updateDatasetManifestFiles(self, dmge: DataModelGraphExplorer, datasetId: str, store:bool = True) -> Union[Tuple[str, pd.DataFrame], None]:
+
+    def updateDatasetManifestFiles(
+        self, dmge: DataModelGraphExplorer, datasetId: str, store: bool = True
+    ) -> Union[Tuple[str, pd.DataFrame], None]:
         """Fetch the names and entity IDs of all current files in dataset in store, if any; update dataset's manifest with new files, if any.
 
         Args:
             dmge: DataModelGraphExplorer Instance
             datasetId: synapse ID of a storage dataset.
             store: if set to True store updated manifest in asset store; if set to False
             return a Pandas dataframe containing updated manifest but do not store to asset store
 
 
         Returns:
-            Synapse ID of updated manifest and Pandas dataframe containing the updated manifest. 
+            Synapse ID of updated manifest and Pandas dataframe containing the updated manifest.
             If there is no existing manifest return None
         """
 
         # get existing manifest Synapse ID
         manifest_id = self.getDatasetManifest(datasetId)
 
         # if there is no manifest return None
@@ -666,38 +725,44 @@
         dataset_files, manifest = self.fill_in_entity_id_filename(datasetId, manifest)
         if dataset_files:
             # update the manifest file, so that it contains the relevant entity IDs
             if store:
                 manifest.to_csv(manifest_filepath, index=False)
 
                 # store manifest and update associated metadata with manifest on Synapse
-                manifest_id = self.associateMetadataWithFiles(dmge, manifest_filepath, datasetId)
+                manifest_id = self.associateMetadataWithFiles(
+                    dmge, manifest_filepath, datasetId
+                )
 
-        
         return manifest_id, manifest
-    
-    def _get_file_entityIds(self, dataset_files: List,  only_new_files: bool = False, manifest: pd.DataFrame = None):
+
+    def _get_file_entityIds(
+        self,
+        dataset_files: List,
+        only_new_files: bool = False,
+        manifest: pd.DataFrame = None,
+    ):
         """
         Get a dictionary of files in a dataset. Either files that are not in the current manifest or all files
-        
+
         Args:
             manifest: metadata manifest
             dataset_file: List of all files in a dataset
             only_new_files: boolean to control whether only new files are returned or all files in the dataset
         Returns:
             files: dictionary of file names and entityIDs, with scope as specified by `only_new_files`
         """
         files = {"Filename": [], "entityId": []}
 
         if only_new_files:
             if manifest is None:
                 raise UnboundLocalError(
                     "No manifest was passed in, a manifest is required when `only_new_files` is True."
                 )
-            
+
             # find new files (that are not in the current manifest) if any
             for file_id, file_name in dataset_files:
                 if not file_id in manifest["entityId"].values:
                     files["Filename"].append(file_name)
                     files["entityId"].append(file_id)
         else:
             # get all files
@@ -721,223 +786,263 @@
                             (componentSchemaLabel, componentSchemaLabel) TODO: # get component name from schema
                         ),
                         ...
                     ]
 
         TODO: Return manifest URI instead of Synapse ID for interoperability with other implementations of a store interface
         """
-        component=None
-        entity=None
+        component = None
+        entity = None
         manifests = []
 
         datasets = self.getStorageDatasetsInProject(projectId)
 
-        for (datasetId, datasetName) in datasets:
+        for datasetId, datasetName in datasets:
             # encode information about the manifest in a simple list (so that R clients can unpack it)
             # eventually can serialize differently
-                
+
             # Get synID of manifest for a dataset
             manifestId = self.getDatasetManifest(datasetId)
 
             # If a manifest exists, get the annotations for it, else return base 'manifest' tuple
             if manifestId:
                 annotations = self.getFileAnnotations(manifestId)
 
                 # If manifest has annotations specifying component, use that
-                if annotations and 'Component' in annotations:
-                    component = annotations['Component']
+                if annotations and "Component" in annotations:
+                    component = annotations["Component"]
                     entity = self.syn.get(manifestId, downloadFile=False)
                     manifest_name = entity["properties"]["name"]
 
                 # otherwise download the manifest and parse for information
-                elif not annotations or 'Component' not in annotations:
+                elif not annotations or "Component" not in annotations:
                     logging.debug(
                         f"No component annotations have been found for manifest {manifestId}. "
                         "The manifest will be downloaded and parsed instead. "
                         "For increased speed, add component annotations to manifest."
-                        )
+                    )
 
-                    manifest_info = self.getDatasetManifest(datasetId,downloadFile=True)
+                    manifest_info = self.getDatasetManifest(
+                        datasetId, downloadFile=True
+                    )
                     manifest_name = manifest_info["properties"].get("name", "")
 
                     if not manifest_name:
-                        logger.error(f'Failed to download manifests from {datasetId}') 
+                        logger.error(f"Failed to download manifests from {datasetId}")
 
                     manifest_path = manifest_info["path"]
 
                     manifest_df = load_df(manifest_path)
 
                     # Get component from component column if it exists
-                    if "Component" in manifest_df and not manifest_df["Component"].empty:
-                        list(set(manifest_df['Component']))
+                    if (
+                        "Component" in manifest_df
+                        and not manifest_df["Component"].empty
+                    ):
+                        list(set(manifest_df["Component"]))
                         component = list(set(manifest_df["Component"]))
 
-                        #Added to address issues raised during DCA testing
-                        if '' in component:
-                            component.remove('')
+                        # Added to address issues raised during DCA testing
+                        if "" in component:
+                            component.remove("")
 
                         if len(component) == 1:
                             component = component[0]
                         elif len(component) > 1:
                             logging.warning(
-                            f"Manifest {manifestId} is composed of multiple components. Schematic does not support mulit-component manifests at this time."
-                            "Behavior of manifests with multiple components is undefined"
+                                f"Manifest {manifestId} is composed of multiple components. Schematic does not support mulit-component manifests at this time."
+                                "Behavior of manifests with multiple components is undefined"
                             )
             else:
                 manifest_name = ""
-                component = None              
+                component = None
             if component:
                 manifest = (
                     (datasetId, datasetName),
                     (manifestId, manifest_name),
                     (component, component),
                 )
             elif manifestId:
-                logging.debug(f"Manifest {manifestId} does not have an associated Component")
+                logging.debug(
+                    f"Manifest {manifestId} does not have an associated Component"
+                )
                 manifest = (
                     (datasetId, datasetName),
                     (manifestId, manifest_name),
                     ("", ""),
                 )
             else:
                 manifest = (
                     (datasetId, datasetName),
                     ("", ""),
                     ("", ""),
                 )
 
             if manifest:
                 manifests.append(manifest)
-                
+
         return manifests
 
-    def upload_project_manifests_to_synapse(self, dmge: DataModelGraphExplorer, projectId: str) -> List[str]:
+    def upload_project_manifests_to_synapse(
+        self, dmge: DataModelGraphExplorer, projectId: str
+    ) -> List[str]:
         """Upload all metadata manifest files across all datasets in a specified project as tables in Synapse.
 
         Returns: String of all the manifest_table_ids of all the manifests that have been loaded.
         """
 
         manifests = []
         manifest_loaded = []
         datasets = self.getStorageDatasetsInProject(projectId)
 
-        for (datasetId, datasetName) in datasets:
+        for datasetId, datasetName in datasets:
             # encode information about the manifest in a simple list (so that R clients can unpack it)
             # eventually can serialize differently
 
             manifest = ((datasetId, datasetName), ("", ""), ("", ""))
 
             manifest_info = self.getDatasetManifest(datasetId, downloadFile=True)
             if manifest_info:
                 manifest_id = manifest_info["properties"]["id"]
                 manifest_name = manifest_info["properties"]["name"]
                 manifest_path = manifest_info["path"]
                 manifest_df = load_df(manifest_path)
-                manifest_table_id = uploadDB(dmge=dmge, manifest=manifest, datasetId=datasetId, table_name=datasetName)
+                manifest_table_id = uploadDB(
+                    dmge=dmge,
+                    manifest=manifest,
+                    datasetId=datasetId,
+                    table_name=datasetName,
+                )
                 manifest_loaded.append(datasetName)
         return manifest_loaded
 
-    def upload_annotated_project_manifests_to_synapse(self, projectId:str, path_to_json_ld: str, dry_run: bool = False) -> List[str]:
-        '''
+    def upload_annotated_project_manifests_to_synapse(
+        self, projectId: str, path_to_json_ld: str, dry_run: bool = False
+    ) -> List[str]:
+        """
         Purpose:
             For all manifests in a project, upload them as a table and add annotations manifest csv.
             Assumes the manifest is already present as a CSV in a dataset in the project.
 
-        '''
+        """
         # Instantiate DataModelParser
-        data_model_parser = DataModelParser(path_to_data_model = path_to_json_ld)
-        #Parse Model
+        data_model_parser = DataModelParser(path_to_data_model=path_to_json_ld)
+        # Parse Model
         parsed_data_model = data_model_parser.parse_model()
 
         # Instantiate DataModelGraph
         data_model_grapher = DataModelGraph(parsed_data_model)
 
         # Generate graph
         graph_data_model = data_model_grapher.generate_data_model_graph()
 
-        #Instantiate DataModelGraphExplorer
+        # Instantiate DataModelGraphExplorer
         dmge = DataModelGraphExplorer(graph_data_model)
 
         manifests = []
         manifest_loaded = []
         datasets = self.getStorageDatasetsInProject(projectId)
-        for (datasetId, datasetName) in datasets:
+        for datasetId, datasetName in datasets:
             # encode information about the manifest in a simple list (so that R clients can unpack it)
             # eventually can serialize differently
 
             manifest = ((datasetId, datasetName), ("", ""), ("", ""))
             manifests.append(manifest)
 
             manifest_info = self.getDatasetManifest(datasetId, downloadFile=True)
 
             if manifest_info:
                 manifest_id = manifest_info["properties"]["id"]
                 manifest_name = manifest_info["properties"]["name"]
                 manifest_path = manifest_info["path"]
-                manifest = ((datasetId, datasetName), (manifest_id, manifest_name), ("", ""))
+                manifest = (
+                    (datasetId, datasetName),
+                    (manifest_id, manifest_name),
+                    ("", ""),
+                )
                 if not dry_run:
-                    manifest_syn_id = self.associateMetadataWithFiles(dmge, manifest_path, datasetId, manifest_record_type='table')
+                    manifest_syn_id = self.associateMetadataWithFiles(
+                        dmge, manifest_path, datasetId, manifest_record_type="table"
+                    )
                 manifest_loaded.append(manifest)
-            
-        return manifests, manifest_loaded
 
+        return manifests, manifest_loaded
 
-    def move_entities_to_new_project(self, projectId: str, newProjectId: str, returnEntities: bool = False, dry_run: bool = False):
+    def move_entities_to_new_project(
+        self,
+        projectId: str,
+        newProjectId: str,
+        returnEntities: bool = False,
+        dry_run: bool = False,
+    ):
         """
         For each manifest csv in a project, look for all the entitiy ids that are associated.
         Look up the entitiy in the files, move the entity to new project.
         """
 
         manifests = []
         manifest_loaded = []
         datasets = self.getStorageDatasetsInProject(projectId)
         if datasets:
-            for (datasetId, datasetName) in datasets:
+            for datasetId, datasetName in datasets:
                 # encode information about the manifest in a simple list (so that R clients can unpack it)
                 # eventually can serialize differently
 
                 manifest = ((datasetId, datasetName), ("", ""), ("", ""))
                 manifests.append(manifest)
 
                 manifest_info = self.getDatasetManifest(datasetId, downloadFile=True)
                 if manifest_info:
                     manifest_id = manifest_info["properties"]["id"]
                     manifest_name = manifest_info["properties"]["name"]
                     manifest_path = manifest_info["path"]
                     manifest_df = load_df(manifest_path)
 
-                    manifest = ((datasetId, datasetName), (manifest_id, manifest_name), ("", ""))
+                    manifest = (
+                        (datasetId, datasetName),
+                        (manifest_id, manifest_name),
+                        ("", ""),
+                    )
                     manifest_loaded.append(manifest)
 
                     annotation_entities = self.storageFileviewTable[
-                            (self.storageFileviewTable['id'].isin(manifest_df['entityId']))
-                            & (self.storageFileviewTable['type'] == 'folder')
-                        ]['id']
+                        (self.storageFileviewTable["id"].isin(manifest_df["entityId"]))
+                        & (self.storageFileviewTable["type"] == "folder")
+                    ]["id"]
 
                     if returnEntities:
-                        for entityId in annotation_entities: 
+                        for entityId in annotation_entities:
                             if not dry_run:
                                 self.syn.move(entityId, datasetId)
                             else:
-                                logging.info(f"{entityId} will be moved to folder {datasetId}.")
-                    else:                
+                                logging.info(
+                                    f"{entityId} will be moved to folder {datasetId}."
+                                )
+                    else:
                         # generate project folder
-                        archive_project_folder = Folder(projectId+'_archive', parent = newProjectId)
+                        archive_project_folder = Folder(
+                            projectId + "_archive", parent=newProjectId
+                        )
                         archive_project_folder = self.syn.store(archive_project_folder)
-        
+
                         # generate dataset folder
-                        dataset_archive_folder = Folder("_".join([datasetId,datasetName,'archive']), parent = archive_project_folder.id)
-                        dataset_archive_folder = self.syn.store(dataset_archive_folder)                    
+                        dataset_archive_folder = Folder(
+                            "_".join([datasetId, datasetName, "archive"]),
+                            parent=archive_project_folder.id,
+                        )
+                        dataset_archive_folder = self.syn.store(dataset_archive_folder)
 
                         for entityId in annotation_entities:
                             # move entities to folder
                             if not dry_run:
                                 self.syn.move(entityId, dataset_archive_folder.id)
                             else:
-                                logging.info(f"{entityId} will be moved to folder {dataset_archive_folder.id}.")
+                                logging.info(
+                                    f"{entityId} will be moved to folder {dataset_archive_folder.id}."
+                                )
         else:
             raise LookupError(
                 f"No datasets were found in the specified project: {projectId}. Re-check specified master_fileview in CONFIG and retry."
             )
         return manifests, manifest_loaded
 
     def get_synapse_table(self, synapse_id: str) -> Tuple[pd.DataFrame, CsvFileTable]:
@@ -953,222 +1058,283 @@
         return df, results
 
     def _get_tables(self, datasetId: str = None, projectId: str = None) -> List[Table]:
         if projectId:
             project = projectId
         elif datasetId:
             project = self.syn.get(self.getDatasetProject(datasetId))
-        
+
         return list(self.syn.getChildren(project, includeTypes=["table"]))
 
     def get_table_info(self, datasetId: str = None, projectId: str = None) -> List[str]:
         """Gets the names of the tables in the schema
         Can pass in a synID for a dataset or project
         Returns:
             list[str]: A list of table names
         """
-        tables = self._get_tables(datasetId = datasetId, projectId = projectId)
+        tables = self._get_tables(datasetId=datasetId, projectId=projectId)
         if tables:
             return {table["name"]: table["id"] for table in tables}
-        else: 
-            return {None:None}
+        else:
+            return {None: None}
 
     @missing_entity_handler
-    def uploadDB(self, 
-        dmge: DataModelGraphExplorer, 
-        manifest: pd.DataFrame, 
-        datasetId: str, 
-        table_name: str, 
-        restrict: bool = False, 
-        useSchemaLabel: bool = True, 
-        table_manipulation: str = 'replace',
-        ):
+    def uploadDB(
+        self,
+        dmge: DataModelGraphExplorer,
+        manifest: pd.DataFrame,
+        datasetId: str,
+        table_name: str,
+        restrict: bool = False,
+        table_manipulation: str = "replace",
+        table_column_names: str = "class_label",
+    ):
         """
         Method to upload a database to an asset store. In synapse, this will upload a metadata table
-        
+
         Args:
             dmge: DataModelGraphExplorer object
             manifest: pd.Df manifest to upload
             datasetId: synID of the dataset for the manifest
             table_name: name of the table to be uploaded
-            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
-            useSchemaLabel: bool whether to use schemaLabel (True) or display label (False)
+            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions
             existingTableId: str of the synId of the existing table, if one already exists
             table_manipulation: str, 'replace' or 'upsert', in the case where a manifest already exists, should the new metadata replace the existing (replace) or be added to it (upsert)
-
+            table_column_names: (str): display_name/display_label/class_label (default). Sets labeling style for table column names. display_name will use the raw display name as the column name. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting.
         Returns:
             manifest_table_id: synID of the uploaded table
             manifest: the original manifset
             table_manifest: manifest formatted appropriately for the table
-        
+
         """
-        
 
-        col_schema, table_manifest = self.formatDB(dmge=dmge, manifest=manifest, useSchemaLabel=useSchemaLabel)
+        col_schema, table_manifest = self.formatDB(
+            dmge=dmge, manifest=manifest, table_column_names=table_column_names
+        )
 
-        manifest_table_id = self.buildDB(datasetId, table_name, col_schema, table_manifest, table_manipulation, dmge, restrict,)
+        manifest_table_id = self.buildDB(
+            datasetId,
+            table_name,
+            col_schema,
+            table_manifest,
+            table_manipulation,
+            dmge,
+            restrict,
+        )
 
         return manifest_table_id, manifest, table_manifest
 
-    def formatDB(self, dmge, manifest, useSchemaLabel):
+    def formatDB(self, dmge, manifest, table_column_names):
         """
         Method to format a manifest appropriatly for upload as table
-        
+
         Args:
             dmge: DataModelGraphExplorer object
             manifest: pd.Df manifest to upload
-            useSchemaLabel: bool whether to use schemaLabel (True) or display label (False)
-
+            table_column_names: (str): display_name/display_label/class_label (default). Sets labeling style for table column names. display_name will use the raw display name as the column name. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting.
         Returns:
             col_schema: schema for table columns: type, size, etc
             table_manifest: formatted manifest
-        
+
         """
         # Rename the manifest columns to display names to match fileview
 
-        blacklist_chars = ['(', ')', '.', ' ', '-']
+        blacklist_chars = ["(", ")", ".", " ", "-"]
         manifest_columns = manifest.columns.tolist()
 
-        table_manifest=deepcopy(manifest)
+        table_manifest = deepcopy(manifest)
 
-        if useSchemaLabel:
+        if table_column_names == "display_name":
+            cols = table_manifest.columns
+
+        elif table_column_names == "display_label":
             cols = [
-                get_class_label_from_display_name(
-                    str(col)
-                    ).translate({ord(x): '' for x in blacklist_chars})
+                str(col).translate({ord(x): "" for x in blacklist_chars})
                 for col in manifest_columns
             ]
 
-            cols = list(map(lambda x: x.replace('EntityId', 'entityId'), cols))
+        elif table_column_names == "class_label":
+            cols = [
+                get_class_label_from_display_name(str(col)).translate(
+                    {ord(x): "" for x in blacklist_chars}
+                )
+                for col in manifest_columns
+            ]
+        else:
+            ValueError(
+                f"The provided table_column_name: {table_column_names} is not valid, please resubmit with an allowed value only."
+            )
 
+        cols = list(map(lambda x: x.replace("EntityId", "entityId"), cols))
 
-            # Reset column names in table manifest
-            table_manifest.columns = cols
+        # Reset column names in table manifest
+        table_manifest.columns = cols
 
-        #move entity id to end of df
-        entity_col = table_manifest.pop('entityId')
-        table_manifest.insert(len(table_manifest.columns), 'entityId', entity_col)
+        # move entity id to end of df
+        entity_col = table_manifest.pop("entityId")
+        table_manifest.insert(len(table_manifest.columns), "entityId", entity_col)
 
         # Get the column schema
         col_schema = as_table_columns(table_manifest)
 
         # Set Id column length to 64 (for some reason not being auto set.)
         for i, col in enumerate(col_schema):
-            if col['name'].lower() == 'id':
-                col_schema[i]['maximumSize'] = 64
+            if col["name"].lower() == "id":
+                col_schema[i]["maximumSize"] = 64
 
         return col_schema, table_manifest
 
-    def buildDB(self,  
-        datasetId: str, 
-        table_name: str, 
+    def buildDB(
+        self,
+        datasetId: str,
+        table_name: str,
         col_schema: List,
         table_manifest: pd.DataFrame,
         table_manipulation: str,
-        dmge: DataModelGraphExplorer,  
+        dmge: DataModelGraphExplorer,
         restrict: bool = False,
-        
-        ):
+    ):
         """
         Method to construct the table appropriately: create new table, replace existing, or upsert new into existing
-        Calls TableOperations class to execute 
-        
+        Calls TableOperations class to execute
+
         Args:
             datasetId: synID of the dataset for the manifest
             table_name: name of the table to be uploaded
             col_schema: schema for table columns: type, size, etc from `formatDB`
             table_manifest: formatted manifest that can be uploaded as a table
             table_manipulation: str, 'replace' or 'upsert', in the case where a manifest already exists, should the new metadata replace the existing (replace) or be added to it (upsert)
-            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
+            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions
 
         Returns:
             manifest_table_id: synID of the uploaded table
-        
+
         """
-        table_info = self.get_table_info(datasetId = datasetId)
+        table_info = self.get_table_info(datasetId=datasetId)
         # Put table manifest onto synapse
-        schema = Schema(name=table_name, columns=col_schema, parent=self.getDatasetProject(datasetId))
+        schema = Schema(
+            name=table_name,
+            columns=col_schema,
+            parent=self.getDatasetProject(datasetId),
+        )
 
         if table_name in table_info:
             existingTableId = table_info[table_name]
         else:
             existingTableId = None
 
-
         tableOps = TableOperations(
-            synStore = self,  
-            tableToLoad = table_manifest,
-            tableName = table_name,
-            datasetId = datasetId, 
-            existingTableId = existingTableId,
-            restrict = restrict,
-            )
+            synStore=self,
+            tableToLoad=table_manifest,
+            tableName=table_name,
+            datasetId=datasetId,
+            existingTableId=existingTableId,
+            restrict=restrict,
+        )
 
         if not table_manipulation or table_name not in table_info.keys():
-            manifest_table_id = tableOps.createTable(columnTypeDict=col_schema, specifySchema=True,)
+            manifest_table_id = tableOps.createTable(
+                columnTypeDict=col_schema,
+                specifySchema=True,
+            )
         elif table_name in table_info.keys() and table_info[table_name]:
-
-            if table_manipulation.lower() == 'replace':
-                manifest_table_id = tableOps.replaceTable(specifySchema = True, columnTypeDict=col_schema,)
-            elif table_manipulation.lower() == 'upsert':
-                manifest_table_id = tableOps.upsertTable(dmge=dmge,)
-            elif table_manipulation.lower() == 'update':
+            if table_manipulation.lower() == "replace":
+                manifest_table_id = tableOps.replaceTable(
+                    specifySchema=True,
+                    columnTypeDict=col_schema,
+                )
+            elif table_manipulation.lower() == "upsert":
+                manifest_table_id = tableOps.upsertTable(
+                    dmge=dmge,
+                )
+            elif table_manipulation.lower() == "update":
                 manifest_table_id = tableOps.updateTable()
 
-
-
-        if table_manipulation and table_manipulation.lower() == 'upsert':
-            existing_tables=self.get_table_info(datasetId=datasetId)
-            tableId=existing_tables[table_name]
+        if table_manipulation and table_manipulation.lower() == "upsert":
+            existing_tables = self.get_table_info(datasetId=datasetId)
+            tableId = existing_tables[table_name]
             annos = self.syn.get_annotations(tableId)
-            annos['primary_key'] = table_manifest['Component'][0] + "_id"
+            annos["primary_key"] = table_manifest["Component"][0] + "_id"
             annos = self.syn.set_annotations(annos)
 
         return manifest_table_id
 
-
-    def upload_manifest_file(self, manifest, metadataManifestPath, datasetId, restrict_manifest, component_name = ''):
+    def upload_manifest_file(
+        self,
+        manifest,
+        metadataManifestPath,
+        datasetId,
+        restrict_manifest,
+        component_name="",
+    ):
         # Update manifest to have the new entityId column
         manifest.to_csv(metadataManifestPath, index=False)
 
         # store manifest to Synapse as a CSV
         # update file name
-        file_name_full = metadataManifestPath.split('/')[-1]
-        file_extension = file_name_full.split('.')[-1]
+        file_name_full = metadataManifestPath.split("/")[-1]
+        file_extension = file_name_full.split(".")[-1]
 
         # Differentiate "censored" and "uncensored" manifest
-        if "censored" in file_name_full: 
-            file_name_new = os.path.basename(CONFIG.synapse_manifest_basename) + "_" + component_name + "_censored" + '.' + file_extension
-        else: 
-            file_name_new = os.path.basename(CONFIG.synapse_manifest_basename) + "_" + component_name + '.' + file_extension
+        if "censored" in file_name_full:
+            file_name_new = (
+                os.path.basename(CONFIG.synapse_manifest_basename)
+                + "_"
+                + component_name
+                + "_censored"
+                + "."
+                + file_extension
+            )
+        else:
+            file_name_new = (
+                os.path.basename(CONFIG.synapse_manifest_basename)
+                + "_"
+                + component_name
+                + "."
+                + file_extension
+            )
 
         manifestSynapseFile = File(
             metadataManifestPath,
             description="Manifest for dataset " + datasetId,
             parent=datasetId,
-            name=file_name_new
+            name=file_name_new,
+        )
+
+        manifest_synapse_file_id = self.syn.store(
+            manifestSynapseFile, isRestricted=restrict_manifest
+        ).id
+        changeFileMetaData(
+            syn=self.syn, entity=manifest_synapse_file_id, downloadAs=file_name_new
         )
 
-        manifest_synapse_file_id = self.syn.store(manifestSynapseFile, isRestricted = restrict_manifest).id
-        changeFileMetaData(syn = self.syn, entity = manifest_synapse_file_id, downloadAs = file_name_new)
-        
         return manifest_synapse_file_id
 
     @missing_entity_handler
-    def format_row_annotations(self, dmge, row, entityId, hideBlanks):
+    def format_row_annotations(
+        self, dmge, row, entityId: str, hideBlanks: bool, annotation_keys: str
+    ):
         # prepare metadata for Synapse storage (resolve display name into a name that Synapse annotations support (e.g no spaces, parenthesis)
         # note: the removal of special characters, will apply only to annotation keys; we are not altering the manifest
         # this could create a divergence between manifest column and annotations. this should be ok for most use cases.
         # columns with special characters are outside of the schema
         metadataSyn = {}
-        blacklist_chars = ['(', ')', '.', ' ', '-']
-        
-        for k, v in row.to_dict().items():
+        blacklist_chars = ["(", ")", ".", " ", "-"]
 
-            keySyn = get_class_label_from_display_name(str(k)).translate({ord(x): '' for x in blacklist_chars})
+        for k, v in row.to_dict().items():
+            if annotation_keys == "display_label":
+                keySyn = str(k).translate({ord(x): "" for x in blacklist_chars})
+            elif annotation_keys == "class_label":
+                keySyn = get_class_label_from_display_name(str(k)).translate(
+                    {ord(x): "" for x in blacklist_chars}
+                )
 
             # Skip `Filename` and `ETag` columns when setting annotations
             if keySyn in ["Filename", "ETag", "eTag"]:
                 continue
 
             # truncate annotation values to 500 characters if the
             # size of values is greater than equal to 500 characters
@@ -1177,76 +1343,83 @@
             # has been truncated
             if isinstance(v, str) and len(v) >= 500:
                 v = v[0:472] + "[truncatedByDataCuratorApp]"
 
             metadataSyn[keySyn] = v
         # set annotation(s) for the various objects/items in a dataset on Synapse
         annos = self.syn.get_annotations(entityId)
-        csv_list_regex=comma_separated_list_regex()
+        csv_list_regex = comma_separated_list_regex()
         for anno_k, anno_v in metadataSyn.items():
-            
             # Remove keys with nan or empty string values from dict of annotations to be uploaded
             # if present on current data annotation
-            if hideBlanks and (anno_v == '' or (isinstance(anno_v,float) and np.isnan(anno_v))):
+            if hideBlanks and (
+                anno_v == "" or (isinstance(anno_v, float) and np.isnan(anno_v))
+            ):
                 annos.pop(anno_k) if anno_k in annos.keys() else annos
             # Otherwise save annotation as approrpriate
             else:
-                if isinstance(anno_v,float) and np.isnan(anno_v):
-                        annos[anno_k] = ""
-                elif isinstance(anno_v,str) and re.fullmatch(csv_list_regex, anno_v) and rule_in_rule_list('list', dmge.get_node_validation_rules(anno_k)):
+                if isinstance(anno_v, float) and np.isnan(anno_v):
+                    annos[anno_k] = ""
+                elif (
+                    isinstance(anno_v, str)
+                    and re.fullmatch(csv_list_regex, anno_v)
+                    and rule_in_rule_list(
+                        "list", dmge.get_node_validation_rules(anno_k)
+                    )
+                ):
                     annos[anno_k] = anno_v.split(",")
                 else:
                     annos[anno_k] = anno_v
-                
+
         return annos
 
     @missing_entity_handler
     def format_manifest_annotations(self, manifest, manifest_synapse_id):
-        '''
+        """
         Set annotations for the manifest (as a whole) so they can be applied to the manifest table or csv.
         For now just getting the Component.
-        '''
-        
+        """
+
         entity = self.syn.get(manifest_synapse_id, downloadFile=False)
         is_file = entity.concreteType.endswith(".FileEntity")
         is_table = entity.concreteType.endswith(".TableEntity")
 
         if is_file:
-
             # Get file metadata
             metadata = self.getFileAnnotations(manifest_synapse_id)
 
             # If there is a defined component add it to the metadata.
-            if 'Component' in manifest.columns:
+            if "Component" in manifest.columns:
                 # Gather component information
-                component = manifest['Component'].unique()
-                
+                component = manifest["Component"].unique()
+
                 # Double check that only a single component is listed, else raise an error.
                 try:
                     len(component) == 1
                 except ValueError as err:
                     raise ValueError(
                         f"Manifest has more than one component. Please check manifest and resubmit."
                     ) from err
 
                 # Add component to metadata
-                metadata['Component'] = component[0]
-        
+                metadata["Component"] = component[0]
+
         elif is_table:
             # Get table metadata
             metadata = self.getTableAnnotations(manifest_synapse_id)
-        
+
         # Get annotations
         annos = self.syn.get_annotations(manifest_synapse_id)
 
         # Add metadata to the annotations
         for annos_k, annos_v in metadata.items():
             annos[annos_k] = annos_v
 
         return annos
+
     '''
     def annotate_upload_manifest_table(self, manifest, datasetId, metadataManifestPath,
         useSchemaLabel: bool = True, hideBlanks: bool = False, restrict_manifest = False):
         """
         Purpose:
             Works very similarly to associateMetadataWithFiles except takes in the manifest
             rather than the manifest path
@@ -1316,63 +1489,73 @@
         
         # Get annotations for the table manifest
         manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_table_id)
         self.syn.set_annotations(manifest_annotations)
         return manifest_synapse_table_id
     '''
 
-    def _read_manifest(self, metadataManifestPath:str) -> pd.DataFrame:
+    def _read_manifest(self, metadataManifestPath: str) -> pd.DataFrame:
         """Helper function to read in provided manifest as a pandas DataFrame for subsequent downstream processing.
         Args:
             metadataManifestPath (str): path where manifest is stored
         Returns:
             manifest(pd.DataFrame): Manifest loaded as a pandas dataframe
         Raises:
             FileNotFoundError: Manifest file does not exist at provided path.
         """
         # read new manifest csv
         try:
-            load_args={
-                "dtype":"string",
+            load_args = {
+                "dtype": "string",
             }
-            manifest = load_df(metadataManifestPath, preserve_raw_input = False, **load_args)
+            manifest = load_df(
+                metadataManifestPath, preserve_raw_input=False, **load_args
+            )
         except FileNotFoundError as err:
             raise FileNotFoundError(
                 f"No manifest file was found at this path: {metadataManifestPath}"
             ) from err
         return manifest
 
-    def _add_id_columns_to_manifest(self, manifest: pd.DataFrame, dmge: DataModelGraphExplorer):
+    def _add_id_columns_to_manifest(
+        self, manifest: pd.DataFrame, dmge: DataModelGraphExplorer
+    ):
         """Helper function to add id and entityId columns to the manifest if they do not already exist, Fill id values per row.
         Args:
             Manifest loaded as a pd.Dataframe
         Returns (pd.DataFrame):
             Manifest df with new Id and EntityId columns (and UUID values) if they were not already present.
         """
 
         # Add Id for table updates and fill.
         if not col_in_dataframe("Id", manifest):
             # See if schema has `Uuid` column specified
             try:
-                uuid_col_in_schema = dmge.is_class_in_schema('Uuid') or dmge.is_class_in_schema('uuid')      
-            except (KeyError):
+                uuid_col_in_schema = dmge.is_class_in_schema(
+                    "Uuid"
+                ) or dmge.is_class_in_schema("uuid")
+            except KeyError:
                 uuid_col_in_schema = False
 
             # Rename `Uuid` column if it wasn't specified in the schema
             if col_in_dataframe("Uuid", manifest) and not uuid_col_in_schema:
-                manifest.rename(columns={'Uuid': 'Id'}, inplace=True)
+                manifest.rename(columns={"Uuid": "Id"}, inplace=True)
             # If no `Uuid` column exists or it is specified in the schema, create a new `Id` column
             else:
-                manifest["Id"] = ''
+                manifest["Id"] = ""
 
-        for idx,row in manifest.iterrows():
-            if not row["Id"]:
+        # Retrieve the ID column name (id, Id and ID) are treated the same.
+        id_col_name = [col for col in manifest.columns if col.lower() == "id"][0]
+
+        # Check if values have been added to the Id coulumn, if not add a UUID so value in the row is not blank.
+        for idx, row in manifest.iterrows():
+            if not row[id_col_name]:
                 gen_uuid = str(uuid.uuid4())
-                row["Id"] = gen_uuid
-                manifest.loc[idx, 'Id'] = gen_uuid
+                row[id_col_name] = gen_uuid
+                manifest.loc[idx, id_col_name] = gen_uuid
 
         # add entityId as a column if not already there or
         # fill any blanks with an empty string.
         if not col_in_dataframe("entityId", manifest):
             manifest["entityId"] = ""
         else:
             manifest["entityId"].fillna("", inplace=True)
@@ -1384,284 +1567,381 @@
         Args:
             Manifest loaded as a pd.Dataframe
         Returns:
             table_name (str): Name of the table to load
             component_name (str): Name of the manifest component (if applicable)
         """
         # Create table name here.
-        if 'Component' in manifest.columns:
-            component_name = manifest['Component'][0].lower()
-            table_name = component_name + '_synapse_storage_manifest_table'
+        if "Component" in manifest.columns:
+            component_name = manifest["Component"][0].lower()
+            table_name = component_name + "_synapse_storage_manifest_table"
         else:
-            component_name = ''
-            table_name = 'synapse_storage_manifest_table'
+            component_name = ""
+            table_name = "synapse_storage_manifest_table"
         return table_name, component_name
 
-    def _add_annotations(self, dmge, row, entityId, hideBlanks):
+    def _add_annotations(
+        self,
+        dmge,
+        row,
+        entityId: str,
+        hideBlanks: bool,
+        annotation_keys: str,
+    ):
         """Helper function to format and add annotations to entities in Synapse.
         Args:
             dmge: DataModelGraphExplorer object,
             row: current row of manifest being processed
             entityId (str): synapseId of entity to add annotations to
             hideBlanks: Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
+            annotation_keys:  (str) display_label/class_label(default), Determines labeling syle for annotation keys. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting while ensuring the label is formatted properly for Synapse annotations.
         Returns:
             Annotations are added to entities in Synapse, no return.
         """
         # Format annotations for Synapse
-        annos = self.format_row_annotations(dmge, row, entityId, hideBlanks)
+        annos = self.format_row_annotations(
+            dmge, row, entityId, hideBlanks, annotation_keys
+        )
 
         if annos:
-        # Store annotations for an entity folder
+            # Store annotations for an entity folder
             self.syn.set_annotations(annos)
         return
 
     def _create_entity_id(self, idx, row, manifest, datasetId):
         """Helper function to generate an entityId and add it to the appropriate row in the manifest.
         Args:
             row: current row of manifest being processed
             manifest (pd.DataFrame): loaded df containing user supplied data.
             datasetId (str): synapse ID of folder containing the dataset
 
         Returns:
             manifest (pd.DataFrame): manifest with entityId added to the appropriate row
             entityId (str): Generated Entity Id.
-        
+
         """
         rowEntity = Folder(str(uuid.uuid4()), parent=datasetId)
         rowEntity = self.syn.store(rowEntity)
         entityId = rowEntity["id"]
         row["entityId"] = entityId
         manifest.loc[idx, "entityId"] = entityId
         return manifest, entityId
 
     def add_annotations_to_entities_files(
-                    self,
-                    dmge,
-                    manifest,
-                    manifest_record_type,
-                    datasetId,
-                    hideBlanks,
-                    manifest_synapse_table_id=''
-                    ):
-        '''Depending on upload type add Ids to entityId row. Add anotations to connected files.
+        self,
+        dmge,
+        manifest,
+        manifest_record_type: str,
+        datasetId: str,
+        hideBlanks: bool,
+        manifest_synapse_table_id="",
+        annotation_keys: str = "class_label",
+    ):
+        """Depending on upload type add Ids to entityId row. Add anotations to connected files.
         Args:
             dmge: DataModelGraphExplorer Object
             manifest (pd.DataFrame): loaded df containing user supplied data.
             manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
             datasetId (str): synapse ID of folder containing the dataset
             hideBlanks (bool): Default is false -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
             manifest_synapse_table_id (str): Default is an empty string ''.
+            annotation_keys: (str) display_label/class_label(default), Determines labeling syle for annotation keys. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting while ensuring the label is formatted properly for Synapse annotations.
         Returns:
             manifest (pd.DataFrame): modified to add entitiyId as appropriate.
 
-        '''
+        """
 
         # Expected behavior is to annotate files if `Filename` is present regardless of `-mrt` setting
-        if 'filename' in [col.lower() for col in manifest.columns]:
+        if "filename" in [col.lower() for col in manifest.columns]:
             # get current list of files and store as dataframe
             dataset_files = self.getFilesInStorageDataset(datasetId)
-            files_and_entityIds = self._get_file_entityIds(dataset_files=dataset_files, only_new_files=False)
+            files_and_entityIds = self._get_file_entityIds(
+                dataset_files=dataset_files, only_new_files=False
+            )
             file_df = pd.DataFrame(files_and_entityIds)
-            
+
             # Merge dataframes to add entityIds
-            manifest = manifest.merge(file_df, how = 'left', on='Filename', suffixes=['_x',None]).drop('entityId_x',axis=1)
+            manifest = manifest.merge(
+                file_df, how="left", on="Filename", suffixes=["_x", None]
+            ).drop("entityId_x", axis=1)
 
         # Fill `entityId` for each row if missing and annotate entity as appropriate
         for idx, row in manifest.iterrows():
-            if not row["entityId"] and (manifest_record_type == 'file_and_entities' or 
-                manifest_record_type == 'table_file_and_entities'):
-                manifest, entityId = self._create_entity_id(idx, row, manifest, datasetId)
-            elif not row["entityId"] and manifest_record_type == 'table_and_file':
-                # If not using entityIds, fill with manifest_table_id so 
+            if not row["entityId"] and (
+                manifest_record_type == "file_and_entities"
+                or manifest_record_type == "table_file_and_entities"
+            ):
+                manifest, entityId = self._create_entity_id(
+                    idx, row, manifest, datasetId
+                )
+            elif not row["entityId"] and manifest_record_type == "table_and_file":
+                # If not using entityIds, fill with manifest_table_id so
                 row["entityId"] = manifest_synapse_table_id
                 manifest.loc[idx, "entityId"] = manifest_synapse_table_id
-                entityId = ''
+                entityId = ""
             else:
                 # get the file id of the file to annotate, collected in above step.
                 entityId = row["entityId"]
 
             # Adding annotations to connected files.
             if entityId:
-                self._add_annotations(dmge, row, entityId, hideBlanks)
+                self._add_annotations(dmge, row, entityId, hideBlanks, annotation_keys)
                 logger.info(f"Added annotations to entity: {entityId}")
         return manifest
 
     def upload_manifest_as_table(
-                            self,
-                            dmge,
-                            manifest,
-                            metadataManifestPath,
-                            datasetId,
-                            table_name,
-                            component_name,
-                            restrict,
-                            manifest_record_type,
-                            useSchemaLabel,
-                            hideBlanks,
-                            table_manipulation,
-                            ):
+        self,
+        dmge: DataModelGraphExplorer,
+        manifest: pd.DataFrame,
+        metadataManifestPath: str,
+        datasetId: str,
+        table_name: str,
+        component_name: str,
+        restrict: bool,
+        manifest_record_type: str,
+        hideBlanks: bool,
+        table_manipulation: str,
+        table_column_names: str,
+        annotation_keys: str,
+    ):
         """Upload manifest to Synapse as a table and csv.
         Args:
             dmge: DataModelGraphExplorer object
             manifest (pd.DataFrame): loaded df containing user supplied data.
             metadataManifestPath: path to csv containing a validated metadata manifest.
             datasetId (str): synapse ID of folder containing the dataset
             table_name (str): Generated to name the table being uploaded.
             component_name (str): Name of the component manifest that is currently being uploaded.
             restrict (bool): Flag for censored data.
             manifest_record_type (str): valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
             hideBlanks (bool): Default is False -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
             table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
+            table_column_names: (str): display_name/display_label/class_label (default). Sets labeling style for table column names. display_name will use the raw display name as the column name. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting.
+            annotation_keys: (str) display_label/class_label (default), Sets labeling syle for annotation keys. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting while ensuring the label is formatted properly for Synapse annotations.
         Return:
             manifest_synapse_file_id: SynID of manifest csv uploaded to synapse.
-        """      
+        """
         # Upload manifest as a table, get the ID and updated manifest.
         manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
-                                                    dmge=dmge,
-                                                    manifest=manifest,
-                                                    datasetId=datasetId,
-                                                    table_name=table_name,
-                                                    restrict=restrict,
-                                                    useSchemaLabel=useSchemaLabel,
-                                                    table_manipulation=table_manipulation)
+            dmge=dmge,
+            manifest=manifest,
+            datasetId=datasetId,
+            table_name=table_name,
+            restrict=restrict,
+            table_manipulation=table_manipulation,
+            table_column_names=table_column_names,
+        )
 
-        manifest = self.add_annotations_to_entities_files(dmge, manifest, manifest_record_type, datasetId, hideBlanks, manifest_synapse_table_id)
+        manifest = self.add_annotations_to_entities_files(
+            dmge,
+            manifest,
+            manifest_record_type,
+            datasetId,
+            hideBlanks,
+            manifest_synapse_table_id,
+            annotation_keys,
+        )
         # Load manifest to synapse as a CSV File
-        manifest_synapse_file_id = self.upload_manifest_file(manifest, metadataManifestPath, datasetId, restrict, component_name = component_name)
-        
+        manifest_synapse_file_id = self.upload_manifest_file(
+            manifest,
+            metadataManifestPath,
+            datasetId,
+            restrict,
+            component_name=component_name,
+        )
+
         # Set annotations for the file manifest.
-        manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
+        manifest_annotations = self.format_manifest_annotations(
+            manifest, manifest_synapse_file_id
+        )
         self.syn.set_annotations(manifest_annotations)
         logger.info("Associated manifest file with dataset on Synapse.")
-        
+
         # Update manifest Synapse table with new entity id column.
         manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
-                                                    dmge=dmge,
-                                                    manifest=manifest, 
-                                                    datasetId=datasetId, 
-                                                    table_name=table_name,  
-                                                    restrict=restrict,
-                                                    useSchemaLabel=useSchemaLabel,
-                                                    table_manipulation='update')
+            dmge=dmge,
+            manifest=manifest,
+            datasetId=datasetId,
+            table_name=table_name,
+            restrict=restrict,
+            table_manipulation="update",
+            table_column_names=table_column_names,
+        )
 
         # Set annotations for the table manifest
-        manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_table_id)
+        manifest_annotations = self.format_manifest_annotations(
+            manifest, manifest_synapse_table_id
+        )
         self.syn.set_annotations(manifest_annotations)
         return manifest_synapse_file_id
 
     def upload_manifest_as_csv(
-                            self,
-                            dmge,
-                            manifest,
-                            metadataManifestPath,
-                            datasetId,
-                            restrict,
-                            manifest_record_type,
-                            hideBlanks,
-                            component_name):
+        self,
+        dmge,
+        manifest,
+        metadataManifestPath,
+        datasetId,
+        restrict,
+        manifest_record_type,
+        hideBlanks,
+        component_name,
+        annotation_keys: str,
+    ):
         """Upload manifest to Synapse as a csv only.
         Args:
             dmge: DataModelGraphExplorer object
             manifest (pd.DataFrame): loaded df containing user supplied data.
             metadataManifestPath: path to csv containing a validated metadata manifest.
             datasetId (str): synapse ID of folder containing the dataset
             restrict (bool): Flag for censored data.
             manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
             hideBlanks (bool): Default is False -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
-            table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
-            with_entities (bool): Default is False - Flag to indicate whether to create entityIds and add annotations.
+            annotation_keys: (str) display_label/class_label (default), Sets labeling syle for annotation keys. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting while ensuring the label is formatted properly for Synapse annotations.
         Return:
             manifest_synapse_file_id (str): SynID of manifest csv uploaded to synapse.
         """
-
-        manifest = self.add_annotations_to_entities_files(dmge, manifest, manifest_record_type, datasetId, hideBlanks)
+        manifest = self.add_annotations_to_entities_files(
+            dmge,
+            manifest,
+            manifest_record_type,
+            datasetId,
+            hideBlanks,
+            annotation_keys=annotation_keys,
+        )
 
         # Load manifest to synapse as a CSV File
-        manifest_synapse_file_id = self.upload_manifest_file(manifest,
-                metadataManifestPath, datasetId, restrict, component_name = component_name)
-        
+        manifest_synapse_file_id = self.upload_manifest_file(
+            manifest,
+            metadataManifestPath,
+            datasetId,
+            restrict,
+            component_name=component_name,
+        )
+
         # Set annotations for the file manifest.
-        manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
+        manifest_annotations = self.format_manifest_annotations(
+            manifest, manifest_synapse_file_id
+        )
         self.syn.set_annotations(manifest_annotations)
 
         logger.info("Associated manifest file with dataset on Synapse.")
-        
+
         return manifest_synapse_file_id
 
     def upload_manifest_combo(
-                            self,
-                            dmge,
-                            manifest,
-                            metadataManifestPath,
-                            datasetId,
-                            table_name,
-                            component_name,
-                            restrict,
-                            manifest_record_type,
-                            useSchemaLabel,
-                            hideBlanks,
-                            table_manipulation,
-                            ):
+        self,
+        dmge,
+        manifest,
+        metadataManifestPath,
+        datasetId,
+        table_name,
+        component_name,
+        restrict,
+        manifest_record_type,
+        hideBlanks,
+        table_manipulation,
+        table_column_names: str,
+        annotation_keys: str,
+    ):
         """Upload manifest to Synapse as a table and CSV with entities.
         Args:
             dmge: DataModelGraphExplorer object
             manifest (pd.DataFrame): loaded df containing user supplied data.
             metadataManifestPath: path to csv containing a validated metadata manifest.
             datasetId (str): synapse ID of folder containing the dataset
             table_name (str): Generated to name the table being uploaded.
             component_name (str): Name of the component manifest that is currently being uploaded.
             restrict (bool): Flag for censored data.
             manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
-            useSchemaLabel (bool): Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
             hideBlanks (bool): Default is False -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
             table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
+            table_column_names: (str): display_name/display_label/class_label (default). Sets labeling style for table column names. display_name will use the raw display name as the column name. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting.
+            annotation_keys: (str) display_label/class_label (default), Sets labeling syle for annotation keys. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting while ensuring the label is formatted properly for Synapse annotations.
         Return:
             manifest_synapse_file_id (str): SynID of manifest csv uploaded to synapse.
         """
         manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
-                                                    dmge=dmge,
-                                                    manifest=manifest,
-                                                    datasetId=datasetId,
-                                                    table_name=table_name,
-                                                    restrict=restrict,
-                                                    useSchemaLabel=useSchemaLabel,
-                                                    table_manipulation=table_manipulation)
+            dmge=dmge,
+            manifest=manifest,
+            datasetId=datasetId,
+            table_name=table_name,
+            restrict=restrict,
+            table_manipulation=table_manipulation,
+            table_column_names=table_column_names,
+        )
+
+        manifest = self.add_annotations_to_entities_files(
+            dmge,
+            manifest,
+            manifest_record_type,
+            datasetId,
+            hideBlanks,
+            manifest_synapse_table_id,
+            annotation_keys=annotation_keys,
+        )
 
-        manifest = self.add_annotations_to_entities_files(dmge, manifest, manifest_record_type, datasetId, hideBlanks, manifest_synapse_table_id)
-        
         # Load manifest to synapse as a CSV File
-        manifest_synapse_file_id = self.upload_manifest_file(manifest, metadataManifestPath, datasetId, restrict, component_name)
-        
+        manifest_synapse_file_id = self.upload_manifest_file(
+            manifest, metadataManifestPath, datasetId, restrict, component_name
+        )
+
         # Set annotations for the file manifest.
-        manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
+        manifest_annotations = self.format_manifest_annotations(
+            manifest, manifest_synapse_file_id
+        )
         self.syn.set_annotations(manifest_annotations)
         logger.info("Associated manifest file with dataset on Synapse.")
-        
+
         # Update manifest Synapse table with new entity id column.
         manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
-                                                                dmge=dmge,
-                                                                manifest=manifest,
-                                                                datasetId=datasetId,
-                                                                table_name=table_name,
-                                                                restrict=restrict,
-                                                                useSchemaLabel=useSchemaLabel,
-                                                                table_manipulation='update')
+            dmge=dmge,
+            manifest=manifest,
+            datasetId=datasetId,
+            table_name=table_name,
+            restrict=restrict,
+            table_manipulation="update",
+            table_column_names=table_column_names,
+        )
 
         # Set annotations for the table manifest
-        manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_table_id)
+        manifest_annotations = self.format_manifest_annotations(
+            manifest, manifest_synapse_table_id
+        )
         self.syn.set_annotations(manifest_annotations)
         return manifest_synapse_file_id
 
     def associateMetadataWithFiles(
-        self, dmge: DataModelGraphExplorer, metadataManifestPath: str, datasetId: str, manifest_record_type: str = 'table_file_and_entities', 
-        useSchemaLabel: bool = True, hideBlanks: bool = False, restrict_manifest = False, table_manipulation: str = 'replace',
+        self,
+        dmge: DataModelGraphExplorer,
+        metadataManifestPath: str,
+        datasetId: str,
+        manifest_record_type: str = "table_file_and_entities",
+        hideBlanks: bool = False,
+        restrict_manifest=False,
+        table_manipulation: str = "replace",
+        table_column_names: str = "class_label",
+        annotation_keys: str = "class_label",
     ) -> str:
         """Associate metadata with files in a storage dataset already on Synapse.
         Upload metadataManifest in the storage dataset folder on Synapse as well. Return synapseId of the uploaded manifest file.
-        
+
         If this is a new manifest there could be no Synapse entities associated with the rows of this manifest
         this may be due to data type (e.g. clinical data) being tabular
         and not requiring files; to utilize uniform interfaces downstream
         (i.e. fileviews), a Synapse entity (a folder) is created for each row
         and an entity column is added to the manifest containing the resulting
         entity IDs; a table is also created at present as an additional interface
         for downstream query and interaction with the data.
@@ -1670,84 +1950,93 @@
             dmge: DataModelGraphExplorer Object
             metadataManifestPath: path to csv containing a validated metadata manifest.
             The manifest should include a column entityId containing synapse IDs of files/entities to be associated with metadata, if that is applicable to the dataset type.
             Some datasets, e.g. clinical data, do not contain file id's, but data is stored in a table: one row per item.
             In this case, the system creates a file on Synapse for each row in the table (e.g. patient, biospecimen) and associates the columnset data as metadata/annotations to his file.
             datasetId: synapse ID of folder containing the dataset
             manifest_record_type: Default value is 'table_file_and_entities'. valid values are 'file_only', 'file_and_entities', 'table_and_file' or 'table_file_and_entities'. 'file_and_entities' will store the manifest as a csv and create Synapse files for each row in the manifest.'table_and_file' will store the manifest as a table and a csv on Synapse. 'file_only' will store the manifest as a csv only on Synapse. 'table_file_and_entities' will perform the options file_with_entites and table in combination.
-            useSchemaLabel: Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
             hideBlanks: Default is false. Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
             restrict_manifest (bool): Default is false. Flag for censored data.
             table_malnipulation (str): Default is 'replace'. Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
+            table_column_names: (str): display_name/display_label/class_label (default). Sets labeling style for table column names. display_name will use the raw display name as the column name. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting.
+            annotation_keys: (str) display_label/class_label (default), Sets labeling syle for annotation keys. class_label will format the display
+                name as upper camelcase, and strip blacklisted characters, display_label will strip blacklisted characters including spaces, to retain
+                display label formatting while ensuring the label is formatted properly for Synapse annotations.
         Returns:
             manifest_synapse_file_id: SynID of manifest csv uploaded to synapse.
         """
         # Read new manifest CSV:
         manifest = self._read_manifest(metadataManifestPath)
         manifest = self._add_id_columns_to_manifest(manifest, dmge)
 
         table_name, component_name = self._generate_table_name(manifest)
 
         # Upload manifest to synapse based on user input (manifest_record_type)
-        
+
         if manifest_record_type == "file_only":
             manifest_synapse_file_id = self.upload_manifest_as_csv(
-                                        dmge,
-                                        manifest,
-                                        metadataManifestPath,
-                                        datasetId=datasetId,
-                                        restrict=restrict_manifest,
-                                        hideBlanks=hideBlanks,
-                                        manifest_record_type=manifest_record_type,
-                                        component_name = component_name,
-                                        )
+                dmge,
+                manifest,
+                metadataManifestPath,
+                datasetId=datasetId,
+                restrict=restrict_manifest,
+                hideBlanks=hideBlanks,
+                manifest_record_type=manifest_record_type,
+                component_name=component_name,
+                annotation_keys=annotation_keys,
+            )
         elif manifest_record_type == "table_and_file":
             manifest_synapse_file_id = self.upload_manifest_as_table(
-                                        dmge,
-                                        manifest,
-                                        metadataManifestPath,
-                                        datasetId=datasetId,
-                                        table_name=table_name,
-                                        component_name=component_name,
-                                        restrict=restrict_manifest,
-                                        useSchemaLabel=useSchemaLabel,
-                                        hideBlanks=hideBlanks,
-                                        manifest_record_type=manifest_record_type,
-                                        table_manipulation=table_manipulation,
-                                        )
+                dmge,
+                manifest,
+                metadataManifestPath,
+                datasetId=datasetId,
+                table_name=table_name,
+                component_name=component_name,
+                restrict=restrict_manifest,
+                hideBlanks=hideBlanks,
+                manifest_record_type=manifest_record_type,
+                table_manipulation=table_manipulation,
+                table_column_names=table_column_names,
+                annotation_keys=annotation_keys,
+            )
         elif manifest_record_type == "file_and_entities":
-            manifest_synapse_file_id = self.upload_manifest_as_csv( 
-                                        dmge,
-                                        manifest,
-                                        metadataManifestPath,
-                                        datasetId=datasetId,
-                                        restrict=restrict_manifest,
-                                        hideBlanks=hideBlanks,
-                                        manifest_record_type=manifest_record_type,
-                                        component_name = component_name,
-                                        )
+            manifest_synapse_file_id = self.upload_manifest_as_csv(
+                dmge,
+                manifest,
+                metadataManifestPath,
+                datasetId=datasetId,
+                restrict=restrict_manifest,
+                hideBlanks=hideBlanks,
+                manifest_record_type=manifest_record_type,
+                component_name=component_name,
+                annotation_keys=annotation_keys,
+            )
         elif manifest_record_type == "table_file_and_entities":
             manifest_synapse_file_id = self.upload_manifest_combo(
-                                        dmge,
-                                        manifest,
-                                        metadataManifestPath,
-                                        datasetId=datasetId,
-                                        table_name=table_name,
-                                        component_name=component_name,
-                                        restrict=restrict_manifest,
-                                        useSchemaLabel=useSchemaLabel,
-                                        hideBlanks=hideBlanks,
-                                        manifest_record_type=manifest_record_type,
-                                        table_manipulation=table_manipulation,
-                                        )
+                dmge,
+                manifest,
+                metadataManifestPath,
+                datasetId=datasetId,
+                table_name=table_name,
+                component_name=component_name,
+                restrict=restrict_manifest,
+                hideBlanks=hideBlanks,
+                manifest_record_type=manifest_record_type,
+                table_manipulation=table_manipulation,
+                table_column_names=table_column_names,
+                annotation_keys=annotation_keys,
+            )
         else:
             raise ValueError("Please enter a valid manifest_record_type.")
         return manifest_synapse_file_id
 
-    def getTableAnnotations(self, table_id:str):
+    def getTableAnnotations(self, table_id: str):
         """Generate dictionary of annotations for the given Synapse file.
         Synapse returns all custom annotations as lists since they
         can contain multiple values. In all cases, the values will
         be converted into strings and concatenated with ", ".
 
         Args:
             fileId (str): Synapse ID for dataset file.
@@ -1877,15 +2166,15 @@
             # Remove any annotations for non-file/folders (stored as None)
             records = filter(None, records)
             table = pd.DataFrame.from_records(records)
 
         # Add filenames for the files that "survived" annotation retrieval
         filenames = [dataset_files_map[i] for i in table["entityId"]]
 
-        if 'Filename' not in table.columns:
+        if "Filename" not in table.columns:
             table.insert(0, "Filename", filenames)
 
         # Ensure that entityId and eTag are at the end
         entity_ids = table.pop("entityId")
         etags = table.pop("eTag")
         table.insert(len(table.columns), "entityId", entity_ids)
         table.insert(len(table.columns), "eTag", etags)
@@ -1900,25 +2189,29 @@
     def raise_final_error(retry_state):
         return retry_state.outcome.result()
 
     def checkIfinAssetView(self, syn_id) -> str:
         # get data in administrative fileview for this pipeline
         assetViewTable = self.getStorageFileviewTable()
         all_files = list(assetViewTable["id"])
-        if syn_id in all_files: 
+        if syn_id in all_files:
             return True
-        else: 
+        else:
             return False
 
-    @retry(stop = stop_after_attempt(5), 
-            wait = wait_chain(*[wait_fixed(10) for i in range (2)] + 
-                    [wait_fixed(15) for i in range(2)] + 
-                    [wait_fixed(20)]),
-            retry=retry_if_exception_type(LookupError),
-            retry_error_callback = raise_final_error)
+    @retry(
+        stop=stop_after_attempt(5),
+        wait=wait_chain(
+            *[wait_fixed(10) for i in range(2)]
+            + [wait_fixed(15) for i in range(2)]
+            + [wait_fixed(20)]
+        ),
+        retry=retry_if_exception_type(LookupError),
+        retry_error_callback=raise_final_error,
+    )
     def getDatasetProject(self, datasetId: str) -> str:
         """Get parent project for a given dataset ID.
 
         Args:
             datasetId (str): Synapse entity ID (folder or project).
 
         Raises:
@@ -1937,15 +2230,14 @@
         if dataset_row.empty:
             sleep(5)
             self._query_fileview()
             # Subset main file view
             dataset_index = self.storageFileviewTable["id"] == datasetId
             dataset_row = self.storageFileviewTable[dataset_index]
 
-
         # Return `projectId` for given row if only one found
         if len(dataset_row) == 1:
             dataset_project = dataset_row["projectId"].values[0]
             return dataset_project
 
         # Otherwise, check if already project itself
         try:
@@ -1955,19 +2247,19 @@
         except SynapseHTTPError:
             raise PermissionError(
                 f"The given dataset ({datasetId}) isn't accessible with this "
                 "user. This might be caused by a typo in the dataset Synapse ID."
             )
 
         # If not, then assume dataset not in file view
-        raise LookupError (
+        raise LookupError(
             f"The given dataset ({datasetId}) doesn't appear in the "
             f"configured file view ({self.storageFileview}). This might "
             "mean that the file view's scope needs to be updated."
-        )     
+        )
 
     def getDatasetAnnotationsBatch(
         self, datasetId: str, dataset_file_ids: Sequence[str] = None
     ) -> pd.DataFrame:
         """Generate table for annotations across all files in given dataset.
         This function uses a temporary file view to generate a table
         instead of iteratively querying for individual entity annotations.
@@ -1990,334 +2282,396 @@
             table = table.loc[table.index.intersection(dataset_file_ids)]
 
         table = table.reset_index(drop=True)
 
         return table
 
     def _get_table_schema_by_cname(self, table_schema):
-
         # assume no duplicate column names in the table
         table_schema_by_cname = {}
 
         for col_record in table_schema:
-
-            #TODO clean up dictionary for compactness (e.g. remove redundant 'name' key)
+            # TODO clean up dictionary for compactness (e.g. remove redundant 'name' key)
             table_schema_by_cname[col_record["name"]] = col_record
 
         return table_schema_by_cname
 
+
 class TableOperations:
     """
     Object to hold functions for various table operations specific to the Synapse Asset Store.
-    
+
     Currently implement operations are:
     createTable: upload a manifest as a new table when none exist
     replaceTable: replace a metadata in a table from one manifest with metadata from another manifest
     updateTable: add a column to a table that already exists on synapse
 
     Operations currently in development are:
     upsertTable: add metadata from a manifest to an existing table that contains metadata from another manifest
     """
-    def __init__(self, 
-                 synStore: SynapseStorage, 
-                 tableToLoad: pd.DataFrame = None, 
-                 tableName: str = None, 
-                 datasetId: str = None, 
-                 existingTableId: str = None,
-                 restrict: bool = False
-                 ):
-        
+
+    def __init__(
+        self,
+        synStore: SynapseStorage,
+        tableToLoad: pd.DataFrame = None,
+        tableName: str = None,
+        datasetId: str = None,
+        existingTableId: str = None,
+        restrict: bool = False,
+    ):
         """
         Class governing table operations (creation, replacement, upserts, updates) in schematic
 
         tableToLoad: manifest formatted appropriately for the table
         tableName: name of the table to be uploaded
         datasetId: synID of the dataset for the manifest
         existingTableId: synId of the table currently exising on synapse (if there is one)
-        restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
+        restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions
 
         """
         self.synStore = synStore
         self.tableToLoad = tableToLoad
         self.tableName = tableName
         self.datasetId = datasetId
         self.existingTableId = existingTableId
         self.restrict = restrict
 
-
-    def createTable(self, columnTypeDict: dict = None, specifySchema: bool = True,):
+    def createTable(
+        self,
+        columnTypeDict: dict = None,
+        specifySchema: bool = True,
+    ):
         """
         Method to create a table from a metadata manifest and upload it to synapse
-        
+
         Args:
             columnTypeDict: dictionary schema for table columns: type, size, etc
-            specifySchema: to specify a specific schema for the table format                      
+            specifySchema: to specify a specific schema for the table format
 
         Returns:
             table.schema.id: synID of the newly created table
         """
 
-        datasetEntity = self.synStore.syn.get(self.datasetId, downloadFile = False)
+        datasetEntity = self.synStore.syn.get(self.datasetId, downloadFile=False)
         datasetName = datasetEntity.name
-        table_schema_by_cname = self.synStore._get_table_schema_by_cname(columnTypeDict) 
+        table_schema_by_cname = self.synStore._get_table_schema_by_cname(columnTypeDict)
 
         if not self.tableName:
-            self.tableName = datasetName + 'table'
+            self.tableName = datasetName + "table"
         datasetParentProject = self.synStore.getDatasetProject(self.datasetId)
         if specifySchema:
             if columnTypeDict == {}:
                 logger.error("Did not provide a columnTypeDict.")
-            #create list of columns:
+            # create list of columns:
             cols = []
             for col in self.tableToLoad.columns:
                 if col in table_schema_by_cname:
-                    col_type = table_schema_by_cname[col]['columnType']
-                    max_size = table_schema_by_cname[col]['maximumSize'] if 'maximumSize' in table_schema_by_cname[col].keys() else 100
+                    col_type = table_schema_by_cname[col]["columnType"]
+                    max_size = (
+                        table_schema_by_cname[col]["maximumSize"]
+                        if "maximumSize" in table_schema_by_cname[col].keys()
+                        else 100
+                    )
                     max_list_len = 250
                     if max_size and max_list_len:
-                        cols.append(Column(name=col, columnType=col_type, 
-                            maximumSize=max_size, maximumListLength=max_list_len))
+                        cols.append(
+                            Column(
+                                name=col,
+                                columnType=col_type,
+                                maximumSize=max_size,
+                                maximumListLength=max_list_len,
+                            )
+                        )
                     elif max_size:
-                        cols.append(Column(name=col, columnType=col_type, 
-                            maximumSize=max_size))
+                        cols.append(
+                            Column(name=col, columnType=col_type, maximumSize=max_size)
+                        )
                     else:
                         cols.append(Column(name=col, columnType=col_type))
                 else:
-                    #TODO add warning that the given col was not found and it's max size is set to 100
-                    cols.append(Column(name=col, columnType='STRING', maximumSize=100))
-            schema = Schema(name=self.tableName, columns=cols, parent=datasetParentProject)
+                    # TODO add warning that the given col was not found and it's max size is set to 100
+                    cols.append(Column(name=col, columnType="STRING", maximumSize=100))
+            schema = Schema(
+                name=self.tableName, columns=cols, parent=datasetParentProject
+            )
             table = Table(schema, self.tableToLoad)
-            table = self.synStore.syn.store(table, isRestricted = self.restrict)
+            table = self.synStore.syn.store(table, isRestricted=self.restrict)
             return table.schema.id
         else:
             # For just uploading the tables to synapse using default
             # column types.
             table = build_table(self.tableName, datasetParentProject, self.tableToLoad)
-            table = self.synStore.syn.store(table, isRestricted = self.restrict)
+            table = self.synStore.syn.store(table, isRestricted=self.restrict)
             return table.schema.id
 
-    def replaceTable(self, specifySchema: bool = True, columnTypeDict: dict = None,):
+    def replaceTable(
+        self,
+        specifySchema: bool = True,
+        columnTypeDict: dict = None,
+    ):
         """
         Method to replace an existing table on synapse with metadata from a new manifest
-        
+
         Args:
-            specifySchema: to infer a schema for the table format      
-            columnTypeDict: dictionary schema for table columns: type, size, etc            
+            specifySchema: to infer a schema for the table format
+            columnTypeDict: dictionary schema for table columns: type, size, etc
 
         Returns:
            existingTableId: synID of the already existing table that had its metadata replaced
         """
-        datasetEntity = self.synStore.syn.get(self.datasetId, downloadFile = False)
+        datasetEntity = self.synStore.syn.get(self.datasetId, downloadFile=False)
         datasetName = datasetEntity.name
-        table_schema_by_cname = self.synStore._get_table_schema_by_cname(columnTypeDict) 
-        existing_table, existing_results = self.synStore.get_synapse_table(self.existingTableId)
+        table_schema_by_cname = self.synStore._get_table_schema_by_cname(columnTypeDict)
+        existing_table, existing_results = self.synStore.get_synapse_table(
+            self.existingTableId
+        )
         # remove rows
         self.synStore.syn.delete(existing_results)
         # wait for row deletion to finish on synapse before getting empty table
         sleep(10)
-        
+
         # removes all current columns
         current_table = self.synStore.syn.get(self.existingTableId)
         current_columns = self.synStore.syn.getTableColumns(current_table)
         for col in current_columns:
             current_table.removeColumn(col)
 
         if not self.tableName:
-            self.tableName = datasetName + 'table'
-        
+            self.tableName = datasetName + "table"
+
         # Process columns according to manifest entries
-        table_schema_by_cname = self.synStore._get_table_schema_by_cname(columnTypeDict) 
+        table_schema_by_cname = self.synStore._get_table_schema_by_cname(columnTypeDict)
         datasetParentProject = self.synStore.getDatasetProject(self.datasetId)
         if specifySchema:
             if columnTypeDict == {}:
                 logger.error("Did not provide a columnTypeDict.")
-            #create list of columns:
+            # create list of columns:
             cols = []
-            
+
             for col in self.tableToLoad.columns:
-                
                 if col in table_schema_by_cname:
-                    col_type = table_schema_by_cname[col]['columnType']
-                    max_size = table_schema_by_cname[col]['maximumSize'] if 'maximumSize' in table_schema_by_cname[col].keys() else 100
+                    col_type = table_schema_by_cname[col]["columnType"]
+                    max_size = (
+                        table_schema_by_cname[col]["maximumSize"]
+                        if "maximumSize" in table_schema_by_cname[col].keys()
+                        else 100
+                    )
                     max_list_len = 250
                     if max_size and max_list_len:
-                        cols.append(Column(name=col, columnType=col_type, 
-                            maximumSize=max_size, maximumListLength=max_list_len))
+                        cols.append(
+                            Column(
+                                name=col,
+                                columnType=col_type,
+                                maximumSize=max_size,
+                                maximumListLength=max_list_len,
+                            )
+                        )
                     elif max_size:
-                        cols.append(Column(name=col, columnType=col_type, 
-                            maximumSize=max_size))
+                        cols.append(
+                            Column(name=col, columnType=col_type, maximumSize=max_size)
+                        )
                     else:
                         cols.append(Column(name=col, columnType=col_type))
                 else:
-                    
-                    #TODO add warning that the given col was not found and it's max size is set to 100
-                    cols.append(Column(name=col, columnType='STRING', maximumSize=100))
-            
+                    # TODO add warning that the given col was not found and it's max size is set to 100
+                    cols.append(Column(name=col, columnType="STRING", maximumSize=100))
+
             # adds new columns to schema
             for col in cols:
                 current_table.addColumn(col)
-            self.synStore.syn.store(current_table, isRestricted = self.restrict)
+            self.synStore.syn.store(current_table, isRestricted=self.restrict)
 
             # wait for synapse store to finish
             sleep(1)
 
             # build schema and table from columns and store with necessary restrictions
-            schema = Schema(name=self.tableName, columns=cols, parent=datasetParentProject)
+            schema = Schema(
+                name=self.tableName, columns=cols, parent=datasetParentProject
+            )
             schema.id = self.existingTableId
-            table = Table(schema, self.tableToLoad, etag = existing_results.etag)
-            table = self.synStore.syn.store(table, isRestricted = self.restrict)
+            table = Table(schema, self.tableToLoad, etag=existing_results.etag)
+            table = self.synStore.syn.store(table, isRestricted=self.restrict)
         else:
             logging.error("Must specify a schema for table replacements")
 
         # remove system metadata from manifest
-        existing_table.drop(columns = ['ROW_ID', 'ROW_VERSION'], inplace = True)
+        existing_table.drop(columns=["ROW_ID", "ROW_VERSION"], inplace=True)
         return self.existingTableId
-    
 
-    def _get_auth_token(self,):
+    def _get_auth_token(
+        self,
+    ):
         authtoken = None
 
         # Get access token from environment variable if available
         # Primarily useful for testing environments, with other possible usefulness for containers
         env_access_token = os.getenv("SYNAPSE_ACCESS_TOKEN")
         if env_access_token:
             authtoken = env_access_token
             return authtoken
 
         # Get token from authorization header
         # Primarily useful for API endpoint functionality
-        if 'Authorization' in self.synStore.syn.default_headers:
-            authtoken = self.synStore.syn.default_headers['Authorization'].split('Bearer ')[-1]
+        if "Authorization" in self.synStore.syn.default_headers:
+            authtoken = self.synStore.syn.default_headers["Authorization"].split(
+                "Bearer "
+            )[-1]
             return authtoken
 
         # retrive credentials from synapse object
         # Primarily useful for local users, could only be stored here when a .synapseConfig file is used, but including to be safe
         synapse_object_creds = self.synStore.syn.credentials
-        if hasattr(synapse_object_creds, '_token'):
+        if hasattr(synapse_object_creds, "_token"):
             authtoken = synapse_object_creds.secret
 
         # Try getting creds from .synapseConfig file if it exists
         # Primarily useful for local users. Seems to correlate with credentials stored in synaspe object when logged in
         if os.path.exists(CONFIG.synapse_configuration_path):
             config = self.synStore.syn.getConfigFile(CONFIG.synapse_configuration_path)
 
             # check which credentials are provided in file
-            if config.has_option('authentication', 'authtoken'):
-                authtoken = config.get('authentication', 'authtoken')
-        
+            if config.has_option("authentication", "authtoken"):
+                authtoken = config.get("authentication", "authtoken")
+
         # raise error if required credentials are not found
         if not authtoken:
             raise NameError(
                 "authtoken credentials could not be found in the environment, synapse object, or the .synapseConfig file"
             )
-        
+
         return authtoken
 
     def upsertTable(self, dmge: DataModelGraphExplorer):
         """
         Method to upsert rows from a new manifest into an existing table on synapse
-        For upsert functionality to work, primary keys must follow the naming convention of <componenet>_id        
+        For upsert functionality to work, primary keys must follow the naming convention of <componenet>_id
         `-tm upsert` should be used for initial table uploads if users intend to upsert into them at a later time; using 'upsert' at creation will generate the metadata necessary for upsert functionality.
         Currently it is required to use -dl/--use_display_label with table upserts.
-        
+
 
         Args:
             dmge: DataModelGraphExplorer instance
-            
+
         Returns:
            existingTableId: synID of the already existing table that had its metadata replaced
-        """            
+        """
 
         authtoken = self._get_auth_token()
 
-        synapseDB = SynapseDatabase(auth_token=authtoken, project_id=self.synStore.getDatasetProject(self.datasetId))
+        synapseDB = SynapseDatabase(
+            auth_token=authtoken,
+            project_id=self.synStore.getDatasetProject(self.datasetId),
+        )
 
         try:
             # Try performing upsert
-            synapseDB.upsert_table_rows(table_name=self.tableName, data=self.tableToLoad)
-        except(SynapseHTTPError) as ex:
+            synapseDB.upsert_table_rows(
+                table_name=self.tableName, data=self.tableToLoad
+            )
+        except SynapseHTTPError as ex:
             # If error is raised because Table has old `Uuid` column and not new `Id` column, then handle and re-attempt upload
-            if 'Id is not a valid column name or id' in str(ex):
+            if "Id is not a valid column name or id" in str(ex):
                 self._update_table_uuid_column(dmge)
-                synapseDB.upsert_table_rows(table_name=self.tableName, data=self.tableToLoad)
+                synapseDB.upsert_table_rows(
+                    table_name=self.tableName, data=self.tableToLoad
+                )
             # Raise if other error
             else:
                 raise ex
 
         return self.existingTableId
-    
-    def _update_table_uuid_column(self, dmge: DataModelGraphExplorer,) -> None:
+
+    def _update_table_uuid_column(
+        self,
+        dmge: DataModelGraphExplorer,
+    ) -> None:
         """Removes the `Uuid` column when present, and relpaces with an `Id` column
         Used to enable backwards compatability for manifests using the old `Uuid` convention
 
         Args:
             dmge: DataModelGraphExplorer instance
 
         Returns:
             None
         """
 
         # Get the columns of the schema
         schema = self.synStore.syn.get(self.existingTableId)
         cols = self.synStore.syn.getTableColumns(schema)
-        
+
         # Iterate through columns until `Uuid` column is found
         for col in cols:
-            if col.name.lower() == 'uuid':
+            if col.name.lower() == "uuid":
                 # See if schema has `Uuid` column specified
                 try:
-                    uuid_col_in_schema = dmge.is_class_in_schema(col.name)      
-                except (KeyError):
+                    uuid_col_in_schema = dmge.is_class_in_schema(col.name)
+                except KeyError:
                     uuid_col_in_schema = False
 
                 # If there is, then create a new `Id` column from scratch
                 if uuid_col_in_schema:
-                    new_col = Column(columnType = "STRING", maximumSize = 64, name = "Id")
+                    new_col = Column(columnType="STRING", maximumSize=64, name="Id")
                     schema.addColumn(new_col)
                     schema = self.synStore.syn.store(schema)
                 # If there is not, then use the old `Uuid` column as a basis for the new `Id` column
                 else:
-                    
                     # Build ColumnModel that will be used for new column
-                    id_column = Column(name='Id', columnType='STRING', maximumSize=64, defaultValue=None, maximumListLength=1)
+                    id_column = Column(
+                        name="Id",
+                        columnType="STRING",
+                        maximumSize=64,
+                        defaultValue=None,
+                        maximumListLength=1,
+                    )
                     new_col_response = self.synStore.syn.store(id_column)
 
-
                     # Define columnChange body
                     columnChangeDict = {
                         "concreteType": "org.sagebionetworks.repo.model.table.TableSchemaChangeRequest",
                         "entityId": self.existingTableId,
                         "changes": [
-                            {                        
-                                "oldColumnId": col['id'],
-                                "newColumnId": new_col_response['id'],
+                            {
+                                "oldColumnId": col["id"],
+                                "newColumnId": new_col_response["id"],
                             }
-                        ]
+                        ],
                     }
 
-                    self.synStore.syn._async_table_update(table=self.existingTableId, changes=[columnChangeDict], wait=False)
+                    self.synStore.syn._async_table_update(
+                        table=self.existingTableId,
+                        changes=[columnChangeDict],
+                        wait=False,
+                    )
                 break
 
         return
 
-    def updateTable(self, update_col: str = 'Id',):
+    def updateTable(
+        self,
+        update_col: str = "Id",
+    ):
         """
         Method to update an existing table with a new column
-        
+
         Args:
-            updateCol: column to index the old and new tables on            
+            updateCol: column to index the old and new tables on
 
         Returns:
            existingTableId: synID of the already existing table that had its metadata replaced
         """
-        existing_table, existing_results = self.synStore.get_synapse_table(self.existingTableId)
-        
+        existing_table, existing_results = self.synStore.get_synapse_table(
+            self.existingTableId
+        )
+
         self.tableToLoad = update_df(existing_table, self.tableToLoad, update_col)
         # store table with existing etag data and impose restrictions as appropriate
-        self.synStore.syn.store(Table(self.existingTableId, self.tableToLoad, etag = existing_results.etag), isRestricted = self.restrict)
+        self.synStore.syn.store(
+            Table(self.existingTableId, self.tableToLoad, etag=existing_results.etag),
+            isRestricted=self.restrict,
+        )
 
         return self.existingTableId
 
 
 class DatasetFileView:
     """Helper class to create temporary dataset file views.
     This class can be used in conjunction with a 'with' statement.
```

### Comparing `schematicpy-24.1.1/schematic/utils/cli_utils.py` & `schematicpy-24.2.1/schematic/utils/cli_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-#!/usr/bin/env python3
+"""CLI utils"""
+
+# pylint: disable=logging-fstring-interpolation
+# pylint: disable=anomalous-backslash-in-string
 
-import inspect
 import logging
 
-from typing import Any, Mapping, Sequence, Union, List
+from typing import Any, Mapping, Sequence, Union, Optional
 from functools import reduce
 import re
 
 logger = logging.getLogger(__name__)
 
-# We are using fstrings in logger methods
-# pylint: disable=logging-fstring-interpolation
-
 
 def query_dict(dictionary: Mapping[Any, Any], keys: Sequence[Any]) -> Union[Any, None]:
     """Access a nested value in a dictionary corresponding
     to a series of keys.
 
     Args:
         dictionary: A dictionary containing anything.
@@ -32,63 +31,72 @@
         if dictionary is None or not isinstance(dictionary, dict):
             return None
         return dictionary.get(key)
 
     return reduce(extract, keys, dictionary)
 
 
-def log_value_from_config(arg_name: str, config_value: Any):
+def log_value_from_config(arg_name: str, config_value: Any) -> None:
     """Logs when getting a value from the config
 
     Args:
         arg_name (str): Name of the argument. Used for logging.
         config_value (Any): The value in the config
     """
     logger.info(
         f"The {arg_name} argument is being taken from configuration file, i.e., {config_value}."
     )
 
-def parse_synIDs(
-    ctx, param, synIDs,
-) -> List[str]:
-    """Parse and validate a comma separated string of synIDs
 
-    Args:
-        ctx:
-            click option context
-        param:
-            click option argument name
-        synIDs:
-            comma separated string of synIDs
+def parse_syn_ids(
+    ctx: Any,  # pylint: disable=unused-argument
+    param: str,  # pylint: disable=unused-argument
+    syn_ids: str,
+) -> Optional[list[str]]:
+    """Parse and validate a comma separated string of synapse ids
 
-    Returns:
-        List of synID strings
+    Args:
+        ctx (Any): click option context
+        param (str): click option argument name
+        syn_ids (str): comma separated string of synapse ids
 
     Raises:
-        ValueError: If the entire string does not match a regex for 
+        ValueError:  If the entire string does not match a regex for
             a valid comma separated string of SynIDs
+
+    Returns:
+        Optional[list[str]]:  List of synapse ids
     """
-    if synIDs:
-        project_regex = re.compile("(syn\d+\,?)+")
-        valid=project_regex.fullmatch(synIDs)
-
-        if valid:
-            synIDs = synIDs.split(",")
-
-            return synIDs
-
-        else:
-            raise ValueError(
-                        f"The provided list of project synID(s): {synIDs}, is not formatted correctly. "
-                        "\nPlease check your list of projects for errors."
-                    )
-    else:
-        return
+    if not syn_ids:
+        return None
+
+    project_regex = re.compile("(syn\d+\,?)+")
+    valid = project_regex.fullmatch(syn_ids)
+
+    if not valid:
+        raise ValueError(
+            f"The provided list of project synID(s): {syn_ids}, is not formatted correctly. "
+            "\nPlease check your list of projects for errors."
+        )
+
+    return syn_ids.split(",")
+
 
 def parse_comma_str_to_list(
-    ctx, param, comma_string,
-) -> List[str]:
+    ctx: Any,  # pylint: disable=unused-argument
+    param: str,  # pylint: disable=unused-argument
+    comma_string: str,
+) -> Optional[list[str]]:
+    """Separates a comma separated sting into a list of strings
+
+    Args:
+        ctx (Any): click option context
+        param (str): click option argument name
+        comma_string (str): comma separated string
+
+    Returns:
+        Optional[list[str]]: _description_
+    """
+    if not comma_string:
+        return None
 
-    if comma_string:
-        return comma_string.split(",")
-    else:
-        return None
+    return comma_string.split(",")
```

### Comparing `schematicpy-24.1.1/schematic/utils/curie_utils.py` & `schematicpy-24.2.1/schematic/utils/curie_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,74 @@
+"""Curie utils"""
+
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
-def extract_name_from_uri_or_curie(item):
+def extract_name_from_uri_or_curie(item: str) -> str:
     """Extract name from uri or curie"""
     if "http" not in item and len(item.split(":")) == 2:
         return item.split(":")[-1]
-    elif len(item.split("//")[-1].split("/")) > 1:
+    if len(item.split("//")[-1].split("/")) > 1:
         return item.split("//")[-1].split("/")[-1]
-    else:
-        raise ValueError("Error extracting name from URI or Curie.")
+    raise ValueError("Error extracting name from URI or Curie.")
 
 
-def expand_curie_to_uri(curie, context_info):
+def expand_curie_to_uri(curie: str, context_info: dict[str, str]) -> str:
     """Expand curie to uri based on the context given
 
     parmas
     ======
     curie: curie to be expanded (e.g. bts:BiologicalEntity)
     context_info: jsonld context specifying prefix-uri relation (e.g. {"bts":
     "http://schema.biothings.io/"})
     """
     # as suggested in SchemaOrg standard file, these prefixes don't expand
-    PREFIXES_NOT_EXPAND = ["rdf", "rdfs", "xsd"]
+    prefixes_not_expand = ["rdf", "rdfs", "xsd"]
     # determine if a value is curie
     if len(curie.split(":")) == 2:
         prefix, value = curie.split(":")
-        if prefix in context_info and prefix not in PREFIXES_NOT_EXPAND:
+        if prefix in context_info and prefix not in prefixes_not_expand:
             return context_info[prefix] + value
         # if the input is not curie, return the input unmodified
-        else:
-            return curie
-    else:
         return curie
+    return curie
 
 
 def expand_curies_in_schema(schema):
     """Expand all curies in a SchemaOrg JSON-LD file into URI"""
     context = schema["@context"]
     graph = schema["@graph"]
     new_schema = {"@context": context, "@graph": [], "@id": schema["@id"]}
     for record in graph:
         new_record = {}
-        for k, v in record.items():
-            if type(v) == str:
-                new_record[expand_curie_to_uri(k, context)] = expand_curie_to_uri(
-                    v, context
+        for key, value in record.items():
+            if isinstance(value, str):
+                new_record[expand_curie_to_uri(key, context)] = expand_curie_to_uri(
+                    value, context
                 )
-            elif type(v) == list:
-                if type(v[0]) == dict:
-                    new_record[expand_curie_to_uri(k, context)] = []
-                    for _item in v:
-                        new_record[expand_curie_to_uri(k, context)].append(
+            elif isinstance(value, list):
+                if isinstance(value[0], dict):
+                    new_record[expand_curie_to_uri(key, context)] = []
+                    for _item in value:
+                        new_record[expand_curie_to_uri(key, context)].append(
                             {"@id": expand_curie_to_uri(_item["@id"], context)}
                         )
                 else:
-                    new_record[expand_curie_to_uri(k, context)] = [
-                        expand_curie_to_uri(_item, context) for _item in v
+                    new_record[expand_curie_to_uri(key, context)] = [
+                        expand_curie_to_uri(_item, context) for _item in value
                     ]
-            elif type(v) == dict and "@id" in v:
-                new_record[expand_curie_to_uri(k, context)] = {
-                    "@id": expand_curie_to_uri(v["@id"], context)
+            elif isinstance(value, dict) and "@id" in value:
+                new_record[expand_curie_to_uri(key, context)] = {
+                    "@id": expand_curie_to_uri(value["@id"], context)
                 }
-            elif v == None:
-                new_record[expand_curie_to_uri(k, context)] = None
+            elif value is None:
+                new_record[expand_curie_to_uri(key, context)] = None
         new_schema["@graph"].append(new_record)
     return new_schema
 
 
 def uri2label(uri, schema):
     """Given a URI, return the label"""
     return [
```

### Comparing `schematicpy-24.1.1/schematic/utils/general.py` & `schematicpy-24.2.1/schematic/utils/general.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,242 +1,316 @@
-# allows specifying explicit variable types
+"""General utils"""
+
+# pylint: disable=logging-fstring-interpolation
+
 import logging
-import math
 import os
 import pstats
 import subprocess
 import tempfile
 from cProfile import Profile
 from datetime import datetime, timedelta
 from functools import wraps
-from typing import Union
-
-from synapseclient.core.exceptions import SynapseHTTPError
-from synapseclient.entity import File, Folder, Project
-from synapseclient.table import EntityViewSchema
+from typing import Union, TypeVar, Any, Optional, Sequence, Callable
 
-import synapseclient.core.cache as cache
+from synapseclient.core.exceptions import SynapseHTTPError  # type: ignore
+from synapseclient.entity import File, Folder, Project  # type: ignore
+from synapseclient.table import EntityViewSchema  # type: ignore
+from synapseclient.core import cache  # type: ignore
+from synapseclient import Synapse  # type: ignore
 
 logger = logging.getLogger(__name__)
 
-def find_duplicates(_list):
+T = TypeVar("T")
+
+
+def find_duplicates(_list: list[T]) -> set[T]:
     """Find duplicate items in a list"""
-    return set([x for x in _list if _list.count(x) > 1])
+    return {x for x in _list if _list.count(x) > 1}
 
 
-def dict2list(dictionary):
-    if type(dictionary) == list:
-        return dictionary
-    elif type(dictionary) == dict:
-        return [dictionary]
+def dict2list(item: Any) -> Optional[Union[dict, list]]:
+    """Puts a dictionary into a list
 
+    Args:
+        item (Any): Any type of input
 
-def str2list(_str):
-    if type(_str) == str:
-        return [_str]
-    elif type(_str) == list:
-        return _str
+    Returns:
+        Optional[Union[dict, list]]:
+          If input is a list, return it
+          If input is a dict, return it in a list
+          Return None for anything else
+    """
+    if isinstance(item, list):
+        return item
+    if isinstance(item, dict):
+        return [item]
+    return None
 
 
-def unlist(_list):
-    if len(_list) == 1:
-        return _list[0]
-    else:
-        return _list
+def str2list(item: Any) -> Optional[list]:
+    """Puts a string into a list
 
+    Args:
+        item (Any): Any type of input
+
+    Returns:
+        Optional[list]:
+          If input is a list, return it
+          If input is a string, return it in a list
+          Return None for anything else
+    """
+    if isinstance(item, str):
+        return [item]
+    if isinstance(item, list):
+        return item
+    return None
+
+
+def unlist(seq: Sequence) -> Any:
+    """Returns the first item of a sequence
 
-def get_dir_size(path: str):
-    """Recursively descend the directory tree rooted at the top and call .st_size function to calculate size of files in bytes. 
+    Args:
+        seq (Sequence): Any sequence
+
+    Returns:
+        Any:
+          if sequence is length one, return the first item
+          otherwise return the sequence
+    """
+    if len(seq) == 1:
+        return seq[0]
+    return seq
+
+
+def get_dir_size(path: str) -> int:
+    """
+    Recursively descend the directory tree rooted at the top and call
+      .st_size function to calculate size of files in bytes.
     Args:
         path: path to a folder
-    return: total size of all the files in a given directory in bytes. 
+    return: total size of all the files in a given directory in bytes.
     """
     total = 0
     # Recursively scan directory to find entries
-    with os.scandir(path) as it:
-        for entry in it:
+    with os.scandir(path) as itr:
+        for entry in itr:
             if entry.is_file():
                 total += entry.stat().st_size
             elif entry.is_dir():
                 total += get_dir_size(entry.path)
     return total
 
-def calculate_datetime(minutes: int, input_date: datetime, before_or_after: str = "before") -> datetime:
-    """calculate date time 
+
+def calculate_datetime(
+    minutes: int, input_date: datetime, before_or_after: str = "before"
+) -> datetime:
+    """calculate date time
 
     Args:
         input_date (datetime): date time object provided by users
         minutes (int): number of minutes
-        before_or_after (str): default to "before". if "before", calculate x minutes before current date time. if "after", calculate x minutes after current date time. 
+        before_or_after (str): default to "before". if "before", calculate x minutes before
+         current date time. if "after", calculate x minutes after current date time.
 
     Returns:
         datetime:  return result of date time calculation
     """
-    if before_or_after=="before": 
+    if before_or_after == "before":
         date_time_result = input_date - timedelta(minutes=minutes)
-    elif before_or_after=="after":
+    elif before_or_after == "after":
         date_time_result = input_date + timedelta(minutes=minutes)
     else:
         raise ValueError("Invalid value. Use either 'before' or 'after'.")
     return date_time_result
 
 
-def check_synapse_cache_size(directory='/root/.synapseCache')-> Union[float, int]:
+def check_synapse_cache_size(
+    directory: str = "/root/.synapseCache",
+) -> Union[float, int]:
     """use du --sh command to calculate size of .synapseCache.
 
     Args:
         directory (str, optional): .synapseCache directory. Defaults to '/root/.synapseCache'
 
     Returns:
         float or integer: returns size of .synapsecache directory in bytes
     """
-    # Note: this command might fail on windows user. But since this command is primarily for running on AWS, it is fine. 
-    command = ['du', '-sh', directory]
-    output = subprocess.run(command, capture_output=True).stdout.decode('utf-8')
-    
+    # Note: this command might fail on windows user.
+    # But since this command is primarily for running on AWS, it is fine.
+    command = ["du", "-sh", directory]
+    output = subprocess.run(command, capture_output=True, check=False).stdout.decode(
+        "utf-8"
+    )
+
     # Parsing the output to extract the directory size
-    size = output.split('\t')[0]
+    size = output.split("\t")[0]
     if "K" in size:
-        size_in_kb = float(size.rstrip('K'))
+        size_in_kb = float(size.rstrip("K"))
         byte_size = size_in_kb * 1000
     elif "M" in size:
-        size_in_mb = float(size.rstrip('M'))
+        size_in_mb = float(size.rstrip("M"))
         byte_size = size_in_mb * 1000000
-    elif "G" in size: 
-        size_in_gb = float(size.rstrip('G'))
+    elif "G" in size:
+        size_in_gb = float(size.rstrip("G"))
         byte_size = convert_gb_to_bytes(size_in_gb)
     elif "B" in size:
-        byte_size = float(size.rstrip('B'))
+        byte_size = float(size.rstrip("B"))
     else:
-        logger.error('Cannot recongize the file size unit')
+        logger.error("Cannot recongize the file size unit")
     return byte_size
 
-def clear_synapse_cache(cache: cache.Cache, minutes: int) -> int:
+
+def clear_synapse_cache(synapse_cache: cache.Cache, minutes: int) -> int:
     """clear synapse cache before a certain time
 
     Args:
-        cache: an object of synapseclient Cache.
+        synapse_cache: an object of synapseclient Cache.
         minutes (int): all files before this minute will be removed
     Returns:
         int: number of files that get deleted
     """
     current_date = datetime.utcnow()
-    minutes_earlier = calculate_datetime(input_date=current_date, minutes=minutes, before_or_after="before")
-    num_of_deleted_files = cache.purge(before_date = minutes_earlier)
+    minutes_earlier = calculate_datetime(
+        input_date=current_date, minutes=minutes, before_or_after="before"
+    )
+    num_of_deleted_files = synapse_cache.purge(before_date=minutes_earlier)
     return num_of_deleted_files
 
-def convert_gb_to_bytes(gb: int):
+
+def convert_gb_to_bytes(g_bytes: int) -> int:
     """convert gb to bytes
     Args:
-        gb: number of gb
+        g_bytes: number of gb
     return: total number of bytes
     """
-    return gb * 1024 * 1024 * 1024
+    return g_bytes * 1024 * 1024 * 1024
 
 
-def entity_type_mapping(syn, entity_id):
-    """
-    Return the entity type of manifest
+def entity_type_mapping(syn: Synapse, entity_id: str) -> str:
+    """Return the entity type of manifest
+
     Args:
-        entity_id: id of an entity
-    Return:
-        type_entity: type of the manifest being returned
+        syn (Synapse): Synapse object
+        entity_id (str): id of an entity
+
+    Raises:
+        SynapseHTTPError: Re-raised SynapseHTTPError
+
+    Returns:
+        str: type of the manifest being returned
     """
     # check the type of entity
     try:
         entity = syn.get(entity_id, downloadFile=False)
-    except SynapseHTTPError as e:
+    except SynapseHTTPError as exc:
         logger.error(
             f"cannot get {entity_id} from asset store. Please make sure that {entity_id} exists"
         )
         raise SynapseHTTPError(
             f"cannot get {entity_id} from asset store. Please make sure that {entity_id} exists"
-        ) from e
+        ) from exc
 
     if isinstance(entity, EntityViewSchema):
-        return "asset view"
+        entity_type = "asset view"
     elif isinstance(entity, Folder):
-        return "folder"
+        entity_type = "folder"
     elif isinstance(entity, File):
-        return "file"
+        entity_type = "file"
     elif isinstance(entity, Project):
-        return "project"
+        entity_type = "project"
     else:
         # if there's no matching type, return concreteType
-        return entity.concreteType
+        entity_type = entity.concreteType
+    return entity_type
+
 
 def create_temp_folder(path: str) -> str:
-    """This function creates a temporary directory in the specified directory 
+    """This function creates a temporary directory in the specified directory
     Args:
         path(str): a directory path where all the temporary files will live
     Returns: returns the absolute pathname of the new directory.
     """
     # Create a temporary directory in the specified directory
     path = tempfile.mkdtemp(dir=path)
     return path
 
 
-def profile(output_file=None, sort_by='cumulative', lines_to_print=None, strip_dirs=False):
+def profile(
+    output_file: Optional[str] = None,
+    sort_by: Any = "cumulative",
+    lines_to_print: Optional[int] = None,
+    strip_dirs: bool = False,
+) -> Callable:
     """
-    The function was initially taken from: https://towardsdatascience.com/how-to-profile-your-code-in-python-e70c834fad89
+    The function was initially taken from:
+    https://towardsdatascience.com/how-to-profile-your-code-in-python-e70c834fad89
     A time profiler decorator.
     Inspired by and modified the profile decorator of Giampaolo Rodola:
     http://code.activestate.com/recipes/577817-profile-decorator/
+
     Args:
-        output_file: str or None. Default is None
+        output_file (Optional[str], optional):
             Path of the output file. If only name of the file is given, it's
             saved in the current directory.
             If it's None, the name of the decorated function is used.
-        sort_by: str or SortKey enum or tuple/list of str/SortKey enum
+            Defaults to None.
+        sort_by (str, optional):
+            str or SortKey enum or tuple/list of str/SortKey enum
             Sorting criteria for the Stats object.
             For a list of valid string and SortKey refer to:
             https://docs.python.org/3/library/profile.html#pstats.Stats.sort_stats
-        lines_to_print: int or None
-            Number of lines to print. Default (None) is for all the lines.
+            Defaults to "cumulative".
+        lines_to_print (Optional[int], optional):
+            Number of lines to print.
             This is useful in reducing the size of the printout, especially
             that sorting by 'cumulative', the time consuming operations
             are printed toward the top of the file.
-        strip_dirs: bool
+            Default (None) is for all the lines.
+        strip_dirs (bool, optional):
             Whether to remove the leading path info from file names.
             This is also useful in reducing the size of the printout
+            Defaults to False.
+
     Returns:
-        Profile of the decorated function
+        Callable: Profile of the decorated function
     """
 
     def inner(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
-            _output_file = output_file or func.__name__ + '.prof'
-            pr = Profile()
-            pr.enable()
+            _output_file = output_file or func.__name__ + ".prof"
+            profiler = Profile()
+            profiler.enable()
             retval = func(*args, **kwargs)
-            pr.disable()
-            pr.dump_stats(_output_file)
+            profiler.disable()
+            profiler.dump_stats(_output_file)
 
-            #if we are running the functions on AWS: 
+            # if we are running the functions on AWS:
             if "SECRETS_MANAGER_SECRETS" in os.environ:
-                ps = pstats.Stats(pr)
+                p_stats = pstats.Stats(profiler)
                 # limit this to 30 line for now otherwise it will be too long for AWS log
-                ps.sort_stats('cumulative').print_stats(30)
-            else: 
-                with open(_output_file, 'w') as f:
-                    ps = pstats.Stats(pr, stream=f)
+                p_stats.sort_stats("cumulative").print_stats(30)
+            else:
+                with open(_output_file, "w", encoding="utf-8") as fle:
+                    p_stats = pstats.Stats(profiler, stream=fle)
                     if strip_dirs:
-                        ps.strip_dirs()
+                        p_stats.strip_dirs()
                     if isinstance(sort_by, (tuple, list)):
-                        ps.sort_stats(*sort_by)
+                        p_stats.sort_stats(*sort_by)
                     else:
-                        ps.sort_stats(sort_by)
-                    ps.print_stats(lines_to_print)
+                        p_stats.sort_stats(sort_by)
+                    p_stats.print_stats(lines_to_print)
             return retval
 
         return wrapper
 
     return inner
 
+
 def normalize_path(path: str, parent_folder: str) -> str:
     """
     Normalizes a path.
     If the path is relative, the parent_folder is added to make it an absolute path.
 
     Args:
         path (str): The path to the file to normalize.
```

### Comparing `schematicpy-24.1.1/schematic/utils/io_utils.py` & `schematicpy-24.2.1/schematic/utils/io_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-import os
+"""io utils"""
+
+from typing import Any
 import json
 import urllib.request
-
 from schematic import LOADER
 
 
-def load_json(file_path):
+def load_json(file_path: str) -> Any:
     """Load json document from file path or url
 
     :arg str file_path: The path of the url doc, could be url or file path
     """
     if file_path.startswith("http"):
         with urllib.request.urlopen(file_path) as url:
             data = json.loads(url.read().decode())
             return data
     # handle file path
     else:
-        with open(file_path, encoding="utf8") as f:
-            data = json.load(f)
+        with open(file_path, encoding="utf8") as fle:
+            data = json.load(fle)
             return data
 
 
-def export_json(json_doc, file_path):
+def export_json(json_doc: Any, file_path: str) -> None:
     """Export JSON doc to file"""
-    with open(file_path, "w", encoding="utf8") as f:
-        json.dump(json_doc, f, sort_keys=True, indent=4, ensure_ascii=False)
+    with open(file_path, "w", encoding="utf8") as fle:
+        json.dump(json_doc, fle, sort_keys=True, indent=4, ensure_ascii=False)
 
 
-def load_default():
+def load_default() -> Any:
     """Load biolink vocabulary"""
     data_path = "data_models/biothings.model.jsonld"
     biothings_path = LOADER.filename(data_path)
-
     return load_json(biothings_path)
 
 
-def load_schemaorg():
-    """Load SchemOrg vocabulary"""
+def load_schemaorg() -> Any:
+    """Load SchemaOrg vocabulary"""
     data_path = "data_models/schema_org.model.jsonld"
-    schemaorg_path = LOADER.filename(data_path)
-
-    return load_json(schemaorg_path)
+    schema_org_path = LOADER.filename(data_path)
+    return load_json(schema_org_path)
```

### Comparing `schematicpy-24.1.1/schematic/utils/validate_utils.py` & `schematicpy-24.2.1/schematic/utils/validate_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,105 @@
-import os
-import pandas as pd
+"""Validation utils"""
+
+# pylint: disable = anomalous-backslash-in-string
+
+import re
+from collections.abc import Mapping
+from typing import Pattern, Union, Iterable, Any, Optional
+from numbers import Number
 from jsonschema import validate
-from re import compile, search, IGNORECASE
+import numpy as np
+import pandas as pd
 from schematic.utils.io_utils import load_json
 from schematic import LOADER
-from typing import List
-import numpy as np
-from numbers import Number
 
-def validate_schema(schema):
+
+def validate_schema(schema: Union[Mapping, bool]) -> None:
     """Validate schema against schema.org standard"""
     data_path = "validation_schemas/model.schema.json"
     json_schema_path = LOADER.filename(data_path)
     json_schema = load_json(json_schema_path)
     return validate(schema, json_schema)
 
 
-def validate_property_schema(schema):
+def validate_property_schema(schema: Union[Mapping, bool]) -> None:
     """Validate schema against SchemaORG property definition standard"""
     data_path = "validation_schemas/property.schema.json"
     json_schema_path = LOADER.filename(data_path)
     json_schema = load_json(json_schema_path)
     return validate(schema, json_schema)
 
 
-def validate_class_schema(schema):
+def validate_class_schema(schema: Union[Mapping, bool]) -> None:
     """Validate schema against SchemaORG class definition standard"""
     data_path = "validation_schemas/class.schema.json"
     json_schema_path = LOADER.filename(data_path)
     json_schema = load_json(json_schema_path)
     return validate(schema, json_schema)
 
-def comma_separated_list_regex():
-    # Regex to match with comma separated list 
-    # Requires at least one element and a comma to be valid 
-    # Does not require a trailing comma
-    csv_list_regex=compile('([^\,]+\,)(([^\,]+\,?)*)')
+
+def comma_separated_list_regex() -> Pattern[str]:
+    """
+    Regex to match with comma separated list
+    Requires at least one element and a comma to be valid
+    Does not require a trailing comma
+
+    Returns:
+        Pattern[str]:
+    """
+    csv_list_regex = re.compile("([^\,]+\,)(([^\,]+\,?)*)")
 
     return csv_list_regex
 
-def rule_in_rule_list(rule: str, rule_list: List[str]):
-    # Function to standardize 
-    # checking to see if a rule is contained in a list of rules. 
-    # Uses regex to avoid issues arising from validation rules with arguments 
-    # or rules that have arguments updated.
 
-    # seperate rule type if arguments are specified
+def rule_in_rule_list(rule: str, rule_list: list[str]) -> Optional[re.Match[str]]:
+    """
+    Function to standardize
+    checking to see if a rule is contained in a list of rules.
+    Uses regex to avoid issues arising from validation rules with arguments
+    or rules that have arguments updated.
+    """
+    # separate rule type if arguments are specified
     rule_type = rule.split(" ")[0]
 
     # Process string and list of strings for regex comparison
-    rule_type = rule_type + '[^\|]*'
-    rule_list = '|'.join(rule_list)
+    rule_type = rule_type + "[^\|]*"
+    rule_list_str = "|".join(rule_list)
+    return re.search(rule_type, rule_list_str, flags=re.IGNORECASE)
 
-    return search(rule_type, rule_list, flags=IGNORECASE)
 
-def parse_str_series_to_list(col: pd.Series):
+def parse_str_series_to_list(col: pd.Series) -> pd.Series:
     """
     Parse a pandas series of comma delimited strings
-    into a series with values that are lists of strings 
-    ex. 
+    into a series with values that are lists of strings
+    ex.
         Input:  'a,b,c'
-        Output: ['a','b','c']     
+        Output: ['a','b','c']
 
     """
-    col = col.apply(
-        lambda x: [s.strip() for s in str(x).split(",")]
-    )
+    col = col.apply(lambda x: [s.strip() for s in str(x).split(",")])
 
     return col
 
-def np_array_to_str_list(np_array):
+
+def np_array_to_str_list(np_array: Any) -> list[str]:
     """
     Parse a numpy array of ints to a list of strings
     """
-    return np.char.mod('%d', np_array).tolist()
+    return np.char.mod("%d", np_array).tolist()
 
-def iterable_to_str_list(iterable):
+
+def iterable_to_str_list(obj: Union[str, Number, Iterable]) -> list[str]:
     """
     Parse an object into a list of strings
     Accepts str, Number, and iterable inputs
     """
 
     # If object is a string, just return wrapped as a list
-    if isinstance(iterable, str):
-        return [iterable]
-    # If object is numberical, convert to string and wrap as a list
-    elif isinstance(iterable, Number):
-        return [str(iterable)]
-    # If the object is iterable and not a string, convert every element to string and wratp as a list
-    else:
-        strlist = []
-        for element in iterable:
-            strlist.append(str(element))
-
-    return strlist
-    
+    if isinstance(obj, str):
+        return [obj]
+    # If object is numerical, convert to string and wrap as a list
+    if isinstance(obj, Number):
+        return [str(obj)]
+    # If the object is iterable and not a string, convert every element
+    # to string and wrap as a list
+    return [str(item) for item in obj]
```

### Comparing `schematicpy-24.1.1/schematic/visualization/attributes_explorer.py` & `schematicpy-24.2.1/schematic/visualization/attributes_explorer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,227 +1,294 @@
-import gc
+"""Attributes Explorer Class"""
 import json
 import logging
-import numpy as np
 import os
+
+import numpy as np
 import pandas as pd
-from typing import Any, Dict, Optional, Text, List
 
 from schematic.schemas.data_model_parser import DataModelParser
 from schematic.schemas.data_model_graph import DataModelGraph, DataModelGraphExplorer
 from schematic.schemas.data_model_json_schema import DataModelJSONSchema
-
 from schematic.utils.io_utils import load_json
 
 logger = logging.getLogger(__name__)
 
-class AttributesExplorer():
-    def __init__(self,
-                 path_to_jsonld: str,
-                 )-> None:
-        
+
+class AttributesExplorer:
+    """AttributesExplorer class"""
+
+    def __init__(
+        self,
+        path_to_jsonld: str,
+        data_model_labels: str,
+    ) -> None:
         self.path_to_jsonld = path_to_jsonld
 
         self.jsonld = load_json(self.path_to_jsonld)
 
         # Instantiate Data Model Parser
-        data_model_parser = DataModelParser(path_to_data_model = self.path_to_jsonld)
-        
-        #Parse Model
+        data_model_parser = DataModelParser(
+            path_to_data_model=self.path_to_jsonld,
+        )
+
+        # Parse Model
         parsed_data_model = data_model_parser.parse_model()
 
         # Instantiate DataModelGraph
-        data_model_grapher = DataModelGraph(parsed_data_model)
+        data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
         # Generate graph
         self.graph_data_model = data_model_grapher.generate_data_model_graph()
 
         # Instantiate Data Model Graph Explorer
         self.dmge = DataModelGraphExplorer(self.graph_data_model)
 
         # Instantiate Data Model Json Schema
-        self.data_model_js = DataModelJSONSchema(jsonld_path=self.path_to_jsonld, graph=self.graph_data_model)
-        
-        self.output_path = self.create_output_path('merged_csv')
-    
-    def create_output_path(self, terminal_folder):
-        ''' Create output path to store Observable visualization data if it does not already exist.
-        
+        self.data_model_js = DataModelJSONSchema(
+            jsonld_path=self.path_to_jsonld, graph=self.graph_data_model
+        )
+
+        self.output_path = self.create_output_path("merged_csv")
+
+    def create_output_path(self, terminal_folder: str) -> str:
+        """Create output path to store Observable visualization data if it does not already exist.
+
         Args: self.path_to_jsonld
-        
-        Returns: output_path (str): path to store outputs 
-        '''
+
+        Returns: output_path (str): path to store outputs
+        """
         base_dir = os.path.dirname(self.path_to_jsonld)
-        self.schema_name = self.path_to_jsonld.split('/')[-1].split('.model.jsonld')[0]
-        output_path = os.path.join(base_dir, 'visualization', self.schema_name, terminal_folder)
+        self.schema_name = self.path_to_jsonld.split("/")[-1].split(".model.jsonld")[0]
+        output_path = os.path.join(
+            base_dir, "visualization", self.schema_name, terminal_folder
+        )
         if not os.path.exists(output_path):
             os.makedirs(output_path)
         return output_path
 
-    def convert_string_cols_to_json(self, df: pd.DataFrame, cols_to_modify: list):
-        """Converts values in a column from strings to JSON list 
+    def convert_string_cols_to_json(
+        self, dataframe: pd.DataFrame, cols_to_modify: list[str]
+    ) -> pd.DataFrame:
+        """Converts values in a column from strings to JSON list
         for upload to Synapse.
         """
-        for col in df.columns:
+        for col in dataframe.columns:
             if col in cols_to_modify:
-                df[col] = df[col].apply(lambda x: json.dumps([y.strip() for y in x]) if x != "NaN" and x  and x == np.nan else x)
-        return df
+                dataframe[col] = dataframe[col].apply(
+                    lambda x: json.dumps([y.strip() for y in x])
+                    if x != "NaN" and x and x == np.nan
+                    else x
+                )
+        return dataframe
 
-    def parse_attributes(self, save_file=True):
-        '''
+    def parse_attributes(self, save_file: bool = True) -> pd.DataFrame:
+        """
         Args: save_file (bool):
                 True: merged_df is saved locally to output_path.
                 False: merged_df is returned.
 
         Returns:
             merged_df (pd.DataFrame): dataframe containing data relating to attributes
-                for the provided data model for all components in the data model. 
+                for the provided data model for all components in the data model.
                 Dataframe is saved locally as a csv if save_file == True, or returned if
-                save_file == False. 
-                
-        '''
+                save_file == False.
+
+        """
         # get all components
-        component_dg = self.dmge.get_digraph_by_edge_type('requiresComponent')
+        component_dg = self.dmge.get_digraph_by_edge_type("requiresComponent")
         components = component_dg.nodes()
-        
-        # For each data type to be loaded gather all attribtes the user would
+
+        # For each data type to be loaded gather all attributes the user would
         # have to provide.
         return self._parse_attributes(components, save_file)
-    
-    def parse_component_attributes(self, component=None, save_file=True, include_index=True):
-        '''
+
+    def parse_component_attributes(
+        self, component=None, save_file: bool = True, include_index: bool = True
+    ) -> pd.DataFrame:
+        """
         Args: save_file (bool):
                 True: merged_df is saved locally to output_path.
                 False: merged_df is returned.
               include_index (bool):
                 Whether to include the index in the returned dataframe (True) or not (False)
 
         Returns:
             merged_df (pd.DataFrame): dataframe containing data relating to attributes
-                for the provided data model for the specified component in the data model. 
+                for the provided data model for the specified component in the data model.
                 Dataframe is saved locally as a csv if save_file == True, or returned if
-                save_file == False. 
-        '''        
+                save_file == False.
+        """
 
         if not component:
             raise ValueError("You must provide a component to visualize.")
-        else:
-            return self._parse_attributes([component], save_file, include_index)
+        return self._parse_attributes([component], save_file, include_index)
 
-    def _parse_attributes(self, components, save_file=True, include_index=True):
-        '''
+    def _parse_attributes(
+        self, components: list, save_file=True, include_index=True
+    ) -> pd.DataFrame:
+        """
         Args: save_file (bool):
                 True: merged_df is saved locally to output_path.
                 False: merged_df is returned.
               components (list):
                 list of components to parse attributes for
               include_index (bool):
                 Whether to include the index in the returned dataframe (True) or not (False)
 
         Returns:
             merged_df (pd.DataFrame): dataframe containing data relating to attributes
-                for the provided data model for specified components in the data model. 
+                for the provided data model for specified components in the data model.
                 Dataframe is saved locally as a csv if save_file == True, or returned if
-                save_file == False. 
+                save_file == False.
         Raises:
             ValueError:
-                If unable hits an error while attempting to get conditional requirements. 
+                If unable hits an error while attempting to get conditional requirements.
                 This error is likely to be found if there is a mismatch in naming.
-        '''
-        
-        # For each data type to be loaded gather all attribtes the user would
+        """
+        # This function needs to be refactored, temporarily disabling some pylint errors
+        # pylint: disable=too-many-locals
+        # pylint: disable=too-many-nested-blocks
+        # pylint: disable=too-many-branches
+        # pylint: disable=too-many-statements
+
+        # For each data type to be loaded gather all attributes the user would
         # have to provide.
         df_store = []
         for component in components:
-            data_dict = {}
+            data_dict: dict = {}
 
             # get the json schema
-            json_schema = self.data_model_js.get_json_validation_schema(source_node=component, schema_name=self.path_to_jsonld)
+            json_schema = self.data_model_js.get_json_validation_schema(
+                source_node=component, schema_name=self.path_to_jsonld
+            )
 
-            # Gather all attribues, their valid values and requirements
-            for key, value in json_schema['properties'].items():
+            # Gather all attributes, their valid values and requirements
+            for key, value in json_schema["properties"].items():
                 data_dict[key] = {}
-                for k, v in value.items():
-                    if k == 'enum':
-                        data_dict[key]['Valid Values'] = value['enum']
-                if key in json_schema['required']:
-                    data_dict[key]['Required'] = True
+                for inner_key in value.keys():
+                    if inner_key == "enum":
+                        data_dict[key]["Valid Values"] = value["enum"]
+                if key in json_schema["required"]:
+                    data_dict[key]["Required"] = True
                 else:
-                    data_dict[key]['Required'] = False
-                data_dict[key]['Component'] = component
+                    data_dict[key]["Required"] = False
+                data_dict[key]["Component"] = component
             # Add additional details per key (from the JSON-ld)
-            for dic in self.jsonld['@graph']:
-                if 'sms:displayName' in dic.keys():
-                    key = dic['sms:displayName']
-                    if key in data_dict.keys():
-                        data_dict[key]['Attribute'] = dic['sms:displayName']
-                        data_dict[key]['Label'] = dic['rdfs:label']
-                        data_dict[key]['Description'] = dic['rdfs:comment']
-                        if 'validationRules' in dic.keys():
-                            data_dict[key]['Validation Rules'] = dic['validationRules']
+            for dic in self.jsonld["@graph"]:
+                if "sms:displayName" in dic:
+                    key = dic["sms:displayName"]
+                    if key in data_dict:
+                        data_dict[key]["Attribute"] = dic["sms:displayName"]
+                        data_dict[key]["Label"] = dic["rdfs:label"]
+                        data_dict[key]["Description"] = dic["rdfs:comment"]
+                        if "validationRules" in dic.keys():
+                            data_dict[key]["Validation Rules"] = dic["validationRules"]
             # Find conditional dependencies
-            if 'allOf' in json_schema.keys():
-                for conditional_dependencies in json_schema['allOf']:
-                    key = list(conditional_dependencies['then']['properties'])[0]
+            if "allOf" in json_schema:
+                for conditional_dependencies in json_schema["allOf"]:
+                    key = list(conditional_dependencies["then"]["properties"])[0]
                     try:
-                        if key in data_dict.keys():
-                            if 'Cond_Req' not in data_dict[key].keys():
-                                data_dict[key]['Cond_Req'] = []
-                                data_dict[key]['Conditional Requirements'] = []
-                            attribute = list(conditional_dependencies['if']['properties'])[0]
-                            value = conditional_dependencies['if']['properties'][attribute]['enum']
-                            # Capitalize attribute if it begins with a lowercase letter, for aesthetics.
+                        if key in data_dict:
+                            if "Cond_Req" not in data_dict[key].keys():
+                                data_dict[key]["Cond_Req"] = []
+                                data_dict[key]["Conditional Requirements"] = []
+                            attribute = list(
+                                conditional_dependencies["if"]["properties"]
+                            )[0]
+                            value = conditional_dependencies["if"]["properties"][
+                                attribute
+                            ]["enum"]
+                            # Capitalize attribute if it begins with a lowercase
+                            # letter, for aesthetics.
                             if attribute[0].islower():
                                 attribute = attribute.capitalize()
 
-                            # Remove "Type" (i.e. turn "Biospecimen Type" to "Biospcimen")
-                            if "Type" in attribute: 
+                            # Remove "Type" (i.e. turn "Biospecimen Type" to "Biospecimen")
+                            if "Type" in attribute:
                                 attribute = attribute.split(" ")[0]
-                            
+
                             # Remove "Type" (i.e. turn "Tissue Type" to "Tissue")
                             if "Type" in value[0]:
                                 value[0] = value[0].split(" ")[0]
 
                             conditional_statement = f'{attribute} is "{value[0]}"'
-                            if conditional_statement not in data_dict[key]['Conditional Requirements']:
-                                data_dict[key]['Cond_Req'] = True
-                                data_dict[key]['Conditional Requirements'].extend([conditional_statement])
-                    except:
+                            if (
+                                conditional_statement
+                                not in data_dict[key]["Conditional Requirements"]
+                            ):
+                                data_dict[key]["Cond_Req"] = True
+                                data_dict[key]["Conditional Requirements"].extend(
+                                    [conditional_statement]
+                                )
+                    except Exception as exc:
                         raise ValueError(
-                            f"There is an error getting conditional requirements related "
-                            "to the attribute: {key}. The error is likely caused by naming inconsistencies (e.g. uppercase, camelcase, ...)"
-                        )
-
-            for key, value in data_dict.items():
-                if 'Conditional Requirements' in value.keys():
-
-                    ## reformat conditional requirement 
-
-                    # get all attributes 
-                    attr_lst = [i.split(" is ")[-1] for i in data_dict[key]['Conditional Requirements']]
-                    
-                    # join a list of attributes by using OR 
+                            (
+                                "There is an error getting conditional requirements related "
+                                f"to the attribute: {key}. The error is likely caused by naming "
+                                "inconsistencies (e.g. uppercase, camelcase, ...)"
+                            )
+                        ) from exc
+
+            for outer_dict_key, inner_dict in data_dict.items():
+                if "Conditional Requirements" in inner_dict.keys():
+                    ## reformat conditional requirement
+                    conditional_requirements = inner_dict["Conditional Requirements"]
+
+                    # get all attributes
+                    attr_lst = [i.split(" is ")[-1] for i in conditional_requirements]
+
+                    # join a list of attributes by using OR
                     attr_str = " OR ".join(attr_lst)
 
-                    # reformat the conditional requirement 
-                    component_name = data_dict[key]['Conditional Requirements'][0].split(' is ')[0]
-                    conditional_statement_str = f' If {component_name} is {attr_str} then "{key}" is required'
-
-                    data_dict[key]['Conditional Requirements'] = conditional_statement_str
-            df = pd.DataFrame(data_dict)
-            df = df.T
-            cols = ['Attribute', 'Label', 'Description', 'Required', 'Cond_Req', 'Valid Values', 'Conditional Requirements', 'Validation Rules', 'Component']
-            cols = [col for col in cols if col in df.columns]
-            df = df[cols]
-            df = self.convert_string_cols_to_json(df, ['Valid Values'])
-            #df.to_csv(os.path.join(csv_output_path, data_type + '.vis_data.csv'))
-            df_store.append(df)
+                    # reformat the conditional requirement
+                    component_name = conditional_requirements[0].split(" is ")[0]
 
-        merged_attributes_df = pd.concat(df_store, join='outer')
-        cols = ['Attribute', 'Label', 'Description', 'Required', 'Cond_Req', 'Valid Values', 'Conditional Requirements', 'Validation Rules', 'Component']
+                    conditional_statement_str = (
+                        f" If {component_name} is {attr_str} then "
+                        f'"{outer_dict_key}" is required'
+                    )
+                    conditional_requirements = conditional_statement_str
+
+            data_dict_df = pd.DataFrame(data_dict)
+            data_dict_df = data_dict_df.T
+            cols = [
+                "Attribute",
+                "Label",
+                "Description",
+                "Required",
+                "Cond_Req",
+                "Valid Values",
+                "Conditional Requirements",
+                "Validation Rules",
+                "Component",
+            ]
+            cols = [col for col in cols if col in data_dict_df.columns]
+            data_dict_df = data_dict_df[cols]
+            data_dict_df = self.convert_string_cols_to_json(
+                data_dict_df, ["Valid Values"]
+            )
+            df_store.append(data_dict_df)
+
+        merged_attributes_df = pd.concat(df_store, join="outer")
+        cols = [
+            "Attribute",
+            "Label",
+            "Description",
+            "Required",
+            "Cond_Req",
+            "Valid Values",
+            "Conditional Requirements",
+            "Validation Rules",
+            "Component",
+        ]
         cols = [col for col in cols if col in merged_attributes_df.columns]
 
         merged_attributes_df = merged_attributes_df[cols]
-        if save_file == True:
-            return merged_attributes_df.to_csv(os.path.join(self.output_path, self.schema_name + 'attributes_data.vis_data.csv'), index=include_index)
-        elif save_file == False:
-            return merged_attributes_df.to_csv(index=include_index)
+        if save_file:
+            return merged_attributes_df.to_csv(
+                os.path.join(
+                    self.output_path, self.schema_name + "attributes_data.vis_data.csv"
+                ),
+                index=include_index,
+            )
+        return merged_attributes_df.to_csv(index=include_index)
```

### Comparing `schematicpy-24.1.1/schematic/visualization/commands.py` & `schematicpy-24.2.1/schematic/visualization/commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,163 @@
-#!/usr/bin/env python3
+"""visualization commands"""
+# pylint: disable=unused-argument
+# pylint: disable=useless-return
+# pylint: disable=unused-variable
+# pylint: disable=logging-fstring-interpolation
 
 import logging
 import sys
+from typing import Any
 
 import click
-import click_log
+import click_log  # type: ignore
 
 from schematic.visualization.attributes_explorer import AttributesExplorer
 from schematic.visualization.tangled_tree import TangledTree
 from schematic.utils.cli_utils import log_value_from_config, query_dict
+from schematic.utils.schema_utils import DisplayLabelType
 from schematic.help import viz_commands
 from schematic.help import model_commands
 from schematic.configuration.configuration import CONFIG
 
 logger = logging.getLogger(__name__)
 click_log.basic_config(logger)
 
-CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
+CONTEXT_SETTINGS = {"help_option_names": ["--help", "-h"]}  # help options
 
-# invoke_without_command=True -> forces the application not to show aids before losing them with a --h
+
+# invoke_without_command=True -> forces the application not to show aids before
+# losing them with a --h
 @click.group(context_settings=CONTEXT_SETTINGS, invoke_without_command=True)
 @click_log.simple_verbosity_option(logger)
 @click.option(
     "-c",
     "--config",
     type=click.Path(),
     envvar="SCHEMATIC_CONFIG",
     help=query_dict(model_commands, ("model", "config")),
 )
 @click.pass_context
-def viz(ctx, config):  # use as `schematic model ...`
+def viz(ctx: Any, config: str) -> None:  # use as `schematic model ...`
     """
     Sub-commands for Visualization methods.
     """
     try:
         logger.debug(f"Loading config file contents in '{config}'")
         CONFIG.load_config(config)
-        ctx.obj =  CONFIG
-    except ValueError as e:
+        ctx.obj = CONFIG
+    except ValueError as exc:
         logger.error("'--config' not provided or environment variable not set.")
-        logger.exception(e)
+        logger.exception(exc)
         sys.exit(1)
 
+
 @viz.command(
     "attributes",
 )
 @click_log.simple_verbosity_option(logger)
-
+@click.option(
+    "--data_model_labels",
+    "-dml",
+    default="class_label",
+    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    help=query_dict(
+        viz_commands, ("visualization", "tangled_tree", "data_model_labels")
+    ),
+)
 @click.pass_obj
-def get_attributes(ctx):
-    """
-    
-    """
+def get_attributes(
+    ctx: Any,
+    data_model_labels: DisplayLabelType,
+) -> None:
+    """Gets attributes"""
     # Get JSONLD file path
     path_to_jsonld = CONFIG.model_location
     log_value_from_config("jsonld", path_to_jsonld)
     # Run attributes explorer
-    AttributesExplorer(path_to_jsonld).parse_attributes(save_file=True)
+    AttributesExplorer(path_to_jsonld, data_model_labels).parse_attributes(
+        save_file=True
+    )
     return
 
-@viz.command(
-    "tangled_tree_text"
-)
+
+@viz.command("tangled_tree_text")
 @click_log.simple_verbosity_option(logger)
 @click.option(
     "-ft",
     "--figure_type",
-    type=click.Choice(['component', 'dependency'], case_sensitive=False),
+    required=True,
+    type=click.Choice(["component", "dependency"], case_sensitive=False),
     help=query_dict(viz_commands, ("visualization", "tangled_tree", "figure_type")),
 )
 @click.option(
     "-tf",
     "--text_format",
-    type=click.Choice(['plain', 'highlighted'], case_sensitive=False),
+    required=True,
+    type=click.Choice(["plain", "highlighted"], case_sensitive=False),
     help=query_dict(viz_commands, ("visualization", "tangled_tree", "text_format")),
 )
-
+@click.option(
+    "--data_model_labels",
+    "-dml",
+    default="class_label",
+    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    help=query_dict(
+        viz_commands, ("visualization", "tangled_tree", "data_model_labels")
+    ),
+)
 @click.pass_obj
-def get_tangled_tree_text(ctx, figure_type, text_format):
-    """ Get text to be placed on the tangled tree visualization.
-    """
+def get_tangled_tree_text(
+    ctx: Any,
+    figure_type: str,
+    text_format: str,
+    data_model_labels: DisplayLabelType,
+) -> None:
+    """Get text to be placed on the tangled tree visualization."""
     # Get JSONLD file path
     path_to_jsonld = CONFIG.model_location
     log_value_from_config("jsonld", path_to_jsonld)
-    
+
     # Initialize TangledTree
-    tangled_tree = TangledTree(path_to_jsonld, figure_type)
+    tangled_tree = TangledTree(path_to_jsonld, figure_type, data_model_labels)
 
     # Get text for tangled tree.
     text_df = tangled_tree.get_text_for_tangled_tree(text_format, save_file=True)
     return
 
-@viz.command(
-    "tangled_tree_layers"
-)
+
+@viz.command("tangled_tree_layers")
 @click_log.simple_verbosity_option(logger)
 @click.option(
     "-ft",
     "--figure_type",
-    type=click.Choice(['component', 'dependency'], case_sensitive=False),
+    required=True,
+    type=click.Choice(["component", "dependency"], case_sensitive=False),
     help=query_dict(viz_commands, ("visualization", "tangled_tree", "figure_type")),
 )
-
+@click.option(
+    "--data_model_labels",
+    "-dml",
+    default="class_label",
+    type=click.Choice(["display_label", "class_label"], case_sensitive=True),
+    help=query_dict(
+        viz_commands, ("visualization", "tangled_tree", "data_model_labels")
+    ),
+)
 @click.pass_obj
-def get_tangled_tree_component_layers(ctx, figure_type):
-    ''' Get the components that belong in each layer of the tangled tree visualization.
-    '''
+def get_tangled_tree_component_layers(
+    ctx: Any,
+    figure_type: str,
+    data_model_labels: DisplayLabelType,
+) -> None:
+    """Get the components that belong in each layer of the tangled tree visualization."""
     # Get JSONLD file path
     path_to_jsonld = CONFIG.model_location
     log_value_from_config("jsonld", path_to_jsonld)
-    
+
     # Initialize Tangled Tree
-    tangled_tree = TangledTree(path_to_jsonld, figure_type)
-    
+    tangled_tree = TangledTree(path_to_jsonld, figure_type, data_model_labels)
+
     # Get tangled trees layers JSON.
     layers = tangled_tree.get_tangled_tree_layers(save_file=True)
 
     return
```

### Comparing `schematicpy-24.1.1/schematic/visualization/tangled_tree.py` & `schematicpy-24.2.1/schematic/visualization/tangled_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,818 +1,971 @@
+"""Tangled tree class"""
+
+# pylint: disable=logging-fstring-interpolation
+
 from io import StringIO
 import json
 import logging
-import networkx as nx
-import numpy as np
 import os
 from os import path
-import pandas as pd
+from typing import Optional, Any, Literal
 
-# allows specifying explicit variable types
-from typing import Any, Dict, Optional, Text, List
+import networkx as nx  # type: ignore
+from networkx.classes.reportviews import NodeView, EdgeDataView  # type: ignore
+import numpy as np
+import pandas as pd
 
-from schematic.utils.viz_utils import visualize
 from schematic.visualization.attributes_explorer import AttributesExplorer
-
 from schematic.schemas.data_model_parser import DataModelParser
 from schematic.schemas.data_model_graph import DataModelGraph, DataModelGraphExplorer
-from schematic.schemas.data_model_relationships import DataModelRelationships
-
-from schematic import LOADER
 from schematic.utils.io_utils import load_json
-from copy import deepcopy
-
-# Make sure to have newest version of decorator
+from schematic.utils.schema_utils import DisplayLabelType
 
 
 logger = logging.getLogger(__name__)
-#OUTPUT_DATA_DIR = str(Path('tests/data/visualization/AMPAD').resolve())
-#DATA_DIR = str(Path('tests/data').resolve())
 
-class TangledTree(object):
-    """
-    """
-
-    def __init__(self,
-                 path_to_json_ld: str,
-                 figure_type: str,
-                 ) -> None:
+
+class TangledTree:  # pylint: disable=too-many-instance-attributes
+    """Tangled tree class"""
+
+    def __init__(
+        self,
+        path_to_json_ld: str,
+        figure_type: str,
+        data_model_labels: DisplayLabelType,
+    ) -> None:
         # Load jsonld
         self.path_to_json_ld = path_to_json_ld
         self.json_data_model = load_json(self.path_to_json_ld)
 
         # Parse schema name
         self.schema_name = path.basename(self.path_to_json_ld).split(".model.jsonld")[0]
 
         # Instantiate Data Model Parser
-        data_model_parser = DataModelParser(path_to_data_model = self.path_to_json_ld)
-        
-        #Parse Model
+        data_model_parser = DataModelParser(
+            path_to_data_model=self.path_to_json_ld,
+        )
+
+        # Parse Model
         parsed_data_model = data_model_parser.parse_model()
 
         # Instantiate DataModelGraph
-        data_model_grapher = DataModelGraph(parsed_data_model)
+        data_model_grapher = DataModelGraph(parsed_data_model, data_model_labels)
 
         # Generate graph
         self.graph_data_model = data_model_grapher.generate_data_model_graph()
 
         # Instantiate Data Model Graph Explorer
         self.dmge = DataModelGraphExplorer(self.graph_data_model)
 
         # Set Parameters
         self.figure_type = figure_type.lower()
-        self.dependency_type = ''.join(('requires', self.figure_type.capitalize()))
+        self.dependency_type = "".join(("requires", self.figure_type.capitalize()))
 
         # Get names
         self.schema = load_json(self.path_to_json_ld)
-        self.schema_abbr = self.schema_name.split('_')[0]
+        self.schema_abbr = self.schema_name.split("_")[0]
 
         # Initialize AttributesExplorer
-        self.ae = AttributesExplorer(self.path_to_json_ld)
+        self.attributes_explorer = AttributesExplorer(
+            self.path_to_json_ld, data_model_labels
+        )
 
         # Create output paths.
-        self.text_csv_output_path = self.ae.create_output_path('text_csv')
-        self.json_output_path = self.ae.create_output_path('tangled_tree_json')
+        self.text_csv_output_path = self.attributes_explorer.create_output_path(
+            "text_csv"
+        )
+        self.json_output_path = self.attributes_explorer.create_output_path(
+            "tangled_tree_json"
+        )
 
-    def strip_double_quotes(self, string):
+    def strip_double_quotes(self, string: str) -> str:
+        """Removes double quotes from string
+
+        Args:
+            string (str): The string to remove quotes from
+
+        Returns:
+            str: The processed string
+        """
         # Remove double quotes from beginning and end of string.
         if string.startswith('"') and string.endswith('"'):
             string = string[1:-1]
         # now remove whitespace
         string = "".join(string.split())
         return string
 
-    def get_text_for_tangled_tree(self, text_type, save_file=False):
-        '''Gather the text that needs to be either higlighted or plain for the tangled tree visualization.
+    def get_text_for_tangled_tree(
+        self, text_type: Literal["highlighted", "plain"], save_file: bool = False
+    ) -> Optional[str]:
+        """
+        Gather the text that needs to be either highlighted or plain for the
+          tangled tree visualization.
         Args:
             text_type (str): Choices = ['highlighted', 'plain'], determines the type of text
                 rendering to return.
             save_file (bool): Determines if the outputs should be saved to disk or returned.
         Returns:
             If save_file==True: Saves plain or highlighted text as a CSV (to disk).
                save_file==False: Returns plain or highlighted text as a csv string.
-        '''
+        """
+        # pylint: disable=too-many-locals
         # Get nodes in the digraph, many more nodes returned if figure type is dependency
         cdg = self.dmge.get_digraph_by_edge_type(self.dependency_type)
         nodes = cdg.nodes()
 
-        if self.dependency_type == 'requiresComponent':
+        if self.dependency_type == "requiresComponent":
             component_nodes = nodes
         else:
             # get component nodes if making dependency figure
-            component_dg = self.dmge.get_digraph_by_edge_type('requiresComponent')
+            component_dg = self.dmge.get_digraph_by_edge_type("requiresComponent")
             component_nodes = component_dg.nodes()
 
         # Initialize lists
         highlighted = []
         plain = []
 
-        # For each component node in the tangled tree gather the plain and higlighted text.
+        # For each component node in the tangled tree gather the plain and highlighted text.
         for node in component_nodes:
             # Get the highlighted components based on figure_type
-            if self.figure_type == 'component':
-                highlight_descendants = self.dmge.get_descendants_by_edge_type(node, 'requiresComponent')
-            elif self.figure_type == 'dependency':
+            if self.figure_type == "component":
+                highlight_descendants = self.dmge.get_descendants_by_edge_type(
+                    node, "requiresComponent"
+                )
+            elif self.figure_type == "dependency":
                 highlight_descendants = [node]
 
-            
-            # Format text to be higlighted and gather text to be formated plain.
+            # Format text to be highlighted and gather text to be formatted plain.
             if not highlight_descendants:
-                # If there are no highlighted descendants just highlight the selected node (format for observable.)
+                # If there are no highlighted descendants just highlight the selected
+                # node (format for observable.)
                 highlighted.append([node, "id", node])
                 # Gather all the text as plain text.
                 plain_descendants = [n for n in nodes if n != node]
             else:
-                # Format higlighted text for Observable.
-                for hd in highlight_descendants:
-                    highlighted.append([node, "id", hd])
-                # Gather the non-higlighted text as plain text descendants.
-                plain_descendants = [node for node in nodes if node not in highlight_descendants]
-            
+                # Format highlighted text for Observable.
+                for descendant in highlight_descendants:
+                    highlighted.append([node, "id", descendant])
+                # Gather the non-highlighted text as plain text descendants.
+                plain_descendants = [
+                    node for node in nodes if node not in highlight_descendants
+                ]
+
             # Format all the plain text for observable.
-            for nd in plain_descendants:
-                plain.append([node, "id", nd])
+            for descendant in plain_descendants:
+                plain.append([node, "id", descendant])
 
         # Prepare df depending on what type of text we need.
-        df = pd.DataFrame(locals()[text_type.lower()], columns = ['Component', 'type', 'name'])
+        dataframe = pd.DataFrame(
+            locals()[text_type.lower()], columns=["Component", "type", "name"]
+        )
 
         # Depending on input either export csv locally to disk or as a string.
-        if save_file==True:
+        if save_file:
             file_name = f"{self.schema_abbr}_{self.figure_type}_{text_type}.csv"
-            df.to_csv(os.path.join(self.text_csv_output_path, file_name))
-            return
-        elif save_file==False:
-            return df.to_csv()
+            dataframe.to_csv(os.path.join(self.text_csv_output_path, file_name))
+            return None
+
+        return dataframe.to_csv()
 
-    def get_topological_generations(self):
-        ''' Gather topological_gen, nodes and edges based on figure type.
+    def get_topological_generations(
+        self,
+    ) -> tuple[list[list], NodeView, EdgeDataView, nx.DiGraph]:
+        """Gather topological_gen, nodes and edges based on figure type.
         Outputs:
             topological_gen (List(list)):list of lists. Indicates layers of nodes.
-            nodes: (Networkx NodeView) Nodes of the component or dependency graph. When iterated over it functions like a list.
-            edges: (Networkx EdgeDataView) Edges of component or dependency graph. When iterated over it works like a list of tuples.
-        '''
+            nodes: (Networkx NodeView) Nodes of the component or dependency graph.
+              When iterated over it functions like a list.
+            edges: (Networkx EdgeDataView) Edges of component or dependency graph.
+              When iterated over it works like a list of tuples.
+        """
         # Get nodes in the digraph
         digraph = self.dmge.get_digraph_by_edge_type(self.dependency_type)
         nodes = digraph.nodes()
 
         # Get subgraph
-        #mm_graph = self.sg.se.get_nx_schema()
-        #subg = self.sg.get_subgraph_by_edge_type(mm_graph, self.dependency_type)
-        subg = self.dmge.get_subgraph_by_edge_type(self.dependency_type)
+        subgraph = self.dmge.get_subgraph_by_edge_type(self.dependency_type)
 
         # Get edges and topological_gen based on figure type.
-        if self.figure_type == 'component':
+        if self.figure_type == "component":
             edges = digraph.edges()
-            topological_gen = list(reversed(list(nx.topological_generations(subg))))
+            topological_gen = list(reversed(list(nx.topological_generations(subgraph))))
 
-        elif self.figure_type == 'dependency':
+        elif self.figure_type == "dependency":
             rev_digraph = nx.DiGraph.reverse(digraph)
             edges = rev_digraph.edges()
-            topological_gen = list(nx.topological_generations(subg))
-        
-        return topological_gen, nodes, edges, subg
-
-    def remove_unwanted_characters_from_conditional_statement(self, cond_req: str) -> str:
-        '''Remove unwanted characters from conditional statement
-        Example of conditional requirement: If File Format IS "BAM" OR "CRAM" OR "CSV/TSV" then Genome Build is required
+            topological_gen = list(nx.topological_generations(subgraph))
+
+        return topological_gen, nodes, edges, subgraph
+
+    def remove_unwanted_characters_from_conditional_statement(
+        self, cond_req: str
+    ) -> str:
+        """Remove unwanted characters from conditional statement
+        Example of conditional requirement: If File Format IS "BAM" OR "CRAM" OR
+          "CSV/TSV" then Genome Build is required
         Example output: File Format IS "BAM" OR "CRAM" OR "CSV/TSV"
-        '''
+        """
         if "then" in cond_req:
             # remove everything after "then"
-            cond_req_new = cond_req.split('then')[0]
+            cond_req_new = cond_req.split("then")[0]
 
             # remove "If" and empty space
             cond_req = cond_req_new.replace("If", "").lstrip().rstrip()
         return cond_req
 
-    def get_ca_alias(self, conditional_requirements: list) -> dict:
-        '''Get the alias for each conditional attribute. 
+    def get_ca_alias(self, conditional_requirements: list) -> dict[str, str]:
+        """Get the alias for each conditional attribute.
 
-        NOTE: Obtaining attributes(attr) and aliases(ali) in this function is specific to how formatting
-            is set in AttributesExplorer. If that formatting changes, this section
-            will likely break or in the worst case have a silent error.         
+        NOTE: Obtaining attributes(attr) and aliases(ali) in this function is specific
+          to how formatting is set in AttributesExplorer. If that formatting changes,
+          this section will likely break or in the worst case have a silent error.
         Input:
-            conditional_requirements_list (list): list of strings of conditional requirements from outputs of AttributesExplorer.
+            conditional_requirements_list (list): list of strings of conditional
+              requirements from outputs of AttributesExplorer.
         Output:
             ca_alias (dict):
                 key: alias (attribute response)
                 value: attribute
-        '''
+        """
         ca_alias = {}
 
         # clean up conditional requirements
-        conditional_requirements = [self.remove_unwanted_characters_from_conditional_statement(req) for req in conditional_requirements]
+        conditional_requirements = [
+            self.remove_unwanted_characters_from_conditional_statement(req)
+            for req in conditional_requirements
+        ]
 
-        for i, req in enumerate(conditional_requirements):
+        for req in conditional_requirements:
             if "OR" not in req:
-                attr, ali = req.split(' is ')
+                attr, ali = req.split(" is ")
                 attr = "".join(attr.split())
                 ali = self.strip_double_quotes(ali)
                 ca_alias[ali] = attr
             else:
-                attr, alias_str = req.split(' is ')
-                alias_lst = alias_str.split(' OR ')
+                attr, alias_str = req.split(" is ")
+                alias_lst = alias_str.split(" OR ")
                 for elem in alias_lst:
                     elem = self.strip_double_quotes(elem)
                     ca_alias[elem] = attr
         return ca_alias
 
-    def gather_component_dependency_info(self, cn, attributes_df):
-        '''Gather all component dependency information.
+    def gather_component_dependency_info(
+        self, component_name: str, attributes_df: pd.DataFrame
+    ) -> tuple[list[str], dict[str, str], list[str]]:
+        """Gather all component dependency information.
         Inputs:
-            cn: (str) component name
-            attributes_df: (Pandas DataFrame) Details for all attributes across all components. From AttributesExplorer.
+            component name: (str) component name
+            attributes_df: (Pandas DataFrame) Details for all attributes across all components.
+              From AttributesExplorer.
         Outputs:
             conditional_attributes (list): List of conditional attributes for a particular component
             ca_alias (dict):
                 key: alias (attribute response)
                 value: attribute
             all_attributes (list): all attributes associated with a particular component.
-        '''
+        """
 
         # Gather all component dependency information
         component_attributes = self.dmge.get_descendants_by_edge_type(
-                                        cn,
-                                        self.dependency_type,
-                                        connected=True
-                                        )
-        
+            component_name, self.dependency_type, connected=True
+        )
+
         # Dont want to display `Component` in the figure so remove
-        if 'Component' in component_attributes:
-            component_attributes.remove('Component')
-        
+        if "Component" in component_attributes:
+            component_attributes.remove("Component")
+
         # Gather conditional attributes so they can be added to the figure.
-        if 'Cond_Req' in attributes_df.columns:
-            conditional_attributes = list(attributes_df[(attributes_df['Cond_Req']==True)
-                &(attributes_df['Component']==cn)]['Label'])
-            ca_df = attributes_df[(attributes_df['Cond_Req']==True)&(attributes_df['Component']==cn)]
-            conditional_requirements = list(attributes_df[(attributes_df['Cond_Req']==True)
-                &(attributes_df['Component']==cn)]['Conditional Requirements'])
+        if "Cond_Req" in attributes_df.columns:
+            conditional_attributes = list(
+                attributes_df[
+                    (attributes_df["Cond_Req"])
+                    & (attributes_df["Component"] == component_name)
+                ]["Label"]
+            )
+            conditional_requirements = list(
+                attributes_df[
+                    (attributes_df["Cond_Req"])
+                    & (attributes_df["Component"] == component_name)
+                ]["Conditional Requirements"]
+            )
             ca_alias = self.get_ca_alias(conditional_requirements)
         else:
             # If there are no conditional attributes/requirements, initialize blank lists.
             conditional_attributes = []
             ca_alias = {}
-        
+
         # Gather a list of all attributes for the current component.
-        all_attributes = list(np.append(component_attributes,conditional_attributes))
-        
+        all_attributes = list(np.append(component_attributes, conditional_attributes))
+
         return conditional_attributes, ca_alias, all_attributes
 
-    def find_source_nodes(self, nodes, edges, all_attributes=[]):
-        '''Find all nodes in the graph that do not have a parent node.
+    def find_source_nodes(
+        self,
+        nodes: NodeView,
+        edges: EdgeDataView,
+        all_attributes: Optional[list[str]] = None,
+    ) -> list[str]:
+        """Find all nodes in the graph that do not have a parent node.
         Inputs:
-            nodes: (Networkx NodeView) Nodes of the component or dependency graph. When iterated over it functions like a list.
-            edges: (Networkx EdgeDataView) Edges of component or dependency graph. When iterated over it works like a list of tuples.
-            attributes_df: (Pandas DataFrame) Details for all attributes across all components. From AttributesExplorer.
+            nodes: (Networkx NodeView) Nodes of the component or dependency graph.
+              When iterated over it functions like a list.
+            edges: (Networkx EdgeDataView) Edges of component or dependency graph.
+              When iterated over it works like a list of tuples.
+            attributes_df: (Pandas DataFrame) Details for all attributes across all
+              components. From AttributesExplorer.
 
         Outputs:
-            source_nodes (list(str)): List of parentless nodes in 
-        '''
+            source_nodes (list(str)): List of parentless nodes in
+        """
+        if all_attributes is None:
+            all_attributes = []
         # Find edges that are not source nodes.
         not_source = []
         for node in nodes:
             for edge_pair in edges:
                 if node == edge_pair[0]:
                     not_source.append(node)
 
         # Find source nodes as nodes that are not in not_source.
         source_nodes = []
         for node in nodes:
-            if self.figure_type == 'dependency':
+            if self.figure_type == "dependency":
                 if node not in not_source and node in all_attributes:
                     source_nodes.append(node)
             else:
                 if node not in not_source:
                     source_nodes.append(node)
         return source_nodes
 
-    def get_parent_child_dictionary(self, nodes, edges, all_attributes=[]):
-        '''Based on the dependency type, create dictionaries between parent and child and child and parent attributes.
+    def get_parent_child_dictionary(
+        self, edges: EdgeDataView, all_attributes: Optional[list[str]] = None
+    ) -> tuple[dict[str, list[str]], dict[str, list[str]]]:
+        """
+        Based on the dependency type, create dictionaries between parent and
+          child and child and parent attributes.
         Input:
-            nodes: (Networkx NodeView) Nodes of the component or dependency graph.
             edges: (Networkx EdgeDataView (component figure) or List(list) (dependency figure))
                 Edges of component or dependency graph.
             all_attributes:
         Output:
             child_parents (dict):
                 key: child
-                value: list of the childs parents
+                value: list of the child's parents
             parent_children (dict):
                 key: parent
                 value: list of the parents children
-        '''
-        child_parents = {}
-        parent_children = {}
+        """
+        # pylint: disable=too-many-branches
+        all_attributes_list = [] if all_attributes is None else all_attributes
+        child_parents: dict[str, list[str]] = {}
+        parent_children: dict[str, list[str]] = {}
 
-        if self.dependency_type == 'requiresComponent':
-            
+        if self.dependency_type == "requiresComponent":
             # Construct child_parents dictionary
             for edge in edges:
-                
                 # Add child as a key
-                if edge[0] not in child_parents.keys():
+                if edge[0] not in child_parents:
                     child_parents[edge[0]] = []
-                
+
                 # Add parents to list
                 child_parents[edge[0]].append(edge[1])
-            
+
             # Construct parent_children dictionary
             for edge in edges:
-                
                 # Add parent as a key
-                if edge[1] not in parent_children.keys():
+                if edge[1] not in parent_children:
                     parent_children[edge[1]] = []
-                
+
                 # Add children to list
                 parent_children[edge[1]].append(edge[0])
-        
-        elif self.dependency_type == 'requiresDependency':
-            
+
+        elif self.dependency_type == "requiresDependency":
             # Construct child_parents dictionary
             for edge in edges:
-                
                 # Check if child is an attribute for the current component
-                if edge[0] in all_attributes:
-                    
+                if edge[0] in all_attributes_list:
                     # Add child as a key
-                    if edge[0] not in child_parents.keys():
+                    if edge[0] not in child_parents:
                         child_parents[edge[0]] = []
-                    
-                    # Add parent to list if it is an attriute for the current component
-                    if edge[1] in all_attributes:
+
+                    # Add parent to list if it is an attribute for the current component
+                    if edge[1] in all_attributes_list:
                         child_parents[edge[0]].append(edge[1])
-            
+
             # Construct parent_children dictionary
             for edge in edges:
-                
                 # Check if parent is an attribute for the current component
-                if edge[1] in all_attributes:
-                    
+                if edge[1] in all_attributes_list:
                     # Add parent as a key
-                    if edge[1] not in parent_children.keys():
+                    if edge[1] not in parent_children:
                         parent_children[edge[1]] = []
-                    
-                    # Add child to list if it is an attriute for the current component
-                    if edge[0] in all_attributes:
+
+                    # Add child to list if it is an attribute for the current component
+                    if edge[0] in all_attributes_list:
                         parent_children[edge[1]].append(edge[0])
 
         return child_parents, parent_children
 
-    def alias_edges(self, ca_alias:dict, edges) -> List[list]:
-        '''Create new edges based on aliasing between an attribute and its response.
+    def alias_edges(self, ca_alias: dict[str, str], edges: EdgeDataView) -> list[list]:
+        """Create new edges based on aliasing between an attribute and its response.
         Purpose:
             Create aliased edges.
-            For example: 
+            For example:
                 If BiospecimenType (attribute) is AnalyteBiospecimenType (response)
                 Then ShippingConditionType (conditional requirement) is now required.
             In the model the edges that connect these options are:
                 (AnalyteBiospecimenType, BiospecimenType)
                 (ShippingConditionType, AnalyteBiospecimenType)
-            Use alias defined in self.get_ca_alias along to define new edges that would 
-            directly link attributes to their conditional requirements, in this 
+            Use alias defined in self.get_ca_alias along to define new edges that would
+            directly link attributes to their conditional requirements, in this
             example the new edge would be:
                 [ShippingConditionType, BiospecimenType]
         Inputs:
             ca_alias (dict):
                 key: alias (attribute response)
                 value: attribute
-            edges (Networkx EdgeDataView): Edges of component or dependency graph. When iterated over it works like a list of tuples.
+            edges (Networkx EdgeDataView): Edges of component or dependency graph.
+              When iterated over it works like a list of tuples.
         Output:
-            aliased_edges (List[lists]) of aliased edges.
-        '''
+            aliased_edges (list[list]) of aliased edges.
+        """
         aliased_edges = []
-        for i, edge in enumerate(edges):
-            
+        for edge in edges:
             # construct one set of edges at a time
             edge_set = []
-            
-            # If the first edge has an alias add alias to the first position in the current edge set
+
+            # If the first edge has an alias add alias to the first
+            # position in the current edge set
             if edge[0] in ca_alias.keys():
                 edge_set.append(ca_alias[edge[0]])
-            
+
             # Else add the non-aliased edge
             else:
                 edge_set.append(edge[0])
 
-            # If the secod edge has an alias add alias to the first position in the current edge set
+            # If the second edge has an alias add alias to the first
+            # position in the current edge set
             if edge[1] in ca_alias.keys():
                 edge_set.append(ca_alias[edge[1]])
-            
+
             # Else add the non-aliased edge
             else:
                 edge_set.append(edge[1])
 
             # Add new edge set to a the list of aliased edges.
             aliased_edges.append(edge_set)
 
         return aliased_edges
 
-    def prune_expand_topological_gen(self, topological_gen, all_attributes, conditional_attributes):
-        '''
+    def prune_expand_topological_gen(
+        self,
+        topological_gen: list[list[str]],
+        all_attributes: list[str],
+        conditional_attributes: list[str],
+    ) -> list[list[str]]:
+        """
         Purpose:
             Remake topological_gen with only relevant nodes.
-                This is necessary since for the figure this function is being used in we 
+                This is necessary since for the figure this function is being used in we
                 only want to display a portion of the graph data.
             In addition to only displaying relevant nodes, we want to add conditional
                 attributes to topological_gen so we can visualize them in the tangled tree
                 as well.
         Input:
             topological_gen (List[list]): Indicates layers of nodes.
             all_attributes (list): all attributes associated with a particular component.
             conditional_attributes (list): List of conditional attributes for a particular component
         Output:
             new_top_gen (List[list]): mimics structure of topological_gen but only
                 includes the nodes we want
-        '''
+        """
 
         pruned_topological_gen = []
 
         # For each layer(gen) in the topological generation list
-        for i, layer in enumerate(topological_gen):
-            
+        for layer in topological_gen:
             current_layer = []
             next_layer = []
-            
+
             # For each node in the layer
             for node in layer:
-                
-                # If the node is relevant to this component and is not a conditional attribute add it to the current layer.
+                # If the node is relevant to this component and is not a conditional
+                # attribute add it to the current layer.
                 if node in all_attributes and node not in conditional_attributes:
                     current_layer.append(node)
-                
+
                 # If its a conditional attribute add it to a followup layer.
                 if node in conditional_attributes:
                     next_layer.append(node)
 
             # Added layers to new pruned_topological_gen list
             if current_layer:
                 pruned_topological_gen.append(current_layer)
             if next_layer:
                 pruned_topological_gen.append(next_layer)
 
         return pruned_topological_gen
 
-    def get_base_layers(self, topological_gen, child_parents, source_nodes, cn):
-        '''
+    def get_base_layers(
+        self,
+        topological_gen: list[list],
+        child_parents: dict,
+        source_nodes: list,
+        component_name: str,
+    ) -> tuple[dict[str, Any], dict[str, Any]]:
+        """
         Purpose:
-            Reconfigure topological gen to move things back appropriate layers if 
+            Reconfigure topological gen to move things back appropriate layers if
             they would have a back reference.
 
-            The Tangle Tree figure requrires an acyclic directed graph that has additional 
+            The Tangle Tree figure requires an acyclic directed graph that has additional
                 layering rules between connected nodes.
                 - If there is a backward connection then the line connecting them will
                     break (this would suggest a cyclic connection.)
-                - Additionally if two or more nodes are connecting to a downstream node it is 
-                    best to put both parent nodes at the same level, if possible, to 
+                - Additionally if two or more nodes are connecting to a downstream node it is
+                    best to put both parent nodes at the same level, if possible, to
                     prevent line breaks.
-                - Also want to move any children nodes one layer below 
+                - Also want to move any children nodes one layer below
                     the parent node(s). If there are multiple parents, put one layer below the
                     parent that is furthest from the origin.
 
             This is an iterative process that needs to run twice to move all the nodes to their
             appropriate positions.
         Input:
             topological_gen: list of lists. Indicates layers of nodes.
             child_parents (dict):
                 key: child
-                value: list of the childs parents
+                value: list of the child's parents
             source_nodes: list, list of nodes that do not have a parent.
-            cn: str, component name, default=''
+            component_name: str, component name, default=''
         Output:
             base_layers: dict, key: component name, value: layer
-                represents initial layering of toplogical_gen
+                represents initial layering of topological_gen
             base_layers_copy_copy: dict, key: component name, value: layer
                 represents the final layering after moving the components/attributes to
                 their desired layer.c
-        '''
+        """
         # Convert topological_gen to a dictionary
-        base_layers = {com:i for i, lev in enumerate(topological_gen)
-                                for com in lev}
-        
+        base_layers = {com: i for i, lev in enumerate(topological_gen) for com in lev}
+
         # Make another version to iterate on -- Cant set to equal or will overwrite the original.
-        base_layers_copy = {com:i for i, lev in enumerate(topological_gen)
-                                for com in lev}
+        base_layers_copy = {
+            com: i for i, lev in enumerate(topological_gen) for com in lev
+        }
 
         # Move child nodes one node downstream of their parents.
         for level in topological_gen:
             for node in level:
-                
                 # Check if node has a parent.
                 if node in child_parents.keys():
-                    
-                    #node_level = base_layers[node]
+                    # node_level = base_layers[node]
                     # Look at the parents for the node.
                     parent_levels = []
                     for par in child_parents[node]:
-                        
                         # Get the layer the parent is located at.
                         parent_levels.append(base_layers[par])
-                        
+
                         # Get the max layer a parent of the node can be found.
                         max_parent_level = max(parent_levels)
 
-                        # Move the node one layer beyond the max parent node position, so it will be downstream of its parents.
+                        # Move the node one layer beyond the max parent node position,
+                        # so it will be downstream of its parents.
                         base_layers_copy[node] = max_parent_level + 1
-        
+
         # Make another version of updated positions iterate on further.
         base_layers_copy_copy = base_layers_copy
 
         # Move parental source nodes if necessary.
         for level in topological_gen:
             for node in level:
-                
                 # Check if node has any parents.
                 if node in child_parents.keys():
                     parent_levels = []
                     modify_par = []
-                    
+
                     # For each parent get their position.
                     for par in child_parents[node]:
                         parent_levels.append(base_layers_copy[par])
-                    
-                    # If one of the parents is a source node move 
+
+                    # If one of the parents is a source node move
                     # it to the same level as the other nodes the child connects to so
                     # that the connections will not be backwards (and result in a broken line)
                     for par in child_parents[node]:
-                        
-                        # For a given parent determine if its a source node and that the parents 
-                        # are not already at level 0, and the parent is not the current component node.
-                        if (par in source_nodes and 
-                            (parent_levels.count(parent_levels[0]) != len(parent_levels))
-                            and par != cn):
-
+                        # For a given parent determine if its a source node and that the parents
+                        # are not already at level 0, and the parent is not the current component
+                        # node.
+                        if (
+                            par in source_nodes
+                            and (
+                                parent_levels.count(parent_levels[0])
+                                != len(parent_levels)
+                            )
+                            and par != component_name
+                        ):
                             # If so, remove its position from parent_levels
                             parent_levels.remove(base_layers_copy[par])
-                            
+
                             # Add this parent to a list of parental positions to modify later.
                             modify_par.append(par)
-                        
+
                         # Get the new max parent level for this node.
                         max_parent_level = max(parent_levels)
-                        
+
                         # Move the node one position downstream of its max parent level.
                         base_layers_copy_copy[node] = max_parent_level + 1
-                    
-                    # For each parental position to modify, move the parents level up to the max_parent_level.
+
+                    # For each parental position to modify, move the parents level up to
+                    # the max_parent_level.
                     for par in modify_par:
                         base_layers_copy_copy[par] = max_parent_level
-        
+
         return base_layers, base_layers_copy_copy
 
-    def adjust_node_placement(self, base_layers_copy_copy, base_layers, topological_gen):
-        '''Reorder nodes within topological_generations to match how they were ordered in base_layers_copy_copy
+    def adjust_node_placement(
+        self,
+        base_layers_copy_copy: dict[str, Any],
+        base_layers: dict[str, Any],
+        topological_gen: list[list],
+    ) -> list[list]:
+        """Reorder nodes within topological_generations to match how they were ordered in
+         base_layers_copy_copy
         Input:
             topological_gen: list of lists. Indicates layers of nodes.
             base_layers: dict, key: component name, value: layer
-                represents initial layering of toplogical_gen
+                represents initial layering of topological_gen
             base_layers_copy_copy: dict, key: component name, value: layer
                 represents the final layering after moving the components/attributes to
                 their desired layer.
         Output:
-            topological_gen: same format but as the incoming topologial_gen but
+            topological_gen: same format but as the incoming topological_gen but
                 ordered to match base_layers_copy_copy.
-        '''
-        if self.figure_type == 'component':
+        """
+        if self.figure_type == "component":
             # For each node get its new layer in the tangled tree
             for node, i in base_layers_copy_copy.items():
-                
                 # Check if node is not already in the proper layer
                 if node not in topological_gen[i]:
-
                     # If not put it in the appropriate layer
                     topological_gen[i].append(node)
-                    
+
                     # Remove from inappropriate layer.
                     topological_gen[base_layers[node]].remove(node)
-        
-        elif self.figure_type == 'dependency':
+
+        elif self.figure_type == "dependency":
             for node, i in base_layers_copy_copy.items():
-                
-                # Check if the location of the node is more than the number of 
+                # Check if the location of the node is more than the number of
                 # layers topological gen current handles
                 if i > len(topological_gen) - 1:
-
                     # If so, add node to new node at the end of topological_gen
                     topological_gen.append([node])
-                    
+
                     # Remove the node from its previous position.
                     topological_gen[base_layers[node]].remove(node)
-                
+
                 # Else, check if node is not already in the proper layer
                 elif node not in topological_gen[i]:
-
                     # If not put it in the appropriate layer
                     topological_gen[i].append(node)
-                    
+
                     # Remove from inappropriate layer.
                     topological_gen[base_layers[node]].remove(node)
         return topological_gen
 
-    def move_source_nodes_to_bottom_of_layer(self, node_layers, source_nodes):
-        '''For aesthetic purposes move source nodes to the bottom of their respective layers.
+    def move_source_nodes_to_bottom_of_layer(
+        self, node_layers: list[list], source_nodes: list
+    ) -> list[list]:
+        """For aesthetic purposes move source nodes to the bottom of their respective layers.
         Input:
-            node_layers (List(list)): Lists of lists of each layer and the nodes contained in that layer as strings.
+            node_layers (List(list)): Lists of lists of each layer and the nodes contained
+              in that layer as strings.
             source_nodes (list): list of nodes that do not have a parent.
         Output:
             node_layers (List(list)): modified to move source nodes to the bottom of each layer.
-        '''
-        for i, layer in enumerate(node_layers):
+        """
+        for layer in node_layers:
             nodes_to_move = []
             for node in layer:
                 if node in source_nodes:
                     nodes_to_move.append(node)
             for node in nodes_to_move:
-                node_layers[i].remove(node)
-                node_layers[i].append(node)
+                layer.remove(node)
+                layer.append(node)
         return node_layers
 
-    def get_layers_dict_list(self, node_layers, child_parents, parent_children, all_parent_children):
-        '''Convert node_layers to a list of lists of dictionaries that specifies each node and its parents (if applicable).
+    def get_layers_dict_list(
+        self,
+        node_layers: list[list],
+        child_parents: dict,
+        parent_children: dict,
+        all_parent_children: dict,
+    ) -> list[list[dict[str, list[str]]]]:
+        """Convert node_layers to a list of lists of dictionaries that specifies each node and
+         its parents (if applicable).
         Inputs:
-            node_layers: list of lists of each layer and the nodes contained in that layer as strings.
+            node_layers: list of lists of each layer and the nodes contained in that layer
+              as strings.
             child_parents (dict):
                 key: child
-                value: list of the childs parents
+                value: list of the child's parents
             parent_children (dict):
                 key: parent
                 value: list of the parents children
         Outputs:
-            layers_list (List(list): list of lists of dictionaries that specifies each node and its parents (if applicable)
-        '''
+            layers_list (List(list): list of lists of dictionaries that specifies each node and its
+             parents (if applicable)
+        """
         num_layers = len(node_layers)
-        layers_list = [[] for i in range(0, num_layers)]
+        layers_list: list[list[dict[str, list[str]]]] = [
+            [] for i in range(0, num_layers)
+        ]
         for i, layer in enumerate(node_layers):
             for node in layer:
                 if node in child_parents.keys():
                     parents = child_parents[node]
-                else: 
+                else:
                     parents = []
 
                 if node in parent_children.keys():
                     direct_children = parent_children[node]
-                else: 
+                else:
                     direct_children = []
 
                 if node in all_parent_children.keys():
                     all_children = all_parent_children[node]
-                else: 
+                else:
                     all_children = []
-                layers_list[i].append({'id': node, 'parents': parents, 'direct_children': direct_children, 'children': all_children})
+                layers_list[i].append(
+                    {
+                        "id": node,
+                        "parents": parents,
+                        "direct_children": direct_children,
+                        "children": all_children,
+                    }
+                )
 
         return layers_list
 
-    def get_node_layers_json(self, topological_gen, source_nodes, child_parents, parent_children, cn='', all_parent_children=None):
-        '''Return all the layers of a single tangled tree as a JSON String.
+    def get_node_layers_json(  # pylint: disable=too-many-arguments
+        self,
+        topological_gen: list[list],
+        source_nodes: list[str],
+        child_parents: dict,
+        parent_children: dict,
+        component_name: str = "",
+        all_parent_children: Optional[dict] = None,
+    ) -> str:
+        """Return all the layers of a single tangled tree as a JSON String.
         Inputs:
             topological_gen:list of lists. Indicates layers of nodes.
             source_nodes: list of nodes that do not have a parent.
             child_parents (dict):
                 key: child
-                value: list of the childs parents
+                value: list of the child's parents
             parent_children (dict):
                 key: parent
                 value: list of the parents children
             all_parent_children (dict):
                 key: parent
-                value: list of the parents children (including all downstream nodes). Default to an empty dictionary
+                value: list of the parents children (including all downstream nodes).
+                  Default to an empty dictionary
         Outputs:
             layers_json (JSON String): Layers of nodes in the tangled tree as a json string.
-        '''
+        """
 
-        base_layers, base_layers_copy_copy = self.get_base_layers(topological_gen, 
-                child_parents, source_nodes, cn)
+        base_layers, base_layers_copy_copy = self.get_base_layers(
+            topological_gen, child_parents, source_nodes, component_name
+        )
 
         # Rearrange node_layers to follow the pattern laid out in component layers.
-        node_layers = self.adjust_node_placement(base_layers_copy_copy, 
-            base_layers, topological_gen)
+        node_layers = self.adjust_node_placement(
+            base_layers_copy_copy, base_layers, topological_gen
+        )
 
         # Move source nodes to the bottom of each layer.
-        node_layers = self.move_source_nodes_to_bottom_of_layer(node_layers, source_nodes)
+        node_layers = self.move_source_nodes_to_bottom_of_layer(
+            node_layers, source_nodes
+        )
 
         # Convert layers to a list of dictionaries
         if not all_parent_children:
-            # default to an empty dictionary 
-            all_parent_children = dict()
-            
-        layers_dicts = self.get_layers_dict_list(node_layers, child_parents, parent_children, all_parent_children)
+            # default to an empty dictionary
+            all_parent_children = {}
+
+        layers_dicts = self.get_layers_dict_list(
+            node_layers, child_parents, parent_children, all_parent_children
+        )
 
         # Convert dictionary to a JSON string
         layers_json = json.dumps(layers_dicts)
 
         return layers_json
 
-    def save_outputs(self, save_file, layers_json, cn='', all_layers=None):
-        '''
+    def save_outputs(
+        self,
+        save_file: bool,
+        layers_json,
+        component_name: str = "",
+        all_layers: Optional[list[str]] = None,
+    ) -> list[str]:
+        """
         Inputs:
             save_file (bool): Indicates whether to save a file locally or not.:
             layers_json (JSON String): Layers of nodes in the tangled tree as a json string.
-            cn (str): component name, default=''
-            all_layers (list of json strings): Each string represents contains the layers for a single tangled tree.
-                If a dependency figure the list is added to each time this function is called, so starts incomplete.
-                default=[].
+            component_name (str): component name, default=''
+            all_layers (list of json strings): Each string represents contains the layers for
+                a single tangled tree. If a dependency figure the list is added to each time
+                this function is called, so starts incomplete. default=[].
         Outputs:
-            all_layers (list of json strings): 
-                If save_file == False: Each string represents contains the layers for a single tangled tree.
+            all_layers (list of json strings):
+                If save_file == False: Each string represents contains the layers for a single
+                 tangled tree.
                 If save_file ==True: is an empty list.
-        '''
-        if all_layers is None:
-            all_layers = []
-        if save_file == True:
-            if cn:
-                output_file_name = f"{self.schema_abbr}_{self.figure_type}_{cn}_tangled_tree.json"
+        """
+        all_layers_list = [] if all_layers is None else all_layers
+        if save_file:
+            if component_name:
+                output_file_name = (
+                    f"{self.schema_abbr}_{self.figure_type}_"
+                    f"{component_name}_tangled_tree.json"
+                )
             else:
-                output_file_name = f"{self.schema_abbr}_{self.figure_type}_tangled_tree.json"
-            with open(os.path.join(self.json_output_path, output_file_name), 'w') as outfile:
+                output_file_name = (
+                    f"{self.schema_abbr}_{self.figure_type}_tangled_tree.json"
+                )
+            with open(
+                os.path.join(self.json_output_path, output_file_name),
+                mode="w",
+                encoding="utf-8",
+            ) as outfile:
                 outfile.write(layers_json)
-            logger.info(f"Tangled Tree JSON String saved to {os.path.join(self.json_output_path, output_file_name)}.")
-            all_layers = layers_json
-        elif save_file == False:
-            all_layers.append(layers_json)
-        return all_layers
 
-    def get_ancestors_nodes(self, subgraph, components):
+            logger.info(
+                (
+                    "Tangled Tree JSON String saved to "
+                    f"{os.path.join(self.json_output_path, output_file_name)}"
+                )
+            )
+            all_layers_list = layers_json
+        else:
+            all_layers_list.append(layers_json)
+        return all_layers_list
+
+    def get_ancestors_nodes(
+        self, subgraph: nx.DiGraph, components: list[str]
+    ) -> dict[str, list[str]]:
         """
-        Inputs: 
+        Inputs:
             subgraph: networkX graph object
-            components: a list of nodes 
-        outputs: 
-            all_parent_children: a dictionary that indicates a list of children (including all the intermediate children) of a given node
+            components: a list of nodes
+        outputs:
+            all_parent_children: a dictionary that indicates a list of children
+              (including all the intermediate children) of a given node
         """
         all_parent_children = {}
-        for component in components: 
-            all_ancestors = self.dmge.get_nodes_ancestors(subgraph=subgraph, node_label=component)
+        for component in components:
+            all_ancestors = self.dmge.get_nodes_ancestors(
+                subgraph=subgraph, node_label=component
+            )
             all_parent_children[component] = all_ancestors
 
         return all_parent_children
 
-    def get_tangled_tree_layers(self, save_file=True):
-        '''Based on user indicated figure type, construct the layers of nodes of a tangled tree.
+    def get_tangled_tree_layers(self, save_file: bool = True):
+        """Based on user indicated figure type, construct the layers of nodes of a tangled tree.
         Inputs:
             save_file (bool): Indicates whether to save a file locally or not.
         Outputs:
-            all_layers (list of json strings): 
-                If save_file == False: Each string represents contains the layers for a single tangled tree.
+            all_layers (list of json strings):
+                If save_file == False: Each string represents contains the layers
+                  for a single tangled tree.
                 If save_file ==True: is an empty list.
 
         Note on Dependency Tangled Tree:
-            If there are many conditional requirements associated with a depependency, and those
+            If there are many conditional requirements associated with a dependency, and those
             conditional requirements have overlapping attributes associated with them
             the tangled tree will only report one
-        
-        '''
+
+        """
+        # pylint: disable=too-many-locals
         # Gather the data model's, topological generations, nodes and edges
-        topological_gen, nodes, edges, subg = self.get_topological_generations()
+        topological_gen, nodes, edges, subgraph = self.get_topological_generations()
 
-        if self.figure_type == 'component':
+        if self.figure_type == "component":
             # Gather all source nodes
             source_nodes = self.find_source_nodes(nodes, edges)
-            
+
             # Map all children to their parents and vice versa
-            child_parents, parent_children = self.get_parent_child_dictionary(nodes, edges)
+            child_parents, parent_children = self.get_parent_child_dictionary(
+                edges=edges
+            )
 
             # find all the downstream nodes
-            all_parent_children = self.get_ancestors_nodes(subg, parent_children.keys())
-            
+            all_parent_children = self.get_ancestors_nodes(
+                subgraph, parent_children.keys()
+            )
+
             # Get the layers that each node belongs to.
-            layers_json = self.get_node_layers_json(topological_gen, source_nodes, child_parents, parent_children, all_parent_children=all_parent_children)
+            layers_json = self.get_node_layers_json(
+                topological_gen,
+                source_nodes,
+                child_parents,
+                parent_children,
+                all_parent_children=all_parent_children,
+            )
 
             # If indicated save outputs locally else gather all layers.
-            all_layers = self.save_outputs(save_file, layers_json)         
+            all_layers = self.save_outputs(save_file, layers_json)
 
-        if self.figure_type == 'dependency':
+        if self.figure_type == "dependency":
             # Get component digraph and nodes.
-            component_dg = self.dmge.get_digraph_by_edge_type('requiresComponent')
+            component_dg = self.dmge.get_digraph_by_edge_type("requiresComponent")
             component_nodes = component_dg.nodes()
 
             # Get table of attributes.
-            attributes_csv_str = self.ae.parse_attributes(save_file=False)
+            attributes_csv_str = self.attributes_explorer.parse_attributes(
+                save_file=False
+            )
             attributes_df = pd.read_table(StringIO(attributes_csv_str), sep=",")
 
-            
-            all_layers =[]
-            for cn in component_nodes:
+            all_layers = []
+            for component_name in component_nodes:
                 # Gather attribute and dependency information per node
-                conditional_attributes, ca_alias, all_attributes = self.gather_component_dependency_info(cn, attributes_df)
+                (
+                    conditional_attributes,
+                    ca_alias,
+                    all_attributes,
+                ) = self.gather_component_dependency_info(component_name, attributes_df)
 
                 # Gather all source nodes
-                source_nodes = self.find_source_nodes(component_nodes, edges, all_attributes)
+                source_nodes = self.find_source_nodes(
+                    component_nodes, edges, all_attributes
+                )
 
                 # Alias the conditional requirement edge back to its actual parent label,
                 # then apply aliasing back to the edges
                 aliased_edges = self.alias_edges(ca_alias, edges)
 
                 # Gather relationships between children and their parents.
-                child_parents, parent_children = self.get_parent_child_dictionary(nodes,
-                    aliased_edges, all_attributes)
+                child_parents, parent_children = self.get_parent_child_dictionary(
+                    aliased_edges, all_attributes
+                )
 
                 # Remake topological_gen so it has only relevant nodes.
-                pruned_topological_gen = self.prune_expand_topological_gen(topological_gen, all_attributes, conditional_attributes)
+                pruned_topological_gen = self.prune_expand_topological_gen(
+                    topological_gen, all_attributes, conditional_attributes
+                )
 
                 # Get the layers that each node belongs to.
-                layers_json = self.get_node_layers_json(pruned_topological_gen, source_nodes, child_parents, parent_children, cn)
+                layers_json = self.get_node_layers_json(
+                    pruned_topological_gen,
+                    source_nodes,
+                    child_parents,
+                    parent_children,
+                    component_name,
+                )
 
                 # If indicated save outputs locally else, gather all layers.
-                all_layers = self.save_outputs(save_file, layers_json, cn, all_layers)
+                all_layers = self.save_outputs(
+                    save_file, layers_json, component_name, all_layers
+                )
         return all_layers
-
-
```

### Comparing `schematicpy-24.1.1/setup.py` & `schematicpy-24.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,18 @@
  'schematic.visualization']
 
 package_data = \
 {'': ['*'],
  'schematic': ['etc/*', 'etc/data_models/*', 'etc/validation_schemas/*']}
 
 install_requires = \
-['Flask-Cors>=3.0.10,<4.0.0',
- 'Flask>=2.0.0,<3.0.0',
- 'Jinja2>2.11.3',
- 'MarkupSafe==2.1.0',
+['MarkupSafe==2.1.0',
  'PyYAML>=6.0.0,<7.0.0',
  'click-log>=0.4.0,<0.5.0',
  'click>=8.0.0,<9.0.0',
- 'connexion[swagger-ui]>=2.8.0,<3.0.0',
  'dataclasses-json>=0.6.1,<0.7.0',
  'dateparser>=1.1.4,<2.0.0',
  'google-api-python-client>=2.0.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.8.0,<0.9.0',
  'graphviz>=0.20.0,<0.21.0',
  'great-expectations>=0.15.0,<0.16.0',
@@ -35,38 +31,43 @@
  'itsdangerous>=2.0.0,<3.0.0',
  'jsonschema>=4.0.0,<5.0.0',
  'networkx>=2.2.8',
  'numpy>=1.21.1,<2.0.0',
  'oauth2client>=4.1.0,<5.0.0',
  'openpyxl>=3.0.9,<4.0.0',
  'pandarallel>=1.6.4,<2.0.0',
- 'pandas>=1.3.1,<2.0.0',
+ 'pandas>=2.0.0,<3.0.0',
  'pdoc>=12.2.0,<13.0.0',
  'pygsheets>=2.0.4,<3.0.0',
  'pyopenssl>=23.0.0,<24.0.0',
  'rdflib>=6.0.0,<7.0.0',
- 'schematic-db[synapse]==0.0.dev33',
+ 'schematic-db[synapse]==0.0.34',
  'setuptools>=66.0.0,<67.0.0',
  'sphinx-click>=4.0.0,<5.0.0',
- 'synapseclient>=3.1.1,<4.0.0',
+ 'synapseclient>=3.2.0,<4.0.0',
  'tenacity>=8.0.1,<9.0.0',
  'toml>=0.10.2,<0.11.0',
  'typing-extensions<4.6.0']
 
 extras_require = \
-{':python_version < "3.9"': ['backports.zoneinfo>=0.2.1,<0.3.0']}
+{':python_version < "3.9"': ['backports.zoneinfo>=0.2.1,<0.3.0'],
+ 'api': ['connexion[swagger-ui]>=2.8.0,<3.0.0',
+         'Flask>=2.0.0,<3.0.0',
+         'Flask-Cors>=3.0.10,<4.0.0',
+         'Jinja2>2.11.3'],
+ 'aws': ['uWSGI>=2.0.21,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['schematic = schematic.__main__:main']}
 
 setup_kwargs = {
     'name': 'schematicpy',
-    'version': '24.1.1',
+    'version': '24.2.1',
     'description': 'Package for biomedical data model and metadata ingress management',
-    'long_description': '# Schematic\n[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FSage-Bionetworks%2Fschematic%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/Sage-Bionetworks/schematic/goto?ref=develop) [![Documentation Status](https://readthedocs.org/projects/sage-schematic/badge/?version=develop)](https://sage-schematic.readthedocs.io/en/develop/?badge=develop) [![PyPI version](https://badge.fury.io/py/schematicpy.svg)](https://badge.fury.io/py/schematicpy)\n\n# Table of contents\n- [Introduction](#introduction)\n- [Installation](#installation)\n  - [Installation Requirements](#installation-requirements)\n  - [Installation guide for data curator app](#installation-guide-for-data-curator-app)\n  - [Installation guide for developers/contributors](#installation-guide-for-developerscontributors)\n- [Other Contribution Guidelines](#other-contribution-guidelines)\n    - [Update readthedocs documentation](#update-readthedocs-documentation)\n- [Command Line Usage](#command-line-usage)\n- [Testing](#testing)\n  - [Updating Synapse test resources](#updating-synapse-test-resources)\n- [Code Style](#code-style)\n- [Contributors](#contributors)\n\n# Introduction\nSCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.\n\n# Installation\n## Installation Requirements\n* Python version 3.9.0≤x<3.11.0 \n\nNote: You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/), and also have the right permissions to download the Google credentials files from Synapse.\n\n\n## Installation guide for data curator app\n\nCreate and activate a virtual environment within which you can install the package:\n\n```\npython3 -m venv .venv\nsource .venv/bin/activate\n```\n\nNote: Python 3 has a built-in support for virtual environment [venv](https://docs.python.org/3/library/venv.html#module-venv) so you no longer need to install virtualenv.\n\nInstall and update the package using [pip](https://pip.pypa.io/en/stable/quickstart/):\n\n```\npython3 -m pip install schematicpy\n```\n\nIf you run into error: Failed building wheel for numpy, the error might be able to resolve by upgrading pip. Please try to upgrade pip by:\n\n```\npip3 install --upgrade pip\n```\n\n## Installation guide for developers/contributors \n\nWhen contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the owners of this repository before making a change.\n\nPlease note we have a [code of conduct](CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.\n\n### Development environment setup\n1. Clone the `schematic` package repository.\n```\ngit clone https://github.com/Sage-Bionetworks/schematic.git\n```\n2. Install `poetry` (version 1.3.0 or later) using either the [official installer](https://python-poetry.org/docs/#installing-with-the-official-installer) or [pipx](https://python-poetry.org/docs/#installing-with-pipx). If you have an older installation of Poetry, we recommend uninstalling it first. \n\n3. Start the virtual environment by doing: \n```\npoetry shell\n```\n4. Install the dependencies by doing: \n```\npoetry install\n```\nThis command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)\n\n5. Fill in credential files: \n*Note*: If you won\'t interact with Synapse, please ignore this section.\n\nThere are two main configuration files that need to be edited:\nconfig.yml\nand [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)\n\n<strong>Configure .synapseConfig File</strong>\n\nDownload a copy of the ``.synapseConfig`` file, open the file in the\neditor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section \n\n*Note*: You could also visit [configparser](https://docs.python.org/3/library/configparser.html#module-configparser>) doc to see the format that `.synapseConfig` must have. For instance:\n>[authentication]<br> username = ABC <br> authtoken = abc\n\n<strong>Configure config.yml File</strong>\n\nThere are some defaults in schematic that can be configured. These fields are in ``config_example.yml``:\n\n```text\n\n# This is an example config for Schematic.\n# All listed values are those that are the default if a config is not used.\n# Save this as config.yml, this will be gitignored.\n# Remove any fields in the config you don\'t want to change\n# Change the values of any fields you do want to change\n\n\n# This describes where assets such as manifests are stored\nasset_store:\n  # This is when assets are stored in a synapse project\n  synapse:\n    # Synapse ID of the file view listing all project data assets.\n    master_fileview_id: "syn23643253"\n    # Path to the synapse config file, either absolute or relative to this file\n    config: ".synapseConfig"\n    # Base name that manifest files will be saved as\n    manifest_basename: "synapse_storage_manifest"\n\n# This describes information about manifests as it relates to generation and validation\nmanifest:\n  # Location where manifests will saved to\n  manifest_folder: "manifests"\n  # Title or title prefix given to generated manifest(s)\n  title: "example"\n  # Data types of manifests to be generated or data type (singular) to validate manifest against\n  data_type:\n    - "Biospecimen"\n    - "Patient"\n\n# Describes the location of your schema\nmodel:\n  # Location of your schema jsonld, it must be a path relative to this file or absolute\n  location: "tests/data/example.model.jsonld"\n\n# This section is for using google sheets with Schematic\ngoogle_sheets:\n  # The Synapse id of the Google service account credentials.\n  service_acct_creds_synapse_id: "syn25171627"\n  # Path to the synapse config file, either absolute or relative to this file\n  service_acct_creds: "schematic_service_account_creds.json"\n  # When doing google sheet validation (regex match) with the validation rules.\n  #   true is alerting the user and not allowing entry of bad values.\n  #   false is warning but allowing the entry on to the sheet.\n  strict_validation: true\n```\n\nIf you want to change any of these copy ``config_example.yml`` to ``config.yml``, change any fields you want to, and remove any fields you don\'t.\n\nFor example if you wanted to change the folder where manifests are downloaded your config should look like:\n\n```text\n\nmanifest:\n  manifest_folder: "my_manifest_folder_path"\n```\n\n_Note_: `config.yml` is ignored by git.\n\n_Note_: Paths can be specified relative to the `config.yml` file or as absolute paths.\n\n6. Login to Synapse by using the command line\nOn the CLI in your virtual environment, run the following command: \n```\nsynapse login -u <synapse username> -p <synapse password> --rememberMe\n```\nPlease make sure that you run the command before running `schematic init` below\n\n7. Obtain Google credential Files\nTo obtain  ``schematic_service_account_creds.json``, please run: \n```\nschematic init --config ~/path/to/config.yml\n```\n> As v22.12.1 version of schematic, using `token` mode of authentication (in other words, using `token.pickle` and `credentials.json`) is no longer supported due to Google\'s decision to move away from using OAuth out-of-band (OOB) flow. Click [here](https://developers.google.com/identity/protocols/oauth2/resources/oob-migration) to learn more. \n\n*Notes*: Use the ``schematic_service_account_creds.json`` file for the service\naccount mode of authentication (*for Google services/APIs*). Service accounts \nare special Google accounts that can be used by applications to access Google APIs \nprogrammatically via OAuth2.0, with the advantage being that they do not require \nhuman authorization. \n\n*Background*: schematic uses Google’s API to generate google sheet templates that users fill in to provide (meta)data.\nMost Google sheet functionality could be authenticated with service account. However, more complex Google sheet functionality\nrequires token-based authentication. As browser support that requires the token-based authentication diminishes, we are hoping to deprecate\ntoken-based authentication and keep only service account authentication in the future. \n\n\n### Development process instruction\n\nFor new features, bugs, enhancements\n\n1. Pull the latest code from [develop branch in the upstream repo](https://github.com/Sage-Bionetworks/schematic)\n2. Checkout a new branch develop-<feature/fix-name> from the develop branch\n3. Do development on branch develop-<feature/fix-name>\n   a. may need to ensure that schematic poetry toml and lock files are compatible with your local environment\n4. Add changed files for tracking and commit changes using [best practices](https://www.perforce.com/blog/vcs/git-best-practices-git-commit)\n5. Have granular commits: not “too many” file changes, and not hundreds of code lines of changes\n6. Commits with work in progress are encouraged:\n   a. add WIP to the beginning of the commit message for “Work In Progress” commits\n7. Keep commit messages descriptive but less than a page long, see best practices\n8. Push code to develop-<feature/fix-name> in upstream repo\n9. Branch out off develop-<feature/fix-name> if needed to work on multiple features associated with the same code base\n10. After feature work is complete and before creating a PR to the develop branch in upstream\n    a. ensure that code runs locally\n    b. test for logical correctness locally\n    c. wait for git workflow to complete (e.g. tests are run) on github\n11. Create a PR from develop-<feature/fix-name> into the develop branch of the upstream repo\n12. Request a code review on the PR\n13. Once code is approved merge in the develop branch\n14. Delete the develop-<feature/fix-name> branch\n\n*Note*: Make sure you have the latest version of the `develop` branch on your local machine.\n\n## Installation Guide - Docker \n\n1. Install docker from https://www.docker.com/ . <br>\n2.  Identify docker image of interest from [Schematic DockerHub](https://hub.docker.com/r/sagebionetworks/schematic/tags) <br>\n    Ex `docker pull sagebionetworks/schematic:latest` from the CLI or, run `docker compose up` after cloning the schematic github repo <br>\n    in this case, `sagebionetworks/schematic:latest` is the name of the image chosen\n3. Run Schematic Command with `docker run <flags> <schematic command and args>`. <br>\n<t> - For more information on flags for `docker run` and what they do, visit the [Docker Documentation](https://docs.docker.com/engine/reference/commandline/run/) <br>\n<t> - These example commands assume that you have navigated to the directory you want to run schematic from. To specify your working directory, use `$(pwd)` on MacOS/Linux or `%cd%` on Windows.  <br>\n<t> - If not using the latest image, then the full name should be specified: ie `sagebionetworks/schematic:commit-e611e4a` <br>\n<t> - If using local image created by `docker compose up`, then the docker image name should be changed: i.e. `schematic_schematic` <br>\n<t> - Using the `--name` flag sets the name of the container running locally on your machine <br>\n\n### Example For REST API <br>\n\n#### Use file path of `config.yml` to run API endpoints: \n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n#### Use content of `config.yml` and `schematic_service_account_creds.json`as an environment variable to run API endpoints: \n1. save content of `config.yml` as to environment variable `SCHEMATIC_CONFIG_CONTENT` by doing: `export SCHEMATIC_CONFIG_CONTENT=$(cat /path/to/config.yml)`\n\n2. Similarly, save the content of `schematic_service_account_creds.json` as `SERVICE_ACCOUNT_CREDS` by doing: `export SERVICE_ACCOUNT_CREDS=$(cat /path/to/schematic_service_account_creds.json)`\n\n3. Pass `SCHEMATIC_CONFIG_CONTENT` and `schematic_service_account_creds` as environment variables by using `docker run`\n\n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  -e SCHEMATIC_CONFIG_CONTENT=$SCHEMATIC_CONFIG_CONTENT \\\n  -e SERVICE_ACCOUNT_CREDS=$SERVICE_ACCOUNT_CREDS \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n\n### Example For Schematic on mac/linux <br>\nTo run example below, first clone schematic into your home directory  `git clone https://github.com/sage-bionetworks/schematic ~/schematic` <br>\nThen update .synapseConfig with your credentials\n```\ndocker run \\\n  -v ~/schematic:/schematic \\\n  -w /schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic schematic model \\\n  -c /schematic/config.yml validate \\\n  -mp /schematic/tests/data/mock_manifests/Valid_Test_Manifest.csv \\\n  -dt MockComponent \\\n  -js /schematic/tests/data/example.model.jsonld\n``` \n\n### Example For Schematic on Windows <br>\n```\ndocker run -v %cd%:/schematic \\\n  -w /schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  schematic model \\\n  -c config.yml validate -mp tests/data/mock_manifests/inValid_Test_Manifest.csv -dt MockComponent -js /schematic/data/example.model.jsonld\n```\n\n# Other Contribution Guidelines\n## Updating readthedocs documentation\n1. `cd docs`\n2. After making relevant changes, you could run the `make html` command to re-generate the `build` folder.\n3. Please contact the dev team to publish your updates\n\n*Other helpful resources*:\n\n1. [Getting started with Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n2. [Installing Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n\n## Update toml file and lock file\nIf you install external libraries by using `poetry add <name of library>`, please make sure that you include `pyproject.toml` and `poetry.lock` file in your commit.\n\n## Reporting bugs or feature requests\nYou can **create bug and feature requests** through [Sage Bionetwork\'s FAIR Data service desk](https://sagebionetworks.jira.com/servicedesk/customer/portal/5/group/8). Providing enough details to the developers to verify and troubleshoot your issue is paramount:\n- **Provide a clear and descriptive title as well as a concise summary** of the issue to identify the problem.\n- **Describe the exact steps which reproduce the problem** in as many details as possible.\n- **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.\n- **Explain which behavior you expected to see** instead and why.\n- **Provide screenshots of the expected or actual behaviour** where applicable.\n\n# Command Line Usage\nPlease visit more documentation [here](https://sage-schematic.readthedocs.io/en/develop/cli_reference.html)\n\n\n\n# Testing \n\nAll code added to the client must have tests. The Python client uses pytest to run tests. The test code is located in the [tests](https://github.com/Sage-Bionetworks/schematic/tree/develop-docs-update/tests) subdirectory.\n\nYou can run the test suite in the following way:\n\n```\npytest -vs tests/\n```\n\n## Updating Synapse test resources\n\n1. Duplicate the entity being updated (or folder if applicable).\n2. Edit the duplicates (_e.g._ annotations, contents, name).\n3. Update the test suite in your branch to use these duplicates, including the expected values in the test assertions.\n4. Open a PR as per the usual process (see above).\n5. Once the PR is merged, leave the original copies on Synapse to maintain support for feature branches that were forked from `develop` before your update.\n   - If the old copies are problematic and need to be removed immediately (_e.g._ contain sensitive data), proceed with the deletion and alert the other contributors that they need to merge the latest `develop` branch into their feature branches for their tests to work.\n\n# Code style\n\n* Please consult the [Google Python style guide](http://google.github.io/styleguide/pyguide.html) prior to contributing code to this project.\n* Be consistent and follow existing code conventions and spirit.\n\n\n# Contributors\n\nMain contributors and developers:\n\n- [Milen Nikolov](https://github.com/milen-sage)\n- [Mialy DeFelice](https://github.com/mialy-defelice)\n- [Sujay Patil](https://github.com/sujaypatil96)\n- [Bruno Grande](https://github.com/BrunoGrandePhD)\n- [Robert Allaway](https://github.com/allaway)\n- [Gianna Jordan](https://github.com/giajordan)\n- [Lingling Peng](https://github.com/linglp)\n',
+    'long_description': '# Schematic\n[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FSage-Bionetworks%2Fschematic%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/Sage-Bionetworks/schematic/goto?ref=develop) [![Documentation Status](https://readthedocs.org/projects/sage-schematic/badge/?version=develop)](https://sage-schematic.readthedocs.io/en/develop/?badge=develop) [![PyPI version](https://badge.fury.io/py/schematicpy.svg)](https://badge.fury.io/py/schematicpy)\n\n# Table of contents\n- [Introduction](#introduction)\n- [Installation](#installation)\n  - [Installation Requirements](#installation-requirements)\n  - [Installation guide for data curator app](#installation-guide-for-data-curator-app)\n  - [Installation guide for developers/contributors](#installation-guide-for-developerscontributors)\n- [Other Contribution Guidelines](#other-contribution-guidelines)\n    - [Update readthedocs documentation](#update-readthedocs-documentation)\n- [Command Line Usage](#command-line-usage)\n- [Testing](#testing)\n  - [Updating Synapse test resources](#updating-synapse-test-resources)\n- [Code Style](#code-style)\n- [Contributors](#contributors)\n\n# Introduction\nSCHEMATIC is an acronym for _Schema Engine for Manifest Ingress and Curation_. The Python based infrastructure provides a _novel_ schema-based, metadata ingress ecosystem, that is meant to streamline the process of biomedical dataset annotation, metadata validation and submission to a data repository for various data contributors.\n\n# Installation\n## Installation Requirements\n* Python version 3.9.0≤x<3.11.0 \n\nNote: You need to be a registered and certified user on [`synapse.org`](https://www.synapse.org/), and also have the right permissions to download the Google credentials files from Synapse.\n\n\n## Installation guide for data curator app\n\nCreate and activate a virtual environment within which you can install the package:\n\n```\npython3 -m venv .venv\nsource .venv/bin/activate\n```\n\nNote: Python 3 has a built-in support for virtual environment [venv](https://docs.python.org/3/library/venv.html#module-venv) so you no longer need to install virtualenv.\n\nInstall and update the package using [pip](https://pip.pypa.io/en/stable/quickstart/):\n\n```\npython3 -m pip install schematicpy\n```\n\nIf you run into error: Failed building wheel for numpy, the error might be able to resolve by upgrading pip. Please try to upgrade pip by:\n\n```\npip3 install --upgrade pip\n```\n\n## Installation guide for developers/contributors \n\nWhen contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the owners of this repository before making a change.\n\nPlease note we have a [code of conduct](CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.\n\n### Development environment setup\n1. Clone the `schematic` package repository.\n```\ngit clone https://github.com/Sage-Bionetworks/schematic.git\n```\n2. Install `poetry` (version 1.3.0 or later) using either the [official installer](https://python-poetry.org/docs/#installing-with-the-official-installer) or [pipx](https://python-poetry.org/docs/#installing-with-pipx). If you have an older installation of Poetry, we recommend uninstalling it first. \n\n3. Start the virtual environment by doing: \n```\npoetry shell\n```\n4. Install the dependencies by doing: \n```\npoetry install\n```\nThis command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)\n\nIf you want to install the API you will need to install those dependencies as well:\n\n```\npoetry install --extras "api"\n```\n\nIf you want to install the uwsgi:\n\n```\npoetry install --extras "api"\n```\n\n5. Fill in credential files: \n*Note*: If you won\'t interact with Synapse, please ignore this section.\n\nThere are two main configuration files that need to be edited:\nconfig.yml\nand [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)\n\n<strong>Configure .synapseConfig File</strong>\n\nDownload a copy of the ``.synapseConfig`` file, open the file in the\neditor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section \n\n*Note*: You could also visit [configparser](https://docs.python.org/3/library/configparser.html#module-configparser>) doc to see the format that `.synapseConfig` must have. For instance:\n>[authentication]<br> username = ABC <br> authtoken = abc\n\n<strong>Configure config.yml File</strong>\n\nThere are some defaults in schematic that can be configured. These fields are in ``config_example.yml``:\n\n```text\n\n# This is an example config for Schematic.\n# All listed values are those that are the default if a config is not used.\n# Save this as config.yml, this will be gitignored.\n# Remove any fields in the config you don\'t want to change\n# Change the values of any fields you do want to change\n\n\n# This describes where assets such as manifests are stored\nasset_store:\n  # This is when assets are stored in a synapse project\n  synapse:\n    # Synapse ID of the file view listing all project data assets.\n    master_fileview_id: "syn23643253"\n    # Path to the synapse config file, either absolute or relative to this file\n    config: ".synapseConfig"\n    # Base name that manifest files will be saved as\n    manifest_basename: "synapse_storage_manifest"\n\n# This describes information about manifests as it relates to generation and validation\nmanifest:\n  # Location where manifests will saved to\n  manifest_folder: "manifests"\n  # Title or title prefix given to generated manifest(s)\n  title: "example"\n  # Data types of manifests to be generated or data type (singular) to validate manifest against\n  data_type:\n    - "Biospecimen"\n    - "Patient"\n\n# Describes the location of your schema\nmodel:\n  # Location of your schema jsonld, it must be a path relative to this file or absolute\n  location: "tests/data/example.model.jsonld"\n\n# This section is for using google sheets with Schematic\ngoogle_sheets:\n  # The Synapse id of the Google service account credentials.\n  service_acct_creds_synapse_id: "syn25171627"\n  # Path to the synapse config file, either absolute or relative to this file\n  service_acct_creds: "schematic_service_account_creds.json"\n  # When doing google sheet validation (regex match) with the validation rules.\n  #   true is alerting the user and not allowing entry of bad values.\n  #   false is warning but allowing the entry on to the sheet.\n  strict_validation: true\n```\n\nIf you want to change any of these copy ``config_example.yml`` to ``config.yml``, change any fields you want to, and remove any fields you don\'t.\n\nFor example if you wanted to change the folder where manifests are downloaded your config should look like:\n\n```text\n\nmanifest:\n  manifest_folder: "my_manifest_folder_path"\n```\n\n_Note_: `config.yml` is ignored by git.\n\n_Note_: Paths can be specified relative to the `config.yml` file or as absolute paths.\n\n6. Login to Synapse by using the command line\nOn the CLI in your virtual environment, run the following command: \n```\nsynapse login -u <synapse username> -p <synapse password> --rememberMe\n```\nPlease make sure that you run the command before running `schematic init` below\n\n7. Obtain Google credential Files\nTo obtain  ``schematic_service_account_creds.json``, please run: \n```\nschematic init --config ~/path/to/config.yml\n```\n> As v22.12.1 version of schematic, using `token` mode of authentication (in other words, using `token.pickle` and `credentials.json`) is no longer supported due to Google\'s decision to move away from using OAuth out-of-band (OOB) flow. Click [here](https://developers.google.com/identity/protocols/oauth2/resources/oob-migration) to learn more. \n\n*Notes*: Use the ``schematic_service_account_creds.json`` file for the service\naccount mode of authentication (*for Google services/APIs*). Service accounts \nare special Google accounts that can be used by applications to access Google APIs \nprogrammatically via OAuth2.0, with the advantage being that they do not require \nhuman authorization. \n\n*Background*: schematic uses Google’s API to generate google sheet templates that users fill in to provide (meta)data.\nMost Google sheet functionality could be authenticated with service account. However, more complex Google sheet functionality\nrequires token-based authentication. As browser support that requires the token-based authentication diminishes, we are hoping to deprecate\ntoken-based authentication and keep only service account authentication in the future. \n\n\n### Development process instruction\n\nFor new features, bugs, enhancements\n\n1. Pull the latest code from [develop branch in the upstream repo](https://github.com/Sage-Bionetworks/schematic)\n2. Checkout a new branch develop-<feature/fix-name> from the develop branch\n3. Do development on branch develop-<feature/fix-name>\n   a. may need to ensure that schematic poetry toml and lock files are compatible with your local environment\n4. Add changed files for tracking and commit changes using [best practices](https://www.perforce.com/blog/vcs/git-best-practices-git-commit)\n5. Have granular commits: not “too many” file changes, and not hundreds of code lines of changes\n6. Commits with work in progress are encouraged:\n   a. add WIP to the beginning of the commit message for “Work In Progress” commits\n7. Keep commit messages descriptive but less than a page long, see best practices\n8. Push code to develop-<feature/fix-name> in upstream repo\n9. Branch out off develop-<feature/fix-name> if needed to work on multiple features associated with the same code base\n10. After feature work is complete and before creating a PR to the develop branch in upstream\n    a. ensure that code runs locally\n    b. test for logical correctness locally\n    c. wait for git workflow to complete (e.g. tests are run) on github\n11. Create a PR from develop-<feature/fix-name> into the develop branch of the upstream repo\n12. Request a code review on the PR\n13. Once code is approved merge in the develop branch\n14. Delete the develop-<feature/fix-name> branch\n\n*Note*: Make sure you have the latest version of the `develop` branch on your local machine.\n\n## Installation Guide - Docker \n\n1. Install docker from https://www.docker.com/ . <br>\n2.  Identify docker image of interest from [Schematic DockerHub](https://hub.docker.com/r/sagebionetworks/schematic/tags) <br>\n    Ex `docker pull sagebionetworks/schematic:latest` from the CLI or, run `docker compose up` after cloning the schematic github repo <br>\n    in this case, `sagebionetworks/schematic:latest` is the name of the image chosen\n3. Run Schematic Command with `docker run <flags> <schematic command and args>`. <br>\n<t> - For more information on flags for `docker run` and what they do, visit the [Docker Documentation](https://docs.docker.com/engine/reference/commandline/run/) <br>\n<t> - These example commands assume that you have navigated to the directory you want to run schematic from. To specify your working directory, use `$(pwd)` on MacOS/Linux or `%cd%` on Windows.  <br>\n<t> - If not using the latest image, then the full name should be specified: ie `sagebionetworks/schematic:commit-e611e4a` <br>\n<t> - If using local image created by `docker compose up`, then the docker image name should be changed: i.e. `schematic_schematic` <br>\n<t> - Using the `--name` flag sets the name of the container running locally on your machine <br>\n\n### Example For REST API <br>\n\n#### Use file path of `config.yml` to run API endpoints: \n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n#### Use content of `config.yml` and `schematic_service_account_creds.json`as an environment variable to run API endpoints: \n1. save content of `config.yml` as to environment variable `SCHEMATIC_CONFIG_CONTENT` by doing: `export SCHEMATIC_CONFIG_CONTENT=$(cat /path/to/config.yml)`\n\n2. Similarly, save the content of `schematic_service_account_creds.json` as `SERVICE_ACCOUNT_CREDS` by doing: `export SERVICE_ACCOUNT_CREDS=$(cat /path/to/schematic_service_account_creds.json)`\n\n3. Pass `SCHEMATIC_CONFIG_CONTENT` and `schematic_service_account_creds` as environment variables by using `docker run`\n\n```\ndocker run --rm -p 3001:3001 \\\n  -v $(pwd):/schematic -w /schematic --name schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  -e SCHEMATIC_CONFIG_CONTENT=$SCHEMATIC_CONFIG_CONTENT \\\n  -e SERVICE_ACCOUNT_CREDS=$SERVICE_ACCOUNT_CREDS \\\n  sagebionetworks/schematic \\\n  python /usr/src/app/run_api.py\n``` \n\n\n### Example For Schematic on mac/linux <br>\nTo run example below, first clone schematic into your home directory  `git clone https://github.com/sage-bionetworks/schematic ~/schematic` <br>\nThen update .synapseConfig with your credentials\n```\ndocker run \\\n  -v ~/schematic:/schematic \\\n  -w /schematic \\\n  -e SCHEMATIC_CONFIG=/schematic/config.yml \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic schematic model \\\n  -c /schematic/config.yml validate \\\n  -mp /schematic/tests/data/mock_manifests/Valid_Test_Manifest.csv \\\n  -dt MockComponent \\\n  -js /schematic/tests/data/example.model.jsonld\n``` \n\n### Example For Schematic on Windows <br>\n```\ndocker run -v %cd%:/schematic \\\n  -w /schematic \\\n  -e GE_HOME=/usr/src/app/great_expectations/ \\\n  sagebionetworks/schematic \\\n  schematic model \\\n  -c config.yml validate -mp tests/data/mock_manifests/inValid_Test_Manifest.csv -dt MockComponent -js /schematic/data/example.model.jsonld\n```\n\n# Other Contribution Guidelines\n## Updating readthedocs documentation\n1. `cd docs`\n2. After making relevant changes, you could run the `make html` command to re-generate the `build` folder.\n3. Please contact the dev team to publish your updates\n\n*Other helpful resources*:\n\n1. [Getting started with Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n2. [Installing Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)\n\n## Update toml file and lock file\nIf you install external libraries by using `poetry add <name of library>`, please make sure that you include `pyproject.toml` and `poetry.lock` file in your commit.\n\n## Reporting bugs or feature requests\nYou can **create bug and feature requests** through [Sage Bionetwork\'s FAIR Data service desk](https://sagebionetworks.jira.com/servicedesk/customer/portal/5/group/8). Providing enough details to the developers to verify and troubleshoot your issue is paramount:\n- **Provide a clear and descriptive title as well as a concise summary** of the issue to identify the problem.\n- **Describe the exact steps which reproduce the problem** in as many details as possible.\n- **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.\n- **Explain which behavior you expected to see** instead and why.\n- **Provide screenshots of the expected or actual behaviour** where applicable.\n\n# Command Line Usage\nPlease visit more documentation [here](https://sage-schematic.readthedocs.io/en/develop/cli_reference.html)\n\n\n\n# Testing \n\nAll code added to the client must have tests. The Python client uses pytest to run tests. The test code is located in the [tests](https://github.com/Sage-Bionetworks/schematic/tree/develop-docs-update/tests) subdirectory.\n\nYou can run the test suite in the following way:\n\n```\npytest -vs tests/\n```\n\n## Updating Synapse test resources\n\n1. Duplicate the entity being updated (or folder if applicable).\n2. Edit the duplicates (_e.g._ annotations, contents, name).\n3. Update the test suite in your branch to use these duplicates, including the expected values in the test assertions.\n4. Open a PR as per the usual process (see above).\n5. Once the PR is merged, leave the original copies on Synapse to maintain support for feature branches that were forked from `develop` before your update.\n   - If the old copies are problematic and need to be removed immediately (_e.g._ contain sensitive data), proceed with the deletion and alert the other contributors that they need to merge the latest `develop` branch into their feature branches for their tests to work.\n\n# Code style\n\n* Please consult the [Google Python style guide](http://google.github.io/styleguide/pyguide.html) prior to contributing code to this project.\n* Be consistent and follow existing code conventions and spirit.\n\n\n# Contributors\n\nMain contributors and developers:\n\n- [Milen Nikolov](https://github.com/milen-sage)\n- [Mialy DeFelice](https://github.com/mialy-defelice)\n- [Sujay Patil](https://github.com/sujaypatil96)\n- [Bruno Grande](https://github.com/BrunoGrandePhD)\n- [Robert Allaway](https://github.com/allaway)\n- [Gianna Jordan](https://github.com/giajordan)\n- [Lingling Peng](https://github.com/linglp)\n',
     'author': 'Milen Nikolov',
     'author_email': 'milen.nikolov@sagebase.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Sage-Bionetworks/schematic',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `schematicpy-24.1.1/PKG-INFO` & `schematicpy-24.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: schematicpy
-Version: 24.1.1
+Version: 24.2.1
 Summary: Package for biomedical data model and metadata ingress management
 Home-page: https://github.com/Sage-Bionetworks/schematic
 Keywords: schema,metadata,validation,data model,linked data
 Author: Milen Nikolov
 Author-email: milen.nikolov@sagebase.org
 Requires-Python: >=3.9.0,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Flask (>=2.0.0,<3.0.0)
-Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
-Requires-Dist: Jinja2 (>2.11.3)
+Provides-Extra: api
+Provides-Extra: aws
+Requires-Dist: Flask (>=2.0.0,<3.0.0) ; extra == "api"
+Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0) ; extra == "api"
+Requires-Dist: Jinja2 (>2.11.3) ; extra == "api"
 Requires-Dist: MarkupSafe (==2.1.0)
 Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: backports.zoneinfo (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
-Requires-Dist: connexion[swagger-ui] (>=2.8.0,<3.0.0)
+Requires-Dist: connexion[swagger-ui] (>=2.8.0,<3.0.0) ; extra == "api"
 Requires-Dist: dataclasses-json (>=0.6.1,<0.7.0)
 Requires-Dist: dateparser (>=1.1.4,<2.0.0)
 Requires-Dist: google-api-python-client (>=2.0.0,<3.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
 Requires-Dist: google-auth-oauthlib (>=0.8.0,<0.9.0)
 Requires-Dist: graphviz (>=0.20.0,<0.21.0)
 Requires-Dist: great-expectations (>=0.15.0,<0.16.0)
@@ -34,26 +36,27 @@
 Requires-Dist: itsdangerous (>=2.0.0,<3.0.0)
 Requires-Dist: jsonschema (>=4.0.0,<5.0.0)
 Requires-Dist: networkx (>=2.2.8)
 Requires-Dist: numpy (>=1.21.1,<2.0.0)
 Requires-Dist: oauth2client (>=4.1.0,<5.0.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Requires-Dist: pandarallel (>=1.6.4,<2.0.0)
-Requires-Dist: pandas (>=1.3.1,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pdoc (>=12.2.0,<13.0.0)
 Requires-Dist: pygsheets (>=2.0.4,<3.0.0)
 Requires-Dist: pyopenssl (>=23.0.0,<24.0.0)
 Requires-Dist: rdflib (>=6.0.0,<7.0.0)
-Requires-Dist: schematic-db[synapse] (==0.0.dev33)
+Requires-Dist: schematic-db[synapse] (==0.0.34)
 Requires-Dist: setuptools (>=66.0.0,<67.0.0)
 Requires-Dist: sphinx-click (>=4.0.0,<5.0.0)
-Requires-Dist: synapseclient (>=3.1.1,<4.0.0)
+Requires-Dist: synapseclient (>=3.2.0,<4.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typing-extensions (<4.6.0)
+Requires-Dist: uWSGI (>=2.0.21,<3.0.0) ; extra == "aws"
 Project-URL: Documentation, https://github.com/Sage-Bionetworks/schematic
 Project-URL: Repository, https://github.com/Sage-Bionetworks/schematic
 Description-Content-Type: text/markdown
 
 # Schematic
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FSage-Bionetworks%2Fschematic%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/Sage-Bionetworks/schematic/goto?ref=develop) [![Documentation Status](https://readthedocs.org/projects/sage-schematic/badge/?version=develop)](https://sage-schematic.readthedocs.io/en/develop/?badge=develop) [![PyPI version](https://badge.fury.io/py/schematicpy.svg)](https://badge.fury.io/py/schematicpy)
 
@@ -123,14 +126,26 @@
 ```
 4. Install the dependencies by doing: 
 ```
 poetry install
 ```
 This command will install the dependencies based on what we specify in poetry.lock. If this step is taking a long time, try to go back to step 2 and check your version of poetry. Alternatively, you could also try deleting the lock file and regenerate it by doing `poetry install` (Please note this method should be used as a last resort because this would force other developers to change their development environment)
 
+If you want to install the API you will need to install those dependencies as well:
+
+```
+poetry install --extras "api"
+```
+
+If you want to install the uwsgi:
+
+```
+poetry install --extras "api"
+```
+
 5. Fill in credential files: 
 *Note*: If you won't interact with Synapse, please ignore this section.
 
 There are two main configuration files that need to be edited:
 config.yml
 and [synapseConfig](https://raw.githubusercontent.com/Sage-Bionetworks/synapsePythonClient/v2.3.0-rc/synapseclient/.synapseConfig)
```

