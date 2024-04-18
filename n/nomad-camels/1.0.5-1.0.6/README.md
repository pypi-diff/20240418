# Comparing `tmp/nomad_camels-1.0.5.tar.gz` & `tmp/nomad_camels-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_camels-1.0.5.tar", last modified: Tue Mar 19 15:19:18 2024, max compression
+gzip compressed data, was "nomad_camels-1.0.6.tar", last modified: Thu Apr 18 10:19:11 2024, max compression
```

## Comparing `nomad_camels-1.0.5.tar` & `nomad_camels-1.0.6.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.528736 nomad_camels-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-03-19 15:19:18.528736 nomad_camels-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.500736 nomad_camels-1.0.5/nomad_camels/
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/CAMELS_start.py
--rw-r--r--   0 runner    (1001) docker     (127)    60424 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/MainApp_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.504736 nomad_camels-1.0.5/nomad_camels/bluesky_handling/
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/EpicsFieldSignal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/builder_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/custom_function_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/evaluation_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    24523 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/make_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    18062 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/protocol_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/special_plan_stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/variable_reading.py
--rw-r--r--   0 runner    (1001) docker     (127)    14527 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/bluesky_handling/visa_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.504736 nomad_camels-1.0.5/nomad_camels/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/commands/change_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.504736 nomad_camels-1.0.5/nomad_camels/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/extensions/extension_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/extensions/extension_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/extensions/extension_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.504736 nomad_camels-1.0.5/nomad_camels/frontpanels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.504736 nomad_camels-1.0.5/nomad_camels/frontpanels/helper_panels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/helper_panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/helper_panels/enterTextDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/helper_panels/pass_ask.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/instrument_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16946 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/instrument_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/manage_instruments.py
--rw-r--r--   0 runner    (1001) docker     (127)    26120 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/plot_definer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27537 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/protocol_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/frontpanels/settings_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.508736 nomad_camels-1.0.5/nomad_camels/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/CAMELS.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/CAMELS_Icon.png
--rw-r--r--   0 runner    (1001) docker     (127)   101760 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   479310 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav
--rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/camels-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/camels-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12919 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/camels_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/camels_vertical.png
--rw-r--r--   0 runner    (1001) docker     (127)    40043 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/dark.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.512736 nomad_camels-1.0.5/nomad_camels/graphics/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)    60728 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS.svg
--rw-r--r--   0 runner    (1001) docker     (127)    52644 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Icon.png
--rw-r--r--   0 runner    (1001) docker     (127)   349358 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico
--rw-r--r--   0 runner    (1001) docker     (127)    34101 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico
--rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    43703 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    96186 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_V1.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_v2.svg
--rw-r--r--   0 runner    (1001) docker     (127)   290607 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/camels - Kopie.png
--rw-r--r--   0 runner    (1001) docker     (127)   252699 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/camels_free.png
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/legacy/plus_sign.png
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/nomad-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/nomad-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/oasis-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/oasis-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/graphics/stuff.kdbx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.512736 nomad_camels-1.0.5/nomad_camels/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/device_installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/enterTextDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/extension_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/fit_definer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/for_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/general_protocol_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/gradient_descent_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/instrument_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    40148 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/mainWindow_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/pass_ask.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/plot_definer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/plot_definer_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/plot_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/protocol_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/read_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/set_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    24988 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/gui/settings_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.516736 nomad_camels-1.0.5/nomad_camels/loop_steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/call_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/change_device_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/export_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    29303 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/for_while_loops.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/gradient_descent.py
--rw-r--r--   0 runner    (1001) docker     (127)     9819 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/if_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/make_step_of_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/nd_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/prompt_loop_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    16801 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/read_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/run_subprotocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/set_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/set_value_popup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/set_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/simple_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/loop_steps/wait_loop_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.520736 nomad_camels-1.0.5/nomad_camels/main_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/main_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35409 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/main_classes/device_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/main_classes/list_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/main_classes/loop_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/main_classes/manual_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/main_classes/measurement_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/main_classes/plot_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)    51824 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/main_classes/plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    27023 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/main_classes/protocol_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.520736 nomad_camels-1.0.5/nomad_camels/manual_controls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/get_manual_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.520736 nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.520736 nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/set_panel_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/set_panel_device_ophyd.py
--rw-r--r--   0 runner    (1001) docker     (127)    18245 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/set_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.520736 nomad_camels-1.0.5/nomad_camels/manual_controls/stage_control/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/stage_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24990 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/stage_control/stage_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/manual_controls/stage_control/ui_stage_control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.520736 nomad_camels-1.0.5/nomad_camels/nomad_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/nomad_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/nomad_integration/file_uploading.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/nomad_integration/nomad_communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/nomad_integration/nomad_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/nomad_integration/sample_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.520736 nomad_camels-1.0.5/nomad_camels/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/tests/instrument_management_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20716 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/tests/startup_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.520736 nomad_camels-1.0.5/nomad_camels/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/tools/EPICS_driver_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/tools/databroker_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/tools/device_driver_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/tools/driver_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.524736 nomad_camels-1.0.5/nomad_camels/ui_widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/ui_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24055 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/ui_widgets/add_remove_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/ui_widgets/channels_check_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/ui_widgets/console_redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/ui_widgets/drag_drop_tree_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/ui_widgets/options_run_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/ui_widgets/path_button_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/ui_widgets/variable_tool_tip_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/ui_widgets/warn_popup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.528736 nomad_camels-1.0.5/nomad_camels/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/databroker_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/device_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/dict_recursive_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/exception_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/fit_variable_renaming.py
--rw-r--r--   0 runner    (1001) docker     (127)    24764 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/load_save_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/load_save_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/logging_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/number_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/password_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/plot_placement.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/qthreads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/theme_changing.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/treeView_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/update_camels.py
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/nomad_camels/utility/variables_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:19:18.528736 nomad_camels-1.0.5/nomad_camels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-03-19 15:19:18.000000 nomad_camels-1.0.5/nomad_camels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-03-19 15:19:18.000000 nomad_camels-1.0.5/nomad_camels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:19:18.000000 nomad_camels-1.0.5/nomad_camels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-19 15:19:18.000000 nomad_camels-1.0.5/nomad_camels.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-19 15:19:18.000000 nomad_camels-1.0.5/nomad_camels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-19 15:19:18.000000 nomad_camels-1.0.5/nomad_camels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-19 15:19:13.000000 nomad_camels-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 15:19:18.528736 nomad_camels-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.801388 nomad_camels-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-04-18 10:19:11.801388 nomad_camels-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.773387 nomad_camels-1.0.6/nomad_camels/
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/CAMELS_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61686 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/MainApp_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.773387 nomad_camels-1.0.6/nomad_camels/bluesky_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/EpicsFieldSignal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/builder_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13163 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/custom_function_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/evaluation_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27924 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/make_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/protocol_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/special_plan_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/variable_reading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14529 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/bluesky_handling/visa_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.773387 nomad_camels-1.0.6/nomad_camels/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/commands/change_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.777387 nomad_camels-1.0.6/nomad_camels/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/extensions/extension_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/extensions/extension_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/extensions/extension_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.777387 nomad_camels-1.0.6/nomad_camels/frontpanels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.777387 nomad_camels-1.0.6/nomad_camels/frontpanels/helper_panels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/helper_panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/helper_panels/enterTextDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/helper_panels/pass_ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/instrument_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17414 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/instrument_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/manage_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26120 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/plot_definer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27537 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/protocol_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/frontpanels/settings_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.781388 nomad_camels-1.0.6/nomad_camels/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/CAMELS.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/CAMELS_Icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   101760 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)   479310 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/camels-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/camels-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12919 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/camels_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/camels_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40043 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/dark.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.785388 nomad_camels-1.0.6/nomad_camels/graphics/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)    60728 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    52644 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   349358 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    34101 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43703 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    96186 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_V1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_v2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   290607 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/camels - Kopie.png
+-rw-r--r--   0 runner    (1001) docker     (127)   252699 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/camels_free.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/legacy/plus_sign.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/nomad-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/nomad-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/oasis-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/oasis-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/graphics/stuff.kdbx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.785388 nomad_camels-1.0.6/nomad_camels/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/device_installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/enterTextDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/extension_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/fit_definer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/general_protocol_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/gradient_descent_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/instrument_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40148 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/mainWindow_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/pass_ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/plot_definer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/plot_definer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/plot_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/protocol_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/read_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/set_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24988 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/gui/settings_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.789388 nomad_camels-1.0.6/nomad_camels/loop_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/call_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/change_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29303 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/for_while_loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9819 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/if_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/make_step_of_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/nd_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/prompt_loop_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16801 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/read_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/run_subprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/set_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/set_value_popup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/set_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/simple_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/loop_steps/wait_loop_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.789388 nomad_camels-1.0.6/nomad_camels/main_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/main_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35409 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/main_classes/device_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/main_classes/list_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/main_classes/loop_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/main_classes/manual_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/main_classes/measurement_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/main_classes/plot_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51824 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/main_classes/plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27023 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/main_classes/protocol_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.793388 nomad_camels-1.0.6/nomad_camels/manual_controls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/get_manual_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.793388 nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.793388 nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/set_panel_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/set_panel_device_ophyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18245 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/set_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.793388 nomad_camels-1.0.6/nomad_camels/manual_controls/stage_control/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/stage_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24990 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/stage_control/stage_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/manual_controls/stage_control/ui_stage_control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.793388 nomad_camels-1.0.6/nomad_camels/nomad_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/nomad_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/nomad_integration/file_uploading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/nomad_integration/nomad_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/nomad_integration/nomad_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/nomad_integration/sample_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.793388 nomad_camels-1.0.6/nomad_camels/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/tests/instrument_management_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20716 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/tests/startup_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.793388 nomad_camels-1.0.6/nomad_camels/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/tools/EPICS_driver_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/tools/databroker_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/tools/device_driver_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/tools/driver_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.797388 nomad_camels-1.0.6/nomad_camels/ui_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/ui_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25071 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/ui_widgets/add_remove_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/ui_widgets/channels_check_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/ui_widgets/console_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/ui_widgets/drag_drop_tree_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/ui_widgets/options_run_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/ui_widgets/path_button_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/ui_widgets/variable_tool_tip_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/ui_widgets/warn_popup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.801388 nomad_camels-1.0.6/nomad_camels/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/databroker_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/device_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/dict_recursive_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/exception_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/fit_variable_renaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24764 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/load_save_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/load_save_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/logging_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/number_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/password_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/plot_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/qthreads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/theme_changing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/treeView_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/update_camels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/nomad_camels/utility/variables_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:19:11.801388 nomad_camels-1.0.6/nomad_camels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-04-18 10:19:11.000000 nomad_camels-1.0.6/nomad_camels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-18 10:19:11.000000 nomad_camels-1.0.6/nomad_camels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:19:11.000000 nomad_camels-1.0.6/nomad_camels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 10:19:11.000000 nomad_camels-1.0.6/nomad_camels.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-18 10:19:11.000000 nomad_camels-1.0.6/nomad_camels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 10:19:11.000000 nomad_camels-1.0.6/nomad_camels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-18 10:19:07.000000 nomad_camels-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:19:11.801388 nomad_camels-1.0.6/setup.cfg
```

### Comparing `nomad_camels-1.0.5/LICENSE` & `nomad_camels-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/PKG-INFO` & `nomad_camels-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad_camels
-Version: 1.0.5
+Version: 1.0.6
 Summary: CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.11.3
