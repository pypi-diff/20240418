# Comparing `tmp/tdf_tool-2.4.4.tar.gz` & `tmp/tdf_tool-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdf_tool-2.4.4.tar", max compression
+gzip compressed data, was "tdf_tool-2.4.5.tar", max compression
```

## Comparing `tdf_tool-2.4.4.tar` & `tdf_tool-2.4.5.tar`

### file list

```diff
@@ -1,164 +1,164 @@
--rw-r--r--   0        0        0     1068 2024-04-16 07:59:17.944743 tdf_tool-2.4.4/LICENSE
--rw-r--r--   0        0        0     9217 2024-04-16 07:59:17.944961 tdf_tool-2.4.4/README.md
--rw-r--r--   0        0        0     1608 2024-04-18 08:34:10.575462 tdf_tool-2.4.4/pyproject.toml
--rw-r--r--   0        0        0      321 2024-04-16 07:59:17.947227 tdf_tool-2.4.4/tdf_tool/app.py
--rw-r--r--   0        0        0     1027 2024-04-17 07:58:00.646956 tdf_tool-2.4.4/tdf_tool/pipeline.py
--rw-r--r--   0        0        0     8469 2024-04-17 06:16:22.770116 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc
--rw-r--r--   0        0        0     4502 2024-04-18 08:28:41.483480 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     7183 2024-04-18 08:28:41.487023 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc
--rw-r--r--   0        0        0      424 2024-04-16 07:59:17.947648 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0     2567 2024-04-16 07:59:17.947827 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
--rw-r--r--   0        0        0     1677 2024-04-17 03:42:57.690636 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
--rw-r--r--   0        0        0     2668 2024-04-16 07:59:17.948134 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
--rw-r--r--   0        0        0     1629 2024-04-17 03:42:57.702854 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0      496 2024-04-16 07:59:17.948441 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
--rw-r--r--   0        0        0     3015 2024-04-16 07:59:17.948597 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
--rw-r--r--   0        0        0     2312 2024-04-17 03:42:57.056562 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
--rw-r--r--   0        0        0     2981 2024-04-16 07:59:17.948929 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
--rw-r--r--   0        0        0     2244 2024-04-17 03:42:57.698366 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
--rw-r--r--   0        0        0    36213 2024-04-16 07:59:17.949402 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
--rw-r--r--   0        0        0    16242 2024-04-17 09:18:30.993839 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
--rw-r--r--   0        0        0     3262 2024-04-16 07:59:17.950144 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0     1990 2024-04-17 03:42:57.553042 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
--rw-r--r--   0        0        0      817 2024-04-16 07:59:17.950609 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
--rw-r--r--   0        0        0      621 2024-04-17 03:42:57.704141 tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
--rw-r--r--   0        0        0     5130 2024-04-18 08:27:43.171640 tdf_tool-2.4.4/tdf_tool/pipelines/annotation.py
--rw-r--r--   0        0        0     7421 2024-04-18 08:28:01.826801 tdf_tool-2.4.4/tdf_tool/pipelines/api_interaction.py
--rw-r--r--   0        0        0     1246 2024-04-16 07:59:17.951140 tdf_tool-2.4.4/tdf_tool/pipelines/fix_header.py
--rw-r--r--   0        0        0     1212 2024-04-16 07:59:17.951401 tdf_tool-2.4.4/tdf_tool/pipelines/git.py
--rw-r--r--   0        0        0     1926 2024-04-16 07:59:17.951649 tdf_tool-2.4.4/tdf_tool/pipelines/module.py
--rw-r--r--   0        0        0     1634 2024-04-16 07:59:17.951927 tdf_tool-2.4.4/tdf_tool/pipelines/package.py
--rw-r--r--   0        0        0    22055 2024-04-17 08:02:42.463284 tdf_tool-2.4.4/tdf_tool/pipelines/router.py
--rw-r--r--   0        0        0     1659 2024-04-16 07:59:17.952587 tdf_tool-2.4.4/tdf_tool/pipelines/translate.py
--rw-r--r--   0        0        0      179 2024-04-16 07:59:17.952763 tdf_tool-2.4.4/tdf_tool/pipelines/upgrade.py
--rw-r--r--   0        0        0     1653 2024-04-16 07:59:17.953204 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
--rw-r--r--   0        0        0     1064 2024-04-17 03:42:57.428644 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0    10270 2024-04-16 07:59:17.953777 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     5149 2024-04-17 03:42:57.424677 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
--rw-r--r--   0        0        0     1328 2024-04-16 07:59:17.954419 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/env.cpython-311.pyc
--rw-r--r--   0        0        0      899 2024-04-17 03:42:57.430200 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/env.cpython-39.pyc
--rw-r--r--   0        0        0     2480 2024-04-16 07:59:17.954948 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1464 2024-04-17 03:42:57.562167 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2969 2024-04-16 07:59:17.955456 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/print.cpython-311.pyc
--rw-r--r--   0        0        0     2040 2024-04-17 03:42:57.419685 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/print.cpython-39.pyc
--rw-r--r--   0        0        0     9661 2024-04-16 07:59:17.955984 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
--rw-r--r--   0        0        0     6181 2024-04-17 03:42:57.564741 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
--rw-r--r--   0        0        0    10739 2024-04-16 07:59:17.956576 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
--rw-r--r--   0        0        0     5620 2024-04-17 07:17:19.963646 tdf_tool-2.4.4/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
--rw-r--r--   0        0        0    11432 2024-04-16 07:59:17.957426 tdf_tool-2.4.4/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
--rw-r--r--   0        0        0     7694 2024-04-17 03:42:57.185360 tdf_tool-2.4.4/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
--rw-r--r--   0        0        0     7216 2024-04-16 07:59:17.958050 tdf_tool-2.4.4/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
--rw-r--r--   0        0        0     4018 2024-04-17 03:42:57.112957 tdf_tool-2.4.4/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
--rw-r--r--   0        0        0     1835 2024-04-17 03:42:57.418130 tdf_tool-2.4.4/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
--rw-r--r--   0        0        0     1628 2024-04-16 07:59:17.959126 tdf_tool-2.4.4/tdf_tool/tools/cli/bean/deps_item.py
--rw-r--r--   0        0        0    12287 2024-04-16 07:59:17.959442 tdf_tool-2.4.4/tdf_tool/tools/cli/module_deps_rewrite.py
--rw-r--r--   0        0        0     5041 2024-04-16 07:59:17.959734 tdf_tool-2.4.4/tdf_tool/tools/cli/project_cli.py
--rw-r--r--   0        0        0     1919 2024-04-17 03:42:57.421774 tdf_tool-2.4.4/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1833 2024-04-16 07:59:17.960396 tdf_tool-2.4.4/tdf_tool/tools/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      559 2024-04-16 07:59:17.960648 tdf_tool-2.4.4/tdf_tool/tools/cmd.py
--rw-r--r--   0        0        0     7002 2024-04-16 07:59:17.961174 tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     3385 2024-04-17 03:42:57.474812 tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     2717 2024-04-16 07:59:17.961718 tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     1491 2024-04-17 07:06:18.116707 tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     2693 2024-04-16 07:59:17.962260 tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0     2732 2024-04-16 07:59:17.962513 tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     2103 2024-04-17 09:18:30.887998 tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     9155 2024-04-16 07:59:17.963058 tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
--rw-r--r--   0        0        0     4496 2024-04-17 03:42:57.689464 tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
--rw-r--r--   0        0        0     3983 2024-04-16 07:59:17.963572 tdf_tool-2.4.4/tdf_tool/tools/config/config.py
--rw-r--r--   0        0        0     1310 2024-04-17 07:03:28.545530 tdf_tool-2.4.4/tdf_tool/tools/config/initial_json_config.py
--rw-r--r--   0        0        0     1267 2024-04-17 09:14:57.974794 tdf_tool-2.4.4/tdf_tool/tools/config/module_json_config.py
--rw-r--r--   0        0        0     5593 2024-04-16 07:59:17.964325 tdf_tool-2.4.4/tdf_tool/tools/config/packages_config.py
--rw-r--r--   0        0        0     7704 2024-04-16 07:59:17.964588 tdf_tool-2.4.4/tdf_tool/tools/dependencies_analysis.py
--rw-r--r--   0        0        0      662 2024-04-16 07:59:17.964838 tdf_tool-2.4.4/tdf_tool/tools/env.py
--rw-r--r--   0        0        0     6312 2024-04-16 07:59:17.965341 tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
--rw-r--r--   0        0        0     3616 2024-04-17 03:42:57.693573 tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
--rw-r--r--   0        0        0     3174 2024-04-16 07:59:17.965839 tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
--rw-r--r--   0        0        0     2004 2024-04-17 03:42:57.692103 tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
--rw-r--r--   0        0        0     4314 2024-04-16 07:59:17.966355 tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
--rw-r--r--   0        0        0     2464 2024-04-17 03:42:57.694912 tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
--rw-r--r--   0        0        0     6437 2024-04-16 07:59:17.966902 tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
--rw-r--r--   0        0        0     3681 2024-04-17 03:42:57.696791 tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
--rw-r--r--   0        0        0     2422 2024-04-16 07:59:17.967708 tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
--rw-r--r--   0        0        0     3345 2024-04-16 07:59:17.967959 tdf_tool-2.4.4/tdf_tool/tools/fix_header/fix_header_entry.py
--rw-r--r--   0        0        0     1586 2024-04-16 07:59:17.968270 tdf_tool-2.4.4/tdf_tool/tools/fix_header/fix_header_lint.py
--rw-r--r--   0        0        0     2137 2024-04-16 07:59:17.968589 tdf_tool-2.4.4/tdf_tool/tools/fix_header/fix_header_lint_tool.py
--rw-r--r--   0        0        0     4095 2024-04-16 07:59:17.968850 tdf_tool-2.4.4/tdf_tool/tools/fix_header/fix_header_replace_tool.py
--rw-r--r--   0        0        0     1159 2024-04-16 07:59:17.969195 tdf_tool-2.4.4/tdf_tool/tools/flutter_script.py
--rw-r--r--   0        0        0     7243 2024-04-16 07:59:17.969845 tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
--rw-r--r--   0        0        0     4190 2024-04-17 03:42:57.549550 tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
--rw-r--r--   0        0        0     7055 2024-04-16 07:59:17.970442 tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
--rw-r--r--   0        0        0     3786 2024-04-17 03:42:57.477039 tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
--rw-r--r--   0        0        0      593 2024-04-16 07:59:17.971051 tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
--rw-r--r--   0        0        0     5019 2024-04-16 07:59:17.971732 tdf_tool-2.4.4/tdf_tool/tools/gitlab/gitlab_utils.py
--rw-r--r--   0        0        0     3814 2024-04-16 07:59:17.972085 tdf_tool-2.4.4/tdf_tool/tools/gitlab/python_gitlab_api.py
--rw-r--r--   0        0        0     2482 2024-04-16 07:59:17.972678 tdf_tool-2.4.4/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1412 2024-04-17 03:42:57.472617 tdf_tool-2.4.4/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1063 2024-04-16 07:59:17.973603 tdf_tool-2.4.4/tdf_tool/tools/module/module_tools.py
--rw-r--r--   0        0        0    11056 2024-04-16 07:59:17.974266 tdf_tool-2.4.4/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
--rw-r--r--   0        0        0     5267 2024-04-17 03:42:57.700870 tdf_tool-2.4.4/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
--rw-r--r--   0        0        0     9752 2024-04-16 07:59:17.974933 tdf_tool-2.4.4/tdf_tool/tools/package/seal_off_package_utils.py
--rw-r--r--   0        0        0      911 2024-04-16 07:59:17.975191 tdf_tool-2.4.4/tdf_tool/tools/platform_tools.py
--rw-r--r--   0        0        0     1226 2024-04-16 07:59:17.975485 tdf_tool-2.4.4/tdf_tool/tools/print.py
--rw-r--r--   0        0        0     7598 2024-04-16 07:59:17.975770 tdf_tool-2.4.4/tdf_tool/tools/regular_tool.py
--rw-r--r--   0        0        0     5718 2024-04-17 07:17:09.536594 tdf_tool-2.4.4/tdf_tool/tools/shell_dir.py
--rw-r--r--   0        0        0     3840 2024-04-16 07:59:17.976600 tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
--rw-r--r--   0        0        0     2161 2024-04-17 03:42:57.656262 tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     2695 2024-04-16 07:59:17.977108 tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     1678 2024-04-17 03:42:57.681260 tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    11711 2024-04-16 07:59:17.977716 tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1999 2024-04-16 07:59:17.977961 tdf_tool-2.4.4/tdf_tool/tools/translate/file_util.py
--rw-r--r--   0        0        0    15484 2024-04-16 07:59:17.978545 tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     8285 2024-04-17 03:42:57.652286 tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    26818 2024-04-16 07:59:17.979344 tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0    13427 2024-04-17 03:42:57.558963 tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0    10691 2024-04-16 07:59:17.980114 tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
--rw-r--r--   0        0        0    18954 2024-04-16 07:59:17.980464 tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
--rw-r--r--   0        0        0     8395 2024-04-16 07:59:17.981075 tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4595 2024-04-17 03:42:57.654824 tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     5228 2024-04-16 07:59:17.981648 tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
--rw-r--r--   0        0        0      859 2024-04-16 07:59:17.982222 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     7351 2024-04-16 07:59:17.982702 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7599 2024-04-16 07:59:17.983077 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
--rw-r--r--   0        0        0     4216 2024-04-17 03:42:57.658661 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
--rw-r--r--   0        0        0     3952 2024-04-16 07:59:17.983786 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     2347 2024-04-17 03:42:57.682489 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0      870 2024-04-16 07:59:17.984330 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0     4766 2024-04-16 07:59:17.984706 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     6219 2024-04-16 07:59:17.985086 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     2631 2024-04-16 07:59:17.985435 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     4438 2024-04-16 07:59:17.985774 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/ios_translate.py
--rw-r--r--   0        0        0     2000 2024-04-16 07:59:17.986154 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/ios_translate_lint.py
--rw-r--r--   0        0        0     5061 2024-04-16 07:59:17.986697 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
--rw-r--r--   0        0        0     2852 2024-04-17 03:42:57.660758 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
--rw-r--r--   0        0        0    17576 2024-04-16 07:59:17.987402 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
--rw-r--r--   0        0        0     9306 2024-04-17 03:42:57.664711 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7901 2024-04-16 07:59:17.988120 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4398 2024-04-17 03:42:57.679975 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     1158 2024-04-16 07:59:17.988695 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
--rw-r--r--   0        0        0     1028 2024-04-17 03:42:57.666587 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0    10070 2024-04-16 07:59:17.989363 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0     5366 2024-04-17 03:42:57.668957 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2773 2024-04-16 07:59:17.989983 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
--rw-r--r--   0        0        0     2689 2024-04-17 03:42:57.675374 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
--rw-r--r--   0        0        0    11353 2024-04-16 07:59:17.990542 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
--rw-r--r--   0        0        0     6226 2024-04-17 03:42:57.678045 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     4943 2024-04-16 07:59:17.991277 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
--rw-r--r--   0        0        0     2687 2024-04-17 03:42:57.671087 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     3270 2024-04-16 07:59:17.991799 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
--rw-r--r--   0        0        0    14326 2024-04-16 07:59:17.992093 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/ios_module.py
--rw-r--r--   0        0        0     5223 2024-04-16 07:59:17.992380 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
--rw-r--r--   0        0        0     1189 2024-04-16 07:59:17.992605 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
--rw-r--r--   0        0        0     8191 2024-04-16 07:59:17.992866 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
--rw-r--r--   0        0        0     2337 2024-04-16 07:59:17.993215 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/location_string_temp.py
--rw-r--r--   0        0        0     8684 2024-04-16 07:59:17.993505 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/podspec.py
--rw-r--r--   0        0        0     2886 2024-04-16 07:59:17.993759 tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/string_util.py
--rw-r--r--   0        0        0     8625 2024-04-16 07:59:17.994344 tdf_tool-2.4.4/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
--rw-r--r--   0        0        0     5032 2024-04-17 03:42:57.673624 tdf_tool-2.4.4/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
--rw-r--r--   0        0        0     5111 2024-04-16 07:59:17.994952 tdf_tool-2.4.4/tdf_tool/tools/translate/tools/translate_tool.py
--rw-r--r--   0        0        0     1408 2024-04-16 07:59:17.995250 tdf_tool-2.4.4/tdf_tool/tools/translate/translate_lint.py
--rw-r--r--   0        0        0     1268 2024-04-16 07:59:17.996782 tdf_tool-2.4.4/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
--rw-r--r--   0        0        0      880 2024-04-17 03:42:57.551180 tdf_tool-2.4.4/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
--rw-r--r--   0        0        0      440 2024-04-16 07:59:17.997353 tdf_tool-2.4.4/tdf_tool/tools/vscode/vscode.py
--rw-r--r--   0        0        0    11029 2024-04-18 08:34:48.857342 tdf_tool-2.4.4/setup.py
--rw-r--r--   0        0        0    10466 2024-04-18 08:34:48.857845 tdf_tool-2.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-16 07:59:17.944743 tdf_tool-2.4.5/LICENSE
+-rw-r--r--   0        0        0     9217 2024-04-16 07:59:17.944961 tdf_tool-2.4.5/README.md
+-rw-r--r--   0        0        0     1608 2024-04-18 09:17:38.034060 tdf_tool-2.4.5/pyproject.toml
+-rw-r--r--   0        0        0      321 2024-04-16 07:59:17.947227 tdf_tool-2.4.5/tdf_tool/app.py
+-rw-r--r--   0        0        0     1106 2024-04-18 09:15:16.438690 tdf_tool-2.4.5/tdf_tool/pipeline.py
+-rw-r--r--   0        0        0     8469 2024-04-17 06:16:22.770116 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc
+-rw-r--r--   0        0        0     4497 2024-04-18 09:17:23.331958 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     7153 2024-04-18 09:13:55.372125 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc
+-rw-r--r--   0        0        0      424 2024-04-16 07:59:17.947648 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0     2567 2024-04-16 07:59:17.947827 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
+-rw-r--r--   0        0        0     1676 2024-04-18 09:17:23.336387 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
+-rw-r--r--   0        0        0     2668 2024-04-16 07:59:17.948134 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
+-rw-r--r--   0        0        0     1619 2024-04-18 09:17:23.343761 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2024-04-16 07:59:17.948441 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
+-rw-r--r--   0        0        0     3015 2024-04-16 07:59:17.948597 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
+-rw-r--r--   0        0        0     2302 2024-04-18 09:17:22.963796 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
+-rw-r--r--   0        0        0     2981 2024-04-16 07:59:17.948929 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
+-rw-r--r--   0        0        0     2243 2024-04-18 09:17:23.340691 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
+-rw-r--r--   0        0        0    36213 2024-04-16 07:59:17.949402 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0        0        0    16242 2024-04-17 09:18:30.993839 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
+-rw-r--r--   0        0        0     3262 2024-04-16 07:59:17.950144 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0     1989 2024-04-18 09:17:23.215708 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
+-rw-r--r--   0        0        0      817 2024-04-16 07:59:17.950609 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
+-rw-r--r--   0        0        0      621 2024-04-17 03:42:57.704141 tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
+-rw-r--r--   0        0        0     5130 2024-04-18 09:17:19.625035 tdf_tool-2.4.5/tdf_tool/pipelines/annotation.py
+-rw-r--r--   0        0        0     7388 2024-04-18 09:13:44.982922 tdf_tool-2.4.5/tdf_tool/pipelines/api_interaction.py
+-rw-r--r--   0        0        0     1244 2024-04-18 09:17:03.333227 tdf_tool-2.4.5/tdf_tool/pipelines/fix_header.py
+-rw-r--r--   0        0        0     1211 2024-04-18 09:16:07.773291 tdf_tool-2.4.5/tdf_tool/pipelines/git.py
+-rw-r--r--   0        0        0     1891 2024-04-18 09:15:46.128657 tdf_tool-2.4.5/tdf_tool/pipelines/module.py
+-rw-r--r--   0        0        0     1630 2024-04-18 09:16:33.493718 tdf_tool-2.4.5/tdf_tool/pipelines/package.py
+-rw-r--r--   0        0        0    22055 2024-04-17 08:02:42.463284 tdf_tool-2.4.5/tdf_tool/pipelines/router.py
+-rw-r--r--   0        0        0     1656 2024-04-18 09:16:44.448736 tdf_tool-2.4.5/tdf_tool/pipelines/translate.py
+-rw-r--r--   0        0        0      179 2024-04-16 07:59:17.952763 tdf_tool-2.4.5/tdf_tool/pipelines/upgrade.py
+-rw-r--r--   0        0        0     1653 2024-04-16 07:59:17.953204 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
+-rw-r--r--   0        0        0     1064 2024-04-17 03:42:57.428644 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0    10270 2024-04-16 07:59:17.953777 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0     5149 2024-04-17 03:42:57.424677 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
+-rw-r--r--   0        0        0     1328 2024-04-16 07:59:17.954419 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/env.cpython-311.pyc
+-rw-r--r--   0        0        0      899 2024-04-17 03:42:57.430200 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0        0        0     2480 2024-04-16 07:59:17.954948 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1464 2024-04-17 03:42:57.562167 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2969 2024-04-16 07:59:17.955456 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/print.cpython-311.pyc
+-rw-r--r--   0        0        0     2040 2024-04-17 03:42:57.419685 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/print.cpython-39.pyc
+-rw-r--r--   0        0        0     9661 2024-04-16 07:59:17.955984 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     6181 2024-04-17 03:42:57.564741 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
+-rw-r--r--   0        0        0    10739 2024-04-16 07:59:17.956576 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
+-rw-r--r--   0        0        0     5620 2024-04-17 07:17:19.963646 tdf_tool-2.4.5/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
+-rw-r--r--   0        0        0    11432 2024-04-16 07:59:17.957426 tdf_tool-2.4.5/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
+-rw-r--r--   0        0        0     7694 2024-04-17 03:42:57.185360 tdf_tool-2.4.5/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
+-rw-r--r--   0        0        0     7216 2024-04-16 07:59:17.958050 tdf_tool-2.4.5/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
+-rw-r--r--   0        0        0     4018 2024-04-17 03:42:57.112957 tdf_tool-2.4.5/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
+-rw-r--r--   0        0        0     1835 2024-04-17 03:42:57.418130 tdf_tool-2.4.5/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
+-rw-r--r--   0        0        0     1628 2024-04-16 07:59:17.959126 tdf_tool-2.4.5/tdf_tool/tools/cli/bean/deps_item.py
+-rw-r--r--   0        0        0    12287 2024-04-16 07:59:17.959442 tdf_tool-2.4.5/tdf_tool/tools/cli/module_deps_rewrite.py
+-rw-r--r--   0        0        0     5041 2024-04-16 07:59:17.959734 tdf_tool-2.4.5/tdf_tool/tools/cli/project_cli.py
+-rw-r--r--   0        0        0     1919 2024-04-17 03:42:57.421774 tdf_tool-2.4.5/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1833 2024-04-16 07:59:17.960396 tdf_tool-2.4.5/tdf_tool/tools/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      559 2024-04-16 07:59:17.960648 tdf_tool-2.4.5/tdf_tool/tools/cmd.py
+-rw-r--r--   0        0        0     7002 2024-04-16 07:59:17.961174 tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     3385 2024-04-17 03:42:57.474812 tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     2717 2024-04-16 07:59:17.961718 tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1491 2024-04-17 07:06:18.116707 tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     2693 2024-04-16 07:59:17.962260 tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0     2732 2024-04-16 07:59:17.962513 tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     2103 2024-04-17 09:18:30.887998 tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     9155 2024-04-16 07:59:17.963058 tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
+-rw-r--r--   0        0        0     4496 2024-04-17 03:42:57.689464 tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
+-rw-r--r--   0        0        0     3983 2024-04-16 07:59:17.963572 tdf_tool-2.4.5/tdf_tool/tools/config/config.py
+-rw-r--r--   0        0        0     1310 2024-04-17 07:03:28.545530 tdf_tool-2.4.5/tdf_tool/tools/config/initial_json_config.py
+-rw-r--r--   0        0        0     1267 2024-04-17 09:14:57.974794 tdf_tool-2.4.5/tdf_tool/tools/config/module_json_config.py
+-rw-r--r--   0        0        0     5593 2024-04-16 07:59:17.964325 tdf_tool-2.4.5/tdf_tool/tools/config/packages_config.py
+-rw-r--r--   0        0        0     7704 2024-04-16 07:59:17.964588 tdf_tool-2.4.5/tdf_tool/tools/dependencies_analysis.py
+-rw-r--r--   0        0        0      662 2024-04-16 07:59:17.964838 tdf_tool-2.4.5/tdf_tool/tools/env.py
+-rw-r--r--   0        0        0     6312 2024-04-16 07:59:17.965341 tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
+-rw-r--r--   0        0        0     3616 2024-04-17 03:42:57.693573 tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
+-rw-r--r--   0        0        0     3174 2024-04-16 07:59:17.965839 tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     2004 2024-04-17 03:42:57.692103 tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
+-rw-r--r--   0        0        0     4314 2024-04-16 07:59:17.966355 tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     2464 2024-04-17 03:42:57.694912 tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     6437 2024-04-16 07:59:17.966902 tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     3681 2024-04-17 03:42:57.696791 tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     2422 2024-04-16 07:59:17.967708 tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     3345 2024-04-16 07:59:17.967959 tdf_tool-2.4.5/tdf_tool/tools/fix_header/fix_header_entry.py
+-rw-r--r--   0        0        0     1586 2024-04-16 07:59:17.968270 tdf_tool-2.4.5/tdf_tool/tools/fix_header/fix_header_lint.py
+-rw-r--r--   0        0        0     2137 2024-04-16 07:59:17.968589 tdf_tool-2.4.5/tdf_tool/tools/fix_header/fix_header_lint_tool.py
+-rw-r--r--   0        0        0     4095 2024-04-16 07:59:17.968850 tdf_tool-2.4.5/tdf_tool/tools/fix_header/fix_header_replace_tool.py
+-rw-r--r--   0        0        0     1159 2024-04-16 07:59:17.969195 tdf_tool-2.4.5/tdf_tool/tools/flutter_script.py
+-rw-r--r--   0        0        0     7243 2024-04-16 07:59:17.969845 tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4190 2024-04-17 03:42:57.549550 tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     7055 2024-04-16 07:59:17.970442 tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
+-rw-r--r--   0        0        0     3786 2024-04-17 03:42:57.477039 tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
+-rw-r--r--   0        0        0      593 2024-04-16 07:59:17.971051 tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
+-rw-r--r--   0        0        0     5019 2024-04-16 07:59:17.971732 tdf_tool-2.4.5/tdf_tool/tools/gitlab/gitlab_utils.py
+-rw-r--r--   0        0        0     3814 2024-04-16 07:59:17.972085 tdf_tool-2.4.5/tdf_tool/tools/gitlab/python_gitlab_api.py
+-rw-r--r--   0        0        0     2482 2024-04-16 07:59:17.972678 tdf_tool-2.4.5/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1412 2024-04-17 03:42:57.472617 tdf_tool-2.4.5/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1063 2024-04-16 07:59:17.973603 tdf_tool-2.4.5/tdf_tool/tools/module/module_tools.py
+-rw-r--r--   0        0        0    11056 2024-04-16 07:59:17.974266 tdf_tool-2.4.5/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     5267 2024-04-17 03:42:57.700870 tdf_tool-2.4.5/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     9752 2024-04-16 07:59:17.974933 tdf_tool-2.4.5/tdf_tool/tools/package/seal_off_package_utils.py
+-rw-r--r--   0        0        0      911 2024-04-16 07:59:17.975191 tdf_tool-2.4.5/tdf_tool/tools/platform_tools.py
+-rw-r--r--   0        0        0     1226 2024-04-16 07:59:17.975485 tdf_tool-2.4.5/tdf_tool/tools/print.py
+-rw-r--r--   0        0        0     7598 2024-04-16 07:59:17.975770 tdf_tool-2.4.5/tdf_tool/tools/regular_tool.py
+-rw-r--r--   0        0        0     5718 2024-04-17 07:17:09.536594 tdf_tool-2.4.5/tdf_tool/tools/shell_dir.py
+-rw-r--r--   0        0        0     3840 2024-04-16 07:59:17.976600 tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2161 2024-04-17 03:42:57.656262 tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     2695 2024-04-16 07:59:17.977108 tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     1678 2024-04-17 03:42:57.681260 tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    11711 2024-04-16 07:59:17.977716 tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1999 2024-04-16 07:59:17.977961 tdf_tool-2.4.5/tdf_tool/tools/translate/file_util.py
+-rw-r--r--   0        0        0    15484 2024-04-16 07:59:17.978545 tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     8285 2024-04-17 03:42:57.652286 tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    26818 2024-04-16 07:59:17.979344 tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0    13427 2024-04-17 03:42:57.558963 tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    10691 2024-04-16 07:59:17.980114 tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
+-rw-r--r--   0        0        0    18954 2024-04-16 07:59:17.980464 tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
+-rw-r--r--   0        0        0     8395 2024-04-16 07:59:17.981075 tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4595 2024-04-17 03:42:57.654824 tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     5228 2024-04-16 07:59:17.981648 tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
+-rw-r--r--   0        0        0      859 2024-04-16 07:59:17.982222 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     7351 2024-04-16 07:59:17.982702 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7599 2024-04-16 07:59:17.983077 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
+-rw-r--r--   0        0        0     4216 2024-04-17 03:42:57.658661 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
+-rw-r--r--   0        0        0     3952 2024-04-16 07:59:17.983786 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     2347 2024-04-17 03:42:57.682489 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0      870 2024-04-16 07:59:17.984330 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0     4766 2024-04-16 07:59:17.984706 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     6219 2024-04-16 07:59:17.985086 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     2631 2024-04-16 07:59:17.985435 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     4438 2024-04-16 07:59:17.985774 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/ios_translate.py
+-rw-r--r--   0        0        0     2000 2024-04-16 07:59:17.986154 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/ios_translate_lint.py
+-rw-r--r--   0        0        0     5061 2024-04-16 07:59:17.986697 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     2852 2024-04-17 03:42:57.660758 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    17576 2024-04-16 07:59:17.987402 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
+-rw-r--r--   0        0        0     9306 2024-04-17 03:42:57.664711 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7901 2024-04-16 07:59:17.988120 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4398 2024-04-17 03:42:57.679975 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     1158 2024-04-16 07:59:17.988695 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
+-rw-r--r--   0        0        0     1028 2024-04-17 03:42:57.666587 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0    10070 2024-04-16 07:59:17.989363 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     5366 2024-04-17 03:42:57.668957 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2773 2024-04-16 07:59:17.989983 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
+-rw-r--r--   0        0        0     2689 2024-04-17 03:42:57.675374 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
+-rw-r--r--   0        0        0    11353 2024-04-16 07:59:17.990542 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
+-rw-r--r--   0        0        0     6226 2024-04-17 03:42:57.678045 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     4943 2024-04-16 07:59:17.991277 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2687 2024-04-17 03:42:57.671087 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     3270 2024-04-16 07:59:17.991799 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
+-rw-r--r--   0        0        0    14326 2024-04-16 07:59:17.992093 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/ios_module.py
+-rw-r--r--   0        0        0     5223 2024-04-16 07:59:17.992380 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
+-rw-r--r--   0        0        0     1189 2024-04-16 07:59:17.992605 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
+-rw-r--r--   0        0        0     8191 2024-04-16 07:59:17.992866 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
+-rw-r--r--   0        0        0     2337 2024-04-16 07:59:17.993215 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/location_string_temp.py
+-rw-r--r--   0        0        0     8684 2024-04-16 07:59:17.993505 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/podspec.py
+-rw-r--r--   0        0        0     2886 2024-04-16 07:59:17.993759 tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/string_util.py
+-rw-r--r--   0        0        0     8625 2024-04-16 07:59:17.994344 tdf_tool-2.4.5/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     5032 2024-04-17 03:42:57.673624 tdf_tool-2.4.5/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     5111 2024-04-16 07:59:17.994952 tdf_tool-2.4.5/tdf_tool/tools/translate/tools/translate_tool.py
+-rw-r--r--   0        0        0     1408 2024-04-16 07:59:17.995250 tdf_tool-2.4.5/tdf_tool/tools/translate/translate_lint.py
+-rw-r--r--   0        0        0     1268 2024-04-16 07:59:17.996782 tdf_tool-2.4.5/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
+-rw-r--r--   0        0        0      880 2024-04-17 03:42:57.551180 tdf_tool-2.4.5/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
+-rw-r--r--   0        0        0      440 2024-04-16 07:59:17.997353 tdf_tool-2.4.5/tdf_tool/tools/vscode/vscode.py
+-rw-r--r--   0        0        0    11029 2024-04-18 09:17:45.002128 tdf_tool-2.4.5/setup.py
+-rw-r--r--   0        0        0    10466 2024-04-18 09:17:45.002982 tdf_tool-2.4.5/PKG-INFO
```

### Comparing `tdf_tool-2.4.4/LICENSE` & `tdf_tool-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/README.md` & `tdf_tool-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/pyproject.toml` & `tdf_tool-2.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 项目信息
 [tool.poetry]
 name = "tdf_tool"
