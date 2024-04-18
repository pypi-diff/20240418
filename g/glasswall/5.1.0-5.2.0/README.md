# Comparing `tmp/glasswall-5.1.0.tar.gz` & `tmp/glasswall-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glasswall-5.1.0.tar", last modified: Wed Apr 10 10:30:57 2024, max compression
+gzip compressed data, was "glasswall-5.2.0.tar", last modified: Thu Apr 18 09:54:45 2024, max compression
```

## Comparing `glasswall-5.1.0.tar` & `glasswall-5.2.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.702555 glasswall-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 10:30:51.000000 glasswall-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    87333 2024-04-10 10:30:57.702555 glasswall-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    86946 2024-04-10 10:30:51.000000 glasswall-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.686555 glasswall-5.1.0/glasswall/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.686555 glasswall-5.1.0/glasswall/config/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.686555 glasswall-5.1.0/glasswall/config/creationflags/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/config/creationflags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.686555 glasswall-5.1.0/glasswall/config/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/config/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.690555 glasswall-5.1.0/glasswall/config/security_tagging/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/config/security_tagging/tags_w3schools.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.690555 glasswall-5.1.0/glasswall/config/word_search/
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/config/word_search/homoglyphs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.690555 glasswall-5.1.0/glasswall/config/xml/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/config/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/config/xml/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.690555 glasswall-5.1.0/glasswall/content_management/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.690555 glasswall-5.1.0/glasswall/content_management/config_elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/archiveConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/config_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/gifConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/jpegConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/pdfConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/pptConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/svgConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/sysConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/textList.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/textSearchConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/tiffConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/webpConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/wordConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/config_elements/xlsConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.690555 glasswall-5.1.0/glasswall/content_management/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/errors/config_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/errors/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/errors/switches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.694555 glasswall-5.1.0/glasswall/content_management/policies/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/policies/archive_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/policies/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/policies/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/policies/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/policies/word_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.694555 glasswall-5.1.0/glasswall/content_management/switches/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/gif.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/jpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/ppt.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/sys.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/webp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/word.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/content_management/switches/xls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.694555 glasswall-5.1.0/glasswall/determine_file_type/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/determine_file_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/determine_file_type/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/determine_file_type/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/determine_file_type/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/determine_file_type/successes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.694555 glasswall-5.1.0/glasswall/libraries/
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.698555 glasswall-5.1.0/glasswall/libraries/archive_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/archive_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53675 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/archive_manager/archive_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/archive_manager/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/archive_manager/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/archive_manager/successes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.698555 glasswall-5.1.0/glasswall/libraries/editor/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/editor/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    83839 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/editor/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/editor/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/editor/successes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/library.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.698555 glasswall-5.1.0/glasswall/libraries/rebuild/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/rebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/rebuild/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/rebuild/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    49127 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/rebuild/rebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/rebuild/successes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.698555 glasswall-5.1.0/glasswall/libraries/security_tagging/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/security_tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/security_tagging/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/security_tagging/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/security_tagging/security_tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/security_tagging/successes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.698555 glasswall-5.1.0/glasswall/libraries/word_search/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/word_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/word_search/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/word_search/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/word_search/successes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/libraries/word_search/word_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.702555 glasswall-5.1.0/glasswall/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/multiprocessing/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/multiprocessing/memory_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/multiprocessing/task_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/multiprocessing/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    22061 2024-04-10 10:30:51.000000 glasswall-5.1.0/glasswall/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.702555 glasswall-5.1.0/glasswall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    87333 2024-04-10 10:30:57.000000 glasswall-5.1.0/glasswall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-10 10:30:57.000000 glasswall-5.1.0/glasswall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:30:57.000000 glasswall-5.1.0/glasswall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-10 10:30:57.000000 glasswall-5.1.0/glasswall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 10:30:57.000000 glasswall-5.1.0/glasswall.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-10 10:30:57.702555 glasswall-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-10 10:30:51.000000 glasswall-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.702555 glasswall-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.702555 glasswall-5.1.0/tests/content_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/content_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/content_management/test_config_element.py
--rw-r--r--   0 runner    (1001) docker     (127)    30224 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/content_management/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/content_management/test_switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:57.702555 glasswall-5.1.0/tests/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/multiprocessing/cicd_test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/multiprocessing/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/multiprocessing/test_task_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/multiprocessing/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-10 10:30:51.000000 glasswall-5.1.0/tests/test_readme_python_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.898833 glasswall-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 09:54:41.000000 glasswall-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    87333 2024-04-18 09:54:45.898833 glasswall-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    86946 2024-04-18 09:54:41.000000 glasswall-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.882833 glasswall-5.2.0/glasswall/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.882833 glasswall-5.2.0/glasswall/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.882833 glasswall-5.2.0/glasswall/config/creationflags/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/config/creationflags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.882833 glasswall-5.2.0/glasswall/config/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/config/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.886833 glasswall-5.2.0/glasswall/config/security_tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/config/security_tagging/tags_w3schools.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.886833 glasswall-5.2.0/glasswall/config/word_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/config/word_search/homoglyphs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.886833 glasswall-5.2.0/glasswall/config/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/config/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/config/xml/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.886833 glasswall-5.2.0/glasswall/content_management/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.886833 glasswall-5.2.0/glasswall/content_management/config_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/archiveConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/config_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/gifConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/jpegConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/pdfConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/pptConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/svgConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/sysConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/textList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/textSearchConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/tiffConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/webpConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/wordConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/config_elements/xlsConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.886833 glasswall-5.2.0/glasswall/content_management/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/errors/config_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/errors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/errors/switches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.890833 glasswall-5.2.0/glasswall/content_management/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/policies/archive_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/policies/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/policies/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/policies/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/policies/word_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.890833 glasswall-5.2.0/glasswall/content_management/switches/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/gif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/webp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/content_management/switches/xls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.890833 glasswall-5.2.0/glasswall/determine_file_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/determine_file_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/determine_file_type/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/determine_file_type/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/determine_file_type/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/determine_file_type/successes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.894833 glasswall-5.2.0/glasswall/libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.894833 glasswall-5.2.0/glasswall/libraries/archive_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/archive_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53675 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/archive_manager/archive_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/archive_manager/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/archive_manager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/archive_manager/successes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.894833 glasswall-5.2.0/glasswall/libraries/editor/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/editor/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83839 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/editor/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/editor/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/editor/successes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.894833 glasswall-5.2.0/glasswall/libraries/rebuild/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/rebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/rebuild/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/rebuild/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49127 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/rebuild/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/rebuild/successes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.894833 glasswall-5.2.0/glasswall/libraries/security_tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/security_tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/security_tagging/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/security_tagging/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/security_tagging/security_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/security_tagging/successes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.898833 glasswall-5.2.0/glasswall/libraries/word_search/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/word_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/word_search/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/word_search/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/word_search/successes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/libraries/word_search/word_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.898833 glasswall-5.2.0/glasswall/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/multiprocessing/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/multiprocessing/memory_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/multiprocessing/task_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/multiprocessing/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22061 2024-04-18 09:54:41.000000 glasswall-5.2.0/glasswall/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.898833 glasswall-5.2.0/glasswall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    87333 2024-04-18 09:54:45.000000 glasswall-5.2.0/glasswall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-18 09:54:45.000000 glasswall-5.2.0/glasswall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:54:45.000000 glasswall-5.2.0/glasswall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 09:54:45.000000 glasswall-5.2.0/glasswall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 09:54:45.000000 glasswall-5.2.0/glasswall.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 09:54:45.902833 glasswall-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-18 09:54:41.000000 glasswall-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.898833 glasswall-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.898833 glasswall-5.2.0/tests/content_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/content_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/content_management/test_config_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30224 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/content_management/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/content_management/test_switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:45.898833 glasswall-5.2.0/tests/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/multiprocessing/cicd_test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/multiprocessing/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/multiprocessing/test_task_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/multiprocessing/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-18 09:54:41.000000 glasswall-5.2.0/tests/test_readme_python_code.py
```

### Comparing `glasswall-5.1.0/PKG-INFO` & `glasswall-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glasswall
-Version: 5.1.0
+Version: 5.2.0
 Summary: Glasswall Python Wrapper
 Home-page: https://github.com/gw-engineering/glasswall-python-wrapper
 Author: AngusWR
 Author-email: aroberts@glasswall.com
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `glasswall-5.1.0/README.md` & `glasswall-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/__init__.py` & `glasswall-5.2.0/glasswall/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 import os
 import pathlib
 import platform
 import tempfile
 
-__version__ = "5.1.0"
+__version__ = "5.2.0"
 
 _OPERATING_SYSTEM = platform.system()
 _PYTHON_VERSION = platform.python_version()
 _ROOT = os.path.dirname(__file__)
 _TEMPDIR = str(pathlib.Path(os.environ.get("AGENT_TEMPDIRECTORY", tempfile.gettempdir())).joinpath("glasswall").resolve())
 
 from glasswall import config, content_management, determine_file_type, utils
```