@@ -94,14 +94,15 @@
 Requires-Dist: iso8601>=1.0.2
 Requires-Dist: tables>=3.7.0
 Requires-Dist: numexpr>=2.8.4
 Requires-Dist: qt-material>=2.12
 Requires-Dist: pyserial>=3.5
 Requires-Dist: pyvisa>=1.13.0
 Requires-Dist: pyvisa-py>=0.7.0
+Requires-Dist: importlib-metadata>=6.6.0
 
 
 ```
  _  _   ___   __  __  ___  ___        ___  ___  __  __  ___  _     ___ 
 | \| | / _ \ |  \/  |/   \|   \      / __|/   \|  \/  || __|| |   / __|
 | .  || (_) || |\/| || - || |) |    | (__ | - || |\/| || _| | |__ \__ \
 |_|\_| \___/ |_|  |_||_|_||___/      \___||_|_||_|  |_||___||____||___/
@@ -121,14 +122,24 @@
 
 Please also see our publication in the Journal of Open Source Software (JOSS):
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.06371/status.svg)](https://doi.org/10.21105/joss.06371)
 
 
 # Changelog
+## 1.0.6
+Features:
+- Added an "owner" field to the samples, it is automatically populated when a new sample is created. This should stop cluttering the samples for all users. Only the current user's samples will show in the comboBox, or those without owner.
+- Added possibility to use instruments that generate their channels at runtime. 
+- Added SequentialDevice that forces every call to the instrument to wait for the previous one to finish.
+- Added the `*.py` and `*_ophyd.py` file contents as metadata to each instrument in the final measurement file. 
+
+Fixes:
+- "Hide info" button in instrument installer now working
+
 ## 1.0.5
 Changes:
 - Driver versions now have a separate branch on CAMELS_drivers to improve keeping them up to date
 - Same for extensions
 - Now checking filenames of protocols for invalid characters
 - Improved speed of looking for updates
```

