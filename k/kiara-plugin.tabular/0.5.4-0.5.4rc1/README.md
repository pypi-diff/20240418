# Comparing `tmp/kiara_plugin_tabular-0.5.4.tar.gz` & `tmp/kiara_plugin_tabular-0.5.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin_tabular-0.5.4.tar", last modified: Thu Apr 18 09:10:32 2024, max compression
+gzip compressed data, was "kiara_plugin_tabular-0.5.4rc1.tar", last modified: Mon Apr 15 14:10:11 2024, max compression
```

## Comparing `kiara_plugin_tabular-0.5.4.tar` & `kiara_plugin_tabular-0.5.4rc1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.107871 kiara_plugin_tabular-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.115871 kiara_plugin_tabular-0.5.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.115871 kiara_plugin_tabular-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.107871 kiara_plugin_tabular-0.5.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.115871 kiara_plugin_tabular-0.5.4/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.115871 kiara_plugin_tabular-0.5.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.119871 kiara_plugin_tabular-0.5.4/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.111871 kiara_plugin_tabular-0.5.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.119871 kiara_plugin_tabular-0.5.4/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.119871 kiara_plugin_tabular-0.5.4/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33121 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.119871 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.111871 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.119871 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/
--rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18280 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18481 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18620 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18698 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.119871 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/
--rw-r--r--   0 runner    (1001) docker     (127)    19397 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20647 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21017 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.123871 kiara_plugin_tabular-0.5.4/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/assemble_tables_1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/assemble_tables_2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/assemble_tables_3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/corpus_onboarding_small.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/create_table_from_file.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/create_tables_from_file_bundle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/import_journal_nodes_table.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/init.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/pick_column_from_tables.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/jobs/pick_table_from_tables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.123871 kiara_plugin_tabular-0.5.4/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/pipelines/corpus_onboarding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/pipelines/database_from_csv_files.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/pipelines/import.table.from.local_folder_path_ignore_errors.json
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/pipelines/init.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/examples/pipelines/tables_from_csv_files.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/pixi.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.111871 kiara_plugin_tabular-0.5.4/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.123871 kiara_plugin_tabular-0.5.4/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.111871 kiara_plugin_tabular-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.111871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.123871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/array/
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/array/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/db/
--rw-r--r--   0 runner    (1001) docker     (127)    21619 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/table/
--rw-r--r--   0 runner    (1001) docker     (127)    30077 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/table/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/tables/
--rw-r--r--   0 runner    (1001) docker     (127)    16968 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.json
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.json
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.json
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.127871 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/src/kiara_plugin.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-18 09:10:32.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-18 09:10:32.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:10:32.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-18 09:10:32.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin.tabular.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-18 09:10:32.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 09:10:32.000000 kiara_plugin_tabular-0.5.4/src/kiara_plugin.tabular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.111871 kiara_plugin_tabular-0.5.4/tests/job_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/job_tests/assemble_tables_1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/assemble_tables_1/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/job_tests/assemble_tables_2/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/assemble_tables_2/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/job_tests/assemble_tables_3/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/assemble_tables_3/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/job_tests/corpus_onboarding_small/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/corpus_onboarding_small/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/job_tests/create_table_from_file/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/create_table_from_file/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/job_tests/create_tables_from_file_bundle/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/create_tables_from_file_bundle/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/create_tables_from_file_bundle/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/job_tests/import_journal_nodes_table/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/import_journal_nodes_table/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/job_tests/pick_column_from_tables/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/pick_column_from_tables/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/job_tests/pick_table_from_tables/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/job_tests/pick_table_from_tables/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/resources/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/resources/jobs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:32.131871 kiara_plugin_tabular-0.5.4/tests/resources/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/resources/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-04-18 09:10:22.000000 kiara_plugin_tabular-0.5.4/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.706406 kiara_plugin_tabular-0.5.4rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.706406 kiara_plugin_tabular-0.5.4rc1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.718406 kiara_plugin_tabular-0.5.4rc1/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33121 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.718406 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.706406 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.718406 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18280 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18481 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18620 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18698 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.718406 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/
+-rw-r--r--   0 runner    (1001) docker     (127)    19397 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20647 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21017 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.722406 kiara_plugin_tabular-0.5.4rc1/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/assemble_tables_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/assemble_tables_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/assemble_tables_3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/corpus_onboarding_small.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/create_table_from_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/create_tables_from_file_bundle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/import_journal_nodes_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/init.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/pick_column_from_tables.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/pick_table_from_tables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.722406 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/corpus_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/database_from_csv_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/import.table.from.local_folder_path_ignore_errors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/init.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/tables_from_csv_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.722406 kiara_plugin_tabular-0.5.4rc1/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.722406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/array/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/db/
+-rw-r--r--   0 runner    (1001) docker     (127)    21619 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/
+-rw-r--r--   0 runner    (1001) docker     (127)    26251 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)    16968 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.json
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_1/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_2/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_3/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_3/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/corpus_onboarding_small/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/corpus_onboarding_small/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_table_from_file/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_table_from_file/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_tables_from_file_bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_tables_from_file_bundle/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_tables_from_file_bundle/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/import_journal_nodes_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/import_journal_nodes_table/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/pick_column_from_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/pick_column_from_tables/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/pick_table_from_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/pick_table_from_tables/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/resources/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/resources/jobs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/resources/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/resources/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin_tabular-0.5.4/.cruft.json` & `kiara_plugin_tabular-0.5.4rc1/.cruft.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'61841496d46e8ce4f79da1126443524bde03f977'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "258218c6205db4125ce34a6b18a4273d31f995e7",
+    "commit": "61841496d46e8ce4f79da1126443524bde03f977",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin_tabular-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/.github/workflows/build-darwin.yaml` & `kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/.github/workflows/build-linux.yaml` & `kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/.github/workflows/build-windows.yaml` & `kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/.gitignore` & `kiara_plugin_tabular-0.5.4rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/.pre-commit-config.yaml` & `kiara_plugin_tabular-0.5.4rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/LICENSE` & `kiara_plugin_tabular-0.5.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/Makefile` & `kiara_plugin_tabular-0.5.4rc1/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/PKG-INFO` & `kiara_plugin_tabular-0.5.4rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.tabular
-Version: 0.5.4
+Version: 0.5.4rc1
 Summary: kiara data-types and modules for working with tables and databases.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.tabular
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.tabular
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.tabular
 Keywords: kiara
