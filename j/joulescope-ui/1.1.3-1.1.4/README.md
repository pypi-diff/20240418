# Comparing `tmp/joulescope_ui-1.1.3.tar.gz` & `tmp/joulescope_ui-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope_ui-1.1.3.tar", last modified: Fri Apr  5 18:34:44 2024, max compression
+gzip compressed data, was "joulescope_ui-1.1.4.tar", last modified: Thu Apr 18 18:58:20 2024, max compression
```

## Comparing `joulescope_ui-1.1.3.tar` & `joulescope_ui-1.1.4.tar`

### file list

```diff
@@ -1,472 +1,476 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.860901 joulescope_ui-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    52810 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-05 18:34:44.860901 joulescope_ui-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-05 18:34:43.000000 joulescope_ui-1.1.3/joulescope.iss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.812900 joulescope_ui-1.1.3/joulescope_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    52810 2024-04-05 18:34:33.000000 joulescope_ui-1.1.3/joulescope_ui/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-05 18:34:33.000000 joulescope_ui-1.1.3/joulescope_ui/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/dev_signal_buffer_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.812900 joulescope_ui-1.1.3/joulescope_ui/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/device_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.812900 joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/js110.py
--rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/js220.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/js220_fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/js220_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.812900 joulescope_ui-1.1.3/joulescope_ui/devices/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/devices/test/test_device_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/disk_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/entry_points/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/entry_points/zip_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/error_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/error_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/expanding_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/file_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/filename_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.788900 joulescope_ui-1.1.3/joulescope_ui/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/fonts/DSEG14-Modern/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/fonts/Hack/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/fonts/Hack/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/fonts/Lato/
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/fonts/Lato/OFL.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/fonts/SourceCodePro/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/fonts/SourceCodePro/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/fonts/SourceSerifPro/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/fonts/SourceSerifPro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-04-05 18:34:44.000000 joulescope_ui-1.1.3/joulescope_ui/fonts.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/getting_started.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/help_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/intel_graphics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/jls_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/jls_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/jls_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/jls_v2_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/json_plus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/locale/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/locale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.788900 joulescope_ui-1.1.3/joulescope_ui/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    80601 2024-04-05 18:34:35.000000 joulescope_ui-1.1.3/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   110830 2024-04-05 18:34:34.000000 joulescope_ui-1.1.3/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.788900 joulescope_ui-1.1.3/joulescope_ui/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70573 2024-04-05 18:34:35.000000 joulescope_ui-1.1.3/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   101203 2024-04-05 18:34:34.000000 joulescope_ui-1.1.3/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.788900 joulescope_ui-1.1.3/joulescope_ui/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    97846 2024-04-05 18:34:35.000000 joulescope_ui-1.1.3/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   128500 2024-04-05 18:34:34.000000 joulescope_ui-1.1.3/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.788900 joulescope_ui-1.1.3/joulescope_ui/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70611 2024-04-05 18:34:35.000000 joulescope_ui-1.1.3/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   101189 2024-04-05 18:34:34.000000 joulescope_ui-1.1.3/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.788900 joulescope_ui-1.1.3/joulescope_ui/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.816900 joulescope_ui-1.1.3/joulescope_ui/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    72050 2024-04-05 18:34:35.000000 joulescope_ui-1.1.3/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   102687 2024-04-05 18:34:34.000000 joulescope_ui-1.1.3/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.788900 joulescope_ui-1.1.3/joulescope_ui/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.820900 joulescope_ui-1.1.3/joulescope_ui/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    74578 2024-04-05 18:34:35.000000 joulescope_ui-1.1.3/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104308 2024-04-05 18:34:34.000000 joulescope_ui-1.1.3/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)    67509 2024-04-05 18:34:34.000000 joulescope_ui-1.1.3/joulescope_ui/locale/joulescope_ui.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.788900 joulescope_ui-1.1.3/joulescope_ui/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.820900 joulescope_ui-1.1.3/joulescope_ui/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    69335 2024-04-05 18:34:35.000000 joulescope_ui-1.1.3/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)    99154 2024-04-05 18:34:34.000000 joulescope_ui-1.1.3/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.788900 joulescope_ui-1.1.3/joulescope_ui/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.820900 joulescope_ui-1.1.3/joulescope_ui/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    60522 2024-04-05 18:34:35.000000 joulescope_ui-1.1.3/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)    90132 2024-04-05 18:34:34.000000 joulescope_ui-1.1.3/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    40941 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/mem_leak_debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.820900 joulescope_ui-1.1.3/joulescope_ui/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.820900 joulescope_ui-1.1.3/joulescope_ui/plugins/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.820900 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.820900 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/p1/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/p1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/p1/index.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.820900 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/p2/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/p2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/p2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/p2/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/plugins/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/process_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    66439 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/pubsub_callable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/pubsub_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/range_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.824900 joulescope_ui-1.1.3/joulescope_ui/range_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/range_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/range_tools/cdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/range_tools/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/range_tools/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/range_tools/max_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/range_tools/plugin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/range_tools/usb_inrush.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.824900 joulescope_ui-1.1.3/joulescope_ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/dmg_background.png
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/dmg_background.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/dmg_background@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.824900 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_128x128.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_256x256.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_512x512.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_64x64.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/logo-large.png
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources/zoom.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-04-05 18:34:43.000000 joulescope_ui-1.1.3/joulescope_ui/resources.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/safe_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/shift_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/source_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.828900 joulescope_ui-1.1.3/joulescope_ui/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/color_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/color_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/font_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.832900 joulescope_ui-1.1.3/joulescope_ui/styles/js1/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/arrow_down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/arrow_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/arrow_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/arrow_up.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/branch_closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/branch_end.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/branch_end_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/branch_more.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/branch_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/branch_vline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/detach.svg
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/hmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/hsepartoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/radio_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/radio_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/style.html
--rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/tabs_menu.svg
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/transparent.svg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/vmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/js1/vsepartoolbars.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.832900 joulescope_ui-1.1.3/joulescope_ui/styles/system/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/system/index.json
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/system/style.html
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/system/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/system/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/system/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/system/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.832900 joulescope_ui-1.1.3/joulescope_ui/styles/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/test/test_color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/styles/test/test_parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.836900 joulescope_ui-1.1.3/joulescope_ui/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/anno1.anno.jls
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_annotation_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_disk_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_pubsub_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_range_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_source_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/test/test_versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 18:34:35.000000 joulescope_ui-1.1.3/joulescope_ui/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/ui_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widget_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.836900 joulescope_ui-1.1.3/joulescope_ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.836900 joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/accumulator_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.836900 joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.836900 joulescope_ui-1.1.3/joulescope_ui/widgets/clock/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/clock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/clock/clock_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.840901 joulescope_ui-1.1.3/joulescope_ui/widgets/developer/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/developer/log_view_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/developer/profile_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/developer/publish_spy_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.840901 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/current_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/device_control_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/device_info_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/device_update_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/active_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/device_close.svg
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/device_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/doc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/open.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/target_power_off.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/double_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/draggable_list_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/example/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/example/example_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/example/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/example/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/example/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/example/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/flyout_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/hamburger/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/hamburger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/hamburger/hamburger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/help/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/help/help_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/jls_info/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/jls_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/jls_info/jls_info_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/js220_cal/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/js220_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/js220_cal/current_offset.png
--rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/js220_cal/voltage_offset.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.844900 joulescope_ui-1.1.3/joulescope_ui/widgets/memory/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/memory/memory_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.848901 joulescope_ui-1.1.3/joulescope_ui/widgets/memory/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/memory/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/memory/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.848901 joulescope_ui-1.1.3/joulescope_ui/widgets/notes/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/notes/notes_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.848901 joulescope_ui-1.1.3/joulescope_ui/widgets/progress_bar/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/progress_bar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.848901 joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/record_status_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.848901 joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.848901 joulescope_ui-1.1.3/joulescope_ui/widgets/report_issue/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/report_issue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/report_issue/report_issue_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.848901 joulescope_ui-1.1.3/joulescope_ui/widgets/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24258 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/settings/settings_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/settings/unique_strings_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.848901 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/sidebar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.852901 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/device.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/help.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/memory.svg
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/misc.svg
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/play.svg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/stop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.852901 joulescope_ui-1.1.3/joulescope_ui/widgets/signal_record/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/signal_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/signal_record/disk_full_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/signal_record/signal_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.852901 joulescope_ui-1.1.3/joulescope_ui/widgets/statistics_record/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/statistics_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/statistics_record/statistics_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.852901 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/condition_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.856901 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/active.svg
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/continuous.svg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/inactive.svg
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/searching.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/single.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.856901 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/test/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/test/test_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/test/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/trigger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.856901 joulescope_ui-1.1.3/joulescope_ui/widgets/value/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/value/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.856901 joulescope_ui-1.1.3/joulescope_ui/widgets/value/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/value/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/value/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/value/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/value/value_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.856901 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.856901 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/styles/add.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/styles/delete.svg
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/styles/move.svg
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/styles/reset.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/view_manager_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.860901 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/annotations.md
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/interval_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/line_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/quantities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.860901 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/marker_add1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/marker_add2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/marker_clear.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/pin_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/pin_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/style_defines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/trace.svg
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.860901 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/test/test_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/text_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/waveform_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/waveform_source_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)   169445 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/waveform_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/y_range_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/joulescope_ui/zip_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:34:44.860901 joulescope_ui-1.1.3/joulescope_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-05 18:34:44.000000 joulescope_ui-1.1.3/joulescope_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17129 2024-04-05 18:34:44.000000 joulescope_ui-1.1.3/joulescope_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:34:44.000000 joulescope_ui-1.1.3/joulescope_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 18:34:44.000000 joulescope_ui-1.1.3/joulescope_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-05 18:34:44.000000 joulescope_ui-1.1.3/joulescope_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 18:34:44.000000 joulescope_ui-1.1.3/joulescope_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-05 18:34:44.864901 joulescope_ui-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-05 18:34:04.000000 joulescope_ui-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.888220 joulescope_ui-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    52815 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-18 18:58:20.888220 joulescope_ui-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-18 18:58:19.000000 joulescope_ui-1.1.4/joulescope.iss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.824219 joulescope_ui-1.1.4/joulescope_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    52815 2024-04-18 18:58:09.000000 joulescope_ui-1.1.4/joulescope_ui/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-18 18:58:09.000000 joulescope_ui-1.1.4/joulescope_ui/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/dev_signal_buffer_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.828219 joulescope_ui-1.1.4/joulescope_ui/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/device_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.828219 joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/js110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/js220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/js220_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/js220_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.828219 joulescope_ui-1.1.4/joulescope_ui/devices/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/devices/test/test_device_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/disk_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.828219 joulescope_ui-1.1.4/joulescope_ui/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/entry_points/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/entry_points/zip_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/error_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/error_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/expanding_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/file_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/filename_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.828219 joulescope_ui-1.1.4/joulescope_ui/fonts/DSEG14-Modern/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.828219 joulescope_ui-1.1.4/joulescope_ui/fonts/Hack/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/fonts/Hack/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.828219 joulescope_ui-1.1.4/joulescope_ui/fonts/Lato/
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/fonts/Lato/OFL.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.828219 joulescope_ui-1.1.4/joulescope_ui/fonts/SourceCodePro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/fonts/SourceCodePro/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.828219 joulescope_ui-1.1.4/joulescope_ui/fonts/SourceSerifPro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/fonts/SourceSerifPro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-04-18 18:58:20.000000 joulescope_ui-1.1.4/joulescope_ui/fonts.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/help_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/intel_graphics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/jls_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/jls_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/jls_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/jls_v2_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/json_plus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.832219 joulescope_ui-1.1.4/joulescope_ui/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/locale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.832219 joulescope_ui-1.1.4/joulescope_ui/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    81477 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   111976 2024-04-18 18:58:10.000000 joulescope_ui-1.1.4/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.832219 joulescope_ui-1.1.4/joulescope_ui/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    71341 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   102241 2024-04-18 18:58:10.000000 joulescope_ui-1.1.4/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.832219 joulescope_ui-1.1.4/joulescope_ui/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    99006 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   129930 2024-04-18 18:58:10.000000 joulescope_ui-1.1.4/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.832219 joulescope_ui-1.1.4/joulescope_ui/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    71457 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   102311 2024-04-18 18:58:10.000000 joulescope_ui-1.1.4/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.832219 joulescope_ui-1.1.4/joulescope_ui/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    72880 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   103793 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.832219 joulescope_ui-1.1.4/joulescope_ui/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    72116 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   103009 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.836219 joulescope_ui-1.1.4/joulescope_ui/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    75360 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   105360 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)    68228 2024-04-18 18:58:10.000000 joulescope_ui-1.1.4/joulescope_ui/locale/joulescope_ui.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.836219 joulescope_ui-1.1.4/joulescope_ui/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    70112 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   100201 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.804219 joulescope_ui-1.1.4/joulescope_ui/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.836219 joulescope_ui-1.1.4/joulescope_ui/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    61187 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    91067 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40925 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/mem_leak_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.836219 joulescope_ui-1.1.4/joulescope_ui/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.836219 joulescope_ui-1.1.4/joulescope_ui/plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.836219 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.836219 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/p1/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/p1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/p1/index.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.840220 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/p2/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/p2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/p2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/p2/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/plugins/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/process_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66439 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/pubsub_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/pubsub_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/range_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.840220 joulescope_ui-1.1.4/joulescope_ui/range_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/range_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/range_tools/cdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/range_tools/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/range_tools/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/range_tools/max_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/range_tools/plugin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/range_tools/usb_inrush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.840220 joulescope_ui-1.1.4/joulescope_ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/dmg_background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/dmg_background.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/dmg_background@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.844220 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_128x128.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_256x256.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_512x512.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_64x64.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/logo-large.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources/zoom.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-04-18 18:58:19.000000 joulescope_ui-1.1.4/joulescope_ui/resources.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/safe_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/shift_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/source_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.844220 joulescope_ui-1.1.4/joulescope_ui/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/color_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/font_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.852220 joulescope_ui-1.1.4/joulescope_ui/styles/js1/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/arrow_down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/arrow_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/arrow_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/arrow_up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/branch_closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/branch_end.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/branch_end_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/branch_more.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/branch_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/branch_vline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/detach.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/hmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/hsepartoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/radio_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/radio_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/tabs_menu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/transparent.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/vmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/js1/vsepartoolbars.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.852220 joulescope_ui-1.1.4/joulescope_ui/styles/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/system/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/system/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/system/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/system/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/system/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/system/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.852220 joulescope_ui-1.1.4/joulescope_ui/styles/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/test/test_color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/styles/test/test_parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.856220 joulescope_ui-1.1.4/joulescope_ui/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/anno1.anno.jls
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_annotation_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_disk_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_pubsub_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_range_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_source_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/test/test_versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 18:58:11.000000 joulescope_ui-1.1.4/joulescope_ui/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/ui_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widget_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.856220 joulescope_ui-1.1.4/joulescope_ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.856220 joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/accumulator_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.860220 joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.860220 joulescope_ui-1.1.4/joulescope_ui/widgets/clock/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/clock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/clock/clock_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.860220 joulescope_ui-1.1.4/joulescope_ui/widgets/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/developer/log_view_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/developer/profile_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/developer/publish_spy_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.860220 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/current_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/device_control_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/device_info_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/device_update_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.864220 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/active_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/device_close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/device_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/doc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/target_power_off.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/double_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/draggable_list_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.864220 joulescope_ui-1.1.4/joulescope_ui/widgets/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/example/example_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.864220 joulescope_ui-1.1.4/joulescope_ui/widgets/example/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/example/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/example/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/example/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.864220 joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/flyout_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.864220 joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.864220 joulescope_ui-1.1.4/joulescope_ui/widgets/hamburger/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/hamburger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/hamburger/hamburger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.868220 joulescope_ui-1.1.4/joulescope_ui/widgets/help/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/help/help_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.868220 joulescope_ui-1.1.4/joulescope_ui/widgets/jls_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/jls_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/jls_info/jls_info_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.868220 joulescope_ui-1.1.4/joulescope_ui/widgets/js220_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/js220_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/js220_cal/current_offset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/js220_cal/voltage_offset.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.868220 joulescope_ui-1.1.4/joulescope_ui/widgets/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/memory/memory_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.868220 joulescope_ui-1.1.4/joulescope_ui/widgets/memory/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/memory/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/memory/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.868220 joulescope_ui-1.1.4/joulescope_ui/widgets/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/notes/notes_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.868220 joulescope_ui-1.1.4/joulescope_ui/widgets/progress_bar/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/progress_bar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.868220 joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/record_status_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.872220 joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.872220 joulescope_ui-1.1.4/joulescope_ui/widgets/report_issue/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/report_issue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/report_issue/report_issue_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.872220 joulescope_ui-1.1.4/joulescope_ui/widgets/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24258 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/settings/settings_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/settings/unique_strings_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.872220 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/sidebar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.876220 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/device.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/memory.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/misc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.876220 joulescope_ui-1.1.4/joulescope_ui/widgets/signal_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/signal_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/signal_record/disk_full_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/signal_record/signal_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.876220 joulescope_ui-1.1.4/joulescope_ui/widgets/statistics_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/statistics_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/statistics_record/statistics_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.876220 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/condition_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.876220 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/active.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/continuous.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/searching.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/single.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.880220 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/test/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/test/test_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/test/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/trigger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.880220 joulescope_ui-1.1.4/joulescope_ui/widgets/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/value/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.880220 joulescope_ui-1.1.4/joulescope_ui/widgets/value/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/value/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/value/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/value/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/value/value_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.880220 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.880220 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/styles/add.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/styles/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/styles/move.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/styles/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/view_manager_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.884220 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/annotations.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/interval_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/line_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/quantities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.884220 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/marker_add1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/marker_add2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/marker_clear.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/pin_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/pin_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/style_defines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/trace.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.888220 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/test/test_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/text_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/waveform_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/waveform_source_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169445 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/waveform_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/y_range_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/joulescope_ui/zip_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:58:20.888220 joulescope_ui-1.1.4/joulescope_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-18 18:58:20.000000 joulescope_ui-1.1.4/joulescope_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-04-18 18:58:20.000000 joulescope_ui-1.1.4/joulescope_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:58:20.000000 joulescope_ui-1.1.4/joulescope_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 18:58:20.000000 joulescope_ui-1.1.4/joulescope_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-18 18:58:20.000000 joulescope_ui-1.1.4/joulescope_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 18:58:20.000000 joulescope_ui-1.1.4/joulescope_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 18:58:20.888220 joulescope_ui-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-18 18:57:50.000000 joulescope_ui-1.1.4/setup.py
```

### Comparing `joulescope_ui-1.1.3/CHANGELOG.md` & `joulescope_ui-1.1.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
-## 1.1.3
+## 1.1.4
 