### Comparing `nomad_camels-1.0.5/README.md` & `nomad_camels-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,24 @@
 
 Please also see our publication in the Journal of Open Source Software (JOSS):
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.06371/status.svg)](https://doi.org/10.21105/joss.06371)
 
 
 # Changelog
+## 1.0.6
+Features:
+- Added an "owner" field to the samples, it is automatically populated when a new sample is created. This should stop cluttering the samples for all users. Only the current user's samples will show in the comboBox, or those without owner.
+- Added possibility to use instruments that generate their channels at runtime. 
+- Added SequentialDevice that forces every call to the instrument to wait for the previous one to finish.
+- Added the `*.py` and `*_ophyd.py` file contents as metadata to each instrument in the final measurement file. 
+
+Fixes:
+- "Hide info" button in instrument installer now working
+
 ## 1.0.5
 Changes:
 - Driver versions now have a separate branch on CAMELS_drivers to improve keeping them up to date
 - Same for extensions
 - Now checking filenames of protocols for invalid characters
 - Improved speed of looking for updates
```

### Comparing `nomad_camels-1.0.5/nomad_camels/CAMELS_start.py` & `nomad_camels-1.0.6/nomad_camels/CAMELS_start.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/MainApp_v2.py` & `nomad_camels-1.0.6/nomad_camels/MainApp_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 
         self.pushButton_editUserInfo.clicked.connect(self.edit_user_info)
         self.load_user_data()
         self.pushButton_editSampleInfo.clicked.connect(self.edit_sample_info)
         self.load_sample_data()
         variables_handling.CAMELS_path = os.path.dirname(__file__)
 
+        self.comboBox_user.currentTextChanged.connect(self.change_user)
         self.comboBox_user_type.addItems(["local user", "NOMAD user"])
         self.comboBox_user_type.currentTextChanged.connect(self.change_user_type)
         self.change_user_type()
 
         self.pushButton_login_nomad.clicked.connect(self.login_logout_nomad)
         self.pushButton_nomad_sample.clicked.connect(self.select_nomad_sample)
 
@@ -559,14 +560,19 @@
             self.active_user = userdat["active_user"]
             userdat.pop("active_user")
         self.userdata = userdat
         self.comboBox_user.addItems(userdat.keys())
         if not self.active_user == "default_user":
             self.comboBox_user.setCurrentText(self.active_user)
 
+    def change_user(self):
+        """Changes the active user to the selected user in the comboBox_user."""
+        self.active_user = self.comboBox_user.currentText()
+        self.update_shown_samples()
+
     def edit_sample_info(self):
         """Calls dialog for user-information when
         pushButton_editSampleInfo is clicked.
 
         The opened AddRemoveDialoge contains columns for Name,
         Identifier, and Preparation-Info.
         If the dialog is canceled, nothing is changed, otherwise the new
@@ -580,38 +586,63 @@
 
         """
         # IMPORT pandas and add_remove_table only if it is needed
         import pandas as pd
         from nomad_camels.ui_widgets import add_remove_table
 
         self.active_sample = self.comboBox_sample.currentText()
-        headers = ["name", "sample_id", "description"]
+        headers = ["name", "sample_id", "description", "owner"]
         tableData = pd.DataFrame.from_dict(self.sampledata, "index")
+        if not "owner" in tableData.columns:
+            tableData["owner"] = ""
+        # filter tableData so that only the samples are kept that have the
+        # current user as owner, or where "owner" is not set
+        tableData = tableData[
+            (tableData["owner"] == self.active_user)
+            | (tableData["owner"].isna())
+            | (tableData["owner"] == "")
+        ]
         dialog = add_remove_table.AddRemoveDialoge(
             headerLabels=headers,
             parent=self,
             title="Sample-Information",
             askdelete=True,
             tableData=tableData,
+            default_values={"owner": self.active_user},
         )
         if dialog.exec():
             # changing the returned dict to dataframe and back to have a
             # dictionary that is formatted as {name: {'Name': name,...}, ...}
             dat = dialog.get_data()
-            if re.search(r"[^\w\s]", str(dat["name"][0])):
-                raise ValueError(
-                    "Sample name contains special characters.\nPlease use only letters, numbers and whitespace."
-                )
-            dat["name"][0] = dat["name"][0].strip()
+            for i, d in enumerate(dat["name"]):
+                if re.search(r"[^\w\s]", str(d)):
+                    raise ValueError(
+                        f'Sample name "{d}" contains special characters.\nPlease use only letters, numbers and whitespace.'
+                    )
+                dat["name"][i] = d.strip()
             dat["Name2"] = dat["name"]
             data = pd.DataFrame(dat)
             data.set_index("Name2", inplace=True)
-            self.sampledata = data.to_dict("index")
+            self.sampledata.update(data.to_dict("index"))
+            self.update_shown_samples()
+
+    def update_shown_samples(self):
         self.comboBox_sample.clear()
-        self.comboBox_sample.addItems(self.sampledata.keys())
+        # filter the samples so that only the ones are shown where the user is
+        # the owner or where the owner is not set
+        self.comboBox_sample.addItems(
+            sorted(
+                [
+                    key
+                    for key in self.sampledata.keys()
+                    if self.sampledata[key]["owner"] == self.active_user
+                    or not self.sampledata[key]["owner"]
+                ]
+            )
+        )
         if self.active_sample in self.sampledata.keys():
             self.comboBox_sample.setCurrentText(self.active_sample)
 
     def save_sample_data(self):
         """Calling the save_dictionary function with the savefile as
         %localappdata%/sampledata.json and self.sampledata as dictionary.
```

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/EpicsFieldSignal.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/EpicsFieldSignal.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/builder_helper_functions.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/builder_helper_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/evaluation_helper.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/evaluation_helper.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/helper_functions.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/helper_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 )
 from PySide6.QtCore import Signal, Qt
 from PySide6.QtGui import QFont
 
 from nomad_camels.ui_widgets.add_remove_table import AddRemoveTable
 from nomad_camels.ui_widgets.channels_check_table import Channels_Check_Table
 
+import inspect
+import os
+import sys
+
 
 def trigger_multi(devices, grp=None):
     """
     This function triggers multiple devices
 
     Parameters
     ----------
@@ -683,14 +687,97 @@
             continue
         name = comp.item.attr
         if name not in dev.configuration_attrs:
             channels[f"{dev.name}_{name}"] = [dev.name, name]
     return channels
 
 
+def get_opyd_and_py_file_contents(classname, md, device_name):
+    """
+    Reads the content of the .py and _opyd.py driver files of the given instrument and adds
+    them to the metadata dictionary. If the files are not found, it adds a corresponding message
+    to the dictionary.
+
+    Parameters
+    ----------
+    classname : class or function
+        The class or function whose associated files' contents are to be read.
+    md : dict
+        The metadata dictionary where the content of the files should be added.
+    device_name : str
+        The name of the device associated with the classname.
+
+    Returns
+    -------
+    md : dict
+        The updated metadata dictionary with the content of the files added or with a message
+        indicating that the file was not found.
+
+    Raises
+    ------
+    FileNotFoundError
+        If the .py or _opyd.py files associated with the classname are not found.
+    """
+    if inspect.isfunction(classname):
+        try:
+            with open(classname.__code__.co_filename, "r") as file:
+                md["devices"][device_name][
+                    f"python_file_{os.path.splitext(os.path.basename(classname.__code__.co_filename))[0]}"
+                ] = file.read()
+        except FileNotFoundError:
+            md["devices"][device_name][
+                os.path.splitext(os.path.basename(classname.__code__.co_filename))[0]
+            ] = "._ophyd file not found"
+        try:
+            with open(
+                classname.__code__.co_filename.replace("_ophyd.py", ".py"), "r"
+            ) as file:
+                md["devices"][device_name][
+                    f"python_file_{os.path.splitext(os.path.basename(classname.__code__.co_filename))[0]}".replace(
+                        "_ophyd", ""
+                    )
+                ] = file.read()
+        except FileNotFoundError:
+            md["devices"][device_name][
+                os.path.splitext(os.path.basename(classname.__code__.co_filename))[
+                    0
+                ].replace("_ophyd", "")
+            ] = ".py file not found"
+
+    elif inspect.isclass(classname):
+        try:
+            with open(sys.modules[classname.__module__].__file__, "r") as file:
+                md["devices"][device_name][
+                    f"python_file_{os.path.splitext(os.path.basename(sys.modules[classname.__module__].__file__))[0]}"
+                ] = file.read()
+        except FileNotFoundError:
+            md["devices"][device_name][
+                os.path.splitext(
+                    os.path.basename(sys.modules[classname.__module__].__file__)
+                )[0]
+            ] = "._ophyd file not found"
+        try:
+            with open(
+                sys.modules[classname.__module__].__file__.replace("_ophyd.py", ".py"),
+                "r",
+            ) as file:
+                md["devices"][device_name][
+                    f"python_file_{os.path.splitext(os.path.basename(sys.modules[classname.__module__].__file__))[0]}".replace(
+                        "_ophyd", ""
+                    )
+                ] = file.read()
+        except FileNotFoundError:
+            md["devices"][device_name][
+                os.path.splitext(
+                    os.path.basename(sys.modules[classname.__module__].__file__)
+                )[0].replace("_ophyd", "")
+            ] = ".py file not found"
+    return md
+
+
 class Value_Setter(QWidget):
     set_signal = Signal(float)
     hide_signal = Signal()
 
 
 class Waiting_Bar(QWidget):
     def __init__(self, parent=None, title="", skipable=False):
```

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/make_catalog.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/make_catalog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/protocol_builder.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/protocol_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
     # clearing leftovers from former builds
     variables_handling.read_channel_names.clear()
     variables_handling.read_channel_sets.clear()
 
     # beginning of larger strings
     device_import_string = "\n"
     devices_string = ""
+    read_device_drivers_string = ""
     variable_string = "\nnamespace = {}\n"
     variable_string += "all_fits = {}\n"
     variable_string += "plots = []\n"
     variable_string += "boxes = {}\n"
     variable_string += "app = None\n"
     variable_string += f'save_path = "{save_path}"\n'
     variable_string += f'session_name = "{protocol.session_name}"\n'
@@ -273,14 +274,22 @@
         devices_string += f'\t\tdevice_config["{dev}"].update(settings)\n'
         devices_string += f'\t\tdevice_config["{dev}"].update(additional_info)\n'
         devices_string += f'\t\tdevs.update({{"{dev}": {dev}}})\n'
         if device.name in device_handling.local_packages:
             device_import_string += f'sys.path.append(r"{device_handling.local_package_paths[device.name]}")\n'
         device_import_string += f"from nomad_camels_driver_{device.name}.{device.name}_ophyd import {classname}\n"
         additional_string_devices += device.get_additional_string()
+        # For each device execute the get_opyd_and_py_file_contents from the helper_functions
+        # This adds the .pya and .py files to the metadata dictionary md
+        read_device_drivers_string += f"\tmd = helper_functions.get_opyd_and_py_file_contents({classname}, md, '{dev}')\n"
+
+
+
+
+
 
     # finishing up the device initialization
     devices_string += '\t\tprint("devices connected")\n'
     devices_string += f'\t\tmd = {{"devices": device_config, "description": "{repr(protocol.description)}"}}\n'
 
     # if using special nexus-format, some restructuring of metadata is done
     if protocol.use_nexus:
@@ -319,14 +328,15 @@
     userdata = userdata or {"name": "default_user"}
     protocol_string += user_sample_string(userdata, sampledata)
     protocol_string += f'\tmd["protocol_overview"] = "{protocol.get_short_string().encode("unicode_escape").decode()}"\n'
 
     # reading the file itself and adding it to the metadata
     protocol_string += '\twith open(__file__, "r", encoding="utf-8") as f:\n'
     protocol_string += '\t\tmd["python_script"] = f.read()\n'
+    protocol_string += read_device_drivers_string
     protocol_string += '\tmd["variables"] = namespace\n'
 
     # adding uid to RunEngine, calling the plan
     protocol_string += '\tRE.subscribe(uid_collector, "start")\n'
     protocol_string += f"\tRE({protocol.name}_plan(devs, md=md, runEngine=RE))\n"
 
     # wait for RunEngine to finish, then save the data
```

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/special_plan_stubs.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/special_plan_stubs.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/variable_reading.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/variable_reading.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/bluesky_handling/visa_signal.py` & `nomad_camels-1.0.6/nomad_camels/bluesky_handling/visa_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     retries,
     just_write=False,
     write_delay=0,
     retry_on_timeout=False,
 ):
     excs = []
     while visa_instrument.currently_reading:
