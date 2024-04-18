# Comparing `tmp/kiara_plugin_core_types-0.5.1.tar.gz` & `tmp/kiara_plugin_core_types-0.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin_core_types-0.5.1.tar", last modified: Thu Apr 18 08:44:39 2024, max compression
+gzip compressed data, was "kiara_plugin_core_types-0.5.1rc1.tar", last modified: Mon Apr 15 13:40:31 2024, max compression
```

## Comparing `kiara_plugin_core_types-0.5.1.tar` & `kiara_plugin_core_types-0.5.1rc1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.153608 kiara_plugin_core_types-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.133608 kiara_plugin_core_types-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.141608 kiara_plugin_core_types-0.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.141608 kiara_plugin_core_types-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-18 08:44:39.153608 kiara_plugin_core_types-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.133608 kiara_plugin_core_types-0.5.1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.141608 kiara_plugin_core_types-0.5.1/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.141608 kiara_plugin_core_types-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/docs/SUMMARY.md.rej
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.141608 kiara_plugin_core_types-0.5.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.133608 kiara_plugin_core_types-0.5.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.141608 kiara_plugin_core_types-0.5.1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.141608 kiara_plugin_core_types-0.5.1/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33121 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.141608 kiara_plugin_core_types-0.5.1/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/jobs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/jobs/check_date_in_range.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/jobs/check_date_in_range_string_inputs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/jobs/logic_and_false.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/jobs/logic_and_true.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/jobs/logic_xor_false.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/jobs/logic_xor_true.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/jobs/parse_date_1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.145608 kiara_plugin_core_types-0.5.1/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/examples/pipelines/example_pipeline_core_types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/pixi.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.133608 kiara_plugin_core_types-0.5.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.145608 kiara_plugin_core_types-0.5.1/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 08:44:39.153608 kiara_plugin_core_types-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.133608 kiara_plugin_core_types-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.133608 kiara_plugin_core_types-0.5.1/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.145608 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.145608 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/data_types/
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/data_types/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.145608 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.145608 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/pipelines/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/pipelines/logic/nand.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/pipelines/logic/nor.json
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/pipelines/logic/xor.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/renderers/lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/src/kiara_plugin.core_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-18 08:44:39.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin.core_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-18 08:44:39.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin.core_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 08:44:39.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin.core_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-18 08:44:39.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin.core_types.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 08:44:39.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin.core_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 08:44:39.000000 kiara_plugin_core_types-0.5.1/src/kiara_plugin.core_types.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.137608 kiara_plugin_core_types-0.5.1/tests/job_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/job_tests/check_date_in_range/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/job_tests/check_date_in_range/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/job_tests/check_date_in_range_string_inputs/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/job_tests/check_date_in_range_string_inputs/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/job_tests/logic_and_false/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/job_tests/logic_and_false/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/job_tests/logic_and_true/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/job_tests/logic_and_true/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/job_tests/logic_xor_false/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/job_tests/logic_xor_false/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/job_tests/logic_xor_true/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/job_tests/logic_xor_true/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/job_tests/parse_date_fail/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/job_tests/parse_date_fail/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/job_tests/parse_date_fail/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/resources/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/resources/jobs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/resources/jobs/init.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/resources/jobs/parse_date_fail.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:39.149608 kiara_plugin_core_types-0.5.1/tests/resources/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/resources/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/resources/pipelines/init.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      236 2024-04-18 08:44:34.000000 kiara_plugin_core_types-0.5.1/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/SUMMARY.md.rej
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33121 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/check_date_in_range.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/check_date_in_range_string_inputs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/logic_and_false.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/logic_and_true.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/logic_xor_false.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/logic_xor_true.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/parse_date_1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/pipelines/example_pipeline_core_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/nand.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/nor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/xor.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/renderers/lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/check_date_in_range/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/check_date_in_range/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/check_date_in_range_string_inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/check_date_in_range_string_inputs/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_and_false/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_and_false/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_and_true/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_and_true/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_xor_false/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_xor_false/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_xor_true/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_xor_true/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/parse_date_fail/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/parse_date_fail/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/parse_date_fail/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/tests/resources/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/jobs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/jobs/init.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/jobs/parse_date_fail.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/tests/resources/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/pipelines/init.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      236 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin_core_types-0.5.1/.cruft.json` & `kiara_plugin_core_types-0.5.1rc1/.cruft.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'61841496d46e8ce4f79da1126443524bde03f977'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "540151144e37354aa9290776b38adbcd96a97a26",
+    "commit": "61841496d46e8ce4f79da1126443524bde03f977",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin_core_types-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/.github/workflows/build-darwin.yaml` & `kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/.github/workflows/build-linux.yaml` & `kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/.github/workflows/build-windows.yaml` & `kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/.gitignore` & `kiara_plugin_core_types-0.5.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/.pre-commit-config.yaml` & `kiara_plugin_core_types-0.5.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/LICENSE` & `kiara_plugin_core_types-0.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/Makefile` & `kiara_plugin_core_types-0.5.1rc1/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/PKG-INFO` & `kiara_plugin_core_types-0.5.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.core_types
-Version: 0.5.1
+Version: 0.5.1rc1
 Summary: Core data types for kiara.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.core_types
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.core_types
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.core_types
 Keywords: kiara
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: kiara<0.6.0,>=0.5.10
+Requires-Dist: kiara==0.5.10rc10
 Requires-Dist: python-dateutil>=2.8.0
 Provides-Extra: dev-documentation
 Requires-Dist: kiara[dev_documentation]; extra == "dev-documentation"
 Provides-Extra: dev-testing
 Requires-Dist: kiara[dev_testing]; extra == "dev-testing"
 Provides-Extra: dev-utils
 Requires-Dist: kiara[dev_utils]; extra == "dev-utils"