-2024 Apr 5
+2024 Apr 18
 
 * Added plugin framework with live code reload  #14
 * Restructured code to support human language translation.
-* Added AI translations: ar, de, el, es, fr, ja, ko, zh.
+* Added AI translations: ar, de, el, es, fr, it, ja, ko, zh.
 * Added Intel graphics dialog to display sequence  #245
 * Modified QComboBox style.
 * Added filename replacement variables.
 * Added Trigger widget.
 
 
 ## 1.0.62
```

### Comparing `joulescope_ui-1.1.3/CREDITS.html` & `joulescope_ui-1.1.4/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/LICENSE.txt` & `joulescope_ui-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/PKG-INFO` & `joulescope_ui-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.3
+Version: 1.1.4
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.1.3/README.md` & `joulescope_ui-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope.iss` & `joulescope_ui-1.1.4/joulescope.iss`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "Joulescope"
-#define MyAppVersion "1.1.3"
-#define MyAppVersionUnderscores "1_1_3"
+#define MyAppVersion "1.1.4"
+#define MyAppVersionUnderscores "1_1_4"
 #define MyAppPublisher "Jetperch LLC"
 #define MyAppURL "https://www.joulescope.com"
 #define MyAppExeName "joulescope.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application.
 ; Do not use the same AppId value in installers for other applications.
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/CHANGELOG.md` & `joulescope_ui-1.1.4/joulescope_ui/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
-## 1.1.3
+## 1.1.4
 
-2024 Apr 5
+2024 Apr 18
 
 * Added plugin framework with live code reload  #14
 * Restructured code to support human language translation.
-* Added AI translations: ar, de, el, es, fr, ja, ko, zh.
+* Added AI translations: ar, de, el, es, fr, it, ja, ko, zh.
 * Added Intel graphics dialog to display sequence  #245
 * Modified QComboBox style.
 * Added filename replacement variables.
 * Added Trigger widget.
 
 
 ## 1.0.62
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/CREDITS.html` & `joulescope_ui-1.1.4/joulescope_ui/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/__main__.py` & `joulescope_ui-1.1.4/joulescope_ui/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/about.py` & `joulescope_ui-1.1.4/joulescope_ui/about.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/api.py` & `joulescope_ui-1.1.4/joulescope_ui/api.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/app.py` & `joulescope_ui-1.1.4/joulescope_ui/app.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/capabilities.py` & `joulescope_ui-1.1.4/joulescope_ui/capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/dev_signal_buffer_source.py` & `joulescope_ui-1.1.4/joulescope_ui/dev_signal_buffer_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/devices/device_update.py` & `joulescope_ui-1.1.4/joulescope_ui/devices/device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/device.py` & `joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/device.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/js110.py` & `joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/js110.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/js220.py` & `joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/js220.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/js220_fuse.py` & `joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/js220_fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/js220_updater.py` & `joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/js220_updater.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py` & `joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py` & `joulescope_ui-1.1.4/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/devices/test/test_device_update.py` & `joulescope_ui-1.1.4/joulescope_ui/devices/test/test_device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/disk_monitor.py` & `joulescope_ui-1.1.4/joulescope_ui/disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/entry_points/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/entry_points/ui.py` & `joulescope_ui-1.1.4/joulescope_ui/entry_points/ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/entry_points/zip_inspector.py` & `joulescope_ui-1.1.4/joulescope_ui/entry_points/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/error_dialog.py` & `joulescope_ui-1.1.4/joulescope_ui/error_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/error_window.py` & `joulescope_ui-1.1.4/joulescope_ui/error_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/expanding_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/expanding_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/exporter.py` & `joulescope_ui-1.1.4/joulescope_ui/exporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/file_dialog.py` & `joulescope_ui-1.1.4/joulescope_ui/file_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/filename_formatter.py` & `joulescope_ui-1.1.4/joulescope_ui/filename_formatter.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from joulescope_ui import N_, time64, pubsub_singleton, get_topic_name
 import os
 
 
+_DEVICE_IDENTIFIER = N_('The device identifier.')
+_DEVICE_NAME = N_('The user-configurable device name.')
+_DEVICE_MODEL = N_('The device model.')
+_DEVICE_SERIAL_NUMBER = N_('The device serial number.')
+_FILENAME_CONFIG = N_('Configure the filename')
+_REPLACEMENTS = N_('The filename supports the following replacements.')
+_TIMESTAMP = N_('The current timestamp.')
+_COUNT = N_('The number of times the filename has been used.')
+_PROCESS_ID = N_('The process ID for this Joulescope UI invocation.')
+
+
 HTML_STYLE = """\
 <style>
 table {
   border-collapse: collapse
 }
 th, td {
   padding: 5px;
@@ -29,50 +40,50 @@
 """
 
 
 def filename_tooltip(device_id=None):
     device_id_str = f"""\
       <tr>
         <td>{{device_id}}</td>
-        <td>{N_('The device identifier.')}</td>
+        <td>{_DEVICE_IDENTIFIER}</td>
       </tr>
       <tr>
         <td>{{device_name}}</td>
-        <td>{N_('The user-configurable device name.')}</td>
+        <td>{_DEVICE_NAME}</td>
       </tr>
       <tr>
         <td>{{device_model}}</td>
-        <td>{N_('The device model.')}</td>
+        <td>{_DEVICE_MODEL}</td>
       </tr>
       <tr>
         <td>{{device_serial_number}}</td>
-        <td>{N_('The device serial number.')}</td>
+        <td>{_DEVICE_SERIAL_NUMBER}</td>
       </tr>\
     """
     if not device_id:
         device_id_str = ''
 
     return f"""\
     <html><header>{HTML_STYLE}</header>
     <body>
-    <h3>{N_('Configure the filename')}</h3>
-    <p>{N_('The filename supports the following replacements.')}
+    <h3>{_FILENAME_CONFIG}</h3>
+    <p>{_REPLACEMENTS}
     <p><table>
       <tr>
         <td>{{timestamp}}</td>
-        <td>{N_('The current timestamp.')}</td>
+        <td>{_TIMESTAMP}</td>
       </tr>
       <tr>
         <td>{{count}}</td>
-        <td>{N_('The number of times the filename has been used.')}</td>
+        <td>{_COUNT}</td>
       </tr>
       {device_id_str}
       <tr>
         <td>{{process_id}}</td>
-        <td>{N_('The process ID for this Joulescope UI invocation.')}</td>
+        <td>{_PROCESS_ID}</td>
       </tr>  
     </table></p></body></html>
     """
 
 
 def filename_formatter(filename, count, device_id=None, **kwargs):
     """Format a filename.
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt` & `joulescope_ui-1.1.4/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/fonts/Hack/LICENSE.md` & `joulescope_ui-1.1.4/joulescope_ui/fonts/Hack/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/fonts/Lato/OFL.txt` & `joulescope_ui-1.1.4/joulescope_ui/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/fonts/SourceCodePro/LICENSE.md` & `joulescope_ui-1.1.4/joulescope_ui/fonts/SourceCodePro/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/fonts/SourceSerifPro/OFL.txt` & `joulescope_ui-1.1.4/joulescope_ui/fonts/SourceSerifPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/fonts.rcc` & `joulescope_ui-1.1.4/joulescope_ui/fonts.rcc`

 * *Files 1% similar despite different names*