-version = "2.4.4"
+version = "2.4.5"
 description = "二维火 flutter 脚手架工具"
 authors = ["Jian Xu <3386218996@qq.com>", "FanJiao Gai <gaijiaofan@2dfire.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://git.2dfire.net/app/flutter/tools/package_tools"
 repository = "https://git.2dfire.net/app/flutter/tools/package_tools.git"
 keywords = ["tdf", "tdf-tool", "tdf_tool"]
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipeline.py` & `tdf_tool-2.4.5/tdf_tool/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from tdf_tool.pipelines.translate import Translate
 from tdf_tool.pipelines.annotation import Annotation
 from tdf_tool.pipelines.fix_header import FixHeader
 from tdf_tool.pipelines.package import Package
 
 from tdf_tool.pipelines.git import Git
 from tdf_tool.pipelines.upgrade import Upgrade
+from tdf_tool.tools.shell_dir import ShellDir
 
 
 class Pipeline:
     """
     二维火 Flutter 脚手架工具，包含项目构建，依赖分析，git等功能。。
     """
 
     def __init__(self):
+        ShellDir.dirInvalidate()
         self.module = Module()
         self.translate = Translate()
         self.package = Package()
         self.fixHeader = FixHeader()
         
         # 注解整合命令
         self.annotation = Annotation()
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 08:27:43 2024 UTC, .py size: 5130 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7fd9 2066 0a14 0000  a......... f....
+00000000: 610d 0d0a 0000 0000 1fe5 2066 0a14 0000  a......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
@@ -27,256 +27,256 @@
 000001a0: 6410 6411 8400 5a0c 6412 5300 2913 da0a  d.d...Z.d.S.)...
 000001b0: 416e 6e6f 7461 7469 6f6e 7545 0000 000a  AnnotationuE....
 000001c0: 2020 2020 e6a8 a1e5 9d97 e997 b4e6 94af      ............
 000001d0: e68c 81e7 9bb8 e585 b3e5 91bd e4bb a4ef  ................
 000001e0: bc9a 746c 2061 6e6e 6f74 6174 696f 6e20  ..tl annotation 
 000001f0: 2d68 20e6 9fa5 e79c 8be8 afa6 e683 850a  -h .............
 00000200: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-00000210: 0001 0000 0003 0000 0043 0000 0073 4600  .........C...sF.
+00000210: 0001 0000 0003 0000 0043 0000 0073 3e00  .........C...s>.
 00000220: 0000 7400 a001 6401 a101 0100 6402 7c00  ..t...d.....d.|.
