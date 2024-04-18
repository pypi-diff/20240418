# Comparing `tmp/streamlit_nightly-1.33.1.dev20240416.tar.gz` & `tmp/streamlit_nightly-1.33.1.dev20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.33.1.dev20240416.tar", last modified: Wed Apr 17 06:58:55 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.33.1.dev20240417.tar", last modified: Thu Apr 18 07:50:01 2024, max compression
```

## Comparing `streamlit_nightly-1.33.1.dev20240416.tar` & `streamlit_nightly-1.33.1.dev20240417.tar`

### file list

```diff
@@ -1,571 +1,571 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.346979 streamlit_nightly-1.33.1.dev20240416/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-17 06:58:55.342979 streamlit_nightly-1.33.1.dev20240416/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.214978 streamlit_nightly-1.33.1.dev20240416/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:58:55.346979 streamlit_nightly-1.33.1.dev20240416/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.222978 streamlit_nightly-1.33.1.dev20240416/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.222978 streamlit_nightly-1.33.1.dev20240416/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.222978 streamlit_nightly-1.33.1.dev20240416/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.222978 streamlit_nightly-1.33.1.dev20240416/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.226978 streamlit_nightly-1.33.1.dev20240416/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.226978 streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.226978 streamlit_nightly-1.33.1.dev20240416/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    34224 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.234978 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/altair_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    57049 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/arrow_altair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/arrow_vega_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    27373 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.234978 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51087 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    26886 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.238978 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30876 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35625 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17561 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13158 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26369 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    21439 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.238978 streamlit_nightly-1.33.1.dev20240416/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.238978 streamlit_nightly-1.33.1.dev20240416/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.238978 streamlit_nightly-1.33.1.dev20240416/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.238978 streamlit_nightly-1.33.1.dev20240416/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.266978 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-17 06:55:06.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.270978 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.274978 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26158 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18570 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.274978 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.274978 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30549 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29567 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.274978 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.278978 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.278978 streamlit_nightly-1.33.1.dev20240416/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-17 06:55:36.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.214978 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.278978 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/css/2411.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/css/3092.95a45cfe.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/css/43.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/css/main.bf304093.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.314978 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1168.1d6408e6.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1307.8ea033f1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/178.b5384fd0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1792.b8efa879.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2090700 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2411.a8823789.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2411.a8823789.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3636801 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2736.914069e5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    43574 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3092.152fd2b7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3513.e3e7300a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3631.be5c35fa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3998.01237fcf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4113.1e7eff4d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4185.935c68ec.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4253.749d5244.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/43.9ae03282.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4319.a6745434.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4477.e10e4373.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4666.492dcf72.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/474.87506447.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5345.65c91ee7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6013.8e80e091.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2249519 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6150.1294fa0d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   840843 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/656.ae85f8f1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/656.ae85f8f1.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6853.d999ac75.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7217.d970c074.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7323.2808d029.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7602.6175e969.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7805.51638fbc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8427.d30dffe1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8477.e948c092.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8492.f56c9d4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9330.d29313d4.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9336.2d95d840.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9758.6e6d8662.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4389306 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/main.713dd29d.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/main.713dd29d.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.334979 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-04-17 06:58:52.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.334979 streamlit_nightly-1.33.1.dev20240416/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.334979 streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    44770 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.334979 streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.338979 streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.338979 streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.338979 streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.338979 streamlit_nightly-1.33.1.dev20240416/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.342979 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.342979 streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-17 06:58:54.000000 streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-04-17 06:58:54.000000 streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:58:54.000000 streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 06:58:54.000000 streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:55:00.000000 streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-17 06:58:54.000000 streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 06:58:54.000000 streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:55.342979 streamlit_nightly-1.33.1.dev20240416/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-17 06:53:25.000000 streamlit_nightly-1.33.1.dev20240416/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.132559 streamlit_nightly-1.33.1.dev20240417/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-18 07:50:01.128559 streamlit_nightly-1.33.1.dev20240417/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.016558 streamlit_nightly-1.33.1.dev20240417/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 07:50:01.132559 streamlit_nightly-1.33.1.dev20240417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.024558 streamlit_nightly-1.33.1.dev20240417/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.024558 streamlit_nightly-1.33.1.dev20240417/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.024558 streamlit_nightly-1.33.1.dev20240417/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.024558 streamlit_nightly-1.33.1.dev20240417/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.024558 streamlit_nightly-1.33.1.dev20240417/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.028558 streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.028558 streamlit_nightly-1.33.1.dev20240417/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33936 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.032559 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/altair_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57049 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/arrow_altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/arrow_vega_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27373 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.036558 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51087 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26886 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9897 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.036558 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31409 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13445 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17437 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17627 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21538 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29179 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.036558 streamlit_nightly-1.33.1.dev20240417/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.036558 streamlit_nightly-1.33.1.dev20240417/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.036558 streamlit_nightly-1.33.1.dev20240417/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.040558 streamlit_nightly-1.33.1.dev20240417/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.064559 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-18 07:46:17.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.064559 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36802 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.068559 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26158 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.068559 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.068559 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29567 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.068559 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.072559 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.072559 streamlit_nightly-1.33.1.dev20240417/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-18 07:46:47.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.016558 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.072559 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/css/2411.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/css/3092.95a45cfe.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/css/43.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29048 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/css/main.bf304093.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.104559 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1168.1d6408e6.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1307.8ea033f1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/178.b5384fd0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1792.b8efa879.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2090700 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2411.a8823789.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2411.a8823789.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2469.3e9c3ce9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3636801 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2736.914069e5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43574 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3092.152fd2b7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3513.e3e7300a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3631.be5c35fa.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3998.01237fcf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4113.1e7eff4d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4185.935c68ec.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   395952 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4253.749d5244.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/43.05a14cc7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4319.a6745434.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4477.e10e4373.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4666.492dcf72.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/474.87506447.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5345.65c91ee7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6013.8e80e091.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2249519 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6150.1294fa0d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   840843 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/656.ae85f8f1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/656.ae85f8f1.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6853.d999ac75.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7217.d970c074.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3383788 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7323.2808d029.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7602.6175e969.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7805.51638fbc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8427.d30dffe1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8477.e948c092.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8492.f56c9d4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9330.d29313d4.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9336.2d95d840.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9758.6e6d8662.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4389247 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/main.f215a056.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/main.f215a056.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.120559 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-04-18 07:49:58.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.120559 streamlit_nightly-1.33.1.dev20240417/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.124559 streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44770 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.124559 streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.124559 streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.124559 streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.124559 streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.124559 streamlit_nightly-1.33.1.dev20240417/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.128559 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.128559 streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-18 07:49:59.000000 streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-04-18 07:49:59.000000 streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:49:59.000000 streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 07:49:59.000000 streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:46:10.000000 streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-18 07:49:59.000000 streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 07:49:59.000000 streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:50:01.128559 streamlit_nightly-1.33.1.dev20240417/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-18 07:44:39.000000 streamlit_nightly-1.33.1.dev20240417/tests/testutil.py
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/PKG-INFO` & `streamlit_nightly-1.33.1.dev20240417/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.33.1.dev20240416
+Version: 1.33.1.dev20240417
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/bin/streamlit.cmd` & `streamlit_nightly-1.33.1.dev20240417/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/setup.py` & `streamlit_nightly-1.33.1.dev20240417/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.33.1.dev20240416"  # PEP-440
+VERSION = "1.33.1.dev20240417"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/__main__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/case_converters.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/cli_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/code_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/color_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/column_config.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/commands/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/commands/execution_control.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/commands/page_config.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/types/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/components.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/components/v1/custom_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import json
 from typing import TYPE_CHECKING, Any
 
 from streamlit import _main, type_util
 from streamlit.components.types.base_custom_component import BaseCustomComponent
 from streamlit.elements.form import current_form_id
+from streamlit.elements.utils import check_cache_replay_rules
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.Components_pb2 import ArrowTable as ArrowTableProto
 from streamlit.proto.Components_pb2 import SpecialArg
 from streamlit.proto.Element_pb2 import Element
 from streamlit.runtime.metrics_util import gather_metrics
 from streamlit.runtime.scriptrunner import get_script_run_ctx
 from streamlit.runtime.state import NoValue, register_widget
@@ -97,14 +98,15 @@
 PyArrow. To do so locally:
 
 `pip install pyarrow`
 
 And if you're using Streamlit Cloud, add "pyarrow" to your requirements.txt."""
             )
 
+        check_cache_replay_rules()
         # In addition to the custom kwargs passed to the component, we also
         # send the special 'default' and 'key' params to the component
         # frontend.
         all_args = dict(kwargs, **{"default": default, "key": key})
 
         json_args = {}
         special_args = []
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/config.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/config_option.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/config_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/connections/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/connections/base_connection.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/connections/util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/constants.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/cursor.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/delta_generator.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/delta_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,19 +524,14 @@
         if ctx and ctx.current_fragment_id and _writes_directly_to_sidebar(dg):
             raise StreamlitAPIException(
                 "Calling `st.sidebar` in a function wrapped with `st.experimental_fragment` "
                 "is not supported. To write elements to the sidebar with a fragment, "
                 "call your fragment function inside a `with st.sidebar` context manager."
             )
 
-        # Warn if we're called from within a legacy @st.cache function
-        legacy_caching.maybe_show_cached_st_function_warning(dg, delta_type)
-        # Warn if we're called from within @st.memo or @st.singleton
-        caching.maybe_show_cached_st_function_warning(dg, delta_type)
-
         # Warn if an element is being changed but the user isn't running the streamlit server.
         _maybe_print_use_warning()
 
         # Some elements have a method.__name__ != delta_type in proto.
         # This really matters for line_chart, bar_chart & area_chart,
         # since add_rows() relies on method.__name__ == delta_type
         # TODO: Fix for all elements (or the cache warning above will be wrong)
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/deprecation_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/development.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/echo.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/alert.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/altair_utils.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/altair_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/arrow.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/arrow_altair.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/arrow_altair.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/arrow_vega_lite.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/arrow_vega_lite.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,15 +151,22 @@
         # This only works for string keys, but kwarg keys are strings anyways.
         spec = dict(spec, **dicttools.unflatten(kwargs, _CHANNELS))
 
     if len(spec) == 0:
         raise ValueError("Vega-Lite charts require a non-empty spec dict.")
 
     if "autosize" not in spec:
-        spec["autosize"] = {"type": "fit", "contains": "padding"}
+        # type fit does not work for many chart types. This change focuses
+        # on vconcat with use_container_width=True as there are unintended
+        # consequences of changing the default autosize for all charts.
+        # fit-x fits the width and height can be adjusted.
+        if "vconcat" in spec and use_container_width:
+            spec["autosize"] = {"type": "fit-x", "contains": "padding"}
+        else:
+            spec["autosize"] = {"type": "fit", "contains": "padding"}
 
     # Pull data out of spec dict when it's in a 'datasets' key:
     #   marshall(proto, {datasets: {foo: df1, bar: df2}, ...})
     if "datasets" in spec:
         for k, v in spec["datasets"].items():
             dataset = proto.datasets.add()
             dataset.name = str(k)
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/balloons.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/code.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/dialog_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/doc_string.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/empty.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/exception.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/form.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,19 +190,23 @@
 
         .. output::
            https://doc-form2.streamlit.app/
            height: 375px
 
         """
         # Import this here to avoid circular imports.
-        from streamlit.elements.utils import check_session_state_rules
+        from streamlit.elements.utils import (
+            check_cache_replay_rules,
+            check_session_state_rules,
+        )
 
         if is_in_form(self.dg):
             raise StreamlitAPIException("Forms cannot be nested in other forms.")
 
+        check_cache_replay_rules()
         check_session_state_rules(default_value=None, key=key, writes_allowed=False)
 
         # A form is uniquely identified by its key.
         form_id = key
 
         ctx = get_script_run_ctx()
         if ctx is not None:
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/heading.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/html.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/iframe.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/image.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/json.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/layouts.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/map.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/markdown.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/media.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/metric.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/progress.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/pyplot.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/snow.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/text.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/toast.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/utils.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from enum import Enum, EnumMeta
 from typing import TYPE_CHECKING, Any, Hashable, Iterable, Sequence, cast, overload
 
 import streamlit
 from streamlit import config, runtime, type_util
 from streamlit.elements.form import is_in_form
-from streamlit.errors import StreamlitAPIException
+from streamlit.errors import StreamlitAPIException, StreamlitAPIWarning
 from streamlit.proto.LabelVisibilityMessage_pb2 import LabelVisibilityMessage
 from streamlit.runtime.state import WidgetCallback, get_session_state
 from streamlit.runtime.state.common import RegisterWidgetResult
 from streamlit.type_util import T
 
 if TYPE_CHECKING:
     from streamlit.delta_generator import DeltaGenerator
@@ -82,14 +82,49 @@
         streamlit.warning(
             f'The widget with key "{key}" was created with a default value but'
             " also had its value set via the Session State API."
         )
         _shown_default_value_warning = True
 
 
+class CachedWidgetWarning(StreamlitAPIWarning):
+    def __init__(self):
+        super().__init__(
+            """
+Your script uses a widget command in a cached function
+(function decorated with `@st.cache_data` or `@st.cache_resource`).
+This code will only be called when we detect a cache "miss",
+which can lead to unexpected results.
+
+How to fix this:
+* Move all widget commands outside the cached function.
+* Or, if you know what you're doing, use `experimental_allow_widgets=True`
+in the cache decorator to enable widget replay and suppress this warning.
+"""
+        )
+
+
+def check_cache_replay_rules() -> None:
+    """Check if a widget is allowed to be used in the current context.
+    More specifically, this checks if the current context is inside a
+    cached function that disallows widget usage. If so, it raises a warning.
+
+    If there are other similar checks in the future, we could extend this
+    function to check for those as well. And rename it to check_widget_usage_rules.
+    """
+    if runtime.exists():
+        from streamlit.runtime.scriptrunner.script_run_context import get_script_run_ctx
+
+        ctx = get_script_run_ctx()
+        if ctx and ctx.disallow_cached_widget_usage:
+            # We use an exception here to show a proper stack trace
+            # that indicates to the user where the issue is.
+            streamlit.exception(CachedWidgetWarning())
+
+
 def get_label_visibility_proto_value(
     label_visibility_string: type_util.LabelVisibility,
 ) -> LabelVisibilityMessage.LabelVisibilityOptions.ValueType:
     """Returns one of LabelVisibilityMessage enum constants.py based on string value."""
 
     if label_visibility_string == "visible":
         return LabelVisibilityMessage.LabelVisibilityOptions.VISIBLE
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from textwrap import dedent
 from typing import TYPE_CHECKING, BinaryIO, Final, Literal, TextIO, Union, cast
 
 from typing_extensions import TypeAlias
 
 from streamlit import runtime, source_util
 from streamlit.elements.form import current_form_id, is_in_form
-from streamlit.elements.utils import check_callback_rules, check_session_state_rules
 from streamlit.errors import StreamlitAPIException
 from streamlit.file_util import get_main_script_directory, normalize_path_join
 from streamlit.proto.Button_pb2 import Button as ButtonProto
 from streamlit.proto.DownloadButton_pb2 import DownloadButton as DownloadButtonProto
 from streamlit.proto.LinkButton_pb2 import LinkButton as LinkButtonProto
 from streamlit.proto.PageLink_pb2 import PageLink as PageLinkProto
 from streamlit.runtime.metrics_util import gather_metrics
@@ -547,15 +546,25 @@
         *,  # keyword-only arguments:
         type: Literal["primary", "secondary"] = "secondary",
         disabled: bool = False,
         use_container_width: bool = False,
         ctx: ScriptRunContext | None = None,
     ) -> bool:
         key = to_key(key)
+
+        # Importing these functions here to avoid circular imports
+        from streamlit.elements.utils import (
+            check_cache_replay_rules,
+            check_callback_rules,
+            check_session_state_rules,
+        )
+
+        check_cache_replay_rules()
         check_session_state_rules(default_value=None, key=key, writes_allowed=False)
+        check_callback_rules(self.dg, on_click)
 
         id = compute_widget_id(
             "download_button",
             user_key=key,
             label=label,
             file_name=file_name,
             mime=mime,
@@ -700,16 +709,26 @@
         kwargs: WidgetKwargs | None = None,
         *,  # keyword-only arguments:
         type: Literal["primary", "secondary"] = "secondary",
         disabled: bool = False,
         use_container_width: bool = False,
         ctx: ScriptRunContext | None = None,
     ) -> bool:
+        key = to_key(key)
+
+        # Importing these functions here to avoid circular imports
+        from streamlit.elements.utils import (
+            check_cache_replay_rules,
+            check_callback_rules,
+            check_session_state_rules,
+        )
+
         if not is_form_submitter:
             check_callback_rules(self.dg, on_click)
+        check_cache_replay_rules()
         check_session_state_rules(default_value=None, key=key, writes_allowed=False)
 
         id = compute_widget_id(
             "button",
             user_key=key,
             label=label,
             key=key,
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/camera_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from textwrap import dedent
 from typing import TYPE_CHECKING, Union, cast
 
 from typing_extensions import TypeAlias
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
 )
 from streamlit.elements.widgets.file_uploader import _get_upload_files
 from streamlit.proto.CameraInput_pb2 import CameraInput as CameraInputProto
 from streamlit.proto.Common_pb2 import FileUploaderState as FileUploaderStateProto
@@ -191,14 +192,16 @@
         kwargs: WidgetKwargs | None = None,
         *,  # keyword-only arguments:
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> UploadedFile | None:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=None, key=key, writes_allowed=False)
         maybe_raise_label_warnings(label, label_visibility)
 
         id = compute_widget_id(
             "camera_input",
             user_key=key,
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import TYPE_CHECKING, Literal, cast
 
 from streamlit import runtime
 from streamlit.elements.form import is_in_form
 from streamlit.elements.image import AtomicImage, WidthBehaviour, image_to_url
-from streamlit.elements.utils import check_callback_rules, check_session_state_rules
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.Block_pb2 import Block as BlockProto
 from streamlit.proto.ChatInput_pb2 import ChatInput as ChatInputProto
 from streamlit.proto.Common_pb2 import StringTriggerValue as StringTriggerValueProto
 from streamlit.proto.RootContainer_pb2 import RootContainer
 from streamlit.runtime.metrics_util import gather_metrics
 from streamlit.runtime.scriptrunner import get_script_run_ctx
@@ -285,14 +284,22 @@
         .. output ::
             https://doc-chat-input-inline.streamlit.app/
             height: 350px
         """
         # We default to an empty string here and disallow user choice intentionally
         default = ""
         key = to_key(key)
+
+        from streamlit.elements.utils import (
+            check_cache_replay_rules,
+            check_callback_rules,
+            check_session_state_rules,
+        )
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_submit)
         check_session_state_rules(default_value=default, key=key, writes_allowed=False)
 
         ctx = get_script_run_ctx()
         id = compute_widget_id(
             "chat_input",
             user_key=key,
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/checkbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import TYPE_CHECKING, cast
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
 )
 from streamlit.proto.Checkbox_pb2 import Checkbox as CheckboxProto
 from streamlit.runtime.metrics_util import gather_metrics
 from streamlit.runtime.scriptrunner import ScriptRunContext, get_script_run_ctx
@@ -270,19 +271,20 @@
         *,  # keyword-only arguments:
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         type: CheckboxProto.StyleType.ValueType = CheckboxProto.StyleType.DEFAULT,
         ctx: ScriptRunContext | None = None,
     ) -> bool:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(
             default_value=None if value is False else value, key=key
         )