```diff
@@ -193814,70 +193814,70 @@
 002f5150: 0000 0000 0000 0000 0000 0080 0002 0000  ................
 002f5160: 000a 0000 0027 0000 0000 0000 0000 0000  .....'..........
 002f5170: 0050 0002 0000 000c 0000 001b 0000 0000  .P..............
 002f5180: 0000 0000 0000 0010 0002 0000 0006 0000  ................
 002f5190: 0015 0000 0000 0000 0000 0000 0030 0002  .............0..
 002f51a0: 0000 000e 0000 0007 0000 0000 0000 0000  ................
 002f51b0: 0000 071a 0004 0000 0001 0025 4f27 0000  ...........%O'..
-002f51c0: 018e af8a 1110 0000 07c4 0004 0000 0001  ................
-002f51d0: 0029 2537 0000 018e af8a 110c 0000 058c  .)%7............
-002f51e0: 0004 0000 0001 001c 6407 0000 018e af8a  ........d.......
-002f51f0: 1110 0000 05ba 0004 0000 0001 001d 95a3  ................
-002f5200: 0000 018e af8a 1118 0000 0750 0004 0000  ...........P....
-002f5210: 0001 0026 8517 0000 018e af8a 111c 0000  ...&............
+002f51c0: 018e f292 7ecb 0000 07c4 0004 0000 0001  ....~...........
+002f51d0: 0029 2537 0000 018e f292 7ec7 0000 058c  .)%7......~.....
+002f51e0: 0004 0000 0001 001c 6407 0000 018e f292  ........d.......
+002f51f0: 7ecb 0000 05ba 0004 0000 0001 001d 95a3  ~...............
+002f5200: 0000 018e f292 7ed3 0000 0750 0004 0000  ......~....P....
+002f5210: 0001 0026 8517 0000 018e f292 7ed7 0000  ...&........~...
 002f5220: 07fc 0004 0000 0001 002a 5802 0000 018e  .........*X.....
-002f5230: af8a 110c 0000 082e 0004 0000 0001 002b  ...............+
-002f5240: c4d1 0000 018e af8a 1114 0000 062c 0004  .............,..
-002f5250: 0000 0001 0020 3160 0000 018e af8a 1118  ..... 1`........
+002f5230: f292 7ec7 0000 082e 0004 0000 0001 002b  ..~............+
+002f5240: c4d1 0000 018e f292 7ecf 0000 062c 0004  ........~....,..
+002f5250: 0000 0001 0020 3160 0000 018e f292 7ed3  ..... 1`......~.
 002f5260: 0000 05f4 0004 0000 0001 001f 01ac 0000  ................
-002f5270: 018e af8a 1114 0000 078e 0004 0000 0001  ................
-002f5280: 0027 bab6 0000 018e af8a 1118 0000 0666  .'.............f
-002f5290: 0004 0000 0001 0021 6449 0000 018e af8a  .......!dI......
-002f52a0: 1110 0000 06e6 0004 0000 0001 0023 e72d  .............#.-
-002f52b0: 0000 018e af8a 110c 0000 0862 0004 0000  ...........b....
-002f52c0: 0001 002d 262d 0000 018e af8a 1118 0000  ...-&-..........
+002f5270: 018e f292 7ecf 0000 078e 0004 0000 0001  ....~...........
+002f5280: 0027 bab6 0000 018e f292 7ed3 0000 0666  .'........~....f
+002f5290: 0004 0000 0001 0021 6449 0000 018e f292  .......!dI......
+002f52a0: 7ecb 0000 06e6 0004 0000 0001 0023 e72d  ~............#.-
+002f52b0: 0000 018e f292 7ec7 0000 0862 0004 0000  ......~....b....
+002f52c0: 0001 002d 262d 0000 018e f292 7ed3 0000  ...-&-......~...
 002f52d0: 06a8 0004 0000 0001 0022 8ce5 0000 018e  ........."......
-002f52e0: af8a 1110 0000 089a 0004 0000 0001 002e  ................
-002f52f0: 90bc 0000 018e af8a 10fc 0000 08d0 0004  ................
-002f5300: 0000 0001 002e af00 0000 018e af8a 10fc  ................
+002f52e0: f292 7ecb 0000 089a 0004 0000 0001 002e  ..~.............
+002f52f0: 90bc 0000 018e f292 7eb7 0000 08d0 0004  ........~.......
+002f5300: 0000 0001 002e af00 0000 018e f292 7eb7  ..............~.
 002f5310: 0000 097c 0004 0000 0001 002f 0ab2 0000  ...|......./....
-002f5320: 018e af8a 10fc 0000 09b0 0004 0000 0001  ................
-002f5330: 002f 293e 0000 018e af8a 10fc 0000 090c  ./)>............
-002f5340: 0004 0000 0001 002e cd3f 0000 018e af8a  .........?......
-002f5350: 10fc 0000 094a 0004 0000 0001 002e ec32  .....J.........2
-002f5360: 0000 018e af8a 10fc 0000 0544 0004 0000  ...........D....
-002f5370: 0001 001b 3ffe 0000 018e af8a 1128 0000  ....?........(..
+002f5320: 018e f292 7eb7 0000 09b0 0004 0000 0001  ....~...........
+002f5330: 002f 293e 0000 018e f292 7eb7 0000 090c  ./)>......~.....
+002f5340: 0004 0000 0001 002e cd3f 0000 018e f292  .........?......
+002f5350: 7eb7 0000 094a 0004 0000 0001 002e ec32  ~....J.........2
+002f5360: 0000 018e f292 7eb7 0000 0544 0004 0000  ......~....D....
+002f5370: 0001 001b 3ffe 0000 018e f292 7ee3 0000  ....?.......~...
 002f5380: 036a 0004 0000 0001 0010 f545 0000 018e  .j.........E....
-002f5390: af8a 1120 0000 041a 0004 0000 0001 0014  ... ............
-002f53a0: f75f 0000 018e af8a 1120 0000 048c 0004  ._....... ......
-002f53b0: 0000 0001 0017 6f8d 0000 018e af8a 1124  ......o........$
+002f5390: f292 7edb 0000 041a 0004 0000 0001 0014  ..~.............
+002f53a0: f75f 0000 018e f292 7edb 0000 048c 0004  ._......~.......
+002f53b0: 0000 0001 0017 6f8d 0000 018e f292 7edf  ......o.......~.
 002f53c0: 0000 04c2 0004 0000 0001 0018 d613 0000  ................
-002f53d0: 018e af8a 1120 0000 03aa 0004 0000 0001  ..... ..........
-002f53e0: 0012 1971 0000 018e af8a 111c 0000 03de  ...q............
-002f53f0: 0004 0000 0001 0013 8810 0000 018e af8a  ................
-002f5400: 1124 0000 02dc 0004 0000 0001 000e c39f  .$..............
-002f5410: 0000 018e af8a 1124 0000 0452 0004 0000  .......$...R....
-002f5420: 0001 0016 0ed3 0000 018e af8a 1124 0000  .............$..
+002f53d0: 018e f292 7edb 0000 03aa 0004 0000 0001  ....~...........
+002f53e0: 0012 1971 0000 018e f292 7ed7 0000 03de  ...q......~.....
+002f53f0: 0004 0000 0001 0013 8810 0000 018e f292  ................
+002f5400: 7edf 0000 02dc 0004 0000 0001 000e c39f  ~...............
+002f5410: 0000 018e f292 7edf 0000 0452 0004 0000  ......~....R....
+002f5420: 0001 0016 0ed3 0000 018e f292 7edf 0000  ............~...
 002f5430: 0502 0004 0000 0001 001a 2aab 0000 018e  ..........*.....
-002f5440: af8a 111c 0000 031e 0004 0000 0001 000f  ................
-002f5450: e47b 0000 018e af8a 1120 0000 02a6 0004  .{....... ......
-002f5460: 0000 0001 000d 65a3 0000 018e af8a 111c  ......e.........
+002f5440: f292 7ed7 0000 031e 0004 0000 0001 000f  ..~.............
+002f5450: e47b 0000 018e f292 7edb 0000 02a6 0004  .{......~.......
+002f5460: 0000 0001 000d 65a3 0000 018e f292 7ed7  ......e.......~.
 002f5470: 0000 01ae 0004 0000 0001 0003 6c6f 0000  ............lo..
-002f5480: 018e af8a 1108 0000 008e 0004 0000 0001  ................
-002f5490: 0000 0000 0000 018e af8a 1108 0000 018a  ................
-002f54a0: 0004 0000 0001 0002 e1fa 0000 018e af8a  ................
-002f54b0: 1108 0000 010a 0004 0000 0001 0001 72aa  ..............r.
-002f54c0: 0000 018e af8a 1108 0000 00e8 0004 0000  ................
-002f54d0: 0001 0000 f2c6 0000 018e af8a 1104 0000  ................
+002f5480: 018e f292 7ec3 0000 008e 0004 0000 0001  ....~...........
+002f5490: 0000 0000 0000 018e f292 7ec3 0000 018a  ..........~.....
+002f54a0: 0004 0000 0001 0002 e1fa 0000 018e f292  ................
+002f54b0: 7ec3 0000 010a 0004 0000 0001 0001 72aa  ~.............r.
+002f54c0: 0000 018e f292 7ec3 0000 00e8 0004 0000  ......~.........
+002f54d0: 0001 0000 f2c6 0000 018e f292 7ebf 0000  ............~...
 002f54e0: 015e 0004 0000 0001 0002 7e0b 0000 018e  .^........~.....
-002f54f0: af8a 1108 0000 00ba 0004 0000 0001 0000  ................
-002f5500: 8b33 0000 018e af8a 1108 0000 01f0 0004  .3..............
-002f5510: 0000 0001 0004 74f0 0000 018e af8a 1108  ......t.........
+002f54f0: f292 7ec3 0000 00ba 0004 0000 0001 0000  ..~.............
+002f5500: 8b33 0000 018e f292 7ec3 0000 01f0 0004  .3......~.......
+002f5510: 0000 0001 0004 74f0 0000 018e f292 7ec3  ......t.......~.
 002f5520: 0000 01ce 0004 0000 0001 0003 ee66 0000  .............f..
-002f5530: 018e af8a 1108 0000 0130 0004 0000 0001  .........0......
-002f5540: 0001 f768 0000 018e af8a 1104 0000 0210  ...h............
-002f5550: 0004 0000 0001 0004 f353 0000 018e af8a  .........S......
-002f5560: 1104 0000 027a 0004 0000 0001 000b 366d  .....z........6m
-002f5570: 0000 018e af8a 1100 0000 0234 0004 0000  ...........4....
-002f5580: 0001 0007 158f 0000 018e af8a 1100 0000  ................
+002f5530: 018e f292 7ec3 0000 0130 0004 0000 0001  ....~....0......
+002f5540: 0001 f768 0000 018e f292 7ebf 0000 0210  ...h......~.....
+002f5550: 0004 0000 0001 0004 f353 0000 018e f292  .........S......
+002f5560: 7ebf 0000 027a 0004 0000 0001 000b 366d  ~....z........6m
+002f5570: 0000 018e f292 7ebb 0000 0234 0004 0000  ......~....4....
+002f5580: 0001 0007 158f 0000 018e f292 7ebb 0000  ............~...
 002f5590: 0254 0004 0000 0001 0009 2ac5 0000 018e  .T........*.....
-002f55a0: af8a 1104                                ....
+002f55a0: f292 7ebf                                ..~.
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/getting_started.py` & `joulescope_ui-1.1.4/joulescope_ui/getting_started.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/help_ui.py` & `joulescope_ui-1.1.4/joulescope_ui/help_ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/intel_graphics_dialog.py` & `joulescope_ui-1.1.4/joulescope_ui/intel_graphics_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/jls_source.py` & `joulescope_ui-1.1.4/joulescope_ui/jls_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/jls_v1.py` & `joulescope_ui-1.1.4/joulescope_ui/jls_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/jls_v2.py` & `joulescope_ui-1.1.4/joulescope_ui/jls_v2.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/jls_v2_annotations.py` & `joulescope_ui-1.1.4/joulescope_ui/jls_v2_annotations.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/json_plus.py` & `joulescope_ui-1.1.4/joulescope_ui/json_plus.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.4/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ar\n"
 "Language-Team: ar <LL@li.org>\n"
 "Plural-Forms: nplurals=6; plural=(n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=0 && n%100<=2 ? 4 : 5);\n"
 "MIME-Version: 1.0\n"
@@ -448,14 +448,17 @@
 msgstr ""
 "قم بتكوين نوع مرشح النطاق الحالي (IRF) الذي يحدد آلية التصفية المطبقة على "
 "تغييرات النطاق الحالي. لا نوصي بتغيير هذه الإعدادات للتشغيل العادي."
 
 msgid "Configure the direction of the JS220's trigger BNC connection."
 msgstr "قم بتكوين اتجاه وصلة BNC لمشغل JS220 الخاص بـ JS220."
 
+msgid "Configure the filename"
+msgstr "تكوين اسم الملف"
+
 msgid "Configure trigger options and then press to start."
 msgstr "قم بتكوين خيارات المشغل ثم اضغط للبدء."
 
 msgid "Connect"
 msgstr "توصيل"
 
 msgid ""
@@ -1668,23 +1671,35 @@
 "to measure your current signal. It can also be helpful in separating target "
 "system behavior from the small current range switching artifacts."
 msgstr ""
 "يعد النطاق الحالي مفيدًا لفهم كيفية قيام جولسكوب Joulescope بالتدرج التلقائي "
 "لقياس الإشارة الحالية. يمكن أن يكون مفيدًا أيضًا في فصل سلوك النظام المستهدف "
 "عن القطع الأثرية لتبديل النطاق الحالي الصغير."
 
+msgid "The current timestamp."
+msgstr "الطابع الزمني الحالي."
+
 msgid "The default path for loading and saving files."
 msgstr "المسار الافتراضي لتحميل الملفات وحفظها."
 
 msgid "The default path method"
 msgstr "طريقة المسار الافتراضي"
 
 msgid "The default unique_id for the default statistics streaming source."
 msgstr "المعرف_الفريد الافتراضي لمصدر تدفق الإحصائيات الافتراضي."
 
+msgid "The device identifier."
+msgstr "معرّف الجهاز."
+
+msgid "The device model."
+msgstr "طراز الجهاز."
+
+msgid "The device serial number."
+msgstr "الرقم التسلسلي للجهاز."
+
 msgid "The device to use for the start condition and stop condition."
 msgstr "الجهاز المستخدم لحالة البدء وحالة التوقف."
 
 msgid "The disk is full"
 msgstr "القرص ممتلئ"
 
 msgid ""
@@ -1700,14 +1715,17 @@
 msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "ثابت زمن التضاؤل الأسي. يبدد المصهر 63.2 بالمائة من الطاقة المتراكمة في هذه "
 "المدة."
 
+msgid "The filename supports the following replacements."
+msgstr "يدعم اسم الملف البدائل التالية."
+
 msgid "The filename with optional replacements."
 msgstr "اسم الملف مع بدائل اختيارية."
 
 msgid "The fixed default path for loading and saving files."
 msgstr "المسار الافتراضي الثابت لتحميل الملفات وحفظها."
 
 msgid "The flyout width in pixels."
@@ -1747,17 +1765,23 @@
 msgid ""
 "The number of samples before the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "عدد العينات قبل نافذة النطاق الحالي المستخدمة لتحديد المتوسط. يتم تجاهل هذه "
 "القيمة لجميع أنواع IRF الأخرى."
 
+msgid "The number of times the filename has been used."
+msgstr "عدد مرات استخدام اسم الملف."
+
 msgid "The precision to display in digits."
 msgstr "دقة العرض بالأرقام."
 
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "معرّف العملية لاستدعاء واجهة مستخدم Joulescope UI هذا."
+
 msgid "The pyjoulescope_driver log level."
 msgstr "مستوى سجل pyjoulescope_driver."
 
 msgid "The quantities to display by default."
 msgstr "الكميات المراد عرضها افتراضيًا."
 
 msgid ""
@@ -1824,14 +1848,17 @@
 
 msgid "The unique_id for the default signal streaming source."
 msgstr "المعرف الفريد لمصدر تدفق الإشارة الافتراضي."
 
 msgid "The units to display."
 msgstr "وحدات العرض."
 
+msgid "The user-configurable device name."
+msgstr "اسم الجهاز القابل للتكوين من قِبل المستخدم."
+
 msgid ""
 "The values displayed by this widget come from a single source device. Select "
 "the source device here."
 msgstr ""
 "تأتي القيم التي تعرضها هذه الأداة من جهاز مصدر واحد. حدد الجهاز المصدر هنا."
 
 msgid "The voltage between any sensor port must never exceed ±15V."
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.4/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ar <LL@li.org>\n"
 "Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -394,14 +394,50 @@
 msgid ""
 "Exporting data to a JLS file. You can open this file later to display the "
 "exported data."
 msgstr ""
 "تصدير البيانات إلى ملف JLS. يمكنك فتح هذا الملف لاحقًا لعرض البيانات "
 "المصدرة."
 
+#: filename_formatter.py:19
+msgid "The device identifier."
+msgstr "معرّف الجهاز."
+
+#: filename_formatter.py:20
+msgid "The user-configurable device name."
+msgstr "اسم الجهاز القابل للتكوين من قِبل المستخدم."
+
+#: filename_formatter.py:21
+msgid "The device model."
+msgstr "طراز الجهاز."
+
+#: filename_formatter.py:22
+msgid "The device serial number."
+msgstr "الرقم التسلسلي للجهاز."
+
+#: filename_formatter.py:23
+msgid "Configure the filename"
+msgstr "تكوين اسم الملف"
+
+#: filename_formatter.py:24
+msgid "The filename supports the following replacements."
+msgstr "يدعم اسم الملف البدائل التالية."
+
+#: filename_formatter.py:25
+msgid "The current timestamp."
+msgstr "الطابع الزمني الحالي."
+
+#: filename_formatter.py:26
+msgid "The number of times the filename has been used."
+msgstr "عدد مرات استخدام اسم الملف."
+
+#: filename_formatter.py:27
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "معرّف العملية لاستدعاء واجهة مستخدم Joulescope UI هذا."
+
 #: getting_started.py:20
 msgid "Getting Started with Your Joulescope"
 msgstr "البدء باستخدام جولسكوب Joulescope الخاص بك"
 
 #: getting_started.py:22
 msgid "Safety"
 msgstr "السلامة"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.4/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -484,14 +484,17 @@
 "Konfigurieren Sie den Typ des Strombereichsfilters (IRF), der den auf "
 "Strombereichsänderungen angewandten Filtermechanismus bestimmt. Es wird "
 "nicht empfohlen, diese Einstellungen für den normalen Betrieb zu ändern."
 
 msgid "Configure the direction of the JS220's trigger BNC connection."
 msgstr "Konfigurieren Sie die Richtung des Trigger-BNC-Anschlusses des JS220."
 
+msgid "Configure the filename"
+msgstr "Konfigurieren Sie den Dateinamen"
+
 msgid "Configure trigger options and then press to start."
 msgstr ""
 "Konfigurieren Sie die Triggeroptionen und drücken Sie dann zum Starten."
 
 msgid "Connect"
 msgstr "Verbinden Sie"
 
@@ -1750,25 +1753,37 @@
 "system behavior from the small current range switching artifacts."
 msgstr ""
 "Der Strombereich ist nützlich, um zu verstehen, wie Ihr Joulescope das "
 "Stromsignal automatisch misst. Er kann auch hilfreich sein, um das Verhalten "
 "des Zielsystems von den Schaltartefakten des kleinen Strombereichs zu "
 "trennen."
 
+msgid "The current timestamp."
+msgstr "Der aktuelle Zeitstempel."
+
 msgid "The default path for loading and saving files."
 msgstr "Der Standardpfad zum Laden und Speichern von Dateien."
 
 msgid "The default path method"
 msgstr "Die Standardpfadmethode"
 
 msgid "The default unique_id for the default statistics streaming source."
 msgstr ""
 "Die standardmäßige unique_id für die standardmäßige Statistik-Streaming-"
 "Quelle."
 
+msgid "The device identifier."
+msgstr "Die Kennung des Geräts."
+
+msgid "The device model."
+msgstr "Das Gerätemodell."
+
+msgid "The device serial number."
+msgstr "Die Seriennummer des Geräts."
+
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "Das Gerät, das für die Startbedingung und die Stoppbedingung zu verwenden "
 "ist."
 
 msgid "The disk is full"
 msgstr "Die Festplatte ist voll"
@@ -1787,14 +1802,17 @@
 msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "Die exponentielle Abklingzeitkonstante. In dieser Zeitspanne baut die "
 "Sicherung 63,2 Prozent der angesammelten Energie ab."
 
+msgid "The filename supports the following replacements."
+msgstr "Der Dateiname unterstützt die folgenden Ersetzungen."
+
 msgid "The filename with optional replacements."
 msgstr "Der Dateiname mit optionalen Ersetzungen."
 
 msgid "The fixed default path for loading and saving files."
 msgstr "Der feste Standardpfad für das Laden und Speichern von Dateien."
 
 msgid "The flyout width in pixels."
@@ -1837,17 +1855,23 @@
 "The number of samples before the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Die Anzahl der Abtastungen vor dem Strombereichsfenster, das zur Bestimmung "
 "des Mittelwerts verwendet wird. Dieser Wert wird für alle anderen IRF-Typen "
 "ignoriert."
 
+msgid "The number of times the filename has been used."
+msgstr "Die Anzahl, wie oft der Dateiname verwendet wurde."
+
 msgid "The precision to display in digits."
 msgstr "Die Genauigkeit der Anzeige in Ziffern."
 
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "Die Prozess-ID für diesen Joulescope UI-Aufruf."
+
 msgid "The pyjoulescope_driver log level."
 msgstr "Der pyjoulescope_driver Log-Level."
 
 msgid "The quantities to display by default."
 msgstr "Die Größen, die standardmäßig angezeigt werden."
 
 msgid ""
@@ -1918,14 +1942,17 @@
 
 msgid "The unique_id for the default signal streaming source."
 msgstr "Die unique_id für die Standard-Signal-Streaming-Quelle."
 
 msgid "The units to display."
 msgstr "Die anzuzeigenden Einheiten."
 
+msgid "The user-configurable device name."
+msgstr "Der benutzerkonfigurierbare Gerätename."
+
 msgid ""
 "The values displayed by this widget come from a single source device. Select "
 "the source device here."
 msgstr ""
 "Die von diesem Widget angezeigten Werte stammen von einem einzigen "
 "Quellgerät. Wählen Sie hier das Quellgerät aus."
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.4/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: de <LL@li.org>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -412,14 +412,50 @@
 msgid ""
 "Exporting data to a JLS file. You can open this file later to display the "
 "exported data."
 msgstr ""
 "Exportieren von Daten in eine JLS-Datei. Sie können diese Datei später "
 "öffnen, um die exportierten Daten anzuzeigen."
 
+#: filename_formatter.py:19
+msgid "The device identifier."
+msgstr "Die Kennung des Geräts."
+
+#: filename_formatter.py:20
+msgid "The user-configurable device name."
+msgstr "Der benutzerkonfigurierbare Gerätename."
+
+#: filename_formatter.py:21
+msgid "The device model."
+msgstr "Das Gerätemodell."
+
+#: filename_formatter.py:22
+msgid "The device serial number."
+msgstr "Die Seriennummer des Geräts."
+
+#: filename_formatter.py:23
+msgid "Configure the filename"
+msgstr "Konfigurieren Sie den Dateinamen"
+
+#: filename_formatter.py:24
+msgid "The filename supports the following replacements."
+msgstr "Der Dateiname unterstützt die folgenden Ersetzungen."
+
+#: filename_formatter.py:25
+msgid "The current timestamp."
+msgstr "Der aktuelle Zeitstempel."
+
+#: filename_formatter.py:26
+msgid "The number of times the filename has been used."
+msgstr "Die Anzahl, wie oft der Dateiname verwendet wurde."
+
+#: filename_formatter.py:27
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "Die Prozess-ID für diesen Joulescope UI-Aufruf."
+
 #: getting_started.py:20
 msgid "Getting Started with Your Joulescope"
 msgstr "Erste Schritte mit Ihrem Joulescope"
 
 #: getting_started.py:22
 msgid "Safety"
 msgstr "Sicherheit"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.4/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: el\n"
 "Language-Team: el <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -480,14 +480,17 @@
 "Διαμορφώστε τον τύπο φίλτρου εύρους ρεύματος (IRF), ο οποίος καθορίζει τον "
 "μηχανισμό φιλτραρίσματος που εφαρμόζεται στις αλλαγές εύρους ρεύματος. Δεν "
 "συνιστούμε την αλλαγή αυτών των ρυθμίσεων για κανονική λειτουργία."
 
 msgid "Configure the direction of the JS220's trigger BNC connection."
 msgstr "Διαμορφώστε την κατεύθυνση της σύνδεσης BNC σκανδαλισμού του JS220."
 
+msgid "Configure the filename"
+msgstr "Διαμόρφωση του ονόματος αρχείου"
+
 msgid "Configure trigger options and then press to start."
 msgstr ""
 "Διαμορφώστε τις επιλογές σκανδαλισμού και, στη συνέχεια, πατήστε για να "
 "ξεκινήσετε."
 
 msgid "Connect"
 msgstr "Σύνδεση"
@@ -1746,25 +1749,37 @@
 "system behavior from the small current range switching artifacts."
 msgstr ""
 "Το εύρος ρεύματος είναι χρήσιμο για την κατανόηση του τρόπου με τον οποίο το "
 "Joulescope σας αυτορυθμίζεται για να μετρήσει το σήμα ρεύματος. Μπορεί "
 "επίσης να είναι χρήσιμο για τον διαχωρισμό της συμπεριφοράς του συστήματος-"
 "στόχου από τα τεχνουργήματα μεταγωγής σε μικρό εύρος ρεύματος."
 
+msgid "The current timestamp."
+msgstr "Η τρέχουσα χρονοσήμανση."
+
 msgid "The default path for loading and saving files."
 msgstr "Η προεπιλεγμένη διαδρομή για τη φόρτωση και την αποθήκευση αρχείων."
 
 msgid "The default path method"
 msgstr "Η προεπιλεγμένη μέθοδος διαδρομής"
 
 msgid "The default unique_id for the default statistics streaming source."
 msgstr ""
 "Το προεπιλεγμένο unique_id για την προεπιλεγμένη πηγή ροής στατιστικών "
 "στοιχείων."
 
+msgid "The device identifier."
+msgstr "Το αναγνωριστικό της συσκευής."
+
+msgid "The device model."
+msgstr "Το μοντέλο της συσκευής."
+
+msgid "The device serial number."
+msgstr "Ο σειριακός αριθμός της συσκευής."
+
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "Η συσκευή που θα χρησιμοποιηθεί για τη συνθήκη εκκίνησης και τη συνθήκη "
 "διακοπής."
 
 msgid "The disk is full"
 msgstr "Ο δίσκος είναι γεμάτος"
@@ -1783,14 +1798,17 @@
 msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "Η σταθερά χρόνου εκθετικής αποσύνθεσης. Η ασφάλεια διαχέει το 63,2 % της "
 "συσσωρευμένης ενέργειας σε αυτή τη διάρκεια."
 
+msgid "The filename supports the following replacements."
+msgstr "Το όνομα αρχείου υποστηρίζει τις ακόλουθες αντικαταστάσεις."
+
 msgid "The filename with optional replacements."
 msgstr "Το όνομα αρχείου με προαιρετικές αντικαταστάσεις."
 
 msgid "The fixed default path for loading and saving files."
 msgstr ""
 "Η σταθερή προεπιλεγμένη διαδρομή για τη φόρτωση και την αποθήκευση αρχείων."
 
@@ -1835,17 +1853,23 @@
 "The number of samples before the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Ο αριθμός των δειγμάτων πριν από το παράθυρο εύρους ρεύματος που "
 "χρησιμοποιείται για τον προσδιορισμό του μέσου όρου. Αυτή η τιμή αγνοείται "
 "για όλους τους άλλους τύπους IRF."
 
+msgid "The number of times the filename has been used."
+msgstr "Ο αριθμός των φορών που έχει χρησιμοποιηθεί το όνομα αρχείου."
+
 msgid "The precision to display in digits."
 msgstr "Η ακρίβεια για την εμφάνιση σε ψηφία."
 
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "Το αναγνωριστικό διεργασίας για αυτή την κλήση του Joulescope UI."
+
 msgid "The pyjoulescope_driver log level."
 msgstr "Το επίπεδο καταγραφής του pyjoulescope_driver."
 
 msgid "The quantities to display by default."
 msgstr "Οι ποσότητες που θα εμφανίζονται από προεπιλογή."
 
 msgid ""
@@ -1919,14 +1943,17 @@
 
 msgid "The unique_id for the default signal streaming source."
 msgstr "Το unique_id για την προεπιλεγμένη πηγή ροής σήματος."
 
 msgid "The units to display."
 msgstr "Οι μονάδες που θα εμφανίζονται."
 
+msgid "The user-configurable device name."
+msgstr "Το όνομα της συσκευής που μπορεί να διαμορφωθεί από τον χρήστη."
+
 msgid ""
 "The values displayed by this widget come from a single source device. Select "
 "the source device here."
 msgstr ""
 "Οι τιμές που εμφανίζονται από αυτό το widget προέρχονται από μία μόνο "
 "συσκευή προέλευσης. Επιλέξτε τη συσκευή προέλευσης εδώ."
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.4/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: el <LL@li.org>\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -414,14 +414,50 @@
 msgid ""
 "Exporting data to a JLS file. You can open this file later to display the "
 "exported data."
 msgstr ""
 "Εξαγωγή δεδομένων σε αρχείο JLS. Μπορείτε να ανοίξετε αυτό το αρχείο "
 "αργότερα για να εμφανίσετε τα εξαγόμενα δεδομένα."
 
+#: filename_formatter.py:19
+msgid "The device identifier."
+msgstr "Το αναγνωριστικό της συσκευής."
+
+#: filename_formatter.py:20
+msgid "The user-configurable device name."
+msgstr "Το όνομα της συσκευής που μπορεί να διαμορφωθεί από τον χρήστη."
+
+#: filename_formatter.py:21
+msgid "The device model."
+msgstr "Το μοντέλο της συσκευής."
+
+#: filename_formatter.py:22
+msgid "The device serial number."
+msgstr "Ο σειριακός αριθμός της συσκευής."
+
+#: filename_formatter.py:23
+msgid "Configure the filename"
+msgstr "Διαμόρφωση του ονόματος αρχείου"
+
+#: filename_formatter.py:24
+msgid "The filename supports the following replacements."
+msgstr "Το όνομα αρχείου υποστηρίζει τις ακόλουθες αντικαταστάσεις."
+
+#: filename_formatter.py:25
+msgid "The current timestamp."
+msgstr "Η τρέχουσα χρονοσήμανση."
+
+#: filename_formatter.py:26
+msgid "The number of times the filename has been used."
+msgstr "Ο αριθμός των φορών που έχει χρησιμοποιηθεί το όνομα αρχείου."
+
+#: filename_formatter.py:27
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "Το αναγνωριστικό διεργασίας για αυτή την κλήση του Joulescope UI."
+
 #: getting_started.py:20
 msgid "Getting Started with Your Joulescope"
 msgstr "Ξεκινώντας με το Joulescope"
 
 #: getting_started.py:22
 msgid "Safety"
 msgstr "Ασφάλεια"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.4/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -480,14 +480,17 @@
 "Configure el tipo de filtro de rango de corriente (IRF) que determina el "
 "mecanismo de filtrado aplicado en los cambios de rango de corriente. No "
 "recomendamos cambiar estos ajustes para un funcionamiento normal."
 
 msgid "Configure the direction of the JS220's trigger BNC connection."
 msgstr "Configure la dirección de la conexión BNC de disparo del JS220."
 
+msgid "Configure the filename"
+msgstr "Configurar el nombre de archivo"
+
 msgid "Configure trigger options and then press to start."
 msgstr "Configure las opciones de disparo y pulse para iniciar."
 
 msgid "Connect"
 msgstr "Conectar"
 
 msgid ""
@@ -1737,25 +1740,37 @@
 "system behavior from the small current range switching artifacts."
 msgstr ""
 "El rango de corriente es útil para comprender cómo se autoajusta el "
 "Joulescope para medir la señal de corriente. También puede ser útil para "
 "separar el comportamiento del sistema objetivo de los artefactos de "
 "conmutación del pequeño rango de corriente."
 
+msgid "The current timestamp."
+msgstr "La marca de tiempo actual."
+
 msgid "The default path for loading and saving files."
 msgstr "La ruta predeterminada para cargar y guardar archivos."
 
 msgid "The default path method"
 msgstr "El método de ruta por defecto"
 
 msgid "The default unique_id for the default statistics streaming source."
 msgstr ""
 "El unique_id por defecto para la fuente de transmisión de estadísticas por "
 "defecto."
 
+msgid "The device identifier."
+msgstr "El identificador del dispositivo."
+
+msgid "The device model."
+msgstr "El modelo de dispositivo."
+
+msgid "The device serial number."
+msgstr "El número de serie del dispositivo."
+
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "El dispositivo a utilizar para la condición de arranque y la condición de "
 "parada."
 
 msgid "The disk is full"
 msgstr "El disco está lleno"
@@ -1774,14 +1789,17 @@
 msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "La constante de tiempo de decaimiento exponencial. El fusible disipa el "
 "63,2% de la energía acumulada en esta duración."
 
+msgid "The filename supports the following replacements."
+msgstr "El nombre de archivo admite las siguientes sustituciones."
+
 msgid "The filename with optional replacements."
 msgstr "El nombre del archivo con sustituciones opcionales."
 
 msgid "The fixed default path for loading and saving files."
 msgstr "La ruta fija por defecto para cargar y guardar archivos."
 
 msgid "The flyout width in pixels."
@@ -1823,17 +1841,25 @@
 "The number of samples before the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "El número de muestras antes de la ventana de rango de corriente utilizada "
 "para determinar la media. Este valor se ignora para todos los demás tipos de "
 "IRF."
 
+msgid "The number of times the filename has been used."
+msgstr "Número de veces que se ha utilizado el nombre del archivo."
+
 msgid "The precision to display in digits."
 msgstr "La precisión a mostrar en dígitos."
 
+msgid "The process ID for this Joulescope UI invocation."
+msgstr ""
+"El ID del proceso para esta invocación a la interfaz de usuario de "
+"Joulescope."
+
 msgid "The pyjoulescope_driver log level."
 msgstr "El nivel de registro de pyjoulescope_driver."
 
 msgid "The quantities to display by default."
 msgstr "Las cantidades a mostrar por defecto."
 
 msgid ""
@@ -1905,14 +1931,17 @@
 
 msgid "The unique_id for the default signal streaming source."
 msgstr "El unique_id para la fuente de corriente de señal por defecto."
 
 msgid "The units to display."
 msgstr "Las unidades a mostrar."
 
+msgid "The user-configurable device name."
+msgstr "Nombre del dispositivo configurable por el usuario."
+
 msgid ""
 "The values displayed by this widget come from a single source device. Select "
 "the source device here."
 msgstr ""
 "Los valores mostrados por este widget proceden de un único dispositivo "
 "fuente. Seleccione aquí el dispositivo de origen."
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.4/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: es <LL@li.org>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -413,14 +413,52 @@
 msgid ""
 "Exporting data to a JLS file. You can open this file later to display the "
 "exported data."
 msgstr ""
 "Exportación de datos a un archivo JLS. Puede abrir este archivo más tarde "
 "para visualizar los datos exportados."
 
+#: filename_formatter.py:19
+msgid "The device identifier."
+msgstr "El identificador del dispositivo."
+
+#: filename_formatter.py:20
+msgid "The user-configurable device name."
+msgstr "Nombre del dispositivo configurable por el usuario."
+
+#: filename_formatter.py:21
+msgid "The device model."
+msgstr "El modelo de dispositivo."
+
+#: filename_formatter.py:22
+msgid "The device serial number."
+msgstr "El número de serie del dispositivo."
+
+#: filename_formatter.py:23
+msgid "Configure the filename"
+msgstr "Configurar el nombre de archivo"
+
+#: filename_formatter.py:24
+msgid "The filename supports the following replacements."
+msgstr "El nombre de archivo admite las siguientes sustituciones."
+
+#: filename_formatter.py:25
+msgid "The current timestamp."
+msgstr "La marca de tiempo actual."
+
+#: filename_formatter.py:26
+msgid "The number of times the filename has been used."
+msgstr "Número de veces que se ha utilizado el nombre del archivo."
+
+#: filename_formatter.py:27
+msgid "The process ID for this Joulescope UI invocation."
+msgstr ""
+"El ID del proceso para esta invocación a la interfaz de usuario de "
+"Joulescope."
+
 #: getting_started.py:20
 msgid "Getting Started with Your Joulescope"
 msgstr "Primeros pasos con su Joulescope"
 
 #: getting_started.py:22
 msgid "Safety"
 msgstr "Seguridad"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.4/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -478,14 +478,17 @@
 "Configure le type de filtre de plage de courant (IRF) qui détermine le "
 "mécanisme de filtrage appliqué aux changements de plage de courant. Il n'est "
 "pas recommandé de modifier ces paramètres pour un fonctionnement normal."
 
 msgid "Configure the direction of the JS220's trigger BNC connection."
 msgstr "Configurer la direction de la connexion BNC de déclenchement du JS220."
 
+msgid "Configure the filename"
+msgstr "Configurer le nom du fichier"
+
 msgid "Configure trigger options and then press to start."
 msgstr "Configurer les options de déclenchement et appuyer sur pour démarrer."
 
 msgid "Connect"
 msgstr "Connecter"
 
 msgid ""
@@ -1743,27 +1746,39 @@
 "system behavior from the small current range switching artifacts."
 msgstr ""
 "La gamme de courant est utile pour comprendre comment votre Joulescope "
 "s'autorégule pour mesurer votre signal de courant. Elle peut également être "
 "utile pour séparer le comportement du système cible des artefacts de "
 "commutation de la petite plage de courant."
 
+msgid "The current timestamp."
+msgstr "L'horodatage actuel."
+
 msgid "The default path for loading and saving files."
 msgstr ""
 "Chemin d'accès par défaut pour le chargement et l'enregistrement des "
 "fichiers."
 
 msgid "The default path method"
 msgstr "La méthode du chemin par défaut"
 
 msgid "The default unique_id for the default statistics streaming source."
 msgstr ""
 "L'identifiant unique par défaut de la source de flux de statistiques par "
 "défaut."
 
+msgid "The device identifier."
+msgstr "L'identifiant de l'appareil."
+
+msgid "The device model."
+msgstr "Le modèle de l'appareil."
+
+msgid "The device serial number."
+msgstr "Le numéro de série de l'appareil."
+
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "Le dispositif à utiliser pour la condition de démarrage et la condition "
 "d'arrêt."
 
 msgid "The disk is full"
 msgstr "Le disque est plein"
@@ -1782,14 +1797,17 @@
 msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "La constante de temps de la décroissance exponentielle. Le fusible dissipe "
 "63,2 % de l'énergie accumulée pendant cette durée."
 
+msgid "The filename supports the following replacements."
+msgstr "Le nom de fichier prend en charge les remplacements suivants."
+
 msgid "The filename with optional replacements."
 msgstr "Le nom du fichier avec des remplacements optionnels."
 
 msgid "The fixed default path for loading and saving files."
 msgstr ""
 "Le chemin fixe par défaut pour le chargement et l'enregistrement des "
 "fichiers."
@@ -1833,17 +1851,25 @@
 "The number of samples before the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Le nombre d'échantillons avant la fenêtre de la plage de courant utilisée "
 "pour déterminer la moyenne. Cette valeur est ignorée pour tous les autres "
 "types d'IRF."
 
+msgid "The number of times the filename has been used."
+msgstr "Nombre de fois où le nom du fichier a été utilisé."
+
 msgid "The precision to display in digits."
 msgstr "La précision à afficher en chiffres."
 
+msgid "The process ID for this Joulescope UI invocation."
+msgstr ""
+"L'ID du processus pour cette invocation de l'interface utilisateur "
+"Joulescope."
+
 msgid "The pyjoulescope_driver log level."
 msgstr "Le niveau de journalisation de pyjoulescope_driver."
 
 msgid "The quantities to display by default."
 msgstr "Les quantités à afficher par défaut."
 
 msgid ""
@@ -1915,14 +1941,17 @@
 
 msgid "The unique_id for the default signal streaming source."
 msgstr "L'identifiant unique de la source de flux de signaux par défaut."
 
 msgid "The units to display."
 msgstr "Les unités à afficher."
 
+msgid "The user-configurable device name."
+msgstr "Le nom de l'appareil configurable par l'utilisateur."
+
 msgid ""
 "The values displayed by this widget come from a single source device. Select "
 "the source device here."
 msgstr ""
 "Les valeurs affichées par ce widget proviennent d'un seul appareil source. "
 "Sélectionnez l'appareil source ici."
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.4/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: fr <LL@li.org>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -416,14 +416,52 @@
 msgid ""
 "Exporting data to a JLS file. You can open this file later to display the "
 "exported data."
 msgstr ""
 "Exportation des données vers un fichier JLS. Vous pouvez ouvrir ce fichier "
 "ultérieurement pour afficher les données exportées."
 
+#: filename_formatter.py:19
+msgid "The device identifier."
+msgstr "L'identifiant de l'appareil."
+
+#: filename_formatter.py:20
+msgid "The user-configurable device name."
+msgstr "Le nom de l'appareil configurable par l'utilisateur."
+
+#: filename_formatter.py:21
+msgid "The device model."
+msgstr "Le modèle de l'appareil."
+
+#: filename_formatter.py:22
+msgid "The device serial number."
+msgstr "Le numéro de série de l'appareil."
+
+#: filename_formatter.py:23
+msgid "Configure the filename"
+msgstr "Configurer le nom du fichier"
+
+#: filename_formatter.py:24
+msgid "The filename supports the following replacements."
+msgstr "Le nom de fichier prend en charge les remplacements suivants."
+
+#: filename_formatter.py:25
+msgid "The current timestamp."
+msgstr "L'horodatage actuel."
+
+#: filename_formatter.py:26
+msgid "The number of times the filename has been used."
+msgstr "Nombre de fois où le nom du fichier a été utilisé."
+
+#: filename_formatter.py:27
+msgid "The process ID for this Joulescope UI invocation."
+msgstr ""
+"L'ID du processus pour cette invocation de l'interface utilisateur "
+"Joulescope."
+
 #: getting_started.py:20
 msgid "Getting Started with Your Joulescope"
 msgstr "Démarrer avec votre Joulescope"
 
 #: getting_started.py:22
 msgid "Safety"
 msgstr "Sécurité"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.4/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -459,14 +459,17 @@
 "電流レンジフィルター（IRF）タイプを設定し、電流レンジの変化に適用されるフィル"
 "タリング機構を決定します。通常の動作では、これらの設定を変更することはお勧め"
 "しません。"
 
 msgid "Configure the direction of the JS220's trigger BNC connection."
 msgstr "JS220のトリガーBNC接続の方向を設定します。"
 
+msgid "Configure the filename"
+msgstr "ファイル名の設定"
+
 msgid "Configure trigger options and then press to start."
 msgstr "トリガーオプションを設定し、 を押して開始します。"
 
 msgid "Connect"
 msgstr "接続"
 
 msgid ""
@@ -1683,23 +1686,35 @@
 "to measure your current signal. It can also be helpful in separating target "
 "system behavior from the small current range switching artifacts."
 msgstr ""
 "電流レンジは、ジュールスコープが電流信号を測定するためにどのようにオートレン"
 "ジするかを理解するのに役立ちます。また、ターゲット・システムの動作を小電流レ"
 "ンジのスイッチング・アーティファクトから分離する際にも役立ちます。"
 
+msgid "The current timestamp."
+msgstr "現在のタイムスタンプ。"
+
 msgid "The default path for loading and saving files."
 msgstr "ファイルの読み込みと保存のデフォルトパス。"
 
 msgid "The default path method"
 msgstr "デフォルトのパスメソッド"
 
 msgid "The default unique_id for the default statistics streaming source."
 msgstr "デフォルトの統計ストリーミング・ソースのデフォルトのユニークID。"
 
+msgid "The device identifier."
+msgstr "デバイス識別子。"
+
+msgid "The device model."
+msgstr "デバイス・モデル。"
+
+msgid "The device serial number."
+msgstr "デバイスのシリアル番号。"
+
 msgid "The device to use for the start condition and stop condition."
 msgstr "開始条件および停止条件に使用するデバイス。"
 
 msgid "The disk is full"
 msgstr "ディスクがいっぱいです"
 
 msgid ""
@@ -1714,14 +1729,17 @@
 
 msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "指数関数的減衰時定数。ヒューズはこの時間内に蓄積エネルギーの63.2%を消散する。"
 
+msgid "The filename supports the following replacements."
+msgstr "ファイル名は以下の置換に対応しています。"
+
 msgid "The filename with optional replacements."
 msgstr "ファイル名。"
 
 msgid "The fixed default path for loading and saving files."
 msgstr "ファイルをロードおよび保存するための固定デフォルトパス。"
 
 msgid "The flyout width in pixels."
@@ -1761,17 +1779,23 @@
 msgid ""
 "The number of samples before the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "平均を決定するために使用される電流範囲ウィンドウの前のサンプル数。他のIRFタイ"
 "プではこの値は無視されます。"
 
+msgid "The number of times the filename has been used."
+msgstr "ファイル名の使用回数。"
+
 msgid "The precision to display in digits."
 msgstr "桁で表示する精度。"
 
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "このJoulescope UI呼び出しのプロセスID。"
+
 msgid "The pyjoulescope_driver log level."
 msgstr "pyjoulescope_driverのログレベル。"
 
 msgid "The quantities to display by default."
 msgstr "デフォルトで表示する量。"
 
 msgid ""
@@ -1838,14 +1862,17 @@
 
 msgid "The unique_id for the default signal streaming source."
 msgstr "デフォルトの信号ストリーミング・ソースのユニークID。"
 
 msgid "The units to display."
 msgstr "表示する単位。"
 
+msgid "The user-configurable device name."
+msgstr "ユーザー設定可能なデバイス名。"
+
 msgid ""
 "The values displayed by this widget come from a single source device. Select "
 "the source device here."
 msgstr ""
 "このウィジェットで表示される値は、単一のソース・デバイスからのものです。ここ"
 "でソース・デバイスを選択してください。"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.4/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ja <LL@li.org>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -368,14 +368,50 @@
 
 #: exporter.py:170
 msgid ""
 "Exporting data to a JLS file. You can open this file later to display the "
 "exported data."
 msgstr "データを JLS ファイルにエクスポートします。このファイルを後で開いて、エクスポートしたデータを表示することができます。"
 
+#: filename_formatter.py:19
+msgid "The device identifier."
+msgstr "デバイス識別子。"
+
+#: filename_formatter.py:20
+msgid "The user-configurable device name."
+msgstr "ユーザー設定可能なデバイス名。"
+
+#: filename_formatter.py:21
+msgid "The device model."
+msgstr "デバイス・モデル。"
+
+#: filename_formatter.py:22
+msgid "The device serial number."
+msgstr "デバイスのシリアル番号。"
+
+#: filename_formatter.py:23
+msgid "Configure the filename"
+msgstr "ファイル名の設定"
+
+#: filename_formatter.py:24
+msgid "The filename supports the following replacements."
+msgstr "ファイル名は以下の置換に対応しています。"
+
+#: filename_formatter.py:25
+msgid "The current timestamp."
+msgstr "現在のタイムスタンプ。"
+
+#: filename_formatter.py:26
+msgid "The number of times the filename has been used."
+msgstr "ファイル名の使用回数。"
+
+#: filename_formatter.py:27
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "このJoulescope UI呼び出しのプロセスID。"
+
 #: getting_started.py:20
 msgid "Getting Started with Your Joulescope"
 msgstr "Joulescopeを使い始めるには"
 
 #: getting_started.py:22
 msgid "Safety"
 msgstr "安全性"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/joulescope_ui.pot` & `joulescope_ui-1.1.4/joulescope_ui/locale/joulescope_ui.pot`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Copyright (C) 2024 Jetperch LLC
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PROJECT 1.1.3\n"
+"Project-Id-Version: PROJECT 1.1.4\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.14.0\n"
@@ -360,14 +360,50 @@
 
 #: exporter.py:170
 msgid ""
 "Exporting data to a JLS file. You can open this file later to display the "
 "exported data."
 msgstr ""
 
