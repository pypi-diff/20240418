# Comparing `tmp/engineai_sdk-0.83.1.tar.gz` & `tmp/engineai_sdk-0.86.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engineai_sdk-0.83.1.tar", max compression
+gzip compressed data, was "engineai_sdk-0.86.1.tar", max compression
```

## Comparing `engineai_sdk-0.83.1.tar` & `engineai_sdk-0.86.1.tar`

### file list

```diff
@@ -1,380 +1,366 @@
--rw-r--r--   0        0        0     1065 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/LICENSE
--rw-r--r--   0        0        0      987 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/README.md
--rw-r--r--   0        0        0      435 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/__init__.py
--rw-r--r--   0        0        0       28 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/__init__.py
--rw-r--r--   0        0        0       33 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/commands/__init__.py
--rw-r--r--   0        0        0     2541 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/commands/app.py
--rw-r--r--   0        0        0    14446 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/commands/dashboard.py
--rw-r--r--   0        0        0     1379 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/console.py
--rw-r--r--   0        0        0     5489 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/generator.py
--rw-r--r--   0        0        0       42 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/template/content/.env.sample
--rw-r--r--   0        0        0      911 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/template/content/main.py
--rw-r--r--   0        0        0     2676 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_dividends.csv
--rw-r--r--   0        0        0      593 2024-04-09 13:47:43.223949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_earnings.csv
--rw-r--r--   0        0        0   152608 2024-04-09 13:47:43.227949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_history.csv
--rw-r--r--   0        0        0     7518 2024-04-09 13:47:43.227949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AAPL_info.json
--rw-r--r--   0        0        0     7217 2024-04-09 13:47:43.227949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/AMZN_info.json
--rw-r--r--   0        0        0   139522 2024-04-09 13:47:43.227949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/GSPC.csv
--rw-r--r--   0        0        0   135696 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/IXIC.csv
--rw-r--r--   0        0        0     8115 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_dividends.csv
--rw-r--r--   0        0        0      581 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_earnings.csv
--rw-r--r--   0        0        0   152152 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_history.csv
--rw-r--r--   0        0        0     8122 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JNJ_info.json
--rw-r--r--   0        0        0     5125 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_dividends.csv
--rw-r--r--   0        0        0      571 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_earnings.csv
--rw-r--r--   0        0        0   151607 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_history.csv
--rw-r--r--   0        0        0     8080 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/JPM_info.json
--rw-r--r--   0        0        0     2425 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_dividends.csv
--rw-r--r--   0        0        0      623 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_earnings.csv
--rw-r--r--   0        0        0   152489 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_history.csv
--rw-r--r--   0        0        0     8221 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/tutorial_data/MSFT_info.json
--rw-r--r--   0        0        0    10363 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/cli/utils.py
--rw-r--r--   0        0        0       38 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/__init__.py
--rw-r--r--   0        0        0      121 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/__init__.py
--rw-r--r--   0        0        0     2181 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/layout.py
--rw-r--r--   0        0        0      207 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/selectable_widgets.py
--rw-r--r--   0        0        0      570 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/typing.py
--rw-r--r--   0        0        0     1600 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/base.py
--rw-r--r--   0        0        0       96 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/__init__.py
--rw-r--r--   0        0        0     3574 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/activate_dashboard.py
--rw-r--r--   0        0        0     7670 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/api.py
--rw-r--r--   0        0        0     1451 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/exceptions.py
--rw-r--r--   0        0        0      217 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/__init__.py
--rw-r--r--   0        0        0      472 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/py.typed
--rw-r--r--   0        0        0      207 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/__init__.py
--rw-r--r--   0        0        0     6861 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py
--rw-r--r--   0        0        0     3134 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/json.py
--rw-r--r--   0        0        0     4618 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/storage.py
--rw-r--r--   0        0        0      515 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/config.py
--rw-r--r--   0        0        0      310 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/__init__.py
--rw-r--r--   0        0        0    13152 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/dashboard.py
--rw-r--r--   0        0        0      140 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/enums.py
--rw-r--r--   0        0        0     4691 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/exceptions.py
--rw-r--r--   0        0        0       27 2024-04-09 13:47:43.231949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/__init__.py
--rw-r--r--   0        0        0     2417 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/executor_config.py
--rw-r--r--   0        0        0     8389 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/instance.py
--rw-r--r--   0        0        0     1231 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/node.py
--rw-r--r--   0        0        0     2586 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/utils.py
--rw-r--r--   0        0        0       41 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/__init__.py
--rw-r--r--   0        0        0     1431 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/dependency.py
--rw-r--r--   0        0        0     5634 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/page.py
--rw-r--r--   0        0        0     1909 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/root.py
--rw-r--r--   0        0        0     2932 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/route.py
--rw-r--r--   0        0        0      345 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/typings.py
--rw-r--r--   0        0        0       33 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/version/__init__.py
--rw-r--r--   0        0        0     5105 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/version/version.py
--rw-r--r--   0        0        0      185 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/__init__.py
--rw-r--r--   0        0        0    12893 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/decorator.py
--rw-r--r--   0        0        0     1822 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/duplicated.py
--rw-r--r--   0        0        0     1047 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/enums.py
--rw-r--r--   0        0        0     4676 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/exceptions.py
--rw-r--r--   0        0        0     1996 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/http.py
--rw-r--r--   0        0        0     3616 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/io_handler.py
--rw-r--r--   0        0        0     1306 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/manager/interface.py
--rw-r--r--   0        0        0     9994 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/data/manager/manager.py
--rw-r--r--   0        0        0     2892 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/decorator.py
--rw-r--r--   0        0        0      441 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/__init__.py
--rw-r--r--   0        0        0     3521 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/datastore.py
--rw-r--r--   0        0        0      141 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/http/__init__.py
--rw-r--r--   0        0        0      966 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/http/header.py
--rw-r--r--   0        0        0     2555 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/http/http.py
--rw-r--r--   0        0        0     2026 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/route.py
--rw-r--r--   0        0        0     2518 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/widget.py
--rw-r--r--   0        0        0      369 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/__init__.py
--rw-r--r--   0        0        0      934 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/align.py
--rw-r--r--   0        0        0      705 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/legend_position.py
--rw-r--r--   0        0        0     5156 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/exceptions.py
--rw-r--r--   0        0        0      569 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/__init__.py
--rw-r--r--   0        0        0     3688 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/axis.py
--rw-r--r--   0        0        0     1817 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/datetime.py
--rw-r--r--   0        0        0      661 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/exceptions.py
--rw-r--r--   0        0        0     1259 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/mapper.py
--rw-r--r--   0        0        0     5108 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/number.py
--rw-r--r--   0        0        0     1272 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/text.py
--rw-r--r--   0        0        0      331 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/typing.py
--rw-r--r--   0        0        0      985 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/validator.py
--rw-r--r--   0        0        0     1056 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/interface.py
--rw-r--r--   0        0        0      825 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/__init__.py
--rw-r--r--   0        0        0      417 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/build_item.py
--rw-r--r--   0        0        0       28 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/__init__.py
--rw-r--r--   0        0        0     5748 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/card.py
--rw-r--r--   0        0        0     2770 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/chip.py
--rw-r--r--   0        0        0     1533 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/header.py
--rw-r--r--   0        0        0       55 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/__init__.py
--rw-r--r--   0        0        0     2949 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/chip.py
--rw-r--r--   0        0        0     1806 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/header.py
--rw-r--r--   0        0        0     6529 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/section.py
--rw-r--r--   0        0        0     5782 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/column.py
--rw-r--r--   0        0        0     2679 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/chip.py
--rw-r--r--   0        0        0     2165 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/header.py
--rw-r--r--   0        0        0     2385 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/label.py
--rw-r--r--   0        0        0     4695 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/exceptions.py
--rw-r--r--   0        0        0       31 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/__init__.py
--rw-r--r--   0        0        0     5658 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py
--rw-r--r--   0        0        0     1697 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/items_build.py
--rw-r--r--   0        0        0     7107 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/grid.py
--rw-r--r--   0        0        0    10297 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/row.py
--rw-r--r--   0        0        0       36 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/__init__.py
--rw-r--r--   0        0        0     7582 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/base.py
--rw-r--r--   0        0        0     2171 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/exceptions.py
--rw-r--r--   0        0        0     4295 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/tab.py
--rw-r--r--   0        0        0      410 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/typings.py
--rw-r--r--   0        0        0      244 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/__init__.py
--rw-r--r--   0        0        0     6016 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/abstract.py
--rw-r--r--   0        0        0     2201 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/route_link.py
--rw-r--r--   0        0        0     2576 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/template_string_link.py
--rw-r--r--   0        0        0      202 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/typing.py
--rw-r--r--   0        0        0     1427 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/url.py
--rw-r--r--   0        0        0      934 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/widget_dependency.py
--rw-r--r--   0        0        0     3039 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/links/widget_field.py
--rw-r--r--   0        0        0        0 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/py.typed
--rw-r--r--   0        0        0     2020 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/selected.py
--rw-r--r--   0        0        0      100 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/__init__.py
--rw-r--r--   0        0        0      744 2024-04-09 13:47:43.235949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/__init__.py
--rw-r--r--   0        0        0     5773 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/default_specs.py
--rw-r--r--   0        0        0     6505 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/discrete_map.py
--rw-r--r--   0        0        0     1690 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/divergent.py
--rw-r--r--   0        0        0     3576 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/gradient.py
--rw-r--r--   0        0        0     5791 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/palette.py
--rw-r--r--   0        0        0      829 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/single.py
--rw-r--r--   0        0        0      946 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/spec.py
--rw-r--r--   0        0        0      277 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/typing.py
--rw-r--r--   0        0        0     3436 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/icons.py
--rw-r--r--   0        0        0     8298 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/templated_string.py
--rw-r--r--   0        0        0     3514 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/utils.py
--rw-r--r--   0        0        0       25 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/__init__.py
--rw-r--r--   0        0        0     8515 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/base.py
--rw-r--r--   0        0        0     2647 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/__init__.py
--rw-r--r--   0        0        0       44 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/__init__.py
--rw-r--r--   0        0        0     3566 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/base.py
--rw-r--r--   0        0        0      365 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/typing.py
--rw-r--r--   0        0        0     2149 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py
--rw-r--r--   0        0        0     5237 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py
--rw-r--r--   0        0        0     4417 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/cartesian.py
--rw-r--r--   0        0        0     4481 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/chart.py
--rw-r--r--   0        0        0     1468 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/exceptions.py
--rw-r--r--   0        0        0      987 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/legend.py
--rw-r--r--   0        0        0       45 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/__init__.py
--rw-r--r--   0        0        0     2640 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/area.py
--rw-r--r--   0        0        0     4026 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py
--rw-r--r--   0        0        0     7256 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/base.py
--rw-r--r--   0        0        0     5303 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py
--rw-r--r--   0        0        0     2660 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/column.py
--rw-r--r--   0        0        0     2640 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/line.py
--rw-r--r--   0        0        0     2679 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py
--rw-r--r--   0        0        0      573 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/typing.py
--rw-r--r--   0        0        0     4957 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/chart_utils.py
--rw-r--r--   0        0        0       39 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/__init__.py
--rw-r--r--   0        0        0       87 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/__init__.py
--rw-r--r--   0        0        0     2630 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/base.py
--rw-r--r--   0        0        0     1475 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py
--rw-r--r--   0        0        0     1910 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py
--rw-r--r--   0        0        0       47 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/__init__.py
--rw-r--r--   0        0        0       56 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/__init__.py
--rw-r--r--   0        0        0      416 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/__init__.py
--rw-r--r--   0        0        0      992 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py
--rw-r--r--   0        0        0     1506 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py
--rw-r--r--   0        0        0     1506 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py
--rw-r--r--   0        0        0     1117 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py
--rw-r--r--   0        0        0     2656 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py
--rw-r--r--   0        0        0      338 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/typing.py
--rw-r--r--   0        0        0      151 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/consts.py
--rw-r--r--   0        0        0     7162 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/exceptions.py
--rw-r--r--   0        0        0       25 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/__init__.py
--rw-r--r--   0        0        0     2787 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/base.py
--rw-r--r--   0        0        0       23 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/__init__.py
--rw-r--r--   0        0        0      955 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py
--rw-r--r--   0        0        0     2138 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py
--rw-r--r--   0        0        0      806 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py
--rw-r--r--   0        0        0      314 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/typing.py
--rw-r--r--   0        0        0      696 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py
--rw-r--r--   0        0        0     1339 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/area.py
--rw-r--r--   0        0        0     1373 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py
--rw-r--r--   0        0        0     4041 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/base.py
--rw-r--r--   0        0        0     3379 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py
--rw-r--r--   0        0        0     2977 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py
--rw-r--r--   0        0        0     1334 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/column.py
--rw-r--r--   0        0        0     1047 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py
--rw-r--r--   0        0        0     1342 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py
--rw-r--r--   0        0        0     3471 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/line.py
--rw-r--r--   0        0        0     1309 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/point.py
--rw-r--r--   0        0        0     1319 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py
--rw-r--r--   0        0        0      802 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py
--rw-r--r--   0        0        0      282 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/toolbar.py
--rw-r--r--   0        0        0      319 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/__init__.py
--rw-r--r--   0        0        0     3647 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py
--rw-r--r--   0        0        0     1292 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py
--rw-r--r--   0        0        0     1452 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py
--rw-r--r--   0        0        0      617 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py
--rw-r--r--   0        0        0     1102 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py
--rw-r--r--   0        0        0     1335 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py
--rw-r--r--   0        0        0     1407 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py
--rw-r--r--   0        0        0      647 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/typing.py
--rw-r--r--   0        0        0       29 2024-04-09 13:47:43.239949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/__init__.py
--rw-r--r--   0        0        0     1192 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/base.py
--rw-r--r--   0        0        0       35 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/__init__.py
--rw-r--r--   0        0        0      228 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/area.py
--rw-r--r--   0        0        0      236 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/column.py
--rw-r--r--   0        0        0      228 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/line.py
--rw-r--r--   0        0        0     1184 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py
--rw-r--r--   0        0        0      379 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/typing.py
--rw-r--r--   0        0        0      974 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py
--rw-r--r--   0        0        0       36 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/__init__.py
--rw-r--r--   0        0        0     1451 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py
--rw-r--r--   0        0        0      902 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py
--rw-r--r--   0        0        0      893 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py
--rw-r--r--   0        0        0      906 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py
--rw-r--r--   0        0        0     1263 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py
--rw-r--r--   0        0        0      339 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/typing.py
--rw-r--r--   0        0        0       34 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/__init__.py
--rw-r--r--   0        0        0      879 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py
--rw-r--r--   0        0        0     1388 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py
--rw-r--r--   0        0        0      943 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py
--rw-r--r--   0        0        0      903 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py
--rw-r--r--   0        0        0      331 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/typing.py
--rw-r--r--   0        0        0     1313 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py
--rw-r--r--   0        0        0     2014 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py
--rw-r--r--   0        0        0     2003 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py
--rw-r--r--   0        0        0      136 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/__init__.py
--rw-r--r--   0        0        0     2890 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/content.py
--rw-r--r--   0        0        0     1265 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/exceptions.py
--rw-r--r--   0        0        0      613 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/item.py
--rw-r--r--   0        0        0     1431 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/markdown.py
--rw-r--r--   0        0        0     3756 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/exceptions.py
--rw-r--r--   0        0        0      350 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/__init__.py
--rw-r--r--   0        0        0      768 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/enums.py
--rw-r--r--   0        0        0      980 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/exceptions.py
--rw-r--r--   0        0        0       25 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/__init__.py
--rw-r--r--   0        0        0     7581 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/base.py
--rw-r--r--   0        0        0     4086 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/geo.py
--rw-r--r--   0        0        0      973 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/legend.py
--rw-r--r--   0        0        0       42 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/__init__.py
--rw-r--r--   0        0        0     4882 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/numeric.py
--rw-r--r--   0        0        0      625 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/series.py
--rw-r--r--   0        0        0     2785 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/styling.py
--rw-r--r--   0        0        0     2113 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pandas_utils.py
--rw-r--r--   0        0        0      672 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/__init__.py
--rw-r--r--   0        0        0     1952 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/chart.py
--rw-r--r--   0        0        0      852 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/exceptions.py
--rw-r--r--   0        0        0      743 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/legend.py
--rw-r--r--   0        0        0     6161 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/pie.py
--rw-r--r--   0        0        0       35 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/__init__.py
--rw-r--r--   0        0        0     6044 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/base.py
--rw-r--r--   0        0        0     3201 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/country.py
--rw-r--r--   0        0        0     2932 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/series.py
--rw-r--r--   0        0        0     3082 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/styling.py
--rw-r--r--   0        0        0      165 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/typings.py
--rw-r--r--   0        0        0     2405 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/tooltip.py
--rw-r--r--   0        0        0      391 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/__init__.py
--rw-r--r--   0        0        0     3415 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/__init__.py
--rw-r--r--   0        0        0     2793 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/base.py
--rw-r--r--   0        0        0      900 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/build_result.py
--rw-r--r--   0        0        0     3346 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/number.py
--rw-r--r--   0        0        0       21 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/__init__.py
--rw-r--r--   0        0        0     3252 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py
--rw-r--r--   0        0        0     1420 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/number.py
--rw-r--r--   0        0        0     1611 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/text.py
--rw-r--r--   0        0        0     2305 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/text.py
--rw-r--r--   0        0        0      280 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/typing.py
--rw-r--r--   0        0        0     7989 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/search.py
--rw-r--r--   0        0        0       79 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/exceptions.py
--rw-r--r--   0        0        0     1783 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/group.py
--rw-r--r--   0        0        0     6345 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/select.py
--rw-r--r--   0        0        0     2453 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/__init__.py
--rw-r--r--   0        0        0       50 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/__init__.py
--rw-r--r--   0        0        0       26 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/__init__.py
--rw-r--r--   0        0        0     6147 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/base.py
--rw-r--r--   0        0        0     6083 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/category.py
--rw-r--r--   0        0        0       46 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/__init__.py
--rw-r--r--   0        0        0     5516 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py
--rw-r--r--   0        0        0     6726 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py
--rw-r--r--   0        0        0     5543 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py
--rw-r--r--   0        0        0     5548 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py
--rw-r--r--   0        0        0     5211 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py
--rw-r--r--   0        0        0     4967 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/country.py
--rw-r--r--   0        0        0     5726 2024-04-09 13:47:43.243949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py
--rw-r--r--   0        0        0     4011 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py
--rw-r--r--   0        0        0     5970 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/number.py
--rw-r--r--   0        0        0     5474 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/range.py
--rw-r--r--   0        0        0     5277 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/text.py
--rw-r--r--   0        0        0     3727 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py
--rw-r--r--   0        0        0       49 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/area.py
--rw-r--r--   0        0        0     1565 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py
--rw-r--r--   0        0        0     5055 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/base.py
--rw-r--r--   0        0        0     1445 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py
--rw-r--r--   0        0        0     2355 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py
--rw-r--r--   0        0        0     1047 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/column.py
--rw-r--r--   0        0        0     1226 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py
--rw-r--r--   0        0        0     1203 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py
--rw-r--r--   0        0        0     1537 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py
--rw-r--r--   0        0        0     1299 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/font.py
--rw-r--r--   0        0        0     1146 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py
--rw-r--r--   0        0        0     1035 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/line.py
--rw-r--r--   0        0        0     1404 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/range.py
--rw-r--r--   0        0        0     2629 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py
--rw-r--r--   0        0        0     1612 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py
--rw-r--r--   0        0        0     1779 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py
--rw-r--r--   0        0        0      473 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/enums.py
--rw-r--r--   0        0        0     5447 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/exceptions.py
--rw-r--r--   0        0        0     1749 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/group.py
--rw-r--r--   0        0        0     9024 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/header.py
--rw-r--r--   0        0        0     2587 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/initial_state.py
--rw-r--r--   0        0        0     1916 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/styling.py
--rw-r--r--   0        0        0    17137 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/table.py
--rw-r--r--   0        0        0     3155 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/__init__.py
--rw-r--r--   0        0        0       45 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/__init__.py
--rw-r--r--   0        0        0     1722 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/base.py
--rw-r--r--   0        0        0      221 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/x_axis.py
--rw-r--r--   0        0        0       35 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/__init__.py
--rw-r--r--   0        0        0     4983 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py
--rw-r--r--   0        0        0      902 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py
--rw-r--r--   0        0        0     3137 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py
--rw-r--r--   0        0        0     4253 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py
--rw-r--r--   0        0        0     8795 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/chart.py
--rw-r--r--   0        0        0      513 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/consts.py
--rw-r--r--   0        0        0     1436 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/enums.py
--rw-r--r--   0        0        0    12101 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/exceptions.py
--rw-r--r--   0        0        0     1126 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/legend.py
--rw-r--r--   0        0        0     3093 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/navigator.py
--rw-r--r--   0        0        0       56 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/__init__.py
--rw-r--r--   0        0        0     2557 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py
--rw-r--r--   0        0        0     1051 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py
--rw-r--r--   0        0        0     5279 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py
--rw-r--r--   0        0        0     1196 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py
--rw-r--r--   0        0        0       46 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/__init__.py
--rw-r--r--   0        0        0     3328 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/area.py
--rw-r--r--   0        0        0     4520 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py
--rw-r--r--   0        0        0     7615 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/base.py
--rw-r--r--   0        0        0     5777 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py
--rw-r--r--   0        0        0     3350 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/column.py
--rw-r--r--   0        0        0     4362 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py
--rw-r--r--   0        0        0     3307 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/line.py
--rw-r--r--   0        0        0     3317 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/point.py
--rw-r--r--   0        0        0     3346 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py
--rw-r--r--   0        0        0      618 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/typing.py
--rw-r--r--   0        0        0    22602 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/timeseries.py
--rw-r--r--   0        0        0     1720 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/transform.py
--rw-r--r--   0        0        0       87 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/__init__.py
--rw-r--r--   0        0        0      543 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/exceptions.py
--rw-r--r--   0        0        0     4938 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/toggle.py
--rw-r--r--   0        0        0     2755 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/utils.py
--rw-r--r--   0        0        0       33 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/__init__.py
--rw-r--r--   0        0        0     1336 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/authentication/auth0.py
--rw-r--r--   0        0        0     5852 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/authentication/utils.py
--rw-r--r--   0        0        0       92 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/clients/__init__.py
--rw-r--r--   0        0        0     5003 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/clients/api.py
--rw-r--r--   0        0        0     1195 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/clients/exceptions.py
--rw-r--r--   0        0        0      482 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/exceptions.py
--rw-r--r--   0        0        0      432 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/__init__.py
--rw-r--r--   0        0        0      348 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/py.typed
--rw-r--r--   0        0        0     3169 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/schema.py
--rw-r--r--   0        0        0     6996 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/types.py
--rw-r--r--   0        0        0      319 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/engineai/sdk/internal/url_config.py
--rw-r--r--   0        0        0     2049 2024-04-09 13:47:43.247949 engineai_sdk-0.83.1/pyproject.toml
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 engineai_sdk-0.83.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-18 10:02:32.115517 engineai_sdk-0.86.1/LICENSE
+-rw-r--r--   0        0        0      987 2024-04-18 10:02:32.115517 engineai_sdk-0.86.1/README.md
+-rw-r--r--   0        0        0      435 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2541 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/commands/app.py
+-rw-r--r--   0        0        0    14251 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/commands/dashboard.py
+-rw-r--r--   0        0        0     1379 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/console.py
+-rw-r--r--   0        0        0     4806 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/generator.py
+-rw-r--r--   0        0        0       43 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/template/content/.env.sample
+-rw-r--r--   0        0        0     5396 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/template/content/data/example.json
+-rw-r--r--   0        0        0      411 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/template/content/main.py
+-rw-r--r--   0        0        0    10363 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/utils.py
+-rw-r--r--   0        0        0       38 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/__init__.py
+-rw-r--r--   0        0        0      121 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/__init__.py
+-rw-r--r--   0        0        0     2181 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/layout.py
+-rw-r--r--   0        0        0      207 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/selectable_widgets.py
+-rw-r--r--   0        0        0      570 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/typing.py
+-rw-r--r--   0        0        0     1600 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/base.py
+-rw-r--r--   0        0        0       96 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/__init__.py
+-rw-r--r--   0        0        0     3574 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/activate_dashboard.py
+-rw-r--r--   0        0        0     7670 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/api.py
+-rw-r--r--   0        0        0     1451 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/exceptions.py
+-rw-r--r--   0        0        0      217 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/__init__.py
+-rw-r--r--   0        0        0      472 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/py.typed
+-rw-r--r--   0        0        0      207 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/__init__.py
+-rw-r--r--   0        0        0     6861 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py
+-rw-r--r--   0        0        0     3134 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/json.py
+-rw-r--r--   0        0        0     4618 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/storage.py
+-rw-r--r--   0        0        0      515 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/config.py
+-rw-r--r--   0        0        0      310 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/__init__.py
+-rw-r--r--   0        0        0    13364 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/dashboard.py
+-rw-r--r--   0        0        0      140 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/enums.py
+-rw-r--r--   0        0        0     4691 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/exceptions.py
+-rw-r--r--   0        0        0       27 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/__init__.py
+-rw-r--r--   0        0        0     2417 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/executor_config.py
+-rw-r--r--   0        0        0     8389 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/instance.py
+-rw-r--r--   0        0        0     1231 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/node.py
+-rw-r--r--   0        0        0     2586 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/utils.py
+-rw-r--r--   0        0        0       41 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/__init__.py
+-rw-r--r--   0        0        0     1431 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/dependency.py
+-rw-r--r--   0        0        0     5667 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/page.py
+-rw-r--r--   0        0        0     1909 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/root.py
+-rw-r--r--   0        0        0     2932 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/route.py
+-rw-r--r--   0        0        0      345 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/typings.py
+-rw-r--r--   0        0        0       33 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/version/__init__.py
+-rw-r--r--   0        0        0     5105 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/version/version.py
+-rw-r--r--   0        0        0      185 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/__init__.py
+-rw-r--r--   0        0        0    12893 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/decorator.py
+-rw-r--r--   0        0        0     1822 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/duplicated.py
+-rw-r--r--   0        0        0     1047 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/enums.py
+-rw-r--r--   0        0        0     4676 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/exceptions.py
+-rw-r--r--   0        0        0     1996 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/http.py
+-rw-r--r--   0        0        0     3616 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/io_handler.py
+-rw-r--r--   0        0        0     1306 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/manager/interface.py
+-rw-r--r--   0        0        0     9994 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/manager/manager.py
+-rw-r--r--   0        0        0     2892 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/decorator.py
+-rw-r--r--   0        0        0      441 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/__init__.py
+-rw-r--r--   0        0        0     3521 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/datastore.py
+-rw-r--r--   0        0        0      141 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/__init__.py
+-rw-r--r--   0        0        0      966 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/header.py
+-rw-r--r--   0        0        0     2555 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/http.py
+-rw-r--r--   0        0        0     2026 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/route.py
+-rw-r--r--   0        0        0     2518 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/widget.py
+-rw-r--r--   0        0        0      369 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/__init__.py
+-rw-r--r--   0        0        0     1112 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/align.py
+-rw-r--r--   0        0        0      741 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/legend_position.py
+-rw-r--r--   0        0        0     5156 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/exceptions.py
+-rw-r--r--   0        0        0      569 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/__init__.py
+-rw-r--r--   0        0        0     3817 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/axis.py
+-rw-r--r--   0        0        0     1888 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/datetime.py
+-rw-r--r--   0        0        0      661 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/exceptions.py
+-rw-r--r--   0        0        0     1331 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/mapper.py
+-rw-r--r--   0        0        0     5254 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/number.py
+-rw-r--r--   0        0        0     1421 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/text.py
+-rw-r--r--   0        0        0      331 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/typing.py
+-rw-r--r--   0        0        0      985 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/validator.py
+-rw-r--r--   0        0        0     1056 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/interface.py
+-rw-r--r--   0        0        0      825 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/__init__.py
+-rw-r--r--   0        0        0      417 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/build_item.py
+-rw-r--r--   0        0        0       28 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/__init__.py
+-rw-r--r--   0        0        0     5990 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/card.py
+-rw-r--r--   0        0        0     2889 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/chip.py
+-rw-r--r--   0        0        0     1679 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/header.py
+-rw-r--r--   0        0        0       55 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/__init__.py
+-rw-r--r--   0        0        0     3082 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/chip.py
+-rw-r--r--   0        0        0     1968 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/header.py
+-rw-r--r--   0        0        0     6641 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/section.py
+-rw-r--r--   0        0        0     5999 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/column.py
+-rw-r--r--   0        0        0     2679 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/chip.py
+-rw-r--r--   0        0        0     2165 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/header.py
+-rw-r--r--   0        0        0     2385 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/label.py
+-rw-r--r--   0        0        0     4695 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/exceptions.py
+-rw-r--r--   0        0        0       31 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/__init__.py
+-rw-r--r--   0        0        0     5791 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py
+-rw-r--r--   0        0        0     1921 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/items_build.py
+-rw-r--r--   0        0        0     7313 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/grid.py
+-rw-r--r--   0        0        0    10423 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/row.py
+-rw-r--r--   0        0        0       36 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/__init__.py
+-rw-r--r--   0        0        0     7582 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/base.py
+-rw-r--r--   0        0        0     2171 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/exceptions.py
+-rw-r--r--   0        0        0     4397 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/tab.py
+-rw-r--r--   0        0        0      676 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/typings.py
+-rw-r--r--   0        0        0      244 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/__init__.py
+-rw-r--r--   0        0        0     6016 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/abstract.py
+-rw-r--r--   0        0        0     2201 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/route_link.py
+-rw-r--r--   0        0        0     2576 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/template_string_link.py
+-rw-r--r--   0        0        0      202 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/typing.py
+-rw-r--r--   0        0        0     1427 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/url.py
+-rw-r--r--   0        0        0      934 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/widget_dependency.py
+-rw-r--r--   0        0        0     3039 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/widget_field.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/py.typed
+-rw-r--r--   0        0        0     2020 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/selected.py
+-rw-r--r--   0        0        0      100 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/__init__.py
+-rw-r--r--   0        0        0     5872 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/default_specs.py
+-rw-r--r--   0        0        0     6985 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/discrete_map.py
+-rw-r--r--   0        0        0     1679 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/divergent.py
+-rw-r--r--   0        0        0     4055 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/gradient.py
+-rw-r--r--   0        0        0     5949 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/palette.py
+-rw-r--r--   0        0        0      920 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/single.py
+-rw-r--r--   0        0        0      946 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/spec.py
+-rw-r--r--   0        0        0      436 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/typing.py
+-rw-r--r--   0        0        0     3436 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/icons.py
+-rw-r--r--   0        0        0     8298 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/templated_string.py
+-rw-r--r--   0        0        0     3514 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/utils.py
+-rw-r--r--   0        0        0       25 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/__init__.py
+-rw-r--r--   0        0        0     8541 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/base.py
+-rw-r--r--   0        0        0     2647 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/__init__.py
+-rw-r--r--   0        0        0     3566 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/base.py
+-rw-r--r--   0        0        0      365 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/typing.py
+-rw-r--r--   0        0        0     2149 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py
+-rw-r--r--   0        0        0     5237 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py
+-rw-r--r--   0        0        0     4410 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/cartesian.py
+-rw-r--r--   0        0        0     4481 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/chart.py
+-rw-r--r--   0        0        0     1468 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/exceptions.py
+-rw-r--r--   0        0        0      987 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/legend.py
+-rw-r--r--   0        0        0       45 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/__init__.py
+-rw-r--r--   0        0        0     2640 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/area.py
+-rw-r--r--   0        0        0     4026 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py
+-rw-r--r--   0        0        0     7256 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/base.py
+-rw-r--r--   0        0        0     5303 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py
+-rw-r--r--   0        0        0     2660 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/column.py
+-rw-r--r--   0        0        0     2640 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/line.py
+-rw-r--r--   0        0        0     2679 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py
+-rw-r--r--   0        0        0      573 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/typing.py
+-rw-r--r--   0        0        0     4957 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/chart_utils.py
+-rw-r--r--   0        0        0       39 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/__init__.py
+-rw-r--r--   0        0        0     2630 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/base.py
+-rw-r--r--   0        0        0     1475 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py
+-rw-r--r--   0        0        0     1910 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py
+-rw-r--r--   0        0        0       47 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/__init__.py
+-rw-r--r--   0        0        0       56 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/__init__.py
+-rw-r--r--   0        0        0      416 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py
+-rw-r--r--   0        0        0     1764 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py
+-rw-r--r--   0        0        0     1764 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py
+-rw-r--r--   0        0        0     1117 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py
+-rw-r--r--   0        0        0     2785 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py
+-rw-r--r--   0        0        0      338 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/typing.py
+-rw-r--r--   0        0        0      151 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/consts.py
+-rw-r--r--   0        0        0     7162 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/exceptions.py
+-rw-r--r--   0        0        0       25 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/__init__.py
+-rw-r--r--   0        0        0     2787 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/base.py
+-rw-r--r--   0        0        0       23 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/__init__.py
+-rw-r--r--   0        0        0      955 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py
+-rw-r--r--   0        0        0     2138 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py
+-rw-r--r--   0        0        0      806 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py
+-rw-r--r--   0        0        0      314 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/typing.py
+-rw-r--r--   0        0        0      696 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py
+-rw-r--r--   0        0        0     1491 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/area.py
+-rw-r--r--   0        0        0     1573 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py
+-rw-r--r--   0        0        0     4041 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/base.py
+-rw-r--r--   0        0        0     3527 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py
+-rw-r--r--   0        0        0     3132 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py
+-rw-r--r--   0        0        0     1484 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/column.py
+-rw-r--r--   0        0        0     1047 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py
+-rw-r--r--   0        0        0     1540 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py
+-rw-r--r--   0        0        0     3635 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/line.py
+-rw-r--r--   0        0        0     1473 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/point.py
+-rw-r--r--   0        0        0     1514 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py
+-rw-r--r--   0        0        0      802 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py
+-rw-r--r--   0        0        0      282 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/toolbar.py
+-rw-r--r--   0        0        0      319 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/__init__.py
+-rw-r--r--   0        0        0     3647 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py
+-rw-r--r--   0        0        0     1490 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py
+-rw-r--r--   0        0        0     1641 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py
+-rw-r--r--   0        0        0      617 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py
+-rw-r--r--   0        0        0     1102 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py
+-rw-r--r--   0        0        0     1526 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py
+-rw-r--r--   0        0        0     1594 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py
+-rw-r--r--   0        0        0      647 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/typing.py
+-rw-r--r--   0        0        0       29 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/__init__.py
+-rw-r--r--   0        0        0     1192 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/base.py
+-rw-r--r--   0        0        0       35 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/__init__.py
+-rw-r--r--   0        0        0      228 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/area.py
+-rw-r--r--   0        0        0      236 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/column.py
+-rw-r--r--   0        0        0      228 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/line.py
+-rw-r--r--   0        0        0     1184 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py
+-rw-r--r--   0        0        0      379 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/typing.py
+-rw-r--r--   0        0        0      974 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py
+-rw-r--r--   0        0        0       36 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py
+-rw-r--r--   0        0        0      902 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py
+-rw-r--r--   0        0        0      893 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py
+-rw-r--r--   0        0        0      906 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py
+-rw-r--r--   0        0        0     1263 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py
+-rw-r--r--   0        0        0      339 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/typing.py
+-rw-r--r--   0        0        0       34 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/__init__.py
+-rw-r--r--   0        0        0      879 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py
+-rw-r--r--   0        0        0     1388 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py
+-rw-r--r--   0        0        0      943 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py
+-rw-r--r--   0        0        0      903 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py
+-rw-r--r--   0        0        0      331 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/typing.py
+-rw-r--r--   0        0        0     1313 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py
+-rw-r--r--   0        0        0     2014 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py
+-rw-r--r--   0        0        0     2003 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py
+-rw-r--r--   0        0        0      136 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/__init__.py
+-rw-r--r--   0        0        0     2890 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/content.py
+-rw-r--r--   0        0        0     1265 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/exceptions.py
+-rw-r--r--   0        0        0      613 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/item.py
+-rw-r--r--   0        0        0     1431 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/markdown.py
+-rw-r--r--   0        0        0     3756 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/exceptions.py
+-rw-r--r--   0        0        0      573 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/__init__.py
+-rw-r--r--   0        0        0     1369 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/color_axis.py
+-rw-r--r--   0        0        0     1043 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/enums.py
+-rw-r--r--   0        0        0      980 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/exceptions.py
+-rw-r--r--   0        0        0       25 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/__init__.py
+-rw-r--r--   0        0        0     8048 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/base.py
+-rw-r--r--   0        0        0     4272 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/geo.py
+-rw-r--r--   0        0        0       29 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/styling/__init__.py
+-rw-r--r--   0        0        0      832 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/styling/label.py
+-rw-r--r--   0        0        0      988 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/styling/styling.py
+-rw-r--r--   0        0        0      954 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/legend.py
+-rw-r--r--   0        0        0       42 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/__init__.py
+-rw-r--r--   0        0        0     4887 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/numeric.py
+-rw-r--r--   0        0        0      625 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/series.py
+-rw-r--r--   0        0        0     2937 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/styling.py
+-rw-r--r--   0        0        0     2113 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pandas_utils.py
+-rw-r--r--   0        0        0      672 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/__init__.py
+-rw-r--r--   0        0        0     1949 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/chart.py
+-rw-r--r--   0        0        0      852 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/exceptions.py
+-rw-r--r--   0        0        0      851 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/legend.py
+-rw-r--r--   0        0        0     6296 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/pie.py
+-rw-r--r--   0        0        0       35 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/__init__.py
+-rw-r--r--   0        0        0     6044 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/base.py
+-rw-r--r--   0        0        0     3413 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/country.py
+-rw-r--r--   0        0        0     3059 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/series.py
+-rw-r--r--   0        0        0     3185 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/styling.py
+-rw-r--r--   0        0        0      165 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/typings.py
+-rw-r--r--   0        0        0     2402 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/tooltip.py
+-rw-r--r--   0        0        0      391 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/__init__.py
+-rw-r--r--   0        0        0     3415 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/__init__.py
+-rw-r--r--   0        0        0     2793 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/base.py
+-rw-r--r--   0        0        0      900 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/build_result.py
+-rw-r--r--   0        0        0     3470 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/number.py
+-rw-r--r--   0        0        0       21 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/__init__.py
+-rw-r--r--   0        0        0     3252 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py
+-rw-r--r--   0        0        0     1523 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/number.py
+-rw-r--r--   0        0        0     1712 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/text.py
+-rw-r--r--   0        0        0     2432 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/text.py
+-rw-r--r--   0        0        0      280 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/typing.py
+-rw-r--r--   0        0        0     8158 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/search.py
+-rw-r--r--   0        0        0       79 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/exceptions.py
+-rw-r--r--   0        0        0     1783 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/group.py
+-rw-r--r--   0        0        0     6575 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/select.py
+-rw-r--r--   0        0        0     2453 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/__init__.py
+-rw-r--r--   0        0        0     6147 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/base.py
+-rw-r--r--   0        0        0     6201 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/category.py
+-rw-r--r--   0        0        0       46 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py
+-rw-r--r--   0        0        0     6726 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py
+-rw-r--r--   0        0        0     5672 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py
+-rw-r--r--   0        0        0     5669 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py
+-rw-r--r--   0        0        0     5330 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py
+-rw-r--r--   0        0        0     5103 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/country.py
+-rw-r--r--   0        0        0     5869 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py
+-rw-r--r--   0        0        0     4011 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py
+-rw-r--r--   0        0        0     6105 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/number.py
+-rw-r--r--   0        0        0     5601 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/range.py
+-rw-r--r--   0        0        0     5419 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/text.py
+-rw-r--r--   0        0        0     3727 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py
+-rw-r--r--   0        0        0       49 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/__init__.py
+-rw-r--r--   0        0        0     1146 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/area.py
+-rw-r--r--   0        0        0     1659 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py
+-rw-r--r--   0        0        0     5055 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/base.py
+-rw-r--r--   0        0        0     1541 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py
+-rw-r--r--   0        0        0     2510 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py
+-rw-r--r--   0        0        0     1161 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/column.py
+-rw-r--r--   0        0        0     1321 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py
+-rw-r--r--   0        0        0     1271 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py
+-rw-r--r--   0        0        0     1537 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py
+-rw-r--r--   0        0        0     1418 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/font.py
+-rw-r--r--   0        0        0     1233 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py
+-rw-r--r--   0        0        0     1147 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/line.py
+-rw-r--r--   0        0        0     1494 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/range.py
+-rw-r--r--   0        0        0     2723 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py
+-rw-r--r--   0        0        0     1727 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py
+-rw-r--r--   0        0        0     1779 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py
+-rw-r--r--   0        0        0      473 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/enums.py
+-rw-r--r--   0        0        0     5447 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/exceptions.py
+-rw-r--r--   0        0        0     1864 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/group.py
+-rw-r--r--   0        0        0     9162 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/header.py
+-rw-r--r--   0        0        0     2713 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/initial_state.py
+-rw-r--r--   0        0        0     2046 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/styling.py
+-rw-r--r--   0        0        0    17305 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/table.py
+-rw-r--r--   0        0        0     3155 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/__init__.py
+-rw-r--r--   0        0        0     1722 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/base.py
+-rw-r--r--   0        0        0      381 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/x_axis.py
+-rw-r--r--   0        0        0       35 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/__init__.py
+-rw-r--r--   0        0        0     4983 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py
+-rw-r--r--   0        0        0      902 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py
+-rw-r--r--   0        0        0     3279 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py
+-rw-r--r--   0        0        0     4413 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py
+-rw-r--r--   0        0        0     9066 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/chart.py
+-rw-r--r--   0        0        0      513 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/consts.py
+-rw-r--r--   0        0        0     1562 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/enums.py
+-rw-r--r--   0        0        0    12101 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/exceptions.py
+-rw-r--r--   0        0        0     1126 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/legend.py
+-rw-r--r--   0        0        0     3322 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/navigator.py
+-rw-r--r--   0        0        0       56 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/__init__.py
+-rw-r--r--   0        0        0     2692 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py
+-rw-r--r--   0        0        0     1051 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py
+-rw-r--r--   0        0        0     5436 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py
+-rw-r--r--   0        0        0     1339 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py
+-rw-r--r--   0        0        0       46 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/__init__.py
+-rw-r--r--   0        0        0     3472 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/area.py
+-rw-r--r--   0        0        0     4698 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py
+-rw-r--r--   0        0        0     7615 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/base.py
+-rw-r--r--   0        0        0     6061 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py
+-rw-r--r--   0        0        0     3621 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/column.py
+-rw-r--r--   0        0        0     4728 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py
+-rw-r--r--   0        0        0     3637 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/line.py
+-rw-r--r--   0        0        0     3623 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/point.py
+-rw-r--r--   0        0        0     3654 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py
+-rw-r--r--   0        0        0      618 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/typing.py
+-rw-r--r--   0        0        0    23062 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/timeseries.py
+-rw-r--r--   0        0        0     2038 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/transform.py
+-rw-r--r--   0        0        0       87 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/__init__.py
+-rw-r--r--   0        0        0      543 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/exceptions.py
+-rw-r--r--   0        0        0     5107 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/toggle.py
+-rw-r--r--   0        0        0     2755 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/utils.py
+-rw-r--r--   0        0        0       33 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/__init__.py
+-rw-r--r--   0        0        0     1336 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/authentication/auth0.py
+-rw-r--r--   0        0        0     5852 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/authentication/utils.py
+-rw-r--r--   0        0        0       92 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/clients/__init__.py
+-rw-r--r--   0        0        0     5003 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/clients/api.py
+-rw-r--r--   0        0        0     1195 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/clients/exceptions.py
+-rw-r--r--   0        0        0      482 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/exceptions.py
+-rw-r--r--   0        0        0      432 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/py.typed
+-rw-r--r--   0        0        0     3169 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/schema.py
+-rw-r--r--   0        0        0     6996 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/types.py
+-rw-r--r--   0        0        0      319 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/url_config.py
+-rw-r--r--   0        0        0     1841 2024-04-18 10:02:47.779638 engineai_sdk-0.86.1/pyproject.toml
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 engineai_sdk-0.86.1/PKG-INFO
```

### Comparing `engineai_sdk-0.83.1/LICENSE` & `engineai_sdk-0.86.1/LICENSE`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/README.md` & `engineai_sdk-0.86.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - Python 3.8 or higher
 
 ### Installation
 
 To install the SDK, run the following command:
 
 ```bash