-
         maybe_raise_label_warnings(label, label_visibility)
 
         id = compute_widget_id(
             "toggle" if type == CheckboxProto.StyleType.TOGGLE else "checkbox",
             user_key=key,
             label=label,
             value=bool(value),
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/color_picker.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import cast
 
 import streamlit
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.ColorPicker_pb2 import ColorPicker as ColorPickerProto
 from streamlit.runtime.metrics_util import gather_metrics
@@ -165,14 +166,16 @@
         kwargs: WidgetKwargs | None = None,
         *,  # keyword-only arguments:
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> str:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=value, key=key)
         maybe_raise_label_warnings(label, label_visibility)
 
         id = compute_widget_id(
             "color_picker",
             user_key=key,
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/data_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     determine_dataframe_schema,
     is_type_compatible,
     marshall_column_config,
     process_config_mapping,
     update_column_config,
 )
 from streamlit.elements.lib.pandas_styler_utils import marshall_styler
-from streamlit.elements.utils import check_callback_rules, check_session_state_rules
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.Arrow_pb2 import Arrow as ArrowProto
 from streamlit.runtime.metrics_util import gather_metrics
 from streamlit.runtime.scriptrunner import get_script_run_ctx
 from streamlit.runtime.state import (
     WidgetArgs,
     WidgetCallback,
@@ -770,18 +769,28 @@
 
 
         .. output::
            https://doc-data-editor-config.streamlit.app/
            height: 350px
 
         """
+        # Lazy-loaded import
         import pandas as pd
         import pyarrow as pa
 
+        # Import here to avoid cyclic import warning
+        from streamlit.elements.utils import (
+            check_cache_replay_rules,
+            check_callback_rules,
+            check_session_state_rules,
+        )
+
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=None, key=key, writes_allowed=False)
 
         if column_order is not None:
             column_order = list(column_order)
 
         column_config_mapping: ColumnConfigMapping = {}
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/file_uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import TYPE_CHECKING, List, Literal, Sequence, Union, cast, overload
 
 from typing_extensions import TypeAlias
 
 from streamlit import config
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
 )
 from streamlit.proto.Common_pb2 import FileUploaderState as FileUploaderStateProto
 from streamlit.proto.Common_pb2 import UploadedFileInfo as UploadedFileInfoProto
 from streamlit.proto.FileUploader_pb2 import FileUploader as FileUploaderProto
@@ -394,14 +395,16 @@
         kwargs: WidgetKwargs | None = None,
         *,  # keyword-only arguments:
         label_visibility: LabelVisibility = "visible",
         disabled: bool = False,
         ctx: ScriptRunContext | None = None,
     ) -> UploadedFile | list[UploadedFile] | None:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=None, key=key, writes_allowed=False)
         maybe_raise_label_warnings(label, label_visibility)
 
         id = compute_widget_id(
             "file_uploader",
             user_key=key,
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/multiselect.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Callable, Generic, Sequence, cast, overload
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
     maybe_coerce_enum_sequence,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.MultiSelect_pb2 import MultiSelect as MultiSelectProto
@@ -278,20 +279,22 @@
         max_selections: int | None = None,
         placeholder: str = "Choose an option",
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> list[T]:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=default, key=key)
+        maybe_raise_label_warnings(label, label_visibility)
 
         opt = ensure_indexable(options)
         check_python_comparable(opt)
-        maybe_raise_label_warnings(label, label_visibility)
 
         indices = _check_and_convert_to_indices(opt, default)
 
         id = compute_widget_id(
             "multiselect",
             user_key=key,
             label=label,
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/number_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from textwrap import dedent
 from typing import TYPE_CHECKING, Literal, Union, cast, overload
 
 from typing_extensions import TypeAlias
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.js_number import JSNumber, JSNumberBoundsException
 from streamlit.proto.NumberInput_pb2 import NumberInput as NumberInputProto
@@ -273,14 +274,16 @@
         *,  # keyword-only arguments:
         placeholder: str | None = None,
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> Number | None:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(
             default_value=value if value != "min" else None, key=key
         )
         maybe_raise_label_warnings(label, label_visibility)
 
         id = compute_widget_id(
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/radio.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Callable, Generic, Sequence, cast
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
     maybe_coerce_enum,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.Radio_pb2 import Radio as RadioProto
@@ -245,17 +246,20 @@
         disabled: bool = False,
         horizontal: bool = False,
         label_visibility: LabelVisibility = "visible",
         captions: Sequence[str] | None = None,
         ctx: ScriptRunContext | None,
     ) -> T | None:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=None if index == 0 else index, key=key)
         maybe_raise_label_warnings(label, label_visibility)
+
         opt = ensure_indexable(options)
         check_python_comparable(opt)
 
         id = compute_widget_id(
             "radio",
             user_key=key,
             label=label,
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/select_slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Callable, Generic, Sequence, Tuple, cast
 
 from typing_extensions import TypeGuard
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
     maybe_coerce_enum,
     maybe_coerce_enum_sequence,
 )
 from streamlit.errors import StreamlitAPIException
@@ -252,17 +253,20 @@
         args: WidgetArgs | None = None,
         kwargs: WidgetKwargs | None = None,
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> T | tuple[T, T]:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=value, key=key)
         maybe_raise_label_warnings(label, label_visibility)
+
         opt = ensure_indexable(options)
         check_python_comparable(opt)
 
         if len(opt) == 0:
             raise StreamlitAPIException("The `options` argument needs to be non-empty")
 
         def as_index_list(v: object) -> list[int]:
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/selectbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Callable, Generic, Sequence, cast
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
     maybe_coerce_enum,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.Selectbox_pb2 import Selectbox as SelectboxProto
@@ -225,17 +226,18 @@
         *,  # keyword-only arguments:
         placeholder: str = "Choose an option",
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> T | None:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=None if index == 0 else index, key=key)
-
         maybe_raise_label_warnings(label, label_visibility)
 
         opt = ensure_indexable(options)
         check_python_comparable(opt)
 
         id = compute_widget_id(
             "selectbox",
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Final, Sequence, Tuple, TypeVar, Union, cast
 
 from typing_extensions import TypeAlias
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.js_number import JSNumber, JSNumberBoundsException
 from streamlit.proto.Slider_pb2 import Slider as SliderProto
@@ -360,17 +361,18 @@
         kwargs: WidgetKwargs | None = None,
         *,  # keyword-only arguments:
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> SliderReturn:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=value, key=key)
-
         maybe_raise_label_warnings(label, label_visibility)
 
         id = compute_widget_id(
             "slider",
             user_key=key,
             label=label,
             min_value=min_value,
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/text_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from dataclasses import dataclass
 from textwrap import dedent
 from typing import TYPE_CHECKING, Literal, cast, overload
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.TextArea_pb2 import TextArea as TextAreaProto
 from streamlit.proto.TextInput_pb2 import TextInput as TextInputProto
@@ -250,17 +251,17 @@
         *,  # keyword-only arguments:
         placeholder: str | None = None,
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> str | None:
         key = to_key(key)
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=None if value == "" else value, key=key)
-
         maybe_raise_label_warnings(label, label_visibility)
 
         # Make sure value is always string or None:
         value = str(value) if value is not None else None
 
         id = compute_widget_id(
             "text_input",
@@ -511,17 +512,18 @@
         *,  # keyword-only arguments:
         placeholder: str | None = None,
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> str | None:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(default_value=None if value == "" else value, key=key)
-
         maybe_raise_label_warnings(label, label_visibility)
 
         value = str(value) if value is not None else None
 
         id = compute_widget_id(
             "text_area",
             user_key=key,
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/time_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     overload,
 )
 
 from typing_extensions import TypeAlias
 
 from streamlit.elements.form import current_form_id
 from streamlit.elements.utils import (
+    check_cache_replay_rules,
     check_callback_rules,
     check_session_state_rules,
     get_label_visibility_proto_value,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.DateInput_pb2 import DateInput as DateInputProto
 from streamlit.proto.TimeInput_pb2 import TimeInput as TimeInputProto
@@ -409,14 +410,15 @@
         *,  # keyword-only arguments:
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         step: int | timedelta = timedelta(minutes=DEFAULT_STEP_MINUTES),
         ctx: ScriptRunContext | None = None,
     ) -> time | None:
         key = to_key(key)
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(
             default_value=value if value != "now" else None, key=key
         )
         maybe_raise_label_warnings(label, label_visibility)
 
         parsed_time: time | None
@@ -664,19 +666,20 @@
         *,  # keyword-only arguments:
         format: str = "YYYY/MM/DD",
         disabled: bool = False,
         label_visibility: LabelVisibility = "visible",
         ctx: ScriptRunContext | None = None,
     ) -> DateWidgetReturn:
         key = to_key(key)
+
+        check_cache_replay_rules()
         check_callback_rules(self.dg, on_change)
         check_session_state_rules(
             default_value=value if value != "default_value_today" else None, key=key
         )
-
         maybe_raise_label_warnings(label, label_visibility)
 
         def parse_date_deterministic(
             v: SingleDateValue | Literal["today"] | Literal["default_value_today"],
         ) -> str | None:
             if isinstance(v, datetime):
                 return date.strftime(v.date(), "%Y/%m/%d")
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/elements/write.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/emojis.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/env_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/error_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/errors.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/external/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/file_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/folder_black_list.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/git_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/hello/Hello.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/hello/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/hello/utils.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/js_number.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/logger.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/net_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/platform.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Toast_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.33.1.dev20240417/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/app_session.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-import contextlib
-from typing import Any, Iterator
+from typing import Any
 
 from google.protobuf.message import Message
 
 from streamlit.proto.Block_pb2 import Block
 from streamlit.runtime.caching.cache_data_api import (
     CACHE_DATA_MESSAGE_REPLAY_CTX,
     CacheDataAPI,
@@ -80,29 +79,14 @@
 
 
 def save_media_data(image_data: bytes | str, mimetype: str, image_id: str) -> None:
     CACHE_DATA_MESSAGE_REPLAY_CTX.save_image_data(image_data, mimetype, image_id)
     CACHE_RESOURCE_MESSAGE_REPLAY_CTX.save_image_data(image_data, mimetype, image_id)
 
 
-def maybe_show_cached_st_function_warning(dg, st_func_name: str) -> None:
-    CACHE_DATA_MESSAGE_REPLAY_CTX.maybe_show_cached_st_function_warning(
-        dg, st_func_name
-    )
-    CACHE_RESOURCE_MESSAGE_REPLAY_CTX.maybe_show_cached_st_function_warning(
-        dg, st_func_name
-    )
-
-
-@contextlib.contextmanager
-def suppress_cached_st_function_warning() -> Iterator[None]:
-    with CACHE_DATA_MESSAGE_REPLAY_CTX.suppress_cached_st_function_warning(), CACHE_RESOURCE_MESSAGE_REPLAY_CTX.suppress_cached_st_function_warning():
-        yield
-
-
 # Explicitly export public symbols
 from streamlit.runtime.caching.cache_data_api import get_data_cache_stats_provider
 from streamlit.runtime.caching.cache_resource_api import (
     get_resource_cache_stats_provider,
 )
 
 # Create and export public API singletons.
@@ -132,16 +116,14 @@
 
 __all__ = [
     "CACHE_DOCS_URL",
     "save_element_message",
     "save_block_message",
     "save_widget_metadata",
     "save_media_data",
-    "maybe_show_cached_st_function_warning",
-    "suppress_cached_st_function_warning",
     "get_data_cache_stats_provider",
     "get_resource_cache_stats_provider",
     "cache_data",
     "cache_resource",
     "experimental_memo",
     "experimental_singleton",
 ]
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,52 +92,14 @@
     pass
 
 
 class CacheError(Exception):
     pass
 
 
-class CachedStFunctionWarning(StreamlitAPIWarning):
-    def __init__(
-        self,
-        cache_type: CacheType,
-        st_func_name: str,
-        cached_func: types.FunctionType,
-    ):
-        args = {
-            "st_func_name": f"`st.{st_func_name}()`",
-            "func_name": self._get_cached_func_name_md(cached_func),
-            "decorator_name": get_decorator_api_name(cache_type),
-        }
-
-        msg = (
-            """
-Your script uses %(st_func_name)s to write to your Streamlit app from within
-some cached code at %(func_name)s. This code will only be called when we detect
-a cache "miss", which can lead to unexpected results.
-
-How to fix this:
-* Move the %(st_func_name)s call outside %(func_name)s.
-* Or, if you know what you're doing, use `@st.%(decorator_name)s(experimental_allow_widgets=True)`
-to enable widget replay and suppress this warning.
-            """
-            % args
-        ).strip("\n")
-
-        super().__init__(msg)
-
-    @staticmethod
-    def _get_cached_func_name_md(func: types.FunctionType) -> str:
-        """Get markdown representation of the function name."""
-        if hasattr(func, "__name__"):
-            return "`%s()`" % func.__name__
-        else:
-            return "a cached function"
-
-
 class CacheReplayClosureError(StreamlitAPIException):
     def __init__(
         self,
         cache_type: CacheType,
         cached_func: types.FunctionType,
     ):
         func_name = get_cached_func_name_md(cached_func)
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/cached_message_replay.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,21 +29,17 @@
     runtime_checkable,
 )
 
 from google.protobuf.message import Message
 
 import streamlit as st
 from streamlit import runtime, util
-from streamlit.elements import NONWIDGET_ELEMENTS, WIDGETS
 from streamlit.logger import get_logger
 from streamlit.proto.Block_pb2 import Block
-from streamlit.runtime.caching.cache_errors import (
-    CachedStFunctionWarning,
-    CacheReplayClosureError,
-)
+from streamlit.runtime.caching.cache_errors import CacheReplayClosureError
 from streamlit.runtime.caching.cache_type import CacheType
 from streamlit.runtime.caching.hashing import update_hash
 from streamlit.runtime.scriptrunner.script_run_context import (
     ScriptRunContext,
     get_script_run_ctx,
 )
 from streamlit.runtime.state.common import WidgetMetadata
@@ -235,48 +231,63 @@
     a cached function.
 
     Data is stored in a thread-local object, so it's safe to use an instance
     of this class across multiple threads.
     """
 
     def __init__(self, cache_type: CacheType):
-        self._cached_func_stack: list[types.FunctionType] = []
-        self._suppress_st_function_warning = 0
         self._cached_message_stack: list[list[MsgData]] = []
         self._seen_dg_stack: list[set[str]] = []
         self._most_recent_messages: list[MsgData] = []
         self._registered_metadata: WidgetMetadata[Any] | None = None
         self._media_data: list[MediaMsgData] = []
         self._cache_type = cache_type
-        self._allow_widgets: int = 0
+        self._allow_widgets: bool = False
 
     def __repr__(self) -> str:
         return util.repr_(self)
 
     @contextlib.contextmanager
     def calling_cached_function(
         self, func: types.FunctionType, allow_widgets: bool
     ) -> Iterator[None]:
         """Context manager that should wrap the invocation of a cached function.
         It allows us to track any `st.foo` messages that are generated from inside the function
         for playback during cache retrieval.
         """
-        self._cached_func_stack.append(func)
         self._cached_message_stack.append([])
         self._seen_dg_stack.append(set())
-        if allow_widgets:
-            self._allow_widgets += 1
+        self._allow_widgets = allow_widgets
+
+        nested_call = False
+        ctx = get_script_run_ctx()
+        if ctx:
+            if ctx.disallow_cached_widget_usage:
+                # The disallow_cached_widget_usage is already set to true.
+                # This indicates that this cached function run is called from another
+                # cached function that disallows widget usage.
+                # We need to deactivate the widget usage for this cached function run
+                # even if it was allowed.
+                self._allow_widgets = False
+                nested_call = True
+
+            if not self._allow_widgets:
+                # If we're in a cached function that disallows widget usage, we need to set
+                # the disallow_cached_widget_usage to true for this cached function run
+                # to prevent widget usage (triggers a warning).
+                ctx.disallow_cached_widget_usage = True
         try:
             yield
         finally:
-            self._cached_func_stack.pop()
             self._most_recent_messages = self._cached_message_stack.pop()
             self._seen_dg_stack.pop()
-            if allow_widgets:
-                self._allow_widgets -= 1
+            if ctx and not nested_call:
+                # Reset the disallow_cached_widget_usage flag. But only if this
+                # is not nested inside a cached function that disallows widget usage.
+                ctx.disallow_cached_widget_usage = False
 
     def save_element_message(
         self,
         delta_type: str,
         element_proto: Message,
         invoked_dg_id: str,
         used_dg_id: str,
@@ -361,67 +372,14 @@
         self._registered_metadata = metadata
 
     def save_image_data(
         self, image_data: bytes | str, mimetype: str, image_id: str
     ) -> None:
         self._media_data.append(MediaMsgData(image_data, mimetype, image_id))
 
-    @contextlib.contextmanager
-    def suppress_cached_st_function_warning(self) -> Iterator[None]:
-        self._suppress_st_function_warning += 1
-        try:
-            yield
-        finally:
-            self._suppress_st_function_warning -= 1
-            assert self._suppress_st_function_warning >= 0
-
-    def maybe_show_cached_st_function_warning(
-        self,
-        dg: DeltaGenerator,
-        st_func_name: str,
-    ) -> None:
-        """If appropriate, warn about calling st.foo inside @st.cache_data.
-
-        DeltaGenerator's @_with_element and @_widget wrappers use this to warn
-        the user when they're calling st.foo() from within a function that is
-        wrapped in @st.cache.
-
-        Parameters
-        ----------
-        dg : DeltaGenerator
-            The DeltaGenerator to publish the warning to.
-
-        st_func_name : str
-            The name of the Streamlit function that was called.
-
-        """
-        # There are some elements not in either list, which we still want to warn about.
-        # Ideally we will fix this by either updating the lists or creating a better
-        # way of categorizing elements.
-        if st_func_name in NONWIDGET_ELEMENTS:
-            return
-        if st_func_name in WIDGETS and self._allow_widgets > 0:
-            return
-
-        if len(self._cached_func_stack) > 0 and self._suppress_st_function_warning <= 0:
-            cached_func = self._cached_func_stack[-1]
-            self._show_cached_st_function_warning(dg, st_func_name, cached_func)
-
-    def _show_cached_st_function_warning(
-        self,
-        dg: DeltaGenerator,
-        st_func_name: str,
-        cached_func: types.FunctionType,
-    ) -> None:
-        # Avoid infinite recursion by suppressing additional cached
-        # function warnings from within the cached function warning.
-        with self.suppress_cached_st_function_warning():
-            e = CachedStFunctionWarning(self._cache_type, st_func_name, cached_func)
-            dg.exception(e)
-
 
 def replay_cached_messages(
     result: CachedResult, cache_type: CacheType, cached_func: types.FunctionType
 ) -> None:
     """Replay the st element function calls that happened when executing a
     cache-decorated function.
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/credentials.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/fragment.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/fragment.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     elements are redrawn on each full-script rerun. The rest of the app is
     persisted during a fragment rerun. When a fragment renders elements into
     externally created containers, the elements will not be cleared with each
     fragment rerun. In this case, elements will accumulate in those containers
     with each fragment rerun, until the next full-script rerun.
 
     Calling `st.sidebar` in a fragment is not supported. To write elements to
-    the sidebar with a fragment, call your fragment funciton inside a
+    the sidebar with a fragment, call your fragment function inside a
     `with st.sidebar` context manager.
 
     Fragment code can interact with Session State, imported modules, and
     other Streamlit elements created outside the fragment. Note that these
     interactions are additive across multiple fragment reruns. You are
     responsible for handling any side effects of that behavior.
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/legacy_caching/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from streamlit.runtime.legacy_caching.caching import (
-    cache,
-    clear_cache,
-    get_cache_path,
-    maybe_show_cached_st_function_warning,
+
+from streamlit.watcher.local_sources_watcher import LocalSourcesWatcher
+from streamlit.watcher.path_watcher import (
+    report_watchdog_availability,
+    watch_dir,
+    watch_file,
 )
 
 __all__ = [
-    "cache",
-    "clear_cache",
-    "get_cache_path",
-    "maybe_show_cached_st_function_warning",
+    "LocalSourcesWatcher",
+    "report_watchdog_availability",
+    "watch_dir",
+    "watch_file",
 ]
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/legacy_caching/caching.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/legacy_caching/caching.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,15 +232,14 @@
 
 
 # A thread-local counter that's incremented when we enter @st.cache
 # and decremented when we exit.
 class ThreadLocalCacheInfo(threading.local):
     def __init__(self):
         self.cached_func_stack: list[Callable[..., Any]] = []
-        self.suppress_st_function_warning = 0
 
     def __repr__(self) -> str:
         return util.repr_(self)
 
 
 _cache_info = ThreadLocalCacheInfo()
 
@@ -250,62 +249,14 @@
     _cache_info.cached_func_stack.append(func)
     try:
         yield
     finally:
         _cache_info.cached_func_stack.pop()
 
 
-@contextlib.contextmanager
-def suppress_cached_st_function_warning() -> Iterator[None]:
-    _cache_info.suppress_st_function_warning += 1
-    try:
-        yield
-    finally:
-        _cache_info.suppress_st_function_warning -= 1
-        assert _cache_info.suppress_st_function_warning >= 0
-
-
-def _show_cached_st_function_warning(
-    dg: st.delta_generator.DeltaGenerator,
-    st_func_name: str,
-    cached_func: Callable[..., Any],
-) -> None:
-    # Avoid infinite recursion by suppressing additional cached
-    # function warnings from within the cached function warning.
-    with suppress_cached_st_function_warning():
-        e = CachedStFunctionWarning(st_func_name, cached_func)
-        dg.exception(e)
-
-
-def maybe_show_cached_st_function_warning(
-    dg: st.delta_generator.DeltaGenerator, st_func_name: str
-) -> None:
-    """If appropriate, warn about calling st.foo inside @cache.
-
-    DeltaGenerator's @_with_element and @_widget wrappers use this to warn
-    the user when they're calling st.foo() from within a function that is
-    wrapped in @st.cache.
-
-    Parameters
-    ----------
-    dg : DeltaGenerator
-        The DeltaGenerator to publish the warning to.
-
-    st_func_name : str
-        The name of the Streamlit function that was called.
-
-    """
-    if (
-        len(_cache_info.cached_func_stack) > 0
-        and _cache_info.suppress_st_function_warning <= 0
-    ):
-        cached_func = _cache_info.cached_func_stack[-1]
-        _show_cached_st_function_warning(dg, st_func_name, cached_func)
-
-
 def _read_from_mem_cache(
     mem_cache: MemCache,
     key: str,
     allow_output_mutation: bool,
     func_or_code: Callable[..., Any],
     hash_funcs: HashFuncsDict | None,
 ) -> Any:
@@ -679,19 +630,15 @@
                 )
                 _LOGGER.debug("Cache hit: %s", non_optional_func)
 
             except CacheKeyNotFoundError:
                 _LOGGER.debug("Cache miss: %s", non_optional_func)
 
                 with _calling_cached_function(non_optional_func):
-                    if suppress_st_warning:
-                        with suppress_cached_st_function_warning():
-                            return_value = non_optional_func(*args, **kwargs)
-                    else:
-                        return_value = non_optional_func(*args, **kwargs)
+                    return_value = non_optional_func(*args, **kwargs)
 
                 _write_to_cache(
                     mem_cache=mem_cache,
                     key=value_key,
                     value=return_value,
                     persist=persist,
                     allow_output_mutation=allow_output_mutation,
@@ -822,40 +769,14 @@
         else:
             self.cached_func_name = _get_cached_func_name_md(func_or_code)
 
     def __repr__(self) -> str:
         return util.repr_(self)
 
 
-class CachedStFunctionWarning(StreamlitAPIWarning):
-    def __init__(self, st_func_name, cached_func):
-        msg = self._get_message(st_func_name, cached_func)
-        super().__init__(msg)
-
-    def _get_message(self, st_func_name, cached_func):
-        args = {
-            "st_func_name": "`st.%s()` or `st.write()`" % st_func_name,
-            "func_name": _get_cached_func_name_md(cached_func),
-        }
-
-        return (
-            """
-Your script uses %(st_func_name)s to write to your Streamlit app from within
-some cached code at %(func_name)s. This code will only be called when we detect
-a cache "miss", which can lead to unexpected results.
-
-How to fix this:
-* Move the %(st_func_name)s call outside %(func_name)s.
-* Or, if you know what you're doing, use `@st.cache(suppress_st_warning=True)`
-to suppress the warning.
-            """
-            % args
-        ).strip("\n")
-
-
 class CachedObjectMutationWarning(StreamlitAPIWarning):
     def __init__(self, orig_exc):
         msg = self._get_message(orig_exc)
         super().__init__(msg)
 
     def _get_message(self, orig_exc):
         return (
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/legacy_caching/hashing.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/runtime.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/script_data.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,17 @@
     form_ids_this_run: set[str] = field(default_factory=set)
     cursors: dict[int, "streamlit.cursor.RunningCursor"] = field(default_factory=dict)
     script_requests: ScriptRequests | None = None
     current_fragment_id: str | None = None
     fragment_ids_this_run: set[str] | None = None
     # we allow only one dialog to be open at the same time
     has_dialog_opened: bool = False
+    # If true, it indicates that we are in a cached function that disallows
+    # the usage of widgets.
+    disallow_cached_widget_usage: bool = False
 
     # TODO(willhuang1997): Remove this variable when experimental query params are removed
     _experimental_query_params_used = False
     _production_query_params_used = False
 
     def reset(
         self,
@@ -101,14 +104,15 @@
         self._has_script_started = False
         self.command_tracking_deactivated: bool = False
         self.tracked_commands = []
         self.tracked_commands_counter = collections.Counter()
         self.current_fragment_id = None
         self.fragment_ids_this_run = fragment_ids_this_run
         self.has_dialog_opened = False
+        self.disallow_cached_widget_usage = False
 
         parsed_query_params = parse.parse_qs(query_string, keep_blank_values=True)
         with self.session_state.query_params() as qp:
             qp.clear_with_no_forward_msg()
             for key, val in parsed_query_params.items():
                 if len(val) == 0:
                     qp.set_with_no_forward_msg(key, val="")
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/secrets.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/common.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/stats.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/source_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/asset-manifest.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8291666666666666%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.f215a056.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.f215a056.js', 'static/js/43.05a14cc7.chunk.js': "*

 * *            "'./static/js/43.05a14cc7.chunk.js', delete: ['static/js/43.9ae03282.chunk.js']}"}*

```diff
@@ -1,16 +1,16 @@
 {
     "entrypoints": [
         "static/css/main.bf304093.css",
-        "static/js/main.713dd29d.js"
+        "static/js/main.f215a056.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.bf304093.css",
-        "main.js": "./static/js/main.713dd29d.js",
+        "main.js": "./static/js/main.f215a056.js",
         "static/css/2411.8b8f33d6.chunk.css": "./static/css/2411.8b8f33d6.chunk.css",
         "static/css/3092.95a45cfe.chunk.css": "./static/css/3092.95a45cfe.chunk.css",
         "static/css/43.e3b876c5.chunk.css": "./static/css/43.e3b876c5.chunk.css",
         "static/js/1074.73973756.chunk.js": "./static/js/1074.73973756.chunk.js",
         "static/js/1168.1d6408e6.chunk.js": "./static/js/1168.1d6408e6.chunk.js",
         "static/js/1307.8ea033f1.chunk.js": "./static/js/1307.8ea033f1.chunk.js",
         "static/js/1451.3b0a3e31.chunk.js": "./static/js/1451.3b0a3e31.chunk.js",
@@ -29,15 +29,15 @@
         "static/js/3631.be5c35fa.chunk.js": "./static/js/3631.be5c35fa.chunk.js",
         "static/js/3998.01237fcf.chunk.js": "./static/js/3998.01237fcf.chunk.js",
         "static/js/4113.1e7eff4d.chunk.js": "./static/js/4113.1e7eff4d.chunk.js",
         "static/js/4132.49bf3f2c.chunk.js": "./static/js/4132.49bf3f2c.chunk.js",
         "static/js/4177.69f9f18d.chunk.js": "./static/js/4177.69f9f18d.chunk.js",
         "static/js/4185.935c68ec.chunk.js": "./static/js/4185.935c68ec.chunk.js",
         "static/js/4253.749d5244.chunk.js": "./static/js/4253.749d5244.chunk.js",
-        "static/js/43.9ae03282.chunk.js": "./static/js/43.9ae03282.chunk.js",
+        "static/js/43.05a14cc7.chunk.js": "./static/js/43.05a14cc7.chunk.js",
         "static/js/4319.a6745434.chunk.js": "./static/js/4319.a6745434.chunk.js",
         "static/js/4477.e10e4373.chunk.js": "./static/js/4477.e10e4373.chunk.js",
         "static/js/4500.b6f348d1.chunk.js": "./static/js/4500.b6f348d1.chunk.js",
         "static/js/4666.492dcf72.chunk.js": "./static/js/4666.492dcf72.chunk.js",
         "static/js/474.87506447.chunk.js": "./static/js/474.87506447.chunk.js",
         "static/js/5106.44f0ff51.chunk.js": "./static/js/5106.44f0ff51.chunk.js",
         "static/js/5117.04bfe5d3.chunk.js": "./static/js/5117.04bfe5d3.chunk.js",
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/favicon.png` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/index.html` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.713dd29d.js"></script><link href="./static/css/main.bf304093.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.f215a056.js"></script><link href="./static/css/main.bf304093.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/css/2411.8b8f33d6.chunk.css` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/css/2411.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/css/3092.95a45cfe.chunk.css` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/css/3092.95a45cfe.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/css/43.e3b876c5.chunk.css` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/css/43.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/css/main.bf304093.css` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/css/main.bf304093.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1168.1d6408e6.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1168.1d6408e6.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1307.8ea033f1.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1307.8ea033f1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/178.b5384fd0.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/178.b5384fd0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/1792.b8efa879.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/1792.b8efa879.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2411.a8823789.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2411.a8823789.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2469.3e9c3ce9.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2469.3e9c3ce9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2736.914069e5.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2736.914069e5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/2736.914069e5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3092.152fd2b7.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3092.152fd2b7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3513.e3e7300a.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3513.e3e7300a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3631.be5c35fa.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3631.be5c35fa.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/3998.01237fcf.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/3998.01237fcf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4113.1e7eff4d.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4113.1e7eff4d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4185.935c68ec.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4185.935c68ec.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4253.749d5244.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4253.749d5244.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/43.9ae03282.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/43.05a14cc7.chunk.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -135,17 +135,21 @@
                 };
                 return t ? f()({}, o, t, ((t, e) => Array.isArray(e) ? e : void 0)) : o
             }
             const y = (0, o(1515).Z)("div", {
                 target: "egd2k5h0"
             })((t => {
                 let {
-                    theme: e
+                    theme: e,
+                    useContainerWidth: o,
+                    isFullScreen: n
                 } = t;
                 return {
+                    width: o || n ? "100%" : "auto",
+                    height: n ? "100%" : "auto",
                     "&.vega-embed": {
                         "&:hover summary, .vega-embed:focus summary": {
                             background: "transparent"
                         },
                         "&.has-actions": {
                             paddingRight: 0
                         },
@@ -206,19 +210,22 @@
                         error: void 0
                     }, this.finalizeView = () => {
                         this.vegaFinalizer && this.vegaFinalizer(), this.vegaFinalizer = void 0, this.vegaView = void 0
                     }, this.generateSpec = () => {
                         var t, e;
                         const {
                             element: o,
-                            theme: n
-                        } = this.props, i = JSON.parse(o.spec), {
-                            useContainerWidth: a
+                            theme: n,
+                            isFullScreen: i,
+                            width: a,
+                            height: s
+                        } = this.props, r = JSON.parse(o.spec), {
+                            useContainerWidth: l
                         } = o;
-                        if ("streamlit" === o.vegaLiteTheme ? i.config = b(i.config, n) : "streamlit" === (null === (t = i.usermeta) || void 0 === t || null === (e = t.embedOptions) || void 0 === e ? void 0 : e.theme) ? (i.config = b(i.config, n), i.usermeta.embedOptions.theme = void 0) : i.config = function(t, e) {
+                        if ("streamlit" === o.vegaLiteTheme ? r.config = b(r.config, n) : "streamlit" === (null === (t = r.usermeta) || void 0 === t || null === (e = t.embedOptions) || void 0 === e ? void 0 : e.theme) ? (r.config = b(r.config, n), r.usermeta.embedOptions.theme = void 0) : r.config = function(t, e) {
                                 const {
                                     colors: o,
                                     fontSizes: n,
                                     genericFonts: i
                                 } = e, a = {
                                     labelFont: i.bodyFont,
                                     titleFont: i.bodyFont,
@@ -253,16 +260,20 @@
                                         continuousWidth: 400
                                     },
                                     mark: {
                                         tooltip: !0
                                     }
                                 };
                                 return t ? u()({}, s, t) : s
-                            }(i.config, n), this.props.height ? (i.width = this.props.width, i.height = this.props.height) : a && (i.width = this.props.width), i.padding || (i.padding = {}), null == i.padding.bottom && (i.padding.bottom = 20), i.datasets) throw new Error("Datasets should not be passed as part of the spec");
-                        return i
+                            }(r.config, n), i ? (r.width = a, r.height = s, "vconcat" in r && r.vconcat.forEach((t => {
+                                t.width = a
+                            }))) : l && (r.width = a, "vconcat" in r && r.vconcat.forEach((t => {
+                                t.width = a
+                            }))), r.padding || (r.padding = {}), null == r.padding.bottom && (r.padding.bottom = 20), r.datasets) throw new Error("Datasets should not be passed as part of the spec");
+                        return r
                     }
                 }
                 async componentDidMount() {
                     try {
                         await this.createView()
                     } catch (t) {
                         const e = (0, c.b)(t);
@@ -379,14 +390,16 @@
                         for (const [a, r] of Object.entries(d)) i.insert(a, r);
                     await i.runAsync(), this.vegaView.resize().runAsync()
                 }
                 render() {
                     if (this.state.error) throw this.state.error;
                     return (0, w.jsx)(y, {
                         "data-testid": "stArrowVegaLiteChart",
+                        useContainerWidth: this.props.element.useContainerWidth,
+                        isFullScreen: this.props.isFullScreen,
                         ref: t => {
                             this.element = t
                         }
                     })
                 }
             }
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4319.a6745434.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4319.a6745434.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4477.e10e4373.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4477.e10e4373.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/4666.492dcf72.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/4666.492dcf72.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/474.87506447.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/474.87506447.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5345.65c91ee7.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5345.65c91ee7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6013.8e80e091.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6013.8e80e091.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6150.1294fa0d.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6150.1294fa0d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/656.ae85f8f1.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/656.ae85f8f1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/6853.d999ac75.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/6853.d999ac75.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7217.d970c074.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7217.d970c074.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7323.2808d029.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7323.2808d029.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7323.2808d029.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7602.6175e969.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7602.6175e969.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/7805.51638fbc.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/7805.51638fbc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8427.d30dffe1.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8427.d30dffe1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8477.e948c092.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8477.e948c092.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8492.f56c9d4c.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8492.f56c9d4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9330.d29313d4.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9330.d29313d4.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9336.2d95d840.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9336.2d95d840.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9758.6e6d8662.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9758.6e6d8662.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/main.713dd29d.js` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/main.f215a056.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.713dd29d.js.LICENSE.txt */
+/*! For license information please see main.f215a056.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
             68785: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     B: () => i,
                     Id: () => r,
@@ -115558,15 +115558,15 @@
         }
     })(), __webpack_require__.d = (e, t) => {
         for (var n in t) __webpack_require__.o(t, n) && !__webpack_require__.o(e, n) && Object.defineProperty(e, n, {
             enumerable: !0,
             get: t[n]
         })
     }, __webpack_require__.f = {}, __webpack_require__.e = e => Promise.all(Object.keys(__webpack_require__.f).reduce(((t, n) => (__webpack_require__.f[n](e, t), t)), [])), __webpack_require__.u = e => "static/js/" + e + "." + {
-        43: "9ae03282",
+        43: "05a14cc7",
         178: "b5384fd0",
         474: "87506447",
         656: "ae85f8f1",
         937: "a1248039",
         1074: "73973756",
         1168: "1d6408e6",
         1307: "8ea033f1",
@@ -116466,15 +116466,15 @@
             }, t.createElement(we.Z, {
                 theme: o
             }, n)))
         };
         var qe = __webpack_require__(17715),
             Ee = __webpack_require__(25621),
             _e = __webpack_require__(35704);
-        const xe = e => (0, Oe.iv)("a,a:visited{color:", e.colors.primary, ";}html{font-size:", e.fontSizes.mdPx, "px;}a:hover,a:active{color:", e.colors.primary, ";text-decoration:underline;}iframe{border:none;padding:0;margin:0;}code{padding:0.2em 0.4em;margin:0;border-radius:", e.radii.md, ";background:", e.colors.codeHighlightColor, ";color:", e.colors.codeTextColor, ";}pre{margin:0 0 1rem 0;background:", e.colors.codeHighlightColor, ";border-radius:", e.radii.md, ";padding:1rem;code{background:transparent;border:0;display:inline;font-size:", e.fontSizes.sm, ";line-height:inherit;margin:0;padding:0;white-space:pre;word-break:normal;word-wrap:normal;overflow-x:auto;color:", e.colors.codeTextColor, ";}}.disabled{color:", e.colors.disabled, ";}#vg-tooltip-element{font-family:", e.genericFonts.bodyFont, ";color:", e.colors.bodyText, ";border:1px solid ", e.colors.fadedText10, ";background-color:", (0, _e.DZ)(e.colors.bgColor, .05), ";font-size:", e.fontSizes.sm, ";box-shadow:rgb(0 0 0 / 16%) 0px 1px 4px;padding:", e.spacing.xs, " ", e.spacing.md, ";border-radius:", e.radii.md, ";z-index:", e.zIndices.fullscreenWrapper, ";}#vg-tooltip-element td{border:none;}#vg-tooltip-element table tr td.key{color:", e.colors.fadedText60, ";white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}body.embedded{overflow:hidden;}body.embedded:hover{overflow:auto;}*,*::before,*::after{box-sizing:border-box;}body{margin:0;font-family:", e.genericFonts.bodyFont, ";font-weight:", e.fontWeights.normal, ";line-height:", e.lineHeights.base, ";color:", e.colors.bodyText, ";background-color:", e.colors.bgColor, ";-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:", (0, _e.DZ)(e.colors.black, 1), ';-webkit-font-smoothing:auto;}[tabindex="-1"]:focus:not(:focus-visible){outline:0!important;}hr{margin:2em 0;padding:0;color:inherit;background-color:transparent;border:none;border-bottom:1px solid ', e.colors.fadedText10, ";}hr:not([size]){height:1px;}h1{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.extrabold, ";color:", e.colors.headingColor, ";padding:1.25rem 0 1rem 0;margin:0;line-height:1.2;}h2{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";letter-spacing:-0.005em;padding:1rem 0 1rem 0;margin:0;line-height:1.2;}h3{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";letter-spacing:-0.005em;padding:0.5rem 0 1rem 0;margin:0;line-height:1.2;}h4{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";padding:0.75rem 0 1rem 0;margin:0;line-height:1.2;}h5{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";padding:0 0 1rem 0;margin:0;line-height:1.2;}h6{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";padding:0 0 1rem 0;margin:0;line-height:1.2;}abbr[title],abbr[data-original-title]{text-decoration:underline;text-decoration:underline dotted;cursor:help;text-decoration-skip-ink:none;}address{margin-bottom:1rem;font-style:normal;line-height:inherit;}p,ol,ul,dl{margin:0 0 1rem 0;padding:0;font-size:1rem;font-weight:400;}ol ol,ul ul,ol ul,ul ol{margin-bottom:0;}dt{font-size:1rem;font-weight:600;margin:1em 0 0.2em 0;padding:0;}dd{margin:0 0 0.2em 1.2em;font-size:1rem;}b,strong{font-weight:", e.fontWeights.bold, ";}mark{padding:0.2em;background-color:", e.colors.secondaryBg, ";}sub,sup{position:relative;line-height:0;vertical-align:baseline;}sub{bottom:-0.25em;}sup{top:-0.5em;}a{color:", e.colors.primary, ";text-decoration:underline;&:hover{color:", (0, _e._j)(e.colors.primary, .15), ";}}a:not([href]):not([class]){&,&:hover{color:inherit;text-decoration:none;}}pre,code,kbd{font-family:", e.genericFonts.codeFont, ";}samp{font-family:", e.genericFonts.codeFont, ";}samp,blockquote{margin:1em 0 1em -1px;padding:0 0 0 1.2em;font-size:1rem;border-left:1px solid ", e.colors.lightGray, ";}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;color:", (0, _e.XV)(e.colors.bgColor), ";-ms-overflow-style:scrollbar;code{color:inherit;word-break:normal;}}code{color:", e.colors.codeTextColor, ";word-wrap:break-word;a>&{color:inherit;}}kbd{padding:0.2rem 0.4rem;color:", e.colors.codeTextColor, ";background-color:", e.colors.codeHighlightColor, ";kbd{padding:0;font-weight:", e.fontWeights.bold, ";}}figure{margin:0 0 1rem;}img,svg{vertical-align:middle;}table{caption-side:bottom;border-collapse:collapse;}table caption{padding-top:", e.spacing.sm, ";padding-bottom:0;color:", e.colors.gray60, ';text-align:left;}th{text-align:inherit;text-align:-webkit-match-parent;}thead,tbody,tfoot,tr,td,th{border-color:inherit;border-style:solid;border-width:0;}label{display:inline-block;}button{border-radius:0;}button:focus{outline:1px dotted;outline:5px auto -webkit-focus-ring-color;}input,button,select,optgroup,textarea{margin:0;font-family:inherit;line-height:inherit;}button,input{overflow:visible;}button,select{text-transform:none;}[role="button"]{cursor:pointer;}select{word-wrap:normal;}[list]::-webkit-calendar-picker-indicator{display:none;}button,[type="button"],[type="reset"],[type="submit"]{-webkit-appearance:button;}::-moz-focus-inner{padding:0;border-style:none;}textarea{resize:vertical;}fieldset{min-width:0;padding:0;margin:0;border:0;}legend{float:left;width:100%;padding:0;margin-bottom:', e.spacing.sm, ';line-height:inherit;white-space:normal;+*{clear:left;}}::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-text,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-year-field{padding:0;}::-webkit-inner-spin-button{height:auto;}[type="search"]{outline-offset:-2px;-webkit-appearance:textfield;}::-webkit-search-decoration{-webkit-appearance:none;}::-webkit-color-swatch-wrapper{padding:0;}::-webkit-file-upload-button{font:inherit;-webkit-appearance:button;}output{display:inline-block;}iframe{border:0;}summary{display:list-item;cursor:pointer;}progress{vertical-align:baseline;}[hidden]{display:none!important;}::-webkit-scrollbar{background:transparent;border-radius:100px;height:6px;width:6px;}::-webkit-scrollbar:active{background:', e.colors.fadedText10, ";}:hover::-webkit-scrollbar-thumb:vertical,:hover::-webkit-scrollbar-thumb:horizontal{background:", e.colors.fadedText40, ";border-radius:100px;}", "");
+        const xe = e => (0, Oe.iv)("a,a:visited{color:", e.colors.primary, ";}html{font-size:", e.fontSizes.mdPx, "px;}@media print{html{height:100%;print-color-adjust:exact;-webkit-print-color-adjust:exact;}}a:hover,a:active{color:", e.colors.primary, ";text-decoration:underline;}iframe{border:none;padding:0;margin:0;}code{padding:0.2em 0.4em;margin:0;border-radius:", e.radii.md, ";background:", e.colors.codeHighlightColor, ";color:", e.colors.codeTextColor, ";}pre{margin:0 0 1rem 0;background:", e.colors.codeHighlightColor, ";border-radius:", e.radii.md, ";padding:1rem;code{background:transparent;border:0;display:inline;font-size:", e.fontSizes.sm, ";line-height:inherit;margin:0;padding:0;white-space:pre;word-break:normal;word-wrap:normal;overflow-x:auto;color:", e.colors.codeTextColor, ";}}.disabled{color:", e.colors.disabled, ";}#vg-tooltip-element{font-family:", e.genericFonts.bodyFont, ";color:", e.colors.bodyText, ";border:1px solid ", e.colors.fadedText10, ";background-color:", (0, _e.DZ)(e.colors.bgColor, .05), ";font-size:", e.fontSizes.sm, ";box-shadow:rgb(0 0 0 / 16%) 0px 1px 4px;padding:", e.spacing.xs, " ", e.spacing.md, ";border-radius:", e.radii.md, ";z-index:", e.zIndices.fullscreenWrapper, ";}#vg-tooltip-element td{border:none;}#vg-tooltip-element table tr td.key{color:", e.colors.fadedText60, ";white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}body.embedded{overflow:hidden;}body.embedded:hover{overflow:auto;}*,*::before,*::after{box-sizing:border-box;}body{margin:0;font-family:", e.genericFonts.bodyFont, ";font-weight:", e.fontWeights.normal, ";line-height:", e.lineHeights.base, ";color:", e.colors.bodyText, ";background-color:", e.colors.bgColor, ";-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:", (0, _e.DZ)(e.colors.black, 1), ';-webkit-font-smoothing:auto;}[tabindex="-1"]:focus:not(:focus-visible){outline:0!important;}hr{margin:2em 0;padding:0;color:inherit;background-color:transparent;border:none;border-bottom:1px solid ', e.colors.fadedText10, ";}hr:not([size]){height:1px;}h1{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.extrabold, ";color:", e.colors.headingColor, ";padding:1.25rem 0 1rem 0;margin:0;line-height:1.2;}h2{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";letter-spacing:-0.005em;padding:1rem 0 1rem 0;margin:0;line-height:1.2;}h3{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";letter-spacing:-0.005em;padding:0.5rem 0 1rem 0;margin:0;line-height:1.2;}h4{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";padding:0.75rem 0 1rem 0;margin:0;line-height:1.2;}h5{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";padding:0 0 1rem 0;margin:0;line-height:1.2;}h6{font-family:", e.genericFonts.headingFont, ";font-weight:", e.fontWeights.bold, ";color:", e.colors.headingColor, ";padding:0 0 1rem 0;margin:0;line-height:1.2;}abbr[title],abbr[data-original-title]{text-decoration:underline;text-decoration:underline dotted;cursor:help;text-decoration-skip-ink:none;}address{margin-bottom:1rem;font-style:normal;line-height:inherit;}p,ol,ul,dl{margin:0 0 1rem 0;padding:0;font-size:1rem;font-weight:400;}ol ol,ul ul,ol ul,ul ol{margin-bottom:0;}dt{font-size:1rem;font-weight:600;margin:1em 0 0.2em 0;padding:0;}dd{margin:0 0 0.2em 1.2em;font-size:1rem;}b,strong{font-weight:", e.fontWeights.bold, ";}mark{padding:0.2em;background-color:", e.colors.secondaryBg, ";}sub,sup{position:relative;line-height:0;vertical-align:baseline;}sub{bottom:-0.25em;}sup{top:-0.5em;}a{color:", e.colors.primary, ";text-decoration:underline;&:hover{color:", (0, _e._j)(e.colors.primary, .15), ";}}a:not([href]):not([class]){&,&:hover{color:inherit;text-decoration:none;}}pre,code,kbd{font-family:", e.genericFonts.codeFont, ";}samp{font-family:", e.genericFonts.codeFont, ";}samp,blockquote{margin:1em 0 1em -1px;padding:0 0 0 1.2em;font-size:1rem;border-left:1px solid ", e.colors.lightGray, ";}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;color:", (0, _e.XV)(e.colors.bgColor), ";-ms-overflow-style:scrollbar;code{color:inherit;word-break:normal;}}code{color:", e.colors.codeTextColor, ";word-wrap:break-word;a>&{color:inherit;}}kbd{padding:0.2rem 0.4rem;color:", e.colors.codeTextColor, ";background-color:", e.colors.codeHighlightColor, ";kbd{padding:0;font-weight:", e.fontWeights.bold, ";}}figure{margin:0 0 1rem;}img,svg{vertical-align:middle;}table{caption-side:bottom;border-collapse:collapse;}table caption{padding-top:", e.spacing.sm, ";padding-bottom:0;color:", e.colors.gray60, ';text-align:left;}th{text-align:inherit;text-align:-webkit-match-parent;}thead,tbody,tfoot,tr,td,th{border-color:inherit;border-style:solid;border-width:0;}label{display:inline-block;}button{border-radius:0;}button:focus{outline:1px dotted;outline:5px auto -webkit-focus-ring-color;}input,button,select,optgroup,textarea{margin:0;font-family:inherit;line-height:inherit;}button,input{overflow:visible;}button,select{text-transform:none;}[role="button"]{cursor:pointer;}select{word-wrap:normal;}[list]::-webkit-calendar-picker-indicator{display:none;}button,[type="button"],[type="reset"],[type="submit"]{-webkit-appearance:button;}::-moz-focus-inner{padding:0;border-style:none;}textarea{resize:vertical;}fieldset{min-width:0;padding:0;margin:0;border:0;}legend{float:left;width:100%;padding:0;margin-bottom:', e.spacing.sm, ';line-height:inherit;white-space:normal;+*{clear:left;}}::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-text,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-year-field{padding:0;}::-webkit-inner-spin-button{height:auto;}[type="search"]{outline-offset:-2px;-webkit-appearance:textfield;}::-webkit-search-decoration{-webkit-appearance:none;}::-webkit-color-swatch-wrapper{padding:0;}::-webkit-file-upload-button{font:inherit;-webkit-appearance:button;}output{display:inline-block;}iframe{border:0;}summary{display:list-item;cursor:pointer;}progress{vertical-align:baseline;}[hidden]{display:none!important;}::-webkit-scrollbar{background:transparent;border-radius:100px;height:6px;width:6px;}::-webkit-scrollbar:active{background:', e.colors.fadedText10, ";}:hover::-webkit-scrollbar-thumb:vertical,:hover::-webkit-scrollbar-thumb:horizontal{background:", e.colors.fadedText40, ";border-radius:100px;}", "");
         var Re;
         const Te = (null === (Re = document.currentScript) || void 0 === Re ? void 0 : Re.nonce) || "",
             ke = (0, qe.Z)({
                 key: "st-emotion-cache",
                 ...Te && {
                     nonce: Te
                 }
@@ -121326,21 +121326,18 @@
                     "&:focus": {
                         outline: "none"
                     },
                     ["@media (max-width: ".concat(t.breakpoints.md, ")")]: {
                         boxShadow: "-2rem 0 2rem 2rem ".concat(n ? "transparent" : "#00000029")
                     },
                     "@media print": {
-                        backgroundColor: "transparent",
-                        margin: "auto",
-                        boxShadow: "none",
-                        maxWidth: "none",
-                        minWidth: "100%",
-                        width: "100% !important",
-                        paddingTop: "1rem"
+                        display: n ? "none" : "initial",
+                        height: "auto !important",
+                        maxHeight: "99%",
+                        boxShadow: "none"
                     }
                 }
             }), ""),
             Ia = (0, Qe.Z)("div", {
                 target: "eczjsme10"
             })((() => ({
                 position: "relative"
@@ -121358,15 +121355,15 @@
                     maxHeight: r ? t ? "75vh" : "33vh" : "100vh",
                     listStyle: "none",
                     overflow: ["auto", "overlay"],
                     margin: 0,
                     paddingTop: o.sizes.sidebarTopSpace,
                     paddingBottom: o.spacing.lg,
                     "@media print": {
-                        paddingTop: o.spacing.sm
+                        paddingTop: o.spacing.threeXL
                     },
                     "&::before": n ? {
                         content: '" "',
                         backgroundImage: "linear-gradient(0deg, transparent, ".concat(o.colors.bgColor, ")"),
                         width: "100%",
                         height: "2rem",
                         position: "absolute",
@@ -121492,17 +121489,14 @@
                     theme: n
                 } = e;
                 return {
                     paddingTop: t ? n.spacing.lg : n.sizes.sidebarTopSpace,
                     paddingBottom: n.sizes.sidebarTopSpace,
                     paddingLeft: n.spacing.twoXL,
                     paddingRight: n.spacing.twoXL,
-                    "@media print": {
-                        paddingTop: "1rem"
-                    },
                     ...(0, ye.XE)(n)
                 }
             }), ""),
             Ha = (0, Qe.Z)("div", {
                 target: "eczjsme3"
             })((e => {
                 let {
@@ -121889,39 +121883,30 @@
                             }
                         }
                     }), r]
                 })
             },
             os = (0, Qe.Z)("div", {
                 target: "ea3mdgi9"
-            })((e => {
-                let {
-                    theme: t
-                } = e;
-                return {
-                    display: "flex",
-                    flexDirection: "row",
-                    justifyContent: "flex-start",
-                    alignItems: "stretch",
-                    alignContent: "flex-start",
-                    position: "absolute",
-                    top: 0,
-                    left: 0,
-                    right: 0,
-                    bottom: 0,
-                    overflow: "hidden",
-                    "@media print": {
-                        display: "block",
-                        float: "none",
-                        height: t.sizes.full,
-                        position: "static",
-                        overflow: "visible"
-                    }
+            })((() => ({
+                display: "flex",
+                flexDirection: "row",
+                justifyContent: "flex-start",
+                alignItems: "stretch",
+                alignContent: "flex-start",
+                position: "absolute",
+                top: 0,
+                left: 0,
+                right: 0,
+                bottom: 0,
+                overflow: "hidden",
+                "@media print": {
+                    overflow: "visible"
                 }
-            }), ""),
+            })), ""),
             is = (0, Qe.Z)("section", {
                 target: "ea3mdgi8"
             })((e => {
                 let {
                     disableScrolling: t,
                     theme: n
                 } = e;
@@ -121930,24 +121915,25 @@
                     flexDirection: "column",
                     width: n.sizes.full,
                     overflow: t ? "hidden" : "auto",
                     alignItems: "center",
                     "&:focus": {
                         outline: "none"
                     },
-                    ["@media (max-width: ".concat(n.breakpoints.md, ")")]: {
-                        position: "absolute",
-                        top: 0,
-                        left: 0,
-                        right: 0,
-                        bottom: 0
+                    "@media not print": {
+                        ["@media (max-width: ".concat(n.breakpoints.md, ")")]: {
+                            position: "absolute",
+                            top: 0,
+                            left: 0,
+                            right: 0,
+                            bottom: 0
+                        }
                     },
                     "@media print": {
-                        position: "relative",
-                        display: "block"
+                        overflow: "visible"
                     }
                 }
             }), ""),
             as = (0, Qe.Z)("div", {
                 target: "ea3mdgi7"
             })((() => ({
                 position: "sticky",
@@ -121981,39 +121967,40 @@
                     hasBottom: n,
                     isEmbedded: r,
                     isWideMode: o,
                     showPadding: i,
                     addPaddingForHeader: a,
                     disableFullscreenMode: s,
                     theme: l
-                } = e, c = i ? "6rem" : "2.1rem";
-                (a && !i || r && t) && (c = "3rem");
-                const u = i && !n ? "10rem" : l.spacing.lg,
-                    p = o ? "5rem" : l.spacing.lg,
-                    d = !o && !s ? {
+                } = e;
+                const c = "2.1rem";
+                let u = i ? "6rem" : c;
+                (a && !i || r && t) && (u = "3rem");
+                const p = i && !n ? "10rem" : l.spacing.lg,
+                    d = o ? "5rem" : l.spacing.lg,
+                    b = !o && !s ? {
                         "@media (max-width: 50.5rem)": {
                             maxWidth: "calc(100vw - 4.5rem)"
                         }
                     } : {};
                 return {
                     width: l.sizes.full,
                     paddingLeft: l.spacing.lg,
                     paddingRight: l.spacing.lg,
                     "@media (min-width: 576px)": {
-                        paddingLeft: p,
-                        paddingRight: p
+                        paddingLeft: d,
+                        paddingRight: d
                     },
-                    paddingTop: c,
-                    paddingBottom: u,
+                    paddingTop: u,
+                    paddingBottom: p,
                     minWidth: o ? "auto" : void 0,
                     maxWidth: o ? "initial" : l.sizes.contentMaxWidth,
-                    ...d,
+                    ...b,
                     "@media print": {
-                        minWidth: "100%",
-                        paddingTop: 0
+                        paddingTop: c
                     }
                 }
             }), ""),
             cs = (0, Qe.Z)("div", {
                 target: "ea3mdgi4"
             })((e => {
                 let {
@@ -122046,15 +122033,14 @@
                         paddingRight: o
                     },
                     paddingTop: r.spacing.lg,
                     paddingBottom: n ? "55px" : r.spacing.threeXL,
                     minWidth: t ? "auto" : void 0,
                     maxWidth: t ? "initial" : r.sizes.contentMaxWidth,
                     "@media print": {
-                        minWidth: "100%",
                         paddingTop: 0
                     }
                 }
             }), ""),
             ds = (0, Qe.Z)("div", {
                 target: "ea3mdgi1"
             })((e => {
@@ -123097,14 +123083,17 @@
                         borderBottomRightRadius: 0
                     },
                     "ul[role=listbox] ~ ul[role=listbox]": {
                         borderTopLeftRadius: 0,
                         borderTopRightRadius: 0,
                         boxShadow: "none",
                         borderTop: "none"
+                    },
+                    "@media print": {
+                        display: "none"
                     }
                 }
             }), ""),
             dl = (0, Qe.Z)("span", {
                 target: "e16jpq800"
             })((() => ({
                 lineHeight: "initial"
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/js/main.713dd29d.js.LICENSE.txt` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/js/main.f215a056.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.33.1.dev20240417/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/string_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/temporary_directory.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/testing/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/testing/v1/util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/time_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/type_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/url_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/user_info.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/version.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/watcher/util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/bootstrap.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/cli.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/__init__.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/routes.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/server.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/server_util.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.33.1.dev20240417/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.33.1.dev20240416
+Version: 1.33.1.dev20240417
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.33.1.dev20240417/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,15 @@
 streamlit/static/static/js/4113.1e7eff4d.chunk.js
 streamlit/static/static/js/4132.49bf3f2c.chunk.js
 streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
 streamlit/static/static/js/4177.69f9f18d.chunk.js
 streamlit/static/static/js/4185.935c68ec.chunk.js
 streamlit/static/static/js/4253.749d5244.chunk.js
 streamlit/static/static/js/4253.749d5244.chunk.js.LICENSE.txt
-streamlit/static/static/js/43.9ae03282.chunk.js
+streamlit/static/static/js/43.05a14cc7.chunk.js
 streamlit/static/static/js/4319.a6745434.chunk.js
 streamlit/static/static/js/4477.e10e4373.chunk.js
 streamlit/static/static/js/4500.b6f348d1.chunk.js
 streamlit/static/static/js/4666.492dcf72.chunk.js
 streamlit/static/static/js/474.87506447.chunk.js
 streamlit/static/static/js/5106.44f0ff51.chunk.js
 streamlit/static/static/js/5117.04bfe5d3.chunk.js
@@ -398,16 +398,16 @@
 streamlit/static/static/js/9330.d29313d4.chunk.js
 streamlit/static/static/js/9336.2d95d840.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
 streamlit/static/static/js/9656.8c935274.chunk.js
 streamlit/static/static/js/9758.6e6d8662.chunk.js
 streamlit/static/static/js/9865.fd93213d.chunk.js
-streamlit/static/static/js/main.713dd29d.js
-streamlit/static/static/js/main.713dd29d.js.LICENSE.txt
+streamlit/static/static/js/main.f215a056.js
+streamlit/static/static/js/main.f215a056.js.LICENSE.txt
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
```

### Comparing `streamlit_nightly-1.33.1.dev20240416/tests/testutil.py` & `streamlit_nightly-1.33.1.dev20240417/tests/testutil.py`

 * *Files identical despite different names*