-00000230: 5f02 7403 a004 a100 0100 7405 8300 7c00  _.t.......t...|.
-00000240: 5f06 7407 8300 7c00 5f08 7c00 a009 a100  _.t...|._.|.....
-00000250: 7c00 5f0a 740b 7403 a00c a100 8301 6a0d  |._.t.t.......j.
-00000260: 7c00 5f0e 6400 5300 2903 4e75 0c00 0000  |._.d.S.).Nu....
-00000270: e6a3 80e6 b58b e4b8 ad2e 2e2e 5a0c 6275  ............Z.bu
-00000280: 696c 645f 7275 6e6e 6572 290f 7207 0000  ild_runner).r...
-00000290: 00da 0574 6974 6c65 da1c 5f41 6e6e 6f74  ...title.._Annot
-000002a0: 6174 696f 6e5f 5f62 7569 6c64 5275 6e6e  ation__buildRunn
-000002b0: 6572 4e61 6d65 7208 0000 00da 0d64 6972  erNamer......dir
-000002c0: 496e 7661 6c69 6461 7465 7209 0000 00da  Invalidater.....
-000002d0: 1d5f 416e 6e6f 7461 7469 6f6e 5f5f 726f  ._Annotation__ro
-000002e0: 7574 6572 416e 6e6f 7461 7469 6f6e 720a  uterAnnotationr.
-000002f0: 0000 00da 1a5f 416e 6e6f 7461 7469 6f6e  ....._Annotation
-00000300: 5f5f 6170 6941 6e6e 6f74 6174 696f 6eda  __apiAnnotation.
-00000310: 235f 416e 6e6f 7461 7469 6f6e 5f5f 6170  #_Annotation__ap
-00000320: 695f 6275 7369 6e65 7373 4d6f 6475 6c65  i_businessModule
-00000330: 4c69 7374 da1f 5f41 6e6e 6f74 6174 696f  List.._Annotatio
-00000340: 6e5f 5f62 7573 696e 6573 734d 6f64 756c  n__businessModul
-00000350: 654c 6973 7472 0600 0000 da0b 6765 7453  eListr......getS
-00000360: 6865 6c6c 4469 72da 0870 6163 6b61 6765  hellDir..package
-00000370: 73da 195f 416e 6e6f 7461 7469 6f6e 5f5f  s.._Annotation__
-00000380: 7061 636b 6167 6573 4c69 7374 a901 da04  packagesList....
-00000390: 7365 6c66 a900 7218 0000 00f5 6900 0000  self..r.....i...
-000003a0: 2f55 7365 7273 2f78 756a 6961 6e2f 446f  /Users/xujian/Do
-000003b0: 6375 6d65 6e74 732f 3230 3234 2fe6 a8a1  cuments/2024/...
-000003c0: e59d 97e9 97b4 e4ba a4e4 ba92 e9a1 b9e7  ................
-000003d0: 9bae 746c e58d 87e7 baa7 2f70 6163 6b61  ..tl....../packa
-000003e0: 6765 5f74 6f6f 6c73 2f74 6466 5f74 6f6f  ge_tools/tdf_too
-000003f0: 6c2f 7069 7065 6c69 6e65 732f 616e 6e6f  l/pipelines/anno
-00000400: 7461 7469 6f6e 2e70 79da 085f 5f69 6e69  tation.py..__ini
-00000410: 745f 5f10 0000 0073 0e00 0000 0001 0a01  t__....s........
-00000420: 0601 0801 0801 0801 0a01 7a13 416e 6e6f  ..........z.Anno
-00000430: 7461 7469 6f6e 2e5f 5f69 6e69 745f 5f63  tation.__init__c
-00000440: 0100 0000 0000 0000 0000 0000 0600 0000  ................
-00000450: 0800 0000 4300 0000 7324 0100 0074 00a0  ....C...s$...t..
-00000460: 0164 01a1 0101 0074 027c 006a 0383 0144  .d.....t.|.j...D
-00000470: 005d 1a5c 027d 017d 0274 047c 019b 0064  .].\.}.}.t.|...d
-00000480: 027c 029b 009d 0383 0101 0071 1474 0483  .|.........q.t..
-00000490: 0001 0074 0564 0383 017d 037c 0364 046b  ...t.d...}.|.d.k
-000004a0: 0273 4e7c 0364 056b 0272 5874 0664 0683  .sN|.d.k.rXt.d..
-000004b0: 0101 0071 367c 0364 076b 0272 727c 00a0  ...q6|.d.k.rr|..
-000004c0: 07a1 0001 0074 0664 0683 0101 0071 367c  .....t.d.....q6|
-000004d0: 037c 006a 0376 0072 a67c 00a0 087c 03a1  .|.j.v.r.|...|..
-000004e0: 0101 0074 00a0 097c 0364 0817 00a1 0101  ...t...|.d......
-000004f0: 007c 00a0 07a1 0001 0074 0664 0683 0101  .|.......t.d....
-00000500: 0071 367a 5874 0a7c 0383 017d 047c 0474  .q6zXt.|...}.|.t
-00000510: 0b7c 006a 0383 016b 0072 f27c 006a 037c  .|.j...k.r.|.j.|
-00000520: 0419 007d 057c 00a0 087c 05a1 0101 0074  ...}.|...|.....t
-00000530: 00a0 097c 0564 0817 00a1 0101 007c 00a0  ...|.d.......|..
-00000540: 07a1 0001 0074 0664 0683 0101 006e 0a74  .....t.d.....n.t
-00000550: 00a0 0c64 09a1 0101 0057 0071 3604 0074  ...d.....W.q6..t
-00000560: 0d90 0179 1c01 0001 0001 0074 00a0 0c64  ...y.......t...d
-00000570: 09a1 0101 0059 0071 3630 0071 3664 0a53  .....Y.q60.q6d.S
-00000580: 0029 0b75 9f00 0000 0a20 2020 2020 2020  .).u.....       
-00000590: 2074 6c20 616e 6e6f 7461 7469 6f6e 2073   tl annotation s
-000005a0: 7461 7274 efbc 9ae4 bc9a e4bb a5e4 baa4  tart............
-000005b0: e4ba 92e5 bc8f e8bf 9be8 a18c e693 8de4  ................
-000005c0: bd9c efbc 8ce5 afb9 e68c 87e5 ae9a e79a  ................
-000005d0: 84e6 a8a1 e59d 97e6 89a7 e8a1 8ce6 8f8f  ................
-000005e0: e8bf b0e6 9687 e4bb b628 e58c 85e6 8bac  .........(......
-000005f0: e8b7 afe7 94b1 efbc 8c61 7069 e4ba a4e4  .........api....
-00000600: ba92 29e7 949f e688 90e5 928c e887 aae5  ..).............
-00000610: 8aa8 e6b3 a8e5 868c e980 bbe8 be91 0a20  ............... 
-00000620: 2020 2020 2020 2075 2e00 0000 e6a3 80e6         u........
-00000630: b58b e588 b0e4 bba5 e4b8 8be6 a8a1 e59d  ................
-00000640: 97e5 8faf e794 9fe6 8890 e68f 8fe8 bfb0  ................
-00000650: e696 87e4 bbb6 efbc 9a0a 7a02 3a20 755f  ..........z.: u_
-00000660: 0000 00e8 afb7 e8be 93e5 85a5 e99c 80e8  ................
-00000670: a681 e794 9fe6 8890 e68f 8fe8 bfb0 e696  ................
-00000680: 87e4 bbb6 e79a 84e6 a8a1 e59d 97e5 908d  ................
-00000690: e688 96e5 85b6 e4b8 8be6 a087 2869 6e70  ............(inp
-000006a0: 7574 2021 20e9 8080 e587 baef bc8c 616c  ut ! .........al
-000006b0: 6c20 e887 aae5 8aa8 e6b3 a8e5 868c 29ef  l ............).
-000006c0: bc9a fa01 2175 0300 0000 efbc 8172 0100  ....!u.......r..
-000006d0: 0000 da03 616c 6c75 1800 0000 e68f 8fe8  ....allu........
-000006e0: bfb0 e696 87e4 bbb6 e794 9fe6 8890 e5ae  ................
-000006f0: 8ce6 8890 751e 0000 00e8 be93 e585 a5e6  ....u...........
-00000700: 9c89 e8af afef bc8c e8af b7e9 878d e696  ................
-00000710: b0e8 be93 e585 a54e 290e 7207 0000 00da  .......N).r.....
-00000720: 0373 7472 da09 656e 756d 6572 6174 6572  .str..enumerater
-00000730: 1200 0000 da05 7072 696e 74da 0569 6e70  ......print..inp
-00000740: 7574 da04 6578 6974 da1c 5f41 6e6e 6f74  ut..exit.._Annot
-00000750: 6174 696f 6e5f 5f69 6e74 6567 7261 7465  ation__integrate
-00000760: 5f73 6865 6c6c da19 5f41 6e6e 6f74 6174  _shell.._Annotat
-00000770: 696f 6e5f 5f67 656e 6572 6174 6543 6f64  ion__generateCod
-00000780: 6572 0c00 0000 da03 696e 74da 036c 656e  er......int..len
-00000790: da07 7761 726e 696e 67da 0a56 616c 7565  ..warning..Value
-000007a0: 4572 726f 7229 0672 1700 0000 da05 696e  Error).r......in
-000007b0: 6465 78da 0469 7465 6dda 0b6d 6f64 756c  dex..item..modul
-000007c0: 655f 6e61 6d65 da01 695a 0c5f 6d6f 6475  e_name..iZ._modu
-000007d0: 6c65 5f61 6e6d 6572 1800 0000 7218 0000  le_anmer....r...
-000007e0: 0072 1900 0000 da05 7374 6172 7419 0000  .r......start...
-000007f0: 0073 3400 0000 0005 0a01 1201 1401 0602  .s4.............
-00000800: 0801 1001 0a01 0801 0801 0a01 0a01 0a01  ................
-00000810: 0e01 0801 0a02 0201 0801 0e01 0a01 0a01  ................
-00000820: 0e01 0801 0a02 0e01 0e01 7a10 416e 6e6f  ..........z.Anno
-00000830: 7461 7469 6f6e 2e73 7461 7274 2901 da0c  tation.start)...
-00000840: 7461 7267 6574 4d6f 6475 6c65 6302 0000  targetModulec...
-00000850: 0000 0000 0000 0000 0003 0000 0006 0000  ................
-00000860: 0043 0000 0073 8600 0000 7400 a001 7c01  .C...s....t...|.
-00000870: 6401 1700 a101 0100 7c00 6a02 4400 5d6c  d.......|.j.D.]l
-00000880: 7d02 7c02 6a03 7c01 6b02 7214 7c02 6a04  }.|.j.|.k.r.|.j.
-00000890: 6402 6b02 7270 7405 a006 a100 0100 7c00  d.k.rpt.......|.
-000008a0: a007 7c02 6a08 a101 725e 7405 a006 a100  ..|.j...r^t.....
-000008b0: 0100 7409 a00a 7c02 6a08 a101 0100 7c00  ..t...|.j.....|.
-000008c0: a00b a100 0100 7180 7400 a00c 6403 a00d  ......q.t...d...
-000008d0: 7c01 a101 a101 0100 7114 7400 a00c 6404  |.......q.t...d.
-000008e0: a00d 7c01 a101 a101 0100 7114 6400 5300  ..|.......q.d.S.
-000008f0: 2905 4e75 2200 0000 20e6 a8a1 e59d 97e7  ).Nu"... .......
-00000900: 949f e688 90e6 b3a8 e8a7 a3e6 8f8f e8bf  ................
-00000910: b0e6 9687 e4bb b62e 2e2e 4675 5400 0000  ..........FuT...
-00000920: e8af b7e7 a1ae e4bf 9de6 a8a1 e59d 977b  ...............{
-00000930: 307d e5b7 b2e4 be9d e8b5 9662 7569 6c64  0}.........build
-00000940: 5f72 756e 6e65 72ef bc8c e58f afe5 8f82  _runner.........
-00000950: e880 83e5 85b6 e4bb 96e6 a8a1 e59d 97e8  ................
-00000960: bf9b e8a1 8ce4 be9d e8b5 96e9 858d e7bd  ................
-00000970: aee2 9d8c 754b 0000 00e6 a380 e6b5 8be5  ....uK..........
-00000980: 88b0 e6a8 a1e5 9d97 7b30 7de5 bd93 e589  ........{0}.....
-00000990: 8de6 98af e8bf 9ce7 a88b e4be 9de8 b596  ................
-000009a0: efbc 8ce6 97a0 e6b3 95e7 949f e688 90e8  ................
-000009b0: b7af e794 b1e6 8f8f e8bf b0e6 9687 e4bb  ................
-000009c0: b6e2 9d8c 290e 7207 0000 0072 0c00 0000  ....).r....r....
-000009d0: 7215 0000 00da 0b70 6163 6b61 6765 4e61  r......packageNa
-000009e0: 6d65 5a08 6973 5265 6d6f 7465 7208 0000  meZ.isRemoter...
-000009f0: 00da 0c67 6f49 6e53 6865 6c6c 4469 72da  ...goInShellDir.
-00000a00: 275f 416e 6e6f 7461 7469 6f6e 5f5f 6a75  '_Annotation__ju
-00000a10: 6467 6548 6173 4275 696c 6452 756e 6e65  dgeHasBuildRunne
-00000a20: 7250 6163 6b61 6765 5a0b 7061 636b 6167  rPackageZ.packag
-00000a30: 6550 6174 68da 026f 73da 0563 6864 6972  ePath..os..chdir
-00000a40: da1a 5f41 6e6e 6f74 6174 696f 6e5f 5f67  .._Annotation__g
-00000a50: 656e 6572 6174 6f72 4675 6e63 721d 0000  eneratorFuncr...
-00000a60: 00da 0666 6f72 6d61 7429 0372 1700 0000  ...format).r....
-00000a70: 722d 0000 0072 2900 0000 7218 0000 0072  r-...r)...r....r
-00000a80: 1800 0000 7219 0000 005a 0e5f 5f67 656e  ....r....Z.__gen
-00000a90: 6572 6174 6543 6f64 653d 0000 0073 2200  erateCode=...s".
-00000aa0: 0000 0001 0e01 0a01 0a01 0a01 0801 0c01  ................
-00000ab0: 0801 0c01 0a02 0401 0401 02ff 02ff 0606  ................
-00000ac0: 0401 08ff 7a19 416e 6e6f 7461 7469 6f6e  ....z.Annotation
-00000ad0: 2e5f 5f67 656e 6572 6174 6543 6f64 6563  .__generateCodec
-00000ae0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000af0: 0300 0000 4300 0000 7318 0000 0074 00a0  ....C...s....t..
-00000b00: 0164 01a1 0101 0074 00a0 0164 02a1 0101  .d.....t...d....
-00000b10: 0064 0053 0029 034e 7a2b 666c 7574 7465  .d.S.).Nz+flutte
-00000b20: 7220 7061 636b 6167 6573 2070 7562 2072  r packages pub r
-00000b30: 756e 2062 7569 6c64 5f72 756e 6e65 7220  un build_runner 
-00000b40: 636c 6561 6e7a 4866 6c75 7474 6572 2070  cleanzHflutter p
-00000b50: 6163 6b61 6765 7320 7075 6220 7275 6e20  ackages pub run 
-00000b60: 6275 696c 645f 7275 6e6e 6572 2062 7569  build_runner bui
-00000b70: 6c64 202d 2d64 656c 6574 652d 636f 6e66  ld --delete-conf
-00000b80: 6c69 6374 696e 672d 6f75 7470 7574 7329  licting-outputs)
-00000b90: 0272 3100 0000 da06 7379 7374 656d 7216  .r1.....systemr.
-00000ba0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000bb0: 0000 5a0f 5f5f 6765 6e65 7261 746f 7246  ..Z.__generatorF
-00000bc0: 756e 6352 0000 0073 0800 0000 0001 0a01  uncR...s........
-00000bd0: 0401 02ff 7a1a 416e 6e6f 7461 7469 6f6e  ....z.Annotation
-00000be0: 2e5f 5f67 656e 6572 6174 6f72 4675 6e63  .__generatorFunc
-00000bf0: 2902 da0e 7061 636b 6167 654c 6962 5061  )...packageLibPa
-00000c00: 7468 da06 7265 7475 726e 6302 0000 0000  th..returnc.....
-00000c10: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
-00000c20: 0000 0073 3e00 0000 7400 a001 7c01 a101  ...s>...t...|...
-00000c30: 0100 7402 7400 a003 a100 6401 6402 8d02  ..t.t.....d.d...
-00000c40: 7d02 6401 7d03 7c02 6a04 4400 5d14 7d04  }.d.}.|.j.D.].}.
-00000c50: 7c04 6a05 7c00 6a06 6b02 7224 6403 7d03  |.j.|.j.k.r$d.}.
-00000c60: 7124 7c03 5300 2904 4e46 2901 5a0d 6669  q$|.S.).NF).Z.fi
-00000c70: 6c74 6572 5f62 795f 7464 6654 2907 7231  lter_by_tdfT).r1
-00000c80: 0000 0072 3200 0000 7206 0000 00da 0667  ...r2...r......g
-00000c90: 6574 6377 6472 1400 0000 722e 0000 0072  etcwdr....r....r
-00000ca0: 0d00 0000 2905 7217 0000 0072 3600 0000  ....).r....r6...
-00000cb0: 5a11 7061 636b 6167 654a 736f 6e43 6f6e  Z.packageJsonCon
-00000cc0: 6669 675a 0e68 6173 4275 696c 6452 756e  figZ.hasBuildRun
-00000cd0: 6e65 7272 2900 0000 7218 0000 0072 1800  nerr)...r....r..
-00000ce0: 0000 7219 0000 005a 1c5f 5f6a 7564 6765  ..r....Z.__judge
-00000cf0: 4861 7342 7569 6c64 5275 6e6e 6572 5061  HasBuildRunnerPa
-00000d00: 636b 6167 6559 0000 0073 1200 0000 0001  ckageY...s......
-00000d10: 0a01 0201 08ff 0603 0401 0a01 0c01 0602  ................
-00000d20: 7a27 416e 6e6f 7461 7469 6f6e 2e5f 5f6a  z'Annotation.__j
-00000d30: 7564 6765 4861 7342 7569 6c64 5275 6e6e  udgeHasBuildRunn
-00000d40: 6572 5061 636b 6167 6563 0100 0000 0000  erPackagec......
-00000d50: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000d60: 0000 7322 0000 007c 006a 00a0 01a1 0001  ..s"...|.j......
-00000d70: 007c 006a 02a0 01a1 0001 0074 03a0 0464  .|.j.......t...d
-00000d80: 01a1 0101 0064 0053 0029 024e 750c 0000  .....d.S.).Nu...
-00000d90: 00e6 95b4 e590 88e5 ae8c e688 9029 0572  .............).r
-00000da0: 0f00 0000 5a0f 696e 7465 6772 6174 655f  ....Z.integrate_
-00000db0: 7368 656c 6c72 1000 0000 7207 0000 0072  shellr....r....r
-00000dc0: 0c00 0000 7216 0000 0072 1800 0000 7218  ....r....r....r.
-00000dd0: 0000 0072 1900 0000 5a11 5f5f 696e 7465  ...r....Z.__inte
-00000de0: 6772 6174 655f 7368 656c 6c66 0000 0073  grate_shellf...s
-00000df0: 0600 0000 0001 0a01 0a01 7a1c 416e 6e6f  ..........z.Anno
-00000e00: 7461 7469 6f6e 2e5f 5f69 6e74 6567 7261  tation.__integra
-00000e10: 7465 5f73 6865 6c6c 6301 0000 0000 0000  te_shellc.......
-00000e20: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
-00000e30: 0073 6000 0000 7400 8300 7d01 6700 7d02  .s`...t...}.g.}.
-00000e40: 7401 8300 6a02 4400 5d48 7d03 7c01 a003  t...j.D.]H}.|...
-00000e50: 7c03 a101 7d04 7c04 6a04 7405 6a06 6b02  |...}.|.j.t.j.k.
-00000e60: 7350 7c04 6a04 7405 6a07 6b02 7350 7c04  sP|.j.t.j.k.sP|.
-00000e70: 6a04 7405 6a08 6b02 7350 7c04 6a04 7405  j.t.j.k.sP|.j.t.
-00000e80: 6a09 6b02 7212 7c02 a00a 7c03 a101 0100  j.k.r.|...|.....
-00000e90: 7112 7c02 5300 2901 4e29 0b72 0400 0000  q.|.S.).N).r....
-00000ea0: 7202 0000 00da 0e6d 6f64 756c 654e 616d  r......moduleNam
-00000eb0: 654c 6973 74da 0867 6574 5f69 7465 6dda  eList..get_item.
-00000ec0: 0474 7970 6572 0300 0000 da03 4c69 62da  .typer......Lib.
-00000ed0: 0341 7069 da06 4d6f 6475 6c65 da06 506c  .Api..Module..Pl
-00000ee0: 7567 696e da06 6170 7065 6e64 2905 7217  ugin..append).r.
-00000ef0: 0000 005a 1a5f 416e 6e6f 7461 7469 6f6e  ...Z._Annotation
-00000f00: 5f5f 6d6f 6475 6c65 5f63 6f6e 6669 675a  __module_configZ
-00000f10: 115f 416e 6e6f 7461 7469 6f6e 5f5f 6c69  ._Annotation__li
-00000f20: 7374 7229 0000 005a 0a63 6f66 6967 5f69  str)...Z.cofig_i
-00000f30: 7465 6d72 1800 0000 7218 0000 0072 1900  temr....r....r..
-00000f40: 0000 5a18 5f5f 6170 695f 6275 7369 6e65  ..Z.__api_busine
-00000f50: 7373 4d6f 6475 6c65 4c69 7374 6b00 0000  ssModuleListk...
-00000f60: 731c 0000 0000 0106 0104 010c 010a 020a  s...............
-00000f70: ff02 020a fe02 030a fd02 040a fc02 060c  ................
-00000f80: 017a 2341 6e6e 6f74 6174 696f 6e2e 5f5f  .z#Annotation.__
-00000f90: 6170 695f 6275 7369 6e65 7373 4d6f 6475  api_businessModu
-00000fa0: 6c65 4c69 7374 4e29 0dda 085f 5f6e 616d  leListN)...__nam
-00000fb0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000fc0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00000fd0: 5f64 6f63 5f5f 721a 0000 0072 2c00 0000  _doc__r....r,...
-00000fe0: 721d 0000 0072 2300 0000 7233 0000 00da  r....r#...r3....
-00000ff0: 0462 6f6f 6c72 3000 0000 7222 0000 0072  .boolr0...r"...r
-00001000: 1100 0000 7218 0000 0072 1800 0000 7218  ....r....r....r.
-00001010: 0000 0072 1900 0000 720b 0000 000b 0000  ...r....r.......
-00001020: 0073 1000 0000 0801 0404 0809 0824 0e15  .s...........$..
-00001030: 0807 100d 0805 720b 0000 0029 1272 3100  ......r....).r1.
-00001040: 0000 da29 7464 665f 746f 6f6c 2e74 6f6f  ...)tdf_tool.too
-00001050: 6c73 2e63 6f6e 6669 672e 696e 6974 6961  ls.config.initia
-00001060: 6c5f 6a73 6f6e 5f63 6f6e 6669 6772 0200  l_json_configr..
-00001070: 0000 da28 7464 665f 746f 6f6c 2e74 6f6f  ...(tdf_tool.too
-00001080: 6c73 2e63 6f6e 6669 672e 6d6f 6475 6c65  ls.config.module
-00001090: 5f6a 736f 6e5f 636f 6e66 6967 7203 0000  _json_configr...
-000010a0: 0072 0400 0000 5a25 7464 665f 746f 6f6c  .r....Z%tdf_tool
-000010b0: 2e74 6f6f 6c73 2e63 6f6e 6669 672e 7061  .tools.config.pa
-000010c0: 636b 6167 6573 5f63 6f6e 6669 6772 0500  ckages_configr..
-000010d0: 0000 7206 0000 00da 1474 6466 5f74 6f6f  ..r......tdf_too
-000010e0: 6c2e 746f 6f6c 732e 7072 696e 7472 0700  l.tools.printr..
-000010f0: 0000 da18 7464 665f 746f 6f6c 2e74 6f6f  ....tdf_tool.too
-00001100: 6c73 2e73 6865 6c6c 5f64 6972 7208 0000  ls.shell_dirr...
-00001110: 005a 1974 6466 5f74 6f6f 6c2e 7069 7065  .Z.tdf_tool.pipe
-00001120: 6c69 6e65 732e 726f 7574 6572 7209 0000  lines.routerr...
-00001130: 005a 2274 6466 5f74 6f6f 6c2e 7069 7065  .Z"tdf_tool.pipe
-00001140: 6c69 6e65 732e 6170 695f 696e 7465 7261  lines.api_intera
-00001150: 6374 696f 6e72 0a00 0000 720b 0000 0072  ctionr....r....r
-00001160: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-00001170: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001180: 0073 1000 0000 0801 0c01 1001 1001 0c01  .s..............
-00001190: 0c02 0c01 0c02                           ......
+00000230: 5f02 7403 8300 7c00 5f04 7405 8300 7c00  _.t...|._.t...|.
+00000240: 5f06 7c00 a007 a100 7c00 5f08 7409 740a  _.|.....|._.t.t.
+00000250: a00b a100 8301 6a0c 7c00 5f0d 6400 5300  ......j.|._.d.S.
+00000260: 2903 4e75 0c00 0000 e6a3 80e6 b58b e4b8  ).Nu............
+00000270: ad2e 2e2e 5a0c 6275 696c 645f 7275 6e6e  ....Z.build_runn
+00000280: 6572 290e 7207 0000 00da 0574 6974 6c65  er).r......title
+00000290: da1c 5f41 6e6e 6f74 6174 696f 6e5f 5f62  .._Annotation__b
+000002a0: 7569 6c64 5275 6e6e 6572 4e61 6d65 7209  uildRunnerNamer.
+000002b0: 0000 00da 1d5f 416e 6e6f 7461 7469 6f6e  ....._Annotation
+000002c0: 5f5f 726f 7574 6572 416e 6e6f 7461 7469  __routerAnnotati
+000002d0: 6f6e 720a 0000 00da 1a5f 416e 6e6f 7461  onr......_Annota
+000002e0: 7469 6f6e 5f5f 6170 6941 6e6e 6f74 6174  tion__apiAnnotat
+000002f0: 696f 6eda 235f 416e 6e6f 7461 7469 6f6e  ion.#_Annotation
+00000300: 5f5f 6170 695f 6275 7369 6e65 7373 4d6f  __api_businessMo
+00000310: 6475 6c65 4c69 7374 da1f 5f41 6e6e 6f74  duleList.._Annot
+00000320: 6174 696f 6e5f 5f62 7573 696e 6573 734d  ation__businessM
+00000330: 6f64 756c 654c 6973 7472 0600 0000 7208  oduleListr....r.
+00000340: 0000 00da 0b67 6574 5368 656c 6c44 6972  .....getShellDir
+00000350: da08 7061 636b 6167 6573 da19 5f41 6e6e  ..packages.._Ann
+00000360: 6f74 6174 696f 6e5f 5f70 6163 6b61 6765  otation__package
+00000370: 734c 6973 74a9 01da 0473 656c 66a9 0072  sList....self..r
+00000380: 1700 0000 f569 0000 002f 5573 6572 732f  .....i.../Users/
+00000390: 7875 6a69 616e 2f44 6f63 756d 656e 7473  xujian/Documents
+000003a0: 2f32 3032 342f e6a8 a1e5 9d97 e997 b4e4  /2024/..........
+000003b0: baa4 e4ba 92e9 a1b9 e79b ae74 6ce5 8d87  ...........tl...
+000003c0: e7ba a72f 7061 636b 6167 655f 746f 6f6c  .../package_tool
+000003d0: 732f 7464 665f 746f 6f6c 2f70 6970 656c  s/tdf_tool/pipel
+000003e0: 696e 6573 2f61 6e6e 6f74 6174 696f 6e2e  ines/annotation.
+000003f0: 7079 da08 5f5f 696e 6974 5f5f 1000 0000  py..__init__....
+00000400: 730c 0000 0000 010a 0106 0208 0108 010a  s...............
+00000410: 017a 1341 6e6e 6f74 6174 696f 6e2e 5f5f  .z.Annotation.__
+00000420: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00000430: 0000 0006 0000 0008 0000 0043 0000 0073  ...........C...s
+00000440: 2c01 0000 7400 a001 a100 0100 7402 a003  ,...t.......t...
+00000450: 6401 a101 0100 7404 7c00 6a05 8301 4400  d.....t.|.j...D.
+00000460: 5d1a 5c02 7d01 7d02 7406 7c01 9b00 6402  ].\.}.}.t.|...d.
+00000470: 7c02 9b00 9d03 8301 0100 711c 7406 8300  |.........q.t...
+00000480: 0100 7407 6403 8301 7d03 7c03 6404 6b02  ..t.d...}.|.d.k.
+00000490: 7356 7c03 6405 6b02 7260 7408 6406 8301  sV|.d.k.r`t.d...
+000004a0: 0100 713e 7c03 6407 6b02 727a 7c00 a009  ..q>|.d.k.rz|...
+000004b0: a100 0100 7408 6406 8301 0100 713e 7c03  ....t.d.....q>|.
+000004c0: 7c00 6a05 7600 72ae 7c00 a00a 7c03 a101  |.j.v.r.|...|...
+000004d0: 0100 7402 a00b 7c03 6408 1700 a101 0100  ..t...|.d.......
+000004e0: 7c00 a009 a100 0100 7408 6406 8301 0100  |.......t.d.....
+000004f0: 713e 7a58 740c 7c03 8301 7d04 7c04 740d  q>zXt.|...}.|.t.
+00000500: 7c00 6a05 8301 6b00 72fa 7c00 6a05 7c04  |.j...k.r.|.j.|.
+00000510: 1900 7d05 7c00 a00a 7c05 a101 0100 7402  ..}.|...|.....t.
+00000520: a00b 7c05 6408 1700 a101 0100 7c00 a009  ..|.d.......|...
+00000530: a100 0100 7408 6406 8301 0100 6e0a 7402  ....t.d.....n.t.
+00000540: a00e 6409 a101 0100 5700 713e 0400 740f  ..d.....W.q>..t.
+00000550: 9001 7924 0100 0100 0100 7402 a00e 6409  ..y$......t...d.
+00000560: a101 0100 5900 713e 3000 713e 640a 5300  ....Y.q>0.q>d.S.
+00000570: 290b 759f 0000 000a 2020 2020 2020 2020  ).u.....        
+00000580: 746c 2061 6e6e 6f74 6174 696f 6e20 7374  tl annotation st
+00000590: 6172 74ef bc9a e4bc 9ae4 bba5 e4ba a4e4  art.............
+000005a0: ba92 e5bc 8fe8 bf9b e8a1 8ce6 938d e4bd  ................
+000005b0: 9cef bc8c e5af b9e6 8c87 e5ae 9ae7 9a84  ................
+000005c0: e6a8 a1e5 9d97 e689 a7e8 a18c e68f 8fe8  ................
+000005d0: bfb0 e696 87e4 bbb6 28e5 8c85 e68b ace8  ........(.......
+000005e0: b7af e794 b1ef bc8c 6170 69e4 baa4 e4ba  ........api.....
+000005f0: 9229 e794 9fe6 8890 e592 8ce8 87aa e58a  .)..............
+00000600: a8e6 b3a8 e586 8ce9 80bb e8be 910a 2020  ..............  
+00000610: 2020 2020 2020 752e 0000 00e6 a380 e6b5        u.........
+00000620: 8be5 88b0 e4bb a5e4 b88b e6a8 a1e5 9d97  ................
+00000630: e58f afe7 949f e688 90e6 8f8f e8bf b0e6  ................
+00000640: 9687 e4bb b6ef bc9a 0a7a 023a 2075 5f00  .........z.: u_.
+00000650: 0000 e8af b7e8 be93 e585 a5e9 9c80 e8a6  ................
+00000660: 81e7 949f e688 90e6 8f8f e8bf b0e6 9687  ................
+00000670: e4bb b6e7 9a84 e6a8 a1e5 9d97 e590 8de6  ................
+00000680: 8896 e585 b6e4 b88b e6a0 8728 696e 7075  ...........(inpu
+00000690: 7420 2120 e980 80e5 87ba efbc 8c61 6c6c  t ! .........all
+000006a0: 20e8 87aa e58a a8e6 b3a8 e586 8c29 efbc   ............)..
+000006b0: 9afa 0121 7503 0000 00ef bc81 7201 0000  ...!u.......r...
+000006c0: 00da 0361 6c6c 7518 0000 00e6 8f8f e8bf  ...allu.........
+000006d0: b0e6 9687 e4bb b6e7 949f e688 90e5 ae8c  ................
+000006e0: e688 9075 1e00 0000 e8be 93e5 85a5 e69c  ...u............
+000006f0: 89e8 afaf efbc 8ce8 afb7 e987 8de6 96b0  ................
+00000700: e8be 93e5 85a5 4e29 1072 0800 0000 da0c  ......N).r......
+00000710: 676f 496e 5368 656c 6c44 6972 7207 0000  goInShellDirr...
+00000720: 00da 0373 7472 da09 656e 756d 6572 6174  ...str..enumerat
+00000730: 6572 1100 0000 da05 7072 696e 74da 0569  er......print..i
+00000740: 6e70 7574 da04 6578 6974 da1c 5f41 6e6e  nput..exit.._Ann
+00000750: 6f74 6174 696f 6e5f 5f69 6e74 6567 7261  otation__integra
+00000760: 7465 5f73 6865 6c6c da19 5f41 6e6e 6f74  te_shell.._Annot
+00000770: 6174 696f 6e5f 5f67 656e 6572 6174 6543  ation__generateC
+00000780: 6f64 6572 0c00 0000 da03 696e 74da 036c  oder......int..l
+00000790: 656e da07 7761 726e 696e 67da 0a56 616c  en..warning..Val
+000007a0: 7565 4572 726f 7229 0672 1600 0000 da05  ueError).r......
+000007b0: 696e 6465 78da 0469 7465 6dda 0b6d 6f64  index..item..mod
+000007c0: 756c 655f 6e61 6d65 da01 695a 0c5f 6d6f  ule_name..iZ._mo
+000007d0: 6475 6c65 5f61 6e6d 6572 1700 0000 7217  dule_anmer....r.
+000007e0: 0000 0072 1800 0000 da05 7374 6172 7419  ...r......start.
+000007f0: 0000 0073 3600 0000 0004 0802 0a01 1201  ...s6...........
+00000800: 1401 0602 0801 1001 0a01 0801 0801 0a01  ................
+00000810: 0a01 0a01 0e01 0801 0a02 0201 0801 0e01  ................
+00000820: 0a01 0a01 0e01 0801 0a02 0e01 0e01 7a10  ..............z.
+00000830: 416e 6e6f 7461 7469 6f6e 2e73 7461 7274  Annotation.start
+00000840: 2901 da0c 7461 7267 6574 4d6f 6475 6c65  )...targetModule
+00000850: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000860: 0006 0000 0043 0000 0073 8600 0000 7400  .....C...s....t.
+00000870: a001 7c01 6401 1700 a101 0100 7c00 6a02  ..|.d.......|.j.
+00000880: 4400 5d6c 7d02 7c02 6a03 7c01 6b02 7214  D.]l}.|.j.|.k.r.
+00000890: 7c02 6a04 6402 6b02 7270 7405 a006 a100  |.j.d.k.rpt.....
+000008a0: 0100 7c00 a007 7c02 6a08 a101 725e 7405  ..|...|.j...r^t.
+000008b0: a006 a100 0100 7409 a00a 7c02 6a08 a101  ......t...|.j...
+000008c0: 0100 7c00 a00b a100 0100 7180 7400 a00c  ..|.......q.t...
+000008d0: 6403 a00d 7c01 a101 a101 0100 7114 7400  d...|.......q.t.
+000008e0: a00c 6404 a00d 7c01 a101 a101 0100 7114  ..d...|.......q.
+000008f0: 6400 5300 2905 4e75 2200 0000 20e6 a8a1  d.S.).Nu"... ...
+00000900: e59d 97e7 949f e688 90e6 b3a8 e8a7 a3e6  ................
+00000910: 8f8f e8bf b0e6 9687 e4bb b62e 2e2e 4675  ..............Fu
+00000920: 5400 0000 e8af b7e7 a1ae e4bf 9de6 a8a1  T...............
+00000930: e59d 977b 307d e5b7 b2e4 be9d e8b5 9662  ...{0}.........b
+00000940: 7569 6c64 5f72 756e 6e65 72ef bc8c e58f  uild_runner.....
+00000950: afe5 8f82 e880 83e5 85b6 e4bb 96e6 a8a1  ................
+00000960: e59d 97e8 bf9b e8a1 8ce4 be9d e8b5 96e9  ................
+00000970: 858d e7bd aee2 9d8c 754b 0000 00e6 a380  ........uK......
+00000980: e6b5 8be5 88b0 e6a8 a1e5 9d97 7b30 7de5  ............{0}.
+00000990: bd93 e589 8de6 98af e8bf 9ce7 a88b e4be  ................
+000009a0: 9de8 b596 efbc 8ce6 97a0 e6b3 95e7 949f  ................
+000009b0: e688 90e8 b7af e794 b1e6 8f8f e8bf b0e6  ................
+000009c0: 9687 e4bb b6e2 9d8c 290e 7207 0000 0072  ........).r....r
+000009d0: 0c00 0000 7214 0000 00da 0b70 6163 6b61  ....r......packa
+000009e0: 6765 4e61 6d65 5a08 6973 5265 6d6f 7465  geNameZ.isRemote
+000009f0: 7208 0000 0072 1c00 0000 da27 5f41 6e6e  r....r.....'_Ann
+00000a00: 6f74 6174 696f 6e5f 5f6a 7564 6765 4861  otation__judgeHa
+00000a10: 7342 7569 6c64 5275 6e6e 6572 5061 636b  sBuildRunnerPack
+00000a20: 6167 655a 0b70 6163 6b61 6765 5061 7468  ageZ.packagePath
+00000a30: da02 6f73 da05 6368 6469 72da 1a5f 416e  ..os..chdir.._An
+00000a40: 6e6f 7461 7469 6f6e 5f5f 6765 6e65 7261  notation__genera
+00000a50: 746f 7246 756e 6372 1d00 0000 da06 666f  torFuncr......fo
+00000a60: 726d 6174 2903 7216 0000 0072 2d00 0000  rmat).r....r-...
+00000a70: 7229 0000 0072 1700 0000 7217 0000 0072  r)...r....r....r
+00000a80: 1800 0000 5a0e 5f5f 6765 6e65 7261 7465  ....Z.__generate
+00000a90: 436f 6465 3e00 0000 7322 0000 0000 010e  Code>...s"......
+00000aa0: 010a 010a 010a 0108 010c 0108 010c 010a  ................
+00000ab0: 0204 0104 0102 ff02 ff06 0604 0108 ff7a  ...............z
+00000ac0: 1941 6e6e 6f74 6174 696f 6e2e 5f5f 6765  .Annotation.__ge
+00000ad0: 6e65 7261 7465 436f 6465 6301 0000 0000  nerateCodec.....
+00000ae0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00000af0: 0000 0073 1800 0000 7400 a001 6401 a101  ...s....t...d...
+00000b00: 0100 7400 a001 6402 a101 0100 6400 5300  ..t...d.....d.S.
+00000b10: 2903 4e7a 2b66 6c75 7474 6572 2070 6163  ).Nz+flutter pac
+00000b20: 6b61 6765 7320 7075 6220 7275 6e20 6275  kages pub run bu
+00000b30: 696c 645f 7275 6e6e 6572 2063 6c65 616e  ild_runner clean
+00000b40: 7a48 666c 7574 7465 7220 7061 636b 6167  zHflutter packag
+00000b50: 6573 2070 7562 2072 756e 2062 7569 6c64  es pub run build
+00000b60: 5f72 756e 6e65 7220 6275 696c 6420 2d2d  _runner build --
+00000b70: 6465 6c65 7465 2d63 6f6e 666c 6963 7469  delete-conflicti
+00000b80: 6e67 2d6f 7574 7075 7473 2902 7230 0000  ng-outputs).r0..
+00000b90: 00da 0673 7973 7465 6d72 1500 0000 7217  ...systemr....r.
+00000ba0: 0000 0072 1700 0000 7218 0000 005a 0f5f  ...r....r....Z._
+00000bb0: 5f67 656e 6572 6174 6f72 4675 6e63 5300  _generatorFuncS.
+00000bc0: 0000 7308 0000 0000 010a 0104 0102 ff7a  ..s............z
+00000bd0: 1a41 6e6e 6f74 6174 696f 6e2e 5f5f 6765  .Annotation.__ge
+00000be0: 6e65 7261 746f 7246 756e 6329 02da 0e70  neratorFunc)...p
+00000bf0: 6163 6b61 6765 4c69 6250 6174 68da 0672  ackageLibPath..r
+00000c00: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
+00000c10: 0000 0500 0000 0400 0000 4300 0000 733e  ..........C...s>
+00000c20: 0000 0074 00a0 017c 01a1 0101 0074 0274  ...t...|.....t.t
+00000c30: 00a0 03a1 0064 0164 028d 027d 0264 017d  .....d.d...}.d.}
+00000c40: 037c 026a 0444 005d 147d 047c 046a 057c  .|.j.D.].}.|.j.|
+00000c50: 006a 066b 0272 2464 037d 0371 247c 0353  .j.k.r$d.}.q$|.S
+00000c60: 0029 044e 4629 015a 0d66 696c 7465 725f  .).NF).Z.filter_
+00000c70: 6279 5f74 6466 5429 0772 3000 0000 7231  by_tdfT).r0...r1
+00000c80: 0000 0072 0600 0000 da06 6765 7463 7764  ...r......getcwd
+00000c90: 7213 0000 0072 2e00 0000 720d 0000 0029  r....r....r....)
+00000ca0: 0572 1600 0000 7235 0000 005a 1170 6163  .r....r5...Z.pac
+00000cb0: 6b61 6765 4a73 6f6e 436f 6e66 6967 5a0e  kageJsonConfigZ.
+00000cc0: 6861 7342 7569 6c64 5275 6e6e 6572 7229  hasBuildRunnerr)
+00000cd0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000ce0: 0000 5a1c 5f5f 6a75 6467 6548 6173 4275  ..Z.__judgeHasBu
+00000cf0: 696c 6452 756e 6e65 7250 6163 6b61 6765  ildRunnerPackage
+00000d00: 5a00 0000 7312 0000 0000 010a 0102 0108  Z...s...........
+00000d10: ff06 0304 010a 010c 0106 027a 2741 6e6e  ...........z'Ann
+00000d20: 6f74 6174 696f 6e2e 5f5f 6a75 6467 6548  otation.__judgeH
+00000d30: 6173 4275 696c 6452 756e 6e65 7250 6163  asBuildRunnerPac
+00000d40: 6b61 6765 6301 0000 0000 0000 0000 0000  kagec...........
+00000d50: 0001 0000 0003 0000 0043 0000 0073 2200  .........C...s".
+00000d60: 0000 7c00 6a00 a001 a100 0100 7c00 6a02  ..|.j.......|.j.
+00000d70: a001 a100 0100 7403 a004 6401 a101 0100  ......t...d.....
+00000d80: 6400 5300 2902 4e75 0c00 0000 e695 b4e5  d.S.).Nu........
+00000d90: 9088 e5ae 8ce6 8890 2905 720e 0000 005a  ........).r....Z
+00000da0: 0f69 6e74 6567 7261 7465 5f73 6865 6c6c  .integrate_shell
+00000db0: 720f 0000 0072 0700 0000 720c 0000 0072  r....r....r....r
+00000dc0: 1500 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+00000dd0: 0000 005a 115f 5f69 6e74 6567 7261 7465  ...Z.__integrate
+00000de0: 5f73 6865 6c6c 6700 0000 7306 0000 0000  _shellg...s.....
+00000df0: 010a 010a 017a 1c41 6e6e 6f74 6174 696f  .....z.Annotatio
+00000e00: 6e2e 5f5f 696e 7465 6772 6174 655f 7368  n.__integrate_sh
+00000e10: 656c 6c63 0100 0000 0000 0000 0000 0000  ellc............
+00000e20: 0500 0000 0400 0000 4300 0000 7360 0000  ........C...s`..
+00000e30: 0074 0083 007d 0167 007d 0274 0183 006a  .t...}.g.}.t...j
+00000e40: 0244 005d 487d 037c 01a0 037c 03a1 017d  .D.]H}.|...|...}
+00000e50: 047c 046a 0474 056a 066b 0273 507c 046a  .|.j.t.j.k.sP|.j
+00000e60: 0474 056a 076b 0273 507c 046a 0474 056a  .t.j.k.sP|.j.t.j
+00000e70: 086b 0273 507c 046a 0474 056a 096b 0272  .k.sP|.j.t.j.k.r
+00000e80: 127c 02a0 0a7c 03a1 0101 0071 127c 0253  .|...|.....q.|.S
+00000e90: 0029 014e 290b 7204 0000 0072 0200 0000  .).N).r....r....
+00000ea0: da0e 6d6f 6475 6c65 4e61 6d65 4c69 7374  ..moduleNameList
+00000eb0: da08 6765 745f 6974 656d da04 7479 7065  ..get_item..type
+00000ec0: 7203 0000 00da 034c 6962 da03 4170 69da  r......Lib..Api.
+00000ed0: 064d 6f64 756c 65da 0650 6c75 6769 6eda  .Module..Plugin.
+00000ee0: 0661 7070 656e 6429 0572 1600 0000 5a1a  .append).r....Z.
+00000ef0: 5f41 6e6e 6f74 6174 696f 6e5f 5f6d 6f64  _Annotation__mod
+00000f00: 756c 655f 636f 6e66 6967 5a11 5f41 6e6e  ule_configZ._Ann
+00000f10: 6f74 6174 696f 6e5f 5f6c 6973 7472 2900  otation__listr).
+00000f20: 0000 5a0a 636f 6669 675f 6974 656d 7217  ..Z.cofig_itemr.
+00000f30: 0000 0072 1700 0000 7218 0000 005a 185f  ...r....r....Z._
+00000f40: 5f61 7069 5f62 7573 696e 6573 734d 6f64  _api_businessMod
+00000f50: 756c 654c 6973 746c 0000 0073 1c00 0000  uleListl...s....
+00000f60: 0001 0601 0401 0c01 0a02 0aff 0202 0afe  ................
+00000f70: 0203 0afd 0204 0afc 0206 0c01 7a23 416e  ............z#An
+00000f80: 6e6f 7461 7469 6f6e 2e5f 5f61 7069 5f62  notation.__api_b
+00000f90: 7573 696e 6573 734d 6f64 756c 654c 6973  usinessModuleLis
+00000fa0: 744e 290d da08 5f5f 6e61 6d65 5f5f da0a  tN)...__name__..
+00000fb0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000fc0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+00000fd0: 5f72 1900 0000 722c 0000 0072 1d00 0000  _r....r,...r....
+00000fe0: 7223 0000 0072 3200 0000 da04 626f 6f6c  r#...r2.....bool
+00000ff0: 722f 0000 0072 2200 0000 7210 0000 0072  r/...r"...r....r
+00001000: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+00001010: 0000 0072 0b00 0000 0b00 0000 7310 0000  ...r........s...
+00001020: 0008 0104 0408 0908 250e 1508 0710 0d08  ........%.......
+00001030: 0572 0b00 0000 2912 7230 0000 00da 2974  .r....).r0....)t
+00001040: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 636f  df_tool.tools.co
+00001050: 6e66 6967 2e69 6e69 7469 616c 5f6a 736f  nfig.initial_jso
+00001060: 6e5f 636f 6e66 6967 7202 0000 00da 2874  n_configr.....(t
+00001070: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 636f  df_tool.tools.co
+00001080: 6e66 6967 2e6d 6f64 756c 655f 6a73 6f6e  nfig.module_json
+00001090: 5f63 6f6e 6669 6772 0300 0000 7204 0000  _configr....r...
+000010a0: 005a 2574 6466 5f74 6f6f 6c2e 746f 6f6c  .Z%tdf_tool.tool
+000010b0: 732e 636f 6e66 6967 2e70 6163 6b61 6765  s.config.package
+000010c0: 735f 636f 6e66 6967 7205 0000 0072 0600  s_configr....r..
+000010d0: 0000 da14 7464 665f 746f 6f6c 2e74 6f6f  ....tdf_tool.too
+000010e0: 6c73 2e70 7269 6e74 7207 0000 00da 1874  ls.printr......t
+000010f0: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 7368  df_tool.tools.sh
+00001100: 656c 6c5f 6469 7272 0800 0000 5a19 7464  ell_dirr....Z.td
+00001110: 665f 746f 6f6c 2e70 6970 656c 696e 6573  f_tool.pipelines
+00001120: 2e72 6f75 7465 7272 0900 0000 5a22 7464  .routerr....Z"td
+00001130: 665f 746f 6f6c 2e70 6970 656c 696e 6573  f_tool.pipelines
+00001140: 2e61 7069 5f69 6e74 6572 6163 7469 6f6e  .api_interaction
+00001150: 720a 0000 0072 0b00 0000 7217 0000 0072  r....r....r....r
+00001160: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
+00001170: 3c6d 6f64 756c 653e 0100 0000 7310 0000  <module>....s...
+00001180: 0008 010c 0110 0110 010c 010c 020c 010c  ................
+00001190: 02                                       .
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 08:28:01 2024 UTC, .py size: 7421 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 91d9 2066 fd1c 0000  a......... f....
+00000000: 610d 0d0a 0000 0000 48e4 2066 dc1c 0000  a.......H. f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6406 6407 8400 6407 8302 5a0b  ..G.d.d...d...Z.
@@ -85,365 +85,364 @@
 00000540: 5300 291e da0d 4170 6941 6e6e 6f74 6174  S.)...ApiAnnotat
 00000550: 696f 6e75 4400 0000 0a20 2020 20e6 a8a1  ionuD....    ...
 00000560: e59d 97e9 97b4 e4ba a4e4 ba92 e694 afe6  ................
 00000570: 8c81 e79b b8e5 85b3 e591 bde4 bba4 efbc  ................
 00000580: 9a74 6c20 6170 6920 2d68 20e6 9fa5 e79c  .tl api -h .....
 00000590: 8be8 afa6 e683 850a 2020 2020 6301 0000  ........    c...
 000005a0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-000005b0: 0043 0000 0073 4400 0000 6400 7c00 5f00  .C...sD...d.|._.
+000005b0: 0043 0000 0073 3c00 0000 6400 7c00 5f00  .C...s<...d.|._.
 000005c0: 6401 7c00 5f01 6700 7c00 5f02 6402 7c00  d.|._.g.|._.d.|.
 000005d0: 5f03 6700 7c00 5f04 6403 7c00 5f05 6404  _.g.|._.d.|._.d.
-000005e0: 7c00 5f06 6700 7c00 5f07 7408 a009 a100  |._.g.|._.t.....
-000005f0: 0100 7c00 a00a a100 0100 6400 5300 2905  ..|.......d.S.).
-00000600: 4e7a 0e2e 7464 665f 696d 706c 2e64 6172  Nz..tdf_impl.dar
-00000610: 747a 0d2e 7464 665f 6170 692e 6461 7274  tz..tdf_api.dart
-00000620: 5a07 7464 665f 6170 69da 1374 6466 5f6d  Z.tdf_api..tdf_m
-00000630: 6f64 756c 655f 6170 695f 616e 6e6f 290b  odule_api_anno).
-00000640: da02 6666 da1a 5f41 7069 416e 6e6f 7461  ..ff.._ApiAnnota
-00000650: 7469 6f6e 5f5f 696d 706c 5375 6666 6978  tion__implSuffix
-00000660: da1c 5f41 7069 416e 6e6f 7461 7469 6f6e  .._ApiAnnotation
-00000670: 5f5f 696d 706c 4e6f 6465 4c69 7374 da19  __implNodeList..
-00000680: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
-00000690: 6170 6953 7566 6669 78da 1b5f 4170 6941  apiSuffix.._ApiA
-000006a0: 6e6e 6f74 6174 696f 6e5f 5f61 7069 4e6f  nnotation__apiNo
-000006b0: 6465 4c69 7374 da1e 5f41 7069 416e 6e6f  deList.._ApiAnno
-000006c0: 7461 7469 6f6e 5f5f 696e 7465 7261 6374  tation__interact
-000006d0: 696f 6e44 6972 5a1e 5f41 7069 416e 6e6f  ionDirZ._ApiAnno
-000006e0: 7461 7469 6f6e 5f5f 616e 6e6f 7461 7469  tation__annotati
-000006f0: 6f6e 4e61 6d65 da1c 5f41 7069 416e 6e6f  onName.._ApiAnno
-00000700: 7461 7469 6f6e 5f5f 7061 636b 6167 6573  tation__packages
-00000710: 4c69 7374 7206 0000 00da 0d64 6972 496e  Listr......dirIn
-00000720: 7661 6c69 6461 7465 da13 6665 7463 685f  validate..fetch_
-00000730: 7061 636b 6167 6573 5f6c 6973 7472 0e00  packages_listr..
-00000740: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000750: 0072 1200 0000 2200 0000 7314 0000 0000  .r...."...s.....
-00000760: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00000770: 0208 017a 1641 7069 416e 6e6f 7461 7469  ...z.ApiAnnotati
-00000780: 6f6e 2e5f 5f69 6e69 745f 5f63 0100 0000  on.__init__c....
-00000790: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000007a0: 4300 0000 731c 0000 0074 00a0 01a1 0001  C...s....t......
-000007b0: 0074 0274 03a0 04a1 0083 016a 057c 005f  .t.t.......j.|._
-000007c0: 0664 0053 0029 014e 2907 7206 0000 00da  .d.S.).N).r.....
-000007d0: 0c67 6f49 6e53 6865 6c6c 4469 7272 0300  .goInShellDirr..
-000007e0: 0000 da02 6f73 da06 6765 7463 7764 da08  ....os..getcwd..
-000007f0: 7061 636b 6167 6573 7225 0000 0072 0e00  packagesr%...r..
-00000800: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000810: 0072 2700 0000 3000 0000 7304 0000 0000  .r'...0...s.....
-00000820: 0108 027a 2141 7069 416e 6e6f 7461 7469  ...z!ApiAnnotati
-00000830: 6f6e 2e66 6574 6368 5f70 6163 6b61 6765  on.fetch_package
-00000840: 735f 6c69 7374 6301 0000 0000 0000 0000  s_listc.........
-00000850: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00000860: 5000 0000 7c00 a000 a100 7d01 7401 6a02  P...|.....}.t.j.
-00000870: a003 7c01 6401 a102 7d02 7404 7c02 6402  ..|.d...}.t.|.d.
-00000880: 8302 7c00 5f05 7c00 a006 a100 0100 7c00  ..|._.|.......|.
-00000890: a007 a100 0100 7c00 a008 a100 0100 7c00  ......|.......|.
-000008a0: 6a05 a009 a100 0100 7c00 a00a a100 0100  j.......|.......
-000008b0: 6400 5300 2903 4e7a 1161 7069 5f72 6567  d.S.).Nz.api_reg
-000008c0: 6973 7465 722e 6461 7274 7a02 772b 290b  ister.dartz.w+).
-000008d0: da13 6765 745f 696e 7465 7261 6374 696f  ..get_interactio
-000008e0: 6e5f 6469 7272 2900 0000 da04 7061 7468  n_dirr).....path
-000008f0: da04 6a6f 696e da04 6f70 656e 721f 0000  ..join..openr...
-00000900: 00da 275f 4170 6941 6e6e 6f74 6174 696f  ..'_ApiAnnotatio
-00000910: 6e5f 5f69 6e74 6567 7261 7465 5f74 6466  n__integrate_tdf
-00000920: 5f61 7069 5f66 696c 6573 da28 5f41 7069  _api_files.(_Api
-00000930: 416e 6e6f 7461 7469 6f6e 5f5f 696e 7465  Annotation__inte
-00000940: 6772 6174 655f 7464 665f 696d 706c 5f66  grate_tdf_impl_f
-00000950: 696c 6573 da26 5f41 7069 416e 6e6f 7461  iles.&_ApiAnnota
-00000960: 7469 6f6e 5f5f 6765 6e65 7261 7465 5f72  tion__generate_r
-00000970: 6567 6973 7465 725f 636f 6465 da05 636c  egister_code..cl
-00000980: 6f73 65da 0a5f 5f66 6f72 6d61 745f 5f29  ose..__format__)
-00000990: 0372 0f00 0000 5a0b 7464 665f 6170 695f  .r....Z.tdf_api_
-000009a0: 6469 725a 1261 7574 6f5f 7265 6769 7374  dirZ.auto_regist
-000009b0: 6572 5f66 696c 6572 1000 0000 7210 0000  er_filer....r...
-000009c0: 0072 1100 0000 da0f 696e 7465 6772 6174  .r......integrat
-000009d0: 655f 7368 656c 6c36 0000 0073 1000 0000  e_shell6...s....
-000009e0: 0002 0801 0e01 0c03 0803 0803 0802 0a03  ................
-000009f0: 7a1d 4170 6941 6e6e 6f74 6174 696f 6e2e  z.ApiAnnotation.
-00000a00: 696e 7465 6772 6174 655f 7368 656c 6c63  integrate_shellc
-00000a10: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000a20: 0700 0000 4300 0000 737c 0000 007c 006a  ....C...s|...|.j
-00000a30: 0044 005d 1c7d 017c 00a0 017c 006a 027c  .D.].}.|...|.j.|
-00000a40: 016a 037c 016a 047c 016a 03a1 0401 0071  .j.|.j.|.j.....q
-00000a50: 067c 006a 0544 005d 1c7d 017c 00a0 017c  .|.j.D.].}.|...|
-00000a60: 006a 027c 016a 037c 016a 047c 016a 03a1  .j.|.j.|.j.|.j..
-00000a70: 0401 0071 2a7c 00a0 067c 006a 0264 0164  ...q*|...|.j.d.d
-00000a80: 02a1 0301 0064 037d 027c 006a 02a0 077c  .....d.}.|.j...|
-00000a90: 02a0 087c 00a0 09a1 007c 00a0 0aa1 00a1  ...|.....|......
-00000aa0: 02a1 0101 0064 0053 0029 044e 721e 0000  .....d.S.).Nr...
-00000ab0: 007a 1874 6466 5f6d 6f64 756c 655f 6170  .z.tdf_module_ap
-00000ac0: 695f 616e 6e6f 2e64 6172 7475 8602 0000  i_anno.dartu....
-00000ad0: 0a0a 2020 2020 2020 2020 636c 6173 7320  ..        class 
-00000ae0: 5444 4641 7069 496d 706c 4175 746f 5265  TDFApiImplAutoRe
-00000af0: 6769 7374 6572 207b 7b0a 2020 2020 2020  gister {{.      
-00000b00: 2020 2020 7374 6174 6963 204c 6973 743c      static List<
-00000b10: 5479 7065 3e20 6170 6973 203d 205b 0a20  Type> apis = [. 
-00000b20: 2020 2020 2020 2020 2020 207b 307d 0a20             {0}. 
-00000b30: 2020 2020 2020 2020 205d 3b0a 2020 2020           ];.    
-00000b40: 2020 2020 2020 2f2f 20e7 a1ae e4bf 9de6        // .......
-00000b50: 8980 e69c 89e8 a2ab e5bc 95e7 94a8 e79a  ................
-00000b60: 8461 7069 e5ba 93e7 9a84 e5ae 9ee7 8eb0  .api............
-00000b70: e7b1 bbe9 83bd e5b7 b2e6 b3a8 e586 8c0a  ................
-00000b80: 2020 2020 2020 2020 2020 7374 6174 6963            static
-00000b90: 2076 6f69 6420 5f65 6e73 7572 6541 7069   void _ensureApi
-00000ba0: 496d 706c 5265 6769 7374 6572 2829 207b  ImplRegister() {
-00000bb0: 7b0a 2020 2020 2020 2020 2020 2020 6170  {.            ap
-00000bc0: 6973 2e66 6f72 4561 6368 2828 656c 656d  is.forEach((elem
-00000bd0: 656e 7429 207b 7b0a 2020 2020 2020 2020  ent) {{.        
-00000be0: 2020 2020 2020 6966 2028 2141 7069 5265        if (!ApiRe
-00000bf0: 6769 7374 6572 4365 6e74 6572 2e6b 6579  gisterCenter.key
-00000c00: 732e 636f 6e74 6169 6e73 2865 6c65 6d65  s.contains(eleme
-00000c10: 6e74 2929 207b 7b0a 2020 2020 2020 2020  nt)) {{.        
-00000c20: 2020 2020 2020 2020 7468 726f 7720 4578          throw Ex
-00000c30: 6365 7074 696f 6e28 2224 7b7b 656c 656d  ception("${{elem
-00000c40: 656e 747d 7de7 9a84 e5ae 9ee7 8eb0 e7b1  ent}}...........
-00000c50: bbe6 9caa e69c aae6 b3a8 e586 8cef bc81  ................
-00000c60: efbc 81ef bc81 e8af b7e5 88a0 e999 a4e5  ................
-00000c70: ba93 247b 7b65 6c65 6d65 6e74 7d7d e79a  ..${{element}}..
-00000c80: 84e5 bc95 e794 a8e6 8896 e880 85e5 bc95  ................
-00000c90: e585 a5e5 ae9e e78e b0e7 b1bb 2229 3b0a  ............");.
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 7d7d                }}
-00000cb0: 0a20 2020 2020 2020 2020 2020 207d 7d29  .            }})
-00000cc0: 3b0a 2020 2020 2020 2020 2020 7d7d 0a0a  ;.          }}..
-00000cd0: 2020 2020 2020 2020 2020 7374 6174 6963            static
-00000ce0: 2076 6f69 6420 6175 746f 5265 6769 7374   void autoRegist
-00000cf0: 6572 2829 207b 7b0a 2020 2020 2020 2020  er() {{.        
-00000d00: 2020 2020 2020 7b31 7d0a 2020 2020 2020        {1}.      
-00000d10: 2020 2020 2020 2020 5f65 6e73 7572 6541          _ensureA
-00000d20: 7069 496d 706c 5265 6769 7374 6572 2829  piImplRegister()
-00000d30: 3b0a 2020 2020 2020 2020 2020 7d7d 0a20  ;.          }}. 
-00000d40: 2020 2020 2020 207d 7d0a 2020 2020 2020         }}.      
-00000d50: 2020 2020 2020 290b 7221 0000 00da 255f        ).r!....%_
-00000d60: 4170 6941 6e6e 6f74 6174 696f 6e5f 5f5f  ApiAnnotation___
-00000d70: 5f69 6d70 6f72 745f 6461 7461 5f63 7265  _import_data_cre
-00000d80: 6174 6f72 721f 0000 0072 0b00 0000 720d  atorr....r....r.
-00000d90: 0000 0072 2300 0000 da31 5f41 7069 416e  ...r#....1_ApiAn
-00000da0: 6e6f 7461 7469 6f6e 5f5f 696d 706f 7274  notation__import
-00000db0: 5f64 6174 615f 6372 6561 746f 725f 7769  _data_creator_wi
-00000dc0: 7468 6f75 745f 616c 6961 73da 0577 7269  thout_alias..wri
-00000dd0: 7465 da06 666f 726d 6174 da10 6170 695f  te..format..api_
-00000de0: 6c69 7374 5f63 7265 6174 6f72 da25 5f41  list_creator.%_A
-00000df0: 7069 416e 6e6f 7461 7469 6f6e 5f5f 7265  piAnnotation__re
-00000e00: 6769 7374 6572 5f6c 6973 745f 6372 6561  gister_list_crea
-00000e10: 746f 7229 0372 0f00 0000 5a05 5f69 7465  tor).r....Z._ite
-00000e20: 6dda 0763 6f6e 7465 6e74 7210 0000 0072  m..contentr....r
-00000e30: 1000 0000 7211 0000 005a 185f 5f67 656e  ....r....Z.__gen
-00000e40: 6572 6174 655f 7265 6769 7374 6572 5f63  erate_register_c
-00000e50: 6f64 654a 0000 0073 1400 0000 0001 0a01  odeJ...s........
-00000e60: 1a01 0a01 1a02 1002 0415 0a01 0601 06fe  ................
-00000e70: 7a26 4170 6941 6e6e 6f74 6174 696f 6e2e  z&ApiAnnotation.
-00000e80: 5f5f 6765 6e65 7261 7465 5f72 6567 6973  __generate_regis
-00000e90: 7465 725f 636f 6465 6301 0000 0000 0000  ter_codec.......
-00000ea0: 0000 0000 0003 0000 0006 0000 0043 0000  .............C..
-00000eb0: 0073 2800 0000 6401 7d01 7c00 6a00 4400  .s(...d.}.|.j.D.
-00000ec0: 5d18 7d02 7c01 6402 a001 7c02 6a02 7c02  ].}.|.d...|.j.|.
-00000ed0: 6a02 a102 3700 7d01 710a 7c01 5300 2903  j...7.}.q.|.S.).
-00000ee0: 4e72 0900 0000 7a69 0a20 2020 2020 2020  Nr....zi.       
-00000ef0: 2020 2020 2041 7069 5265 6769 7374 6572       ApiRegister
-00000f00: 4365 6e74 6572 2e72 6567 6973 7465 7228  Center.register(
-00000f10: 7b30 7d2e 4175 746f 5265 6769 7374 6572  {0}.AutoRegister
-00000f20: 2e61 7069 5479 7065 2c7b 317d 2e41 7574  .apiType,{1}.Aut
-00000f30: 6f52 6567 6973 7465 722e 7072 6f76 6964  oRegister.provid
-00000f40: 6572 293b 0a20 2020 2020 2020 2020 2020  er);.           
-00000f50: 2029 0372 2100 0000 7239 0000 0072 0b00   ).r!...r9...r..
-00000f60: 0000 a903 720f 0000 0072 3c00 0000 da04  ....r....r<.....
-00000f70: 6974 656d 7210 0000 0072 1000 0000 7211  itemr....r....r.
-00000f80: 0000 005a 175f 5f72 6567 6973 7465 725f  ...Z.__register_
-00000f90: 6c69 7374 5f63 7265 6174 6f72 6b00 0000  list_creatork...
-00000fa0: 730c 0000 0000 0104 010a 0106 0208 fe08  s...............
-00000fb0: 037a 2541 7069 416e 6e6f 7461 7469 6f6e  .z%ApiAnnotation
-00000fc0: 2e5f 5f72 6567 6973 7465 725f 6c69 7374  .__register_list
-00000fd0: 5f63 7265 6174 6f72 6301 0000 0000 0000  _creatorc.......
-00000fe0: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-00000ff0: 0073 2400 0000 6401 7d01 7c00 6a00 4400  .s$...d.}.|.j.D.
-00001000: 5d14 7d02 7c01 6402 a001 7c02 6a02 a101  ].}.|.d...|.j...
-00001010: 3700 7d01 710a 7c01 5300 2903 4e72 0900  7.}.q.|.S.).Nr..
-00001020: 0000 7a43 0a20 2020 2020 2020 2020 2020  ..zC.           
-00001030: 207b 307d 2e54 4446 4170 6941 7574 6f49   {0}.TDFApiAutoI
-00001040: 6e76 616c 6964 6174 652e 6170 6954 7970  nvalidate.apiTyp
-00001050: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001060: 2020 2020 2020 2029 0372 2300 0000 7239         ).r#...r9
-00001070: 0000 0072 0b00 0000 723d 0000 0072 1000  ...r....r=...r..
-00001080: 0000 7210 0000 0072 1100 0000 723a 0000  ..r....r....r:..
-00001090: 0073 0000 0073 0c00 0000 0001 0401 0a01  .s...s..........
-000010a0: 0602 04fe 0803 7a1e 4170 6941 6e6e 6f74  ......z.ApiAnnot
-000010b0: 6174 696f 6e2e 6170 695f 6c69 7374 5f63  ation.api_list_c
-000010c0: 7265 6174 6f72 6301 0000 0000 0000 0000  reatorc.........
-000010d0: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
-000010e0: 6200 0000 7400 a001 6401 a101 0100 7c00  b...t...d.....|.
-000010f0: 6a02 4400 5d4c 7d01 7c00 a003 7c01 6a04  j.D.]L}.|...|.j.
-00001100: 7c00 6a05 a102 7d02 7c02 6400 7501 7210  |.j...}.|.d.u.r.
-00001110: 7406 8300 7d03 7c01 6a04 7c03 5f04 7c01  t...}.|.j.|._.|.
-00001120: 6a07 7c03 5f07 7c02 7c03 5f08 7c03 a009  j.|._.|.|._.|...
-00001130: a100 0100 7c00 6a0a a00b 7c03 a101 0100  ....|.j...|.....
-00001140: 7110 6400 5300 2902 4e75 1c00 0000 e695  q.d.S.).Nu......
-00001150: b4e5 9088 e689 80e6 9c89 e4ba a4e4 ba92  ................
-00001160: 696d 706c e696 87e4 bbb6 290c 7205 0000  impl......).r...
-00001170: 00da 0574 6974 6c65 7225 0000 00da 1f5f  ...titler%....._
-00001180: 4170 6941 6e6e 6f74 6174 696f 6e5f 5f67  ApiAnnotation__g
-00001190: 6574 5f74 6172 6765 745f 6669 6c65 720c  et_target_filer.
-000011a0: 0000 0072 2000 0000 7207 0000 0072 0b00  ...r ...r....r..
-000011b0: 0000 720d 0000 0072 1700 0000 7221 0000  ..r....r....r!..
-000011c0: 00da 0661 7070 656e 6429 0472 0f00 0000  ...append).r....
-000011d0: da0b 7061 636b 6167 6549 7465 6dda 195f  ..packageItem.._
-000011e0: 4170 6941 6e6e 6f74 6174 696f 6e5f 5f66  ApiAnnotation__f
-000011f0: 696c 655f 7061 7468 5a09 5f69 6d70 6c4e  ile_pathZ._implN
-00001200: 6f64 6572 1000 0000 7210 0000 0072 1100  oder....r....r..
-00001210: 0000 5a1a 5f5f 696e 7465 6772 6174 655f  ..Z.__integrate_
-00001220: 7464 665f 696d 706c 5f66 696c 6573 7b00  tdf_impl_files{.
-00001230: 0000 7314 0000 0000 010a 010a 0110 0108  ..s.............
-00001240: 0106 0108 0108 0106 0108 017a 2841 7069  ...........z(Api
-00001250: 416e 6e6f 7461 7469 6f6e 2e5f 5f69 6e74  Annotation.__int
-00001260: 6567 7261 7465 5f74 6466 5f69 6d70 6c5f  egrate_tdf_impl_
-00001270: 6669 6c65 7363 0100 0000 0000 0000 0000  filesc..........
-00001280: 0000 0400 0000 0500 0000 4300 0000 7362  ..........C...sb
-00001290: 0000 0074 00a0 0164 01a1 0101 007c 006a  ...t...d.....|.j
-000012a0: 0244 005d 4c7d 017c 00a0 037c 016a 047c  .D.]L}.|...|.j.|
-000012b0: 006a 05a1 027d 027c 0264 0075 0172 1074  .j...}.|.d.u.r.t
-000012c0: 0683 007d 037c 016a 047c 035f 047c 016a  ...}.|.j.|._.|.j
-000012d0: 077c 035f 077c 027c 035f 087c 03a0 09a1  .|._.|.|._.|....
-000012e0: 0001 007c 006a 0aa0 0b7c 03a1 0101 0071  ...|.j...|.....q
-000012f0: 1064 0053 0029 024e 751b 0000 00e6 95b4  .d.S.).Nu.......
-00001300: e590 88e6 8980 e69c 89e4 baa4 e4ba 9261  ...............a
-00001310: 7069 e696 87e4 bbb6 290c 7205 0000 0072  pi......).r....r
-00001320: 3f00 0000 7225 0000 0072 4000 0000 720c  ?...r%...r@...r.
-00001330: 0000 0072 2200 0000 721c 0000 0072 0b00  ...r"...r....r..
-00001340: 0000 720d 0000 0072 1700 0000 7223 0000  ..r....r....r#..
-00001350: 0072 4100 0000 2904 720f 0000 0072 4200  .rA...).r....rB.
-00001360: 0000 7243 0000 005a 085f 6170 694e 6f64  ..rC...Z._apiNod
-00001370: 6572 1000 0000 7210 0000 0072 1100 0000  er....r....r....
-00001380: 5a19 5f5f 696e 7465 6772 6174 655f 7464  Z.__integrate_td
-00001390: 665f 6170 695f 6669 6c65 7387 0000 0073  f_api_files....s
-000013a0: 1400 0000 0001 0a01 0a01 1001 0801 0601  ................
-000013b0: 0801 0801 0601 0801 7a27 4170 6941 6e6e  ........z'ApiAnn
-000013c0: 6f74 6174 696f 6e2e 5f5f 696e 7465 6772  otation.__integr
-000013d0: 6174 655f 7464 665f 6170 695f 6669 6c65  ate_tdf_api_file
-000013e0: 7329 03da 0966 696c 655f 7061 7468 da06  s)...file_path..
-000013f0: 7375 6666 6978 da06 7265 7475 726e 6303  suffix..returnc.
-00001400: 0000 0000 0000 0000 0000 000c 0000 0006  ................
-00001410: 0000 0043 0000 0073 ce00 0000 7400 a001  ...C...s....t...
-00001420: a100 0100 7402 a003 7c01 a101 0100 6401  ....t...|.....d.
-00001430: 7d03 7402 a004 7405 a006 a100 a101 a007  }.t...t.........
-00001440: a100 a008 6402 a101 6401 1900 7d04 7402  ....d...d...}.t.
-00001450: a009 7c04 a101 4400 5d66 5c03 7d05 7d06  ..|...D.]f\.}.}.
-00001460: 7d07 7c07 4400 5d56 7d08 7402 6a0a a00b  }.|.D.]V}.t.j...
-00001470: 7c05 7c08 a102 7d09 7c09 a00c 7c02 a101  |.|...}.|...|...
-00001480: 724a 7c03 6403 3700 7d03 7405 a00d a100  rJ|.d.7.}.t.....
-00001490: 7292 7c09 a008 6404 a101 6403 1900 7d0a  r.|...d...d...}.
-000014a0: 7c0a a00e 6405 6406 a102 7d0b 714a 7c09  |...d.d...}.qJ|.
-000014b0: a008 6407 a101 6403 1900 7d0b 714a 713c  ..d...d...}.qJq<
-000014c0: 7c03 6403 6b02 72b0 7c0b 5300 7c03 6403  |.d.k.r.|.S.|.d.
-000014d0: 6b04 72ca 740f 6408 a010 7c01 a101 8301  k.r.t.d...|.....
-000014e0: 8201 6400 5300 6400 5300 2909 4e72 0100  ..d.S.d.S.).Nr..
-000014f0: 0000 da01 0ae9 0100 0000 7a05 5c6c 6962  ..........z.\lib
-00001500: 5cfa 015c 7214 0000 007a 052f 6c69 622f  \..\r....z./lib/
-00001510: 7530 0000 00e6 a8a1 e59d 977b 307d e5ad  u0.........{0}..
-00001520: 98e5 9ca8 e5a4 9ae4 b8aa e4ba a4e4 ba92  ................
-00001530: e696 87e4 bbb6 efbc 8ce8 afb7 e6a3 80e6  ................
-00001540: 9fa5 e29d 8c29 1172 0600 0000 7228 0000  .....).r....r(..
-00001550: 0072 2900 0000 da05 6368 6469 72da 0570  .r).....chdir..p
-00001560: 6f70 656e 7204 0000 00da 0770 7764 5f63  openr......pwd_c
-00001570: 6d64 da04 7265 6164 da05 7370 6c69 74da  md..read..split.
-00001580: 0477 616c 6b72 2d00 0000 722e 0000 00da  .walkr-...r.....
-00001590: 0865 6e64 7377 6974 68da 0a69 735f 7769  .endswith..is_wi
-000015a0: 6e64 6f77 73da 0772 6570 6c61 6365 da09  ndows..replace..
-000015b0: 4578 6365 7074 696f 6e72 3900 0000 290c  Exceptionr9...).
-000015c0: 720f 0000 0072 4400 0000 7245 0000 00da  r....rD...rE....
-000015d0: 0563 6f75 6e74 da08 6e6f 7761 5061 7468  .count..nowaPath
-000015e0: da04 726f 6f74 da04 6469 7273 da05 6669  ..root..dirs..fi
-000015f0: 6c65 73da 0466 696c 65da 0873 7263 5f66  les..file..src_f
-00001600: 696c 65da 0474 656d 705a 1b5f 4170 6941  ile..tempZ._ApiA
-00001610: 6e6e 6f74 6174 696f 6e5f 5f74 6172 6765  nnotation__targe
-00001620: 745f 6669 6c65 7210 0000 0072 1000 0000  t_filer....r....
-00001630: 7211 0000 005a 115f 5f67 6574 5f74 6172  r....Z.__get_tar
-00001640: 6765 745f 6669 6c65 9400 0000 7326 0000  get_file....s&..
-00001650: 0000 0108 010a 0204 021c 0114 0108 010e  ................
-00001660: 010a 0108 0108 010e 010e 0212 0108 0104  ................
-00001670: 0108 010e 0104 017a 1f41 7069 416e 6e6f  .......z.ApiAnno
-00001680: 7461 7469 6f6e 2e5f 5f67 6574 5f74 6172  tation.__get_tar
-00001690: 6765 745f 6669 6c65 6301 0000 0000 0000  get_filec.......
-000016a0: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
-000016b0: 0073 4e00 0000 7400 a001 a100 0100 7402  .sN...t.......t.
-000016c0: a003 6401 a101 0100 7402 6a04 a005 7c00  ..d.....t.j...|.
-000016d0: 6a06 a101 722c 7407 a008 7c00 6a06 a101  j...r,t...|.j...
-000016e0: 0100 7402 a009 7c00 6a06 a101 0100 7402  ..t...|.j.....t.
-000016f0: 6a04 a00a 7400 a00b a100 6401 7c00 6a06  j...t.....d.|.j.
-00001700: a103 5300 2902 4eda 036c 6962 290c 7206  ..S.).N..lib).r.
-00001710: 0000 0072 2800 0000 7229 0000 0072 4a00  ...r(...r)...rJ.
-00001720: 0000 722d 0000 00da 0665 7869 7374 7372  ..r-.....existsr
-00001730: 2400 0000 da06 7368 7574 696c da06 726d  $.....shutil..rm
-00001740: 7472 6565 da05 6d6b 6469 7272 2e00 0000  tree..mkdirr....
-00001750: da0b 6765 7453 6865 6c6c 4469 7272 0e00  ..getShellDirr..
-00001760: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00001770: 0072 2c00 0000 ac00 0000 730c 0000 0000  .r,.......s.....
-00001780: 0108 010a 010e 010c 010c 017a 2141 7069  ...........z!Api
-00001790: 416e 6e6f 7461 7469 6f6e 2e67 6574 5f69  Annotation.get_i
-000017a0: 6e74 6572 6163 7469 6f6e 5f64 6972 6301  nteraction_dirc.
-000017b0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-000017c0: 0000 0043 0000 0073 3200 0000 7400 a001  ...C...s2...t...
-000017d0: a100 0100 7402 6a03 a004 7400 a005 a100  ....t.j...t.....
-000017e0: 6401 7c00 6a06 a103 7d01 7402 a007 6402  d.|.j...}.t...d.
-000017f0: a008 7c01 a101 a101 0100 6400 5300 2903  ..|.......d.S.).
-00001800: 4e72 5c00 0000 7a0f 6461 7274 2066 6f72  Nr\...z.dart for
-00001810: 6d61 7420 7b30 7d29 0972 0600 0000 da0f  mat {0}).r......
-00001820: 676f 496e 5368 656c 6c4c 6962 4469 7272  goInShellLibDirr
-00001830: 2900 0000 722d 0000 0072 2e00 0000 7261  )...r-...r....ra
-00001840: 0000 0072 2400 0000 da06 7379 7374 656d  ...r$.....system
-00001850: 7239 0000 0029 0272 0f00 0000 5a14 5f41  r9...).r....Z._A
-00001860: 7069 416e 6e6f 7461 7469 6f6e 5f5f 7061  piAnnotation__pa
-00001870: 7468 7210 0000 0072 1000 0000 7211 0000  thr....r....r...
-00001880: 0072 3400 0000 b500 0000 7306 0000 0000  .r4.......s.....
-00001890: 0108 0116 017a 1841 7069 416e 6e6f 7461  .....z.ApiAnnota
-000018a0: 7469 6f6e 2e5f 5f66 6f72 6d61 745f 5f63  tion.__format__c
-000018b0: 0500 0000 0000 0000 0000 0000 0500 0000  ................
-000018c0: 0700 0000 4300 0000 7318 0000 007c 01a0  ....C...s....|..
-000018d0: 0064 01a0 017c 027c 037c 04a1 03a1 0101  .d...|.|.|......
-000018e0: 0064 0053 0029 024e 7a21 696d 706f 7274  .d.S.).Nz!import
-000018f0: 2022 7061 636b 6167 653a 7b30 7d2f 7b31   "package:{0}/{1
-00001900: 7d22 2061 7320 7b32 7d3b 0aa9 0272 3800  }" as {2};...r8.
-00001910: 0000 7239 0000 0029 0572 0f00 0000 da07  ..r9...).r......
-00001920: 665f 7772 6974 65da 0b6d 6f64 756c 655f  f_write..module_
-00001930: 6e61 6d65 7244 0000 00da 0561 6c69 6173  namerD.....alias
-00001940: 7210 0000 0072 1000 0000 7211 0000 005a  r....r....r....Z
-00001950: 175f 5f5f 5f69 6d70 6f72 745f 6461 7461  .____import_data
-00001960: 5f63 7265 6174 6f72 bb00 0000 730a 0000  _creator....s...
-00001970: 0000 0304 0104 0106 ff02 ff7a 2541 7069  ...........z%Api
-00001980: 416e 6e6f 7461 7469 6f6e 2e5f 5f5f 5f69  Annotation.____i
-00001990: 6d70 6f72 745f 6461 7461 5f63 7265 6174  mport_data_creat
-000019a0: 6f72 6304 0000 0000 0000 0000 0000 0004  orc.............
-000019b0: 0000 0006 0000 0043 0000 0073 1600 0000  .......C...s....
-000019c0: 7c01 a000 6401 a001 7c02 7c03 a102 a101  |...d...|.|.....
-000019d0: 0100 6400 5300 2902 4e7a 1a69 6d70 6f72  ..d.S.).Nz.impor
-000019e0: 7420 2270 6163 6b61 6765 3a7b 307d 2f7b  t "package:{0}/{
-000019f0: 317d 223b 0a72 6400 0000 2904 720f 0000  1}";.rd...).r...
-00001a00: 0072 6500 0000 7266 0000 0072 4400 0000  .re...rf...rD...
-00001a10: 7210 0000 0072 1000 0000 7211 0000 005a  r....r....r....Z
-00001a20: 235f 5f69 6d70 6f72 745f 6461 7461 5f63  #__import_data_c
-00001a30: 7265 6174 6f72 5f77 6974 686f 7574 5f61  reator_without_a
-00001a40: 6c69 6173 c500 0000 730a 0000 0000 0304  lias....s.......
-00001a50: 0104 0104 ff02 ff7a 3141 7069 416e 6e6f  .......z1ApiAnno
-00001a60: 7461 7469 6f6e 2e5f 5f69 6d70 6f72 745f  tation.__import_
-00001a70: 6461 7461 5f63 7265 6174 6f72 5f77 6974  data_creator_wit
-00001a80: 686f 7574 5f61 6c69 6173 4e29 1272 1900  hout_aliasN).r..
-00001a90: 0000 721a 0000 0072 1b00 0000 da07 5f5f  ..r....r......__
-00001aa0: 646f 635f 5f72 1200 0000 7227 0000 0072  doc__r....r'...r
-00001ab0: 3500 0000 7232 0000 0072 3b00 0000 723a  5...r2...r;...r:
-00001ac0: 0000 0072 3100 0000 7230 0000 00da 0373  ...r1...r0.....s
-00001ad0: 7472 7240 0000 0072 2c00 0000 7234 0000  trr@...r,...r4..
-00001ae0: 0072 3600 0000 7237 0000 0072 1000 0000  .r6...r7...r....
-00001af0: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00001b00: 1d00 0000 1d00 0000 731c 0000 0008 0104  ........s.......
-00001b10: 0408 0e08 0608 1408 2108 0808 0808 0c08  ........!.......
-00001b20: 0d12 1808 0908 0608 0a72 1d00 0000 290e  .........r....).
-00001b30: 7229 0000 0072 5e00 0000 da25 7464 665f  r)...r^....%tdf_
-00001b40: 746f 6f6c 2e74 6f6f 6c73 2e63 6f6e 6669  tool.tools.confi
-00001b50: 672e 7061 636b 6167 6573 5f63 6f6e 6669  g.packages_confi
-00001b60: 6772 0200 0000 7203 0000 00da 1d74 6466  gr....r......tdf
-00001b70: 5f74 6f6f 6c2e 746f 6f6c 732e 706c 6174  _tool.tools.plat
-00001b80: 666f 726d 5f74 6f6f 6c73 7204 0000 00da  form_toolsr.....
-00001b90: 1474 6466 5f74 6f6f 6c2e 746f 6f6c 732e  .tdf_tool.tools.
-00001ba0: 7072 696e 7472 0500 0000 da18 7464 665f  printr......tdf_
-00001bb0: 746f 6f6c 2e74 6f6f 6c73 2e73 6865 6c6c  tool.tools.shell
-00001bc0: 5f64 6972 7206 0000 0072 0700 0000 721c  _dirr....r....r.
-00001bd0: 0000 0072 1d00 0000 7210 0000 0072 1000  ...r....r....r..
-00001be0: 0000 7210 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
-00001bf0: 6f64 756c 653e 0100 0000 7310 0000 0008  odule>....s.....
-00001c00: 0108 0110 010c 010c 010c 030e 0a0e 0a    ...............
+000005e0: 7c00 5f06 6700 7c00 5f07 7c00 a008 a100  |._.g.|._.|.....
+000005f0: 0100 6400 5300 2905 4e7a 0e2e 7464 665f  ..d.S.).Nz..tdf_
+00000600: 696d 706c 2e64 6172 747a 0d2e 7464 665f  impl.dartz..tdf_
+00000610: 6170 692e 6461 7274 5a07 7464 665f 6170  api.dartZ.tdf_ap
+00000620: 69da 1374 6466 5f6d 6f64 756c 655f 6170  i..tdf_module_ap
+00000630: 695f 616e 6e6f 2909 da02 6666 da1a 5f41  i_anno)...ff.._A
+00000640: 7069 416e 6e6f 7461 7469 6f6e 5f5f 696d  piAnnotation__im
+00000650: 706c 5375 6666 6978 da1c 5f41 7069 416e  plSuffix.._ApiAn
+00000660: 6e6f 7461 7469 6f6e 5f5f 696d 706c 4e6f  notation__implNo
+00000670: 6465 4c69 7374 da19 5f41 7069 416e 6e6f  deList.._ApiAnno
+00000680: 7461 7469 6f6e 5f5f 6170 6953 7566 6669  tation__apiSuffi
+00000690: 78da 1b5f 4170 6941 6e6e 6f74 6174 696f  x.._ApiAnnotatio
+000006a0: 6e5f 5f61 7069 4e6f 6465 4c69 7374 da1e  n__apiNodeList..
+000006b0: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
+000006c0: 696e 7465 7261 6374 696f 6e44 6972 5a1e  interactionDirZ.
+000006d0: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
+000006e0: 616e 6e6f 7461 7469 6f6e 4e61 6d65 da1c  annotationName..
+000006f0: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
+00000700: 7061 636b 6167 6573 4c69 7374 da13 6665  packagesList..fe
+00000710: 7463 685f 7061 636b 6167 6573 5f6c 6973  tch_packages_lis
+00000720: 7472 0e00 0000 7210 0000 0072 1000 0000  tr....r....r....
+00000730: 7211 0000 0072 1200 0000 2200 0000 7312  r....r...."...s.
+00000740: 0000 0000 0106 0106 0106 0106 0106 0106  ................
+00000750: 0106 0106 027a 1641 7069 416e 6e6f 7461  .....z.ApiAnnota
+00000760: 7469 6f6e 2e5f 5f69 6e69 745f 5f63 0100  tion.__init__c..
+00000770: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000780: 0000 4300 0000 731c 0000 0074 00a0 01a1  ..C...s....t....
+00000790: 0001 0074 0274 03a0 04a1 0083 016a 057c  ...t.t.......j.|
+000007a0: 005f 0664 0053 0029 014e 2907 7206 0000  ._.d.S.).N).r...
+000007b0: 00da 0c67 6f49 6e53 6865 6c6c 4469 7272  ...goInShellDirr
+000007c0: 0300 0000 da02 6f73 da06 6765 7463 7764  ......os..getcwd
+000007d0: da08 7061 636b 6167 6573 7225 0000 0072  ..packagesr%...r
+000007e0: 0e00 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
+000007f0: 0000 0072 2600 0000 2f00 0000 7304 0000  ...r&.../...s...
+00000800: 0000 0108 027a 2141 7069 416e 6e6f 7461  .....z!ApiAnnota
+00000810: 7469 6f6e 2e66 6574 6368 5f70 6163 6b61  tion.fetch_packa
+00000820: 6765 735f 6c69 7374 6301 0000 0000 0000  ges_listc.......
+00000830: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000840: 0073 5000 0000 7c00 a000 a100 7d01 7401  .sP...|.....}.t.
+00000850: 6a02 a003 7c01 6401 a102 7d02 7404 7c02  j...|.d...}.t.|.
+00000860: 6402 8302 7c00 5f05 7c00 a006 a100 0100  d...|._.|.......
+00000870: 7c00 a007 a100 0100 7c00 a008 a100 0100  |.......|.......
+00000880: 7c00 6a05 a009 a100 0100 7c00 a00a a100  |.j.......|.....
+00000890: 0100 6400 5300 2903 4e7a 1161 7069 5f72  ..d.S.).Nz.api_r
+000008a0: 6567 6973 7465 722e 6461 7274 7a02 772b  egister.dartz.w+
+000008b0: 290b da13 6765 745f 696e 7465 7261 6374  )...get_interact
+000008c0: 696f 6e5f 6469 7272 2800 0000 da04 7061  ion_dirr(.....pa
+000008d0: 7468 da04 6a6f 696e da04 6f70 656e 721f  th..join..openr.
+000008e0: 0000 00da 275f 4170 6941 6e6e 6f74 6174  ....'_ApiAnnotat
+000008f0: 696f 6e5f 5f69 6e74 6567 7261 7465 5f74  ion__integrate_t
+00000900: 6466 5f61 7069 5f66 696c 6573 da28 5f41  df_api_files.(_A
+00000910: 7069 416e 6e6f 7461 7469 6f6e 5f5f 696e  piAnnotation__in
+00000920: 7465 6772 6174 655f 7464 665f 696d 706c  tegrate_tdf_impl
+00000930: 5f66 696c 6573 da26 5f41 7069 416e 6e6f  _files.&_ApiAnno
+00000940: 7461 7469 6f6e 5f5f 6765 6e65 7261 7465  tation__generate
+00000950: 5f72 6567 6973 7465 725f 636f 6465 da05  _register_code..
+00000960: 636c 6f73 65da 0a5f 5f66 6f72 6d61 745f  close..__format_
+00000970: 5f29 0372 0f00 0000 5a0b 7464 665f 6170  _).r....Z.tdf_ap
+00000980: 695f 6469 725a 1261 7574 6f5f 7265 6769  i_dirZ.auto_regi
+00000990: 7374 6572 5f66 696c 6572 1000 0000 7210  ster_filer....r.
+000009a0: 0000 0072 1100 0000 da0f 696e 7465 6772  ...r......integr
+000009b0: 6174 655f 7368 656c 6c35 0000 0073 1000  ate_shell5...s..
+000009c0: 0000 0002 0801 0e01 0c03 0803 0803 0802  ................
+000009d0: 0a03 7a1d 4170 6941 6e6e 6f74 6174 696f  ..z.ApiAnnotatio
+000009e0: 6e2e 696e 7465 6772 6174 655f 7368 656c  n.integrate_shel
+000009f0: 6c63 0100 0000 0000 0000 0000 0000 0300  lc..............
+00000a00: 0000 0700 0000 4300 0000 737c 0000 007c  ......C...s|...|
+00000a10: 006a 0044 005d 1c7d 017c 00a0 017c 006a  .j.D.].}.|...|.j
+00000a20: 027c 016a 037c 016a 047c 016a 03a1 0401  .|.j.|.j.|.j....
+00000a30: 0071 067c 006a 0544 005d 1c7d 017c 00a0  .q.|.j.D.].}.|..
+00000a40: 017c 006a 027c 016a 037c 016a 047c 016a  .|.j.|.j.|.j.|.j
+00000a50: 03a1 0401 0071 2a7c 00a0 067c 006a 0264  .....q*|...|.j.d
+00000a60: 0164 02a1 0301 0064 037d 027c 006a 02a0  .d.....d.}.|.j..
+00000a70: 077c 02a0 087c 00a0 09a1 007c 00a0 0aa1  .|...|.....|....
+00000a80: 00a1 02a1 0101 0064 0053 0029 044e 721e  .......d.S.).Nr.
+00000a90: 0000 007a 1874 6466 5f6d 6f64 756c 655f  ...z.tdf_module_
+00000aa0: 6170 695f 616e 6e6f 2e64 6172 7475 8602  api_anno.dartu..
+00000ab0: 0000 0a0a 2020 2020 2020 2020 636c 6173  ....        clas
+00000ac0: 7320 5444 4641 7069 496d 706c 4175 746f  s TDFApiImplAuto
+00000ad0: 5265 6769 7374 6572 207b 7b0a 2020 2020  Register {{.    
+00000ae0: 2020 2020 2020 7374 6174 6963 204c 6973        static Lis
+00000af0: 743c 5479 7065 3e20 6170 6973 203d 205b  t<Type> apis = [
+00000b00: 0a20 2020 2020 2020 2020 2020 207b 307d  .            {0}
+00000b10: 0a20 2020 2020 2020 2020 205d 3b0a 2020  .          ];.  
+00000b20: 2020 2020 2020 2020 2f2f 20e7 a1ae e4bf          // .....
+00000b30: 9de6 8980 e69c 89e8 a2ab e5bc 95e7 94a8  ................
+00000b40: e79a 8461 7069 e5ba 93e7 9a84 e5ae 9ee7  ...api..........
+00000b50: 8eb0 e7b1 bbe9 83bd e5b7 b2e6 b3a8 e586  ................
+00000b60: 8c0a 2020 2020 2020 2020 2020 7374 6174  ..          stat
+00000b70: 6963 2076 6f69 6420 5f65 6e73 7572 6541  ic void _ensureA
+00000b80: 7069 496d 706c 5265 6769 7374 6572 2829  piImplRegister()
+00000b90: 207b 7b0a 2020 2020 2020 2020 2020 2020   {{.            
+00000ba0: 6170 6973 2e66 6f72 4561 6368 2828 656c  apis.forEach((el
+00000bb0: 656d 656e 7429 207b 7b0a 2020 2020 2020  ement) {{.      
+00000bc0: 2020 2020 2020 2020 6966 2028 2141 7069          if (!Api
+00000bd0: 5265 6769 7374 6572 4365 6e74 6572 2e6b  RegisterCenter.k
+00000be0: 6579 732e 636f 6e74 6169 6e73 2865 6c65  eys.contains(ele
+00000bf0: 6d65 6e74 2929 207b 7b0a 2020 2020 2020  ment)) {{.      
+00000c00: 2020 2020 2020 2020 2020 7468 726f 7720            throw 
+00000c10: 4578 6365 7074 696f 6e28 2224 7b7b 656c  Exception("${{el
+00000c20: 656d 656e 747d 7de7 9a84 e5ae 9ee7 8eb0  ement}}.........
+00000c30: e7b1 bbe6 9caa e69c aae6 b3a8 e586 8cef  ................
+00000c40: bc81 efbc 81ef bc81 e8af b7e5 88a0 e999  ................
+00000c50: a4e5 ba93 247b 7b65 6c65 6d65 6e74 7d7d  ....${{element}}
+00000c60: e79a 84e5 bc95 e794 a8e6 8896 e880 85e5  ................
+00000c70: bc95 e585 a5e5 ae9e e78e b0e7 b1bb 2229  ..............")
+00000c80: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00000c90: 7d7d 0a20 2020 2020 2020 2020 2020 207d  }}.            }
+00000ca0: 7d29 3b0a 2020 2020 2020 2020 2020 7d7d  });.          }}
+00000cb0: 0a0a 2020 2020 2020 2020 2020 7374 6174  ..          stat
+00000cc0: 6963 2076 6f69 6420 6175 746f 5265 6769  ic void autoRegi
+00000cd0: 7374 6572 2829 207b 7b0a 2020 2020 2020  ster() {{.      
+00000ce0: 2020 2020 2020 2020 7b31 7d0a 2020 2020          {1}.    
+00000cf0: 2020 2020 2020 2020 2020 5f65 6e73 7572            _ensur
+00000d00: 6541 7069 496d 706c 5265 6769 7374 6572  eApiImplRegister
+00000d10: 2829 3b0a 2020 2020 2020 2020 2020 7d7d  ();.          }}
+00000d20: 0a20 2020 2020 2020 207d 7d0a 2020 2020  .        }}.    
+00000d30: 2020 2020 2020 2020 290b 7221 0000 00da          ).r!....
+00000d40: 255f 4170 6941 6e6e 6f74 6174 696f 6e5f  %_ApiAnnotation_
+00000d50: 5f5f 5f69 6d70 6f72 745f 6461 7461 5f63  ___import_data_c
+00000d60: 7265 6174 6f72 721f 0000 0072 0b00 0000  reatorr....r....
+00000d70: 720d 0000 0072 2300 0000 da31 5f41 7069  r....r#....1_Api
+00000d80: 416e 6e6f 7461 7469 6f6e 5f5f 696d 706f  Annotation__impo
+00000d90: 7274 5f64 6174 615f 6372 6561 746f 725f  rt_data_creator_
+00000da0: 7769 7468 6f75 745f 616c 6961 73da 0577  without_alias..w
+00000db0: 7269 7465 da06 666f 726d 6174 da10 6170  rite..format..ap
+00000dc0: 695f 6c69 7374 5f63 7265 6174 6f72 da25  i_list_creator.%
+00000dd0: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
+00000de0: 7265 6769 7374 6572 5f6c 6973 745f 6372  register_list_cr
+00000df0: 6561 746f 7229 0372 0f00 0000 5a05 5f69  eator).r....Z._i
+00000e00: 7465 6dda 0763 6f6e 7465 6e74 7210 0000  tem..contentr...
+00000e10: 0072 1000 0000 7211 0000 005a 185f 5f67  .r....r....Z.__g
+00000e20: 656e 6572 6174 655f 7265 6769 7374 6572  enerate_register
+00000e30: 5f63 6f64 6549 0000 0073 1400 0000 0001  _codeI...s......
+00000e40: 0a01 1a01 0a01 1a02 1002 0415 0a01 0601  ................
+00000e50: 06fe 7a26 4170 6941 6e6e 6f74 6174 696f  ..z&ApiAnnotatio
+00000e60: 6e2e 5f5f 6765 6e65 7261 7465 5f72 6567  n.__generate_reg
+00000e70: 6973 7465 725f 636f 6465 6301 0000 0000  ister_codec.....
+00000e80: 0000 0000 0000 0003 0000 0006 0000 0043  ...............C
+00000e90: 0000 0073 2800 0000 6401 7d01 7c00 6a00  ...s(...d.}.|.j.
+00000ea0: 4400 5d18 7d02 7c01 6402 a001 7c02 6a02  D.].}.|.d...|.j.
+00000eb0: 7c02 6a02 a102 3700 7d01 710a 7c01 5300  |.j...7.}.q.|.S.
+00000ec0: 2903 4e72 0900 0000 7a69 0a20 2020 2020  ).Nr....zi.     
+00000ed0: 2020 2020 2020 2041 7069 5265 6769 7374         ApiRegist
+00000ee0: 6572 4365 6e74 6572 2e72 6567 6973 7465  erCenter.registe
+00000ef0: 7228 7b30 7d2e 4175 746f 5265 6769 7374  r({0}.AutoRegist
+00000f00: 6572 2e61 7069 5479 7065 2c7b 317d 2e41  er.apiType,{1}.A
+00000f10: 7574 6f52 6567 6973 7465 722e 7072 6f76  utoRegister.prov
+00000f20: 6964 6572 293b 0a20 2020 2020 2020 2020  ider);.         
+00000f30: 2020 2029 0372 2100 0000 7238 0000 0072     ).r!...r8...r
+00000f40: 0b00 0000 a903 720f 0000 0072 3b00 0000  ......r....r;...
+00000f50: da04 6974 656d 7210 0000 0072 1000 0000  ..itemr....r....
+00000f60: 7211 0000 005a 175f 5f72 6567 6973 7465  r....Z.__registe
+00000f70: 725f 6c69 7374 5f63 7265 6174 6f72 6a00  r_list_creatorj.
+00000f80: 0000 730c 0000 0000 0104 010a 0106 0208  ..s.............
+00000f90: fe08 037a 2541 7069 416e 6e6f 7461 7469  ...z%ApiAnnotati
+00000fa0: 6f6e 2e5f 5f72 6567 6973 7465 725f 6c69  on.__register_li
+00000fb0: 7374 5f63 7265 6174 6f72 6301 0000 0000  st_creatorc.....
+00000fc0: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
+00000fd0: 0000 0073 2400 0000 6401 7d01 7c00 6a00  ...s$...d.}.|.j.
+00000fe0: 4400 5d14 7d02 7c01 6402 a001 7c02 6a02  D.].}.|.d...|.j.
+00000ff0: a101 3700 7d01 710a 7c01 5300 2903 4e72  ..7.}.q.|.S.).Nr
+00001000: 0900 0000 7a43 0a20 2020 2020 2020 2020  ....zC.         
+00001010: 2020 207b 307d 2e54 4446 4170 6941 7574     {0}.TDFApiAut
+00001020: 6f49 6e76 616c 6964 6174 652e 6170 6954  oInvalidate.apiT
+00001030: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+00001040: 2020 2020 2020 2020 2029 0372 2300 0000           ).r#...
+00001050: 7238 0000 0072 0b00 0000 723c 0000 0072  r8...r....r<...r
+00001060: 1000 0000 7210 0000 0072 1100 0000 7239  ....r....r....r9
+00001070: 0000 0072 0000 0073 0c00 0000 0001 0401  ...r...s........
+00001080: 0a01 0602 04fe 0803 7a1e 4170 6941 6e6e  ........z.ApiAnn
+00001090: 6f74 6174 696f 6e2e 6170 695f 6c69 7374  otation.api_list
+000010a0: 5f63 7265 6174 6f72 6301 0000 0000 0000  _creatorc.......
+000010b0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+000010c0: 0073 6200 0000 7400 a001 6401 a101 0100  .sb...t...d.....
+000010d0: 7c00 6a02 4400 5d4c 7d01 7c00 a003 7c01  |.j.D.]L}.|...|.
+000010e0: 6a04 7c00 6a05 a102 7d02 7c02 6400 7501  j.|.j...}.|.d.u.
+000010f0: 7210 7406 8300 7d03 7c01 6a04 7c03 5f04  r.t...}.|.j.|._.
+00001100: 7c01 6a07 7c03 5f07 7c02 7c03 5f08 7c03  |.j.|._.|.|._.|.
+00001110: a009 a100 0100 7c00 6a0a a00b 7c03 a101  ......|.j...|...
+00001120: 0100 7110 6400 5300 2902 4e75 1c00 0000  ..q.d.S.).Nu....
+00001130: e695 b4e5 9088 e689 80e6 9c89 e4ba a4e4  ................
+00001140: ba92 696d 706c e696 87e4 bbb6 290c 7205  ..impl......).r.
+00001150: 0000 00da 0574 6974 6c65 7225 0000 00da  .....titler%....
+00001160: 1f5f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
+00001170: 5f67 6574 5f74 6172 6765 745f 6669 6c65  _get_target_file
+00001180: 720c 0000 0072 2000 0000 7207 0000 0072  r....r ...r....r
+00001190: 0b00 0000 720d 0000 0072 1700 0000 7221  ....r....r....r!
+000011a0: 0000 00da 0661 7070 656e 6429 0472 0f00  .....append).r..
+000011b0: 0000 da0b 7061 636b 6167 6549 7465 6dda  ....packageItem.
+000011c0: 195f 4170 6941 6e6e 6f74 6174 696f 6e5f  ._ApiAnnotation_
+000011d0: 5f66 696c 655f 7061 7468 5a09 5f69 6d70  _file_pathZ._imp
+000011e0: 6c4e 6f64 6572 1000 0000 7210 0000 0072  lNoder....r....r
+000011f0: 1100 0000 5a1a 5f5f 696e 7465 6772 6174  ....Z.__integrat
+00001200: 655f 7464 665f 696d 706c 5f66 696c 6573  e_tdf_impl_files
+00001210: 7a00 0000 7314 0000 0000 010a 010a 0110  z...s...........
+00001220: 0108 0106 0108 0108 0106 0108 017a 2841  .............z(A
+00001230: 7069 416e 6e6f 7461 7469 6f6e 2e5f 5f69  piAnnotation.__i
+00001240: 6e74 6567 7261 7465 5f74 6466 5f69 6d70  ntegrate_tdf_imp
+00001250: 6c5f 6669 6c65 7363 0100 0000 0000 0000  l_filesc........
+00001260: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
+00001270: 7362 0000 0074 00a0 0164 01a1 0101 007c  sb...t...d.....|
+00001280: 006a 0244 005d 4c7d 017c 00a0 037c 016a  .j.D.]L}.|...|.j
+00001290: 047c 006a 05a1 027d 027c 0264 0075 0172  .|.j...}.|.d.u.r
+000012a0: 1074 0683 007d 037c 016a 047c 035f 047c  .t...}.|.j.|._.|
+000012b0: 016a 077c 035f 077c 027c 035f 087c 03a0  .j.|._.|.|._.|..
+000012c0: 09a1 0001 007c 006a 0aa0 0b7c 03a1 0101  .....|.j...|....
+000012d0: 0071 1064 0053 0029 024e 751b 0000 00e6  .q.d.S.).Nu.....
+000012e0: 95b4 e590 88e6 8980 e69c 89e4 baa4 e4ba  ................
+000012f0: 9261 7069 e696 87e4 bbb6 290c 7205 0000  .api......).r...
+00001300: 0072 3e00 0000 7225 0000 0072 3f00 0000  .r>...r%...r?...
+00001310: 720c 0000 0072 2200 0000 721c 0000 0072  r....r"...r....r
+00001320: 0b00 0000 720d 0000 0072 1700 0000 7223  ....r....r....r#
+00001330: 0000 0072 4000 0000 2904 720f 0000 0072  ...r@...).r....r
+00001340: 4100 0000 7242 0000 005a 085f 6170 694e  A...rB...Z._apiN
+00001350: 6f64 6572 1000 0000 7210 0000 0072 1100  oder....r....r..
+00001360: 0000 5a19 5f5f 696e 7465 6772 6174 655f  ..Z.__integrate_
+00001370: 7464 665f 6170 695f 6669 6c65 7386 0000  tdf_api_files...
+00001380: 0073 1400 0000 0001 0a01 0a01 1001 0801  .s..............
+00001390: 0601 0801 0801 0601 0801 7a27 4170 6941  ..........z'ApiA
+000013a0: 6e6e 6f74 6174 696f 6e2e 5f5f 696e 7465  nnotation.__inte
+000013b0: 6772 6174 655f 7464 665f 6170 695f 6669  grate_tdf_api_fi
+000013c0: 6c65 7329 03da 0966 696c 655f 7061 7468  les)...file_path
+000013d0: da06 7375 6666 6978 da06 7265 7475 726e  ..suffix..return
+000013e0: 6303 0000 0000 0000 0000 0000 000c 0000  c...............
+000013f0: 0006 0000 0043 0000 0073 ce00 0000 7400  .....C...s....t.
+00001400: a001 a100 0100 7402 a003 7c01 a101 0100  ......t...|.....
+00001410: 6401 7d03 7402 a004 7405 a006 a100 a101  d.}.t...t.......
+00001420: a007 a100 a008 6402 a101 6401 1900 7d04  ......d...d...}.
+00001430: 7402 a009 7c04 a101 4400 5d66 5c03 7d05  t...|...D.]f\.}.
+00001440: 7d06 7d07 7c07 4400 5d56 7d08 7402 6a0a  }.}.|.D.]V}.t.j.
+00001450: a00b 7c05 7c08 a102 7d09 7c09 a00c 7c02  ..|.|...}.|...|.
+00001460: a101 724a 7c03 6403 3700 7d03 7405 a00d  ..rJ|.d.7.}.t...
+00001470: a100 7292 7c09 a008 6404 a101 6403 1900  ..r.|...d...d...
+00001480: 7d0a 7c0a a00e 6405 6406 a102 7d0b 714a  }.|...d.d...}.qJ
+00001490: 7c09 a008 6407 a101 6403 1900 7d0b 714a  |...d...d...}.qJ
+000014a0: 713c 7c03 6403 6b02 72b0 7c0b 5300 7c03  q<|.d.k.r.|.S.|.
+000014b0: 6403 6b04 72ca 740f 6408 a010 7c01 a101  d.k.r.t.d...|...
+000014c0: 8301 8201 6400 5300 6400 5300 2909 4e72  ....d.S.d.S.).Nr
+000014d0: 0100 0000 da01 0ae9 0100 0000 7a05 5c6c  ............z.\l
+000014e0: 6962 5cfa 015c 7214 0000 007a 052f 6c69  ib\..\r....z./li
+000014f0: 622f 7530 0000 00e6 a8a1 e59d 977b 307d  b/u0.........{0}
+00001500: e5ad 98e5 9ca8 e5a4 9ae4 b8aa e4ba a4e4  ................
+00001510: ba92 e696 87e4 bbb6 efbc 8ce8 afb7 e6a3  ................
+00001520: 80e6 9fa5 e29d 8c29 1172 0600 0000 7227  .......).r....r'
+00001530: 0000 0072 2800 0000 da05 6368 6469 72da  ...r(.....chdir.
+00001540: 0570 6f70 656e 7204 0000 00da 0770 7764  .popenr......pwd
+00001550: 5f63 6d64 da04 7265 6164 da05 7370 6c69  _cmd..read..spli
+00001560: 74da 0477 616c 6b72 2c00 0000 722d 0000  t..walkr,...r-..
+00001570: 00da 0865 6e64 7377 6974 68da 0a69 735f  ...endswith..is_
+00001580: 7769 6e64 6f77 73da 0772 6570 6c61 6365  windows..replace
+00001590: da09 4578 6365 7074 696f 6e72 3800 0000  ..Exceptionr8...
+000015a0: 290c 720f 0000 0072 4300 0000 7244 0000  ).r....rC...rD..
+000015b0: 00da 0563 6f75 6e74 da08 6e6f 7761 5061  ...count..nowaPa
+000015c0: 7468 da04 726f 6f74 da04 6469 7273 da05  th..root..dirs..
+000015d0: 6669 6c65 73da 0466 696c 65da 0873 7263  files..file..src
+000015e0: 5f66 696c 65da 0474 656d 705a 1b5f 4170  _file..tempZ._Ap
+000015f0: 6941 6e6e 6f74 6174 696f 6e5f 5f74 6172  iAnnotation__tar
+00001600: 6765 745f 6669 6c65 7210 0000 0072 1000  get_filer....r..
+00001610: 0000 7211 0000 005a 115f 5f67 6574 5f74  ..r....Z.__get_t
+00001620: 6172 6765 745f 6669 6c65 9300 0000 7326  arget_file....s&
+00001630: 0000 0000 0108 010a 0204 021c 0114 0108  ................
+00001640: 010e 010a 0108 0108 010e 010e 0212 0108  ................
+00001650: 0104 0108 010e 0104 017a 1f41 7069 416e  .........z.ApiAn
+00001660: 6e6f 7461 7469 6f6e 2e5f 5f67 6574 5f74  notation.__get_t
+00001670: 6172 6765 745f 6669 6c65 6301 0000 0000  arget_filec.....
+00001680: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+00001690: 0000 0073 4e00 0000 7400 a001 a100 0100  ...sN...t.......
+000016a0: 7402 a003 6401 a101 0100 7402 6a04 a005  t...d.....t.j...
+000016b0: 7c00 6a06 a101 722c 7407 a008 7c00 6a06  |.j...r,t...|.j.
+000016c0: a101 0100 7402 a009 7c00 6a06 a101 0100  ....t...|.j.....
+000016d0: 7402 6a04 a00a 7400 a00b a100 6401 7c00  t.j...t.....d.|.
+000016e0: 6a06 a103 5300 2902 4eda 036c 6962 290c  j...S.).N..lib).
+000016f0: 7206 0000 0072 2700 0000 7228 0000 0072  r....r'...r(...r
+00001700: 4900 0000 722c 0000 00da 0665 7869 7374  I...r,.....exist
+00001710: 7372 2400 0000 da06 7368 7574 696c da06  sr$.....shutil..
+00001720: 726d 7472 6565 da05 6d6b 6469 7272 2d00  rmtree..mkdirr-.
+00001730: 0000 da0b 6765 7453 6865 6c6c 4469 7272  ....getShellDirr
+00001740: 0e00 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
+00001750: 0000 0072 2b00 0000 ab00 0000 730c 0000  ...r+.......s...
+00001760: 0000 0108 010a 010e 010c 010c 017a 2141  .............z!A
+00001770: 7069 416e 6e6f 7461 7469 6f6e 2e67 6574  piAnnotation.get
+00001780: 5f69 6e74 6572 6163 7469 6f6e 5f64 6972  _interaction_dir
+00001790: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000017a0: 0005 0000 0043 0000 0073 3200 0000 7400  .....C...s2...t.
+000017b0: a001 a100 0100 7402 6a03 a004 7400 a005  ......t.j...t...
+000017c0: a100 6401 7c00 6a06 a103 7d01 7402 a007  ..d.|.j...}.t...
+000017d0: 6402 a008 7c01 a101 a101 0100 6400 5300  d...|.......d.S.
+000017e0: 2903 4e72 5b00 0000 7a0f 6461 7274 2066  ).Nr[...z.dart f
+000017f0: 6f72 6d61 7420 7b30 7d29 0972 0600 0000  ormat {0}).r....
+00001800: da0f 676f 496e 5368 656c 6c4c 6962 4469  ..goInShellLibDi
+00001810: 7272 2800 0000 722c 0000 0072 2d00 0000  rr(...r,...r-...
+00001820: 7260 0000 0072 2400 0000 da06 7379 7374  r`...r$.....syst
+00001830: 656d 7238 0000 0029 0272 0f00 0000 5a14  emr8...).r....Z.
+00001840: 5f41 7069 416e 6e6f 7461 7469 6f6e 5f5f  _ApiAnnotation__
+00001850: 7061 7468 7210 0000 0072 1000 0000 7211  pathr....r....r.
+00001860: 0000 0072 3300 0000 b400 0000 7306 0000  ...r3.......s...
+00001870: 0000 0108 0116 017a 1841 7069 416e 6e6f  .......z.ApiAnno
+00001880: 7461 7469 6f6e 2e5f 5f66 6f72 6d61 745f  tation.__format_
+00001890: 5f63 0500 0000 0000 0000 0000 0000 0500  _c..............
+000018a0: 0000 0700 0000 4300 0000 7318 0000 007c  ......C...s....|
+000018b0: 01a0 0064 01a0 017c 027c 037c 04a1 03a1  ...d...|.|.|....
+000018c0: 0101 0064 0053 0029 024e 7a21 696d 706f  ...d.S.).Nz!impo
+000018d0: 7274 2022 7061 636b 6167 653a 7b30 7d2f  rt "package:{0}/
+000018e0: 7b31 7d22 2061 7320 7b32 7d3b 0aa9 0272  {1}" as {2};...r
+000018f0: 3700 0000 7238 0000 0029 0572 0f00 0000  7...r8...).r....
+00001900: da07 665f 7772 6974 65da 0b6d 6f64 756c  ..f_write..modul
+00001910: 655f 6e61 6d65 7243 0000 00da 0561 6c69  e_namerC.....ali
+00001920: 6173 7210 0000 0072 1000 0000 7211 0000  asr....r....r...
+00001930: 005a 175f 5f5f 5f69 6d70 6f72 745f 6461  .Z.____import_da
+00001940: 7461 5f63 7265 6174 6f72 ba00 0000 730a  ta_creator....s.
+00001950: 0000 0000 0304 0104 0106 ff02 ff7a 2541  .............z%A
+00001960: 7069 416e 6e6f 7461 7469 6f6e 2e5f 5f5f  piAnnotation.___
+00001970: 5f69 6d70 6f72 745f 6461 7461 5f63 7265  _import_data_cre
+00001980: 6174 6f72 6304 0000 0000 0000 0000 0000  atorc...........
+00001990: 0004 0000 0006 0000 0043 0000 0073 1600  .........C...s..
+000019a0: 0000 7c01 a000 6401 a001 7c02 7c03 a102  ..|...d...|.|...
+000019b0: a101 0100 6400 5300 2902 4e7a 1a69 6d70  ....d.S.).Nz.imp
+000019c0: 6f72 7420 2270 6163 6b61 6765 3a7b 307d  ort "package:{0}
+000019d0: 2f7b 317d 223b 0a72 6300 0000 2904 720f  /{1}";.rc...).r.
+000019e0: 0000 0072 6400 0000 7265 0000 0072 4300  ...rd...re...rC.
+000019f0: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00001a00: 005a 235f 5f69 6d70 6f72 745f 6461 7461  .Z#__import_data
+00001a10: 5f63 7265 6174 6f72 5f77 6974 686f 7574  _creator_without
+00001a20: 5f61 6c69 6173 c400 0000 730a 0000 0000  _alias....s.....
+00001a30: 0304 0104 0104 ff02 ff7a 3141 7069 416e  .........z1ApiAn
+00001a40: 6e6f 7461 7469 6f6e 2e5f 5f69 6d70 6f72  notation.__impor
+00001a50: 745f 6461 7461 5f63 7265 6174 6f72 5f77  t_data_creator_w
+00001a60: 6974 686f 7574 5f61 6c69 6173 4e29 1272  ithout_aliasN).r
+00001a70: 1900 0000 721a 0000 0072 1b00 0000 da07  ....r....r......
+00001a80: 5f5f 646f 635f 5f72 1200 0000 7226 0000  __doc__r....r&..
+00001a90: 0072 3400 0000 7231 0000 0072 3a00 0000  .r4...r1...r:...
+00001aa0: 7239 0000 0072 3000 0000 722f 0000 00da  r9...r0...r/....
+00001ab0: 0373 7472 723f 0000 0072 2b00 0000 7233  .strr?...r+...r3
+00001ac0: 0000 0072 3500 0000 7236 0000 0072 1000  ...r5...r6...r..
+00001ad0: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00001ae0: 0072 1d00 0000 1d00 0000 731c 0000 0008  .r........s.....
+00001af0: 0104 0408 0d08 0608 1408 2108 0808 0808  ..........!.....
+00001b00: 0c08 0d12 1808 0908 0608 0a72 1d00 0000  ...........r....
+00001b10: 290e 7228 0000 0072 5d00 0000 da25 7464  ).r(...r]....%td
+00001b20: 665f 746f 6f6c 2e74 6f6f 6c73 2e63 6f6e  f_tool.tools.con
+00001b30: 6669 672e 7061 636b 6167 6573 5f63 6f6e  fig.packages_con
+00001b40: 6669 6772 0200 0000 7203 0000 00da 1d74  figr....r......t
+00001b50: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 706c  df_tool.tools.pl
+00001b60: 6174 666f 726d 5f74 6f6f 6c73 7204 0000  atform_toolsr...
+00001b70: 00da 1474 6466 5f74 6f6f 6c2e 746f 6f6c  ...tdf_tool.tool
+00001b80: 732e 7072 696e 7472 0500 0000 da18 7464  s.printr......td
+00001b90: 665f 746f 6f6c 2e74 6f6f 6c73 2e73 6865  f_tool.tools.she
+00001ba0: 6c6c 5f64 6972 7206 0000 0072 0700 0000  ll_dirr....r....
+00001bb0: 721c 0000 0072 1d00 0000 7210 0000 0072  r....r....r....r
+00001bc0: 1000 0000 7210 0000 0072 1100 0000 da08  ....r....r......
+00001bd0: 3c6d 6f64 756c 653e 0100 0000 7310 0000  <module>....s...
+00001be0: 0008 0108 0110 010c 010c 010c 030e 0a0e  ................
+00001bf0: 0a                                       .
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 16 07:59:17 2024 UTC, .py size: 1246 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d52f 1e66 de04 0000  a......../.f....
+00000000: 610d 0d0a 0000 0000 0fe5 2066 dc04 0000  a......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 8302 5a0a 6407 5300 2908 e900 0000 0029  ..Z.d.S.)......)
@@ -48,58 +48,58 @@
 000002f0: 2020 2020 2020 746c 2066 6978 4865 6164        tl fixHead
 00000300: 6572 2073 7461 7274 efbc 8ce4 bc9a e4bb  er start........
 00000310: a5e4 baa4 e4ba 92e5 bc8f e8bf 9be8 a18c  ................
 00000320: e8bf 9be8 a18c e5a4 b4e6 9687 e4bb b6e4  ................
 00000330: bfae e5a4 8d0a 2020 2020 2020 2020 f519  ......        ..
 00000340: 0000 0074 6c20 6669 7848 6561 6465 7220  ...tl fixHeader 
 00000350: e58f aae6 94af e68c 8169 4f53 4e29 0a72  .........iOSN).r