### Comparing `glasswall-5.1.0/glasswall/config/creationflags/__init__.py` & `glasswall-5.2.0/glasswall/config/creationflags/__init__.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/config/logging/__init__.py` & `glasswall-5.2.0/glasswall/config/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/config/word_search/homoglyphs.json` & `glasswall-5.2.0/glasswall/config/word_search/homoglyphs.json`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/__init__.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/archiveConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/archiveConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/config_element.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/config_element.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/gifConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/gifConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/jpegConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/jpegConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/pdfConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/pdfConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/pptConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/pptConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/svgConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/svgConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/sysConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/sysConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/textSearchConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/textSearchConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/tiffConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/tiffConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/webpConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/webpConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/wordConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/wordConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/config_elements/xlsConfig.py` & `glasswall-5.2.0/glasswall/content_management/config_elements/xlsConfig.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/policies/archive_manager.py` & `glasswall-5.2.0/glasswall/content_management/policies/archive_manager.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/policies/editor.py` & `glasswall-5.2.0/glasswall/content_management/policies/editor.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/policies/policy.py` & `glasswall-5.2.0/glasswall/content_management/policies/policy.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/policies/rebuild.py` & `glasswall-5.2.0/glasswall/content_management/policies/rebuild.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/policies/word_search.py` & `glasswall-5.2.0/glasswall/content_management/policies/word_search.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/switches/archive.py` & `glasswall-5.2.0/glasswall/content_management/switches/archive.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/switches/pdf.py` & `glasswall-5.2.0/glasswall/content_management/switches/pdf.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/switches/ppt.py` & `glasswall-5.2.0/glasswall/content_management/switches/ppt.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/switches/svg.py` & `glasswall-5.2.0/glasswall/content_management/switches/svg.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/switches/switch.py` & `glasswall-5.2.0/glasswall/content_management/switches/switch.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/switches/sys.py` & `glasswall-5.2.0/glasswall/content_management/switches/sys.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/switches/word.py` & `glasswall-5.2.0/glasswall/content_management/switches/word.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/content_management/switches/xls.py` & `glasswall-5.2.0/glasswall/content_management/switches/xls.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/determine_file_type/errors.py` & `glasswall-5.2.0/glasswall/determine_file_type/errors.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/determine_file_type/helpers.py` & `glasswall-5.2.0/glasswall/determine_file_type/helpers.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/determine_file_type/successes.py` & `glasswall-5.2.0/glasswall/determine_file_type/successes.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/libraries/__init__.py` & `glasswall-5.2.0/glasswall/libraries/__init__.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/libraries/archive_manager/archive_manager.py` & `glasswall-5.2.0/glasswall/libraries/archive_manager/archive_manager.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/libraries/editor/editor.py` & `glasswall-5.2.0/glasswall/libraries/editor/editor.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/libraries/editor/errors.py` & `glasswall-5.2.0/glasswall/libraries/editor/errors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+# Statuses from sdk.editor\src\core.support\sdk.interface\gw2_returnstatus.h
 
 
 from glasswall.libraries.editor.classes import EditorError
 
 
 class UnknownErrorCode(EditorError):
     """ Unknown error code. """
     pass
 
 