+#: filename_formatter.py:19
+msgid "The device identifier."
+msgstr ""
+
+#: filename_formatter.py:20
+msgid "The user-configurable device name."
+msgstr ""
+
+#: filename_formatter.py:21
+msgid "The device model."
+msgstr ""
+
+#: filename_formatter.py:22
+msgid "The device serial number."
+msgstr ""
+
+#: filename_formatter.py:23
+msgid "Configure the filename"
+msgstr ""
+
+#: filename_formatter.py:24
+msgid "The filename supports the following replacements."
+msgstr ""
+
+#: filename_formatter.py:25
+msgid "The current timestamp."
+msgstr ""
+
+#: filename_formatter.py:26
+msgid "The number of times the filename has been used."
+msgstr ""
+
+#: filename_formatter.py:27
+msgid "The process ID for this Joulescope UI invocation."
+msgstr ""
+
 #: getting_started.py:20
 msgid "Getting Started with Your Joulescope"
 msgstr ""
 
 #: getting_started.py:22
 msgid "Safety"
 msgstr ""
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.4/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ko\n"
 "Language-Team: ko <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -449,14 +449,17 @@
 msgstr ""
 "전류 범위 변경에 적용되는 필터링 메커니즘을 결정하는 전류 범위 필터(IRF) 유형"
 "을 구성합니다. 정상 작동을 위해 이 설정을 변경하지 않는 것이 좋습니다."
 
 msgid "Configure the direction of the JS220's trigger BNC connection."
 msgstr "JS220의 트리거 BNC 연결 방향을 구성합니다."
 