```

### Comparing `kiara_plugin_core_types-0.5.1/README.md` & `kiara_plugin_core_types-0.5.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/docs/index.md` & `kiara_plugin_core_types-0.5.1rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin_core_types-0.5.1rc1/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin_core_types-0.5.1rc1/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/examples/pipelines/example_pipeline_core_types.yaml` & `kiara_plugin_core_types-0.5.1rc1/examples/pipelines/example_pipeline_core_types.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/mkdocs.yml` & `kiara_plugin_core_types-0.5.1rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/pixi.toml` & `kiara_plugin_core_types-0.5.1rc1/pixi.toml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/pyproject.toml` & `kiara_plugin_core_types-0.5.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-    "kiara>=0.5.10,<0.6.0",
+    "kiara==0.5.10rc10",
     "python-dateutil>=2.8.0",
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
```

### Comparing `kiara_plugin_core_types-0.5.1/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/scripts/documentation/gen_info_pages.py` & `kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/scripts/documentation/gen_module_doc.py` & `kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/__init__.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/data_types/__init__.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/data_types/models.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/models.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/__init__.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/boolean.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/boolean.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/date.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/date.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/list.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/list.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/models.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/modules/string.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/string.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/pipelines/logic/xor.json` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/xor.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin/core_types/renderers/lineage.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/renderers/lineage.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin.core_types.egg-info/PKG-INFO` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.core_types
-Version: 0.5.1
+Version: 0.5.1rc1
 Summary: Core data types for kiara.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.core_types
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.core_types
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.core_types
 Keywords: kiara
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: kiara<0.6.0,>=0.5.10
+Requires-Dist: kiara==0.5.10rc10
 Requires-Dist: python-dateutil>=2.8.0
 Provides-Extra: dev-documentation
 Requires-Dist: kiara[dev_documentation]; extra == "dev-documentation"
 Provides-Extra: dev-testing
 Requires-Dist: kiara[dev_testing]; extra == "dev-testing"
 Provides-Extra: dev-utils
 Requires-Dist: kiara[dev_utils]; extra == "dev-utils"
```

### Comparing `kiara_plugin_core_types-0.5.1/src/kiara_plugin.core_types.egg-info/SOURCES.txt` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/tests/conftest.py` & `kiara_plugin_core_types-0.5.1rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_core_types-0.5.1/tests/test_job_descs.py` & `kiara_plugin_core_types-0.5.1rc1/tests/test_job_descs.py`

 * *Files identical despite different names*