-00000360: 0300 0000 da0d 6469 7249 6e76 616c 6964  ......dirInvalid
-00000370: 6174 65da 0e67 6574 5072 6f6a 6563 7454  ate..getProjectT
-00000380: 7970 6572 0200 0000 da07 464c 5554 5445  yper......FLUTTE
-00000390: 5272 0400 0000 da05 6572 726f 72da 0349  Rr......error..I
-000003a0: 4f53 720a 0000 00da 0573 7461 7274 2902  OSr......start).
-000003b0: 720b 0000 00da 0b70 726f 6a65 6374 5479  r......projectTy
-000003c0: 7065 720c 0000 0072 0c00 0000 720d 0000  per....r....r...
-000003d0: 0072 1500 0000 1000 0000 730c 0000 0000  .r........s.....
-000003e0: 0408 0108 010a 010c 010a 017a 0f46 6978  ...........z.Fix
-000003f0: 4865 6164 6572 2e73 7461 7274 2901 da04  Header.start)...
-00000400: 6e61 6d65 6302 0000 0000 0000 0000 0000  namec...........
-00000410: 0003 0000 0003 0000 0043 0000 0073 4000  .........C...s@.
-00000420: 0000 7400 a001 a100 0100 7400 a002 a100  ..t.......t.....
-00000430: 7d02 7c02 7403 6a04 6b02 7226 7405 a006  }.|.t.j.k.r&t...
-00000440: 6401 a101 0100 6e16 7c02 7403 6a07 6b02  d.....n.|.t.j.k.
-00000450: 723c 7c00 6a08 a009 7c01 a101 0100 6402  r<|.j...|.....d.
-00000460: 5300 2903 754c 0000 000a 2020 2020 2020  S.).uL....      
-00000470: 2020 746c 2066 6978 4865 6164 6572 206d    tl fixHeader m
-00000480: 6f64 756c 65e3 8090 e6a8 a1e5 9d97 e590  odule...........
-00000490: 8de3 8091 efbc 8ce4 bfae e5a4 8de6 8c87  ................
-000004a0: e5ae 9ae6 a8a1 e59d 97e5 908d 0a20 2020  .............   
-000004b0: 2020 2020 2072 0f00 0000 4e29 0a72 0300       r....N).r..
-000004c0: 0000 7210 0000 0072 1100 0000 7202 0000  ..r....r....r...
-000004d0: 0072 1200 0000 7204 0000 0072 1300 0000  .r....r....r....
-000004e0: 7214 0000 0072 0a00 0000 da06 6d6f 6475  r....r......modu
-000004f0: 6c65 2903 720b 0000 0072 1700 0000 7216  le).r....r....r.
-00000500: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000510: 0000 7218 0000 001b 0000 0073 0c00 0000  ..r........s....
-00000520: 0004 0801 0801 0a01 0c01 0a01 7a10 4669  ............z.Fi
-00000530: 7848 6561 6465 722e 6d6f 6475 6c65 4e29  xHeader.moduleN)
-00000540: 08da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000550: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000560: 616d 655f 5fda 075f 5f64 6f63 5f5f 720e  ame__..__doc__r.
-00000570: 0000 0072 1500 0000 da03 7374 7272 1800  ...r......strr..
-00000580: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00000590: 0072 0d00 0000 7208 0000 0007 0000 0073  .r....r........s
-000005a0: 0800 0000 0801 0404 0804 080b 7208 0000  ............r...
-000005b0: 004e 290b da18 7464 665f 746f 6f6c 2e74  .N)...tdf_tool.t
-000005c0: 6f6f 6c73 2e73 6865 6c6c 5f64 6972 7202  ools.shell_dirr.
-000005d0: 0000 0072 0300 0000 da14 7464 665f 746f  ...r......tdf_to
-000005e0: 6f6c 2e74 6f6f 6c73 2e70 7269 6e74 7204  ol.tools.printr.
-000005f0: 0000 005a 2974 6466 5f74 6f6f 6c2e 746f  ...Z)tdf_tool.to
-00000600: 6f6c 732e 6669 785f 6865 6164 6572 2e66  ols.fix_header.f
-00000610: 6978 5f68 6561 6465 725f 6c69 6e74 7205  ix_header_lintr.
-00000620: 0000 005a 2a74 6466 5f74 6f6f 6c2e 746f  ...Z*tdf_tool.to
-00000630: 6f6c 732e 6669 785f 6865 6164 6572 2e66  ols.fix_header.f
-00000640: 6978 5f68 6561 6465 725f 656e 7472 7972  ix_header_entryr
-00000650: 0600 0000 7207 0000 0072 0800 0000 720c  ....r....r....r.
-00000660: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000670: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000680: 7308 0000 0010 010c 010c 0110 03         s............
+00000360: 0300 0000 da0c 676f 496e 5368 656c 6c44  ......goInShellD
+00000370: 6972 da0e 6765 7450 726f 6a65 6374 5479  ir..getProjectTy
+00000380: 7065 7202 0000 00da 0746 4c55 5454 4552  per......FLUTTER
+00000390: 7204 0000 00da 0565 7272 6f72 da03 494f  r......error..IO
+000003a0: 5372 0a00 0000 da05 7374 6172 7429 0272  Sr......start).r
+000003b0: 0b00 0000 da0b 7072 6f6a 6563 7454 7970  ......projectTyp
+000003c0: 6572 0c00 0000 720c 0000 0072 0d00 0000  er....r....r....
+000003d0: 7215 0000 0010 0000 0073 0c00 0000 0004  r........s......
+000003e0: 0801 0801 0a01 0c01 0a01 7a0f 4669 7848  ..........z.FixH
+000003f0: 6561 6465 722e 7374 6172 7429 01da 046e  eader.start)...n
+00000400: 616d 6563 0200 0000 0000 0000 0000 0000  amec............
+00000410: 0300 0000 0300 0000 4300 0000 7340 0000  ........C...s@..
+00000420: 0074 00a0 01a1 0001 0074 00a0 02a1 007d  .t.......t.....}
+00000430: 027c 0274 036a 046b 0272 2674 05a0 0664  .|.t.j.k.r&t...d
+00000440: 01a1 0101 006e 167c 0274 036a 076b 0272  .....n.|.t.j.k.r
+00000450: 3c7c 006a 08a0 097c 01a1 0101 0064 0253  <|.j...|.....d.S
+00000460: 0029 0375 4c00 0000 0a20 2020 2020 2020  .).uL....       
+00000470: 2074 6c20 6669 7848 6561 6465 7220 6d6f   tl fixHeader mo
+00000480: 6475 6c65 e380 90e6 a8a1 e59d 97e5 908d  dule............
+00000490: e380 91ef bc8c e4bf aee5 a48d e68c 87e5  ................
+000004a0: ae9a e6a8 a1e5 9d97 e590 8d0a 2020 2020  ............    
+000004b0: 2020 2020 720f 0000 004e 290a 7203 0000      r....N).r...
+000004c0: 0072 1000 0000 7211 0000 0072 0200 0000  .r....r....r....
+000004d0: 7212 0000 0072 0400 0000 7213 0000 0072  r....r....r....r
+000004e0: 1400 0000 720a 0000 00da 066d 6f64 756c  ....r......modul
+000004f0: 6529 0372 0b00 0000 7217 0000 0072 1600  e).r....r....r..
+00000500: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000510: 0072 1800 0000 1b00 0000 730c 0000 0000  .r........s.....
+00000520: 0408 0108 010a 010c 010a 017a 1046 6978  ...........z.Fix
+00000530: 4865 6164 6572 2e6d 6f64 756c 654e 2908  Header.moduleN).
+00000540: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000550: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000560: 6d65 5f5f da07 5f5f 646f 635f 5f72 0e00  me__..__doc__r..
+00000570: 0000 7215 0000 00da 0373 7472 7218 0000  ..r......strr...
+00000580: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000590: 720d 0000 0072 0800 0000 0700 0000 7308  r....r........s.
+000005a0: 0000 0008 0104 0408 0408 0b72 0800 0000  ...........r....
+000005b0: 4e29 0bda 1874 6466 5f74 6f6f 6c2e 746f  N)...tdf_tool.to
+000005c0: 6f6c 732e 7368 656c 6c5f 6469 7272 0200  ols.shell_dirr..
+000005d0: 0000 7203 0000 00da 1474 6466 5f74 6f6f  ..r......tdf_too
+000005e0: 6c2e 746f 6f6c 732e 7072 696e 7472 0400  l.tools.printr..
+000005f0: 0000 5a29 7464 665f 746f 6f6c 2e74 6f6f  ..Z)tdf_tool.too
+00000600: 6c73 2e66 6978 5f68 6561 6465 722e 6669  ls.fix_header.fi
+00000610: 785f 6865 6164 6572 5f6c 696e 7472 0500  x_header_lintr..
+00000620: 0000 5a2a 7464 665f 746f 6f6c 2e74 6f6f  ..Z*tdf_tool.too
+00000630: 6c73 2e66 6978 5f68 6561 6465 722e 6669  ls.fix_header.fi
+00000640: 785f 6865 6164 6572 5f65 6e74 7279 7206  x_header_entryr.
+00000650: 0000 0072 0700 0000 7208 0000 0072 0c00  ...r....r....r..
+00000660: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000670: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000680: 0800 0000 1001 0c01 0c01 1003            ............
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 16 07:59:17 2024 UTC, .py size: 1212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d52f 1e66 bc04 0000  a......../.f....
+00000000: 610d 0d0a 0000 0000 d7e4 2066 bb04 0000  a......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a09  ..G.d.d...d...Z.
 00000070: 6407 5300 2908 e900 0000 0029 01da 1149  d.S.)......)...I