-        time.sleep(0.1)
+        time.sleep(0.001)
     visa_instrument.currently_reading = True
     if write_delay:
         time.sleep(write_delay)
     for i in range(retries + 1):
         try:
             if retry_on_timeout:
                 try:
```

### Comparing `nomad_camels-1.0.5/nomad_camels/commands/change_sequence.py` & `nomad_camels-1.0.6/nomad_camels/commands/change_sequence.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/extensions/extension_contexts.py` & `nomad_camels-1.0.6/nomad_camels/extensions/extension_contexts.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/extensions/extension_management.py` & `nomad_camels-1.0.6/nomad_camels/extensions/extension_management.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py` & `nomad_camels-1.0.6/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/frontpanels/helper_panels/enterTextDialog.py` & `nomad_camels-1.0.6/nomad_camels/frontpanels/helper_panels/enterTextDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/frontpanels/instrument_config.py` & `nomad_camels-1.0.6/nomad_camels/frontpanels/instrument_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/frontpanels/instrument_installer.py` & `nomad_camels-1.0.6/nomad_camels/frontpanels/instrument_installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     import importlib_metadata
 
 all_instr = {}
 installed_instr = {}
 last_repo = ""
 last_branch = ""
 last_dir = ""
-repo_url = ""
+repo_url = "https://raw.githubusercontent.com/FAU-LAP/CAMELS_drivers/main"
 
 
 def getInstalledDevices(force=False, return_packages=False):
     """Goes through the given device_driver_path and returns a list of
     the available devices.
 
     Parameters
@@ -258,20 +258,31 @@
         self.build_table()
 
         self.install_thread = None
 
         self.pushButton_install_update_selected.clicked.connect(self.install_selected)
         self.pushButton_uninstall.clicked.connect(self.uninstall_selected)
         self.pushButton_update_drivers.clicked.connect(self.update_installed)
+        self.pushButton_info.clicked.connect(self.show_hide_info)
 
         self.device_table.clicked.connect(self.table_click)
 
         self.info_widge = Info_Widget()
         self.info_widge.setHidden(True)
-        self.layout().addWidget(self.info_widge, 0, 5, 5, 1)
+        self.layout().addWidget(self.info_widge, 0, 5, 8, 1)
+
+    def show_hide_info(self):
+        if self.info_widge.isHidden():
+            self.info_widge.setHidden(False)
+            self.adjustSize()
+            self.pushButton_info.setText("hide info")
+        else:
+            self.info_widge.setHidden(True)
+            self.adjustSize()
+            self.pushButton_info.setText("show info")
 
     def checkBox_change(self, row):
         """
 
         Parameters
         ----------
         row :