+msgid "Configure the filename"
+msgstr "파일 이름 구성"
+
 msgid "Configure trigger options and then press to start."
 msgstr "트리거 옵션을 구성한 다음 을 눌러 시작하세요."
 
 msgid "Connect"
 msgstr "연결"
 
 msgid ""
@@ -1662,23 +1665,35 @@
 "to measure your current signal. It can also be helpful in separating target "
 "system behavior from the small current range switching artifacts."
 msgstr ""
 "전류 범위는 줄스코프가 전류 신호를 측정하기 위해 자동 범위를 설정하는 방법을 "
 "이해하는 데 유용합니다. 또한 작은 전류 범위 스위칭 아티팩트에서 대상 시스템 "
 "동작을 분리하는 데 도움이 될 수 있습니다."
 
+msgid "The current timestamp."
+msgstr "현재 타임스탬프."
+
 msgid "The default path for loading and saving files."
 msgstr "파일 로드 및 저장을 위한 기본 경로입니다."
 
 msgid "The default path method"
 msgstr "기본 경로 방법"
 
 msgid "The default unique_id for the default statistics streaming source."
 msgstr "기본 통계 스트리밍 소스의 기본 고유 ID입니다."
 
+msgid "The device identifier."
+msgstr "디바이스 식별자."
+
+msgid "The device model."
+msgstr "디바이스 모델."
+
+msgid "The device serial number."
+msgstr "디바이스 일련 번호."
+
 msgid "The device to use for the start condition and stop condition."
 msgstr "시작 조건 및 중지 조건에 사용할 장치입니다."
 
 msgid "The disk is full"
 msgstr "디스크가 꽉 찼습니다."
 
 msgid ""