@@ -35,68 +35,68 @@
 00000220: 6466 5f74 6f6f 6c2f 7069 7065 6c69 6e65  df_tool/pipeline
 00000230: 732f 6769 742e 7079 da08 5f5f 696e 6974  s/git.py..__init
 00000240: 5f5f 0c00 0000 7304 0000 0000 010c 017a  __....s........z
 00000250: 0c47 6974 2e5f 5f69 6e69 745f 5f63 0100  .Git.__init__c..
 00000260: 0000 0000 0000 0000 0000 0100 0000 0200  ................
 00000270: 0000 4300 0000 7314 0000 0074 00a0 01a1  ..C...s....t....
 00000280: 0001 007c 00a0 02a1 0001 0064 0053 0029  ...|.......d.S.)
-00000290: 014e 2903 7206 0000 00da 0d64 6972 496e  .N).r......dirIn
-000002a0: 7661 6c69 6461 7465 da13 5f47 6974 5f5f  validate.._Git__
-000002b0: 6261 7463 685f 7275 6e5f 6769 7429 0172  batch_run_git).r
-000002c0: 0c00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-000002d0: 0000 00da 0372 756e 1000 0000 7304 0000  .....run....s...
-000002e0: 0000 0108 017a 0747 6974 2e72 756e 6301  .....z.Git.runc.
-000002f0: 0000 0000 0000 0000 0000 0004 0000 0007  ................
-00000300: 0000 0043 0000 0073 b200 0000 7400 a001  ...C...s....t...
-00000310: a100 0100 7400 a002 a100 7d01 7c01 7403  ....t.....}.|.t.
-00000320: 6a04 6b02 7288 7405 a006 6401 6402 a007  j.k.r.t...d.d...
-00000330: 7c00 6a08 a101 1700 a101 0100 7409 6a0a  |.j.........t.j.
-00000340: 7c00 6a08 6403 6404 8d02 0100 740b 8300  |.j.d.d.....t...
-00000350: 6a0c 4400 5d3c 7d02 7400 a00d 7c02 a101  j.D.]<}.t...|...
-00000360: 0100 7405 a006 6405 7c02 1700 6406 1700  ..t...d.|...d...
-00000370: 6402 a007 7c00 6a08 a101 1700 a101 0100  d...|.j.........
-00000380: 7409 6a0a 7c00 6a08 6403 6404 8d02 0100  t.j.|.j.d.d.....
-00000390: 7148 6e26 7c01 7403 6a0e 6b02 72ae 6700  qHn&|.t.j.k.r.g.
-000003a0: 6407 a201 7c00 6a0f 1700 7d03 7409 6a0a  d...|.j...}.t.j.
-000003b0: 7c03 6403 6404 8d02 0100 6400 5300 2908  |.d.d.....d.S.).
-000003c0: 4e75 1200 0000 e5bc 80e5 a78b e693 8de4  Nu..............
-000003d0: bd9c e5a3 b3ef bc9a fa01 2046 2901 da05  .......... F)...
-000003e0: 7368 656c 6c75 0c00 0000 e5bc 80e5 a78b  shellu..........
-000003f0: e693 8de4 bd9c 7509 0000 00e6 a8a1 e59d  ......u.........
-00000400: 97ef bc9a 2905 da06 6275 6e64 6c65 da04  ....)...bundle..
-00000410: 6578 6563 da03 706f 64da 0362 696e da05  exec..pod..bin..
-00000420: 6261 7463 6829 1072 0600 0000 da0c 676f  batch).r......go
-00000430: 496e 5368 656c 6c44 6972 da0e 6765 7450  InShellDir..getP
-00000440: 726f 6a65 6374 5479 7065 7205 0000 00da  rojectTyper.....
-00000450: 0746 4c55 5454 4552 7204 0000 00da 0574  .FLUTTERr......t
-00000460: 6974 6c65 da04 6a6f 696e 720a 0000 0072  itle..joinr....r
-00000470: 0300 0000 da0b 7275 6e41 6e64 5072 696e  ......runAndPrin
-00000480: 7472 0200 0000 da0e 6d6f 6475 6c65 4e61  tr......moduleNa
-00000490: 6d65 4c69 7374 da0d 676f 496e 4d6f 6475  meList..goInModu
-000004a0: 6c65 4469 72da 0349 4f53 720b 0000 0029  leDir..IOSr....)
-000004b0: 0472 0c00 0000 da0b 7072 6f6a 6563 7454  .r......projectT
-000004c0: 7970 65da 066d 6f64 756c 65da 0769 6f73  ype..module..ios
-000004d0: 5f61 7267 720d 0000 0072 0d00 0000 720e  _argr....r....r.
-000004e0: 0000 005a 0f5f 5f62 6174 6368 5f72 756e  ...Z.__batch_run
-000004f0: 5f67 6974 1400 0000 7318 0000 0000 0108  _git....s.......
-00000500: 0108 010a 0116 0110 020c 010a 011e 0114  ................
-00000510: 010a 010e 017a 1347 6974 2e5f 5f62 6174  .....z.Git.__bat
-00000520: 6368 5f72 756e 5f67 6974 4e29 08da 085f  ch_run_gitN)..._
-00000530: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000540: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000550: 5fda 075f 5f64 6f63 5f5f da04 6c69 7374  _..__doc__..list
-00000560: 720f 0000 0072 1200 0000 7211 0000 0072  r....r....r....r
-00000570: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00000580: 0000 0072 0700 0000 0700 0000 7308 0000  ...r........s...
-00000590: 0008 0104 040e 0408 0472 0700 0000 4e29  .........r....N)
-000005a0: 0ada 2974 6466 5f74 6f6f 6c2e 746f 6f6c  ..)tdf_tool.tool
-000005b0: 732e 636f 6e66 6967 2e69 6e69 7469 616c  s.config.initial
-000005c0: 5f6a 736f 6e5f 636f 6e66 6967 7202 0000  _json_configr...
-000005d0: 00da 1274 6466 5f74 6f6f 6c2e 746f 6f6c  ...tdf_tool.tool
-000005e0: 732e 636d 6472 0300 0000 da14 7464 665f  s.cmdr......tdf_
-000005f0: 746f 6f6c 2e74 6f6f 6c73 2e70 7269 6e74  tool.tools.print
-00000600: 7204 0000 00da 1874 6466 5f74 6f6f 6c2e  r......tdf_tool.
-00000610: 746f 6f6c 732e 7368 656c 6c5f 6469 7272  tools.shell_dirr
-00000620: 0500 0000 7206 0000 0072 0700 0000 720d  ....r....r....r.
-00000630: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000640: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000650: 7308 0000 000c 010c 010c 0110 03         s............
+00000290: 014e 2903 7206 0000 00da 0c67 6f49 6e53  .N).r......goInS
+000002a0: 6865 6c6c 4469 72da 135f 4769 745f 5f62  hellDir.._Git__b
+000002b0: 6174 6368 5f72 756e 5f67 6974 2901 720c  atch_run_git).r.
+000002c0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+000002d0: 0000 da03 7275 6e10 0000 0073 0400 0000  ....run....s....
+000002e0: 0001 0801 7a07 4769 742e 7275 6e63 0100  ....z.Git.runc..
+000002f0: 0000 0000 0000 0000 0000 0400 0000 0700  ................
+00000300: 0000 4300 0000 73b2 0000 0074 00a0 01a1  ..C...s....t....
+00000310: 0001 0074 00a0 02a1 007d 017c 0174 036a  ...t.....}.|.t.j
+00000320: 046b 0272 8874 05a0 0664 0164 02a0 077c  .k.r.t...d.d...|
+00000330: 006a 08a1 0117 00a1 0101 0074 096a 0a7c  .j.........t.j.|
+00000340: 006a 0864 0364 048d 0201 0074 0b83 006a  .j.d.d.....t...j
+00000350: 0c44 005d 3c7d 0274 00a0 0d7c 02a1 0101  .D.]<}.t...|....
+00000360: 0074 05a0 0664 057c 0217 0064 0617 0064  .t...d.|...d...d
+00000370: 02a0 077c 006a 08a1 0117 00a1 0101 0074  ...|.j.........t
+00000380: 096a 0a7c 006a 0864 0364 048d 0201 0071  .j.|.j.d.d.....q
+00000390: 486e 267c 0174 036a 0e6b 0272 ae67 0064  Hn&|.t.j.k.r.g.d
+000003a0: 07a2 017c 006a 0f17 007d 0374 096a 0a7c  ...|.j...}.t.j.|
+000003b0: 0364 0364 048d 0201 0064 0053 0029 084e  .d.d.....d.S.).N
+000003c0: 7512 0000 00e5 bc80 e5a7 8be6 938d e4bd  u...............
+000003d0: 9ce5 a3b3 efbc 9afa 0120 4629 01da 0573  ......... F)...s
+000003e0: 6865 6c6c 750c 0000 00e5 bc80 e5a7 8be6  hellu...........
+000003f0: 938d e4bd 9c75 0900 0000 e6a8 a1e5 9d97  .....u..........
+00000400: efbc 9a29 05da 0662 756e 646c 65da 0465  ...)...bundle..e
+00000410: 7865 63da 0370 6f64 da03 6269 6eda 0562  xec..pod..bin..b
+00000420: 6174 6368 2910 7206 0000 0072 1000 0000  atch).r....r....
+00000430: da0e 6765 7450 726f 6a65 6374 5479 7065  ..getProjectType
+00000440: 7205 0000 00da 0746 4c55 5454 4552 7204  r......FLUTTERr.
+00000450: 0000 00da 0574 6974 6c65 da04 6a6f 696e  .....title..join
+00000460: 720a 0000 0072 0300 0000 da0b 7275 6e41  r....r......runA
+00000470: 6e64 5072 696e 7472 0200 0000 da0e 6d6f  ndPrintr......mo
+00000480: 6475 6c65 4e61 6d65 4c69 7374 da0d 676f  duleNameList..go
+00000490: 496e 4d6f 6475 6c65 4469 72da 0349 4f53  InModuleDir..IOS
+000004a0: 720b 0000 0029 0472 0c00 0000 da0b 7072  r....).r......pr
+000004b0: 6f6a 6563 7454 7970 65da 066d 6f64 756c  ojectType..modul
+000004c0: 65da 0769 6f73 5f61 7267 720d 0000 0072  e..ios_argr....r
+000004d0: 0d00 0000 720e 0000 005a 0f5f 5f62 6174  ....r....Z.__bat
+000004e0: 6368 5f72 756e 5f67 6974 1400 0000 7318  ch_run_git....s.
+000004f0: 0000 0000 0108 0108 010a 0116 0110 020c  ................
+00000500: 010a 011e 0114 010a 010e 017a 1347 6974  ...........z.Git
+00000510: 2e5f 5f62 6174 6368 5f72 756e 5f67 6974  .__batch_run_git
+00000520: 4e29 08da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000530: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000540: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000550: da04 6c69 7374 720f 0000 0072 1200 0000  ..listr....r....
+00000560: 7211 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000570: 0d00 0000 720e 0000 0072 0700 0000 0700  ....r....r......
+00000580: 0000 7308 0000 0008 0104 040e 0408 0472  ..s............r
+00000590: 0700 0000 4e29 0ada 2974 6466 5f74 6f6f  ....N)..)tdf_too
+000005a0: 6c2e 746f 6f6c 732e 636f 6e66 6967 2e69  l.tools.config.i
+000005b0: 6e69 7469 616c 5f6a 736f 6e5f 636f 6e66  nitial_json_conf
+000005c0: 6967 7202 0000 00da 1274 6466 5f74 6f6f  igr......tdf_too
+000005d0: 6c2e 746f 6f6c 732e 636d 6472 0300 0000  l.tools.cmdr....
+000005e0: da14 7464 665f 746f 6f6c 2e74 6f6f 6c73  ..tdf_tool.tools
+000005f0: 2e70 7269 6e74 7204 0000 00da 1874 6466  .printr......tdf
+00000600: 5f74 6f6f 6c2e 746f 6f6c 732e 7368 656c  _tool.tools.shel
+00000610: 6c5f 6469 7272 0500 0000 7206 0000 0072  l_dirr....r....r
+00000620: 0700 0000 720d 0000 0072 0d00 0000 720d  ....r....r....r.
+00000630: 0000 0072 0e00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000640: 653e 0100 0000 7308 0000 000c 010c 010c  e>....s.........
+00000650: 0110 03                                  ...
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 16 07:59:17 2024 UTC, .py size: 1926 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,125 @@
-00000000: 610d 0d0a 0000 0000 d52f 1e66 8607 0000  a......../.f....
+00000000: 610d 0d0a 0000 0000 fce4 2066 7806 0000  a......... fx...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
-00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
-00000070: 6406 6407 8400 6407 8302 5a0b 6408 5300  d.d...d...Z.d.S.
-00000080: 2909 e900 0000 0029 01da 0a50 726f 6a65  )......)...Proje
-00000090: 6374 434c 4929 01da 0343 6d64 2901 da0d  ctCLI)...Cmd)...
-000000a0: 434c 494a 736f 6e43 6f6e 6669 6729 02da  CLIJsonConfig)..
-000000b0: 0b50 726f 6a65 6374 5479 7065 da08 5368  .ProjectType..Sh
-000000c0: 656c 6c44 6972 2901 da0d 5673 436f 6465  ellDir)...VsCode
-000000d0: 4d61 6e61 6765 7263 0000 0000 0000 0000  Managerc........
-000000e0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-000000f0: 7340 0000 0065 005a 0164 005a 0264 015a  s@...e.Z.d.Z.d.Z
-00000100: 0364 0264 0384 005a 0464 0464 0584 005a  .d.d...Z.d.d...Z
-00000110: 0564 0664 0784 005a 0664 0864 0984 005a  .d.d...Z.d.d...Z
-00000120: 0764 0a64 0b84 005a 0864 0c64 0d84 005a  .d.d...Z.d.d...Z
-00000130: 0964 0e53 0029 0fda 064d 6f64 756c 6575  .d.S.)...Moduleu
-00000140: 3900 0000 0a20 2020 20e6 a8a1 e59d 97e7  9....    .......
-00000150: 9bb8 e585 b3e5 b7a5 e585 b7ef bc9a 2074  .............. t
-00000160: 6c20 6d6f 6475 6c65 202d 6820 e69f a5e7  l module -h ....
-00000170: 9c8b e8af a6e6 8385 0a20 2020 2063 0100  .........    c..
-00000180: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000190: 0000 4300 0000 7314 0000 0074 0083 007c  ..C...s....t...|
-000001a0: 005f 0174 0283 007c 005f 0364 0053 0029  ._.t...|._.d.S.)
-000001b0: 014e 2904 7202 0000 00da 0c5f 4d6f 6475  .N).r......_Modu
-000001c0: 6c65 5f5f 636c 6972 0700 0000 da16 5f4d  le__clir......_M
-000001d0: 6f64 756c 655f 5f76 7363 6f64 654d 616e  odule__vscodeMan
-000001e0: 6167 6572 a901 da04 7365 6c66 a900 720d  ager....self..r.
-000001f0: 0000 00f5 6500 0000 2f55 7365 7273 2f78  ....e.../Users/x
-00000200: 756a 6961 6e2f 446f 6375 6d65 6e74 732f  ujian/Documents/
-00000210: 3230 3234 2fe6 a8a1 e59d 97e9 97b4 e4ba  2024/...........
-00000220: a4e4 ba92 e9a1 b9e7 9bae 746c e58d 87e7  ..........tl....
-00000230: baa7 2f70 6163 6b61 6765 5f74 6f6f 6c73  ../package_tools
-00000240: 2f74 6466 5f74 6f6f 6c2f 7069 7065 6c69  /tdf_tool/pipeli
-00000250: 6e65 732f 6d6f 6475 6c65 2e70 79da 085f  nes/module.py.._
-00000260: 5f69 6e69 745f 5f0d 0000 0073 0400 0000  _init__....s....
-00000270: 0001 0801 7a0f 4d6f 6475 6c65 2e5f 5f69  ....z.Module.__i
-00000280: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00000290: 0000 0100 0000 0200 0000 4300 0000 7316  ..........C...s.
-000002a0: 0000 0074 00a0 01a1 0001 007c 006a 02a0  ...t.......|.j..
-000002b0: 03a1 0001 0064 0153 0029 0275 2100 0000  .....d.S.).u!...
-000002c0: 0a20 2020 2020 2020 20e9 a1b9 e79b aee5  .        .......
-000002d0: 889d e5a7 8be5 8c96 0a20 2020 2020 2020  .........       
-000002e0: 204e 2904 7206 0000 00da 0d64 6972 496e   N).r......dirIn
-000002f0: 7661 6c69 6461 7465 7209 0000 00da 0769  validater......i
-00000300: 6e69 7469 616c 720b 0000 0072 0d00 0000  nitialr....r....
-00000310: 720d 0000 0072 0e00 0000 da04 696e 6974  r....r......init
-00000320: 1100 0000 7304 0000 0000 0408 017a 0b4d  ....s........z.M
-00000330: 6f64 756c 652e 696e 6974 6301 0000 0000  odule.initc.....
-00000340: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00000350: 0000 0073 5200 0000 7400 a001 a100 0100  ...sR...t.......
-00000360: 7400 a002 a100 0100 7400 a003 a100 7d01  t.......t.....}.
-00000370: 7c01 7404 6a05 6b02 722e 7c00 6a06 a007  |.t.j.k.r.|.j...
-00000380: a100 0100 6e20 7c01 7404 6a08 6b02 724e  ....n |.t.j.k.rN
-00000390: 6700 6401 a201 7d02 7409 6a0a 7c02 6402  g.d...}.t.j.|.d.
-000003a0: 6403 8d02 0100 6404 5300 a905 7555 0000  d.....d.S...uU..
-000003b0: 000a 2020 2020 2020 2020 e4bf aee6 94b9  ..        ......
-000003c0: 696e 6974 6961 6c5f 636f 6e66 6967 2e6a  initial_config.j
-000003d0: 736f 6ee6 9687 e4bb b6e5 908e efbc 8ce6  son.............
-000003e0: 89a7 e8a1 8ce8 afa5 e591 bde4 bba4 efbc  ................
-000003f0: 8ce6 9bb4 e696 b0e4 be9d e8b5 960a 2020  ..............  
-00000400: 2020 2020 2020 2906 5a06 6275 6e64 6c65        ).Z.bundle
-00000410: da04 6578 6563 5a03 706f 64da 0362 696e  ..execZ.pod..bin
-00000420: 5a05 6261 7463 68da 0563 6c6f 6e65 4629  Z.batch..cloneF)
-00000430: 01da 0573 6865 6c6c 4e29 0b72 0600 0000  ...shellN).r....
-00000440: 7210 0000 00da 0c67 6f49 6e53 6865 6c6c  r......goInShell
-00000450: 4469 72da 0e67 6574 5072 6f6a 6563 7454  Dir..getProjectT
-00000460: 7970 6572 0500 0000 da07 464c 5554 5445  yper......FLUTTE
-00000470: 5272 0900 0000 5a07 636c 6944 6570 73da  Rr....Z.cliDeps.
-00000480: 0349 4f53 7203 0000 00da 0b72 756e 416e  .IOSr......runAn
-00000490: 6450 7269 6e74 a903 720c 0000 005a 0b70  dPrint..r....Z.p
-000004a0: 726f 6a65 6374 5479 7065 5a07 696f 735f  rojectTypeZ.ios_
-000004b0: 6172 6772 0d00 0000 720d 0000 0072 0e00  argr....r....r..
-000004c0: 0000 da04 6465 7073 1800 0000 7310 0000  ....deps....s...
-000004d0: 0000 0408 0108 0108 010a 010c 010a 0108  ................
-000004e0: 017a 0b4d 6f64 756c 652e 6465 7073 6301  .z.Module.depsc.
-000004f0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000500: 0000 0043 0000 0073 5200 0000 7400 a001  ...C...sR...t...
-00000510: a100 0100 7400 a002 a100 0100 7400 a003  ....t.......t...
-00000520: a100 7d01 7c01 7404 6a05 6b02 722e 7c00  ..}.|.t.j.k.r.|.
-00000530: 6a06 a007 a100 0100 6e20 7c01 7404 6a08  j.......n |.t.j.
-00000540: 6b02 724e 6700 6401 a201 7d02 7409 6a0a  k.rNg.d...}.t.j.
-00000550: 7c02 6402 6403 8d02 0100 6404 5300 7213  |.d.d.....d.S.r.
-00000560: 0000 0029 0b72 0600 0000 7210 0000 0072  ...).r....r....r
-00000570: 1800 0000 7219 0000 0072 0500 0000 721a  ....r....r....r.
-00000580: 0000 0072 0900 0000 da0a 6465 7073 556e  ...r......depsUn
-00000590: 5379 6e63 721b 0000 0072 0300 0000 721c  Syncr....r....r.
-000005a0: 0000 0072 1d00 0000 720d 0000 0072 0d00  ...r....r....r..
-000005b0: 0000 720e 0000 0072 1f00 0000 2500 0000  ..r....r....%...
-000005c0: 7310 0000 0000 0408 0108 0108 010a 010c  s...............
-000005d0: 010a 0108 017a 114d 6f64 756c 652e 6465  .....z.Module.de
-000005e0: 7073 556e 5379 6e63 6301 0000 0000 0000  psUnSyncc.......
-000005f0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00000600: 0073 1600 0000 7400 a001 a100 0100 7c00  .s....t.......|.
-00000610: 6a02 a003 a100 0100 6401 5300 2902 7548  j.......d.S.).uH
-00000620: 0000 000a 2020 2020 2020 2020 e689 93e5  ....        ....
-00000630: bc80 7673 636f 6465 efbc 8ce5 908c e697  ..vscode........
-00000640: b6e5 b086 e689 80e6 9c89 e6a8 a1e5 9d97  ................
-00000650: e6b7 bbe5 8aa0 e585 a576 7363 6f64 65e4  .........vscode.
-00000660: b8ad 0a20 2020 2020 2020 204e 2904 7206  ...        N).r.
-00000670: 0000 0072 1000 0000 720a 0000 005a 126f  ...r....r....Z.o
-00000680: 7065 6e46 6c75 7474 6572 5072 6f6a 6563  penFlutterProjec
-00000690: 7472 0b00 0000 720d 0000 0072 0d00 0000  tr....r....r....
-000006a0: 720e 0000 00da 046f 7065 6e32 0000 0073  r......open2...s
-000006b0: 0400 0000 0004 0801 7a0b 4d6f 6475 6c65  ........z.Module
-000006c0: 2e6f 7065 6e63 0100 0000 0000 0000 0000  .openc..........
-000006d0: 0000 0100 0000 0200 0000 4300 0000 7314  ..........C...s.
-000006e0: 0000 0074 00a0 01a1 0001 0074 02a0 03a1  ...t.......t....
-000006f0: 0001 0064 0153 0029 0275 3a00 0000 0a20  ...d.S.).u:.... 
-00000700: 2020 2020 2020 20e6 9bb4 e696 b0e5 ad98         .........
-00000710: e582 a8e9 a1b9 e79b ae67 6974 e4bf a1e6  .........git....
-00000720: 81af e79a 846a 736f 6ee6 9687 e4bb b60a  .....json.......
-00000730: 2020 2020 2020 2020 4e29 0472 0600 0000          N).r....
-00000740: 7210 0000 0072 0400 0000 5a12 7570 6461  r....r....Z.upda
-00000750: 7465 4d6f 6475 6c65 436f 6e66 6967 720b  teModuleConfigr.
-00000760: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000770: 0000 da0d 6d6f 6475 6c65 5f75 7064 6174  ....module_updat
-00000780: 6539 0000 0073 0400 0000 0004 0801 7a14  e9...s........z.
-00000790: 4d6f 6475 6c65 2e6d 6f64 756c 655f 7570  Module.module_up
-000007a0: 6461 7465 4e29 0ada 085f 5f6e 616d 655f  dateN)...__name_
-000007b0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000007c0: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-000007d0: 6f63 5f5f 720f 0000 0072 1200 0000 721e  oc__r....r....r.
-000007e0: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
-000007f0: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000800: 0072 0e00 0000 7208 0000 0008 0000 0073  .r....r........s
-00000810: 0e00 0000 0801 0404 0804 0807 080d 080d  ................
-00000820: 0807 7208 0000 004e 290c 5a1e 7464 665f  ..r....N).Z.tdf_
-00000830: 746f 6f6c 2e74 6f6f 6c73 2e63 6c69 2e70  tool.tools.cli.p
-00000840: 726f 6a65 6374 5f63 6c69 7202 0000 005a  roject_clir....Z
-00000850: 1274 6466 5f74 6f6f 6c2e 746f 6f6c 732e  .tdf_tool.tools.
-00000860: 636d 6472 0300 0000 5a1c 7464 665f 746f  cmdr....Z.tdf_to
-00000870: 6f6c 2e74 6f6f 6c73 2e63 6f6e 6669 672e  ol.tools.config.
-00000880: 636f 6e66 6967 7204 0000 005a 1874 6466  configr....Z.tdf
-00000890: 5f74 6f6f 6c2e 746f 6f6c 732e 7368 656c  _tool.tools.shel
-000008a0: 6c5f 6469 7272 0500 0000 7206 0000 005a  l_dirr....r....Z
-000008b0: 1c74 6466 5f74 6f6f 6c2e 746f 6f6c 732e  .tdf_tool.tools.
-000008c0: 7673 636f 6465 2e76 7363 6f64 6572 0700  vscode.vscoder..
-000008d0: 0000 7208 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-000008e0: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
-000008f0: 6475 6c65 3e01 0000 0073 0a00 0000 0c01  dule>....s......
-00000900: 0c01 0c01 1001 0c03                      ........
+00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
+00000060: 0100 4700 6405 6406 8400 6406 8302 5a09  ..G.d.d...d...Z.
+00000070: 6407 5300 2908 e900 0000 0029 02da 0b50  d.S.)......)...P
+00000080: 726f 6a65 6374 5479 7065 da08 5368 656c  rojectType..Shel
+00000090: 6c44 6972 2901 da15 466c 7574 7465 7254  lDir)...FlutterT
+000000a0: 7261 6e73 6c61 7465 546f 6f6c 7329 01da  ranslateTools)..
+000000b0: 0c69 4f53 5472 616e 736c 6174 6529 01da  .iOSTranslate)..
+000000c0: 0d54 7261 6e73 6c61 7465 4c69 6e74 6300  .TranslateLintc.
+000000d0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+000000e0: 0000 0040 0000 0073 3600 0000 6500 5a01  ...@...s6...e.Z.
+000000f0: 6400 5a02 6401 5a03 6402 6403 9c01 6404  d.Z.d.Z.d.d...d.
+00000100: 6405 8404 5a04 6406 6407 8400 5a05 6408  d...Z.d.d...Z.d.
+00000110: 6409 8400 5a06 640a 640b 8400 5a07 6402  d...Z.d.d...Z.d.
+00000120: 5300 290c da09 5472 616e 736c 6174 6575  S.)...Translateu
+00000130: 3800 0000 0a20 2020 20e5 9bbd e999 85e5  8....    .......
+00000140: 8c96 e79b b8e5 85b3 efbc 9a74 6c20 7472  ...........tl tr
+00000150: 616e 736c 6174 6520 2d68 20e6 9fa5 e79c  anslate -h .....
+00000160: 8be8 afa6 e683 850a 2020 2020 4e29 01da  ........    N)..
+00000170: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
+00000180: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000190: 730c 0000 0074 0083 007c 005f 0164 0053  s....t...|._.d.S
+000001a0: 0029 014e 2902 7206 0000 00da 046c 696e  .).N).r......lin
+000001b0: 7429 01da 0473 656c 66a9 0072 0b00 0000  t)...self..r....
+000001c0: f568 0000 002f 5573 6572 732f 7875 6a69  .h.../Users/xuji
+000001d0: 616e 2f44 6f63 756d 656e 7473 2f32 3032  an/Documents/202
+000001e0: 342f e6a8 a1e5 9d97 e997 b4e4 baa4 e4ba  4/..............
+000001f0: 92e9 a1b9 e79b ae74 6ce5 8d87 e7ba a72f  .......tl....../
+00000200: 7061 636b 6167 655f 746f 6f6c 732f 7464  package_tools/td
+00000210: 665f 746f 6f6c 2f70 6970 656c 696e 6573  f_tool/pipelines
+00000220: 2f74 7261 6e73 6c61 7465 2e70 79da 085f  /translate.py.._
+00000230: 5f69 6e69 745f 5f0c 0000 0073 0200 0000  _init__....s....
+00000240: 0001 7a12 5472 616e 736c 6174 652e 5f5f  ..z.Translate.__
+00000250: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00000260: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00000270: 3e00 0000 7400 a001 a100 0100 7400 a002  >...t.......t...
+00000280: a100 7d01 7c01 7403 6a04 6b02 7226 7405  ..}.|.t.j.k.r&t.
+00000290: 8300 a006 a100 0100 6e14 7c01 7403 6a07  ........n.|.t.j.
+000002a0: 6b02 723a 7408 8300 a006 a100 0100 6401  k.r:t.........d.
+000002b0: 5300 2902 754b 0000 000a 2020 2020 2020  S.).uK....      
+000002c0: 2020 e59b bde9 9985 e58c 96e7 9bb8 e585    ..............
+000002d0: b3ef bc9a e980 9ae8 bf87 e4ba a4e4 ba92  ................
+000002e0: e5bc 8fe7 9a84 e696 b9e5 bc8f e5a4 84e7  ................
+000002f0: 9086 e59b bde9 9985 e58c 960a 2020 2020  ............    
+00000300: 2020 2020 4e29 0972 0300 0000 da0c 676f      N).r......go
+00000310: 496e 5368 656c 6c44 6972 da0e 6765 7450  InShellDir..getP
+00000320: 726f 6a65 6374 5479 7065 7202 0000 00da  rojectTyper.....
+00000330: 0746 4c55 5454 4552 7204 0000 00da 0974  .FLUTTERr......t
+00000340: 7261 6e73 6c61 7465 da03 494f 5372 0500  ranslate..IOSr..
+00000350: 0000 a902 720a 0000 00da 0b70 726f 6a65  ....r......proje
+00000360: 6374 5479 7065 720b 0000 0072 0b00 0000  ctTyper....r....
+00000370: 720c 0000 00da 0573 7461 7274 0f00 0000  r......start....
+00000380: 730c 0000 0000 0408 0108 010a 010c 010a  s...............
+00000390: 017a 0f54 7261 6e73 6c61 7465 2e73 7461  .z.Translate.sta
+000003a0: 7274 6302 0000 0000 0000 0000 0000 0003  rtc.............
+000003b0: 0000 0003 0000 0043 0000 0073 4a00 0000  .......C...sJ...
+000003c0: 7400 a001 a100 0100 7400 a002 a100 7d02  t.......t.....}.
+000003d0: 7c02 7403 6a04 6b02 7228 7405 8300 a006  |.t.j.k.r(t.....
+000003e0: 7c01 a101 0100 6e16 7c02 7403 6a07 6b02  |.....n.|.t.j.k.
+000003f0: 723e 7408 8300 a006 7c01 a101 0100 7409  r>t.....|.....t.
+00000400: 6401 8301 0100 6402 5300 2903 753f 0000  d.....d.S.).u?..
+00000410: 000a 2020 2020 2020 2020 e59b bde9 9985  ..        ......
+00000420: e58c 96e7 9bb8 e585 b3ef bc9a e68c 87e5  ................
+00000430: ae9a e6a8 a1e5 9d97 e8bf 9be8 a18c e59b  ................
+00000440: bde9 9985 e58c 960a 2020 2020 2020 2020  ........        
+00000450: 7201 0000 004e 290a 7203 0000 0072 0e00  r....N).r....r..
+00000460: 0000 720f 0000 0072 0200 0000 7210 0000  ..r....r....r...
+00000470: 0072 0400 0000 5a10 7472 616e 736c 6174  .r....Z.translat
+00000480: 655f 6d6f 6475 6c65 7212 0000 0072 0500  e_moduler....r..
+00000490: 0000 da04 6578 6974 2903 720a 0000 00da  ....exit).r.....
+000004a0: 046e 616d 6572 1400 0000 720b 0000 0072  .namer....r....r
+000004b0: 0b00 0000 720c 0000 00da 066d 6f64 756c  ....r......modul
+000004c0: 651a 0000 0073 0e00 0000 0004 0801 0801  e....s..........
+000004d0: 0a01 0e01 0a01 0c01 7a10 5472 616e 736c  ........z.Transl
+000004e0: 6174 652e 6d6f 6475 6c65 6301 0000 0000  ate.modulec.....
+000004f0: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00000500: 0000 0073 4600 0000 7400 a001 a100 0100  ...sF...t.......
+00000510: 7400 a002 a100 7d01 7c01 7403 6a04 6b02  t.....}.|.t.j.k.
+00000520: 7226 7405 8300 a006 a100 0100 6e14 7c01  r&t.........n.|.
+00000530: 7403 6a07 6b02 723a 7408 8300 a006 a100  t.j.k.r:t.......
+00000540: 0100 7409 6401 8301 0100 6402 5300 2903  ..t.d.....d.S.).
+00000550: 757e 0000 000a 2020 2020 2020 2020 e59b  u~....        ..
+00000560: bde9 9985 e58c 96e7 9bb8 e585 b3ef bc9a  ................
+00000570: e695 b4e5 9088 e689 80e6 9c89 e7bb 84e4  ................
+00000580: bbb6 e79a 84e5 9bbd e999 85e5 8c96 e696  ................
+00000590: 87e4 bbb6 e588 b0e4 b880 e4b8 aae6 9687  ................
+000005a0: e4bb b6e4 b8ad efbc 8ce7 94a8 e69d a5e7  ................
+000005b0: bbb4 e68a a4e4 b880 e4bb bde5 9bbd e999  ................
+000005c0: 85e5 8c96 e696 87e4 bbb6 0a20 2020 2020  ...........     
+000005d0: 2020 2072 0100 0000 4e29 0a72 0300 0000     r....N).r....
+000005e0: 720e 0000 0072 0f00 0000 7202 0000 0072  r....r....r....r
+000005f0: 1000 0000 7204 0000 00da 0969 6e74 6567  ....r......integ
+00000600: 7261 7465 7212 0000 0072 0500 0000 7216  rater....r....r.
+00000610: 0000 0072 1300 0000 720b 0000 0072 0b00  ...r....r....r..
+00000620: 0000 720c 0000 0072 1900 0000 2600 0000  ..r....r....&...
+00000630: 730e 0000 0000 0408 0108 010a 010c 010a  s...............
+00000640: 010a 017a 1354 7261 6e73 6c61 7465 2e69  ...z.Translate.i
+00000650: 6e74 6567 7261 7465 2908 da08 5f5f 6e61  ntegrate)...__na
+00000660: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000670: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000680: 5f5f 646f 635f 5f72 0d00 0000 7215 0000  __doc__r....r...
+00000690: 0072 1800 0000 7219 0000 0072 0b00 0000  .r....r....r....
+000006a0: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+000006b0: 0700 0000 0700 0000 730a 0000 0008 0104  ........s.......
+000006c0: 040e 0308 0b08 0c72 0700 0000 4e29 0ada  .......r....N)..
+000006d0: 1874 6466 5f74 6f6f 6c2e 746f 6f6c 732e  .tdf_tool.tools.
+000006e0: 7368 656c 6c5f 6469 7272 0200 0000 7203  shell_dirr....r.
+000006f0: 0000 005a 3874 6466 5f74 6f6f 6c2e 746f  ...Z8tdf_tool.to
+00000700: 6f6c 732e 7472 616e 736c 6174 652e 666c  ols.translate.fl
+00000710: 7574 7465 722e 666c 7574 7465 725f 7472  utter.flutter_tr
+00000720: 616e 736c 6174 655f 746f 6f6c 7372 0400  anslate_toolsr..
+00000730: 0000 5a2a 7464 665f 746f 6f6c 2e74 6f6f  ..Z*tdf_tool.too
+00000740: 6c73 2e74 7261 6e73 6c61 7465 2e69 6f73  ls.translate.ios
+00000750: 2e69 6f73 5f74 7261 6e73 6c61 7465 7205  .ios_translater.
+00000760: 0000 005a 2774 6466 5f74 6f6f 6c2e 746f  ...Z'tdf_tool.to
+00000770: 6f6c 732e 7472 616e 736c 6174 652e 7472  ols.translate.tr
+00000780: 616e 736c 6174 655f 6c69 6e74 7206 0000  anslate_lintr...
+00000790: 0072 0700 0000 720b 0000 0072 0b00 0000  .r....r....r....
+000007a0: 720b 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
+000007b0: 756c 653e 0100 0000 7308 0000 0010 010c  ule>....s.......
+000007c0: 010c 010c 03                             .....
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 16 07:59:17 2024 UTC, .py size: 1634 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d52f 1e66 6206 0000  a......../.fb...
+00000000: 610d 0d0a 0000 0000 f1e4 2066 5e06 0000  a......... f^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6406 6407 8400 6407 8302 5a0b 6401 5300  d.d...d...Z.d.S.
@@ -33,109 +33,109 @@
 00000200: bbb4 e695 b0e7 bb84 e5bd a2e5 bc8f e8be  ................
 00000210: 93e5 87ba e6a8 a1e5 9d97 e79a 84e4 be9d  ................
 00000220: e8b5 96e9 a1ba e5ba 8fef bc8c e6af 8fe4  ................
 00000230: b880 6974 656d e588 97e8 a1a8 e4bb a3e8  ..item..........
 00000240: a1a8 e58f afe5 908c e697 b6e6 8993 7461  ..............ta
 00000250: 67e7 9a84 e6a8 a1e5 9d97 0a20 2020 2020  g..........     
 00000260: 2020 2072 0100 0000 4e29 0672 0700 0000     r....N).r....