```

### Comparing `nomad_camels-1.0.5/nomad_camels/frontpanels/manage_instruments.py` & `nomad_camels-1.0.6/nomad_camels/frontpanels/manage_instruments.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/frontpanels/plot_definer.py` & `nomad_camels-1.0.6/nomad_camels/frontpanels/plot_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/frontpanels/protocol_config.py` & `nomad_camels-1.0.6/nomad_camels/frontpanels/protocol_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/frontpanels/settings_window.py` & `nomad_camels-1.0.6/nomad_camels/frontpanels/settings_window.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/CAMELS.ico` & `nomad_camels-1.0.6/nomad_camels/graphics/CAMELS.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/CAMELS_Icon.png` & `nomad_camels-1.0.6/nomad_camels/graphics/CAMELS_Icon.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3` & `nomad_camels-1.0.6/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav` & `nomad_camels-1.0.6/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/camels-horizontal.svg` & `nomad_camels-1.0.6/nomad_camels/graphics/camels-horizontal.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/camels-vertical.svg` & `nomad_camels-1.0.6/nomad_camels/graphics/camels-vertical.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/camels_horizontal.png` & `nomad_camels-1.0.6/nomad_camels/graphics/camels_horizontal.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/camels_vertical.png` & `nomad_camels-1.0.6/nomad_camels/graphics/camels_vertical.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/dark.qss` & `nomad_camels-1.0.6/nomad_camels/graphics/dark.qss`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS.svg` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Icon.png` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Icon.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Logo.png` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Logo.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Logo.svg` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Logo.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_V1.svg` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_V1.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/CAMELS_v2.svg` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/CAMELS_v2.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/camels - Kopie.png` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/camels - Kopie.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/camels_free.png` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/camels_free.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/legacy/plus_sign.png` & `nomad_camels-1.0.6/nomad_camels/graphics/legacy/plus_sign.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/nomad-horizontal.png` & `nomad_camels-1.0.6/nomad_camels/graphics/nomad-horizontal.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/nomad-horizontal.svg` & `nomad_camels-1.0.6/nomad_camels/graphics/nomad-horizontal.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/oasis-horizontal.png` & `nomad_camels-1.0.6/nomad_camels/graphics/oasis-horizontal.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/oasis-horizontal.svg` & `nomad_camels-1.0.6/nomad_camels/graphics/oasis-horizontal.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/graphics/stuff.kdbx` & `nomad_camels-1.0.6/nomad_camels/graphics/stuff.kdbx`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/device_installer.py` & `nomad_camels-1.0.6/nomad_camels/gui/device_installer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/enterTextDialog.py` & `nomad_camels-1.0.6/nomad_camels/gui/enterTextDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/extension_manager.py` & `nomad_camels-1.0.6/nomad_camels/gui/extension_manager.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/fit_definer.py` & `nomad_camels-1.0.6/nomad_camels/gui/fit_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/for_loop.py` & `nomad_camels-1.0.6/nomad_camels/gui/for_loop.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/general_protocol_settings.py` & `nomad_camels-1.0.6/nomad_camels/gui/general_protocol_settings.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/gradient_descent_step.py` & `nomad_camels-1.0.6/nomad_camels/gui/gradient_descent_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/instrument_config.py` & `nomad_camels-1.0.6/nomad_camels/gui/instrument_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/mainWindow_v2.py` & `nomad_camels-1.0.6/nomad_camels/gui/mainWindow_v2.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/pass_ask.py` & `nomad_camels-1.0.6/nomad_camels/gui/pass_ask.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/plot_definer.py` & `nomad_camels-1.0.6/nomad_camels/gui/plot_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/plot_definer_2d.py` & `nomad_camels-1.0.6/nomad_camels/gui/plot_definer_2d.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/plot_options.py` & `nomad_camels-1.0.6/nomad_camels/gui/plot_options.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/protocol_view.py` & `nomad_camels-1.0.6/nomad_camels/gui/protocol_view.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/read_channels.py` & `nomad_camels-1.0.6/nomad_camels/gui/read_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/set_channels.py` & `nomad_camels-1.0.6/nomad_camels/gui/set_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/gui/settings_window.py` & `nomad_camels-1.0.6/nomad_camels/gui/settings_window.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/call_function.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/call_function.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/change_device_config.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/change_device_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/export_data.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/export_data.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/for_while_loops.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/for_while_loops.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/gradient_descent.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/if_step.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/if_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/make_step_of_type.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/make_step_of_type.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/nd_sweep.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/nd_sweep.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/prompt_loop_step.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/prompt_loop_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/read_channels.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/read_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/run_subprotocol.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/run_subprotocol.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/set_channels.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/set_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/set_value_popup.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/set_value_popup.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/set_variables.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/set_variables.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/simple_sweep.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/simple_sweep.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/loop_steps/wait_loop_step.py` & `nomad_camels-1.0.6/nomad_camels/loop_steps/wait_loop_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/main_classes/device_class.py` & `nomad_camels-1.0.6/nomad_camels/main_classes/device_class.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/main_classes/list_plot.py` & `nomad_camels-1.0.6/nomad_camels/main_classes/list_plot.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/main_classes/loop_step.py` & `nomad_camels-1.0.6/nomad_camels/main_classes/loop_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/main_classes/manual_control.py` & `nomad_camels-1.0.6/nomad_camels/main_classes/manual_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/main_classes/measurement_channel.py` & `nomad_camels-1.0.6/nomad_camels/main_classes/measurement_channel.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/main_classes/plot_2D.py` & `nomad_camels-1.0.6/nomad_camels/main_classes/plot_2D.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/main_classes/plot_widget.py` & `nomad_camels-1.0.6/nomad_camels/main_classes/plot_widget.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/main_classes/protocol_class.py` & `nomad_camels-1.0.6/nomad_camels/main_classes/protocol_class.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/manual_controls/get_manual_controls.py` & `nomad_camels-1.0.6/nomad_camels/manual_controls/get_manual_controls.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/set_panel_device.py` & `nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/set_panel_device.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/set_panel_device_ophyd.py` & `nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/nomad_camels_driver_set_panel_device/set_panel_device_ophyd.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/manual_controls/set_panel/set_panel.py` & `nomad_camels-1.0.6/nomad_camels/manual_controls/set_panel/set_panel.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/manual_controls/stage_control/stage_control.py` & `nomad_camels-1.0.6/nomad_camels/manual_controls/stage_control/stage_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/manual_controls/stage_control/ui_stage_control.py` & `nomad_camels-1.0.6/nomad_camels/manual_controls/stage_control/ui_stage_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/nomad_integration/file_uploading.py` & `nomad_camels-1.0.6/nomad_camels/nomad_integration/file_uploading.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/nomad_integration/nomad_communication.py` & `nomad_camels-1.0.6/nomad_camels/nomad_integration/nomad_communication.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/nomad_integration/nomad_login.py` & `nomad_camels-1.0.6/nomad_camels/nomad_integration/nomad_login.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/nomad_integration/sample_selection.py` & `nomad_camels-1.0.6/nomad_camels/nomad_integration/sample_selection.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/tests/instrument_management_test.py` & `nomad_camels-1.0.6/nomad_camels/tests/instrument_management_test.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/tests/protocol_test.py` & `nomad_camels-1.0.6/nomad_camels/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/tests/startup_test.py` & `nomad_camels-1.0.6/nomad_camels/tests/startup_test.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/tools/EPICS_driver_builder.py` & `nomad_camels-1.0.6/nomad_camels/tools/EPICS_driver_builder.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/tools/databroker_exporter.py` & `nomad_camels-1.0.6/nomad_camels/tools/databroker_exporter.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/tools/device_driver_builder.py` & `nomad_camels-1.0.6/nomad_camels/tools/device_driver_builder.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/tools/driver_builder.py` & `nomad_camels-1.0.6/nomad_camels/tools/driver_builder.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/ui_widgets/add_remove_table.py` & `nomad_camels-1.0.6/nomad_camels/ui_widgets/add_remove_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         comboBoxes=None,
         subtables=None,
         growsize=False,
         checkstrings=None,
         askdelete=False,
         fixedsize=False,
         enableds=None,