@@ -19,28 +19,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: kiara<0.6.0,>=0.5.10
-Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.1
+Requires-Dist: kiara<0.6.0,>=0.5.10rc10
+Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.1rc1
 Requires-Dist: duckdb<0.11.0,>=0.10.0
 Requires-Dist: pandas>=1.4.0
 Requires-Dist: polars>=0.18.0
 Requires-Dist: pyarrow>=12.0.0
 Requires-Dist: sqlalchemy>=2.0.0
 Requires-Dist: sqlalchemy-utc>=0.10.0
 Requires-Dist: sqlalchemy-utils>=0.38.0
 Requires-Dist: sqlite-utils==3.30
 Provides-Extra: dev-documentation
 Requires-Dist: kiara[dev_documentation]; extra == "dev-documentation"
 Provides-Extra: dev-testing
-Requires-Dist: kiara[dev_testing]; extra == "dev-testing"
+Requires-Dist: kiara[dev_testing]==0.5.10rc10; extra == "dev-testing"
 Requires-Dist: pandas-stubs; extra == "dev-testing"
 Provides-Extra: dev-utils
 Requires-Dist: kiara[dev_utils]; extra == "dev-utils"
 Provides-Extra: dev-all
 Requires-Dist: kiara[dev_all]; extra == "dev-all"
 Provides-Extra: streamlit
 Requires-Dist: kiara_plugin.streamlit; extra == "streamlit"
```

### Comparing `kiara_plugin_tabular-0.5.4/README.md` & `kiara_plugin_tabular-0.5.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/docs/index.md` & `kiara_plugin_tabular-0.5.4rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin_tabular-0.5.4rc1/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin_tabular-0.5.4rc1/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/jobs/init.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/jobs/init.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/pipelines/corpus_onboarding.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/pipelines/corpus_onboarding.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         source_table:
           type: table
           doc: The original table.
         date_array:
           type: array
           doc: The array containing the parsed date items.
       column_map:
