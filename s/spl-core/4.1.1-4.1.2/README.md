# Comparing `tmp/spl_core-4.1.1.tar.gz` & `tmp/spl_core-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_core-4.1.1.tar", max compression
+gzip compressed data, was "spl_core-4.1.2.tar", max compression
```

## Comparing `spl_core-4.1.1.tar` & `spl_core-4.1.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1099 2024-04-17 08:36:46.128766 spl_core-4.1.1/LICENSE
--rw-r--r--   0        0        0      824 2024-04-17 08:36:46.128766 spl_core-4.1.1/README.md
--rw-r--r--   0        0        0     4335 2024-04-17 08:36:47.064766 spl_core-4.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-17 08:36:47.064766 spl_core-4.1.1/src/spl_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/common/__init__.py
--rw-r--r--   0        0        0     2054 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/common/cmake.py
--rw-r--r--   0        0        0     2019 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/common/command_line_executor.py
--rw-r--r--   0        0        0      462 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/common/path.py
--rw-r--r--   0        0        0        0 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/gcov_maid/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/gcov_maid/gcov_maid.py
--rw-r--r--   0        0        0        0 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/kconfig/__init__.py
--rw-r--r--   0        0        0     9795 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/kconfig/kconfig.py
--rw-r--r--   0        0        0        0 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/__init__.py
--rw-r--r--   0        0        0     7342 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/creator.py
--rw-r--r--   0        0        0      239 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/cookiecutter.json
--rw-r--r--   0        0        0       33 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.flake8
--rw-r--r--   0        0        0      599 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.gitignore
--rw-r--r--   0        0        0      269 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-kits.json
--rw-r--r--   0        0        0      718 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-variants.json
--rw-r--r--   0        0        0      626 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json
--rw-r--r--   0        0        0     1103 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json
--rw-r--r--   0        0        0     1369 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json
--rw-r--r--   0        0        0     2853 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json
--rw-r--r--   0        0        0     1400 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt
--rw-r--r--   0        0        0      598 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig
--rw-r--r--   0        0        0     1108 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE
--rw-r--r--   0        0        0      513 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/Pipfile
--rw-r--r--   0        0        0      337 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/README.md
--rw-r--r--   0        0        0       73 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.bat
--rw-r--r--   0        0        0    10528 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1
--rw-r--r--   0        0        0     6705 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py
--rw-r--r--   0        0        0   123927 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in
--rw-r--r--   0        0        0       90 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/common/index.rst
--rw-r--r--   0        0        0      594 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst
--rw-r--r--   0        0        0     1072 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/LICENSE
--rw-r--r--   0        0        0    63071 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css
--rw-r--r--   0        0        0       44 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_architecture/index.rst
--rw-r--r--   0        0        0       95 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_requirements/index.rst
--rw-r--r--   0        0        0     1217 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt
--rw-r--r--   0        0        0     1021 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst
--rw-r--r--   0        0        0       46 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/install-mandatory.bat
--rw-r--r--   0        0        0      127 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/pytest.ini
--rw-r--r--   0        0        0     1077 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/scoopfile.json
--rw-r--r--   0        0        0     1518 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_build.py
--rw-r--r--   0        0        0      941 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_unittests.py
--rw-r--r--   0        0        0      617 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/utils.py
--rw-r--r--   0        0        0      348 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/tools/setup/git-config.ps1
--rw-r--r--   0        0        0      123 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/CMakeLists.txt
--rw-r--r--   0        0        0     7588 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/_images/screenshot.png
--rw-r--r--   0        0        0      477 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/design.rst
--rw-r--r--   0        0        0      135 2024-04-17 08:36:46.132766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/index.rst
--rw-r--r--   0        0        0      433 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.c
--rw-r--r--   0        0        0       40 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.h
--rw-r--r--   0        0        0     1048 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/test/test_component.cc
--rw-r--r--   0        0        0       68 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/CMakeLists.txt
--rw-r--r--   0        0        0      311 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/doc/index.rst
--rw-r--r--   0        0        0      272 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/src/main.c
--rw-r--r--   0        0        0      714 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake
--rw-r--r--   0        0        0      183 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/gcc/toolchain.cmake
--rw-r--r--   0        0        0       57 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/variant/cookiecutter.json
--rw-r--r--   0        0        0       94 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.cmake
--rw-r--r--   0        0        0       24 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.txt
--rw-r--r--   0        0        0       77 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/parts.cmake
--rw-r--r--   0        0        0      532 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/variant.py
--rw-r--r--   0        0        0     1279 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/project_creator/workspace_artifacts.py
--rw-r--r--   0        0        0     2665 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/test_utils/base_variant_test_runner.py
--rw-r--r--   0        0        0     2172 2024-04-17 08:36:46.136766 spl_core-4.1.1/src/spl_core/test_utils/spl_build.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 spl_core-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-18 13:58:45.985234 spl_core-4.1.2/LICENSE
+-rw-r--r--   0        0        0      824 2024-04-18 13:58:45.985234 spl_core-4.1.2/README.md
+-rw-r--r--   0        0        0     4335 2024-04-18 13:58:47.185249 spl_core-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-18 13:58:47.185249 spl_core-4.1.2/src/spl_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/common/__init__.py
+-rw-r--r--   0        0        0     2054 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/common/cmake.py
+-rw-r--r--   0        0        0     2019 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/common/command_line_executor.py
+-rw-r--r--   0        0        0      462 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/common/path.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/gcov_maid/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/gcov_maid/gcov_maid.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/kconfig/__init__.py
+-rw-r--r--   0        0        0     9795 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/kconfig/kconfig.py
+-rw-r--r--   0        0        0        0 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/__init__.py
+-rw-r--r--   0        0        0     7342 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/creator.py
+-rw-r--r--   0        0        0      239 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/cookiecutter.json
+-rw-r--r--   0        0        0       33 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.flake8
+-rw-r--r--   0        0        0      599 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.gitignore
+-rw-r--r--   0        0        0      269 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-kits.json
+-rw-r--r--   0        0        0      718 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-variants.json
+-rw-r--r--   0        0        0      626 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json
+-rw-r--r--   0        0        0     1103 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json
+-rw-r--r--   0        0        0     1369 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json
+-rw-r--r--   0        0        0     2853 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json
+-rw-r--r--   0        0        0     1400 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt
+-rw-r--r--   0        0        0      598 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig
+-rw-r--r--   0        0        0     1108 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE
+-rw-r--r--   0        0        0      513 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/Pipfile
+-rw-r--r--   0        0        0      337 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/README.md
+-rw-r--r--   0        0        0       73 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.bat
+-rw-r--r--   0        0        0    10528 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1
+-rw-r--r--   0        0        0     6705 2024-04-18 13:58:45.989234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py
+-rw-r--r--   0        0        0   123927 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in
+-rw-r--r--   0        0        0       90 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/common/index.rst
+-rw-r--r--   0        0        0      594 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst
+-rw-r--r--   0        0        0     1072 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/LICENSE
+-rw-r--r--   0        0        0    63071 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css
+-rw-r--r--   0        0        0       44 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_architecture/index.rst
+-rw-r--r--   0        0        0       95 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_requirements/index.rst
+-rw-r--r--   0        0        0     1217 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt
+-rw-r--r--   0        0        0     1021 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst
+-rw-r--r--   0        0        0       46 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/install-mandatory.bat
+-rw-r--r--   0        0        0      127 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/pytest.ini
+-rw-r--r--   0        0        0     1077 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/scoopfile.json
+-rw-r--r--   0        0        0     1518 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_build.py
+-rw-r--r--   0        0        0      941 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_unittests.py
+-rw-r--r--   0        0        0      617 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/utils.py
+-rw-r--r--   0        0        0      348 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/tools/setup/git-config.ps1
+-rw-r--r--   0        0        0      123 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/CMakeLists.txt
+-rw-r--r--   0        0        0     7588 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/_images/screenshot.png
+-rw-r--r--   0        0        0      477 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/design.rst
+-rw-r--r--   0        0        0      135 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/index.rst
+-rw-r--r--   0        0        0      433 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.c
+-rw-r--r--   0        0        0       40 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.h
+-rw-r--r--   0        0        0     1048 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/test/test_component.cc
+-rw-r--r--   0        0        0       68 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/CMakeLists.txt
+-rw-r--r--   0        0        0      311 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/doc/index.rst
+-rw-r--r--   0        0        0      272 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/src/main.c
+-rw-r--r--   0        0        0      714 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake
+-rw-r--r--   0        0        0      183 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/gcc/toolchain.cmake
+-rw-r--r--   0        0        0       57 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/variant/cookiecutter.json
+-rw-r--r--   0        0        0       94 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.cmake
+-rw-r--r--   0        0        0       24 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.txt
+-rw-r--r--   0        0        0       77 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/parts.cmake
+-rw-r--r--   0        0        0      532 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/variant.py
+-rw-r--r--   0        0        0     1279 2024-04-18 13:58:45.993234 spl_core-4.1.2/src/spl_core/project_creator/workspace_artifacts.py
+-rw-r--r--   0        0        0     3221 2024-04-18 13:58:45.997234 spl_core-4.1.2/src/spl_core/test_utils/base_variant_test_runner.py
+-rw-r--r--   0        0        0     5599 2024-04-18 13:58:45.997234 spl_core-4.1.2/src/spl_core/test_utils/spl_build.py
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 spl_core-4.1.2/PKG-INFO
```

### Comparing `spl_core-4.1.1/LICENSE` & `spl_core-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/README.md` & `spl_core-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/pyproject.toml` & `spl_core-4.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spl-core"
-version = "4.1.1"
+version = "4.1.2"
 description = "Software Product Line Support for CMake"
 authors = ["Avengineers <karsten.guenther@kamg.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/avengineers/spl-core"
 documentation = "https://spl-core.readthedocs.io"
 classifiers = [
```

### Comparing `spl_core-4.1.1/src/spl_core/common/cmake.py` & `spl_core-4.1.2/src/spl_core/common/cmake.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/common/command_line_executor.py` & `spl_core-4.1.2/src/spl_core/common/command_line_executor.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/gcov_maid/gcov_maid.py` & `spl_core-4.1.2/src/spl_core/gcov_maid/gcov_maid.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/kconfig/kconfig.py` & `spl_core-4.1.2/src/spl_core/kconfig/kconfig.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/creator.py` & `spl_core-4.1.2/src/spl_core/project_creator/creator.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.gitignore` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-variants.json` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-variants.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/Pipfile` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/Pipfile`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/LICENSE` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/scoopfile.json` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/scoopfile.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_build.py` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_build.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_unittests.py` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_unittests.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/utils.py` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/utils.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/_images/screenshot.png` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/_images/screenshot.png`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/test/test_component.cc` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/test/test_component.cc`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake` & `spl_core-4.1.2/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/variant.py` & `spl_core-4.1.2/src/spl_core/project_creator/variant.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/project_creator/workspace_artifacts.py` & `spl_core-4.1.2/src/spl_core/project_creator/workspace_artifacts.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.1.1/src/spl_core/test_utils/base_variant_test_runner.py` & `spl_core-4.1.2/src/spl_core/test_utils/base_variant_test_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,25 +35,42 @@
             Path("coverage.html"),
             Path("unit_test_results.html"),
             Path("unit_test_spec.html"),
             Path("doxygen/html/index.html"),
             Path("coverage/index.html"),
         ]
 
+    @property
+    def create_artifacts_archive(self) -> bool:
+        return True
+
+    @property
+    def create_artifacts_json(self) -> bool:
+        return True
+
+    @property
+    def expected_archive_artifacts(self) -> List[Path]:
+        return self.expected_build_artifacts
+
     def assert_artifact_exists(self, dir: Path, artifact: Path) -> None:
         if artifact.is_absolute():
             assert artifact.exists(), f"Artifact {artifact} does not exist"  # noqa: S101
         else:
             assert Path.joinpath(dir, artifact).exists(), f"Artifact {Path.joinpath(dir, artifact)} does not exist"  # noqa: S101
 
     def test_build(self) -> None:
         spl_build: SplBuild = SplBuild(variant=self.variant, build_kit="prod")
         assert 0 == spl_build.execute(target="all")  # noqa: S101
         for artifact in self.expected_build_artifacts:
             self.assert_artifact_exists(dir=spl_build.build_dir, artifact=artifact)
+        if self.create_artifacts_archive:
+            # create artifacts archive
+            spl_build.create_artifacts_archive(self.expected_archive_artifacts)
+        if self.create_artifacts_json:
+            spl_build.create_artifacts_json(self.expected_archive_artifacts)
 
     def test_unittest(self) -> None:
         spl_build: SplBuild = SplBuild(variant=self.variant, build_kit="test")
         assert 0 == spl_build.execute(target="unittests")  # noqa: S101
         for artifact in self.expected_test_artifacts:
             self.assert_artifact_exists(dir=spl_build.build_dir, artifact=artifact)
```

### Comparing `spl_core-4.1.1/PKG-INFO` & `spl_core-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spl-core
-Version: 4.1.1
+Version: 4.1.2
 Summary: Software Product Line Support for CMake
 Home-page: https://github.com/avengineers/spl-core
 License: MIT
 Author: Avengineers
 Author-email: karsten.guenther@kamg.de
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