-pip install engineai-sdk
+pip install engineai.sdk
 ```
 
 ### Create your First Dashboard
 
 To create your dashboard, you need to run the following command:
 
 ```bash
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/cli/commands/app.py` & `engineai_sdk-0.86.1/engineai/sdk/cli/commands/app.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/cli/commands/dashboard.py` & `engineai_sdk-0.86.1/engineai/sdk/cli/commands/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,30 +250,22 @@
 def dashboard(ctx: click.Context, slug: str) -> None:
     """Dashboard commands."""
     ctx.ensure_object(dict)
     ctx.obj["SLUG"] = slug
 
 
 @dashboard.command()
-@click.option(
-    "--tutorial-data",
-    is_flag=True,
-    default=False,
-    help="Adds example data to the dashboard.",
-)
-def init(tutorial_data: bool) -> None:
+def init() -> None:
     """Create a simple and functional dashboard."""
     try:
         slug = click.prompt(
             "Name your project", default="new_dashboard", type=str, show_default=True
         )
 
-        is_new_project = generate_template(
-            dashboard_slug=slug, tutorial_data=tutorial_data
-        )
+        is_new_project = generate_template(dashboard_slug=slug)
         if is_new_project:
             write_console(DASHBOARD_CREATED_MSG.format(slug))
         else:
             write_console("Tutorial data has been successfully added to your project.")
     except ProjectAlreadyExistsError:
         write_console(
             "\nDashboard already exists! "
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/cli/console.py` & `engineai_sdk-0.86.1/engineai/sdk/cli/console.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/cli/generator.py` & `engineai_sdk-0.86.1/engineai/sdk/cli/generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,63 +10,51 @@
 
 
 class _TemplateGenerator:
     PLACEHOLDER_SLUG = "@dashboard_slug@"
     DIRECTORY_NAME = "content"
     MAIN_FILE = "main%s.py"
 
-    def __init__(self, dashboard_slug: str, tutorial_data: bool = False) -> None:
-        self.__tutorial_data = tutorial_data
+    def __init__(self, dashboard_slug: str) -> None:
         self._dashboard_slug = dashboard_slug
         self.empty = True
         self.__is_new_project = False
 
     @property
     def _template_path(self) -> Path:
         return Path(f"{Path(__file__).parent.absolute()}/template")
 
     @property
-    def _tutorial_path(self) -> Path:
-        return Path(f"{Path(__file__).parent.absolute()}/tutorial_data")
-
-    @property
     def _project_path(self) -> Path:
         return Path(Path(os.getcwd()) / f"{self._dashboard_slug}")
 
     @property
     def is_new_project(self) -> bool:
         return self.__is_new_project
 
     def run(self) -> None:
         os.chdir(os.getcwd())
         self.__validate_project()
         self.__add_project()
 
     def __validate_project(self) -> None:
         """Validate current project."""
-        if (
-            not self.__tutorial_data
-            and os.path.exists(self._dashboard_slug)
-            or self.__tutorial_data
-            and os.path.exists(self._project_path / "data")
-        ):
+        if os.path.exists(self._dashboard_slug):
             raise ProjectAlreadyExistsError()
 
     def __add_project(self):
         if not os.path.exists(self._project_path):
             self.__copy_paths()
             self.__update_dashboard_slug()
 
             self.__move_files()
             self.__create_dot_env()
 
             self.__is_new_project = True
 
-        self.__copy_tutorial_files()
-
     def __copy_paths(self) -> None:
         shutil.copytree(
             self._template_path / self.DIRECTORY_NAME,
             Path(os.getcwd()) / self.DIRECTORY_NAME,
         )
 
     def __update_dashboard_slug(self) -> None:
@@ -122,33 +110,26 @@
 
     def __create_dot_env(self) -> None:
         if not os.path.exists(f"{self._dashboard_slug}/.env"):
             os.rename(
                 f"{self._dashboard_slug}/.env.sample", f"{self._dashboard_slug}/.env"
             )
 
-    def __copy_tutorial_files(self):
-        if self.__tutorial_data and not os.path.exists(self._project_path / "data"):
-            shutil.copytree(
-                self._tutorial_path,
-                self._project_path / "data",
-            )
-
 
-def generate_template(dashboard_slug: str, tutorial_data: bool) -> bool:
+def generate_template(dashboard_slug: str) -> bool:
     """Interface to generate a template for a new dashboard.
 
     Args:
         dashboard_slug (str): Dashboard slug.
         tutorial_data (bool): If True, will generate example data.
 
     Returns:
         True if it is a new project, False otherwise.
     """
-    template_generator = _TemplateGenerator(dashboard_slug, tutorial_data)
+    template_generator = _TemplateGenerator(dashboard_slug)
     template_generator.run()
     return template_generator.is_new_project
 
 
 def remove_temporary_files():
     """Method that removes the temporary files created by the cookiecutter."""
     if os.path.isdir(main_folder := os.path.join(os.getcwd(), "content")):
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/cli/utils.py` & `engineai_sdk-0.86.1/engineai/sdk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/layout.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/layout.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/abstract/typing.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/activate_dashboard.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/activate_dashboard.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/api.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/api.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/serialization/json.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/json.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/clients/storage/storage.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/storage.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/config.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/config.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/dashboard.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,20 @@
     DEFAULT = "default"
     DEV = "dev"
     DRAFT = "draft"
     LIVE = "live"
 
 
 class Dashboard:
-    """Dashboard class."""
+    """Central component for managing layouts, widgets, cards.
+
+    The Dashboard class is the central component for creating
+    and managing dashboards. It serves as the container for various
+    layout elements, widgets, and cards.
+    """
 
     @type_check
     def __init__(
         self,
         *,
         slug: str = "new_dashboard",
         content: Union[List[Page], DashboardContent],
@@ -83,15 +88,15 @@
         last_available_data: Optional[Union[datetime, List[str]]] = None,
         status: Optional[DashboardStatus] = None,
         version: Optional[str] = None,
         skip_data: bool = False,
         storage_type: StorageType = StorageType.BLOB,
         publish_mode: PublishMode = PublishMode.DEFAULT,
     ):
-        """Construct for Dashboard class.
+        """Constructor for Dashboard.
 
         Args:
             slug: unique identifier for dashboard.
             content: Dashboard content.
             app_id: App id where the dashboard will be published.
                 For development purposes the app_id can be set as environment variable
                 as APP_ID.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/executor_config.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/executor_config.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/instance.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/instance.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/node.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/node.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/graph/utils.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/dependency.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/dependency.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/page.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,26 @@
 from .root import RootGrid
 from .route import Route
 
 ROW_HEIGHT_PIXELS: Final[int] = 100
 
 
 class Page:
-    """Dashboard Page spec."""
+    """Provides a flexible way to structure dashboard content."""
 
     @type_check
     def __init__(
         self,
         *,
         name: TemplatedStringItem,
         content: DashboardContent,
         route: Optional[Route] = None,
         path: str = "/",
     ):
-        """Page class constructor.
+        """Constructor for Page.
 
         Args:
             name: Dashboard name to be displayed. Defaults to slug
                 title case.
             content: Dashboard content.
             route: Specs for Page routing.
             path: page endpoint path.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/root.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/root.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/page/route.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/route.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dashboard/version/version.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/version/version.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/decorator.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/decorator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/duplicated.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/duplicated.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/enums.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/http.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/http.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/io_handler.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/io_handler.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/manager/interface.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/manager/interface.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/data/manager/manager.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/manager/manager.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/decorator.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/decorator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/datastore.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/datastore.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/http/header.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/http/http.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/http.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/route.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/route.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/dependencies/widget.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/widget.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/align.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/align.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """Dashboard Alignment Enums."""
 import enum
 
 
 class HorizontalAlignment(enum.Enum):
-    """Horizontal Alignment keys.
+    """Horizontal alignment keys.
+
+    Description of horizontal alignment keys.
 
     Attributes:
         LEFT (str): Left alignment.
         CENTER (str): Center alignment.
         RIGHT (str): Right alignment.
     """
 
     LEFT = "LEFT"
     CENTER = "CENTER"
     RIGHT = "RIGHT"
 
 
 class FluidHorizontalAlignment(enum.Enum):
-    """Horizontal Alignment keys.
+    """Horizontal alignment keys for fluid layout.
+
+    Description of horizontal alignment keys used for fluid layout.
 
     Attributes:
         LEFT (str): Left alignment.
         CENTER (str): Center alignment.
         RIGHT (str): Right alignment.
         STRETCH (str): Stretch alignment.
     """
@@ -31,14 +35,16 @@
     RIGHT = "RIGHT"
     STRETCH = "STRETCH"
 
 
 class VerticalAlignment(enum.Enum):
     """Vertical alignment keys.
 
+    Description of vertical alignment keys.
+
     Attributes:
         TOP (str): Top alignment.
         MIDDLE (str): Middle alignment.
         BOTTOM (str): Bottom alignment.
     """
 
     TOP = "TOP"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/enum/legend_position.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/legend_position.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Legend position enum."""
 import enum
 
 
 class LegendPosition(enum.Enum):
-    """Options for positions of charts legend.
+    """Chart legend position options.
+
+    Options for positions of charts legend.
 
     Attributes:
         RIGHT (str): Legend is placed to the right of the chart.
         BOTTOM (str): Legend is placed below the chart.
         RIGHT_GROUPED (str): Legend is placed to the right of the chart
             and grouped with other legends.
         BOTTOM_GROUPED (str): Legend is placed below the chart
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/__init__.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/axis.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,29 @@
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 
 from .number import NumberScale
 
 
 class AxisNumberFormatting(AbstractFactoryLinkItemsHandler):
-    """Spec to format Numeric Axis."""
+    """Numeric axis formatting.
+
+    Description for formatting numeric axis, allowing
+    customization of scale, decimal places, prefix, and suffix.
+    """
 
     def __init__(
         self,
         *,
         scale: NumberScale = NumberScale.DYNAMIC_ABSOLUTE,
         decimals: Optional[int] = None,
         prefix: Optional[Union[TemplatedStringItem, DataField]] = None,
         suffix: Optional[Union[TemplatedStringItem, DataField]] = None,
     ):
-        """Spec to format Numeric Axis.
+        """Constructor for AxisNumberFormatting.
 
         Args:
             scale (NumberScale): scale used to format number.
                 For example, if NumberScale.THOUSAND, number is divided by 1_000
                 and a suffix "K" is added.
                 Defaults to NumberScale.DYNAMIC_ABSOLUTE (formats K, M, Bn), but
                 not percentage or basis point values.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/datetime.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/datetime.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,23 +13,27 @@
 
     DATE = "DATE"
     TIME = "TIME"
     DATETIME = "DATETIME"
 
 
 class DateTimeFormatting(AbstractFactory):
-    """Spec to format date and time values."""
+    """Date and time value formatting.
+
+    Description for formatting date and time values,
+    specifying template and time unit.
+    """
 
     def __init__(
         self,
         *,
         template: Optional[str] = None,
         time_unit: DateTimeUnit = DateTimeUnit.DATE
     ):
-        """Spec to format DateTime values represented as timestamps.
+        """Constructor for DateTimeFormatting.
 
         Args:
             template (Optional[str]): using spec from
                 https://date-fns.org/v1.30.1/docs/format
             time_unit (DateTimeUnit): determines part of timestamp to consider.
                 Defaults to DateTimeUnit.DATE.
         """
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/mapper.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/mapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 from typing import Mapping
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class MapperFormatting(AbstractFactory):
-    """Factory class to map a column with ordinal numbers to text."""
+    """Factory class to map a column with ordinal numbers to text.
+
+    Factory class to map ordinal numbers to text
+    labels for categorical data.
+    """
 
     def __init__(self, *, mapping: Mapping[int, str]):
-        """Spec to format numbers that represent categories.
+        """Constructor for MapperFormatting.
 
         Args:
             mapping (Mapping[int, str]): mapping between number and text label.
         """
         super().__init__()
         self.__mapping = mapping
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/number.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/number.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,27 +34,31 @@
         "DYNAMIC_ABSOLUTE"  # scale is dynamically detected based on range of values
     )
     DYNAMIC_RELATIVE = "DYNAMIC_RELATIVE"  # apply Basis point if median < 0.01
     # apply Percentage otherwise
 
 
 class NumberFormatting(AbstractFactoryLinkItemsHandler):
-    """Spec to format numeric values."""
+    """Numeric value formatting.
+
+    Description for formatting numeric values, providing options for scale,
+    decimal places, prefix, suffix, and displaying positive sign.
+    """
 
     @beartype
     def __init__(
         self,
         *,
         scale: Union[NumberScale, GenericLink] = NumberScale.DYNAMIC_ABSOLUTE,
         decimals: Optional[int] = None,
         prefix: Optional[Union[TemplatedStringItem, DataField]] = None,
         suffix: Optional[Union[TemplatedStringItem, DataField]] = None,
         show_positive_sign: bool = False
     ):
-        """Spec to format numeric values.
+        """Constructor for NumberFormatting.
 
         Args:
             scale: scale used to format number if is type NumberScale. For example, if
                 NumberScale.THOUSAND, number is divided by 1_000 and a suffix "K" is
                 added. If is type TemplatedStringItem, this variable allow formatting
                 to be dynamically.
                 Defaults to NumberScale.DYNAMIC_ABSOLUTE (formats K, M, Bn), but
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/text.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/text.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 from typing import Optional
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class TextFormatting(AbstractFactory):
-    """Spec to format text."""
+    """Customize maximum characters and splitting options.
+
+    Description for formatting text, allowing customization
+    of maximum characters and splitting.
+    """
 
     def __init__(self, *, max_characters: int = 30, split: Optional[str] = None):
-        """Spec to format text.
+        """Constructor for TextFormatting.
 
         Args:
             max_characters (int): number of characters to show before text is trimmed.
                 If len(text) > max_characters, text is trimmed to max_characters and
                 ... are added and full text shown on hover.
                 Defaults to 30.
             split (Optional[str]): split character to determine first word.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/formatting/validator.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/validator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/interface.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/interface.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/__init__.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/card.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/card.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,31 @@
 from engineai.sdk.dashboard.utils import generate_input
 
 from ...base import DependencyInterface
 from .header import CardHeader
 
 
 class Card(CardInterface):
-    """Spec for a Card in a dashboard layout."""
+    """Groups content with widgets, grids, and selectable sections.
+
+    The Card class is a fundamental component in a dashboard layout,
+    allowing users to group and organize content. It provides a container
+    for various layout items such as widgets, cards, grids, and selectable sections.
+    """
 
     _INPUT_KEY = "card"
 
     @type_check
     def __init__(
         self,
         *,
         content: Union[LayoutItem, List[LayoutItem]],
         header: Optional[Union[TemplatedStringItem, CardHeader]] = None,
     ) -> None:
-        """Construct Card in dashboard layout.
+        """Constructor for Card.
 
         Args:
             content: content within the Card. One of Widget, Card, Grid,
                 SelectableSection.
             header: Header card spec. Defaults to None, i.e. a card without title.
 
         Examples:
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/card/chip.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/chip.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..components.chip import BaseChip
 
 
 class CardChip(BaseChip):
-    """Spec for the layout Card Header chip."""
+    """Labels or links within a card header for additional context.
+
+    The CardChip class represents individual chips within a card
+    header, providing additional labels or links.
+    """
 
     @type_check
     def __init__(
         self,
         *,
         label: Union[str, GenericLink],
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         prefix: str = "",
         suffix: str = "",
     ) -> None:
-        """Construct CardHeaderContext in Layout Card Header.
+        """Constructor for CardChip.
 
         Args:
             label: Card Header label value. Can assume a static label or a single
                 GenericLink.
             tooltip_text: informational pop up text. Each element of list is displayed
                 as a separate paragraph. Can only use this option if the `label` is
                 set.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/chip.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/chip.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 from engineai.sdk.dashboard.links.typing import GenericLink
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..components.chip import BaseChip
 
 
 class CollapsibleSectionChip(BaseChip):
-    """Spec for the layout Collapsible Section Header context."""
+    """Labels or links within collapsible section headers for extra context.
+
+    The CollapsibleSectionChip class represents individual chips within a
+    collapsible section header, providing additional labels or links.
+    """
 
     @type_check
     def __init__(
         self,
         *,
         label: Union[str, GenericLink],
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         prefix: str = "",
         suffix: str = "",
     ) -> None:
-        """Construct CollapsibleSectionChip in Layout Collapsible Section Header.
+        """Constructor for CollapsibleSectionChip.
 
         Args:
             label: Collapsible Section Header label value. Can assume a static label.
             tooltip_text: informational pop up text. Each element of list is displayed
                 as a separate paragraph. Can only use this option if the `label` is
                 set.
             prefix: prefix value to use in before each label.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/header.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/header.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,23 +6,28 @@
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..components.header import BaseHeader
 from .chip import CollapsibleSectionChip
 
 
 class CollapsibleSectionHeader(BaseHeader):
-    """Spec for the layout Collapsible Section Header."""
+    """Provides title and chips for collapsible section headers.
+
+    The CollapsibleSectionHeader class represents the header of a
+    collapsible section, providing additional information such as
+    title and chips.
+    """
 
     @type_check
     def __init__(
         self,
         *chips: CollapsibleSectionChip,
         title: Optional[TemplatedStringItem] = None,
     ):
-        """Construct Header for Collapsible Section layout.
+        """Constructor for CollapsibleSectionHeader.
 
         Args:
             chips: chips to be added to the collapsible section header.
             title: Collapsible Section title.
 
         Examples:
             ??? example "Create a Collapsible Section layout with a title"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/collapsible/section.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/section.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,32 @@
 from engineai.sdk.dashboard.utils import generate_input
 
 from ...base import DependencyInterface
 from .header import CollapsibleSectionHeader
 
 
 class CollapsibleSection(CollapsibleInterface):
-    """Spec for a Collapsible Section in a dashboard layout."""
+    """Organize and group content with expandable/collapsible sections.
+
+    The CollapsibleSection class is used to create collapsible sections
+    within a dashboard layout, providing a way to organize and group
+    content that can be expanded or collapsed.
+    """
 
     _INPUT_KEY = "collapsible"
 
     @type_check
     def __init__(
         self,
         *,
         content: Union[LayoutItem, List[LayoutItem]],
         header: Optional[Union[TemplatedStringItem, CollapsibleSectionHeader]] = None,
         expanded: bool = True,
     ) -> None:
-        """Construct Collapsible Section in dashboard layout.
-
-        CollapsibleSection is only supported in the root level in each Page.
+        """Constructor for CollapsibleSection.
 
         Args:
             content: content within the Section. One of Widget, Card, Grid,
                 SelectableSection.
             header: Header specifications. By default the CollapsibleSection does
                 not have title
             expanded: Whether the section is expanded or not.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/column.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,27 @@
 from ..widgets.base import Widget
 from .exceptions import ColumnLimitsWidthError
 from .exceptions import ColumnWrongWidthSizeError
 from .exceptions import ElementHeightNotDefinedError
 
 
 class Column(AbstractFactory):
-    """Spec for a column in a dashboard vertical grid layout."""
+    """Organize and group content vertically within a vertical grid layout.
+
+    The Column class represents a column within a vertical grid layout,
+    providing a way to organize and group content vertically.
+    """
 
     @type_check
     def __init__(self, *, content: LayoutItem, width: Optional[int] = None):
-        """Construct column in dashboard vertical grid layout.
+        """Constructor for Column.
 
         Args:
-            content: Content that is going to be added inside the column.
+            content: Representing the base class for items in a dashboard layout.
+                It's a common type that other layout-related classes inherit from.
             width: Sets the column width, value between 3 and 12. If value is None
                 the width will be set automatically based on the number of columns
                 in the row.
 
         Examples:
             ??? example "Create Column with widget"
                 ```py linenums="1"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/chip.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/chip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/header.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/components/label.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/label.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,27 @@
 
 from ..exceptions import ElementHeightNotDefinedError
 from .items_build import DashboardFluidRowItem
 from .items_build import build_fluid_item
 
 
 class FluidRow(AbstractFactory):
-    """Spec for a fluid row in a dashboard vertical grid layout."""
+    """Enables flexible and responsive content alignment in a vertical grid layout.
+
+    The FluidRow class represents a fluid row within a vertical grid layout,
+    allowing for flexible and responsive content alignment.
+    """
 
     def __init__(
         self,
         *items: DashboardFluidRowItem,
         vertical_alignment: VerticalAlignment = VerticalAlignment.TOP,
         horizontal_alignment: HorizontalAlignment = HorizontalAlignment.CENTER,
     ) -> None:
-        """Construct fluid row in dashboard vertical grid layout.
+        """Constructor for FluidRow.
 
         Args:
             items: item within the FluidRow. One of Select, Toggle.
             vertical_alignment: Fluid Row vertical alignment option.
                 `TOP`, `MIDDLE` or `BOTTOM`, available.
             horizontal_alignment: Fluid Row horizontal alignment option.
                 `LEFT`, `CENTER`, `RIGHT` or `STRETCH` available.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/fluid_row/items_build.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/items_build.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.search.search import Search
 from engineai.sdk.dashboard.widgets.select.select import Select
 from engineai.sdk.dashboard.widgets.toggle.toggle import Toggle
 
 DashboardFluidRowItem = Union[Select, Toggle, Search]
+"""Includes Select, Toggle, and Search as valid items within FluidRow,
+
+The DashboardFluidRowItem union represents the items that can
+be included within a FluidRow. It includes Select, Toggle,
+and Search as valid items.
+"""
 
 
 def build_fluid_item(item: DashboardFluidRowItem) -> Any:
     """Method implemented by all factories to generate Input spec.
 
     Args:
         item (DashboardFluidRowItem): Fluid row item spec.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/grid.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,26 @@
 from ..utils import generate_input
 from .exceptions import ElementHeightNotDefinedError
 from .fluid_row.fluid_row import FluidRow
 from .row import Row
 
 
 class Grid(GridInterface):
-    """Spec for a grid in a dashboard vertical grid layout."""
+    """Organize dashboard content with vertical grid structure.
+
+    The Grid class is component in a dashboard layout,
+    allowing users to organize content using a vertical grid structure.
+    It provides a way to arrange widgets, rows, and selectable sections.
+    """
 
     _INPUT_KEY = "grid"
 
     @type_check
     def __init__(self, *items: Union[LayoutItem, Row, FluidRow]) -> None:
-        """Construct dashboard grid.
+        """Constructor for Grid.
 
         Args:
             items: items to add to grid. Can be widgets, rows or
                 selectable sections (e.g tabs).
 
         Examples:
             ??? example "Create Grid with widget"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/row.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/row.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,27 @@
 from .exceptions import RowMinimumItemsError
 from .exceptions import RowsDifferentCustomHeightError
 from .exceptions import RowsHeightsSetMultipleLevelsError
 from .typings import LayoutItem
 
 
 class Row(AbstractFactory):
-    """Spec for a row in a dashboard vertical grid layout."""
+    """Organize and group content horizontally within a vertical grid layout.
+
+    The Row class represents a row within a vertical grid layout, allowing
+    users to organize and group content horizontally.
+    """
 
     @type_check
     def __init__(
         self,
         *items: Union[LayoutItem, Column],
         height: Optional[Union[float, int]] = None,
     ) -> None:
-        """Construct row in dashboard vertical grid layout.
+        """Constructor for Row.
 
         Args:
             *items: Content that is going to be added inside the Row,
                 if the item is a Column, it will be added to the row, if the item
                 is a Widget or a Grid, it will be added to a Column.
             height: Custom height for the row.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/layout/selectable/tab.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/tab.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 from engineai.sdk.dashboard.utils import is_valid_url
 
 from .base import SelectableItem
 from .base import SelectableSection
 
 
 class Tab(SelectableItem):
-    """Specs for tab in a tab section."""
+    """Represents an individual tab within a TabSection."""
 
     @type_check
     def __init__(
         self,
         *,
         label: TemplatedStringItem,
         content: Union[LayoutItem, List[LayoutItem]],
         icon: Optional[Union[Icons, WidgetField, str]] = None,
         default_selected: bool = False,
     ):
-        """Construct tab for tab section dashboard vertical grid layout.
+        """Constructor for Tab.
 
         Args:
             label: label to be displayed in tab.
             content: item to be added in tab.
             icon: tab icon.
             default_selected: set tab as default selected.
         """
@@ -65,25 +65,30 @@
             if self.__icon is not None
             else None,
             preSelected=self.default_selected,
         )
 
 
 class TabSection(SelectableSection):
-    """Spec for tab section in the layout."""
+    """Organize dashboard content within tabs.
+
+    The TabSection class is a crucial part of a dashboard
+    layout, allowing users to organize content within tabs.
+
+    """
 
     _API_TYPE = "tabSection"
     _INPUT_KEY = "tabSection"
 
     @type_check
     def __init__(
         self,
         *tabs: Tab,
     ):
-        """Construct for TabSection class.
+        """Constructor for TabSection.
 
         Args:
             tabs: tabs to be added to tab section.
 
         Examples:
             ??? example "Create a TabSection with different tabs"
                 ```py linenums="1"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/abstract.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/abstract.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/route_link.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/route_link.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/template_string_link.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/template_string_link.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/url.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/url.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/widget_dependency.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/widget_dependency.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/links/widget_field.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/widget_field.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/selected.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/selected.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/__init__.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/default_specs.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/default_specs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,22 @@
 from .gradient import Gradient
 from .gradient import GradientItem
 from .single import Palette
 from .single import Single
 
 
 class PositiveNegativeDiscreteMap(DiscreteMap):
-    """Template DiscreteMap for Positive/Negative Numbers."""
+    """Template for discrete map with positive/negative numbers.
+
+    Template for creating a discrete map specifically designed
+    for positive and negative numbers.
+    """
 
     def __init__(self) -> None:
-        """Creates template DiscreteMap for Positive/Negative Numbers."""
+        """Constructor for PositiveNegativeDiscreteMap."""
         super().__init__(
             DiscreteMapIntervalItem(
                 color=Palette.RUBI_RED,
                 min_value=-sys.maxsize,
                 max_value=0,
                 exclude_max=True,
             ),
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/discrete_map.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/discrete_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,32 @@
 from engineai.sdk.dashboard.utils import generate_input
 
 from .palette import Palette
 from .single import Single
 
 
 class DiscreteMapIntervalItem(AbstractFactory):
-    """Spec to create a color discrete map item with a value connected to a color."""
+    """Map value intervals to colors.
+
+    Define specifications for creating a color discrete
+    map item, enabling association of a color with an
+    interval of numerical values.
+    """
 
     @type_check
     def __init__(
         self,
         *,
         min_value: Union[float, int],
         max_value: Union[float, int],
         color: Union[Palette, Single],
         exclude_min: bool = False,
         exclude_max: bool = False,
     ):
-        """Construct spec to map a color to an interval of values.
+        """Constructor for DiscreteMapIntervalItem.
 
         Args:
             min_value: start of the interval.
             max_value: end of the interval.
             color: color applied to interval (Palette)
                 or color itself (Single).
             exclude_min: whether to make min exclusive. (Default: ``False``)
@@ -56,23 +61,27 @@
             color=self.__color.build(),
             excludeMax=self.__exclude_max,
             excludeMin=self.__exclude_min,
         )
 
 
 class DiscreteMapValueItem(AbstractFactory):
-    """Helper to create a color discrete map item with a value connected to a color."""
+    """Map single values to colors.
+
+    Create a specification to represent a discrete mapping between a
+    single value and a specific color within a discrete color map.
+    """
 
     @type_check
     def __init__(
         self,
         value: Union[float, int],
         color: Union[Palette, Single],
     ):
-        """Construct spec to map a single value to a specific color.
+        """Constructor for DiscreteMapValueItem.
 
         Args:
             value: value for which the color will be applied.
             color: color applied to interval (Palette)
                 or color itself (Single).
         """
         super().__init__()
@@ -90,19 +99,25 @@
         )
 
 
 DiscreteMapItem = Union[DiscreteMapIntervalItem, DiscreteMapValueItem]
 
 
 class DiscreteMap(AbstractFactory):