-        date_array: date
-        source_table.content: content
-        source_table.file_name: file_name
+        date: date_array
+        content: source_table.content
+        file_name: source_table.file_name
     input_links:
       source_table: create_text_corpus.table
       date_array: create_date_array.date_array
 
 input_aliases:
   extract_filename_column.column_name: filename_column_name
   import_text_corpus.path: text_corpus_folder_path
```

### Comparing `kiara_plugin_tabular-0.5.4/examples/pipelines/database_from_csv_files.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/pipelines/database_from_csv_files.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/pipelines/import.table.from.local_folder_path_ignore_errors.json` & `kiara_plugin_tabular-0.5.4rc1/examples/pipelines/import.table.from.local_folder_path_ignore_errors.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/pipelines/init.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/pipelines/init.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/examples/pipelines/tables_from_csv_files.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/pipelines/tables_from_csv_files.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/mkdocs.yml` & `kiara_plugin_tabular-0.5.4rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/pixi.toml` & `kiara_plugin_tabular-0.5.4rc1/pixi.toml`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/pyproject.toml` & `kiara_plugin_tabular-0.5.4rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,34 +43,33 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-    "kiara>=0.5.10,<0.6.0",
-    "kiara_plugin.core_types>=0.5.1,<0.6.0",
+    "kiara>=0.5.10rc10,<0.6.0",
+    "kiara_plugin.core_types>=0.5.1rc1,<0.6.0",
     "duckdb>=0.10.0,<0.11.0",
     "pandas>=1.4.0",
     "polars>=0.18.0",
     "pyarrow>=12.0.0",
     "sqlalchemy>=2.0.0",
     "sqlalchemy-utc>=0.10.0",
     "sqlalchemy-utils>=0.38.0",
     "sqlite-utils==3.30",
 ]
-
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
 dev_testing = [
-    "kiara[dev_testing]",
+    "kiara[dev_testing]==0.5.10rc10",
     "pandas-stubs"
 ]
 dev_utils = [
     "kiara[dev_utils]",
 ]
 dev_all = [
     "kiara[dev_all]"
```

### Comparing `kiara_plugin_tabular-0.5.4/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/scripts/documentation/gen_info_pages.py` & `kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/scripts/documentation/gen_module_doc.py` & `kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/array.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/array.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/db.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/db.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/table.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/table.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/data_types/tables.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/tables.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/defaults.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/array.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/array.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/db.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/db.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/table.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/table.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/models/tables.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/tables.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/array/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/array/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/db/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/table/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Mapping,
     Type,
     Union,
 )
 
 from pydantic import BaseModel, Field
 
-from kiara.exceptions import KiaraException, KiaraProcessingException
+from kiara.exceptions import KiaraProcessingException
 from kiara.models.filesystem import (
     FILE_BUNDLE_IMPORT_AVAILABLE_COLUMNS,
     KiaraFile,
     KiaraFileBundle,
 )
 from kiara.models.module import KiaraModuleConfig
 from kiara.models.module.jobs import JobLog
@@ -353,159 +353,76 @@
 
     type: str = Field(description="The type of the value.")
     type_config: Dict[str, Any] = Field(
         description="Configuration for the type, in case it's complex.",
         default_factory=dict,
     )
     default: Any = Field(description="A default value.", default=None)
-    doc: str = Field(description="A description for the value of this input field.")
 
-    # optional: bool = Field(
-    #     description="Whether this value is required (True), or whether 'None' value is allowed (False).",
-    #     default=False,
-    # )
+    optional: bool = Field(
+        description="Whether this value is required (True), or whether 'None' value is allowed (False).",
+        default=False,
+    )
 
 
 class MergeTableConfig(KiaraModuleConfig):
 
     inputs_schema: Dict[str, ValueSchemaInput] = Field(
         description="A dict describing the inputs for this merge process."
     )
     column_map: Dict[str, str] = Field(
-        description="A dict describing how to map column names from inputs to the output table.",
-        default_factory=dict,
+        description="A map describing", default_factory=dict
     )
