# Comparing `tmp/pyodide_mkdocs_theme-0.3.0.tar.gz` & `tmp/pyodide_mkdocs_theme-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.3.0.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.3.1.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.3.0.tar` & `pyodide_mkdocs_theme-0.3.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.3.0/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.3.0/README.md
--rw-r--r--   0        0        0     1347 2024-04-14 21:38:36.831215 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2160 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-14 21:38:36.867216 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4969 2024-04-09 19:35:36.226493 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    21303 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     4093 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11548 2024-04-14 21:34:08.611259 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    12363 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    11594 2024-04-14 21:34:08.611259 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0    12992 2024-04-14 21:34:08.619259 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
--rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     3236 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9974 2024-04-14 21:34:08.619259 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1064 2024-04-14 21:38:36.819214 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6881 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/scripts/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     3974 2024-04-14 21:38:36.831215 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py
--rw-r--r--   0        0        0     5490 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     4510 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     6426 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9780 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6600 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4218 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12716 2024-04-14 21:34:08.623259 pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1775 2024-04-14 21:38:33.567118 pyodide_mkdocs_theme-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.3.1/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.3.1/README.md
+-rw-r--r--   0        0        0     1347 2024-04-18 21:28:53.878591 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2160 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-18 21:28:53.914592 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4991 2024-04-18 21:28:32.174075 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    21241 2024-04-18 21:28:32.174075 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     4093 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11548 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13167 2024-04-18 21:28:32.174075 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    11594 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0    13039 2024-04-18 09:36:07.501012 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
+-rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     3236 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9974 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1064 2024-04-18 21:28:53.870591 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6881 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     3983 2024-04-18 21:28:53.878591 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py
+-rw-r--r--   0        0        0     5490 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
+-rw-r--r--   0        0        0     6426 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9780 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6600 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
+-rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
+-rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4218 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
+-rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1775 2024-04-18 21:28:50.330507 pyodide_mkdocs_theme-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.3.1/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.3.0/LICENSE` & `pyodide_mkdocs_theme-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/README.md` & `pyodide_mkdocs_theme-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                       - Every string section that matches a builtin callable forbid that function
                         by replacing it with another function which will raise an error if called
                       - Every string section prefixed with a fot forbids a method call. Here a
                         simple string containment check is done opn the user's code, to check it
                         does not contain the desired method name with the dot before it.
                       - Any other string section is considered as a module name and doing an
                         import (in any way/syntax) involving that name will raise an error.
-    @SIZE:        Max number of lines of the IDE (default=30).
+    @MAX_SIZE:        Max number of lines of the IDE (default=30).
     @ID:          Optional. To use to differentiate two IDEs using the same python root file.
     @WHITE:       String of spaces or coma separated python modules/packages that have to be
                   preloaded before the code restrictions (@SANS) are applied.
     @LOGS:        If True, failing assertions without feedback during the private tests will
                   be augmented automatically with the code of the assertion itself. If None,
                   use the global `show_assertion_code_on_failed_test` plugin value, defined in
                   `mkdocs.yml`, to determine what to do (default=None).
@@ -63,23 +63,23 @@
     """
 
     @wraps(_IDE_maker)
     def wrapped(
         script_name: str = "",
         MAX: Optional[Union[int, Literal["+"]]] = None,
         SANS: str = "",
-        SIZE: int = 30,
-        ID: int = None,
+        MAX_SIZE: int = 30,
+        ID: Optional[int] = None,
         WHITE: str = "",
         LOGS: Optional[bool] = None,
         REC_LIMIT: int = -1,
         TERM_H: int = 10,
     ) -> str:
         return Ide(
-            env, script_name, mode, MAX, SANS, SIZE, WHITE, ID, LOGS, REC_LIMIT, TERM_H
+            env, script_name, mode, MAX, SANS, MAX_SIZE, WHITE, ID, LOGS, REC_LIMIT, TERM_H
         ).make_ide()
 
     wrapped.__name__ = wrapped.__qualname__ = 'IDE' + mode.strip('_')
     return wrapped
```

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
         Note that the restrictions are rather strict, and may have unexpected side effects, such
         as, forbidding `exec` will also forbid to import numpy, because the package relies on exec
         for some operations at import time.
         To circumvent such a kind of problems, use the white_list argument.
     """
 