@@ -1693,14 +1708,17 @@
 
 msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "지수 감쇠 시간 상수. 퓨즈는 이 기간 동안 누적된 에너지의 63.2%를 소산합니다."
 
+msgid "The filename supports the following replacements."
+msgstr "파일 이름은 다음과 같은 대체를 지원합니다."
+
 msgid "The filename with optional replacements."
 msgstr "선택적으로 대체할 수 있는 파일 이름입니다."
 
 msgid "The fixed default path for loading and saving files."
 msgstr "파일 로드 및 저장을 위한 고정된 기본 경로입니다."
 
 msgid "The flyout width in pixels."
@@ -1740,17 +1758,23 @@
 msgid ""
 "The number of samples before the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "평균을 결정하는 데 사용되는 전류 범위 창 이전의 샘플 수입니다. 다른 모든 IRF "
 "유형에서는 이 값이 무시됩니다."
 
+msgid "The number of times the filename has been used."
+msgstr "파일 이름이 사용된 횟수입니다."
+
 msgid "The precision to display in digits."
 msgstr "숫자로 표시되는 정밀도."
 
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "이 줄스코프 UI 호출의 프로세스 ID입니다."
+
 msgid "The pyjoulescope_driver log level."
 msgstr "pyjoulescope_driver 로그 레벨."
 
 msgid "The quantities to display by default."
 msgstr "기본적으로 표시되는 수량입니다."
 
 msgid ""