-    # ask_column_map: bool = Field(
-    #     description="Whether to ask the user for a column map.", default=False
-    # )
 
 
 class MergeTableModule(KiaraModule):
     """Create a table from other tables and/or arrays.
 
-    This module is a general purpose module to merge arrays and tables into a table data item. It does not have a no-config operation, meaning it needs to be configured before it can be used.
-
-    It does include one module config by default thought, which results in the operation `table.add_column', which takes a table and a single array, and adds the specified array as new column to the (also) provided input table.
-
-    Otherwise it is not possible to merge an arbitrary number of tables/arrays, the number of tables or arrays to be merged must always be specified in the module configuration.
-
-    Note: this module might still be re-worked a bit, because it's not straight-forward how to use tables here, since it's not possible to forsee the column names user-provided input tables will have. For now, the 'table.add_column' is the only use-case for this module, but I'd like it to be more generally useful in the future, for all kinds of table assembly tasks.
-
-    ## Module configuration options
-
-    ### `inputs_schema`
-
-    This is a dict describing which tables/arrays need to be provided by the user. The format is the same as
-    what is used in the `create_inputs_schema` method of a `KiaraModule` (apart from 'optional', which is not allowed here), e.g.:
-
-    ```
-        inputs_schema: {
-          "table1": {
-             "type": "table",
-             "doc": "The first table to merge.",
-          },
-          "table2": {
-            "type": "table",
-            "doc": "The second table to merge.",
-          },
-          "array": {
-            "type": "array",
-            "doc": "An array to add as column.",
-          }
-    }
-    ```
-
-    ### `column_map`
+    This module needs configuration to be set (for now). It's currently not possible to merge an arbitrary
+    number of tables/arrays, all tables to be merged must be specified in the module configuration.
 
     Column names of the resulting table can be controlled by the 'column_map' configuration, which takes the
-    desired column name as value, and a field-name in the following format as key:
+    desired column name as key, and a field-name in the following format as value:
     - '[inputs_schema key]' for inputs of type 'array'
     - '[inputs_schema_key].orig_column_name' for inputs of type 'table'
-
-    Additionally, the 'column_map' can also contain the special value 'input:[inputs_field_name]', which will prompt the resulting operation to have an additional input field with the name '[inputs_field_name]',  which will be used as the new column name of the referenced input field key.
-
-    Example:
-
-    ```
-        column_map: {
-            "array": "input:array_column_name"
-        }
-    ```
-
-    This would result in a module with 4 inputs ('table1', 'table2', "array", and 'array_column_name'), and the 'array_column_name' input would be used as the column name for the 'array' input, and the column names of the 2 tables would be used as-is, with an exception thrown if there is a duplicate column name.
-
-    For known column names in a table, a key/value pair might look like:
-
-    ```
-        column_map: {
-           "table1.first_name": "first_name"
-        }
-    ```
-
     """
 
-    @classmethod
-    def retrieve_included_operations(cls):
-
-        return {
-            "table.add_column": {
-                "doc": """Add a column to a table.
-
-This module takes a table and an array, and adds the array as a new column to the end table. The table and array must have the same number of rows for this to work.""",
-                "module_config": {
-                    "inputs_schema": {
-                        "table": {
-                            "type": "table",
-                            "doc": "The table to add the column to.",
-                        },
-                        "array": {
-                            "type": "array",
-                            "doc": "The column to add.",
-                        },
-                    },
-                    "column_map": {"array": "input:column_name"},
-                },
-            }
-        }
+    # @classmethod
+    # def retrieve_included_operations(cls):
+    #
+    #     return {
+    #         "table.add_column": {
+    #             "module_config": {
+    #                 "inputs_schema": {
+    #                     "table": {
+    #                         "type": "table",
+    #                         "doc": "The table to add the column to.",
+    #                     },
+    #                     "column": {
+    #                         "type": "array",
+    #                         "doc": "The column to add.",
+    #                     }
+    #                 }
+    #             }
+    #         }
+    #     }
 
     _module_type_name = "table.merge"
     _config_cls = MergeTableConfig
 
     def create_inputs_schema(
         self,
     ) -> ValueMapSchema:
 
         input_schema_models = self.get_config_value("inputs_schema")
 
         input_schema_dict = {}
         for k, v in input_schema_models.items():
-            if k == "column_map":
-                raise KiaraException(
-                    "Invalid input schema for 'table.merge' module: 'column_map' is a reserved keyword."
-                )
             input_schema_dict[k] = v.model_dump()
 