-00000270: da0d 6469 7249 6e76 616c 6964 6174 6572  ..dirInvalidater
-00000280: 0200 0000 da08 6765 6e65 7261 7465 da05  ......generate..
-00000290: 7072 696e 74da 0465 7869 7429 02da 0473  print..exit)...s
-000002a0: 656c 66da 046a 736f 6ea9 0072 0f00 0000  elf..json..r....
-000002b0: f566 0000 002f 5573 6572 732f 7875 6a69  .f.../Users/xuji
-000002c0: 616e 2f44 6f63 756d 656e 7473 2f32 3032  an/Documents/202
-000002d0: 342f e6a8 a1e5 9d97 e997 b4e4 baa4 e4ba  4/..............
-000002e0: 92e9 a1b9 e79b ae74 6ce5 8d87 e7ba a72f  .......tl....../
-000002f0: 7061 636b 6167 655f 746f 6f6c 732f 7464  package_tools/td
-00000300: 665f 746f 6f6c 2f70 6970 656c 696e 6573  f_tool/pipelines
-00000310: 2f70 6163 6b61 6765 2e70 79da 036d 6170  /package.py..map
-00000320: 1100 0000 7308 0000 0000 0408 010a 0108  ....s...........
-00000330: 017a 0b50 6163 6b61 6765 2e6d 6170 6301  .z.Package.mapc.
-00000340: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000350: 0000 0043 0000 0073 1200 0000 7400 a001  ...C...s....t...
-00000360: a100 0100 7402 8300 0100 6401 5300 2902  ....t.....d.S.).
-00000370: 753d 0100 000a 2020 2020 2020 2020 746c  u=....        tl
-00000380: 2070 6163 6b61 6765 2074 6167 496e 666f   package tagInfo
-00000390: efbc 9ae8 be93 e587 bae4 b880 e4b8 aa6a  ...............j
-000003a0: 736f 6eef bc8c e6af 8fe4 b880 e88a 82e7  son.............
-000003b0: 82b9 e58c 85e5 90ab e4b8 80e4 b8aa e6a8  ................
-000003c0: a1e5 9d97 efbc 8c0a 2020 2020 2020 2020  ........        
-000003d0: e586 85e9 83a8 e58c 85e5 90ab efbc 9a72  ...............r
-000003e0: 656d 6f74 65ef bc9a e8bf 9ce7 a88b e69c  emote...........
-000003f0: 80e6 96b0 e789 88e6 9cac e58f b7ef bc9b  ................
-00000400: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
-00000410: efbc 9ae6 a8a1 e59d 97e5 8685 e985 8de7  ................
-00000420: bdae e79a 84e7 8988 e69c ace5 8fb7 efbc  ................
-00000430: 9b0a 2020 2020 2020 2020 7570 6772 6164  ..        upgrad
-00000440: 65ef bc9a e5af b9e6 af94 e887 aae5 a29e  e...............
-00000450: e590 8ee7 9a84 e789 88e6 9cac e58f b7ef  ................
-00000460: bc9b 0a20 2020 2020 2020 2073 6f72 74ef  ...        sort.
-00000470: bc9a e6a8 a1e5 9d97 e689 9374 6167 e9a1  ...........tag..
-00000480: bae5 ba8f efbc 8c73 6f72 74e7 9bb8 e590  .......sort.....
-00000490: 8ce5 8db3 e4bb a3e8 a1a8 e58f afe5 908c  ................
-000004a0: e697 b6e6 8993 7461 670a 2020 2020 2020  ......tag.      
-000004b0: 2020 4e29 0372 0700 0000 7209 0000 0072    N).r....r....r
-000004c0: 0500 0000 2901 720d 0000 0072 0f00 0000  ....).r....r....
-000004d0: 720f 0000 0072 1000 0000 da07 7461 6749  r....r......tagI
-000004e0: 6e66 6f1a 0000 0073 0400 0000 0008 0801  nfo....s........
-000004f0: 7a0f 5061 636b 6167 652e 7461 6749 6e66  z.Package.tagInf
-00000500: 6f29 01da 086a 736f 6e44 6174 6163 0200  o)...jsonDatac..
-00000510: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000520: 0000 4300 0000 7314 0000 0074 00a0 01a1  ..C...s....t....
-00000530: 0001 0074 027c 0183 0101 0064 0153 0029  ...t.|.....d.S.)
-00000540: 0275 9e00 0000 0a20 2020 2020 2020 2074  .u.....        t
-00000550: 6c20 7061 636b 6167 6520 7072 6570 6172  l package prepar
-00000560: 6554 6167 5461 736b efbc 9ae4 bfae e694  eTagTask........
-00000570: b979 616d 6ce4 b8ad e79a 8474 6167 e58f  .yaml......tag..
-00000580: b7e5 928c e689 80e6 9c89 e79a 84e4 be9d  ................
-00000590: e8b5 96ef bc8c e8af a5e5 91bd e4bb a4e5  ................
-000005a0: 8faf e79c 8be6 8890 e698 afe5 819a e689  ................
-000005b0: 9374 6167 e589 8de7 9a84 e587 86e5 a487  .tag............
-000005c0: e5b7 a5e4 bd9c efbc 8ce6 8a8a e4be 9de8  ................
-000005d0: b596 e8a7 84e8 8c83 e58c 960a 2020 2020  ............    
-000005e0: 2020 2020 4e29 0372 0700 0000 7209 0000      N).r....r...
-000005f0: 0072 0300 0000 2902 720d 0000 0072 1300  .r....).r....r..
-00000600: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000610: 00da 0e70 7265 7061 7265 5461 6754 6173  ...prepareTagTas
-00000620: 6b25 0000 0073 0400 0000 0004 0801 7a16  k%...s........z.
-00000630: 5061 636b 6167 652e 7072 6570 6172 6554  Package.prepareT
-00000640: 6167 5461 736b 2901 da07 6d6f 6475 6c65  agTask)...module
-00000650: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
-00000660: 0000 0400 0000 4300 0000 731a 0000 0074  ......C...s....t
-00000670: 00a0 01a1 0001 0074 027c 01a0 0364 01a1  .......t.|...d..
-00000680: 0183 0101 0064 0253 0029 0375 8500 0000  .....d.S.).u....
-00000690: 0a20 2020 2020 2020 2074 6c20 7061 636b  .        tl pack
-000006a0: 6167 6520 7461 67ef bc9a e689 b9e9 878f  age tag.........
-000006b0: 7461 67e6 938d e4bd 9cef bc8c e58f 82e6  tag.............
-000006c0: 95b0 e980 9ae8 bf87 e980 97e5 8fb7 e99a  ................
-000006d0: 94e5 bc80 efbc 8ce4 b88d e8a6 81e6 9c89  ................
-000006e0: e7a9 bae6 a0bc e380 82e5 a682 7464 665f  ............tdf_
-000006f0: 746f 6f6c 2070 6163 6b61 6765 2074 6167  tool package tag
-00000700: 2074 6466 5f77 6964 6765 7473 0a20 2020   tdf_widgets.   
-00000710: 2020 2020 20fa 012c 4e29 0472 0700 0000       ..,N).r....
-00000720: 7209 0000 0072 0400 0000 da05 7370 6c69  r....r......spli
-00000730: 7429 0272 0d00 0000 7215 0000 0072 0f00  t).r....r....r..
-00000740: 0000 720f 0000 0072 1000 0000 da03 7461  ..r....r......ta
-00000750: 672c 0000 0073 0400 0000 0004 0801 7a0b  g,...s........z.
-00000760: 5061 636b 6167 652e 7461 674e 2909 da08  Package.tagN)...
-00000770: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000780: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000790: 5f5f da07 5f5f 646f 635f 5f72 1100 0000  __..__doc__r....
-000007a0: 7212 0000 00da 0373 7472 7214 0000 0072  r......strr....r
-000007b0: 1800 0000 720f 0000 0072 0f00 0000 720f  ....r....r....r.
-000007c0: 0000 0072 1000 0000 7208 0000 000c 0000  ...r....r.......
-000007d0: 0073 0a00 0000 0801 0404 0809 080b 0e07  .s..............
-000007e0: 7208 0000 0029 0cda 026f 73da 2474 6466  r....)...os.$tdf
-000007f0: 5f74 6f6f 6c2e 746f 6f6c 732e 6465 7065  _tool.tools.depe
-00000800: 6e64 656e 6369 6573 5f61 6e61 6c79 7369  ndencies_analysi
-00000810: 7372 0200 0000 5a2d 7464 665f 746f 6f6c  sr....Z-tdf_tool
-00000820: 2e74 6f6f 6c73 2e70 6163 6b61 6765 2e73  .tools.package.s
-00000830: 6561 6c5f 6f66 665f 7061 636b 6167 655f  eal_off_package_
-00000840: 7574 696c 7372 0300 0000 7204 0000 0072  utilsr....r....r
-00000850: 0500 0000 da14 7464 665f 746f 6f6c 2e74  ......tdf_tool.t
-00000860: 6f6f 6c73 2e70 7269 6e74 7206 0000 00da  ools.printr.....
-00000870: 1874 6466 5f74 6f6f 6c2e 746f 6f6c 732e  .tdf_tool.tools.
-00000880: 7368 656c 6c5f 6469 7272 0700 0000 7208  shell_dirr....r.
-00000890: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
-000008a0: 0000 7210 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-000008b0: 3e01 0000 0073 0a00 0000 0801 0c01 1405  >....s..........
-000008c0: 0c01 0c03                                ....
+00000270: da0c 676f 496e 5368 656c 6c44 6972 7202  ..goInShellDirr.
+00000280: 0000 00da 0867 656e 6572 6174 65da 0570  .....generate..p
+00000290: 7269 6e74 da04 6578 6974 2902 da04 7365  rint..exit)...se
+000002a0: 6c66 da04 6a73 6f6e a900 720f 0000 00f5  lf..json..r.....
+000002b0: 6600 0000 2f55 7365 7273 2f78 756a 6961  f.../Users/xujia
+000002c0: 6e2f 446f 6375 6d65 6e74 732f 3230 3234  n/Documents/2024
+000002d0: 2fe6 a8a1 e59d 97e9 97b4 e4ba a4e4 ba92  /...............
+000002e0: e9a1 b9e7 9bae 746c e58d 87e7 baa7 2f70  ......tl....../p
+000002f0: 6163 6b61 6765 5f74 6f6f 6c73 2f74 6466  ackage_tools/tdf
+00000300: 5f74 6f6f 6c2f 7069 7065 6c69 6e65 732f  _tool/pipelines/
+00000310: 7061 636b 6167 652e 7079 da03 6d61 7011  package.py..map.
+00000320: 0000 0073 0800 0000 0004 0801 0a01 0801  ...s............
+00000330: 7a0b 5061 636b 6167 652e 6d61 7063 0100  z.Package.mapc..
+00000340: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000350: 0000 4300 0000 7312 0000 0074 00a0 01a1  ..C...s....t....
+00000360: 0001 0074 0283 0001 0064 0153 0029 0275  ...t.....d.S.).u
+00000370: 3d01 0000 0a20 2020 2020 2020 2074 6c20  =....        tl 
+00000380: 7061 636b 6167 6520 7461 6749 6e66 6fef  package tagInfo.
+00000390: bc9a e8be 93e5 87ba e4b8 80e4 b8aa 6a73  ..............js
+000003a0: 6f6e efbc 8ce6 af8f e4b8 80e8 8a82 e782  on..............
+000003b0: b9e5 8c85 e590 abe4 b880 e4b8 aae6 a8a1  ................
+000003c0: e59d 97ef bc8c 0a20 2020 2020 2020 20e5  .......        .
+000003d0: 8685 e983 a8e5 8c85 e590 abef bc9a 7265  ..............re
+000003e0: 6d6f 7465 efbc 9ae8 bf9c e7a8 8be6 9c80  mote............
+000003f0: e696 b0e7 8988 e69c ace5 8fb7 efbc 9b0a  ................
+00000400: 2020 2020 2020 2020 6375 7272 656e 74ef          current.
+00000410: bc9a e6a8 a1e5 9d97 e586 85e9 858d e7bd  ................
+00000420: aee7 9a84 e789 88e6 9cac e58f b7ef bc9b  ................
+00000430: 0a20 2020 2020 2020 2075 7067 7261 6465  .        upgrade
+00000440: efbc 9ae5 afb9 e6af 94e8 87aa e5a2 9ee5  ................
+00000450: 908e e79a 84e7 8988 e69c ace5 8fb7 efbc  ................
+00000460: 9b0a 2020 2020 2020 2020 736f 7274 efbc  ..        sort..
+00000470: 9ae6 a8a1 e59d 97e6 8993 7461 67e9 a1ba  ..........tag...
+00000480: e5ba 8fef bc8c 736f 7274 e79b b8e5 908c  ......sort......
+00000490: e58d b3e4 bba3 e8a1 a8e5 8faf e590 8ce6  ................
+000004a0: 97b6 e689 9374 6167 0a20 2020 2020 2020  .....tag.       
+000004b0: 204e 2903 7207 0000 0072 0900 0000 7205   N).r....r....r.
+000004c0: 0000 0029 0172 0d00 0000 720f 0000 0072  ...).r....r....r
+000004d0: 0f00 0000 7210 0000 00da 0774 6167 496e  ....r......tagIn
+000004e0: 666f 1a00 0000 7304 0000 0000 0808 017a  fo....s........z
+000004f0: 0f50 6163 6b61 6765 2e74 6167 496e 666f  .Package.tagInfo
+00000500: 2901 da08 6a73 6f6e 4461 7461 6302 0000  )...jsonDatac...
+00000510: 0000 0000 0000 0000 0002 0000 0002 0000  ................
+00000520: 0043 0000 0073 1400 0000 7400 a001 a100  .C...s....t.....
+00000530: 0100 7402 7c01 8301 0100 6401 5300 2902  ..t.|.....d.S.).
+00000540: 759e 0000 000a 2020 2020 2020 2020 746c  u.....        tl
+00000550: 2070 6163 6b61 6765 2070 7265 7061 7265   package prepare
+00000560: 5461 6754 6173 6bef bc9a e4bf aee6 94b9  TagTask.........
+00000570: 7961 6d6c e4b8 ade7 9a84 7461 67e5 8fb7  yaml......tag...
+00000580: e592 8ce6 8980 e69c 89e7 9a84 e4be 9de8  ................
+00000590: b596 efbc 8ce8 afa5 e591 bde4 bba4 e58f  ................
+000005a0: afe7 9c8b e688 90e6 98af e581 9ae6 8993  ................
+000005b0: 7461 67e5 898d e79a 84e5 8786 e5a4 87e5  tag.............
+000005c0: b7a5 e4bd 9cef bc8c e68a 8ae4 be9d e8b5  ................
+000005d0: 96e8 a784 e88c 83e5 8c96 0a20 2020 2020  ...........     
+000005e0: 2020 204e 2903 7207 0000 0072 0900 0000     N).r....r....
+000005f0: 7203 0000 0029 0272 0d00 0000 7213 0000  r....).r....r...
+00000600: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
+00000610: da0e 7072 6570 6172 6554 6167 5461 736b  ..prepareTagTask
+00000620: 2500 0000 7304 0000 0000 0408 017a 1650  %...s........z.P
+00000630: 6163 6b61 6765 2e70 7265 7061 7265 5461  ackage.prepareTa
+00000640: 6754 6173 6b29 01da 076d 6f64 756c 6573  gTask)...modules
+00000650: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000660: 0004 0000 0043 0000 0073 1a00 0000 7400  .....C...s....t.
+00000670: a001 a100 0100 7402 7c01 a003 6401 a101  ......t.|...d...
+00000680: 8301 0100 6402 5300 2903 7585 0000 000a  ....d.S.).u.....
+00000690: 2020 2020 2020 2020 746c 2070 6163 6b61          tl packa
+000006a0: 6765 2074 6167 efbc 9ae6 89b9 e987 8f74  ge tag.........t
+000006b0: 6167 e693 8de4 bd9c efbc 8ce5 8f82 e695  ag..............
+000006c0: b0e9 809a e8bf 87e9 8097 e58f b7e9 9a94  ................
+000006d0: e5bc 80ef bc8c e4b8 8de8 a681 e69c 89e7  ................
+000006e0: a9ba e6a0 bce3 8082 e5a6 8274 6466 5f74  ...........tdf_t
+000006f0: 6f6f 6c20 7061 636b 6167 6520 7461 6720  ool package tag 
+00000700: 7464 665f 7769 6467 6574 730a 2020 2020  tdf_widgets.    
+00000710: 2020 2020 fa01 2c4e 2904 7207 0000 0072      ..,N).r....r
+00000720: 0900 0000 7204 0000 00da 0573 706c 6974  ....r......split
+00000730: 2902 720d 0000 0072 1500 0000 720f 0000  ).r....r....r...
+00000740: 0072 0f00 0000 7210 0000 00da 0374 6167  .r....r......tag
+00000750: 2c00 0000 7304 0000 0000 0408 017a 0b50  ,...s........z.P
+00000760: 6163 6b61 6765 2e74 6167 4e29 09da 085f  ackage.tagN)..._
+00000770: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000780: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000790: 5fda 075f 5f64 6f63 5f5f 7211 0000 0072  _..__doc__r....r
+000007a0: 1200 0000 da03 7374 7272 1400 0000 7218  ......strr....r.
+000007b0: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
+000007c0: 0000 7210 0000 0072 0800 0000 0c00 0000  ..r....r........
+000007d0: 730a 0000 0008 0104 0408 0908 0b0e 0772  s..............r
+000007e0: 0800 0000 290c da02 6f73 da24 7464 665f  ....)...os.$tdf_
+000007f0: 746f 6f6c 2e74 6f6f 6c73 2e64 6570 656e  tool.tools.depen
+00000800: 6465 6e63 6965 735f 616e 616c 7973 6973  dencies_analysis
+00000810: 7202 0000 005a 2d74 6466 5f74 6f6f 6c2e  r....Z-tdf_tool.
+00000820: 746f 6f6c 732e 7061 636b 6167 652e 7365  tools.package.se
+00000830: 616c 5f6f 6666 5f70 6163 6b61 6765 5f75  al_off_package_u
+00000840: 7469 6c73 7203 0000 0072 0400 0000 7205  tilsr....r....r.
+00000850: 0000 00da 1474 6466 5f74 6f6f 6c2e 746f  .....tdf_tool.to
+00000860: 6f6c 732e 7072 696e 7472 0600 0000 da18  ols.printr......
+00000870: 7464 665f 746f 6f6c 2e74 6f6f 6c73 2e73  tdf_tool.tools.s
+00000880: 6865 6c6c 5f64 6972 7207 0000 0072 0800  hell_dirr....r..
+00000890: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+000008a0: 0072 1000 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000008b0: 0100 0000 730a 0000 0008 010c 0114 050c  ....s...........
+000008c0: 010c 03                                  ...
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/annotation.py` & `tdf_tool-2.4.5/tdf_tool/pipelines/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,25 @@
     """
     模块间支持相关命令：tl annotation -h 查看详情
     """
 
     def __init__(self):
         Print.title("检测中...")
         self.__buildRunnerName: str = "build_runner" # build_runner库名