-    size: int
+    max_size: int
     """ Max height of the editor (in number of lines) """
 
     white_list: str
     """ String of spaces or coma separated python modules/packages names the have to be
         preloaded before the code restrictions are enforced on the user's side.
     """
 
@@ -295,15 +295,15 @@
         if the value coming from the macro is the default one or not.
         """
         max_ide = str(self.max_attempts)        # from macro call
 
         # If something about MAX in the file, it has precedence (if exists -> legacy...)
         max_from_file = self.files_data.file_max_attempts
         if max_from_file != "":
-            max_ide = "+" if max_from_file == "+" else max_from_file
+            max_ide = max_from_file
 
         is_inf = max_ide in ("+", "1000")     # 1000: legacy...
 
         # If ever there are neither correction nor remark, or if no tests, use also inf:
         is_inf = is_inf or not (self.has_corr or self.has_rem) or not self.has_test
 
         self.max_attempts_symbol = self.INFINITY_SYMBOL if is_inf else str(max_ide)
@@ -348,26 +348,26 @@
     def generate_empty_ide(self) -> str:
         """
         Generate the global layout that will receive later the ace elements.
         """
         is_v = self.mode == '_v'
         toggle_txt = '###'
         tip: Tip = self.my_env.lang.comments
-        msg = str(tip).format(tests=self.my_env.lang.tests)
+        msg = str(tip)
 
         shortcut_comment_asserts = Html.span(
             toggle_txt + Html.tooltip(msg, tip.em, shift=95),
             id = Prefix.comment_ + self.editor_name,
             kls = f'{HtmlClass.comment} {HtmlClass.tooltip}',
         )
         editor_div = Html.div(
             id = self.editor_name,
             is_v = str(is_v).lower(),
             mode = self.mode,
-            max_size = self.size,
+            max_size = self.max_size,
             script_name = self.script_name,
         )
         editor_wrapper = Html.div(
             editor_div + shortcut_comment_asserts,
             kls = Prefix.comment_ + HtmlClass.py_mk_wrapper
         )
```

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,39 +16,43 @@
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 import json
 import re
-from typing import ClassVar, Dict, Tuple, Union
+from typing import Any, ClassVar, Dict, Tuple, Union, TYPE_CHECKING
 from dataclasses import dataclass
 from argparse import Namespace
 
 from mkdocs.exceptions import BuildError
 
 
-from pyodide_mkdocs_theme.pyodide_macros.plugin.maestro_tools import dump_and_dumper
+from .plugin.maestro_tools import dump_and_dumper
+
+if TYPE_CHECKING:
+    from .plugin.pyodide_macros_plugin import PyodideMacrosPlugin
 
 
 
 Tr = Union['Msg', 'MsgPlural', 'Tip', 'TestsToken']
 LangProp = str
 Pattern = re.compile('')       # done this way for linting and mkdocstrings... :/
 
 
 
 
 
 @dataclass
 class JsDumper:
     """ Base class to automatically transfer "lang" messages from python to JS """
-    # pylint: disable=no-member
+    # pylint: disable=no-member,missing-function-docstring
 
     PROPS: ClassVar[Tuple[str]] = tuple('msg plural em as_pattern kbd'.split())
+    ENV: ClassVar[Dict[str,Any]] = None
 
     def __str__(self):
         return self.msg
 
     def dump_as_dct(self):
         dct = {
             prop: v for prop in self.PROPS if (v := self.get_prop(prop)) is not None
@@ -56,14 +60,22 @@
         return dct
 
 
     def get_prop(self,prop):
         return str(self) if prop=='msg' else getattr(self, prop, None)
 
 
+    @staticmethod
+    def register_env(env:'PyodideMacrosPlugin'):
+        JsDumper.ENV = {
+            name: getattr(env,name) for name in "site_name".split()
+        }
+        JsDumper.ENV['tests'] = str(env.lang.tests) # pylint: disable=unsupported-assignment-operation
+
+
 
 @dataclass
 class Msg(JsDumper):
     """
     A simple message to display in the application.
 
     Parameters:
@@ -159,29 +171,29 @@
 class Tip(JsDumper):
     """
     Data for tooltips.
 
     Parameters:
         em:     Width of the tooltip element, in em units.
         msg:    Tooltip message.
-        kbd:    Keyboard shortcut (as "Ctrl+I", for example). Informational only (no impact on the behaviors)
+        kbd:    Keyboard shortcut (as "Ctrl+I", for example). Informational only (no
+                impact on the behaviors)
 
-    If a `kbd` combination is present, it will be automatically added in a new line after
-    the tooltip `msg`.
+    If a `kbd` combination is present, it will be automatically added in a new line
+    after the tooltip `msg`.
     """
     em: int         # Width, in em. If 0, use automatic width
     msg: str        # tooltip message
     kbd: str = ""   # ex: "Ctrl+I" / WARNING: DO NOT MODIFY DEFAULTS!
 
     def __str__(self):
-        if not self.kbd:
-            return self.msg
-
-        kbd = re.sub(r"(\w+)", r"<kbd>\1</kbd>", self.kbd)
-        msg = f"{ self.msg }<br>({ kbd })"
+        msg = self.msg.format(**self.ENV)       # pylint: disable=not-a-mapping
+        if self.kbd:
+            kbd = re.sub(r"(\w+)", r"<kbd>\1</kbd>", self.kbd)
+            msg = f"{ msg }<br>({ kbd })"
         return msg
 
 
 
 
 
 
@@ -222,16 +234,16 @@
     """
     Message affiché dans la console avant le chargement de micropip, en vue d'installer des modules manquants.
     """###
     install_done:  Tr = Msg("Installations terminées!")    ###
     """
     Message affiché lorsque les installation de paquets par micropip sont finies.
     """###
-    feedback:   Tr = Tip(15,  "Tronquer ou non le feedback dans les terminaux (sortie standard"
-                              " & stacktrace / relancer le code pour appliquer)")    ###
+    feedback:      Tr = Tip(15, "Tronquer ou non le feedback dans les terminaux (sortie standard"
+                                " & stacktrace / relancer le code pour appliquer)")    ###
     """
     Info-bulle du bouton contrôlant le "niveau de feedback" affiché dans le terminal
     """###
 
     # Terminals: validation success/failure messages
     success_head:  Tr = Msg("Bravo !")    ###
     """
@@ -241,15 +253,15 @@
     """
     Fin du message annonçant un succès.
     """###
     fail_head:     Tr = Msg("Dommage !")    ###
     """
     Entête du message d'échec (gras, italique, en orange)
     """###
-    success_tail: Tr = Msg("Pensez à lire")    ###
+    success_tail:  Tr = Msg("Pensez à lire")    ###
     """
     Fin du message de succès.
     """###
     reveal_corr:   Tr = Msg("le corrigé")    ###
     """
     Bout de phrase annonçant l'existence d'une correction.
     """###
@@ -258,36 +270,40 @@
     Conjonction de coordination joignant reveal_corr et reveal_rem, quand correction et
     remarques sont présentes.
     """###
     reveal_rem:    Tr = Msg("les commentaires")    ###
     """
     Bout de phrase annonçant l'existence de remarques.
     """###