@@ -1817,14 +1841,17 @@
 
 msgid "The unique_id for the default signal streaming source."
 msgstr "기본 신호 스트리밍 소스의 고유 ID입니다."
 
 msgid "The units to display."
 msgstr "표시할 단위."
 
+msgid "The user-configurable device name."
+msgstr "사용자가 구성할 수 있는 장치 이름입니다."
+
 msgid ""
 "The values displayed by this widget come from a single source device. Select "
 "the source device here."
 msgstr ""
 "이 위젯에 표시되는 값은 단일 소스 장치에서 가져온 것입니다. 여기에서 소스 장"
 "치를 선택하세요."
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.4/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ko <LL@li.org>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -371,14 +371,50 @@
 
 #: exporter.py:170
 msgid ""
 "Exporting data to a JLS file. You can open this file later to display the "
 "exported data."
 msgstr "데이터를 JLS 파일로 내보내기. 나중에 이 파일을 열어 내보낸 데이터를 표시할 수 있습니다."
 
+#: filename_formatter.py:19
+msgid "The device identifier."
+msgstr "디바이스 식별자."
+
+#: filename_formatter.py:20
+msgid "The user-configurable device name."
+msgstr "사용자가 구성할 수 있는 장치 이름입니다."
+
+#: filename_formatter.py:21
+msgid "The device model."
+msgstr "디바이스 모델."
+
+#: filename_formatter.py:22
+msgid "The device serial number."
+msgstr "디바이스 일련 번호."
+
+#: filename_formatter.py:23
+msgid "Configure the filename"
+msgstr "파일 이름 구성"
+
+#: filename_formatter.py:24
+msgid "The filename supports the following replacements."
+msgstr "파일 이름은 다음과 같은 대체를 지원합니다."
+
+#: filename_formatter.py:25
+msgid "The current timestamp."
+msgstr "현재 타임스탬프."
+
+#: filename_formatter.py:26
+msgid "The number of times the filename has been used."
+msgstr "파일 이름이 사용된 횟수입니다."
+
+#: filename_formatter.py:27
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "이 줄스코프 UI 호출의 프로세스 ID입니다."
+
 #: getting_started.py:20
 msgid "Getting Started with Your Joulescope"
 msgstr "줄스코프 시작하기"
 
 #: getting_started.py:22
 msgid "Safety"
 msgstr "안전"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.4/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh\n"
 "Language-Team: zh <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -423,14 +423,17 @@
 msgstr ""
 "配置电流范围滤波器 (IRF) 类型，该类型决定应用于电流范围变化的滤波机制。我们不"
 "建议在正常操作时更改这些设置。"
 
 msgid "Configure the direction of the JS220's trigger BNC connection."
 msgstr "配置 JS220 触发器 BNC 连接的方向。"
 
+msgid "Configure the filename"
+msgstr "配置文件名"
+
 msgid "Configure trigger options and then press to start."
 msgstr "配置触发选项，然后按 开始。"
 
 msgid "Connect"
 msgstr "连接"
 
 msgid ""
@@ -1601,23 +1604,35 @@
 "The current range is useful for understanding how your Joulescope autoranges "
 "to measure your current signal. It can also be helpful in separating target "
 "system behavior from the small current range switching artifacts."
 msgstr ""
 "电流量程有助于了解 Joulescope 如何自动量程以测量电流信号。它还有助于将目标系"
 "统行为与小电流范围开关伪影区分开来。"
 
+msgid "The current timestamp."
+msgstr "当前时间戳。"
+
 msgid "The default path for loading and saving files."
 msgstr "加载和保存文件的默认路径。"
 
 msgid "The default path method"
 msgstr "默认路径方法"
 
 msgid "The default unique_id for the default statistics streaming source."
 msgstr "默认统计数据流源的默认唯一 ID。"
 
+msgid "The device identifier."
+msgstr "设备标识符。"
+
+msgid "The device model."
+msgstr "设备型号。"
+
+msgid "The device serial number."
+msgstr "设备序列号。"
+
 msgid "The device to use for the start condition and stop condition."
 msgstr "用于启动条件和停止条件的设备。"
 
 msgid "The disk is full"
 msgstr "磁盘已满"
 
 msgid ""
@@ -1630,14 +1645,17 @@
 "是，统计数据将继续累积（如果选择）。"
 
 msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr "指数衰减时间常数。保险丝在此时间内耗散了 63.2% 的累积能量。"
 
+msgid "The filename supports the following replacements."
+msgstr "文件名支持以下替换。"
+
 msgid "The filename with optional replacements."
 msgstr "可选替换的文件名。"
 
 msgid "The fixed default path for loading and saving files."
 msgstr "加载和保存文件的固定默认路径。"
 
 msgid "The flyout width in pixels."
@@ -1677,17 +1695,23 @@
 msgid ""
 "The number of samples before the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "用于确定平均值的电流范围窗口之前的采样次数。对于所有其他 IRF 类型，该值将被忽"
 "略。"
 
+msgid "The number of times the filename has been used."
+msgstr "文件名被使用的次数。"
+
 msgid "The precision to display in digits."
 msgstr "以位数显示的精度。"
 
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "此 Joulescope UI 调用的进程 ID。"
+
 msgid "The pyjoulescope_driver log level."
 msgstr "pyjoulescope_driver 的日志级别。"
 
 msgid "The quantities to display by default."
 msgstr "默认显示的量。"
 
 msgid ""
@@ -1752,14 +1776,17 @@
 
 msgid "The unique_id for the default signal streaming source."
 msgstr "默认信号流源的唯一 ID。"
 
 msgid "The units to display."
 msgstr "要显示的单位。"
 
+msgid "The user-configurable device name."
+msgstr "用户可配置的设备名称。"
+
 msgid ""
 "The values displayed by this widget come from a single source device. Select "
 "the source device here."
 msgstr "此 widget 显示的值来自单个源器件。在此选择源设备。"
 
 msgid "The voltage between any sensor port must never exceed ±15V."
 msgstr "任何传感器端口之间的电压不得超过 ±15V。"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.4/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-05 09:09-0400\n"
+"POT-Creation-Date: 2024-04-18 14:15-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: zh <LL@li.org>\n"
 "Language: zh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -363,14 +363,50 @@
 
 #: exporter.py:170
 msgid ""
 "Exporting data to a JLS file. You can open this file later to display the "
 "exported data."
 msgstr "将数据导出到 JLS 文件。稍后可以打开该文件以显示导出的数据。"
 
+#: filename_formatter.py:19
+msgid "The device identifier."
+msgstr "设备标识符。"
+
+#: filename_formatter.py:20
+msgid "The user-configurable device name."
+msgstr "用户可配置的设备名称。"
+
+#: filename_formatter.py:21
+msgid "The device model."
+msgstr "设备型号。"
+
+#: filename_formatter.py:22
+msgid "The device serial number."
+msgstr "设备序列号。"
+
+#: filename_formatter.py:23
+msgid "Configure the filename"
+msgstr "配置文件名"
+
+#: filename_formatter.py:24
+msgid "The filename supports the following replacements."
+msgstr "文件名支持以下替换。"
+
+#: filename_formatter.py:25
+msgid "The current timestamp."
+msgstr "当前时间戳。"
+
+#: filename_formatter.py:26
+msgid "The number of times the filename has been used."
+msgstr "文件名被使用的次数。"
+
+#: filename_formatter.py:27
+msgid "The process ID for this Joulescope UI invocation."
+msgstr "此 Joulescope UI 调用的进程 ID。"
+
 #: getting_started.py:20
 msgid "Getting Started with Your Joulescope"
 msgstr "开始使用 Joulescope"
 
 #: getting_started.py:22
 msgid "Safety"
 msgstr "安全性"
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/logging_util.py` & `joulescope_ui-1.1.4/joulescope_ui/logging_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/main.py` & `joulescope_ui-1.1.4/joulescope_ui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 # https://stackoverflow.com/questions/11874767/real-time-plotting-in-while-loop-with-matplotlib
 # https://wiki.qt.io/Gallery_of_Qt_CSS_Based_Styles
 
 from joulescope_ui import pubsub_singleton, N_, get_topic_name, get_instance, \
     tooltip_format, CAPABILITIES, Metadata, __version__
-from joulescope_ui.locale import gettext_locale_get
+from joulescope_ui.locale import locale_get
 from joulescope_ui.pubsub import UNDO_TOPIC, REDO_TOPIC, is_pubsub_registered
 from joulescope_ui.pubsub_aggregator import PubsubAggregator
 from joulescope_ui.shortcuts import Shortcuts
 from joulescope_ui.widgets import *   # registers all built-in widgets
 from joulescope_ui import logging_util
 from joulescope_ui.plugins import PluginManager
 from joulescope_ui.reporter import create as reporter_create
@@ -269,15 +269,15 @@
         self._mem_utilization.setToolTip(_MEMORY_UTILIZATION_TOOLTIP)
         self._status_bar.addPermanentWidget(self._mem_utilization)
 
         pubsub_singleton.register(self, 'ui', parent=None)
         self._pubsub_process_count_last = pubsub_singleton.process_count
 
         locale_prev = self.locale_str