-    """Spec to create a discrete map of colors."""
+    """Map values to specific colors.
+
+    Construct a specification for creating a discrete map of colors.
+    The DiscreteMap class allows users to define a set of
+    DiscreteMapItem objects, each representing a mapping
+    between a specific value or category and a corresponding color.
+    """
 
     @type_check
     def __init__(self, *items: DiscreteMapItem):
-        """Builds spec for a discrete map of colors.
+        """Constructor for DiscreteMap.
 
         Args:
             items: list of values, intervals composing the
                 color map (DiscreteMapIntervalItem or DiscreteMapValueItem)
 
         Examples:
             ??? example "Create a discrete color map with DiscreteMapIntervalItem"
@@ -164,15 +179,18 @@
 
 class _ColorMethod(Protocol):
     def __call__(self, *, index: int) -> Palette:
         ...
 
 
 def generate_color_mapping(*, length: int, color_method: _ColorMethod) -> DiscreteMap:
-    """Generate a category color mapping based on the color method used.
+    """Generate color mapping by length, method.
+
+    Function to generate a color mapping based on specified
+    parameters like length and color method.
 
     Examples:
         ??? example "Create a discrete color map with DiscreteMapIntervalItem"
             ```py linenums="1"
             from engineai.sdk.dashboard.styling.color.palette import (
                 qualitative_palette
             )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/divergent.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/divergent.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def __init__(
         self,
         mid_value: int,
         mid_color: Palette,
         above_color: ColorSpec,
         below_color: ColorSpec,
     ) -> None:
-        """Construct method for ColorDivergent class.
+        """Constructor for ColorDivergent.
 
         Args:
             mid_value: intermediate value for comparison.
             mid_color: color for intermediate
                 value.
             above_color: color spec for value above mid_value.
             below_color: color spec for value below mid_value.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/gradient.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/gradient.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,24 +8,29 @@
 from engineai.sdk.dashboard.styling.color.palette import Palette
 from engineai.sdk.dashboard.utils import generate_input
 
 from .single import Single
 
 
 class GradientItem(AbstractFactory):
-    """Item of a color gradient."""
+    """Represents value and corresponding color in a gradient.
+
+    Item within a color gradient, representing a value and its
+    corresponding color. For instance suppose that a gradient has
+    3 colors, the Gradient class will have 3 GradientItem(s).
+    """
 
     @type_check
     def __init__(
         self,
         *,
         value: Union[float, int],
         color: Union[Palette, Single],
     ):
-        """Item of a Color Gradient.
+        """Constructor for GradientItem.
 
         Args:
             value: initial value of interval with color.
             color: color applied to interval (Palette)
                 or color itself (Single).
         """
         super().__init__()
@@ -40,21 +45,26 @@
         """
         return generate_input(
             "GradientItemInput", color=self.__color.build(), value=self.__value
         )
 
 
 class Gradient(AbstractFactory):
-    """Gradient of transition between colors."""
+    """Define gradient for smooth transitions between colors.
+
+    Create a specification for defining a color gradient, allowing
+    for smooth transitions between colors. The Gradient class
+    facilitates the creation of a continuous range of colors by
+    specifying a set of GradientItem objects representing key
+    points along the gradient.
+    """
 
     @type_check
     def __init__(self, *items: GradientItem, steps: int = 10):
-        """Color Gradient spec.
-
-        This class is used to create a gradient of colors using
+        """Constructor for Gradient.
 
         Args:
             items: map between color and intervals.
             steps: number of intermediate colors between gradient items.
                 Defaults to 10.
 
         Examples:
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/palette.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/palette.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """Color palette."""
 import enum
 from typing import Any
 from typing import Optional
 
 
 class PaletteTypes(enum.Enum):
-    """Selection of Palettes."""
+    """Selection of color palettes.
+
+    Selection of different types of color palettes available.
+    """
 
     QUALITATIVE = "QUALITATIVE"
     SEQUENTIAL = "SEQUENTIAL"
 
 
 class Palette(enum.Enum):
-    """Color Palette."""
+    """Predefined color palettes.
+
+    Collection of predefined color palettes for various purposes.
+    """
 
     # qualitative
     MINT_GREEN = "#57DBD8"
     SUNSET_ORANGE = "#F79F5F"
     BUBBLEGUM_PINK = "#BA5479"
     GRASS_GREEN = "#68B056"
     LAVENDER_PURPLE = "#9A77FF"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/color/spec.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/spec.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/styling/icons.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/icons.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/templated_string.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/templated_string.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/utils.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from ..abstract.layout import AbstractLayoutItem
 from ..abstract.selectable_widgets import AbstractSelectWidget
 
 WidgetTitleType = Optional[Union[str, GenericLink]]
 
 
 class Widget(DependencyManager, AbstractLayoutItem, WidgetInterface):
-    """Base spec shared by all widgets."""
+    """Building blocks of visualizations within the Platform SDK."""
 
     _WIDGET_API_TYPE: Optional[str] = None
     _DEFAULT_HEIGHT: Union[int, float] = 4
     _FORCE_HEIGHT: bool = False
     _WIDGET_HEIGHT_STEP = 0.1
     _WIDGET_ID_COUNTER = 0
     _INPUT_KEY = "widget"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/__init__.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/cartesian.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/cartesian.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         x_axis: Union[str, GenericLink, XAxis],
         left_y_axis: Optional[Union[YAxisSeries, YAxis]] = None,
         right_y_axis: Optional[Union[YAxisSeries, YAxis]] = None,
         legend_position: LegendPosition = LegendPosition.BOTTOM,
         title: WidgetTitleType = "",
         enable_toolbar: bool = True,
     ):
-        """Construct spec for the Cartesian widget.
+        """Constructor for Cartesian widget.
 
         Args:
             data: data to be used by widget. Accepts Storages as well as raw data.
             widget_id: unique widget id in a dashboard.
             x_axis: spec for X Axis.
             left_y_axis: spec for left Y Axis.
             right_y_axis: spec for right Y Axis
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/chart.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/chart.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/legend.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/legend.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/area.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/area.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/column.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/column.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/line.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/line.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/cartesian/series/typing.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/chart_utils.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/chart_utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class AxisScaleDynamic(AbstractFactory):
-    """Spec for dynamic scale for y axis.
+    """Dynamically set y-axis extremes for optimal spacing.
 
-    Axis extremes are calculated dynamically to minimize the amount of dead space
-        in a chart.
+    Construct specifications for a dynamic scale for the y-axis of a chart.
+    By default, it dynamically calculates axis extremes to minimize
+    dead space in the chart.
     """
 
     @type_check
     def __init__(self, *, tick_amount: int = 3):
-        """Construct dynamic scale for y axis.
+        """Constructor for AxisScaleDynamic.
 
         Args:
             tick_amount: number of ticks beyond min and max.
         """
         super().__init__()
         self.__tick_amount = tick_amount
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class AxisScaleNegative(AbstractFactory):
-    """Spec for scale for y axis with only negative values.
-
-    Assumes max value of chart to be fixed at 0.
+    """Y-axis scale for charts with negative values.
 
+    Construct specifications for a scale for the y-axis with only
+    negative values. It assumes the maximum value of the chart to
+    be fixed at 0. Specify a fixed minimum value for the axis with
+    the min_value parameter, which defaults to None, allowing
+    for dynamic calculation of the minimum value.
     """
 
     @type_check
     def __init__(
         self, *, min_value: Optional[int] = None, intermediate_tick_amount: int = 3
     ):
-        """Construct positive scale spec.
+        """Constructor for AxisScaleNegative.
 
         Args:
             min_value: fixed minimum value for axis.
                 Defaults to None (min value calculated dynamically)
             intermediate_tick_amount: number of extra ticks between extremes.
         """
         super().__init__()
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class AxisScalePositive(AbstractFactory):
-    """Spec for scale for y axis with only negative values.
-
-    Assumes min value of chart to be fixed at 0.
+    """Y-axis scale for charts with positive values.
 
+    Construct specifications for a scale for the y-axis with only
+    positive values. It assumes the minimum value of the chart to be
+    fixed at 0. Specify a fixed maximum value for the axis with the
+    max_value parameter, which defaults to None, allowing for
+    dynamic calculation of the maximum value.
     """
 
     @type_check
     def __init__(
         self, *, max_value: Optional[int] = None, intermediate_tick_amount: int = 3
     ):
-        """Construct positive scale spec.
+        """Constructor for AxisScalePositive.
 
         Args:
             max_value: fixed maximum value for axis.
                 Defaults to None (max value calculated dynamically)
             intermediate_tick_amount: number of extra ticks between extremes.
         """
         super().__init__()
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
     ChartScaleSymmetricValueError,
 )
 
 
 class AxisScaleSymmetric(AbstractFactory):
-    """Spec for scale for y axis with only positive and negative values.
-
-    Extremes determined by max(abs(data)) and 0 added as the middle tick.
+    """Y-axis scale for charts with positive and negative values.
 
+    Construct specifications for a scale for the y-axis with both
+    positive and negative values. It determines extremes based on
+    the maximum absolute value of the data, with 0 added as the middle tick.
     """
 
     @type_check
     def __init__(
         self,
         *,
         min_value: Optional[int] = None,
         max_value: Optional[int] = None,
         intermediate_tick_amount: int = 1,
         strict: Optional[bool] = None
     ):
-        """Construct symmetric y axis scale.
+        """Constructor for AxisScaleSymmetric.
 
         Args:
             min_value (Optional[int]): fixed minimum value for axis.
                 Defaults to None (calculated dynamically).
             max_value (Optional[int]): fixed maximum value for axis.
                 Defaults to None (calculated dynamically).
             intermediate_tick_amount (int): number of ticks between min-mid and
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/area.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/area.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
 class AreaSeriesStyling(BaseChartSeriesStyling):
-    """Spec to style an area series."""
+    """Customize appearance of filled areas in Charts.
+
+    Specify styling options for an area series within a Chart
+    widget to customize the appearance of filled areas on the chart.
+    """
 
     _API_TYPE = "ChartAreaSeriesStylingInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
-        """Construct style spec for area series.
+        """Constructor for AreaSeriesStyling.
 
         Args:
             color_spec: spec for coloring area.
             data_column: name of column in pandas dataframe(s) used for color spec if
                 a gradient is used. Optional for single colors.
             marker_symbol: symbol for marker in tooltips and legends.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,33 @@
-"""Spec to style an area range series."""
+"""Spec fot Number Styling Dot."""
+
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.styling.color.typing import ColorSpec
+from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
-from .base import BaseChartSeriesStyling
-from .enums import MarkerSymbol
+from ..base import BaseItemStyling
 
 
-class AreaRangeSeriesStyling(BaseChartSeriesStyling):
-    """Spec to style an area range series."""
+class NumberStylingDot(BaseItemStyling):
+    """Spec for Number Dot Styling class."""
 
-    _API_TYPE = "ChartAreaRangeSeriesStylingInput"
+    _API_TYPE = "NumberStylingDotInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
-        marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
-        """Construct style spec for area range series.
+        """Construct spec for Number Dot Styling.
 
         Args:
-            color_spec: spec for coloring area range.
-            data_column: name of column in pandas dataframe(s) used for color spec if
-                a gradient is used. Optional for single colors.
-            marker_symbol: symbol for marker in tooltips and legends.
-
-        Raises:
-            ChartStylingMissingDataColumnError: if color_spec is
-                ColorDiscreteMap/ColorGradient and data_column
-                has not been specified
+            color_spec (ColorSpec): specs for color.
+            data_column (Optional[TemplatedStringItem]): styling value key.
         """
         super().__init__(
-            color_spec=color_spec, data_column=data_column, marker_symbol=marker_symbol
+            color_spec=color_spec,
+            data_column=data_column,
         )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,29 +14,33 @@
 from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import ChartStylingNoDataColumnError
 from .base import BaseChartSeriesStyling
 
 
 class BubbleCircleSeriesStyling(BaseChartSeriesStyling):
-    """Spec to style a bubble series as circles."""
+    """Customize appearance of bubble markers.
+
+    Specify styling options for a bubble circle series within a Chart
+    widget to customize the appearance of bubble markers on the chart.
+    """
 
     _API_TYPE = "ChartBubbleSeriesStylingCircleInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         label_column: Optional[TemplatedStringItem] = None,
         max_size_percentage: Optional[Union[float, int]] = 0.5,
         min_size_percentage: Optional[Union[float, int]] = 0.2,
     ):
-        """Construct style spec for bubble series.
+        """Constructor for BubbleCircleSeriesStyling.
 
         Args:
             color_spec: spec for coloring bubble.
             data_column: name of column in pandas dataframe(s) used for color spec if
                 a gradient is used. Optional for single colors.
             label_column: name of column in pandas dataframe(s) used for labeling the
                 bubble.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.exceptions import (
     ChartStylingNoDataColumnError,
 )
 
 
 class BubbleCountrySeriesStyling(AbstractFactory):
-    """Spec to style a bubble series using country flags."""
+    """Customize appearance of country bubble markers.
+
+    Specify styling options for a bubble country series within a Chart widget
+    to customize the appearance of bubble markers representing countries on the chart.
+    """
 
     @type_check
     def __init__(
         self,
         *,
         country_column: TemplatedStringItem,
         max_size_percentage: Optional[Union[float, int]] = 0.5,
         min_size_percentage: Optional[Union[float, int]] = 0.2,
     ):
-        """Constructs country flags styling spec for bubble series.
+        """Constructor for BubbleCountrySeriesStyling.
 
         Args:
             country_column: name of column in pandas dataframe(s) with country codes.
             max_size_percentage: Percentage of the highest one of the plot width and
                 height.
             min_size_percentage: Percentage of the smallest one of the plot width and
                 height.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/column.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-"""Spec to style a column series."""
+"""Spec fot Text Styling Dot."""
+
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.styling.color.typing import ColorSpec
+from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
-from .base import BaseChartSeriesStyling
-from .enums import MarkerSymbol
+from ..base import BaseItemStyling
 
 
-class ColumnSeriesStyling(BaseChartSeriesStyling):
-    """Spec to style a column series."""
+class TextStylingDot(BaseItemStyling):
+    """Spec for Text Dot Styling Class."""
 
-    _API_TYPE = "ChartColumnSeriesStylingInput"
+    _API_TYPE = "TextStylingDotInput"
 
     @type_check
     def __init__(
         self,
         *,
-        color_spec: ColorSpec,
+        color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
-        marker_symbol: MarkerSymbol = MarkerSymbol.SQUARE,
     ):
-        """Construct style spec for column series.
+        """Construct spec for Text Dot Styling.
 
         Args:
-            color_spec: spec for coloring columns.
-            data_column: name of column in pandas dataframe(s) used for color spec if
-                a gradient is used. Optional for single colors.
-            marker_symbol: symbol for marker in tooltips and legends.
-
-        Raises:
-            ChartStylingMissingDataColumnError: if a data_column is not defined when
-                color_spec is a ColorDiscreteMap or ColorGradient
+            color_spec (Optional[ColorSpec): specs for color.
+            data_column (Optional[TemplatedStringItem]): styling value key.
+                Defaults to None.
         """
         super().__init__(
-            color_spec=color_spec, data_column=data_column, marker_symbol=marker_symbol
+            color_spec=color_spec,
+            data_column=data_column,
         )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
 class ErrorBarSeriesStyling(BaseChartSeriesStyling):
-    """Spec to style error bar series."""
+    """Customize appearance of error bars in Chart.
+
+    Specify styling options for an error bar series within a
+    Chart widget to customize the appearance of error bars
+    representing data variability or uncertainty on the chart.
+    """
 
     _API_TYPE = "ChartErrorBarSeriesStylingInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.SQUARE,
     ):
-        """Construct style spec for error bar series.
+        """Constructor for ErrorBarSeriesStyling.
 
         Args:
             color_spec: spec for coloring columns.
             data_column: name of column in pandas dataframe(s) used for color spec if
                 a gradient is used. Optional for single colors.
             marker_symbol: symbol for marker in tooltips and legends.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/line.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/line.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,29 +17,33 @@
 from ...items.styling.exceptions import StylingInvalidDashValuesError
 from .base import BaseChartSeriesStyling
 from .enums import DashStyle
 from .enums import MarkerSymbol
 
 
 class LineSeriesStyling(BaseChartSeriesStyling):
-    """Spec to style a line series."""
+    """Customize appearance of lines in Chart.
+
+    Specify styling options for a line series within a Chart widget
+    to customize the appearance of the lines connecting data points on the chart.
+    """
 
     _API_TYPE = "ChartLineSeriesStylingInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
         dash_style: Union[DashStyle, TemplatedStringItem] = DashStyle.SOLID,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
         width: int = 2,
     ):
-        """Construct style spec for line series.
+        """Constructor for LineSeriesStyling.
 
         Args:
             color_spec: spec for coloring area.
             data_column: name of column in pandas dataframe(s) used for color spec if
                 a gradient is used. Optional for single colors.
             dash_style: dash style of line.
             marker_symbol: symbol for marker in tooltips and legends.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/point.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-"""Spec to style a point series."""
+"""Spec fot Text Styling Font."""
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.styling.color.typing import ColorSpec
+from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
-from .base import BaseChartSeriesStyling
-from .enums import MarkerSymbol
+from ..base import BaseItemStyling
 
 
-class PointSeriesStyling(BaseChartSeriesStyling):
-    """Spec to style a point series."""
+class TextStylingChip(BaseItemStyling):
+    """Spec for Text Chip Styling Class."""
 
-    _API_TYPE = "ChartPointSeriesStylingInput"
+    _API_TYPE = "TextStylingChipInput"
 
     @type_check
     def __init__(
         self,
         *,
-        color_spec: ColorSpec,
+        color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
-        marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
-        """Construct style spec for point series.
+        """Construct spec for Text Chip Styling.
 
         Args:
-            color_spec: spec for coloring columns.
-            data_column: name of column in pandas dataframe(s) used for color spec if
-                a gradient is used. Optional for single colors.
-            marker_symbol: symbol for each point.
-
-        Raises:
-            ChartStylingMissingDataColumnError: if a data_column is not defined when
-                color_spec is a ColorDiscreteMap or ColorGradient
+            color_spec (Optional[ColorSpec]): specs for color.
+            data_column (Optional[TemplatedStringItem]): styling value key.
         """
-        super().__init__(
-            color_spec=color_spec, data_column=data_column, marker_symbol=marker_symbol
-        )
+        super().__init__(data_column=data_column, color_spec=color_spec)
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseChartSeriesStyling
 from .enums import MarkerSymbol
 
 
 class ScatterSeriesStyling(BaseChartSeriesStyling):
-    """Spec to style a scatter series."""
+    """Customize appearance of scatter markers.
+
+    Specify styling options for a scatter series within a Timeseries
+    widget to customize the appearance of individual data points
+    represented as scatter markers on the chart.
+    """
 
     _API_TYPE = "ChartScatterSeriesStylingInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
         marker_symbol: MarkerSymbol = MarkerSymbol.CIRCLE,
     ):
-        """Construct style spec for scatter series.
+        """Constructor for ScatterSeriesStyling.
 
         Args:
             color_spec: spec for coloring columns.
             data_column: name of column in pandas dataframe(s) used for color spec if
                 a gradient is used. Optional for single colors.
             marker_symbol: symbol for each point.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,46 @@
-"""Specs for category item for a tooltip."""
+"""Specs for number item for a tooltip."""
 
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.formatting import MapperFormatting
+from engineai.sdk.dashboard.formatting import NumberFormatting
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseTooltipItem
 
 
-class CategoryTooltipItem(BaseTooltipItem):
-    """Specs for category tooltip item."""
+class NumberTooltipItem(BaseTooltipItem):
+    """Customize tooltips for numerical data in Chart.
 
-    _API_TYPE = "TooltipCategoricalItemInput"
+    Define specifications for a number item within a tooltip for a Chart
+    widget to customize the appearance and content of tooltips displayed
+    for numerical data.
+    """
+
+    _API_TYPE = "TooltipNumberItemInput"
 
     @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
-        formatting: MapperFormatting,
+        formatting: Optional[NumberFormatting] = None,
         label: Optional[Union[str, DataField]] = None,
     ):
-        """Construct category tooltip item.
+        """Constructor for NumberTooltipItem.
 
         Args:
-            data_column (TemplatedStringItem): name of column in pandas dataframe(s)
-                used for the value of the tooltip item.
-            formatting (MapperFormatting): tooltip formatting spec.
-            label (Optional[Union[str, DataField]]): label to be used for tooltip item,
-                it can be either a string or a DataField object.
+            data_column: name of column in pandas dataframe(s) used for the value of
+                the tooltip item.
+            formatting: tooltip formatting spec.
+                Defaults to None (Base NumberFormatting).
+            label: label to be used for tooltip item, it can be either a string or a
+                DataField object.
         """
         super().__init__(
             data_column=data_column,
-            formatting=formatting,
+            formatting=formatting if formatting is not None else NumberFormatting(),
             label=label,
         )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,27 +8,32 @@
 from engineai.sdk.dashboard.templated_string import DataField
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from .base import BaseTooltipItem
 
 
 class DatetimeTooltipItem(BaseTooltipItem):
-    """Specs for datetime item for a tooltip."""
+    """Customize tooltips for datetime data in Chart.
+
+    Define specifications for a datetime item within a tooltip for a
+    Chart widget to customize the appearance and content
+    of tooltips displayed for datetime data.
+    """
 
     _API_TYPE = "TooltipDateTimeItemInput"
 
     @type_check
     def __init__(
         self,
         *,
         data_column: TemplatedStringItem,
         formatting: Optional[DateTimeFormatting] = None,
         label: Optional[Union[str, DataField]] = None,
     ):
-        """Construct datetime tooltip item.
+        """Constructor for DatetimeTooltipItem.
 
         Args:
             data_column (TemplatedStringItem): name of column in pandas dataframe(s)
                 used for the value of the tooltip item.
             formatting (DateTimeFormatting): tooltip formatting spec
                 Defaults to DateTimeFormatting for Dates (i.e. not include HH:MM).
             label (Optional[Union[str, DataField]]): label to be used for tooltip item,
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,30 @@
-"""Specs for number item for a tooltip."""
-
+"""Spec fot Text Styling Font."""
 from typing import Optional
-from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.formatting import NumberFormatting
-from engineai.sdk.dashboard.templated_string import DataField
+from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
-from .base import BaseTooltipItem
+from ..base import BaseItemStyling
 
 
-class NumberTooltipItem(BaseTooltipItem):
-    """Specs for number item for a tooltip."""
+class TextStylingFont(BaseItemStyling):
+    """Spec for Text Font Styling Class."""
 
-    _API_TYPE = "TooltipNumberItemInput"
+    _API_TYPE = "TextStylingFontInput"
 
     @type_check
     def __init__(
         self,
         *,
-        data_column: TemplatedStringItem,
-        formatting: Optional[NumberFormatting] = None,
-        label: Optional[Union[str, DataField]] = None,
+        color_spec: Optional[ColorSpec] = None,
+        data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct number tooltip item.
+        """Construct spec for Text Font Styling.
 
         Args:
-            data_column: name of column in pandas dataframe(s) used for the value of
-                the tooltip item.
-            formatting: tooltip formatting spec.
-                Defaults to None (Base NumberFormatting).
-            label: label to be used for tooltip item, it can be either a string or a
-                DataField object.
+            color_spec (ColorSpec): specs for color.
+            data_column (Optional[TemplatedStringItem]): styling value key.
+                Defaults to None.
         """
-        super().__init__(
-            data_column=data_column,
-            formatting=formatting if formatting is not None else NumberFormatting(),
-            label=label,
-        )
+        super().__init__(data_column=data_column, color_spec=color_spec)
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-"""Specs for text item for a tooltip."""
-
+"""Specification for styling a column with a country flag to a value."""
+from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.formatting import TextFormatting
-from engineai.sdk.dashboard.templated_string import DataField
-from engineai.sdk.dashboard.templated_string import TemplatedStringItem
+from engineai.sdk.dashboard.links import WidgetField
+
+from .base import TableColumnStylingBase
 
-from .base import BaseTooltipItem
 
+class CountryFlagStyling(TableColumnStylingBase):
+    """Styling options for country flag column.
 
-class TextTooltipItem(BaseTooltipItem):
-    """Specs for text item for a tooltip."""
+    Specify the styling options for a country flag column
+    in the table widget, including position and data column.
+    """
 
-    _API_TYPE = "TooltipTextItemInput"
+    _API_TYPE = "TableColumnStylingCountryFlagInput"
 
     @type_check
     def __init__(
         self,
         *,
-        data_column: TemplatedStringItem,
-        formatting: Optional[TextFormatting] = None,
-        label: Optional[Union[str, DataField]] = None,
+        left: bool = True,
+        data_column: Optional[Union[str, WidgetField]] = None,
     ):
-        """Construct text tooltip item.
+        """Constructor for CountryFlagStyling.
 
         Args:
-            data_column (TemplatedStringItem): name of column in pandas dataframe(s)
-                used for the value of the tooltip item.
-            formatting (Optional[TextFormatting]): tooltip formatting spec.
-                Defaults to TextFormatting(max_characters=30).
-            label (Optional[Union[str, DataField]]): label to be used for tooltip item,
-                it can be either a string or a DataField object.
+            data_column: id of column which values are used to determine behavior of
+                arrow.
+                By default, will use values of column to which styling is applied.
+            left: whether to put flag to the left (True) or right (False) of column
+                value.
         """
-        super().__init__(
-            data_column=data_column,
-            formatting=formatting if formatting is not None else TextFormatting(),
-            label=label,
-        )
+        super().__init__(data_column=data_column, color_spec=None)
+        self.__left = left
+
+    def _build_extra_inputs(self) -> Dict[str, Any]:
+        return {"left": self.__left}
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/charts/typing.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-"""Spec fot Number Styling Dot."""
+"""Spec fot Number Styling Font."""
 
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
 from ..base import BaseItemStyling
 
 
-class NumberStylingDot(BaseItemStyling):
-    """Spec for Number Dot Styling class."""
+class NumberStylingFont(BaseItemStyling):
+    """Spec for Number Font Styling class."""
 
-    _API_TYPE = "NumberStylingDotInput"
+    _API_TYPE = "NumberStylingFontInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Number Dot Styling.
+        """Construct spec for Number Font Styling.
 
         Args:
-            color_spec (ColorSpec): specs for color.
+            color_spec (Optional[ColorSpec): specs for color.
             data_column (Optional[TemplatedStringItem]): styling value key.
+                Defaults to None.
         """
-        super().__init__(
-            color_spec=color_spec,
-            data_column=data_column,
-        )
+        super().__init__(data_column=data_column, color_spec=color_spec)
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-"""Spec fot Number Styling Font."""
-
+"""Spec for Number Styling Progress Bar."""
+from typing import Any
 from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.styling.color.spec import ColorSpec
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-
-from ..base import BaseItemStyling
+from engineai.sdk.dashboard.templated_string import build_templated_strings
+from engineai.sdk.dashboard.utils import generate_input
+from engineai.sdk.dashboard.widgets.components.items.styling.base import BaseItemStyling
 
 
-class NumberStylingFont(BaseItemStyling):
-    """Spec for Number Font Styling class."""
+class NumberStylingProgressBar(BaseItemStyling):
+    """Spec for Number Styling Progress Bar class."""
 
-    _API_TYPE = "NumberStylingFontInput"
+    _API_TYPE = "NumberStylingProgressBarInput"
 
     @type_check
     def __init__(
         self,
         *,
-        color_spec: ColorSpec,
-        data_column: Optional[TemplatedStringItem] = None,
+        column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Number Font Styling.
+        """Construct spec for Number Styling Progress Bar.
 
         Args:
-            color_spec (Optional[ColorSpec): specs for color.
-            data_column (Optional[TemplatedStringItem]): styling value key.
+            column (Optional[TemplatedStringItem]): styling value key.
                 Defaults to None.
         """
-        super().__init__(data_column=data_column, color_spec=color_spec)
+        super().__init__(data_column=column)
+
+    def build(self) -> Any:
+        """Method implemented by all factories to generate Input spec.
+
+        Returns:
+            Input object for Dashboard API
+        """
+        return generate_input(
+            self._api_type,
+            valueKey=build_templated_strings(items=self.column),
+        )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/content.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/content.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/item.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/item.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/content/markdown.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/markdown.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/enums.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/enums.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Specs for Position and Region."""
 import enum
 
 
 class LegendPosition(enum.Enum):
-    """Options for positions of Map legend.
+    """Legend positioning options on map.
+
+    Options for positioning the legend on the map,
+    including top, left, right, and bottom.
 
     Attributes:
         TOP: Legend is placed on the top of the map.
         LEFT: Legend is placed on the left side of the map.
         RIGHT: Legend is placed on the right side of the map.
         BOTTOM: Legend is placed on the bottom of the map.
     """
@@ -15,20 +18,25 @@
     TOP = "TOP"
     LEFT = "LEFT"
     RIGHT = "RIGHT"
     BOTTOM = "BOTTOM"
 
 
 class Region(enum.Enum):
-    """Options for region.
+    """Region options for map.
+
+    Options for defining the region of the map,
+    such as world, Europe, USA, and North America.
 
     Attributes:
         WORLD: World region.
         EUROPE: Europe region.
         USA: USA region.
         NORTH_AMERICA: North America region.
+        SAUDI_ARABIA: Saudi Arabia region.
     """
 
     WORLD = "WORLD"
     EUROPE = "EUROPE"
     USA = "USA"
     NORTH_AMERICA = "NORTH_AMERICA"
+    SAUDI_ARABIA = "SAUDI_ARABIA"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.number import (
     NumberTooltipItem,
 )
 from engineai.sdk.dashboard.widgets.components.charts.tooltip.text import (
     TextTooltipItem,
 )
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
+from engineai.sdk.dashboard.widgets.maps.color_axis import ColorAxis
 from engineai.sdk.dashboard.widgets.maps.enums import LegendPosition
 from engineai.sdk.dashboard.widgets.maps.enums import Region
 from engineai.sdk.dashboard.widgets.maps.exceptions import MapColumnDataNotFoundError
+from engineai.sdk.dashboard.widgets.maps.geo.styling.styling import MapStyling
 from engineai.sdk.dashboard.widgets.maps.legend import Legend
 from engineai.sdk.dashboard.widgets.maps.series.numeric import NumericSeries
 
 from ...base import Widget
 from ...base import WidgetTitleType
 from ...utils import build_data
 from ...utils import get_tooltips
@@ -58,28 +60,32 @@
         self,
         data: Union[DataSource, T, Http],
         *,
         series: Optional[MapSeries] = None,
         region_column: str = "region",
         widget_id: Optional[str] = None,
         title: Optional[WidgetTitleType] = None,
+        color_axis: Optional[ColorAxis] = None,
         legend_position: LegendPosition = LegendPosition.BOTTOM,
+        styling: Optional[MapStyling] = None,
         region: Region = Region.WORLD,
         tooltips: Optional[TooltipItems] = None,
     ):
         """Construct spec for the Base Map Geo class.
 
         Args:
             data: data source for the widget.
             series: Series to be added to y axis.
             region_column: key to match region code in DS.
             widget_id: unique widget id in a dashboard.
             title: title of widget can be either a string (fixed value) or determined
                 by a value from another widget using a WidgetField.
+            styling: styling for the map.
             legend_position: location of position relative to data, maps.
+            color_axis: color axis spec.
             region: sets the region os the Map.
             tooltips: tooltip items to be displayed at Chart level.
 
         Examples:
             >>> # Create a minimal map widget
             >>> import pandas as pd
             >>> from engineai.sdk.dashboard.dashboard import Dashboard
@@ -91,14 +97,16 @@
             ...     ]
             ... )
             >>> Dashboard(content=maps.Geo(data=data))
         """
         super().__init__(data=data, widget_id=widget_id)
         self._title = title
         self._legend_position = Legend(position=legend_position)
+        self._color_axis = color_axis if color_axis else ColorAxis()
+        self._styling = styling if styling is not None else MapStyling()
         self._series: List[MapSeries] = [series] if series else [NumericSeries()]
         self._region = region
         self._region_column = region_column
         self._extra_tooltip_items = get_tooltips(tooltips)
         self._auto_generate_tooltips(
             data=data, series=series, region_column=region_column
         )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/geo/geo.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/geo.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,48 +8,58 @@
 
 from engineai.sdk.dashboard.data import DataSource
 from engineai.sdk.dashboard.data.http import Http
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
+from engineai.sdk.dashboard.widgets.maps.color_axis import ColorAxis
 from engineai.sdk.dashboard.widgets.maps.enums import LegendPosition
 from engineai.sdk.dashboard.widgets.maps.enums import Region
 
 from ...base import WidgetTitleType
 from ..series.series import MapSeries
 from .base import BaseMapGeo
+from .styling.styling import MapStyling
 
 
 class Geo(BaseMapGeo[pd.DataFrame]):
-    """Spec for MapGeo widget."""
+    """Widget for tailored geographic data visualization.
+
+    Allows the construction of a widget specifically tailored
+    for geographical data visualization.
+    """
 
     @type_check
     def __init__(
         self,
         data: Union[DataSource, pd.DataFrame, Http],
         *,
         series: Optional[MapSeries] = None,
         region_column: str = "region",
+        color_axis: Optional[ColorAxis] = None,
         widget_id: Optional[str] = None,
         title: Optional[WidgetTitleType] = None,
         legend_position: LegendPosition = LegendPosition.BOTTOM,
+        styling: Optional[MapStyling] = None,
         region: Region = Region.WORLD,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct spec for the Map Geo widget.
+        """Constructor for Map Geo widget.
 
         Args:
             data: data source for the widget.
             series: Series to be added to y axis.
             region_column: key to match region code in DS.
             widget_id: unique widget id in a dashboard.
+            color_axis: color axis spec.
             title: title of widget can be either a string (fixed value) or determined
                 by a value from another widget using a WidgetField.
             legend_position: location of position relative to data, maps.
+            styling: styling for the map.
             region: sets the region os the Map.
             tooltips: tooltip items to be displayed at Chart level.
 
         Examples:
             ??? example "Create a minimal Map widget"
                 ```python linenums="1"
                 import pandas as pd