-        ShellDir.dirInvalidate()
+
         self.__routerAnnotation: Router = Router()
         self.__apiAnnotation: ApiAnnotation = ApiAnnotation()
         self.__businessModuleList = self.__api_businessModuleList()
         self.__packagesList: list[PackageNode] = PackagesJsonConfig(ShellDir.getShellDir()).packages # 壳依赖的所有库
 
     def start(self):
         """
         tl annotation start：会以交互式进行操作，对指定的模块执行描述文件(包括路由，api交互)生成和自动注册逻辑
         """
+        ShellDir.goInShellDir()
         
         Print.str("检测到以下模块可生成描述文件：\n")
         for index, item in enumerate(self.__businessModuleList):
             print(f"{index}: {item}")
         print()
         while True:
             module_name = input("请输入需要生成描述文件的模块名或其下标(input ! 退出，all 自动注册)：")
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/api_interaction.py` & `tdf_tool-2.4.5/tdf_tool/pipelines/api_interaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         self.__implNodeList: list[ImplNode] = []  # impl描述文件列表
         self.__apiSuffix: str = ".tdf_api.dart"  # 交互api描述文件后缀
         self.__apiNodeList: list[ApiNode] = []  # api描述文件列表
         self.__interactionDir: str = "tdf_api"  # 交互文件目录
         self.__annotationName: str = "tdf_module_api_anno"  # 注解库名
         self.__packagesList: list[PackageNode] = []  # 壳依赖的所有库
 