-        locale_now = gettext_locale_get()
+        locale_now = locale_get()
         if locale_now != locale_prev:
             self._log.info('locale changed %s -> %s, update names', locale_prev, locale_now)
             _name_set_to_default(pubsub_singleton)
             self.locale_str = locale_now
 
         self._style_manager = StyleManager()
         self.pubsub.register(self._style_manager, 'style')
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/mem_leak_debugger.py` & `joulescope_ui-1.1.4/joulescope_ui/mem_leak_debugger.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/metadata.py` & `joulescope_ui-1.1.4/joulescope_ui/metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/paths.py` & `joulescope_ui-1.1.4/joulescope_ui/paths.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/plugins/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/plugins/manager.py` & `joulescope_ui-1.1.4/joulescope_ui/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/plugins/selector.py` & `joulescope_ui-1.1.4/joulescope_ui/plugins/selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/plugins/test/plugins/p1/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/plugins/test/plugins/p1/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/plugins/test/test_manager.py` & `joulescope_ui-1.1.4/joulescope_ui/plugins/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/process_monitor.py` & `joulescope_ui-1.1.4/joulescope_ui/process_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/profile.py` & `joulescope_ui-1.1.4/joulescope_ui/profile.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/pubsub.py` & `joulescope_ui-1.1.4/joulescope_ui/pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/pubsub_aggregator.py` & `joulescope_ui-1.1.4/joulescope_ui/pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/pubsub_callable.py` & `joulescope_ui-1.1.4/joulescope_ui/pubsub_callable.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/pubsub_proxy.py` & `joulescope_ui-1.1.4/joulescope_ui/pubsub_proxy.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/range_tool.py` & `joulescope_ui-1.1.4/joulescope_ui/range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/range_tools/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/range_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/range_tools/cdf.py` & `joulescope_ui-1.1.4/joulescope_ui/range_tools/cdf.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/range_tools/frequency.py` & `joulescope_ui-1.1.4/joulescope_ui/range_tools/frequency.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/range_tools/histogram.py` & `joulescope_ui-1.1.4/joulescope_ui/range_tools/histogram.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/range_tools/max_window.py` & `joulescope_ui-1.1.4/joulescope_ui/range_tools/max_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/range_tools/plugin_helpers.py` & `joulescope_ui-1.1.4/joulescope_ui/range_tools/plugin_helpers.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/range_tools/usb_inrush.py` & `joulescope_ui-1.1.4/joulescope_ui/range_tools/usb_inrush.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/reporter.py` & `joulescope_ui-1.1.4/joulescope_ui/reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/dmg_background.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/dmg_background.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/dmg_background.svg` & `joulescope_ui-1.1.4/joulescope_ui/resources/dmg_background.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/dmg_background@2x.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/dmg_background@2x.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.ico` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_128x128.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_128x128@2.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_128x128@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_16x16@2.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_16x16@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_256x256.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_256x256@2.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_256x256@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_32x32.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_32x32@2.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_32x32@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_512x512.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_512x512@2.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_512x512@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_64x64.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icon.iconset/icon_64x64@2.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/icon.iconset/icon_64x64@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/icons.svg` & `joulescope_ui-1.1.4/joulescope_ui/resources/icons.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/logo-large.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/logo-large.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/logo-small.png` & `joulescope_ui-1.1.4/joulescope_ui/resources/logo-small.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources/zoom.svg` & `joulescope_ui-1.1.4/joulescope_ui/resources/zoom.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources.py` & `joulescope_ui-1.1.4/joulescope_ui/resources.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/resources.rcc` & `joulescope_ui-1.1.4/joulescope_ui/resources.rcc`

 * *Files 4% similar despite different names*

```diff
@@ -1416,11 +1416,11 @@
 00005870: 5f00 3600 3400 7800 3600 3400 2e00 6900  _.6.4.x.6.4...i.
 00005880: 6300 6f00 0e03 14ce 8700 6c00 6f00 6700  c.o.......l.o.g.
 00005890: 6f00 2d00 6c00 6100 7200 6700 6500 2e00  o.-.l.a.r.g.e...
 000058a0: 7000 6e00 6700 0e0f ebc7 e700 6c00 6f00  p.n.g.......l.o.
 000058b0: 6700 6f00 2d00 7300 6d00 6100 6c00 6c00  g.o.-.s.m.a.l.l.
 000058c0: 2e00 7000 6e00 6700 0000 0000 0200 0000  ..p.n.g.........
 000058d0: 0300 0000 0100 0000 0000 0000 0000 0000  ................
-000058e0: 2200 0000 0000 0100 0001 9900 0001 8eaf  "...............
-000058f0: 8a11 3000 0000 0000 0400 0000 0100 0000  ..0.............
-00005900: 0000 0001 8eaf 8a11 3000 0000 4400 0000  ........0...D...
-00005910: 0000 0100 0043 f800 0001 8eaf 8a11 30    .....C........0
+000058e0: 2200 0000 0000 0100 0001 9900 0001 8ef2  "...............
+000058f0: 927e eb00 0000 0000 0400 0000 0100 0000  .~..............
+00005900: 0000 0001 8ef2 927e eb00 0000 4400 0000  .......~....D...
+00005910: 0000 0100 0043 f800 0001 8ef2 927e eb    .....C.......~.
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui/safe_mode.py` & `joulescope_ui-1.1.4/joulescope_ui/safe_mode.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/sanitize.py` & `joulescope_ui-1.1.4/joulescope_ui/sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/shift_key.py` & `joulescope_ui-1.1.4/joulescope_ui/shift_key.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/shortcuts.py` & `joulescope_ui-1.1.4/joulescope_ui/shortcuts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/software_update.py` & `joulescope_ui-1.1.4/joulescope_ui/software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/source_selector.py` & `joulescope_ui-1.1.4/joulescope_ui/source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/README.md` & `joulescope_ui-1.1.4/joulescope_ui/styles/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/color_editor.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/color_editor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/color_file.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/color_picker.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/color_picker.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/color_scheme.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/color_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.4/joulescope_ui/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/color_scheme_light.txt` & `joulescope_ui-1.1.4/joulescope_ui/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/font_scheme.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/font_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/fonts.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/fonts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/js1/detach.svg` & `joulescope_ui-1.1.4/joulescope_ui/styles/js1/detach.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/js1/index.json` & `joulescope_ui-1.1.4/joulescope_ui/styles/js1/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/js1/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/styles/js1/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/js1/vmovetoolbar.svg` & `joulescope_ui-1.1.4/joulescope_ui/styles/js1/vmovetoolbar.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/js1/vsepartoolbars.svg` & `joulescope_ui-1.1.4/joulescope_ui/styles/js1/vsepartoolbars.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/manager.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/parameter_file.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/system/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/styles/system/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/system/zoom_all.svg` & `joulescope_ui-1.1.4/joulescope_ui/styles/system/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/test/test_color_file.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/test/test_color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/test/test_manager.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/styles/test/test_parameter_file.py` & `joulescope_ui-1.1.4/joulescope_ui/styles/test/test_parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/anno1.anno.jls` & `joulescope_ui-1.1.4/joulescope_ui/test/anno1.anno.jls`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_annotation_load.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_annotation_load.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_capabilities.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_disk_monitor.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_metadata.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_pubsub.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_pubsub_aggregator.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_pubsub_registry.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_pubsub_registry.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_range_tool.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_reporter.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_sanitize.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_software_update.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_source_selector.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_time_map.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_tooltip.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_units.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/test/test_versioned_file.py` & `joulescope_ui-1.1.4/joulescope_ui/test/test_versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/time_map.py` & `joulescope_ui-1.1.4/joulescope_ui/time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/tokens.py` & `joulescope_ui-1.1.4/joulescope_ui/tokens.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/tooltip.py` & `joulescope_ui-1.1.4/joulescope_ui/tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/ui_util.py` & `joulescope_ui-1.1.4/joulescope_ui/ui_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/units.py` & `joulescope_ui-1.1.4/joulescope_ui/units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/urls.py` & `joulescope_ui-1.1.4/joulescope_ui/urls.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/versioned_file.py` & `joulescope_ui-1.1.4/joulescope_ui/versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/view.py` & `joulescope_ui-1.1.4/joulescope_ui/view.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widget_tools.py` & `joulescope_ui-1.1.4/joulescope_ui/widget_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/accumulator_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/accumulator_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/accumulator/styles/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/widgets/accumulator/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/clock/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/clock/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/clock/clock_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/clock/clock_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/developer/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/developer/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/developer/log_view_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/developer/log_view_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/developer/profile_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/developer/profile_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/developer/publish_spy_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/developer/publish_spy_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/developer/pubsub_explorer_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/developer/pubsub_explorer_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/current_limits.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/current_limits.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/device_control_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/device_control_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/device_info_dialog.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/device_info_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/device_update_dialog.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/device_update_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/fuse.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/js220_ctrl_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/js220_ctrl_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/device_open.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/device_open.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/fuse_normal.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/index.json` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/info.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/info.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/device_control/styles/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/widgets/device_control/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/double_slider.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/double_slider.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/draggable_list_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/draggable_list_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/example/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/example/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/example/example_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/example/example_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/flyout_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/flyout_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/flyout/styles/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/widgets/flyout/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/hamburger/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/hamburger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/hamburger/hamburger_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/hamburger/hamburger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/help/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/help/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/help/help_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/help/help_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/jls_info/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/jls_info/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/jls_info/jls_info_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/jls_info/jls_info_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/js220_cal/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/js220_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/js220_cal/current_offset.png` & `joulescope_ui-1.1.4/joulescope_ui/widgets/js220_cal/current_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/js220_cal/js220_cal_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/js220_cal/js220_cal_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/js220_cal/voltage_offset.png` & `joulescope_ui-1.1.4/joulescope_ui/widgets/js220_cal/voltage_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/memory/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/memory/memory_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/memory/memory_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/memory/styles/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/widgets/memory/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/notes/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/notes/notes_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/notes/notes_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/progress_bar/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/progress_bar/progress_bar_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/progress_bar/progress_bar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/record_status_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/record_status_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/styles/index.json` & `joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/record_status/styles/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/widgets/record_status/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/report_issue/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/report_issue/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/report_issue/report_issue_dialog.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/report_issue/report_issue_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/settings/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/settings/settings_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/settings/settings_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/settings/unique_strings_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/settings/unique_strings_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/sidebar_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/sidebar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt` & `joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/index.json` & `joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/sidebar/styles/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/widgets/sidebar/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/signal_record/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/signal_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/signal_record/disk_full_dialog.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/signal_record/disk_full_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/signal_record/signal_record.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/signal_record/signal_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/signal_record/signal_record_config_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/signal_record/signal_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/statistics_record/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/statistics_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/statistics_record/statistics_record.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/statistics_record/statistics_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/switch.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/condition_detector.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/condition_detector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/continuous.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/continuous.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/index.json` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/searching.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/searching.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/styles/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/test/test_const.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/test/test_const.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/test/test_duration.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/test/test_duration.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/test/test_edge.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/test/test_edge.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/trigger/trigger_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/trigger/trigger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/value/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/value/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/value/value_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/value/value_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/styles/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/view_manager/view_manager_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/view_manager/view_manager_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/__init__.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/annotations.md` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/annotations.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/axis_ticks.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/interval_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/interval_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/line_segments.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/line_segments.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/quantities.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/index.json` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/style.qss` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/styles/zoom_all.svg` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/styles/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/test/test_axis_ticks.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/test/test_axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/test/test_quantities.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/test/test_quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/text_annotation.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/text_annotation.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/waveform_control.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/waveform_control.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/waveform_source_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/waveform_source_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/waveform_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/waveform_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/widgets/waveform/y_range_widget.py` & `joulescope_ui-1.1.4/joulescope_ui/widgets/waveform/y_range_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui/zip_inspector.py` & `joulescope_ui-1.1.4/joulescope_ui/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/joulescope_ui.egg-info/PKG-INFO` & `joulescope_ui-1.1.4/joulescope_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.3
+Version: 1.1.4
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.1.3/joulescope_ui.egg-info/SOURCES.txt` & `joulescope_ui-1.1.4/joulescope_ui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,16 @@
 joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
 joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
 joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
 joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
 joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
 joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
 joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
+joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo
+joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po
 joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
 joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
 joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
 joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
 joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
 joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
 joulescope_ui/plugins/__init__.py
```

### Comparing `joulescope_ui-1.1.3/pyproject.toml` & `joulescope_ui-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.3/setup.py` & `joulescope_ui-1.1.4/setup.py`

 * *Files identical despite different names*