@@ -67,40 +77,33 @@
         super().__init__(
             data=data,
             series=series,
             region_column=region_column,
             widget_id=widget_id,
             title=title,
             legend_position=legend_position,
+            color_axis=color_axis,
+            styling=styling,
             region=region,
             tooltips=tooltips,
         )
 
     def _build_widget_input(self) -> Any:
         """Method to build map widget."""
         return generate_input(
             "MapGeoWidgetInput",
             title=build_templated_strings(items=self._title) if self._title else None,
-            colorAxis=self._build_color_axis(),  # not being used by API for now.
+            colorAxis=self._color_axis.build(),
             legend=self._legend_position.build(),
             series=self._build_series(),
             region=self._region.value,
+            styling=self._styling.build(),
             tooltip=self._build_tooltips(),
         )
 
-    def _build_color_axis(self) -> Any:
-        """Method implemented by all factories to generate Input spec.
-
-        Returns:
-            Input object for Dashboard API
-        """
-        return generate_input(
-            "MapWidgetColorAxisInput", position=LegendPosition.BOTTOM.value
-        )
-
     def validate(self, data: pd.DataFrame, **kwargs: Any) -> None:
         """Validates widget spec.
 
         Args:
             data: pandas DataFrame where
                 the data is present.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/legend.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/legend.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Legend(AbstractFactory):
     """Spec for legend of a Map widget."""
 
     @type_check
     def __init__(self, *, position: LegendPosition = LegendPosition.BOTTOM):
-        """Construct a legend for a Map Shape widget.
+        """Constructor for Legend.
 
         Args:
             position (Position): location of position
                 relative to data, maps.
         """
         super().__init__()
         self.__position = position
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/numeric.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/numeric.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         data_column: TemplatedStringItem = "value",
         name: Optional[TemplatedStringItem] = None,
         formatting: Optional[NumberFormatting] = None,
         styling: Optional[Union[Palette, SeriesStyling]] = None,
         required: bool = True,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct numeric series.