-        ShellDir.dirInvalidate()
         self.fetch_packages_list()
 
     # 遍历壳应用.packages下的所有package,将所有tdf开头的模块都添加入packagesList中
     def fetch_packages_list(self):
         ShellDir.goInShellDir()
         # 遍历壳应用的所有package,将所有tdf开头的模块都添加入packagesList中
         self.__packagesList = PackagesJsonConfig(os.getcwd()).packages
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/fix_header.py` & `tdf_tool-2.4.5/tdf_tool/pipelines/fix_header.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,24 @@
         self.lint = FixHeaderLint()
         self.__fix_entry = FixHeaderEntry(FixHeaderType.REPLACE)
 
     def start(self):
         """
         tl fixHeader start，会以交互式进行进行头文件修复
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         projectType = ShellDir.getProjectType()
         if projectType == ProjectType.FLUTTER:
             Print.error("tl fixHeader 只支持iOS")
         elif projectType == ProjectType.IOS:
             self.__fix_entry.start()
 
     def module(self, name: str):
         """
         tl fixHeader module【模块名】，修复指定模块名
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         projectType = ShellDir.getProjectType()
         if projectType == ProjectType.FLUTTER:
             Print.error("tl fixHeader 只支持iOS")
         elif projectType == ProjectType.IOS:
             self.__fix_entry.module(name)
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/git.py` & `tdf_tool-2.4.5/tdf_tool/pipelines/git.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """
 
     def __init__(self, arg: list):
         self.__gitArg = ["git"] + arg
         self.__arg = arg
 
     def run(self):
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         self.__batch_run_git()
 
     def __batch_run_git(self):
         ShellDir.goInShellDir()
         projectType = ShellDir.getProjectType()
         if projectType == ProjectType.FLUTTER:
             Print.title("开始操作壳：" + " ".join(self.__gitArg))
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/module.py` & `tdf_tool-2.4.5/tdf_tool/pipelines/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,42 +7,41 @@
 
 class Module:
     """
     模块相关工具： tl module -h 查看详情
     """
 
     def __init__(self):
+        ShellDir.goInShellDir()
         self.__cli = ProjectCLI()
         self.__vscodeManager = VsCodeManager()
 
     def init(self):
         """
         项目初始化
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         self.__cli.initial()
 
     def deps(self):
         """
         修改initial_config.json文件后，执行该命令，更新依赖
         """
-        ShellDir.dirInvalidate()
         ShellDir.goInShellDir()
         projectType = ShellDir.getProjectType()
         if projectType == ProjectType.FLUTTER:
             self.__cli.cliDeps()
         elif projectType == ProjectType.IOS:
             ios_arg = ["bundle", "exec", "pod", "bin", "batch", "clone"]
             Cmd.runAndPrint(ios_arg, shell=False)
     
     def depsUnSync(self):
         """
         修改initial_config.json文件后，执行该命令，更新依赖
         """
-        ShellDir.dirInvalidate()
         ShellDir.goInShellDir()
         projectType = ShellDir.getProjectType()
         if projectType == ProjectType.FLUTTER:
             self.__cli.depsUnSync()
         elif projectType == ProjectType.IOS:
             ios_arg = ["bundle", "exec", "pod", "bin", "batch", "clone"]
             Cmd.runAndPrint(ios_arg, shell=False)
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/package.py` & `tdf_tool-2.4.5/tdf_tool/pipelines/package.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,36 +14,36 @@
     封包工具相关：tl package -h 查看详情
     """
 
     def map(self):
         """
         tl package map：以二维数组形式输出模块的依赖顺序，每一item列表代表可同时打tag的模块
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         json = DependencyAnalysis().generate()
         print(json)
         exit(0)
 
     def tagInfo(self):
         """
         tl package tagInfo：输出一个json，每一节点包含一个模块，
         内部包含：remote：远程最新版本号；
         current：模块内配置的版本号；
         upgrade：对比自增后的版本号；
         sort：模块打tag顺序，sort相同即代表可同时打tag
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         tagInfoObj()
 
     def prepareTagTask(self, jsonData: str):
         """
         tl package prepareTagTask：修改yaml中的tag号和所有的依赖，该命令可看成是做打tag前的准备工作，把依赖规范化
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         changeVersionAndDependencies(jsonData)
 
     def tag(self, modules: str):
         """
         tl package tag：批量tag操作，参数通过逗号隔开，不要有空格。如tdf_tool package tag tdf_widgets
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         createAndPushTag(modules.split(","))
```

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/router.py` & `tdf_tool-2.4.5/tdf_tool/pipelines/router.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/pipelines/translate.py` & `tdf_tool-2.4.5/tdf_tool/pipelines/translate.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,37 +12,37 @@
     def __init__(self) -> None:
         self.lint = TranslateLint()
 
     def start(self):
         """
         国际化相关：通过交互式的方式处理国际化
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         projectType = ShellDir.getProjectType()
         if projectType == ProjectType.FLUTTER:
             FlutterTranslateTools().translate()
         elif projectType == ProjectType.IOS:
             iOSTranslate().translate()
 
     def module(self, name):
         """
         国际化相关：指定模块进行国际化
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         projectType = ShellDir.getProjectType()
         if projectType == ProjectType.FLUTTER:
             FlutterTranslateTools().translate_module(name)
         elif projectType == ProjectType.IOS:
             iOSTranslate().translate_module(name)
         exit(0)
 
     def integrate(self):
         """
         国际化相关：整合所有组件的国际化文件到一个文件中，用来维护一份国际化文件
         """
-        ShellDir.dirInvalidate()
+        ShellDir.goInShellDir()
         projectType = ShellDir.getProjectType()
         if projectType == ProjectType.FLUTTER:
             FlutterTranslateTools().integrate()
         elif projectType == ProjectType.IOS:
             iOSTranslate().integrate()
         exit(0)
```

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/env.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/env.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/env.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/env.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/print.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/print.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/print.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/print.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/bean/deps_item.py` & `tdf_tool-2.4.5/tdf_tool/tools/cli/bean/deps_item.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/module_deps_rewrite.py` & `tdf_tool-2.4.5/tdf_tool/tools/cli/module_deps_rewrite.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/project_cli.py` & `tdf_tool-2.4.5/tdf_tool/tools/cli/project_cli.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cli/utils/yaml_utils.py` & `tdf_tool-2.4.5/tdf_tool/tools/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/cmd.py` & `tdf_tool-2.4.5/tdf_tool/tools/cmd.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/config.py` & `tdf_tool-2.4.5/tdf_tool/tools/config/config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/initial_json_config.py` & `tdf_tool-2.4.5/tdf_tool/tools/config/initial_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/module_json_config.py` & `tdf_tool-2.4.5/tdf_tool/tools/config/module_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/config/packages_config.py` & `tdf_tool-2.4.5/tdf_tool/tools/config/packages_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/dependencies_analysis.py` & `tdf_tool-2.4.5/tdf_tool/tools/dependencies_analysis.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/env.py` & `tdf_tool-2.4.5/tdf_tool/tools/env.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/fix_header_entry.py` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/fix_header_entry.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/fix_header_lint.py` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/fix_header_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/fix_header_lint_tool.py` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/fix_header_lint_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/fix_header/fix_header_replace_tool.py` & `tdf_tool-2.4.5/tdf_tool/tools/fix_header/fix_header_replace_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/flutter_script.py` & `tdf_tool-2.4.5/tdf_tool/tools/flutter_script.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/gitlab/gitlab_utils.py` & `tdf_tool-2.4.5/tdf_tool/tools/gitlab/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/gitlab/python_gitlab_api.py` & `tdf_tool-2.4.5/tdf_tool/tools/gitlab/python_gitlab_api.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/module/module_tools.py` & `tdf_tool-2.4.5/tdf_tool/tools/module/module_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/package/seal_off_package_utils.py` & `tdf_tool-2.4.5/tdf_tool/tools/package/seal_off_package_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/platform_tools.py` & `tdf_tool-2.4.5/tdf_tool/tools/platform_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/print.py` & `tdf_tool-2.4.5/tdf_tool/tools/print.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/regular_tool.py` & `tdf_tool-2.4.5/tdf_tool/tools/regular_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/shell_dir.py` & `tdf_tool-2.4.5/tdf_tool/tools/shell_dir.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/file_util.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/file_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/flutter_translate_lint.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/flutter_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/flutter_translate_tools.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/flutter_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/ios_translate.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/ios_translate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/ios_translate_lint.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/ios_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/ios_module.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/ios_module.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/location_string_temp.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/location_string_temp.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/podspec.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/podspec.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/ios/tools/string_util.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/ios/tools/string_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/tools/translate_tool.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/tools/translate_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/translate/translate_lint.py` & `tdf_tool-2.4.5/tdf_tool/tools/translate/translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc` & `tdf_tool-2.4.5/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.4/setup.py` & `tdf_tool-2.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'ruamel.yaml>=0.17.21,<0.18.0']
 
 entry_points = \
 {'console_scripts': ['tdf_tool = tdf_tool.app:main', 'tl = tdf_tool.app:main']}
 
 setup_kwargs = {
     'name': 'tdf-tool',
-    'version': '2.4.4',
+    'version': '2.4.5',
     'description': '二维火 flutter 脚手架工具',
     'long_description': '## 帮助文档\n\n```shell\nNAME\n    tdf_tool - 二维火 Flutter 脚手架工具，包含项目构建，依赖分析，git等功能。。\n\nSYNOPSIS\n    tdf_tool GROUP | COMMAND\n\nDESCRIPTION\n    二维火 Flutter 脚手架工具，包含项目构建，依赖分析，git等功能。。\n\nGROUPS\n    GROUP is one of the following:\n\n     module\n       模块相关工具： tdf_tool module -h 查看详情\n\n     package\n       封包工具相关：tdf_tool package -h 查看详情\n\n     translate\n       国际化相关：tdf_tool translate -h 查看详情\n\nCOMMANDS\n    COMMAND is one of the following:\n\n     git\n       tdf_tool git【git 命令】：批量操作 git 命令, 例如 tdf_tool git push\n\n     router\n       tdf_tool router：会以交互式进行路由操作，对指定的模块执行路由生成和路由注册逻辑\n\n     upgrade\n       tdf_tool upgrade：升级插件到最新版本\n        \n```\n\n\n\n## 插件安装方式\n\n安装python包\n\n```\npip3 install tdf-tool --user\n```\n\n安装并更新python包\n\n```\npip3 install --upgrade tdf-tool --user\n```\n\n安装测试环境python包\n\n```\npip3 install -i https://test.pypi.org/simple/ tdf-tool --user\n```\n\n安装并更新测试环境python包\n\n```\npip3 install --upgrade -i https://test.pypi.org/simple/ tdf-tool --user\n```\n\n\n\n## 工具使用流程说明\n\n### 1.准备工作\n\n- 确保python的bin插件目录已经被配置到环境变量中（这一步不满足的话，插件安装之后是无法识别到本插件命令的）\n\n- 在~目录下，创建.tdf_tool_config文件并配置相关必需属性如下\n\n```json\ngit_private_token=***\n```\n\ngit_private_token是gitlab的token\n\n获取途径：进入gitlab页面，点击右上角头像，选择Preferences，选择左侧列表中的AccessToken进行创建\n\n**上述步骤如果没有做，会在使用插件时，会有提示**\n\n### 2.初始化\n\n#### i.进入壳目录（确保执行命令在壳目录内）\n\n#### ii.执行tdf_tool module init\n\n- 判断当前目录是否存在tdf_cache，若不存在，则会自动创建tdf_cache\n- 自动读取当前壳模块名称，写入initial_config.json配置文件；\n- 读取当前壳分支，写入initial_config.json配置文件；\n- 交互式提示用户输入需要开发的模块名并写入initial_config.json配置文件的moduleNameList列表字段中\n- ！退出，即输入完成\n- 自动clone所有开发模块到  ```../.tdf_flutter```  隐藏目录中；\n- 将所有开发模块分支切换至与壳一致；\n- 自动分析依赖树，并**由下至上**对所有模块自动执行```flutter pub upgrade```;\n\n#### iii.开发过程中\n\n##### 1.开发模块添加\n\n- 若是有新模块需要添加入开发模块中，可直接修改initial_config.json配置文件，修改moduleNameList字段；\n- 执行tdf_tool deps更新依赖\n\n##### 2.新开发模块添加\n\n- 添加新模块后，会提示找不到模块，实际查找的是```tdf_cache```文件夹中的module_config.json文件；\n- 如果没有找到该模块，则可以执行```tdf_tool module-update```,更新远程module_config.json文件；\n- 删掉本地的module_config.json文件，重新执行命令即可，脚本会自动判断本地是否存在该配置文件，如果不存在会**下载**；\n\n<span style="color:#ff0000">请确保gitlab仓库的新开发模块master分支是一个flutter模块，如果判定不是flutter模块，则会报错（判定条件为存在pubspec.yaml文件）</span>\n\n\n\n### 3.版本控制\n\n版本控制请使用tdf_tool命令，命令详情可使用  ```tdf_tool -h```  查看，现已支持大部分命令，若有特殊命令需要执行，可以使用  ```tdf_tool <git命令>``` ，如：```tdf_tool git add .```\n\n\n\n### 4.自动打包发布\n\n暂未接入打包工具，预计下一季度进行支持；\n\n\n\n**<span style="color:#ff0000">FAQ</span>**\n\nwindows系统请使用bash命令；\n\n\n\n## 额外功能说明\n\n### 1.二维数组表达依赖树\n\n生成一个二维数组，可根据该二维数组的数据进行**并发**打tag，每一层的模块，都可以同时进行打tag发布操作，减少发布耗时；\n\n```json\n[\n\t["tdf_channel", "tdf_event", "tdf_network"], \n\t["tdf_widgets"], \n\t["tdf_smart_devices", "tdf_account_module"], \n\t["flutter_reset_module"]\n]\n```\n\n如上数据，数组中每一个节点中的模块均可同时打tag，节点之间需要由上至下的顺序进行tag操作\n\n\n\n### 2.插件更新\n\n执行 ```tdf_tool upgrade```\n\n\n\n### 3.远程模块配置文件更新\n\n执行 ```tdf_tool module module_update```\n\n\n\n## 依赖树分析原理\n\n采用有向有/无环图进行依赖树的分析\n\n数据结构采用如下：\n\n```python\nclass DependencyNode:\n    def __init__(self):\n        self.nodeName = \'\'\n        self.parent = []  # 父亲节点列表\n        self.children = []  # 子孙节点列表\n        self.delete = False\n```\n\n![dependency](./README_DIR/dependency.png)\n\n如上图1：一个正常的依赖树表示；\n\n如上图2：对图1中，依赖树所有节点去重，变换为图2有向图；\t\n\n\n\n**分析流程：**\n\n**依赖图构建**\n\n```python\n# 生成依赖图\n    def _generateDependenciesMap(self):\n        for package in self.__moduleDependenciesMap:\n            for module in moduleNameList:\n                if package == module:\n                    # 到这一步表明当前这个模块属于开发模块且在当前模块的依赖模块列表中，是当前模块的子模块\n                    self._mNodeDict[self.__moduleName].children.append(package)\n                    self._mNodeDict[package].parent.append(self.__moduleName)\n```\n\n- 共5个节点\n\n  - node构建：\n\n    - ```python\n      {\n      \t"模块1":{\n          "nodeNmae": "模块1",\n          "parent": [],\n          "children": ["模块2","模块3","模块4","模块5"],\n          "delete": False\n      \t},\n      \t"模块2":{\n          "nodeNmae": "模块2",\n          "parent": ["模块1"],\n          "children": ["模块4","模块5"],\n          "delete": False\n      \t}\n      \t"模块3":{\n          "nodeNmae": "模块3",\n          "parent": ["模块1"],\n          "children": ["模块5"],\n          "delete": False\n      \t}\n      \t"模块4":{\n          "nodeNmae": "模块4",\n          "parent": ["模块1","模块2"],\n          "children": [],\n          "delete": False\n      \t}\n      \t"模块5":{\n          "nodeNmae": "模块5",\n          "parent": ["模块1","模块2","模块3"],\n          "children": [],\n          "delete": False\n      \t}\n      }\n      ```\n\n**依赖图解析伪代码（以一维数组为例）**\n\n```python\n# 返回二维数组，用于并发打tag\n    def _generateDependenciesOrder(self):\n        resList = []\n        while 存在节点delete属性不为True:\n            \n            for：查找子节点为0的节点\n            \t设置节点delete属性为True\n              \n            for：deleteItemList = 拿到所有delete属性为true的节点\n\n            for：遍历所有节点，如果节点的子节点中包含deleteItemList的节点，则将其从子节点列表中删除\n```\n\n\n\n\n\n- **initial_config.json文件说明**\n\n  ```json\n  {\n      "featureBranch": "feature/test_dev_1", // 开发分支\n      "shellName": "flutter_reset_module",\n      // 项目需要开发的模块,可自由配置\n      "moduleNameList": [\n          "flutter_reset_module",\n          "tdf_smart_devices",\n          "tdf_widgets",\n          "tdf_channel"\n      ]\n  }\n  ```\n\n- **module_config.json文件说明**\n\n  ```json\n  {\n      "flutter_globalyun_us_module": {\n        \t"id": "11111"\n          "type": "shell",\n          "git": "git@git.2dfire.net:app/flutter/app/flutter_globalyun_us_module.git"\n      },\n      "tdf_router_anno": {\n          "type": "base",\n          "git": "git@git.2dfire.net:app/flutter/app/tdf_router_anno.git"\n      },\n  }\n  //语意\n  {\n    "模块名":{\n      "id": 项目gitlab id\n      "类型": gitlab group名\n      "git": gitlab地址\n    }\n  }\n  ```\n\n\n\n## 后续计划\n\n<span style="color:#ff0000">**问题：**</span>由于现在flutter ci 【lint】【tag】任务脚本成功率过于低，很多时候是因为项目模块的配置问题导致的，且后续会接入一键打tag工具\n\n方案：在执行统一push前，对所有模块的项目配置信息进行校验，确保数据规范；\n\n\n\n## 插件打包发布命令\n\n**插件打包命令**\n\n```\npoetry build\n```\n**插件发布命令**\n\n```\npoetry publish\n```\n\n## History\n\n### 2.1.00\n\n- 路由功能支持flutter版本3.3.10，兼容flutter版本2.2.3；\n\n### 2.0.61\n\n- Flutter国际化字符串整合；\n\n### 2.0.38\n\n- 路由生成完后增加路由相关代码format（解决windows代码生成后顺序错乱）；\n\n### 2.0.01\n\n- Cli 框架升级；\n- 代码重构；\n\n### **1.1.00（2022-4-28）**\n\n- 国际化解决输出json中包含转义字符的问题，如\\n；\n- 四类语言输出文件自动格式化\n\n### **1.0.55（2022-4-28）**\n\n- 国际化key使用中文（依照ios项目开发形式）；\n\n### **1.0.53（2022-4-28）**\n\n- 国际化流程中，兼容解决部分json解析失败问题，譬如字符串中包含"="符号；\n\n> 错误日志如：Unterminated string starting at: line 1 column 5650 (char 5649)\n\n### **1.0.50（2022-4-28）**\n\n- 国际化增加繁体字翻译；\n\n',
     'author': 'Jian Xu',
     'author_email': '3386218996@qq.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://git.2dfire.net/app/flutter/tools/package_tools',
```

### Comparing `tdf_tool-2.4.4/PKG-INFO` & `tdf_tool-2.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdf-tool
-Version: 2.4.4
+Version: 2.4.5
 Summary: 二维火 flutter 脚手架工具
 Home-page: https://git.2dfire.net/app/flutter/tools/package_tools
 License: MIT
 Keywords: tdf,tdf-tool,tdf_tool
 Author: Jian Xu
 Author-email: 3386218996@qq.com
 Requires-Python: >=3.9.0,<4.0.0
```