-    fail_tail:     Tr = MsgPlural("est maintenant disponible", "sont maintenant disponibles")    ###
+    fail_tail:     Tr = MsgPlural("est maintenant disponible", "sont maintenant disponibles") ###
     """
     Fin du message annonçant un échec.
     """###
 
 
     # Corr  rems admonition:
     title_corr: Tr = Msg('Solution')    ###
     """
-    Utilisé pour construire le titre de l'admonition contenant la correction et les remarques, sous les IDEs.
+    Utilisé pour construire le titre de l'admonition contenant la correction et les remarques,
+    sous les IDEs.
     """###
     title_rem:  Tr = Msg('Remarques')   ###
     """
-    Utilisé pour construire le titre de l'admonition contenant la correction et les remarques, sous les IDEs.
+    Utilisé pour construire le titre de l'admonition contenant la correction et les remarques,
+    sous les IDEs.
     """###
     corr:       Tr = Msg('🐍 Proposition de correction')    ###
     """
-    Titre du bloc de code contenant la correction d'un IDE, dans l'admonition "correction & remarques".
+    Titre du bloc de code contenant la correction d'un IDE, dans l'admonition "correction &
+    remarques".
     """###
     rem:        Tr = Msg('Remarques')    ###
     """
-    Titre (équivalent &lt;h3&gt;) annonçant le début des remarques, dans l'admonition "correction & remarques"
+    Titre (équivalent &lt;h3&gt;) annonçant le début des remarques, dans l'admonition "correction &
+    remarques"
     """###
 
 
     # IDEs buttons & counter:
     play:       Tr = Tip(9,  "Exécuter le code", "Ctrl+S")    ###
     """
     Info-bulle du bouton pour lancer les tests publics.
@@ -306,19 +322,21 @@
     """###
     restart:    Tr = Tip(0,  "Réinitialiser l'éditeur")    ###
     """
     Info-bulle du bouton réinitialisant le contenu d'un éditeur.
     """###
     save:       Tr = Tip(0,  "Sauvegarder dans le navigateur")    ###
     """
-    Info-bulle du bouton pour enregistrer le contenu d'un éditeur dans le LocaleStorage du navigateur.
+    Info-bulle du bouton pour enregistrer le contenu d'un éditeur dans le LocaleStorage du
+    navigateur.
     """###
     attempts_left: Tr = Msg("Évaluations restantes")    ###
     """
-    Info-bulle du bouton pour enregistrer le contenu d'un éditeur dans le LocaleStorage du navigateur.
+    Info-bulle du bouton pour enregistrer le contenu d'un éditeur dans le LocaleStorage du
+    navigateur.
     """###
 
     # QCMS
     qcm_title:     Tr = MsgPlural("Question")    ###
     """
     Titre utilisé par défaut pour les admonitions contenant les qcms (si pas d'argument renseigné
     dans l'appel de la macro `multi_qcm`).
@@ -333,18 +351,20 @@
     """###
     qcm_redo_tip:  Tr = Tip(9,  "Recommencer")    ###
     """
     Info-bulle du bouton de réinitialisation des qcms.
     """###
 
     # Others
-    tip_trash:     Tr = Tip(15, "Supprimer tous les codes enregistrés sur ce navigateur")    ###
+    tip_trash: Tr = Tip(15, "Supprimer du navigateur les codes enregistrés pour {site_name}") ###
     """
     Info-bulle du bouton de pour supprimer les données stockées dans le navigateur
     (la poubelle en haut à côté de la barre de recherche).
+    Le nom du site (`site_name` dans `mkdocs.yml`) est automatiquement intégré dans la phrase
+    avec "{site_name}".
     """###
 
 
     # LANG_TOKEN
     #-------------------------------------------------------------------------
 
 
@@ -364,14 +384,18 @@
                 raise BuildError(f"Invalid Lang property: {k!r}")
             if not isinstance(v, current.__class__):
                 kls = current.__class__.__name__
                 raise BuildError(f"Invalid Translation type: {v!r} should be an instance of {kls}")
             setattr(self,k,v)
 
 
+    def register_env(self, env:'PyodideMacrosPlugin'):
+        """ Register the config data in the JsDumper class (for messages rendering) """
+        JsDumper.register_env(env)
+
 
     @classmethod
     def dump_as_str(cls, obj=None):
         """
         Create a complete json object with all teh string representations of all the messages.
         - Takes potential overloads in consideration
         - WARNING: js dumps are simple str conversions, so far, so some messages might be
```

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,14 +124,16 @@
 
 
 
     def on_config(self, config:MkDocsConfig):
         # pylint: disable=unused-argument, no-member, missing-function-docstring
         self._pages_indents = PageIndents()
         self.lang = Lang()
+        self.lang.register_env(self)
+
         super().on_config(config)     # MacrosPlugin is actually "next in line" and has the method
 
 
     def override_messages(self, dct_lang: Dict[str, Union[Msg,Tip]]):
         """ Replace some default messages or configurations with the given content """
         self.lang.overload(dct_lang)
 
@@ -207,38 +209,37 @@
     """ Cache storing the indentations for each jinja/macro template in all Pages.
         a page is entirely studied the first time it's seen and the result of the indentation
         levels are stored.
         The data stays correct throughout the md->html conversion because the indentation
         levels "horizontal") are not affected by the content growing ("vertical").
     """
 
-    def _explore_page_markdown(self, env:'BaseMaestro'):
+    def _explore_page_markdown(self, env:'BaseMaestro', txt:str):
         """
         Gather the indentations for all the macros insertions (aka `{{...}}`) in the page markdown.
         Only insertions following spaces or right at the beginning of a line are extracted.
 
         During parsing, it is also checked that there is no  `{{` starting again inside a macro
         call (this is subject to false positives, if the call contains `"{{"`!)
         """
         dct = {}
-        txt = env.page.markdown
         end = len(txt)
 
         i,i_cmd = eat(txt, '{{', skip_error=True)
         while i < end:
 
             i_next_open = eat(txt, '{{', start=i+2, skip_error=True)
             i_close, _  = eat(txt, '}}', start=i)
 
             # Check no nested macro calls:
             if i_next_open[0] < i_close:
                 self._handle_error(
                     env,
                     f"""