+        """Constructor for NumericSeries.
 
         Args:
             data_column: data column to match field in DataStore.
             name: series name (shown in legend and tooltip).
             formatting: formatting spec for value.
             styling: styling spec.
             required: Flag to make the Series mandatory. If required == True and no
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/series.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/series.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/maps/series/styling.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,98 @@
-"""Spec to style a line series."""
+"""Spec for Search Widget Result Column Style."""
 
 from typing import Any
 from typing import Optional
 
 import pandas as pd
 
-from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.discrete_map import DiscreteMap
 from engineai.sdk.dashboard.styling.color.gradient import Gradient
 from engineai.sdk.dashboard.styling.color.palette import Palette
-from engineai.sdk.dashboard.styling.color.single import Single
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
+from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
-from engineai.sdk.dashboard.widgets.components.charts.styling.enums import MarkerSymbol
-from engineai.sdk.dashboard.widgets.maps.exceptions import MapColumnDataNotFoundError
 
+from ...exceptions import SearchStylingMissingDataColumnError
+from ...exceptions import SearchValidateNoDataColumnError
 
-class SeriesStyling:
-    """Spec to style a numeric series."""
 
-    @type_check
+class ResultColumnStyling:
+    """Spec for Search Widget Result Column Style."""
+
+    _API_TYPE: Optional[str] = None
+
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
-        data_column: Optional[str] = None,
+        data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct style spec for numeric series.
+        """Construct for Search Widget Result Column Style.
 
         Args:
-            color_spec: spec for coloring area
-            data_column: name of column in pandas dataframe(s) used for color spec if
-                a gradient is used. Optional for single colors.
-
-        Raises:
-            ValueError: if color_spec is ColorDiscreteMap/ColorGradient and data_column
-                has not been specified.
+            color_spec: Spec for coloring columns.
+            data_column: Name of column in pandas
+                dataframe(s) used for color spec if a gradient is used. Optional for
+                single colors.
         """
         super().__init__()
-        if not data_column and isinstance(color_spec, (DiscreteMap, Gradient)):
-            raise ValueError(
-                "data_column argument cannot be None if color_spec is "
-                "ColorDiscreteMap or ColorGradient"
-            )
+        if (
+            color_spec is not None
+            and isinstance(color_spec, (DiscreteMap, Gradient))
+            and data_column is None
+        ):
+            raise SearchStylingMissingDataColumnError()
         self.__color_spec = color_spec or Palette.AQUA_GREEN
         self.__data_column = data_column
 
+    @property
+    def _api_type(self) -> str:
+        """Returns styling API type argument value.
+
+        All Select Layout Items must now have the _API_TYPE defined.
+        """
+        if self._API_TYPE is None:
+            raise NotImplementedError(
+                f"Class {self.__class__.__name__}._API_TYPE not defined."
+            )
+        return self._API_TYPE
+
     def validate(
         self,
         *,
         data: pd.DataFrame,
     ) -> None:
-        """Validate if dataframe that will be used for column contains required columns.
+        """Validate if data has the right columns.
 
         Args:
-            data: pandas dataframe which will be used for table
+            data: pandas dataframe which will be used for table.
 
         Raises:
-            ValueError: if data does not contain data_column
+            SearchValidateNoDataColumnError: if data does not contain data_column
         """
         if (
-            not isinstance(self.__color_spec, Single)
-            and self.__data_column
+            isinstance(self.__data_column, str)
             and self.__data_column not in data.columns
         ):