-        # if self.get_config_value("ask_column_map"):
-        #     input_schema_dict["column_map"] = {
-        #         "type": "dict",
-        #         "doc": "A dict describing how to map column names from inputs to the output table.",
-        #     }
-
-        for k, v in self.get_config_value("column_map").items():
-            if v.startswith("input:"):
-                input_name = v[6:]
-                if input_name in input_schema_dict.keys():
-                    raise KiaraException(
-                        "Can't use input field with name '{input_name}': already used for table or array input."
-                    )
-                input_schema_dict[input_name] = {
-                    "type": "string",
-                    "doc": f"The column-name for the input '{input_name}'.",
-                }
-
         return input_schema_dict
 
     def create_outputs_schema(
         self,
     ) -> ValueMapSchema:
 
         outputs = {
@@ -516,84 +433,94 @@
         }
         return outputs
 
     def process(self, inputs: ValueMap, outputs: ValueMap, job_log: JobLog) -> None:
 
         import pyarrow as pa
 
-        # first we need to assemble the final column map, in case there was user input
-        final_column_map = {}
-        config_column_map = self.get_config_value("column_map")
-        for k, v in config_column_map.items():
-            if v.startswith("input:"):
-                input_name = v[6:]
-                final_column_map[k] = inputs.get_value_data(input_name)
-            else:
-                final_column_map[k] = v
+        inputs_schema: Dict[str, Any] = self.get_config_value("inputs_schema")
+        column_map: Dict[str, str] = self.get_config_value("column_map")
 
-        inputs_schema: Dict[str, ValueSchemaInput] = self.get_config_value(
-            "inputs_schema"
-        )
-
-        sources: Dict[str, pa.Array] = {}
-        lengths_dict: Dict[int, List[str]] = {}
-        column_map_sources = {}
-        column_order = []
-
-        for field_name, schema in inputs_schema.items():
-
-            if schema.type == "array":
-                kiara_array_data: KiaraArray = inputs.get_value_data(field_name)
-                array_data = kiara_array_data.arrow_array
-                no_rows = array_data.length()
-                sources[field_name] = array_data
-                lengths_dict.setdefault(no_rows, []).append(field_name)
-                column_map_sources[field_name] = field_name
-                column_order.append(field_name)
-            elif schema.type == "table":
-                table_data: KiaraTable = inputs.get_value_data(field_name)
-                arrow_table = table_data.arrow_table
-                for column_name in arrow_table.column_names:
-                    arrow_array = arrow_table.column(column_name)
-                    name = f"{field_name}.{column_name}"
-                    no_rows = arrow_array.length()
-                    sources[name] = arrow_array
-                    lengths_dict.setdefault(no_rows, []).append(name)
-                    column_map_sources[name] = column_name
-                    column_order.append(name)
+        sources = {}
+        for field_name in inputs_schema.keys():
+            sources[field_name] = inputs.get_value_data(field_name)
+
+        len_dict = {}
+        arrays = {}
+
+        column_map_final = dict(column_map)
+
+        for source_key, table_or_array in sources.items():
+
+            if isinstance(table_or_array, KiaraTable):
+                rows = table_or_array.num_rows
+                for name in table_or_array.column_names:
+                    array_name = f"{source_key}.{name}"
+                    if column_map and array_name not in column_map.values():
+                        job_log.add_log(
+                            f"Ignoring column '{name}' of input table '{source_key}': not listed in column_map."
+                        )
+                        continue
+
+                    column = table_or_array.arrow_table.column(name)
+                    arrays[array_name] = column
+                    if not column_map:
+                        if name in column_map_final:
+                            raise Exception(
+                                f"Can't merge table, duplicate column name: {name}."
+                            )
+                        column_map_final[name] = array_name
+
+            elif isinstance(table_or_array, KiaraArray):
+
+                if column_map and source_key not in column_map.values():
+                    job_log.add_log(
+                        f"Ignoring array '{source_key}': not listed in column_map."
+                    )
+                    continue
 
-        if len(lengths_dict) > 1:
-            lengths_str = ", ".join((str(x) for x in lengths_dict.keys()))
-            raise KiaraProcessingException(
-                f"Can't merge table, sources have different lengths: {lengths_str}"
-            )
+                rows = len(table_or_array)
+                arrays[source_key] = table_or_array.arrow_array
 