-Couldn't figure out the structure of macros calls in the template of the page {env.page!s} :
+Couldn't figure out the structure of macros calls in the template of the page {env.page.file.src_uri!s} :
     {"{{"!r} at index {i}
     {"{{"!r} at index {i_next_open[0]}  << should be after the next one
     {"}}"!r} at index {i_close}
 If you are trying to use {"{{"!r} or {"}}"!r}:
   - in data structures: just add some extra spaces in between.
   - inside a string: please raise an issue on { env.pmt_url }.
                     """.strip()
@@ -284,15 +285,15 @@
     def get_indent(self, env:'BaseMaestro', macro_predicate:re.Pattern) -> str :
         """
         Extract the indentation needed for the given macro template call.
         @throws:    BuildError if the same macro call is found several times in the page.
         """
         page:Page = env.page
         if page.url not in self:
-            self._explore_page_markdown(env)
+            self._explore_page_markdown(env, env.page.markdown)
 
         all_indents_in_page = self[page.url]
         indents_gen = ( indent for cmd,indent in all_indents_in_page.items()
                                if macro_predicate.match(cmd) )
         target = next( indents_gen, None)
         second = next( indents_gen, None)
```

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/scripts/__init__.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/scripts/custom_lang_src.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 
 
     # Terminals
         "run_script":    Msg("Script lancé..."),
         "success_msg":   Msg("Terminé sans erreur !"),
         "install_start": Msg("Installation de paquets python. Ceci peut prendre un certain temps..."),
         "install_done":  Msg("Installations terminées!"),
-        "feedback":   Tip(15,  "Tronquer ou non le feedback dans les terminaux (sortie standard"
-                              " & stacktrace / relancer le code pour appliquer)"),
+        "feedback":      Tip(15, "Tronquer ou non le feedback dans les terminaux (sortie standard"
+                                " & stacktrace / relancer le code pour appliquer)"),
 
     # Terminals: validation success/failure messages
         "success_head":  Msg("Bravo !"),
         "success_head_extra":  Msg("Vous avez réussi tous les tests !"),
         "fail_head":     Msg("Dommage !"),
-        "success_tail": Msg("Pensez à lire"),
+        "success_tail":  Msg("Pensez à lire"),
         "reveal_corr":   Msg("le corrigé"),
         "reveal_join":   Msg("et"),
         "reveal_rem":    Msg("les commentaires"),
         "fail_tail":     MsgPlural("est maintenant disponible", "sont maintenant disponibles"),
 
 
     # Corr  rems admonition:
@@ -87,11 +87,11 @@
     # QCMS
         "qcm_title":     MsgPlural("Question"),
         "qcm_mask_tip":  Tip(15, "Les réponses resteront cachées..."),
         "qcm_check_tip": Tip(11, "Vérifier les réponses"),
         "qcm_redo_tip":  Tip(9,  "Recommencer"),
 
     # Others
-        "tip_trash":     Tip(15, "Supprimer tous les codes enregistrés sur ce navigateur")
+        "tip_trash": Tip(15, "Supprimer du navigateur les codes enregistrés pour {site_name}")
     }
 
     env.lang.overload(custom)
```

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.0/pyproject.toml` & `pyodide_mkdocs_theme-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.3.0"
+version = "0.3.1"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-0.3.0/PKG-INFO` & `pyodide_mkdocs_theme-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.3.0
+Version: 0.3.1
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