-            raise MapColumnDataNotFoundError(column_data=self.__data_column)
+            raise SearchValidateNoDataColumnError(data_column=self.__data_column)
+
+        # TODO: Validate abstractLinks if used (widgetField, f.e)
 
     def build(self) -> Any:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
         return generate_input(
-            "MapWidgetSeriesStylingInput",
-            colorSpec=build_color_spec(spec=self.__color_spec),
-            markerSymbol=MarkerSymbol.CIRCLE.value,
+            self._api_type,
+            chip=generate_input(
+                "SearchWidgetResultColumnChipStylingInput",
+                colorSpec=build_color_spec(spec=self.__color_spec)
+                if self.__color_spec
+                else None,
+                dataKey=build_templated_strings(items=self.__data_column),
+            ),
         )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pandas_utils.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/__init__.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/chart.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """Spec for Pie Chart."""
 
     def __init__(
         self,
         series: ChartSeries,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct spec for Pie Chart.
+        """Constructor for Pie Chart.
 
         Args:
             series: spec for series.
             tooltips: tooltip items to be displayed at Chart level.
         """
         self._series = series
         self._tooltip = Tooltip(
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/pie.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/pie.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 from .legend import LegendPosition
 from .legend import build_legend
 from .series.series import Series
 from .series.typings import ChartSeries
 
 
 class Pie(Widget):
-    """Spec for Pie Widget."""
+    """Construct pie chart widget.
+
+    Construct a pie chart widget for visualizing data distribution,
+    allowing customization of legends, tooltips, and series.
+    """
 
     _WIDGET_API_TYPE = "pie"
     _DEPENDENCY_ID = "__PIE_DATA_DEPENDENCY__"
 
     @type_check
     def __init__(
         self,
@@ -50,15 +54,15 @@
         *,
         series: Optional[ChartSeries] = None,
         legend_position: LegendPosition = LegendPosition.BOTTOM,
         widget_id: Optional[str] = None,
         title: Optional[WidgetTitleType] = None,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct spec for the Pie Widget.
+        """Constructor for Pie widget.
 
         Args:
             data: data for the widget. Can be a pandas dataframe or DataStorage object
                 if the data is to be retrieved from a storage.
             widget_id: unique widget id in a dashboard.
             title: title of widget can be either a string (fixed value) or determined
                 by a value from another widget using a WidgetLink.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/country.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/country.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .base import BaseSeries
 from .styling import SeriesStyling
 
 
 class CountrySeries(BaseSeries):
-    """Spec for Pie Country Series."""
+    """Define country-based pie chart series.
+
+    Define a series specifically for pie charts representing data
+    categorized by country, with options for customizing country code
+    column, data column, formatting, styling, and tooltips.
+    """
 
     _API_TYPE = "PieWidgetChartSeriesCountryInput"
     _INPUT_KEY = "country"
 
     @type_check
     def __init__(
         self,
@@ -30,15 +35,15 @@
         name: TemplatedStringItem = "Country Series",
         country_column: TemplatedStringItem = "country_code",
         data_column: TemplatedStringItem = "value",
         formatting: Optional[NumberFormatting] = None,
         styling: Optional[Union[Palette, SeriesStyling]] = None,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct spec for Pie Series.
+        """Constructor for CountrySeries.
 
         Args:
             name: name for the Pie series.
             country_column: name of column in pandas dataframe(s) that has country code
                 within the pie.
             data_column: name of column in pandas dataframe(s) that has pie data.
             formatting: spec for number formatting.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/series.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/series.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 from engineai.sdk.dashboard.widgets.components.charts.typing import TooltipItems
 
 from .base import BaseSeries
 from .styling import SeriesStyling
 
 
 class Series(BaseSeries):
-    """Spec for Pie Series."""
+    """Define pie chart series.
+
+    Define a generic series for the pie chart, specifying
+    category and data columns, formatting, styling, and tooltips.
+    """
 
     _API_TYPE = "PieWidgetChartSeriesStandardInput"
     _INPUT_KEY = "standard"
 
     @type_check
     def __init__(
         self,
@@ -27,15 +31,15 @@
         name: TemplatedStringItem = "Series",
         category_column: TemplatedStringItem = "category",
         data_column: TemplatedStringItem = "value",
         formatting: Optional[NumberFormatting] = None,
         styling: Optional[Union[Palette, SeriesStyling]] = None,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct spec for Pie Series.
+        """Constructor for Series.
 
         Args:
             name: name for the Pie series.
             category_column: name of column in pandas dataframe(s) that has category
                 info within the pie.
             data_column: name of column in pandas dataframe(s) that has pie data.
             formatting: spec for number formatting.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/series/styling.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/styling.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.widgets.components.charts.styling.base import (
     BaseChartSeriesStyling,
 )
 
 
 class SeriesStyling(BaseChartSeriesStyling):
-    """Spec for Pie Series Styling."""
+    """Style pie chart series.
+
+    Specify styling options for pie chart series, including
+    color specifications and data column mapping.
+    """
 
     _API_TYPE = "ChartPieSeriesStylingInput"
 
     @type_check
     def __init__(
         self,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[TemplatedStringItem] = None,
     ):
-        """Construct spec for Pie Series Styling.
+        """Constructor for SeriesStyling.
 
         Args:
             color_spec: specs for color.
             data_column: name of column in pandas dataframe(s)
                 that has the styling value.
 
         Examples:
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/pie/tooltip.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/tooltip.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """Spec for Pie Tooltip."""
 
     def __init__(
         self,
         category_column: TemplatedStringItem,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct spec for Pie Tooltip.
+        """Constructor for Pie Tooltip.
 
         Args:
             category_column: name of column in pandas dataframe(s)
                 that has category info within the pie.
             tooltips: tooltip items to be displayed at Chart level.
         """
         self._tooltips = (
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/build_result.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/build_result.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/number.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/number.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,29 @@
 from engineai.sdk.dashboard.widgets.search.results.base import BaseResultItem
 from engineai.sdk.dashboard.widgets.search.results.styling.number import (
     ResultNumberStyling,
 )
 
 
 class ResultNumberItem(BaseResultItem):
-    """Specs for Search Result Column Number."""
+    """Define number item for search results.
+
+    Define a number item for search results, specifying the data column
+    to display, formatting options, and styling options.
+    """
 
     _API_TYPE = "SearchWidgetResultColumnNumberInput"
 
     def __init__(
         self,
         data_column: TemplatedStringItem,
         formatting: Optional[NumberFormatting] = None,
         styling: Optional[Union[Palette, ResultNumberStyling]] = None,
     ) -> None:
-        """Constructor for Search Result Column Number.
+        """Constructor for ResultNumberItem.
 
         Args:
             data_column: Column name in pandas DataFrame used for
                 search result.
             formatting: formatting spec.
             styling: Specs for Search Result styling.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/styling.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,85 @@
-"""Spec for Search Widget Result Column Style."""
+"""Spec to style a line series."""
 
 from typing import Any
 from typing import Optional
 
 import pandas as pd
 
+from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.styling.color.discrete_map import DiscreteMap
 from engineai.sdk.dashboard.styling.color.gradient import Gradient
 from engineai.sdk.dashboard.styling.color.palette import Palette
+from engineai.sdk.dashboard.styling.color.single import Single
 from engineai.sdk.dashboard.styling.color.spec import build_color_spec
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
-from engineai.sdk.dashboard.templated_string import TemplatedStringItem
-from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
+from engineai.sdk.dashboard.widgets.components.charts.styling.enums import MarkerSymbol
+from engineai.sdk.dashboard.widgets.maps.exceptions import MapColumnDataNotFoundError
 
-from ...exceptions import SearchStylingMissingDataColumnError
-from ...exceptions import SearchValidateNoDataColumnError
 
+class SeriesStyling:
+    """Style numeric series appearance on map.
 
-class ResultColumnStyling:
-    """Spec for Search Widget Result Column Style."""
-
-    _API_TYPE: Optional[str] = None
+    Style the appearance of numeric series on a map,
+    including color specifications and data column mapping for
+    gradients or discrete maps.
+    """
 
+    @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
-        data_column: Optional[TemplatedStringItem] = None,
+        data_column: Optional[str] = None,
     ):
-        """Construct for Search Widget Result Column Style.
+        """Constructor for SeriesStyling.
 
         Args:
-            color_spec: Spec for coloring columns.
-            data_column: Name of column in pandas
-                dataframe(s) used for color spec if a gradient is used. Optional for
-                single colors.
+            color_spec: spec for coloring area
+            data_column: name of column in pandas dataframe(s) used for color spec if
+                a gradient is used. Optional for single colors.
+
+        Raises:
+            ValueError: if color_spec is ColorDiscreteMap/ColorGradient and data_column
+                has not been specified.
         """
         super().__init__()
-        if (
-            color_spec is not None
-            and isinstance(color_spec, (DiscreteMap, Gradient))
-            and data_column is None
-        ):
-            raise SearchStylingMissingDataColumnError()
+        if not data_column and isinstance(color_spec, (DiscreteMap, Gradient)):
+            raise ValueError(
+                "data_column argument cannot be None if color_spec is "
+                "ColorDiscreteMap or ColorGradient"
+            )
         self.__color_spec = color_spec or Palette.AQUA_GREEN
         self.__data_column = data_column
 
-    @property
-    def _api_type(self) -> str:
-        """Returns styling API type argument value.
-
-        All Select Layout Items must now have the _API_TYPE defined.
-        """
-        if self._API_TYPE is None:
-            raise NotImplementedError(
-                f"Class {self.__class__.__name__}._API_TYPE not defined."
-            )
-        return self._API_TYPE
-
     def validate(
         self,
         *,
         data: pd.DataFrame,
     ) -> None:
-        """Validate if data has the right columns.
+        """Validate if dataframe that will be used for column contains required columns.
 
         Args:
-            data: pandas dataframe which will be used for table.
+            data: pandas dataframe which will be used for table
 
         Raises:
-            SearchValidateNoDataColumnError: if data does not contain data_column
+            ValueError: if data does not contain data_column
         """
         if (
-            isinstance(self.__data_column, str)
+            not isinstance(self.__color_spec, Single)
+            and self.__data_column
             and self.__data_column not in data.columns
         ):
-            raise SearchValidateNoDataColumnError(data_column=self.__data_column)
-
-        # TODO: Validate abstractLinks if used (widgetField, f.e)
+            raise MapColumnDataNotFoundError(column_data=self.__data_column)
 
     def build(self) -> Any:
         """Method implemented by all factories to generate Input spec.
 
         Returns:
             Input object for Dashboard API
         """
         return generate_input(
-            self._api_type,
-            chip=generate_input(
-                "SearchWidgetResultColumnChipStylingInput",
-                colorSpec=build_color_spec(spec=self.__color_spec)
-                if self.__color_spec
-                else None,
-                dataKey=build_templated_strings(items=self.__data_column),
-            ),
+            "MapWidgetSeriesStylingInput",
+            colorSpec=build_color_spec(spec=self.__color_spec),
+            markerSymbol=MarkerSymbol.CIRCLE.value,
         )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/number.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/number.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Spec for Number Search Result styling."""
 from .base_styling import ResultColumnStyling
 
 
 class ResultNumberStyling(ResultColumnStyling):
-    """Construct for Search Widget Result Column Number Style.
+    """Style number search result columns.
+
+    Specify styling options for number search result columns,
+    including color specifications and data column mapping.
 
     Examples:
         ??? example "Changing the color of a number search result item"
             ```py linenums="1"
             #
             import pandas as pd
             from engineai.sdk.dashboard.dashboard import Dashboard
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/styling/text.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Spec for Text Search Result styling."""
 from .base_styling import ResultColumnStyling
 
 
 class ResultTextStyling(ResultColumnStyling):
-    """Construct for Search Widget Result Column Text Style.
+    """Style text search result columns.
+
+    Specify styling options for text search result columns,
+    including color specifications and data column mapping.
 
     Args:
         color_spec (Optional[ColorSpec]): Spec for coloring columns.
         data_column (Optional[TemplatedStringItem]): Name of column in pandas
             dataframe(s) used for color spec if a gradient is used. Optional for
             single colors.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/results/text.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,29 @@
     SearchValidateNoValidDataTypeError,
 )
 from engineai.sdk.dashboard.widgets.search.results.base import BaseResultItem
 from engineai.sdk.dashboard.widgets.search.results.styling.text import ResultTextStyling
 
 
 class ResultTextItem(BaseResultItem):
-    """Specs for Search Result Column Text."""
+    """Define text item for search results.
+
+    Define a text item for search results, specifying the data column
+    to display, whether it's searchable, and styling options.
+    """
 
     _API_TYPE = "SearchWidgetResultColumnTextInput"
 
     def __init__(
         self,
         data_column: TemplatedStringItem,
         searchable: bool = True,
         styling: Optional[Union[Palette, ResultTextStyling]] = None,
     ) -> None:
-        """Constructor for Search Result Column Text.
+        """Constructor for ResultTextItem.
 
         Args:
             data_column: Column name in pandas DataFrame used for
                 search result.
             searchable: Flag that makes the result searchable.
             styling: Specs for Search Result styling.
         """
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/search/search.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,20 @@
 from .exceptions import SearchNoSearchableColumnError
 from .exceptions import SearchValidateNoDataColumnError
 from .exceptions import SearchValidateNoValidDataTypeError
 from .results.build_result import build_search_result
 
 
 class Search(SelectableWidget):
-    """Specs for Search Widget."""
+    """Construct search widget.
+
+    Construct a search widget for searching through data, allowing
+    customization of selected text column, widget ID, search items,
+    and placeholder text.
+    """
 
     _WIDGET_API_TYPE = "search"
     _DEPENDENCY_ID = "__SEARCH_DATA_DEPENDENCY__"
     _DEFAULT_HEIGHT = 0.6
     _FORCE_HEIGHT = True
 
     @type_check
@@ -43,15 +48,15 @@
         *,
         data: Union[DataSource, pd.DataFrame, Http],
         selected_text_column: TemplatedStringItem,
         widget_id: Optional[str] = None,
         items: Optional[Union[TemplatedStringItem, List[ResultItemType]]] = None,
         placeholder: Optional[TemplatedStringItem] = None,
     ):
-        """Construct for Search widget.
+        """Constructor for Search widget.
 
         Args:
             data: data source for the widget.
             selected_text_column: Column with information to show
                 when the option is selected.
             widget_id: widget ID.
             items: List of ResultItemTypes to be displayed in the search results.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/group.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/group.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/select/select.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/select.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,21 @@
 from ..base import SelectableWidget
 from .exceptions import SelectValidateUniqueIDError
 from .exceptions import SelectValidateValueError
 from .group import Group
 
 
 class Select(SelectableWidget):
-    """Spec for Select widget."""
+    """Construct select widget.
+
+    Construct a select widget for choosing from a list of options,
+    with options to customize the data source, ID column,
+    default selection, label column, widget ID, label text,
+    grouping, and label display options.
+    """
 
     _DEPENDENCY_ID = "__SELECT_DATA_DEPENDENCY__"
 
     _WIDGET_API_TYPE = "select"
 
     _DEFAULT_HEIGHT = 0.5
     _FORCE_HEIGHT = True
@@ -40,15 +46,15 @@
         label_column: Optional[TemplatedStringItem] = None,
         widget_id: Optional[str] = None,
         label: TemplatedStringItem = "",
         label_outside: bool = True,
         group_column: Optional[TemplatedStringItem] = None,
         show_group_when_selected: bool = False,
     ):
-        """Construct spec for Select widget.
+        """Constructor for Select widget.
 
         Args:
             data: data to be used by widget. Accepts storages as well as raw data.
             widget_id: unique widget id in a dashboard.
             id_column: name of column in pandas dataframe(s) used for the id associated
                 with each entry.
             label_column: name of column in pandas dataframe(s) used for the value
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/__init__.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/category.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/category.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,19 @@
     CountryFlagStyling,
     DotStyling,
     FontStyling,
 ]
 
 
 class CategoryColumn(Column):
-    """Specifications for CategoryColumn class."""
+    """Define table widget column: Categorize data with source.
+
+    Define a column in the table widget that categorizes data, with
+    options for data source, label, formatting, styling, and alignment.
+    """
 
     _ITEM_ID_TYPE: str = "CATEGORY"
 
     @type_check
     def __init__(
         self,
         *,
@@ -50,15 +54,15 @@
         align: HorizontalAlignment = HorizontalAlignment.LEFT,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = False,
         optional: bool = False,
     ):
-        """Class CategoryColumn is used as categorization column for the Table Widget.
+        """Constructor for CategoryColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
             label: label to be displayed for this column.
             formatting: formatting spec.
             styling: styling spec for column. One of TableColumnStylingCell,
                 TableColumnStylingCountryFlag or TableColumnStylingDot.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 
 from ...styling.area import AreaChartStyling
 from .base import ChartColumn
 from .base import ReferenceLineType
 
 
 class AreaChartColumn(ChartColumn):
-    """Specifications for AreaChartColumn class."""
+    """Define table widget column area.
+
+    Define a column in the table widget that displays an area sparkline
+    chart, including options for data, formatting, styling, and more.
+    """
 
     _ITEM_ID_TYPE: str = "AREA_CHART"
 
     @type_check
     def __init__(
         self,
         *,
@@ -43,15 +47,15 @@
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = True,
         optional: bool = False,
         tooltip: Optional[ChartTooltip] = None,
     ):
-        """Class AreaChartColumn is used as area sparkline column for the Table Widget.
+        """Constructor for AreaChartColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
             data_key: key in object that contains the value for the line chart.
             label: label to be displayed for this column.
             formatting: formatting spec.
             styling: styling spec for area chart.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 
 from ...styling.column import ColumnChartStyling
 from .base import ChartColumn
 from .base import ReferenceLineType
 
 
 class ColumnChartColumn(ChartColumn):
-    """Specifications for ColumnChartColumn class."""
+    """Define table widget column: Column sparkline chart with data.
+
+    Define a column in the table widget that displays a column
+    sparkline chart, including options for data, formatting, styling,
+    and more.
+    """
 
     _ITEM_ID_TYPE: str = "COLUMN_CHART"
 
     @type_check
     def __init__(
         self,
         *,
@@ -43,15 +48,15 @@
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = True,
         optional: bool = False,
         tooltip: Optional[ChartTooltip] = None,
     ):
-        """Class ColumnChartColumn is used as column sparkline column for Table Widget.
+        """Constructor for ColumnChartColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
             data_key: key in object that contains the value for the line chart.
             label: label to be displayed for this column.
             formatting: formatting spec.
             styling: styling spec for column chart.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 
 from ...styling.line import LineChartStyling
 from .base import ChartColumn
 from .base import ReferenceLineType
 
 
 class LineChartColumn(ChartColumn):
-    """Specifications for LineChartColumn class."""
+    """Define table widget column: Line sparkline chart with data.
+
+    Define a column in the table widget that displays a line sparkline
+    chart, including options for data, formatting, styling, and more.
+    """
 
     _ITEM_ID_TYPE: str = "LINE_CHART"
 
     @type_check
     def __init__(
         self,
         *,
@@ -43,15 +47,15 @@
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = True,
         optional: bool = False,
         tooltip: Optional[ChartTooltip] = None,
     ):
-        """Class LineChartColumn is used as line sparkline column for the Table Widget.
+        """Constructor for LineChartColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
             data_key: key in object that contains the value for the line chart.
             label: label to be displayed for this column.
             formatting: formatting spec.
             styling: styling spec for line chart.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 from engineai.sdk.dashboard.utils import generate_input
 
 from ...styling.stacked_bar import StackedBarStyling
 from .base import ChartColumn
 
 
 class StackedBarColumn(ChartColumn):
-    """Specifications for StackedBarColumn class."""
+    """Define table widget column: Stacked bar chart with data.
+
+    Define a column in the table widget that displays a stacked bar chart,
+    including options for data, formatting, styling, and more.
+    """
 
     _ITEM_ID_TYPE: str = "STACKED_BAR"
 
     @type_check
     def __init__(
         self,
         *,
@@ -35,15 +39,15 @@
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = True,
         display_total_value: bool = True,
         optional: bool = False,
     ):
-        """Class StackedBarColumn is used as stack bar column for the Table Widget.
+        """Constructor for StackedBarColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
             data_key: key in object that contains the value for the stack bar chart.
             label_key: key in object that contains the label for the stack bar chart.
             label: label to be displayed for this column.
             formatting: formatting spec.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/country.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/country.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,19 @@
 
     LEFT: bool = True
     RIGHT: bool = False
     HIDDEN: None = None
 
 
 class CountryColumn(Column):
-    """Specifications for CountryColumn class."""
+    """Define table widget column: Country information with data source.
+
+    Define a column in the table widget that displays country information,
+    including options for data source, label, formatting, and alignment.
+    """
 
     _ITEM_ID_TYPE: str = "COUNTRY"
 
     @type_check
     def __init__(
         self,
         *,
@@ -50,15 +54,15 @@
         align: HorizontalAlignment = HorizontalAlignment.LEFT,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = False,
         optional: bool = False,
     ):
-        """Class CountryColumn is used as Country information column for Table Widget.
+        """Constructor for Country Column.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
                 Data in this column should be ISO 3166-1 alpha-2 country codes.
             label: label to be displayed for this column.
             flag_position: position of country flag.
             formatting: text formatting spec.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/text.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,94 +4,99 @@
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.formatting import DateTimeFormatting
-from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.formatting import TextFormatting
 from engineai.sdk.dashboard.links.typing import GenericLink
+from engineai.sdk.dashboard.links.widget_field import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
 
 from ..styling.cell import CellStyling
 from ..styling.country_flag import CountryFlagStyling
 from ..styling.dot import DotStyling
 from ..styling.font import FontStyling
+from ..styling.icon import IconStyling
 from ..styling.utils import build_styling_input
 from .base import Column
-from .exceptions import TableDatetimeColumnMappingError
 
-DatetimeColumnStyling = Union[
+TextColumnStyling = Union[
     CellStyling,
     CountryFlagStyling,
     DotStyling,
     FontStyling,
+    IconStyling,
 ]
 
 
-class DatetimeColumn(Column):
-    """Specifications for DatetimeColumn class."""
+class TextColumn(Column):
+    """Define table widget column: Text data with data source.
 
-    _ITEM_ID_TYPE: str = "DATETIME"
+    Define a column in the table widget that displays text data,
+    including options for data source, label, formatting, styling,
+    and alignment.
+    """
+
+    _ITEM_ID_TYPE: str = "TEXT"
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
-        formatting: Optional[DateTimeFormatting] = None,
-        styling: Optional[Union[Palette, DatetimeColumnStyling]] = None,
-        align: HorizontalAlignment = HorizontalAlignment.CENTER,
+        formatting: Optional[TextFormatting] = None,
+        styling: Optional[Union[Palette, TextColumnStyling]] = None,
+        align: HorizontalAlignment = HorizontalAlignment.LEFT,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = True,
         optional: bool = False,
     ):
-        """Class DatetimeColumn is used as datetime column for the Table Widget.
+        """Constructor for TextColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
             label: label to be displayed for this column.
             formatting: formatting spec.
-            styling: styling spec for column. One of TableColumnStylingCell,
-                TableColumnStylingCountryFlag or TableColumnStylingDot.
-            align: horizontal alignment of the column.
+            styling: styling spec for column. One of CellStyling, CountryFlagStyling
+                DotStyling, FontStyling or IconStyling.
+            align: align text.
             hiding_priority: columns with lower hiding_priority are hidden first
                 if not all data can be shown.
-            tooltip_text: info text to explain column. Each element of list is
-                displayed as a separate paragraph.
+            tooltip_text: info text to explain column.
+                Each element of list is displayed as a separate paragraph.
             min_width: min width of the column in pixels.
             sortable: determines if column can be sorted.
             optional: flag to make the column optional if there is no Data for that
                 columns.
 
         Examples:
-            ??? example "Create a Table widget with DatetimeColumn"
+            ??? example "Create a Table widget with TextColumn"
                 ```py linenums="1"
                 import pandas as pd
-                import datetime
                 from engineai.sdk.dashboard.dashboard import Dashboard
                 from engineai.sdk.dashboard.widgets import table
                 data = pd.DataFrame(
                     {
-                        "datetime": datetime.datetime.now().timestamp(),
-                    },
+                        "text": "Apple has ticker=AAPL",
+                    }
                 )
                 Dashboard(
                     content=table.Table(
                         data=data,
                         columns=[
-                            table.DatetimeColumn(
-                                data_column="datetime",
+                            table.TextColumn(
+                                data_column="text",
                                 ),
                             ),
                         ],
                     )
                 )
                 ```
         """
@@ -104,55 +109,46 @@
             optional=optional,
         )
         self.__align = align
         self.__styling = (
             CellStyling(color_spec=styling) if isinstance(styling, Palette) else styling
         )
         self.__sortable = sortable
-        self.__formatting = formatting if formatting else DateTimeFormatting()
+        self.__formatting = formatting if formatting else TextFormatting()
 
     def prepare(self) -> None:
         """Prepare data column."""
         if self.__styling is not None:
             self.__styling.prepare(self._data_column)
 
     def _custom_validation(self, *, data: pd.DataFrame) -> None:
         """Custom validation for each columns to implement.
 
         Args:
             data: pandas dataframe which will be used for table.
-
-        Raises:
-            TableDatetimeColumnMappingError: if data contains data_column which are
-                not epoch time
         """
-        try:
-            pd.to_datetime(data[self.data_column], unit="ms")
-        except ValueError as e:
-            raise TableDatetimeColumnMappingError(data_column=self.data_column) from e
-
-        if self.__styling:
+        if self.__styling is not None:
             self.__styling.validate(data=data)
 
     def _build_styling(self) -> Any:
         column_styling = None
         if self.__styling:
             column_styling = generate_input(
-                "TableDateTimeColumnStylingInput",
+                "TableTextColumnStylingInput",
                 **build_styling_input(
                     data_column=self.data_column, styling=self.__styling
                 ),
             )
         return column_styling
 
     def _build_column(self) -> Any:
         return generate_input(
             "TableColumnTypeInput",
-            dateTimeColumn=generate_input(
-                "TableDateTimeColumnInput",
+            textColumn=generate_input(
+                "TableTextColumnInput",
                 sortable=self.__sortable,
                 formatting=self.__formatting.build(),
                 align=self.__align.value,
                 styling=self._build_styling(),
                 optional=self._optional,
             ),
         )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/number.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/number.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,19 @@
     DotStyling,
     FontStyling,
     SplitBarStyling,
 ]
 
 
 class NumberColumn(Column):
-    """Specifications for NumberColumn class."""
+    """Define table widget column: Numerical data with data source.
+
+    Define a column in the table widget that displays numerical data, including
+    options for data source, label, formatting, and alignment.
+    """
 
     _ITEM_ID_TYPE: str = "NUMBER"
 
     @type_check
     def __init__(
         self,
         *,
@@ -53,15 +57,15 @@
         align: Optional[HorizontalAlignment] = None,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = True,
         optional: bool = False,
     ):
-        """Class NumberColumn is used as number column for the Table Widget.
+        """Constructor for NumberColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
             label: label to be displayed for this column.
             formatting: formatting spec.
             styling: styling spec for column. One of TableColumnStylingCell,
                 TableColumnStylingCountryFlag or TableColumnStylingDot.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/range.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/range.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 from ..styling.range import RangeStyling
 from .base import Column
 from .exceptions import TableColumnDataTypeError
 from .exceptions import TableRangeColumnValueError
 
 
 class RangeColumn(Column):
-    """Specifications for RangeColumn class."""
+    """Define table widget column: Range values with data source.
+
+    Define a column in the table widget that represents a range of values,
+    including options for data source, label, formatting, and styling.
+    """
 
     _ITEM_ID_TYPE: str = "RANGE"
 
     @type_check
     def __init__(
         self,
         *,
@@ -37,15 +41,15 @@
         styling: Optional[Union[Palette, RangeStyling]] = None,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = True,
         optional: bool = False,
     ):
-        """Class RangeColumn is used as range representation column for Table Widget.
+        """Constructor for RangeColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
             label: label to be displayed for this column.
             formatting: formatting spec.
             styling: styling spec for range.
             hiding_priority: columns with lower hiding_priority are hidden first
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/text.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,94 +4,98 @@
 from typing import List
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.formatting import TextFormatting
+from engineai.sdk.dashboard.formatting import DateTimeFormatting
+from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.links.typing import GenericLink
-from engineai.sdk.dashboard.links.widget_field import WidgetField
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 from engineai.sdk.dashboard.utils import generate_input
 from engineai.sdk.dashboard.widgets.table.enums import HorizontalAlignment
 
 from ..styling.cell import CellStyling
 from ..styling.country_flag import CountryFlagStyling
 from ..styling.dot import DotStyling
 from ..styling.font import FontStyling
-from ..styling.icon import IconStyling
 from ..styling.utils import build_styling_input
 from .base import Column
+from .exceptions import TableDatetimeColumnMappingError
 
-TextColumnStyling = Union[
+DatetimeColumnStyling = Union[
     CellStyling,
     CountryFlagStyling,
     DotStyling,
     FontStyling,
-    IconStyling,
 ]
 
 
-class TextColumn(Column):
-    """Specifications for TextColumn class."""
+class DatetimeColumn(Column):
+    """Define table widget column: Datetime information with data source.
 
-    _ITEM_ID_TYPE: str = "TEXT"
+    Define a column in the table widget that displays datetime information,
+    including options for data source, label, formatting, and alignment.
+    """
+
+    _ITEM_ID_TYPE: str = "DATETIME"
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         label: Optional[Union[str, GenericLink]] = None,
-        formatting: Optional[TextFormatting] = None,
-        styling: Optional[Union[Palette, TextColumnStyling]] = None,
-        align: HorizontalAlignment = HorizontalAlignment.LEFT,
+        formatting: Optional[DateTimeFormatting] = None,
+        styling: Optional[Union[Palette, DatetimeColumnStyling]] = None,
+        align: HorizontalAlignment = HorizontalAlignment.CENTER,
         hiding_priority: int = 0,
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
         min_width: Optional[int] = None,
         sortable: bool = True,
         optional: bool = False,
     ):
-        """Class TextColumn is used as text column for the Table Widget.
+        """Constructor for DatetimeColumn.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for this widget.
             label: label to be displayed for this column.
             formatting: formatting spec.
-            styling: styling spec for column. One of CellStyling, CountryFlagStyling
-                DotStyling, FontStyling or IconStyling.
-            align: align text.
+            styling: styling spec for column. One of TableColumnStylingCell,
+                TableColumnStylingCountryFlag or TableColumnStylingDot.
+            align: horizontal alignment of the column.
             hiding_priority: columns with lower hiding_priority are hidden first
                 if not all data can be shown.
-            tooltip_text: info text to explain column.
-                Each element of list is displayed as a separate paragraph.
+            tooltip_text: info text to explain column. Each element of list is
+                displayed as a separate paragraph.
             min_width: min width of the column in pixels.
             sortable: determines if column can be sorted.
             optional: flag to make the column optional if there is no Data for that
                 columns.
 
         Examples:
-            ??? example "Create a Table widget with TextColumn"
+            ??? example "Create a Table widget with DatetimeColumn"
                 ```py linenums="1"
                 import pandas as pd
+                import datetime
                 from engineai.sdk.dashboard.dashboard import Dashboard
                 from engineai.sdk.dashboard.widgets import table
                 data = pd.DataFrame(
                     {
-                        "text": "Apple has ticker=AAPL",
-                    }
+                        "datetime": datetime.datetime.now().timestamp(),
+                    },
                 )
                 Dashboard(
                     content=table.Table(
                         data=data,
                         columns=[
-                            table.TextColumn(
-                                data_column="text",
+                            table.DatetimeColumn(
+                                data_column="datetime",
                                 ),
                             ),
                         ],
                     )
                 )
                 ```
         """
@@ -104,46 +108,55 @@
             optional=optional,
         )
         self.__align = align
         self.__styling = (
             CellStyling(color_spec=styling) if isinstance(styling, Palette) else styling
         )
         self.__sortable = sortable
-        self.__formatting = formatting if formatting else TextFormatting()
+        self.__formatting = formatting if formatting else DateTimeFormatting()
 
     def prepare(self) -> None:
         """Prepare data column."""
         if self.__styling is not None:
             self.__styling.prepare(self._data_column)
 
     def _custom_validation(self, *, data: pd.DataFrame) -> None:
         """Custom validation for each columns to implement.
 
         Args:
             data: pandas dataframe which will be used for table.
+
+        Raises:
+            TableDatetimeColumnMappingError: if data contains data_column which are
+                not epoch time
         """
-        if self.__styling is not None:
+        try:
+            pd.to_datetime(data[self.data_column], unit="ms")
+        except ValueError as e:
+            raise TableDatetimeColumnMappingError(data_column=self.data_column) from e
+
+        if self.__styling:
             self.__styling.validate(data=data)
 
     def _build_styling(self) -> Any:
         column_styling = None
         if self.__styling:
             column_styling = generate_input(
-                "TableTextColumnStylingInput",
+                "TableDateTimeColumnStylingInput",
                 **build_styling_input(
                     data_column=self.data_column, styling=self.__styling
                 ),
             )
         return column_styling
 
     def _build_column(self) -> Any:
         return generate_input(
             "TableColumnTypeInput",
-            textColumn=generate_input(
-                "TableTextColumnInput",
+            dateTimeColumn=generate_input(
+                "TableDateTimeColumnInput",
                 sortable=self.__sortable,
                 formatting=self.__formatting.build(),
                 align=self.__align.value,
                 styling=self._build_styling(),
                 optional=self._optional,
             ),
         )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/area.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/area.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableSparklineColumnStylingBase
 
 
 class AreaChartStyling(TableSparklineColumnStylingBase):
-    """Specifications for AreaChartStyling."""
+    """Styling options for area chart column.
+
+    Specify the styling options for an area chart column in
+    the table widget, including color and data key.
+    """
 
     _API_TYPE = "SparkChartAreaStylingInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_key: Optional[Union[str, WidgetField]] = None,
     ):
-        """Construct for AreaChartStyling class.
+        """Constructor for AreaChartStyling.
 
         Args:
             data_key: Dictionary key, stored in data, that is used for chart.
                 By default, will use values of column to which styling is applied.
             color_spec: spec for color of area chart.
         """
         super().__init__(
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
 class ArrowStyling(TableColumnStylingBase):
-    """Specification for styling a column with an arrow next to value."""
+    """Styling options for arrow column.
+
+    Specify the styling options for an arrow column in the
+    table widget, including data column, mid value, and color.
+    """
 
     _API_TYPE = "TableColumnStylingArrowInput"
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Optional[Union[str, WidgetField]] = None,
         mid: Union[float, int] = 0,
         color_spec: Optional[ColorSpec] = None,
     ):
-        """Construct for ArrowStyling class.
+        """Constructor for ArrowStyling.
 
         Args:
             data_column: id of column which values are used to determine behavior of
                 arrow. By default, will use values of column to which styling is
                 applied.
             mid: value that determines when arrow flips up/down.
             color_spec: spec for color of arrows. By default, used the
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
 class CellStyling(TableColumnStylingBase):
-    """Specification for styling a column with an arrow next to value."""
+    """Styling options for table widget cell.
+
+    Specify the styling options for a cell in the table widget,
+    including color, data column, and percentage fill.
+    """
 
     _API_TYPE = "TableColumnStylingCellInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
         percentage_fill: Optional[Union[float, int]] = 1,
     ):
-        """Construct for CellStyling class.
+        """Constructor for CellStyling.
 
         Args:
             data_column: id of column which values are used to determine behavior of
                 arrow. By default, will use values of column to which styling is
                 applied.
             percentage_fill: how much of the cell should the color
                 fill. Default to 1, meaning the whole cell
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,35 @@
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 from .exceptions import TableColumnStylingMinMaxValueError
 
 
 class ColorBarStyling(TableColumnStylingBase):
-    """Specification for styling a column with a color bar."""
+    """Styling options for split color bar column.
+
+    Specify the styling options for a color bar column in the
+    table widget, including color, data column, direction,
+    min/max values, and percentage fill.
+    """
 
     _API_TYPE = "TableColumnStylingColorBarInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
         left_to_right: bool = True,
         min_value: Optional[Union[float, int]] = None,
         max_value: Optional[Union[float, int]] = None,
         percentage_fill: float = 0.9,
     ):
-        """Construct for ColorBarStyling class.
+        """Constructor for ColorBarStyling.
 
         Args:
             color_spec: spec for bar color.
             data_column: id of column which values are used to determine behavior of
                 arrow. By default, will use values of column to which styling is
                 applied.
             left_to_right: determines the direction of color bar.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/column.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/column.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableSparklineColumnStylingBase
 
 
 class ColumnChartStyling(TableSparklineColumnStylingBase):
-    """Specification for styling a column chart."""
+    """Styling options for column chart column.
+
+    Specify the styling options for a column chart column in
+    the table widget, including color and data key.
+    """
 
     _API_TYPE = "SparkChartColumnStylingInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_key: Optional[Union[str, WidgetField]] = None,
     ):
-        """Construct for ColumnChartStyling class.
+        """Constructor for ColumnChartStyling.
 
         Args:
             data_key: Dictionary key, stored in data, that is used for chart.
                 By default, will use values of column to which styling is applied.
             color_spec: spec for color of column chart.
         """
         super().__init__(
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-"""Specification for styling a column with a country flag to a value."""
+"""Specification for styling a column with an icon to a value."""
 from typing import Any
 from typing import Dict
-from typing import Optional
 from typing import Union
 
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.links import WidgetField
 
 from .base import TableColumnStylingBase
 
 
-class CountryFlagStyling(TableColumnStylingBase):
-    """Specification for styling a column with a country flag to a value."""
+class IconStyling(TableColumnStylingBase):
+    """Styling options for icon column.
 
-    _API_TYPE = "TableColumnStylingCountryFlagInput"
+    Specify the styling options for an icon column in the
+    table widget, including data column and position.
+    """
+
+    _API_TYPE = "TableColumnStylingIconInput"
 
     @type_check
     def __init__(
         self,
         *,
+        data_column: Union[str, WidgetField],
         left: bool = True,
-        data_column: Optional[Union[str, WidgetField]] = None,
     ):
-        """Construct for CountryFlagStyling class.
+        """Constructor for IconStyling.
 
         Args:
             data_column: id of column which values are used to determine behavior of
                 arrow.
                 By default, will use values of column to which styling is applied.
-            left: whether to put flag to the left (True) or right (False) of column
+            left: whether to put icon to the left (True) or right (False) of column
                 value.
         """
         super().__init__(data_column=data_column, color_spec=None)
         self.__left = left
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
         return {"left": self.__left}
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,26 +7,30 @@
 from engineai.sdk.dashboard.styling import color
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
 class DotStyling(TableColumnStylingBase):
-    """Specification for styling a column with a colored dot left to the value."""
+    """Styling options for dot column.
+
+    Specify the styling options for a dot column in the table
+    widget, including color and data column.
+    """
 
     _API_TYPE = "TableColumnStylingDotInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: Optional[ColorSpec] = None,
         data_column: Optional[Union[str, WidgetField]] = None,
     ):
-        """Construct for DotStyling class.
+        """Constructor for DotStyling.
 
         Args:
             data_column: id of column which values are used to determine behavior of
                 color of dot. Optional if color_spec is a single color.
             color_spec: spec for color of dot.
         """
         super().__init__(
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/font.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/font.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 
 
 class FontStyling(TableColumnStylingBase):
-    """Specification for column font styling."""
+    """Font styling options.
+
+    Specify the font styling options for a column in the table widget,
+    including color, data column, and background highlighting.
+    """
 
     _API_TYPE = "TableColumnStylingFontInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
         highlight_background: bool = False
     ):
-        """Construct for FontStyling class.
+        """Constructor for FontStyling.
 
         Args:
             data_column: id of column which values are used to determine behavior of
                 color of dot. Optional if color_spec is a single color.
             color_spec: spec for color of dot.
             highlight_background: Highlight value background.
         """
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/column.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-"""Specification for styling a column with an icon to a value."""
-from typing import Any
-from typing import Dict
-from typing import Union
+"""Spec to style a column series."""
+from typing import Optional
 
 from engineai.sdk.dashboard.decorator import type_check
-from engineai.sdk.dashboard.links import WidgetField
+from engineai.sdk.dashboard.styling.color.typing import ColorSpec
+from engineai.sdk.dashboard.templated_string import TemplatedStringItem
 
-from .base import TableColumnStylingBase
+from .base import BaseChartSeriesStyling
+from .enums import MarkerSymbol
 
 
-class IconStyling(TableColumnStylingBase):
-    """Specification for styling a column with an icon to a value."""
+class ColumnSeriesStyling(BaseChartSeriesStyling):
+    """Customize appearance of vertical columns.
 
-    _API_TYPE = "TableColumnStylingIconInput"
+    Specify styling options for a column series within a
+    Chart widget to customize the appearance of vertical columns on the chart.
+    """
+
+    _API_TYPE = "ChartColumnSeriesStylingInput"
 
     @type_check
     def __init__(
         self,
         *,
-        data_column: Union[str, WidgetField],
-        left: bool = True,
+        color_spec: ColorSpec,
+        data_column: Optional[TemplatedStringItem] = None,
+        marker_symbol: MarkerSymbol = MarkerSymbol.SQUARE,
     ):
-        """Construct for IconStyling class.
+        """Constructor for ColumnSeriesStyling.
 
         Args:
-            data_column: id of column which values are used to determine behavior of
-                arrow.
-                By default, will use values of column to which styling is applied.
-            left: whether to put icon to the left (True) or right (False) of column
-                value.
+            color_spec: spec for coloring columns.
+            data_column: name of column in pandas dataframe(s) used for color spec if
+                a gradient is used. Optional for single colors.
+            marker_symbol: symbol for marker in tooltips and legends.
+
+        Raises:
+            ChartStylingMissingDataColumnError: if a data_column is not defined when
+                color_spec is a ColorDiscreteMap or ColorGradient
         """
-        super().__init__(data_column=data_column, color_spec=None)
-        self.__left = left
-
-    def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {"left": self.__left}
+        super().__init__(
+            color_spec=color_spec, data_column=data_column, marker_symbol=marker_symbol
+        )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/line.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/line.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 from engineai.sdk.dashboard.links import WidgetField
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableSparklineColumnStylingBase
 
 
 class LineChartStyling(TableSparklineColumnStylingBase):
-    """Specification for styling a line chart."""
+    """Styling options for line chart column.
+
+    Specify the styling options for a line chart column in
+    the table widget, including color and data key.
+    """
 
     _API_TYPE = "SparkChartLineStylingInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_key: Optional[Union[str, WidgetField]] = None,
     ):
-        """Construct for LineChartStyling class.
+        """Constructor for LineChartStyling.
 
         Args:
             data_key: Dictionary key, stored in data, that is used for chart.
                 By default, will use values of column to which styling is applied.
             color_spec: spec for color of line chart.
         """
         super().__init__(
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/range.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/range.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,27 +16,31 @@
     """Range shape options."""
 
     CIRCLE = "CIRCLE"
     RECTANGLE = "RECTANGLE"
 
 
 class RangeStyling(TableColumnStylingBase):
-    """Specification for styling a column with a range next to value."""
+    """Styling options for range column.
+
+    Specify the styling options for a range column in the
+    table widget, including color, data column, and shape.
+    """
 
     _API_TYPE = "TableColumnStylingRangeInput"
 
     @type_check
     def __init__(
         self,
         *,
         color_spec: ColorSpec,
         data_column: Optional[Union[str, WidgetField]] = None,
         shape: RangeShape = RangeShape.CIRCLE,
     ):
-        """Construct for RangeStyling class.
+        """Constructor for RangeStyling.
 
         Args:
             data_column: id of column which values are used to determine behavior of
                 arrow.
             color_spec: spec for color of range value.
             shape: shape of range indicator.
         """
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,32 +12,34 @@
 from engineai.sdk.dashboard.styling.color.typing import ColorSpec
 
 from .base import TableColumnStylingBase
 from .exceptions import TableColumnStylingMinMaxValueError
 
 
 class SplitBarStyling(TableColumnStylingBase):
-    """Specification for styling a column with a split color bar.
+    """Styling options for split color bar column.
 
-    Use for positive and negative values.
+    Specify the styling options for a split color bar column in the
+    table widget, including color, data column, min/max values,
+    and percentage fill.
     """
 
     _API_TYPE = "TableColumnStylingSplitBarInput"
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Optional[Union[str, WidgetField]] = None,
         color_spec: Optional[ColorSpec] = None,
         min_value: Optional[Union[float, int]] = None,
         max_value: Optional[Union[float, int]] = None,
         percentage_fill: float = 0.9,
     ):
-        """Construct for StackedBarStyling class.
+        """Constructor for SplitBarStyling.
 
         Args:
             data_column: id of column which values are used to determine behavior of
                 arrow.
                 By default, will use values of column to which styling is applied.
             color_spec: spec for color class.
             min_value: value that determines a 0% bar. By default, takes the minimum
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/group.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 from engineai.sdk.dashboard.templated_string import build_templated_strings
 from engineai.sdk.dashboard.utils import generate_input
 
 from .exceptions import TableGroupColumnKeyNotFoundError
 
 
 class Group(AbstractFactoryLinkItemsHandler):
-    """Spec for Table group column."""
+    """Define group column for table widget.
+
+    Define a group column for the table widget,
+    which allows grouping rows based on specified columns.
+    """
 
     @type_check
     def __init__(
         self,
         data_column: Union[str, WidgetField],
         label: Union[str, WidgetField],
     ):
-        """Construct Table group column.
+        """Constructor for Group.
 
         Args:
             data_column: column that will be used to group the table rows.
             label: table group label.
         """
         super().__init__()
         self.__data_column = data_column
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/header.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/header.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,24 +22,28 @@
 from .exceptions import TableHeaderChildTypeError
 from .exceptions import TableHeaderLevelsError
 
 TableColumns = Union[str, Column, "Header", List[Union[str, Column, "Header"]]]
 
 
 class Header(AbstractFactoryLinkItemsHandler):
-    """Spec for table header columns (i.e. above normal columns)."""
+    """Specify header columns with optional tooltips for table widget.
+
+    Specify the columns to be displayed as headers above the normal
+    columns in the table widget, along with optional tooltip text.
+    """
 
     @type_check
     def __init__(
         self,
         columns: TableColumns,
         label: Union[str, GenericLink],
         tooltip_text: Optional[List[TemplatedStringItem]] = None,
     ):
-        """Construct Table header columns.
+        """Constructor for Header.
 
         Args:
             columns: header(s)/column(s) into the Table Widget. When this is of type
                 string, it is assumed to be a text column.
             label: label to be displayed for this column.
             tooltip_text: info text to explain column. Each element of list is
                 displayed as a separate paragraph.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/initial_state.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/initial_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,29 @@
 from engineai.sdk.dashboard.utils import generate_input
 
 from .exceptions import TableInitialStateIncompatiblePreSelectedIndexError
 from .exceptions import TableInitialStateIncompatiblePreSelectedRowsError
 
 
 class InitialState(AbstractFactory):
-    """Spec for Table widget state."""
+    """Define initial state for table widget.
+
+    Define the initial state for the table widget,
+    including the default page, search text, and pre-selected rows.
+    """
 
     @type_check
     def __init__(
         self,
         *,
         page: int = 0,
         search_text: str = "",
         selected: Optional[List[str]] = None,
     ):
-        """Construct state spec for table widget.
+        """Constructor for InitialState.
 
         Args:
             page: the default initial page.
             search_text: Initial string in the search box.
             selected: List of rows pre-selected by default.
         """
         super().__init__()
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/styling.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/styling.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 
 from engineai.sdk.dashboard.base import AbstractFactory
 from engineai.sdk.dashboard.decorator import type_check
 from engineai.sdk.dashboard.utils import generate_input
 
 
 class TableStyling(AbstractFactory):
-    """Spec for Table widget styling."""
+    """Visual styling options for table widget.
+
+    Specify the visual styling options for the table widget,
+    including borders, column lines, row lines, and row height.
+    """
 
     @type_check
     def __init__(
         self,
         *,
         has_borders: bool = True,
         has_column_lines: bool = True,
         has_body_column_lines: bool = True,
         has_row_lines: bool = True,
         single_height_row: bool = True
     ):
-        """Construct styling spec for table widget.
+        """Constructor for TableStyling.
 
         Args:
             has_borders: whether the outer border of the table are shown.
             has_column_lines: whether vertical lines that separate columns are visible.
             has_body_column_lines: whether vertical lines that separate body columns
                 are visible.
             has_row_lines: whether horizontal lines that separate rows are
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/table/table.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,19 @@
 from .header import Header
 from .header import TableColumns
 from .initial_state import InitialState
 from .styling import TableStyling
 
 
 class Table(SelectableWidget):
-    """Spec for Table widget."""
+    """Construct table widget.
+
+    Construct a table widget with customizable parameters such as data source,
+    columns, title, styling, row selection, pagination, search box, and more.
+    """
 
     _DEPENDENCY_ID = "__TABLE_DATA_DEPENDENCY__"
     _WIDGET_API_TYPE = "tableGrid"
 
     _HEIGHT_TABLE_BODY_BORDER = 0.01
     _HEIGHT_TABLE_ROW = 0.30
     _HEIGHT_TABLE_HEADER_ROW = 0.31
@@ -103,15 +107,15 @@
         rows_per_page: int = 10,
         initial_state: Optional[InitialState] = None,
         has_search_box: bool = False,
         has_filter_row: bool = False,
         has_header_filter: bool = False,
         group_columns: Optional[List[Group]] = None,
     ):
-        """Construct a table widget.
+        """Constructor for Table widget.
 
         Args:
             data: data to be used by widget. Accepts DataSource as well as raw data.
             columns: header(s)/column(s) into the Table Widget. When this is of type
                 string, it is assumed to be a text column.
             widget_id: unique widget id in a dashboard.
             title: title of widget can be either a string (fixed value) or determined
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/__init__.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,28 +16,32 @@
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
 
 from ...series.typing import TimeseriesSeries
 from .base import BaseTimeseriesYAxis
 
 
 class YAxis(BaseTimeseriesYAxis):
-    """Specs for y axis of a Timeseries chart."""
+    """Specify y-axis appearance & behavior in Timeseries chart.
+
+    Construct specifications for the y-axis of a Timeseries chart with
+    a range of options to customize its appearance and behavior.
+    """
 
     _API_TYPE = "TimeseriesWidgetChartStandardYAxisInput"
 
     @type_check
     def __init__(
         self,
         *,
         formatting: Optional[AxisNumberFormatting] = None,
         title: Union[str, WidgetField] = "",
         enable_crosshair: bool = False,
         scale: Optional[AxisScale] = None,
     ):
-        """Construct y axis for a Timeseries chart.
+        """Constructor for YAxis.
 
         Args:
             formatting (Optional[AxisNumberFormatting]): formatting spec for axis
                 labels.
                 Defaults to None (Base AxisFormatting).
             title (Union[str, WidgetField]): axis title.
                 Defaults to empty string.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,28 +16,32 @@
 from engineai.sdk.dashboard.widgets.components.charts.axis.scale import AxisScale
 
 from ...series.typing import TimeseriesSeries
 from .base import BaseTimeseriesYAxis
 
 
 class MirrorYAxis(BaseTimeseriesYAxis):
-    """Specs for mirror y axis of a Timeseries chart."""
+    """Customize appearance & behavior of mirror y-axis in Timeseries chart.
+
+    Construct specifications for the mirror y-axis of a Timeseries
+    chart with a range of options to customize its appearance and behavior.
+    """
 
     _API_TYPE = "TimeseriesWidgetChartMirrorYAxisInput"
 
     @type_check
     def __init__(
         self,
         *,
         formatting: Optional[AxisNumberFormatting] = None,
         title: Union[str, WidgetField] = "",
         enable_crosshair: bool = False,
         scale: Optional[AxisScale] = None,
     ):
-        """Construct y axis for a Timeseries chart.
+        """Constructor for MirrorYAxis.
 
         Args:
             formatting (Optional[AxisNumberFormatting]): formatting spec for axis
                 labels.
                 Defaults to None (Base AxisFormatting).
             title (Union[str, WidgetField]): axis title.
                 Defaults to empty string.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/chart.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,21 @@
 from .exceptions import TimeseriesHeightWrongDefinitionError
 from .exceptions import TimeseriesWrongSeriesAxisError
 from .series.base import TimeseriesBaseSeries
 from .series.typing import TimeseriesSeries
 
 
 class Chart(AbstractFactoryLinkItemsHandler):
-    """Spec for charts in a Timeseries widget."""
+    """Customize charts in Timeseries widget.
+
+    Construct charts within a timeseries widget, offering a variety of
+    customizable options for effective data visualization. Specify parameters
+    such as the x-axis specification, left and right y-axis configurations, chart
+    title, height, area series stacking, and tooltips.
+    """
 
     _HEIGHT_TIMESERIES_CHART_TITLE = 0.19
     __height: float  # Added here to use property logic for all entries
 
     @type_check
     def __init__(
         self,
@@ -47,15 +53,15 @@
         height: Union[float, int] = 3,
         x_axis: Optional[XAxis] = None,
         right_y_axis: Optional[Union[YAxisSpec, TimeseriesSeries]] = None,
         title: Optional[Union[str, WidgetField]] = None,
         area_series_stacked: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct a chart for a timeseries widget.
+        """Constructor for Chart.
 
         Args:
             x_axis: spec for x axis or the specific date column that must be used for
                 the x axis.
             left_y_axis: spec for left y axis. If `TimeseriesSeries` added directly,
                 a `YAxis` will be used as the default axis spec.
             right_y_axis: spec for right y axis (optional). If `TimeseriesSeries`
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/consts.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/consts.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/enums.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Enums for timeseries widget."""
 import enum
 
 
 class TransformChoices(enum.Enum):
-    """Options for transforms of timeseries legend.
+    """Options for transforming data within Timeseries legend.
+
+    Below are the various options for transformations of timeseries
+    data within a Timeseries widget's legend.
 
     Attributes:
         CUMSUM: Transform series to the cumulative sum of its values.
         CUMPROD: Transform series to the cumulative product of its values.
         CUMRETURNPROD: Similar to CUMPROD but fixes the initial value as 0. Example
             used is to represent Return on Investment.
         CUMRETURNSUM: Similar to CUMSUM but fixes the initial value as 0. Example
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/legend.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/legend.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/navigator.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/navigator.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,27 @@
 from engineai.sdk.dashboard.widgets.base import WidgetTitleType
 
 from .exceptions import TimeseriesNavigatorEmptyDefinitionError
 from .series.typing import TimeseriesSeries
 
 
 class Navigator(AbstractFactoryLinkItemsHandler):
-    """Spec for navigator of a timeseries widget."""
+    """Navigation of Timeseries data.
+
+    Construct a navigator for a timeseries widget for efficient
+    navigation and exploration of time-series data. Specify one or
+    more series to be included in the navigator for easy visualization
+    of trends and patterns across different metrics.
+    """
 
     @type_check
     def __init__(
         self, *series: TimeseriesSeries, title: Optional[WidgetTitleType] = None
     ) -> None:
-        """Construct a navigator for a timeseries widget.
+        """Constructor for Navigator.
 
         Args:
             title: title to be added to navigator
             series: series to be added to navigator
 
         Examples:
             ??? examples "Create a minimal timeseries widget with a navigator"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 from engineai.sdk.dashboard.links.abstract import AbstractFactoryLinkItemsHandler
 from engineai.sdk.dashboard.utils import generate_input
 
 from ..exceptions import TimeseriesPeriodSelectorDatesDefinitionError
 
 
 class CustomPeriod(AbstractFactoryLinkItemsHandler):
-    """Spec for a custom period for a period selector."""
+    """Define custom time intervals for period selector in Timeseries.
+
+    Construct specifications for a custom period for a period selector
+    component to define time intervals.
+    """
 
     @type_check
     def __init__(
         self,
         *,
         label: Optional[str] = None,
         start_date: Union[str, datetime],
         end_date: Union[str, datetime]
     ):
-        """Constructs a custom period.
+        """Constructor for CustomPeriod.
 
         Args:
             label: label to show in period selector.
             start_date: start date of custom period in a format supported by
                 pandas.to_datetime.
             end_date: end date of custom period in a format supported by
                 pandas.to_datetime.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,28 @@
 from .custom_period import CustomPeriod
 from .period import PeriodType
 from .period import build_timeseries_period
 from .standard import Period
 
 
 class PeriodSelector(AbstractFactory):
-    """Spec for period selector of a timeseries widget."""
+    """Select predefined periods for Timeseries visualization.
+
+    Construct specifications for a period selector component of a
+    timeseries widget, select predefined periods for data visualization.
+    """
 
     @type_check
     def __init__(
         self,
         *periods: PeriodType,
         default_selection: Optional[int] = None,
         visible: bool = True,
     ) -> None:
-        """Construct period selector.
+        """Constructor for PeriodSelector.
 
         Args:
             periods: specs for periods added into timeseries widget
                 period selector component.
             default_selection: choose which period selector to be the default.
             visible: flag that makes the period selector visible.
                 If False, all periods added and default selection will be ignored.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Spec for a standard period for a period selector."""
 import enum
 
 
 class Period(enum.Enum):
-    """Standard periods for period selector.
+    """Standard time intervals for period selector in Timeseries.
 
-    Each period is defined as a lookback relative to the last date of the chart.
+    Defines standard periods for a period selector component to choose
+    predefined time intervals for data visualization. Each period
+    represents a lookback relative to the last date of the chart.
 
     Attributes:
         D1: 1 day.
         W1: 1 week.
         W2: 2 weeks.
         M1: 1 month.
         M3: 3 months.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/area.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/point.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Spec for a area series of a Timeseries widget."""
+"""Spec for a point series of a Timeseries widget."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
@@ -13,47 +13,53 @@
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
-from engineai.sdk.dashboard.widgets.components.charts.styling import AreaSeriesStyling
+from engineai.sdk.dashboard.widgets.components.charts.styling import PointSeriesStyling
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
-class AreaSeries(TimeseriesBaseSeries):
-    """Spec for a area series of a Timeseries widget."""
+class PointSeries(TimeseriesBaseSeries):
+    """Visualize individual data points in Timeseries.
 
-    _API_TYPE = "TimeseriesWidgetAreaSeriesInput"
-    _INPUT_KEY = "area"
-    _styling_class = AreaSeriesStyling
+    Construct specifications for a point series within a Timeseries widget,
+    enabling users to visualize individual data points on the chart as
+    distinct markers. Each marker represents a specific data value,
+    providing a clear and concise depiction of the data distribution over time.
+    """
+
+    _API_TYPE = "TimeseriesWidgetPointSeriesInput"
+    _INPUT_KEY = "point"
+    _styling_class = PointSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
-        styling: Optional[Union[Palette, AreaSeriesStyling]] = None,
+        styling: Optional[Union[Palette, PointSeriesStyling]] = None,
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct area series.
+        """Constructor for PointSeries.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for the values of
                 this series.
-            name: series name shown in legend and tooltip.
+            name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
             entity: entity spec.
             show_in_legend: whether to show series in legend or not.
             required: Flag to make the Series mandatory. If required == True and no
                 Data the widget will show an error. If required==False and no Data,
                 the widget hides the Series.
@@ -63,15 +69,15 @@
         """
         super().__init__(
             name=name,
             data_column=data_column,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=AreaSeriesStyling(color_spec=styling)
+            styling=PointSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
 
@@ -83,10 +89,8 @@
         """
         super().validate(data=data)
 
         if self._entity is not None and isinstance(self._entity, CountryEntity):
             self._entity.validate_country_code()
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {
-            "transforms": [transform.build() for transform in self._transforms],
-        }
+        return {"transforms": [transform.build() for transform in self._transforms]}
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Spec for a area range series of a Timeseries widget."""
+"""Spec for error bar series of a Timeseries widget."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
@@ -15,50 +15,57 @@
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
 from engineai.sdk.dashboard.widgets.components.charts.styling import (
-    AreaRangeSeriesStyling,
+    ErrorBarSeriesStyling,
 )
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
-class AreaRangeSeries(TimeseriesBaseSeries):
-    """Spec for a area range series of a Timeseries widget."""
+class ErrorBarSeries(TimeseriesBaseSeries):
+    """Depict data variability with error bars in Timeseries.
 
-    _API_TYPE = "TimeseriesWidgetAreaRangeSeriesInput"
-    _INPUT_KEY = "range"
-    _styling_class = AreaRangeSeriesStyling
+    Construct specifications for an error bar series within a Timeseries widget,
+    providing a visual representation of the variability or uncertainty
+    associated with data points. Each data point is depicted on the chart
+    along with error bars, which indicate the range of possible values or the
+    extent of deviation from a central value.
+    """
+
+    _API_TYPE = "TimeseriesWidgetErrorBarSeriesInput"
+    _INPUT_KEY = "errorBar"
+    _styling_class = ErrorBarSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         low_data_column: Union[str, WidgetField],
         high_data_column: Union[str, WidgetField],
-        name: Union[str, GenericLink],
-        styling: Optional[Union[Palette, AreaRangeSeriesStyling]] = None,
+        name: Optional[Union[str, GenericLink]] = None,
+        styling: Optional[Union[Palette, ErrorBarSeriesStyling]] = None,
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct area range series.
+        """Constructor for ErrorBarSeries.
 
         Args:
-            low_data_column: name of column in pandas dataframe(s) used for the low
-                values of this series.
-            high_data_column: name of column in pandas dataframe(s) used for the high
-                values of this series.
+            low_data_column: name of data column in pandas dataframe(s) used for the
+                low values of this series.
+            high_data_column: name of data column in pandas dataframe(s) used for the
+                high values of this series.
             name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
             entity: entity spec.
             show_in_legend: whether to show series in legend or not.
             required: Flag to make the Series mandatory. If required == True and no
                 Data the widget will show an error. If required==False and no Data,
@@ -69,15 +76,15 @@
         """
         super().__init__(
             name=name,
             data_column=None,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=AreaRangeSeriesStyling(color_spec=styling)
+            styling=ErrorBarSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
         self._low_data_column: Union[str, WidgetField] = (
@@ -91,29 +98,27 @@
         """Validate if dataframe that will be used for series contains required columns.
 
         Args:
             data: pandas dataframe which will be used for table
         """
         super().validate(data=data)
 
-        super()._validate_data_column(
+        self._validate_data_column(
             data=data,
             data_column=self._low_data_column,
             data_column_name="low_data_column",
         )
 
-        super()._validate_data_column(
+        self._validate_data_column(
             data=data,
             data_column=self._high_data_column,
             data_column_name="high_data_column",
         )
 
         if self._entity is not None and isinstance(self._entity, CountryEntity):
             self._entity.validate_country_code()
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
         return {
             "lowKey": build_templated_strings(items=self._low_data_column),
             "highKey": build_templated_strings(items=self._high_data_column),
-            "lowTransforms": [transform.build() for transform in self._transforms],
-            "highTransforms": [transform.build() for transform in self._transforms],
         }
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/base.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,21 @@
 from ..transform import Transform
 from .base import TimeseriesBaseSeries
 
 BubbleSeriesStyling = Union[BubbleCircleSeriesStyling, BubbleCountrySeriesStyling]
 
 
 class BubbleSeries(TimeseriesBaseSeries):
-    """Spec for a bubble series of a Timeseries widget."""
+    """Visualize data with bubbles in Timeseries widget.
+
+    Construct specifications for a bubble series within a Timeseries widget.
+    Visually represent data with bubbles on the chart. The size of each
+    bubble corresponds to a specific data value, providing an intuitive way
+    to grasp the magnitude of each data point.
+    """
 
     _API_TYPE = "TimeseriesWidgetBubbleSeriesInput"
     _INPUT_KEY = "bubble"
     _styling_class = BubbleCircleSeriesStyling
 
     @type_check
     def __init__(
@@ -54,15 +60,15 @@
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct bubble series.
+        """Constructor for BubbleSeries.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for the values of
                 this series associated with the y axis.
             bubble_size_data_column: name of column in pandas dataframe(s) used for
                 the values of this series associated with the size of the bubble.
             name: series name (shown in legend and tooltip).
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/column.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/column.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,15 +20,21 @@
 from engineai.sdk.dashboard.widgets.components.charts.styling import ColumnSeriesStyling
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
 class ColumnSeries(TimeseriesBaseSeries):
-    """Spec for a column series of a Timeseries widget."""
+    """Visualize data as vertical columns in Timeseries widget.
+
+    Construct specifications for a column series within a Timeseries widget to
+    visualize data as vertical columns on the chart. Each column represents a
+    distinct data point, with the height of the column reflecting its
+    corresponding value.
+    """
 
     _API_TYPE = "TimeseriesWidgetColumnSeriesInput"
     _INPUT_KEY = "column"
     _styling_class = ColumnSeriesStyling
 
     @type_check
     def __init__(
@@ -40,15 +46,15 @@
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct column series.
+        """Constructor for ColumnSeries.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for the values of
                 this series.
             name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Spec for error bar series of a Timeseries widget."""
+"""Spec for a area range series of a Timeseries widget."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
@@ -15,50 +15,54 @@
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
 from engineai.sdk.dashboard.widgets.components.charts.styling import (
-    ErrorBarSeriesStyling,
+    AreaRangeSeriesStyling,
 )
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
-class ErrorBarSeries(TimeseriesBaseSeries):
-    """Spec for error bar series of a Timeseries widget."""
+class AreaRangeSeries(TimeseriesBaseSeries):
+    """Visualize data as filled areas between low and high values.
 
-    _API_TYPE = "TimeseriesWidgetErrorBarSeriesInput"
-    _INPUT_KEY = "errorBar"
-    _styling_class = ErrorBarSeriesStyling
+    Construct specifications for an area range series within a Timeseries
+    widget to visualize data as filled areas between low and high values on the chart.
+    """
+
+    _API_TYPE = "TimeseriesWidgetAreaRangeSeriesInput"
+    _INPUT_KEY = "range"
+    _styling_class = AreaRangeSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         low_data_column: Union[str, WidgetField],
         high_data_column: Union[str, WidgetField],
-        name: Optional[Union[str, GenericLink]] = None,
-        styling: Optional[Union[Palette, ErrorBarSeriesStyling]] = None,
+        name: Union[str, GenericLink],
+        styling: Optional[Union[Palette, AreaRangeSeriesStyling]] = None,
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct error bar series.
+        """Constructor for AreaRangeSeries.
 
         Args:
-            low_data_column: name of data column in pandas dataframe(s) used for the
-                low values of this series.
-            high_data_column: name of data column in pandas dataframe(s) used for the
-                high values of this series.
+            low_data_column: name of column in pandas dataframe(s) used for the low
+                values of this series.
+            high_data_column: name of column in pandas dataframe(s) used for the high
+                values of this series.
             name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
             entity: entity spec.
             show_in_legend: whether to show series in legend or not.
             required: Flag to make the Series mandatory. If required == True and no
                 Data the widget will show an error. If required==False and no Data,
@@ -69,15 +73,15 @@
         """
         super().__init__(
             name=name,
             data_column=None,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=ErrorBarSeriesStyling(color_spec=styling)
+            styling=AreaRangeSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
         self._low_data_column: Union[str, WidgetField] = (
@@ -91,27 +95,29 @@
         """Validate if dataframe that will be used for series contains required columns.
 
         Args:
             data: pandas dataframe which will be used for table
         """
         super().validate(data=data)
 
-        self._validate_data_column(
+        super()._validate_data_column(
             data=data,
             data_column=self._low_data_column,
             data_column_name="low_data_column",
         )
 
-        self._validate_data_column(
+        super()._validate_data_column(
             data=data,
             data_column=self._high_data_column,
             data_column_name="high_data_column",
         )
 
         if self._entity is not None and isinstance(self._entity, CountryEntity):
             self._entity.validate_country_code()
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
         return {
             "lowKey": build_templated_strings(items=self._low_data_column),
             "highKey": build_templated_strings(items=self._high_data_column),
+            "lowTransforms": [transform.build() for transform in self._transforms],
+            "highTransforms": [transform.build() for transform in self._transforms],
         }
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/line.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/area.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Spec for a line series of a Timeseries widget."""
+"""Spec for a area series of a Timeseries widget."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
@@ -13,47 +13,51 @@
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
-from engineai.sdk.dashboard.widgets.components.charts.styling import LineSeriesStyling
+from engineai.sdk.dashboard.widgets.components.charts.styling import AreaSeriesStyling
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
-class LineSeries(TimeseriesBaseSeries):
-    """Spec for a line series of a Timeseries widget."""
+class AreaSeries(TimeseriesBaseSeries):
+    """Visualize data as filled areas in Timeseries widget.
 
-    _API_TYPE = "TimeseriesWidgetLineSeriesInput"
-    _INPUT_KEY = "line"
-    _styling_class = LineSeriesStyling
+    Construct specifications for an area series within a Timeseries
+    widget to visualize data as filled areas on the chart.
+    """
+
+    _API_TYPE = "TimeseriesWidgetAreaSeriesInput"
+    _INPUT_KEY = "area"
+    _styling_class = AreaSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
-        styling: Optional[Union[Palette, LineSeriesStyling]] = None,
+        styling: Optional[Union[Palette, AreaSeriesStyling]] = None,
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct line series.
+        """Constructor for AreaSeries.
 
         Args:
-            data_column: name of column in pandas dataframe(s) used for the values
-                of this series.
-            name: series name (shown in legend and tooltip).
+            data_column: name of column in pandas dataframe(s) used for the values of
+                this series.
+            name: series name shown in legend and tooltip.
             styling: styling spec, by default uses the values from the sequential
                 palette.
             entity: entity spec.
             show_in_legend: whether to show series in legend or not.
             required: Flag to make the Series mandatory. If required == True and no
                 Data the widget will show an error. If required==False and no Data,
                 the widget hides the Series.
@@ -63,15 +67,15 @@
         """
         super().__init__(
             name=name,
             data_column=data_column,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=LineSeriesStyling(color_spec=styling)
+            styling=AreaSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
 
@@ -83,8 +87,10 @@
         """
         super().validate(data=data)
 
         if self._entity is not None and isinstance(self._entity, CountryEntity):
             self._entity.validate_country_code()
 
     def _build_extra_inputs(self) -> Dict[str, Any]:
-        return {"transforms": [transform.build() for transform in self._transforms]}
+        return {
+            "transforms": [transform.build() for transform in self._transforms],
+        }
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/point.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/line.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Spec for a point series of a Timeseries widget."""
+"""Spec for a line series of a Timeseries widget."""
 
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pandas as pd
@@ -13,46 +13,52 @@
 from engineai.sdk.dashboard.styling.color import Palette
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.country import (
     CountryEntity,
 )
 from engineai.sdk.dashboard.widgets.components.charts.series.entities.typing import (
     Entities,
 )
-from engineai.sdk.dashboard.widgets.components.charts.styling import PointSeriesStyling
+from engineai.sdk.dashboard.widgets.components.charts.styling import LineSeriesStyling
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
-class PointSeries(TimeseriesBaseSeries):
-    """Spec for a point series of a Timeseries widget."""
+class LineSeries(TimeseriesBaseSeries):
+    """Visualize data with continuous lines in Timeseries.
 
-    _API_TYPE = "TimeseriesWidgetPointSeriesInput"
-    _INPUT_KEY = "point"
-    _styling_class = PointSeriesStyling
+    Construct specifications for a line series within a Timeseries widget to
+    visualize data as a continuous line connecting data points on the chart.
+    Each data point represents a specific value along the timeline, and the
+    lines provide a clear depiction of the trends and patterns present in the data.
+    """
+
+    _API_TYPE = "TimeseriesWidgetLineSeriesInput"
+    _INPUT_KEY = "line"
+    _styling_class = LineSeriesStyling
 
     @type_check
     def __init__(
         self,
         *,
         data_column: Union[str, WidgetField],
         name: Optional[Union[str, GenericLink]] = None,
-        styling: Optional[Union[Palette, PointSeriesStyling]] = None,
+        styling: Optional[Union[Palette, LineSeriesStyling]] = None,
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct point series.
+        """Constructor for LineSeries.
 
         Args:
-            data_column: name of column in pandas dataframe(s) used for the values of
-                this series.
+            data_column: name of column in pandas dataframe(s) used for the values
+                of this series.
             name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
             entity: entity spec.
             show_in_legend: whether to show series in legend or not.
             required: Flag to make the Series mandatory. If required == True and no
                 Data the widget will show an error. If required==False and no Data,
@@ -63,15 +69,15 @@
         """
         super().__init__(
             name=name,
             data_column=data_column,
             show_in_legend=show_in_legend,
             required=required,
             visible=visible,
-            styling=PointSeriesStyling(color_spec=styling)
+            styling=LineSeriesStyling(color_spec=styling)
             if isinstance(styling, Palette)
             else styling,
             entity=entity,
             right_axis=right_axis,
             tooltips=tooltips,
         )
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,21 @@
 )
 
 from ...components.charts.typing import TooltipItems
 from .base import TimeseriesBaseSeries
 
 
 class ScatterSeries(TimeseriesBaseSeries):
-    """Spec for a scatter series of a Timeseries widget."""
+    """Visualize data as individual points in Timeseries.
+
+    Construct specifications for a scatter series within a Timeseries widget
+    to visualize data as individual points on the chart without any connections
+    between them. Each data point is represented by a distinct marker, providing
+    a clear depiction of the data distribution over time.
+    """
 
     _API_TYPE = "TimeseriesWidgetScatterSeriesInput"
     _INPUT_KEY = "scatter"
     _styling_class = ScatterSeriesStyling
 
     @type_check
     def __init__(
@@ -42,15 +48,15 @@
         entity: Optional[Entities] = None,
         show_in_legend: bool = True,
         required: bool = True,
         visible: bool = True,
         right_axis: bool = False,
         tooltips: Optional[TooltipItems] = None,
     ):
-        """Construct scatter series.
+        """Constructor for ScatterSeries.
 
         Args:
             data_column: name of column in pandas dataframe(s) used for the values of
                 this series.
             name: series name (shown in legend and tooltip).
             styling: styling spec, by default uses the values from the sequential
                 palette.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/series/typing.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/timeseries.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,20 @@
 from .period_selector.selector import PeriodSelector
 from .series.line import LineSeries
 from .series.line import LineSeriesStyling
 from .series.typing import TimeseriesSeries
 
 
 class Timeseries(Widget):
-    """Spec for Timeseries widget."""
+    """Visualize charts, customize data, date, toolbar.
+
+    Visualize multiple charts with date selector, navigator, legend.
+    Customize data source, date column, toolbar. Enable or disable
+    toolbar for enhanced user control.
+    """
 
     _HEIGHT_TIMESERIES_PERIOD_SELECTOR = 0.32
     _HEIGHT_TIMESERIES_PERIOD_NAVIGATOR = 0.48
     _HEIGHT_TIMESERIES_LEGENDS_BOTTOM = 0.18
     _HEIGHT_TIMESERIES_LEGENDS_BOTTOM_GROUPED = 0.37
     _WIDGET_API_TYPE = "timeseries"
     _DEPENDENCY_ID = "__TIMESERIES_DATA_DEPENDENCY__"
@@ -72,19 +77,15 @@
         widget_id: Optional[str] = None,
         period_selector: Optional[PeriodSelector] = None,
         title: Optional[WidgetTitleType] = None,
         legend: Optional[LegendPosition] = None,
         navigator: Optional[Union[Navigator, TimeseriesSeries]] = None,
         enable_toolbar: bool = True,
     ):
-        """Class to build a timeseries widget.
-
-        The timeseries widget is a widget that allows to display multiple charts
-        in a single widget. It is possible to add a period selector, a navigator
-        and a legend to the widget.
+        """Constructor for Timeseries widget.
 
         Args:
             data: data to be used by widget. Accepts DataSource method as well as raw
                 data.
             date_column: column that must be used as x axis date. This column must be
                 of type datetime.
             widget_id: unique widget id in a dashboard.
@@ -278,15 +279,19 @@
         if navigator is None or isinstance(navigator, Navigator):
             self.__navigator = navigator
         else:
             self.__navigator = Navigator(navigator)
 
     @type_check
     def set_series(self, *items: Union[str, TimeseriesSeries]) -> "Timeseries":
-        """Set series to a chart in timeseries widget.
+        """Set series for timeseries chart, change type.
+
+        Allows users to set series for a chart within a timeseries widget.
+        Add multiple series to the same chart using this method, enabling the
+        visualization of various data metrics on a single chart.
 
         Args:
             items: series to be added to timeseries widget, using this method you can
                 add multiple series to the same chart. If you want to add multiple
                 charts to the same widget, use set_charts method instead.
 
                 By default, when adding a series, the series will be a line series,
@@ -375,15 +380,20 @@
             for item in list(items)
             if not isinstance(item, str) and item.is_right_axis
         ]
         return YAxis().add_series(*series) if len(series) > 0 else None
 
     @type_check
     def set_charts(self, *items: Union[str, TimeseriesSeries, Chart]) -> "Timeseries":
-        """Set chart(s) into timeseries widget.
+        """Set charts for timeseries widget.
+
+        Allows the addition of one or more charts to a timeseries widget.
+        Include multiple charts within the same widget using this method,
+        allowing for the simultaneous visualization of
+        diverse datasets or metrics
 
         Args:
             items: chart(s) to be added to timeseries widget, using this method you
                 can add multiple charts to the same widget.
 
         Examples:
             ??? example "Add a basic chart with a line series"
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/timeseries/transform.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,24 +8,30 @@
 from engineai.sdk.dashboard.utils import generate_input
 
 from .enums import TransformChoices
 from .exceptions import TimeseriesTransformScalarRequiredError
 
 
 class Transform(AbstractFactoryLinkItemsHandler):
-    """Spec for transforms of a timeseries series."""
+    """Modify data representation in Timeseries with various transformations.
+
+    Define specifications for transforming data within a Timeseries widget
+    to modify or enhance the representation of data series. Select from a
+    range of transformation choices to apply to the data, such as scaling,
+    normalization, or logarithmic transformation, depending on analytical needs.
+    """
 
     @type_check
     def __init__(
         self,
         *,
         transform: TransformChoices,
         scalar: Optional[Union[float, int]] = None,
     ):
-        """Construct a transform for a timeseries widget.
+        """Constructor for Transform.
 
         Args:
             transform: transform to apply to series data.
             scalar: Applies scalar value to data. Only applies when using the
                 following transformations ADD, SUBTRACT, DIVIDE and MULTIPLY.
         """
         super().__init__()
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/toggle/toggle.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/toggle.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 from engineai.sdk.dashboard.widgets.utils import build_data
 
 from ..base import SelectableWidget
 from .exceptions import ToggleValidateValueError
 
 
 class Toggle(SelectableWidget):
-    """Spec for Toggle Widget."""
+    """Enables selection from list, toggling between entries/settings.
+
+    Enables users to select from a list of entries, providing a mechanism to
+    toggle between different selections or settings.
+    """
 
     _DEPENDENCY_ID = "__TOGGLE_DATA_DEPENDENCY__"
     _WIDGET_API_TYPE = "toggle"
     _DEFAULT_HEIGHT = 0.5
     _FORCE_HEIGHT = True
 
     @type_check
@@ -33,15 +37,15 @@
         *,
         id_column: str = "id",
         label: Union[str, WidgetField] = "",
         label_column: Optional[str] = None,
         widget_id: Optional[str] = None,
         default_selection: Optional[str] = None,
     ) -> None:
-        """Construct spec for the Toggle Widget.
+        """Constructor for Toggle widget.
 
         Args:
             id_column: Column name in pandas DataFrame used as entries ids.
             data: data source for the widget.
             label: toggle widget label.
             label_column: Column name in pandas DataFrame used for the
                 widget labeling.
```

### Comparing `engineai_sdk-0.83.1/engineai/sdk/dashboard/widgets/utils.py` & `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/internal/authentication/auth0.py` & `engineai_sdk-0.86.1/engineai/sdk/internal/authentication/auth0.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/internal/authentication/utils.py` & `engineai_sdk-0.86.1/engineai/sdk/internal/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/internal/clients/api.py` & `engineai_sdk-0.86.1/engineai/sdk/internal/clients/api.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/internal/clients/exceptions.py` & `engineai_sdk-0.86.1/engineai/sdk/internal/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/schema.py` & `engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/schema.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/engineai/sdk/internal/graphql_dataclasses/types.py` & `engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.83.1/pyproject.toml` & `engineai_sdk-0.86.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "engineai.sdk"
-version = "0.83.1"
+version = "0.86.1"
 description = "EngineAI's Platform SDK"
 authors = ["Pedro Rodrigues <pedro@dystematic.com>"]
 maintainers = [
   "Pedro Cunha <cunha@engineai.com>",
   "Pedro Feiteira <feiteira@engineai.com>",
   "Li Zixiang <li.zixiang@engineai.com>",
   "Joao Matos <matos@engineai.com>",
@@ -15,15 +15,15 @@
 license = "MIT"
 documentation = "https://docs.engineai.com/"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numpy = "^1"
 pandas = "^1.0 || ^2.0"
-environs = "^11.0.0"
+environs = "^9.2.0"
 pyjwt = "^2.3.0"
 more-itertools = "^9"
 beartype = "^0.17.0"
 tenacity = "^8.2.1"
 pync = "^2.0.3"
 toml = "^0.10.2"
 click = "^8.1.3"
@@ -40,49 +40,42 @@
 rich = "^13.6.0"
 inquirer = "3.1.4"
 
 [tool.poetry.dev-dependencies]
 types-backports = "^0.1.3"
 bandit = "^1.6.2"
 black = "^23.1.0"
-blacken-docs = "^1.16.0"
 coverage = "^7.2.0"
 flake8 = "^5.0.0"
 flake8-black = "^0.3"
 flake8-breakpoint = "^1.1.0"
 flake8-bugbear = "^23.2.13"
 flake8-builtins = "^2.0.1"
 flake8-comprehensions = "^3.2.3"
 flake8-docstrings = "^1.5.0"
 flake8-eradicate = "^1.0.0"
 flake8-mutable = "^1.2.0"
 flake8-print = "^5.0.0"
-flake8-markdown = "^0.4.0"
 mypy = "^1.7"
 pep8-naming = "^0.13.3"
 pre-commit = "^2.8.2"
 pylint = "^2.7.0"
 pytest = "^7.2.0"
 radon = "^5.1.0"
 safety = "^2.3.1"
 isort = "^5.10.1"
 furo = "^2022.04.07"
 faker = "^17.0.0"
 tox = "^4.4.11"
-mkdocs = "^1.4.3"
-mkdocs-material = "^9.1.17"
-mkdocs-click = "^0.8.0"
-mkdocstrings = { extras = ["python"], version = "^0.22.0" }
-mkdocs-macros-plugin = "^1.0.4"
 pygments = "^2.15.1"
 types-toposort = "^1.10"
 
 [[tool.poetry.source]]
 name = "engineaipypi"
-url = "https://nexus.engineai.dev/repository/pypi-dystematic-dev/simple"
+url = "https://nexus.engineai.dev/repository/pypi-dystematic-production/simple"
 
 [build-system]
 requires = ["poetry>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 engineai = "engineai.sdk.cli.console:process"
```

### Comparing `engineai_sdk-0.83.1/PKG-INFO` & `engineai_sdk-0.86.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engineai.sdk
-Version: 0.83.1
+Version: 0.86.1
 Summary: EngineAI's Platform SDK
 License: MIT
 Author: Pedro Rodrigues
 Author-email: pedro@dystematic.com
 Maintainer: Pedro Cunha
 Maintainer-email: cunha@engineai.com
 Requires-Python: >=3.8,<3.12
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.0b0,<4.0.0)
 Requires-Dist: beartype (>=0.17.0,<0.18.0)
 Requires-Dist: brotli (>=1.0.9,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dataclasses-json (>=0.5.2,<0.6.0)
-Requires-Dist: environs (>=11.0.0,<12.0.0)
+Requires-Dist: environs (>=9.2.0,<10.0.0)
 Requires-Dist: inquirer (==3.1.4)
 Requires-Dist: more-itertools (>=9,<10)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: orjson (==3.9.10)
 Requires-Dist: pandas (>=1.0,<3.0)
 Requires-Dist: pyjwt (>=2.3.0,<3.0.0)
@@ -46,15 +46,15 @@
 - Python 3.8 or higher
 
 ### Installation
 
 To install the SDK, run the following command:
 
 ```bash
-pip install engineai-sdk
+pip install engineai.sdk
 ```
 
 ### Create your First Dashboard
 
 To create your dashboard, you need to run the following command:
 
 ```bash
```

