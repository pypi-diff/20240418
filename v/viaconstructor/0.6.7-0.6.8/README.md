# Comparing `tmp/viaconstructor-0.6.7.tar.gz` & `tmp/viaconstructor-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viaconstructor-0.6.7.tar", last modified: Thu Apr  4 15:56:18 2024, max compression
+gzip compressed data, was "viaconstructor-0.6.8.tar", last modified: Thu Apr 18 20:17:37 2024, max compression
```

## Comparing `viaconstructor-0.6.7.tar` & `viaconstructor-0.6.8.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.350472 viaconstructor-0.6.7/
--rwxr-xr-x   0 root         (0) root         (0)    35147 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      194 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3885 2024-04-04 15:56:18.350472 viaconstructor-0.6.7/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3624 2023-04-08 23:55:39.000000 viaconstructor-0.6.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.333472 viaconstructor-0.6.7/bin/
--rwxr-xr-x   0 root         (0) root         (0)       36 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/bin/dxfpreview
--rwxr-xr-x   0 root         (0) root         (0)       38 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/bin/gcodepreview
--rwxr-xr-x   0 root         (0) root         (0)       42 2022-08-17 21:04:13.000000 viaconstructor-0.6.7/bin/viaconstructor
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.333472 viaconstructor-0.6.7/dxfpreview/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/dxfpreview/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/dxfpreview/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     4087 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/dxfpreview/dxfpreview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.334472 viaconstructor-0.6.7/gcodepreview/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/gcodepreview/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       96 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/gcodepreview/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     3564 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/gcodepreview/gcodepreview.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 15:56:18.350472 viaconstructor-0.6.7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1232 2024-04-04 15:55:51.000000 viaconstructor-0.6.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.336472 viaconstructor-0.6.7/viaconstructor/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/viaconstructor/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.7/viaconstructor/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)    50043 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/calc.py
--rwxr-xr-x   0 root         (0) root         (0)    24211 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/draw2d.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-03-26 08:12:36.000000 viaconstructor-0.6.7/viaconstructor/dxfcolors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.331472 viaconstructor-0.6.7/viaconstructor/ext/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.337472 viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/
--rw-r--r--   0 root         (0) root         (0)    91220 2022-08-22 17:54:34.000000 viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/HersheyFonts.py
--rw-r--r--   0 root         (0) root         (0)       63 2022-08-22 17:54:34.000000 viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      101 2022-08-22 17:54:34.000000 viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.337472 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/
--rw-r--r--   0 root         (0) root         (0)       39 2022-08-22 18:47:24.000000 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8813 2023-03-23 17:27:32.000000 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/cavaliercontours.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.338472 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/
--rwxr-xr-x   0 root         (0) root         (0)   872112 2023-03-23 17:27:32.000000 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
--rwxr-xr-x   0 root         (0) root         (0)  1383488 2023-03-23 17:27:32.000000 viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.340472 viaconstructor-0.6.7/viaconstructor/ext/meshcut/
--rw-r--r--   0 root         (0) root         (0)    12866 2022-08-22 19:00:32.000000 viaconstructor-0.6.7/viaconstructor/ext/meshcut/meshcut.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.341472 viaconstructor-0.6.7/viaconstructor/ext/stl/
--rw-r--r--   0 root         (0) root         (0)      321 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/__about__.py
--rw-r--r--   0 root         (0) root         (0)      375 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22397 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/base.py
--rw-r--r--   0 root         (0) root         (0)     3277 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/main.py
--rw-r--r--   0 root         (0) root         (0)       55 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/mesh.py
--rw-r--r--   0 root         (0) root         (0)    15642 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/stl.py
--rw-r--r--   0 root         (0) root         (0)      541 2022-08-22 19:01:54.000000 viaconstructor-0.6.7/viaconstructor/ext/stl/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.343472 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/
--rw-r--r--   0 root         (0) root         (0)     1097 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14309 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/bezier.py
--rw-r--r--   0 root         (0) root         (0)    18496 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/document.py
--rw-r--r--   0 root         (0) root         (0)     2026 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/misctools.py
--rw-r--r--   0 root         (0) root         (0)     3939 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/parser.py
--rw-r--r--   0 root         (0) root         (0)   133535 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/path.py
--rw-r--r--   0 root         (0) root         (0)    18991 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/paths2svg.py
--rw-r--r--   0 root         (0) root         (0)     2473 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/polytools.py
--rw-r--r--   0 root         (0) root         (0)     7642 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/smoothing.py
--rw-r--r--   0 root         (0) root         (0)     7089 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/svg_io_sax.py
--rw-r--r--   0 root         (0) root         (0)    11331 2022-08-22 18:57:05.000000 viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/svg_to_paths.py
--rwxr-xr-x   0 root         (0) root         (0)    51945 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/gldraw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.347472 viaconstructor-0.6.7/viaconstructor/icons/
--rw-r--r--   0 root         (0) root         (0)     1577 2023-03-30 20:02:43.000000 viaconstructor-0.6.7/viaconstructor/icons/camotics.png
--rw-r--r--   0 root         (0) root         (0)     2046 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/delete.png
--rwxr-xr-x   0 root         (0) root         (0)     2633 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/exit.png
--rw-r--r--   0 root         (0) root         (0)     1606 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/flip-x.png
--rw-r--r--   0 root         (0) root         (0)     1348 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/flip-y.png
--rw-r--r--   0 root         (0) root         (0)     2413 2023-04-04 16:17:31.000000 viaconstructor-0.6.7/viaconstructor/icons/fonts.png
--rw-r--r--   0 root         (0) root         (0)     3221 2024-02-01 14:48:19.000000 viaconstructor-0.6.7/viaconstructor/icons/gears.png
--rw-r--r--   0 root         (0) root         (0)    20293 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/load-setup-gcode.png
--rw-r--r--   0 root         (0) root         (0)    16209 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/load-setup.png
--rw-r--r--   0 root         (0) root         (0)     2237 2022-09-23 15:31:33.000000 viaconstructor-0.6.7/viaconstructor/icons/load-tooltable.png
--rw-r--r--   0 root         (0) root         (0)      523 2023-02-25 16:12:56.000000 viaconstructor-0.6.7/viaconstructor/icons/nesting.png
--rw-r--r--   0 root         (0) root         (0)     2237 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/open.png
--rw-r--r--   0 root         (0) root         (0)    11071 2023-03-30 20:02:43.000000 viaconstructor-0.6.7/viaconstructor/icons/openscad.png
--rw-r--r--   0 root         (0) root         (0)      912 2022-09-22 16:28:41.000000 viaconstructor-0.6.7/viaconstructor/icons/pause.png
--rw-r--r--   0 root         (0) root         (0)     1473 2022-09-20 19:38:29.000000 viaconstructor-0.6.7/viaconstructor/icons/play.png
--rw-r--r--   0 root         (0) root         (0)     2120 2023-03-27 15:46:36.000000 viaconstructor-0.6.7/viaconstructor/icons/redraw.png
--rw-r--r--   0 root         (0) root         (0)     1843 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/repair.png
--rw-r--r--   0 root         (0) root         (0)     2967 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/rotate.png
--rwxr-xr-x   0 root         (0) root         (0)    12941 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save-gcode.png
--rw-r--r--   0 root         (0) root         (0)    16787 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save-setup-as.png
--rwxr-xr-x   0 root         (0) root         (0)     3096 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save-setup.png
--rw-r--r--   0 root         (0) root         (0)     3484 2022-09-23 15:31:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save-tooltable.png
--rw-r--r--   0 root         (0) root         (0)     3196 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/save.png
--rw-r--r--   0 root         (0) root         (0)     1254 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/scale.png
--rw-r--r--   0 root         (0) root         (0)      291 2022-09-21 16:00:41.000000 viaconstructor-0.6.7/viaconstructor/icons/select.png
--rw-r--r--   0 root         (0) root         (0)     1759 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/start.png
--rw-r--r--   0 root         (0) root         (0)      729 2022-09-22 16:28:41.000000 viaconstructor-0.6.7/viaconstructor/icons/stop.png
--rw-r--r--   0 root         (0) root         (0)     1500 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/tab-selector.png
--rw-r--r--   0 root         (0) root         (0)     2496 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/view-2d.png
--rw-r--r--   0 root         (0) root         (0)     4342 2022-08-24 16:12:33.000000 viaconstructor-0.6.7/viaconstructor/icons/view-reset.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.348472 viaconstructor-0.6.7/viaconstructor/input_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6762 2023-04-12 16:19:12.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/brdread.py
--rwxr-xr-x   0 root         (0) root         (0)    25832 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/dxfread.py
--rw-r--r--   0 root         (0) root         (0)     6483 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/hpglread.py
--rw-r--r--   0 root         (0) root         (0)     2441 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/imgread.py
--rw-r--r--   0 root         (0) root         (0)     7853 2023-04-07 10:50:08.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/stlread.py
--rwxr-xr-x   0 root         (0) root         (0)    10584 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/svgread.py
--rw-r--r--   0 root         (0) root         (0)     9336 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins/ttfread.py
--rw-r--r--   0 root         (0) root         (0)     2936 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/input_plugins_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.331472 viaconstructor-0.6.7/viaconstructor/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.332472 viaconstructor-0.6.7/viaconstructor/locales/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.348472 viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     5083 2023-04-10 16:36:40.000000 viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 root         (0) root         (0)     8633 2024-02-01 14:48:19.000000 viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/base.po
--rwxr-xr-x   0 root         (0) root         (0)    39246 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/machine_cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.349472 viaconstructor-0.6.7/viaconstructor/output_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.7/viaconstructor/output_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10849 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/output_plugins/gcode_grbl.py
--rw-r--r--   0 root         (0) root         (0)    11015 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/output_plugins/gcode_linuxcnc.py
--rw-r--r--   0 root         (0) root         (0)     7376 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/output_plugins/hpgl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.349472 viaconstructor-0.6.7/viaconstructor/preview_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.7/viaconstructor/preview_plugins/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10745 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/preview_plugins/gcode.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/preview_plugins/hpgl.py
--rwxr-xr-x   0 root         (0) root         (0)    22882 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/setupdefaults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.350472 viaconstructor-0.6.7/viaconstructor/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-01 14:48:19.000000 viaconstructor-0.6.7/viaconstructor/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8970 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/tools/font.py
--rw-r--r--   0 root         (0) root         (0)     8709 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/tools/gear.py
--rw-r--r--   0 root         (0) root         (0)     2560 2023-02-25 16:12:56.000000 viaconstructor-0.6.7/viaconstructor/vc_types.py
--rwxr-xr-x   0 root         (0) root         (0)   122156 2024-04-04 15:54:13.000000 viaconstructor-0.6.7/viaconstructor/viaconstructor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:18.336472 viaconstructor-0.6.7/viaconstructor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3885 2024-04-04 15:56:17.000000 viaconstructor-0.6.7/viaconstructor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3690 2024-04-04 15:56:18.000000 viaconstructor-0.6.7/viaconstructor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 15:56:17.000000 viaconstructor-0.6.7/viaconstructor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2024-04-04 15:56:17.000000 viaconstructor-0.6.7/viaconstructor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-04 15:56:17.000000 viaconstructor-0.6.7/viaconstructor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.873057 viaconstructor-0.6.8/
+-rwxr-xr-x   0 root         (0) root         (0)    35147 2022-07-11 18:18:57.000000 viaconstructor-0.6.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      194 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3885 2024-04-18 20:17:37.873057 viaconstructor-0.6.8/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3624 2023-04-08 23:55:39.000000 viaconstructor-0.6.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.855057 viaconstructor-0.6.8/bin/
+-rwxr-xr-x   0 root         (0) root         (0)       36 2022-07-11 18:18:57.000000 viaconstructor-0.6.8/bin/dxfpreview
+-rwxr-xr-x   0 root         (0) root         (0)       38 2022-07-11 18:18:57.000000 viaconstructor-0.6.8/bin/gcodepreview
+-rwxr-xr-x   0 root         (0) root         (0)       42 2022-08-17 21:04:13.000000 viaconstructor-0.6.8/bin/viaconstructor
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.855057 viaconstructor-0.6.8/dxfpreview/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.8/dxfpreview/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.8/dxfpreview/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4087 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/dxfpreview/dxfpreview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.856057 viaconstructor-0.6.8/gcodepreview/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.8/gcodepreview/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       96 2022-07-11 18:18:57.000000 viaconstructor-0.6.8/gcodepreview/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3564 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/gcodepreview/gcodepreview.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 20:17:37.873057 viaconstructor-0.6.8/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1232 2024-04-18 20:17:09.000000 viaconstructor-0.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.858057 viaconstructor-0.6.8/viaconstructor/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-07-11 18:18:57.000000 viaconstructor-0.6.8/viaconstructor/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       92 2022-07-11 18:18:57.000000 viaconstructor-0.6.8/viaconstructor/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)    50043 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/calc.py
+-rwxr-xr-x   0 root         (0) root         (0)    24211 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/draw2d.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2023-03-26 08:12:36.000000 viaconstructor-0.6.8/viaconstructor/dxfcolors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.853057 viaconstructor-0.6.8/viaconstructor/ext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.859057 viaconstructor-0.6.8/viaconstructor/ext/HersheyFonts/
+-rw-r--r--   0 root         (0) root         (0)    91220 2022-08-22 17:54:34.000000 viaconstructor-0.6.8/viaconstructor/ext/HersheyFonts/HersheyFonts.py
+-rw-r--r--   0 root         (0) root         (0)       63 2022-08-22 17:54:34.000000 viaconstructor-0.6.8/viaconstructor/ext/HersheyFonts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      101 2022-08-22 17:54:34.000000 viaconstructor-0.6.8/viaconstructor/ext/HersheyFonts/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.859057 viaconstructor-0.6.8/viaconstructor/ext/cavaliercontours/
+-rw-r--r--   0 root         (0) root         (0)       39 2022-08-22 18:47:24.000000 viaconstructor-0.6.8/viaconstructor/ext/cavaliercontours/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8813 2023-03-23 17:27:32.000000 viaconstructor-0.6.8/viaconstructor/ext/cavaliercontours/cavaliercontours.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.861057 viaconstructor-0.6.8/viaconstructor/ext/cavaliercontours/lib/
+-rwxr-xr-x   0 root         (0) root         (0)   872112 2023-03-23 17:27:32.000000 viaconstructor-0.6.8/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
+-rwxr-xr-x   0 root         (0) root         (0)  1383488 2023-03-23 17:27:32.000000 viaconstructor-0.6.8/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.862057 viaconstructor-0.6.8/viaconstructor/ext/meshcut/
+-rw-r--r--   0 root         (0) root         (0)    12866 2022-08-22 19:00:32.000000 viaconstructor-0.6.8/viaconstructor/ext/meshcut/meshcut.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.863057 viaconstructor-0.6.8/viaconstructor/ext/stl/
+-rw-r--r--   0 root         (0) root         (0)      321 2022-08-22 19:01:54.000000 viaconstructor-0.6.8/viaconstructor/ext/stl/__about__.py
+-rw-r--r--   0 root         (0) root         (0)      375 2022-08-22 19:01:54.000000 viaconstructor-0.6.8/viaconstructor/ext/stl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22397 2022-08-22 19:01:54.000000 viaconstructor-0.6.8/viaconstructor/ext/stl/base.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2022-08-22 19:01:54.000000 viaconstructor-0.6.8/viaconstructor/ext/stl/main.py
+-rw-r--r--   0 root         (0) root         (0)       55 2022-08-22 19:01:54.000000 viaconstructor-0.6.8/viaconstructor/ext/stl/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    15642 2022-08-22 19:01:54.000000 viaconstructor-0.6.8/viaconstructor/ext/stl/stl.py
+-rw-r--r--   0 root         (0) root         (0)      541 2022-08-22 19:01:54.000000 viaconstructor-0.6.8/viaconstructor/ext/stl/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.865057 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/
+-rw-r--r--   0 root         (0) root         (0)     1097 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14309 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/bezier.py
+-rw-r--r--   0 root         (0) root         (0)    18496 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/document.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/misctools.py
+-rw-r--r--   0 root         (0) root         (0)     3939 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/parser.py
+-rw-r--r--   0 root         (0) root         (0)   133535 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/path.py
+-rw-r--r--   0 root         (0) root         (0)    18991 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/paths2svg.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/polytools.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/smoothing.py
+-rw-r--r--   0 root         (0) root         (0)     7089 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/svg_io_sax.py
+-rw-r--r--   0 root         (0) root         (0)    11331 2022-08-22 18:57:05.000000 viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/svg_to_paths.py
+-rwxr-xr-x   0 root         (0) root         (0)    51945 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/gldraw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.870057 viaconstructor-0.6.8/viaconstructor/icons/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-03-30 20:02:43.000000 viaconstructor-0.6.8/viaconstructor/icons/camotics.png
+-rw-r--r--   0 root         (0) root         (0)     2046 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/delete.png
+-rwxr-xr-x   0 root         (0) root         (0)     2633 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/exit.png
+-rw-r--r--   0 root         (0) root         (0)     1606 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/flip-x.png
+-rw-r--r--   0 root         (0) root         (0)     1348 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/flip-y.png
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-04-04 16:17:31.000000 viaconstructor-0.6.8/viaconstructor/icons/fonts.png
+-rw-r--r--   0 root         (0) root         (0)     3221 2024-02-01 14:48:19.000000 viaconstructor-0.6.8/viaconstructor/icons/gears.png
+-rw-r--r--   0 root         (0) root         (0)    20293 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/load-setup-gcode.png
+-rw-r--r--   0 root         (0) root         (0)    16209 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/load-setup.png
+-rw-r--r--   0 root         (0) root         (0)     2237 2022-09-23 15:31:33.000000 viaconstructor-0.6.8/viaconstructor/icons/load-tooltable.png
+-rw-r--r--   0 root         (0) root         (0)      523 2023-02-25 16:12:56.000000 viaconstructor-0.6.8/viaconstructor/icons/nesting.png
+-rw-r--r--   0 root         (0) root         (0)     2237 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/open.png
+-rw-r--r--   0 root         (0) root         (0)    11071 2023-03-30 20:02:43.000000 viaconstructor-0.6.8/viaconstructor/icons/openscad.png
+-rw-r--r--   0 root         (0) root         (0)      912 2022-09-22 16:28:41.000000 viaconstructor-0.6.8/viaconstructor/icons/pause.png
+-rw-r--r--   0 root         (0) root         (0)     1473 2022-09-20 19:38:29.000000 viaconstructor-0.6.8/viaconstructor/icons/play.png
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-03-27 15:46:36.000000 viaconstructor-0.6.8/viaconstructor/icons/redraw.png
+-rw-r--r--   0 root         (0) root         (0)     1843 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/repair.png
+-rw-r--r--   0 root         (0) root         (0)     2967 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/rotate.png
+-rwxr-xr-x   0 root         (0) root         (0)    12941 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/save-gcode.png
+-rw-r--r--   0 root         (0) root         (0)    16787 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/save-setup-as.png
+-rwxr-xr-x   0 root         (0) root         (0)     3096 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/save-setup.png
+-rw-r--r--   0 root         (0) root         (0)     3484 2022-09-23 15:31:33.000000 viaconstructor-0.6.8/viaconstructor/icons/save-tooltable.png
+-rw-r--r--   0 root         (0) root         (0)     3196 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/save.png
+-rw-r--r--   0 root         (0) root         (0)     1254 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/scale.png
+-rw-r--r--   0 root         (0) root         (0)      291 2022-09-21 16:00:41.000000 viaconstructor-0.6.8/viaconstructor/icons/select.png
+-rw-r--r--   0 root         (0) root         (0)     1759 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/start.png
+-rw-r--r--   0 root         (0) root         (0)      729 2022-09-22 16:28:41.000000 viaconstructor-0.6.8/viaconstructor/icons/stop.png
+-rw-r--r--   0 root         (0) root         (0)     1500 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/tab-selector.png
+-rw-r--r--   0 root         (0) root         (0)     2496 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/view-2d.png
+-rw-r--r--   0 root         (0) root         (0)     4342 2022-08-24 16:12:33.000000 viaconstructor-0.6.8/viaconstructor/icons/view-reset.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.871057 viaconstructor-0.6.8/viaconstructor/input_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.8/viaconstructor/input_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6762 2023-04-12 16:19:12.000000 viaconstructor-0.6.8/viaconstructor/input_plugins/brdread.py
+-rwxr-xr-x   0 root         (0) root         (0)    25832 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/input_plugins/dxfread.py
+-rw-r--r--   0 root         (0) root         (0)     6483 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/input_plugins/hpglread.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/input_plugins/imgread.py
+-rw-r--r--   0 root         (0) root         (0)     7853 2023-04-07 10:50:08.000000 viaconstructor-0.6.8/viaconstructor/input_plugins/stlread.py
+-rwxr-xr-x   0 root         (0) root         (0)    10584 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/input_plugins/svgread.py
+-rw-r--r--   0 root         (0) root         (0)     9336 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/input_plugins/ttfread.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/input_plugins_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.853057 viaconstructor-0.6.8/viaconstructor/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.854057 viaconstructor-0.6.8/viaconstructor/locales/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.871057 viaconstructor-0.6.8/viaconstructor/locales/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-04-10 16:36:40.000000 viaconstructor-0.6.8/viaconstructor/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 root         (0) root         (0)     8633 2024-02-01 14:48:19.000000 viaconstructor-0.6.8/viaconstructor/locales/de/LC_MESSAGES/base.po
+-rwxr-xr-x   0 root         (0) root         (0)    39246 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/machine_cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.872057 viaconstructor-0.6.8/viaconstructor/output_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.8/viaconstructor/output_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10849 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/output_plugins/gcode_grbl.py
+-rw-r--r--   0 root         (0) root         (0)    11015 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/output_plugins/gcode_linuxcnc.py
+-rw-r--r--   0 root         (0) root         (0)     7376 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/output_plugins/hpgl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.873057 viaconstructor-0.6.8/viaconstructor/preview_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-03 19:17:04.000000 viaconstructor-0.6.8/viaconstructor/preview_plugins/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10745 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/preview_plugins/gcode.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/preview_plugins/hpgl.py
+-rwxr-xr-x   0 root         (0) root         (0)    22882 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/setupdefaults.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.873057 viaconstructor-0.6.8/viaconstructor/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-01 14:48:19.000000 viaconstructor-0.6.8/viaconstructor/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8970 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/tools/font.py
+-rw-r--r--   0 root         (0) root         (0)     8709 2024-04-04 15:54:13.000000 viaconstructor-0.6.8/viaconstructor/tools/gear.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-02-25 16:12:56.000000 viaconstructor-0.6.8/viaconstructor/vc_types.py
+-rwxr-xr-x   0 root         (0) root         (0)   122586 2024-04-18 20:16:58.000000 viaconstructor-0.6.8/viaconstructor/viaconstructor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:17:37.859057 viaconstructor-0.6.8/viaconstructor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3885 2024-04-18 20:17:37.000000 viaconstructor-0.6.8/viaconstructor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-04-18 20:17:37.000000 viaconstructor-0.6.8/viaconstructor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 20:17:37.000000 viaconstructor-0.6.8/viaconstructor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2024-04-18 20:17:37.000000 viaconstructor-0.6.8/viaconstructor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-18 20:17:37.000000 viaconstructor-0.6.8/viaconstructor.egg-info/top_level.txt
```

### Comparing `viaconstructor-0.6.7/LICENSE` & `viaconstructor-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/PKG-INFO` & `viaconstructor-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.7
+Version: 0.6.8
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
```

### Comparing `viaconstructor-0.6.7/README.md` & `viaconstructor-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/dxfpreview/dxfpreview.py` & `viaconstructor-0.6.8/dxfpreview/dxfpreview.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/gcodepreview/gcodepreview.py` & `viaconstructor-0.6.8/gcodepreview/gcodepreview.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/setup.py` & `viaconstructor-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 from setuptools import setup
 
 
 setup(
     name='viaconstructor',
-    version='0.6.7',
+    version='0.6.8',
     author='Oliver Dippel',
     author_email='o.dippel@gmx.de',
     packages=['viaconstructor', 'viaconstructor.ext.cavaliercontours', 'viaconstructor.ext.HersheyFonts', 'viaconstructor.ext.meshcut', 'viaconstructor.ext.stl', 'viaconstructor.ext.svgpathtools', 'viaconstructor.input_plugins', 'viaconstructor.output_plugins', 'viaconstructor.preview_plugins', 'viaconstructor.tools', 'gcodepreview', 'dxfpreview'],
     package_data={'viaconstructor.ext.cavaliercontours': ['lib/libCavalierContours.x86_64-linux.so'], 'viaconstructor/ext/nest2D': ['nest2D.cpython-39-x86_64-linux-gnu.so']},
     scripts=['bin/viaconstructor','bin/gcodepreview','bin/dxfpreview'],
     url='https://github.com/multigcs/viaconstructor',
     license='LICENSE',
```

### Comparing `viaconstructor-0.6.7/viaconstructor/calc.py` & `viaconstructor-0.6.8/viaconstructor/calc.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/draw2d.py` & `viaconstructor-0.6.8/viaconstructor/draw2d.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/dxfcolors.py` & `viaconstructor-0.6.8/viaconstructor/dxfcolors.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/HersheyFonts/HersheyFonts.py` & `viaconstructor-0.6.8/viaconstructor/ext/HersheyFonts/HersheyFonts.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/cavaliercontours.py` & `viaconstructor-0.6.8/viaconstructor/ext/cavaliercontours/cavaliercontours.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so` & `viaconstructor-0.6.8/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so` & `viaconstructor-0.6.8/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/meshcut/meshcut.py` & `viaconstructor-0.6.8/viaconstructor/ext/meshcut/meshcut.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/stl/base.py` & `viaconstructor-0.6.8/viaconstructor/ext/stl/base.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/stl/main.py` & `viaconstructor-0.6.8/viaconstructor/ext/stl/main.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/stl/stl.py` & `viaconstructor-0.6.8/viaconstructor/ext/stl/stl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/stl/utils.py` & `viaconstructor-0.6.8/viaconstructor/ext/stl/utils.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/__init__.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/__init__.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/bezier.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/bezier.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/document.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/document.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/misctools.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/misctools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/parser.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/parser.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/path.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/path.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/paths2svg.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/paths2svg.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/polytools.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/polytools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/smoothing.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/smoothing.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/svg_io_sax.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/svg_io_sax.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/ext/svgpathtools/svg_to_paths.py` & `viaconstructor-0.6.8/viaconstructor/ext/svgpathtools/svg_to_paths.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/gldraw.py` & `viaconstructor-0.6.8/viaconstructor/gldraw.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/camotics.png` & `viaconstructor-0.6.8/viaconstructor/icons/camotics.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/delete.png` & `viaconstructor-0.6.8/viaconstructor/icons/delete.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/exit.png` & `viaconstructor-0.6.8/viaconstructor/icons/exit.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/flip-x.png` & `viaconstructor-0.6.8/viaconstructor/icons/flip-x.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/flip-y.png` & `viaconstructor-0.6.8/viaconstructor/icons/flip-y.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/fonts.png` & `viaconstructor-0.6.8/viaconstructor/icons/fonts.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/gears.png` & `viaconstructor-0.6.8/viaconstructor/icons/gears.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/load-setup-gcode.png` & `viaconstructor-0.6.8/viaconstructor/icons/load-setup-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/load-setup.png` & `viaconstructor-0.6.8/viaconstructor/icons/load-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/load-tooltable.png` & `viaconstructor-0.6.8/viaconstructor/icons/load-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/nesting.png` & `viaconstructor-0.6.8/viaconstructor/icons/nesting.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/open.png` & `viaconstructor-0.6.8/viaconstructor/icons/open.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/openscad.png` & `viaconstructor-0.6.8/viaconstructor/icons/openscad.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/pause.png` & `viaconstructor-0.6.8/viaconstructor/icons/pause.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/play.png` & `viaconstructor-0.6.8/viaconstructor/icons/play.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/redraw.png` & `viaconstructor-0.6.8/viaconstructor/icons/redraw.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/repair.png` & `viaconstructor-0.6.8/viaconstructor/icons/repair.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/rotate.png` & `viaconstructor-0.6.8/viaconstructor/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/save-gcode.png` & `viaconstructor-0.6.8/viaconstructor/icons/save-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/save-setup-as.png` & `viaconstructor-0.6.8/viaconstructor/icons/save-setup-as.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/save-setup.png` & `viaconstructor-0.6.8/viaconstructor/icons/save-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/save-tooltable.png` & `viaconstructor-0.6.8/viaconstructor/icons/save-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/save.png` & `viaconstructor-0.6.8/viaconstructor/icons/save.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/scale.png` & `viaconstructor-0.6.8/viaconstructor/icons/scale.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/start.png` & `viaconstructor-0.6.8/viaconstructor/icons/start.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/stop.png` & `viaconstructor-0.6.8/viaconstructor/icons/stop.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/tab-selector.png` & `viaconstructor-0.6.8/viaconstructor/icons/tab-selector.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/view-2d.png` & `viaconstructor-0.6.8/viaconstructor/icons/view-2d.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/icons/view-reset.png` & `viaconstructor-0.6.8/viaconstructor/icons/view-reset.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/input_plugins/brdread.py` & `viaconstructor-0.6.8/viaconstructor/input_plugins/brdread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/input_plugins/dxfread.py` & `viaconstructor-0.6.8/viaconstructor/input_plugins/dxfread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/input_plugins/hpglread.py` & `viaconstructor-0.6.8/viaconstructor/input_plugins/hpglread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/input_plugins/imgread.py` & `viaconstructor-0.6.8/viaconstructor/input_plugins/imgread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/input_plugins/stlread.py` & `viaconstructor-0.6.8/viaconstructor/input_plugins/stlread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/input_plugins/svgread.py` & `viaconstructor-0.6.8/viaconstructor/input_plugins/svgread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/input_plugins/ttfread.py` & `viaconstructor-0.6.8/viaconstructor/input_plugins/ttfread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/input_plugins_base.py` & `viaconstructor-0.6.8/viaconstructor/input_plugins_base.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/base.mo` & `viaconstructor-0.6.8/viaconstructor/locales/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/locales/de/LC_MESSAGES/base.po` & `viaconstructor-0.6.8/viaconstructor/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/machine_cmd.py` & `viaconstructor-0.6.8/viaconstructor/machine_cmd.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/output_plugins/gcode_grbl.py` & `viaconstructor-0.6.8/viaconstructor/output_plugins/gcode_grbl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/output_plugins/gcode_linuxcnc.py` & `viaconstructor-0.6.8/viaconstructor/output_plugins/gcode_linuxcnc.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/output_plugins/hpgl.py` & `viaconstructor-0.6.8/viaconstructor/output_plugins/hpgl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/preview_plugins/gcode.py` & `viaconstructor-0.6.8/viaconstructor/preview_plugins/gcode.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/preview_plugins/hpgl.py` & `viaconstructor-0.6.8/viaconstructor/preview_plugins/hpgl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/setupdefaults.py` & `viaconstructor-0.6.8/viaconstructor/setupdefaults.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/tools/font.py` & `viaconstructor-0.6.8/viaconstructor/tools/font.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/tools/gear.py` & `viaconstructor-0.6.8/viaconstructor/tools/gear.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/vc_types.py` & `viaconstructor-0.6.8/viaconstructor/vc_types.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.7/viaconstructor/viaconstructor.py` & `viaconstructor-0.6.8/viaconstructor/viaconstructor.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,18 @@
     QLabel,
     QLineEdit,
     QMainWindow,
     QMenuBar,
     QMessageBox,
     QPlainTextEdit,
     QPushButton,
+    QScrollArea,
     QSizePolicy,
     QSpinBox,
+    QSplitter,
     QStatusBar,
     QTableWidget,
     QTableWidgetItem,
     QTabWidget,
     QToolBar,
     QVBoxLayout,
     QWidget,
@@ -1770,108 +1772,113 @@
                 elif entry["type"] == "color":
                     pass
                 else:
                     eprint(f"Unknown setup-type: {entry['type']}")
 
     def create_global_setup(self, tabwidget) -> None:
         for sname in self.project["setup_defaults"]:
+            scrollarea = QScrollArea()
+            scrollarea.setWidgetResizable(True)
             vcontainer = QWidget()
             vlayout = QVBoxLayout(vcontainer)
             vlayout.setContentsMargins(0, 0, 0, 0)
+            scrollarea.setWidget(vcontainer)
 
             titles = {
                 "mill": "M&ill",
                 "tool": "&Tool",
                 "workpiece": "&Workpiece",
                 "pockets": "P&ockets",
                 "tabs": "Ta&bs",
                 "leads": "Lea&ds",
                 "machine": "M&achine",
                 "view": "&View",
             }
-            tabwidget.addTab(vcontainer, titles.get(sname, sname))
+            tabwidget.addTab(scrollarea, titles.get(sname, sname))
             for ename, entry in self.project["setup_defaults"][sname].items():
+                helptext = entry.get("tooltip", f"{sname}/{ename}")
                 container = QWidget()
                 hlayout = QHBoxLayout(container)
                 hlayout.setContentsMargins(10, 0, 10, 0)
                 label = QLabel(entry.get("title", ename))
+                label.setToolTip(helptext)
                 hlayout.addWidget(label)
                 vlayout.addWidget(container)
                 hlayout.addStretch(1)
                 if entry["type"] == "bool":
                     checkbox = QCheckBox(entry.get("title", ename))
                     checkbox.setChecked(self.project["setup"][sname][ename])
-                    checkbox.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    checkbox.setToolTip(helptext)
                     checkbox.stateChanged.connect(self.global_changed)  # type: ignore
                     hlayout.addWidget(checkbox)
                     entry["widget"] = checkbox
                 elif entry["type"] == "select":
                     combobox = QComboBox()
                     for option in entry["options"]:
                         combobox.addItem(option[0])
                     combobox.setCurrentText(self.project["setup"][sname][ename])
-                    combobox.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    combobox.setToolTip(helptext)
                     combobox.currentTextChanged.connect(self.global_changed)  # type: ignore
                     hlayout.addWidget(combobox)
                     entry["widget"] = combobox
                 elif entry["type"] == "color":
                     color = self.project["setup"][sname][ename]
                     rgb = f"{color[0] * 255:1.0f},{color[1] * 255:1.0f},{color[2] * 255:1.0f}"
                     button = QPushButton(rgb)
                     button.setStyleSheet(f"background-color:rgb({rgb})")
-                    button.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    button.setToolTip(helptext)
                     button.clicked.connect(partial(self.color_select, sname, ename))  # type: ignore
                     hlayout.addWidget(button)
                     entry["widget"] = button
                 elif entry["type"] == "float":
                     dspinbox = QDoubleSpinBox()
                     dspinbox.setDecimals(entry.get("decimals", 4))
                     dspinbox.setSingleStep(entry.get("step", 1.0))
                     dspinbox.setMinimum(entry["min"])
                     dspinbox.setMaximum(entry["max"])
                     dspinbox.setValue(self.project["setup"][sname][ename])
-                    dspinbox.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    dspinbox.setToolTip(helptext)
                     dspinbox.valueChanged.connect(self.global_changed)  # type: ignore
                     hlayout.addWidget(dspinbox)
                     entry["widget"] = dspinbox
                 elif entry["type"] == "int":
                     spinbox = QSpinBox()
                     spinbox.setSingleStep(entry.get("step", 1))
                     spinbox.setMinimum(entry["min"])
                     spinbox.setMaximum(entry["max"])
                     spinbox.setValue(self.project["setup"][sname][ename])
-                    spinbox.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    spinbox.setToolTip(helptext)
                     spinbox.valueChanged.connect(self.global_changed)  # type: ignore
                     hlayout.addWidget(spinbox)
                     entry["widget"] = spinbox
                 elif entry["type"] == "str":
                     lineedit = QLineEdit()
                     lineedit.setText(self.project["setup"][sname][ename])
-                    lineedit.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    lineedit.setToolTip(helptext)
                     lineedit.textChanged.connect(self.global_changed)  # type: ignore
                     hlayout.addWidget(lineedit)
                     entry["widget"] = lineedit
                 elif entry["type"] == "mstr":
                     mlineedit = QPlainTextEdit()
                     mlineedit.setPlainText(self.project["setup"][sname][ename])
-                    mlineedit.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    mlineedit.setToolTip(helptext)
                     mlineedit.textChanged.connect(self.global_changed)  # type: ignore
                     hlayout.addWidget(mlineedit)
                     entry["widget"] = mlineedit
                 elif entry["type"] == "table":
                     # add empty row if not exist
                     first_element = list(entry["columns"].keys())[0]
                     if entry.get("column_defaults") is not None and str(self.project["setup"][sname][ename][-1][first_element]) != "":
                         new_row = {}
                         for key, default in entry["column_defaults"].items():
                             new_row[key] = default
                         self.project["setup"][sname][ename].append(new_row)
 
                     table = QTableWidget()
-                    label.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    label.setToolTip(helptext)
                     table.setRowCount(len(self.project["setup"][sname][ename]))
                     idxf_offset = 0
                     table.setColumnCount(len(entry["columns"]))
                     if entry["selectable"]:
                         table.setColumnCount(len(entry["columns"]) + 1)
                         table.setHorizontalHeaderItem(0, QTableWidgetItem("Select"))
                         idxf_offset = 1
@@ -2032,101 +2039,105 @@
             titles = {
                 "mill": "Mill",
                 "tool": "Tool",
                 "pockets": "Pockets",
                 "tabs": "Tabs",
                 "leads": "Leads",
             }
+            scrollarea = QScrollArea()
+            scrollarea.setWidgetResizable(True)
             vcontainer = QWidget()
             vlayout = QVBoxLayout(vcontainer)
             vlayout.setContentsMargins(0, 0, 0, 0)
-            tabwidget.addTab(vcontainer, titles.get(sname, sname))
+            scrollarea.setWidget(vcontainer)
+            tabwidget.addTab(scrollarea, titles.get(sname, sname))
 
             for ename, entry in self.project["setup_defaults"][sname].items():
                 if not entry.get("per_object", False):
                     continue
-
+                helptext = entry.get("tooltip", f"{sname}/{ename}")
                 container = QWidget()
                 hlayout = QHBoxLayout(container)
                 hlayout.setContentsMargins(10, 0, 10, 0)
                 entry["widget_obj_label"] = QLabel(entry.get("title", ename))
+                entry["widget_obj_label"].setToolTip(helptext)
                 hlayout.addWidget(entry["widget_obj_label"])
                 vlayout.addWidget(container)
                 hlayout.addStretch(1)
                 if entry["type"] == "bool":
                     checkbox = QCheckBox(entry.get("title", ename))
                     checkbox.setChecked(self.project["setup"][sname][ename])
-                    checkbox.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    checkbox.setToolTip(helptext)
                     checkbox.stateChanged.connect(self.object_changed)  # type: ignore
                     hlayout.addWidget(checkbox)
                     entry["widget_obj"] = checkbox
                 elif entry["type"] == "select":
                     combobox = QComboBox()
                     for option in entry["options"]:
                         combobox.addItem(option[0])
                     combobox.setCurrentText(self.project["setup"][sname][ename])
-                    combobox.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    combobox.setToolTip(helptext)
                     combobox.currentTextChanged.connect(self.object_changed)  # type: ignore
                     hlayout.addWidget(combobox)
                     entry["widget_obj"] = combobox
                 elif entry["type"] == "color":
                     color = self.project["setup"][sname][ename]
                     rgb = f"{color[0] * 255:1.0f},{color[1] * 255:1.0f},{color[2] * 255:1.0f}"
                     button = QPushButton(rgb)
                     button.setStyleSheet(f"background-color:rgb({rgb})")
-                    button.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    button.setToolTip(helptext)
                     button.clicked.connect(partial(self.color_select, sname, ename))  # type: ignore
                     hlayout.addWidget(button)
                     entry["widget_obj"] = button
                 elif entry["type"] == "float":
                     dspinbox = QDoubleSpinBox()
                     dspinbox.setDecimals(entry.get("decimals", 4))
                     dspinbox.setSingleStep(entry.get("step", 1.0))
                     dspinbox.setMinimum(entry["min"])
                     dspinbox.setMaximum(entry["max"])
                     dspinbox.setValue(self.project["setup"][sname][ename])
-                    dspinbox.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    dspinbox.setToolTip(helptext)
                     dspinbox.valueChanged.connect(self.object_changed)  # type: ignore
                     hlayout.addWidget(dspinbox)
                     entry["widget_obj"] = dspinbox
                 elif entry["type"] == "int":
                     spinbox = QSpinBox()
                     spinbox.setSingleStep(entry.get("step", 1))
                     spinbox.setMinimum(entry["min"])
                     spinbox.setMaximum(entry["max"])
                     spinbox.setValue(self.project["setup"][sname][ename])
-                    spinbox.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    spinbox.setToolTip(helptext)
                     spinbox.valueChanged.connect(self.object_changed)  # type: ignore
                     hlayout.addWidget(spinbox)
                     entry["widget_obj"] = spinbox
                 elif entry["type"] == "str":
                     lineedit = QLineEdit()
                     lineedit.setText(self.project["setup"][sname][ename])
-                    lineedit.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    lineedit.setToolTip(helptext)
                     lineedit.textChanged.connect(self.object_changed)  # type: ignore
                     hlayout.addWidget(lineedit)
                     entry["widget_obj"] = lineedit
                 elif entry["type"] == "mstr":
                     mlineedit = QPlainTextEdit()
                     mlineedit.setPlainText(self.project["setup"][sname][ename])
-                    mlineedit.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    mlineedit.setToolTip(helptext)
                     mlineedit.textChanged.connect(self.object_changed)  # type: ignore
                     hlayout.addWidget(mlineedit)
                     entry["widget_obj"] = mlineedit
                 elif entry["type"] == "table":
                     # add empty row if not exist
                     first_element = list(entry["columns"].keys())[0]
                     if entry.get("column_defaults") is not None and str(self.project["setup"][sname][ename][-1][first_element]) != "":
                         new_row = {}
                         for key, default in entry["column_defaults"].items():
                             new_row[key] = default
                         self.project["setup"][sname][ename].append(new_row)
 
                     table = QTableWidget()
-                    table.setToolTip(entry.get("tooltip", f"{sname}/{ename}"))
+                    table.setToolTip(helptext)
                     table.setRowCount(len(self.project["setup"][sname][ename]))
                     idxf_offset = 0
                     table.setColumnCount(len(entry["columns"]))
                     if entry["selectable"]:
                         table.setColumnCount(len(entry["columns"]) + 1)
                         table.setHorizontalHeaderItem(0, QTableWidgetItem("Select"))
                         idxf_offset = 1
@@ -2188,17 +2199,20 @@
             if with_childs:
                 for inner in object_active_obj["inner_objects"]:
                     move_object(self.project["objects"][inner], step_x, step_y)
 
             self.update_tabs_data()
             self.update_drawing()
 
+        scrollarea = QScrollArea()
+        scrollarea.setWidgetResizable(True)
         vcontainer = QWidget()
         vlayout = QVBoxLayout(vcontainer)
         vlayout.setContentsMargins(0, 0, 0, 0)
+        scrollarea.setWidget(vcontainer)
 
         vlayout.addWidget(QLabel("Move:"))
 
         vlayout.addWidget(QLabel("Steps"))
 
         dspinbox = QDoubleSpinBox()
         dspinbox.setDecimals(4)
@@ -2438,15 +2452,15 @@
 
         button = QPushButton("Clone Bottom")
         button.setToolTip(_("clone object"))
         button.clicked.connect(partial(object_copy, checkbox, "bottom"))  # type: ignore
         glayout.addWidget(button, 2, 1)
 
         vlayout.addStretch(1)
-        tabwidget.addTab(vcontainer, _("Manipulate"))
+        tabwidget.addTab(scrollarea, _("Manipulate"))
 
     def update_tabs_data(self) -> None:
         self.project["tabs"]["data"] = []
         for obj in self.project["objects"].values():
             layer = obj.get("layer")
             if layer.startswith(("BREAKS:", "_TABS")):
                 obj["setup"]["mill"]["active"] = False
@@ -2920,22 +2934,31 @@
         bottom_container.setLayout(left_gridlayout)
         vbox.addWidget(bottom_container, stretch=0)
 
         right_widget = QWidget()
         right_widget.setLayout(right_gridlayout)
 
         hlay = QHBoxLayout(self.project["window"])
-        hlay.addWidget(left_widget, stretch=1)
-        hlay.addWidget(right_widget, stretch=3)
+        hlay.setContentsMargins(0, 0, 0, 0)
+        splitter = QSplitter(Qt.Horizontal)
+        hlay.addWidget(splitter)
+
+        splitter.addWidget(left_widget)
+        splitter.addWidget(right_widget)
+
+        mwin_width = 1200
+        mwin_height = 800
+        lratio = 0.24
+        splitter.setSizes([int(mwin_width * lratio), int(mwin_height * (1.0 - lratio))])
 
         # Tools
         self.font_tool = FontTool(self)
         self.gear_tool = GearTool(self)
 
-        self.main.resize(1600, 1200)
+        self.main.resize(mwin_width, mwin_height)
         self.main.show()
         debug("main: gui ready")
 
         if self.project["engine"] == "2D":
             if self.project["status"] == "INIT":
                 self.project["status"] = "READY"
             self.update_drawing()
```

### Comparing `viaconstructor-0.6.7/viaconstructor.egg-info/PKG-INFO` & `viaconstructor-0.6.8/viaconstructor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.7
+Version: 0.6.8
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
```

### Comparing `viaconstructor-0.6.7/viaconstructor.egg-info/SOURCES.txt` & `viaconstructor-0.6.8/viaconstructor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