+        default_values=None,
     ):
         """
 
         Parameters
         ----------
         addLabel : str, default "+"
             The label of the add-button
@@ -100,14 +101,25 @@
             data is contained
         checkstrings : int, list of int, default None
             Positions of the columns (if horizontal) that are to be
             checked for validity, if None, none are
         askdelete : bool, default False
             Whether to have a PopUp make sure, that the user wants to
             delete the selected column
+        fixedsize : bool, default False
+            Whether the widget should have a fixed size
+        enableds : int, list of int, default None
+            Positions of the columns (if horizontal) that are enabled,
+            If None, all are
+        default_values : dict, default None
+            A dict with the default values for the table. The keys are
+            the column names and the values are the default values. If
+            a column is not in the dict, the default value is an empty
+            string. If None, all default values are empty strings.
+            The default values are used for new entries.
         """
         super().__init__(parent)
         self.setContextMenuPolicy(Qt.CustomContextMenu)
         self.customContextMenuRequested.connect(self.context_menu)
         layout = QGridLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(layout)
@@ -118,14 +130,15 @@
         self.checkstrings = (
             checkstrings if not type(checkstrings) is int else [checkstrings]
         )
         self.horizontal = horizontal
         self.orderBy = orderBy
         self.comboBoxes = {} if comboBoxes is None else comboBoxes
         self.subtables = {} if subtables is None else subtables