-# Statuses from sdk.editor\src\core.support\sdk.interface\gw2_returnstatus.h
 class GeneralFail(EditorError):
     """ Editor error code -1. """
     pass
 
 
 class UnexpectedEndOfFile(EditorError):
     """ Editor error code -2. """
```

### Comparing `glasswall-5.1.0/glasswall/libraries/library.py` & `glasswall-5.2.0/glasswall/libraries/library.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/libraries/rebuild/errors.py` & `glasswall-5.2.0/glasswall/libraries/rebuild/errors.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+# Statuses from sdk.rebuild\src\code\dll.gwfile\dll.gwfilestatus.h
 
 
 from glasswall.libraries.rebuild.classes import RebuildError
 
 
 class UnknownErrorCode(RebuildError):
     """ Unknown error code. """
     pass
 
 
-# Statuses from sdk.rebuild\src\code\dll.gwfile\dll.gwfilestatus.h
 class Error(RebuildError):
     """ Rebuild error code 0. This value indicates that the document was non-conformant in some way, but any requested output files were written. """
     pass
 
 
 class SuccessDocumentWriteFailure(RebuildError):
     """ Rebuild error code -1. This value indicates that the document was managed successfully, but a failure occured when writing the managed version of the document to file. """
```

### Comparing `glasswall-5.1.0/glasswall/libraries/rebuild/rebuild.py` & `glasswall-5.2.0/glasswall/libraries/rebuild/rebuild.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/libraries/security_tagging/security_tagging.py` & `glasswall-5.2.0/glasswall/libraries/security_tagging/security_tagging.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/libraries/word_search/word_search.py` & `glasswall-5.2.0/glasswall/libraries/word_search/word_search.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/multiprocessing/manager.py` & `glasswall-5.2.0/glasswall/multiprocessing/manager.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/multiprocessing/memory_usage.py` & `glasswall-5.2.0/glasswall/multiprocessing/memory_usage.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/multiprocessing/task_watcher.py` & `glasswall-5.2.0/glasswall/multiprocessing/task_watcher.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/multiprocessing/tasks.py` & `glasswall-5.2.0/glasswall/multiprocessing/tasks.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall/utils.py` & `glasswall-5.2.0/glasswall/utils.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/glasswall.egg-info/PKG-INFO` & `glasswall-5.2.0/glasswall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glasswall
-Version: 5.1.0
+Version: 5.2.0
 Summary: Glasswall Python Wrapper
 Home-page: https://github.com/gw-engineering/glasswall-python-wrapper
 Author: AngusWR
 Author-email: aroberts@glasswall.com
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `glasswall-5.1.0/glasswall.egg-info/SOURCES.txt` & `glasswall-5.2.0/glasswall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/setup.py` & `glasswall-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/tests/content_management/test_config_element.py` & `glasswall-5.2.0/tests/content_management/test_config_element.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/tests/content_management/test_policy.py` & `glasswall-5.2.0/tests/content_management/test_policy.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/tests/content_management/test_switch.py` & `glasswall-5.2.0/tests/content_management/test_switch.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/tests/multiprocessing/cicd_test_integration.py` & `glasswall-5.2.0/tests/multiprocessing/cicd_test_integration.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/tests/multiprocessing/test_manager.py` & `glasswall-5.2.0/tests/multiprocessing/test_manager.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/tests/multiprocessing/test_task_watcher.py` & `glasswall-5.2.0/tests/multiprocessing/test_task_watcher.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/tests/multiprocessing/test_tasks.py` & `glasswall-5.2.0/tests/multiprocessing/test_tasks.py`

 * *Files identical despite different names*

### Comparing `glasswall-5.1.0/tests/test_readme_python_code.py` & `glasswall-5.2.0/tests/test_readme_python_code.py`

 * *Files identical despite different names*