-        column_names = []
-        columns = []
+                if not column_map:
+                    if source_key in column_map_final.keys():
+                        raise Exception(
+                            f"Can't merge table, duplicate column name: {source_key}."
+                        )
+                    column_map_final[source_key] = source_key
 
-        for k in final_column_map.keys():
-            if k not in column_map_sources.keys():
+            else:
                 raise KiaraProcessingException(
-                    f"Invalid column map key '{k}': not in sources."
+                    f"Can't merge table: invalid type '{type(table_or_array)}' for source '{source_key}'."
                 )
 
-        for column_ref, column_name in column_map_sources.items():
-            if column_ref in final_column_map.keys():
-                continue
+            len_dict[source_key] = rows
 
-            final_column_map[column_ref] = column_name
+        all_rows = None
+        for source_key, rows in len_dict.items():
+            if all_rows is None:
+                all_rows = rows
+            elif all_rows != rows:
+                all_rows = None
+                break
+
+        if all_rows is None:
+            len_str = ""
+            for name, rows in len_dict.items():
+                len_str = f" {name} ({rows})"
 
-        for column_ref in column_order:
-            column_name = final_column_map[column_ref]
-            if column_name in column_names:
-                raise KiaraProcessingException(
-                    f"Can't merge table: duplicate column name '{column_name}'."
-                )
+            raise KiaraProcessingException(
+                f"Can't merge table, sources have different lengths: {len_str}"
+            )
+
+        column_names = []
+        columns = []
+        for column_name, ref in column_map_final.items():
             column_names.append(column_name)
-            column = sources[column_ref]
+            column = arrays[ref]
             columns.append(column)
 
         table = pa.Table.from_arrays(arrays=columns, names=column_names)
 
         outputs.set_value("table", table)
```

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/table/filters.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/filters.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/modules/tables/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.json` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.json` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.json` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.json` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/utils/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin/tabular/utils/tables.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/tables.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin.tabular.egg-info/PKG-INFO` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.tabular
-Version: 0.5.4
+Version: 0.5.4rc1
 Summary: kiara data-types and modules for working with tables and databases.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.tabular
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.tabular
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.tabular
 Keywords: kiara
@@ -19,28 +19,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: kiara<0.6.0,>=0.5.10
-Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.1
+Requires-Dist: kiara<0.6.0,>=0.5.10rc10
+Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.1rc1
 Requires-Dist: duckdb<0.11.0,>=0.10.0
 Requires-Dist: pandas>=1.4.0
 Requires-Dist: polars>=0.18.0
 Requires-Dist: pyarrow>=12.0.0
 Requires-Dist: sqlalchemy>=2.0.0
 Requires-Dist: sqlalchemy-utc>=0.10.0
 Requires-Dist: sqlalchemy-utils>=0.38.0
 Requires-Dist: sqlite-utils==3.30
 Provides-Extra: dev-documentation
 Requires-Dist: kiara[dev_documentation]; extra == "dev-documentation"
 Provides-Extra: dev-testing
-Requires-Dist: kiara[dev_testing]; extra == "dev-testing"
+Requires-Dist: kiara[dev_testing]==0.5.10rc10; extra == "dev-testing"
 Requires-Dist: pandas-stubs; extra == "dev-testing"
 Provides-Extra: dev-utils
 Requires-Dist: kiara[dev_utils]; extra == "dev-utils"
 Provides-Extra: dev-all
 Requires-Dist: kiara[dev_all]; extra == "dev-all"
 Provides-Extra: streamlit
 Requires-Dist: kiara_plugin.streamlit; extra == "streamlit"
```

### Comparing `kiara_plugin_tabular-0.5.4/src/kiara_plugin.tabular.egg-info/SOURCES.txt` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/tests/conftest.py` & `kiara_plugin_tabular-0.5.4rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/tests/job_tests/create_tables_from_file_bundle/outputs.py` & `kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_tables_from_file_bundle/outputs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin_tabular-0.5.4/tests/test_job_descs.py` & `kiara_plugin_tabular-0.5.4rc1/tests/test_job_descs.py`

 * *Files identical despite different names*