+        self.default_values = {} if default_values is None else default_values
         self.growsize = growsize
         self.fixedsize = fixedsize
         self.boxes = []
         self.tables = []
         if headerLabels is None and tableData is not None:
             headerLabels = tableData.keys()
         elif tableData is None and headerLabels is not None:
@@ -396,14 +409,18 @@
 
         Returns
         -------
 
         """
         if vals is None:
             vals = [""] * len(self.headerLabels) if len(self.headerLabels) else ""
+            if self.default_values:
+                for i, name in enumerate(self.headerLabels):
+                    if name in self.default_values:
+                        vals[i] = self.default_values[name]
         items = []
         box_indexes = []
         boxes = []
         table_indexes = []
         tables = []
         for i, name in enumerate(self.headerLabels):
             item = QStandardItem()
@@ -595,14 +612,15 @@
         parent=None,
         tableData=None,
         title="",
         comboBoxes=None,
         subtables=None,
         checkstrings=None,
         askdelete=False,
+        default_values=None,
     ):
         super().__init__(parent)
         self.setWindowFlags(self.windowFlags() | Qt.WindowMaximizeButtonHint)
         self.buttonBox = QDialogButtonBox(self)
         self.buttonBox.setOrientation(Qt.Horizontal)
         self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel | QDialogButtonBox.Ok)
         self.buttonBox.setObjectName("buttonBox")
@@ -622,14 +640,15 @@
             tableData=tableData,
             title=title,
             comboBoxes=comboBoxes,
             subtables=subtables,
             growsize=False,
             checkstrings=checkstrings,
             askdelete=askdelete,
+            default_values=default_values,
         )
 
         layout = QGridLayout()
         self.setLayout(layout)
         layout.addWidget(self.table, 0, 0)
         layout.addWidget(self.buttonBox, 1, 0)
         self.setWindowTitle(title)
```

### Comparing `nomad_camels-1.0.5/nomad_camels/ui_widgets/channels_check_table.py` & `nomad_camels-1.0.6/nomad_camels/ui_widgets/channels_check_table.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/ui_widgets/console_redirect.py` & `nomad_camels-1.0.6/nomad_camels/ui_widgets/console_redirect.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/ui_widgets/drag_drop_tree_view.py` & `nomad_camels-1.0.6/nomad_camels/ui_widgets/drag_drop_tree_view.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/ui_widgets/options_run_button.py` & `nomad_camels-1.0.6/nomad_camels/ui_widgets/options_run_button.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/ui_widgets/path_button_edit.py` & `nomad_camels-1.0.6/nomad_camels/ui_widgets/path_button_edit.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/ui_widgets/variable_tool_tip_box.py` & `nomad_camels-1.0.6/nomad_camels/ui_widgets/variable_tool_tip_box.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/databroker_export.py` & `nomad_camels-1.0.6/nomad_camels/utility/databroker_export.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/device_handling.py` & `nomad_camels-1.0.6/nomad_camels/utility/device_handling.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/dict_recursive_string.py` & `nomad_camels-1.0.6/nomad_camels/utility/dict_recursive_string.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/exception_hook.py` & `nomad_camels-1.0.6/nomad_camels/utility/exception_hook.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/fit_variable_renaming.py` & `nomad_camels-1.0.6/nomad_camels/utility/fit_variable_renaming.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/load_save_functions.py` & `nomad_camels-1.0.6/nomad_camels/utility/load_save_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/load_save_helper_functions.py` & `nomad_camels-1.0.6/nomad_camels/utility/load_save_helper_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/logging_settings.py` & `nomad_camels-1.0.6/nomad_camels/utility/logging_settings.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/number_formatting.py` & `nomad_camels-1.0.6/nomad_camels/utility/number_formatting.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/password_widgets.py` & `nomad_camels-1.0.6/nomad_camels/utility/password_widgets.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/plot_placement.py` & `nomad_camels-1.0.6/nomad_camels/utility/plot_placement.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/qthreads.py` & `nomad_camels-1.0.6/nomad_camels/utility/qthreads.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/theme_changing.py` & `nomad_camels-1.0.6/nomad_camels/utility/theme_changing.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/tqdm_progress_bar.py` & `nomad_camels-1.0.6/nomad_camels/utility/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/treeView_functions.py` & `nomad_camels-1.0.6/nomad_camels/utility/treeView_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/update_camels.py` & `nomad_camels-1.0.6/nomad_camels/utility/update_camels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels/utility/variables_handling.py` & `nomad_camels-1.0.6/nomad_camels/utility/variables_handling.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels.egg-info/PKG-INFO` & `nomad_camels-1.0.6/nomad_camels.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomad_camels
-Version: 1.0.5
+Version: 1.0.6
 Summary: CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.11.3
@@ -94,14 +94,15 @@
 Requires-Dist: iso8601>=1.0.2
 Requires-Dist: tables>=3.7.0
 Requires-Dist: numexpr>=2.8.4
 Requires-Dist: qt-material>=2.12
 Requires-Dist: pyserial>=3.5
 Requires-Dist: pyvisa>=1.13.0
 Requires-Dist: pyvisa-py>=0.7.0
+Requires-Dist: importlib-metadata>=6.6.0
 
 
 ```
  _  _   ___   __  __  ___  ___        ___  ___  __  __  ___  _     ___ 
 | \| | / _ \ |  \/  |/   \|   \      / __|/   \|  \/  || __|| |   / __|
 | .  || (_) || |\/| || - || |) |    | (__ | - || |\/| || _| | |__ \__ \
 |_|\_| \___/ |_|  |_||_|_||___/      \___||_|_||_|  |_||___||____||___/
@@ -121,14 +122,24 @@
 
 Please also see our publication in the Journal of Open Source Software (JOSS):
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.06371/status.svg)](https://doi.org/10.21105/joss.06371)
 
 
 # Changelog
+## 1.0.6
+Features:
+- Added an "owner" field to the samples, it is automatically populated when a new sample is created. This should stop cluttering the samples for all users. Only the current user's samples will show in the comboBox, or those without owner.
+- Added possibility to use instruments that generate their channels at runtime. 
+- Added SequentialDevice that forces every call to the instrument to wait for the previous one to finish.
+- Added the `*.py` and `*_ophyd.py` file contents as metadata to each instrument in the final measurement file. 
+
+Fixes:
+- "Hide info" button in instrument installer now working
+
 ## 1.0.5
 Changes:
 - Driver versions now have a separate branch on CAMELS_drivers to improve keeping them up to date
 - Same for extensions
 - Now checking filenames of protocols for invalid characters
 - Improved speed of looking for updates
```

### Comparing `nomad_camels-1.0.5/nomad_camels.egg-info/SOURCES.txt` & `nomad_camels-1.0.6/nomad_camels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels-1.0.5/nomad_camels.egg-info/requires.txt` & `nomad_camels-1.0.6/nomad_camels.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -82,7 +82,8 @@
 iso8601>=1.0.2
 tables>=3.7.0
 numexpr>=2.8.4
 qt-material>=2.12
 pyserial>=3.5
 pyvisa>=1.13.0
 pyvisa-py>=0.7.0
+importlib-metadata>=6.6.0
```

### Comparing `nomad_camels-1.0.5/pyproject.toml` & `nomad_camels-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nomad_camels"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     { name="FAIRmat - HU Berlin", email="nomad-camels@fau.de" }
 ]
 description = "CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics."
 readme = "README.md"
 requires-python = ">=3.11.3"
 classifiers = [
```

### Comparing `nomad_camels-1.0.5/requirements.txt` & `nomad_camels-1.0.6/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -82,7 +82,8 @@
 iso8601>=1.0.2
 tables>=3.7.0
 numexpr>=2.8.4
 qt-material>=2.12
 pyserial>=3.5
 pyvisa>=1.13.0
 pyvisa-py>=0.7.0
+importlib-metadata>=6.6.0
```

